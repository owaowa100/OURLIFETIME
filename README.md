import React, { Component } from 'react';
import {
    View,
    Text,
} from 'react-native';

export default class CountUp extends Component  {

    state = {
        seconds: null,
    }

    get formatedTime() {
        const { seconds } = this.state;

        return [
            pad(parseInt(seconds / 60)),
            pad(seconds % 60),
        ].join(':');
    }

    componentWillMount() {
        this.setState({ seconds: 0 });
    }

    componentDidMount() {
        this.timer = setInterval(
            () => this.setState({
                seconds: ++this.state.seconds
            }),
            1000
        );
    }

    componentWillUnmount() {
        clearInterval(this.timer);
    }

    render() {
        return (
            <View>
                <Text>{this.formatedTime}</Text>
            </View>
        );
    }
}

function pad(num) {
    return num.toString().length > 1 ? num : `0${num}`;
}
