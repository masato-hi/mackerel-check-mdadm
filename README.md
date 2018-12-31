# mackerel-check-mdadm
Add mdadm check result to mackerel.

## Installation
#### Place check-mdadm and make it executable.
```
curl -o /usr/local/bin/check-mdadm https://raw.githubusercontent.com/masato-hi/mackerel-check-mdadm/master/check-mdadm
chmod +x /usr/local/bin/check-mdadm
```

#### Please add the following contents to /etc/mackerel-agent/mackerel-agent.conf
```
[plugin.checks.mdadm]
command = "check-mdadm"
```

#### Please reload mackerel-agent.
```
service mackerel-agent reload
```


## Contributing

Bug reports and pull requests are welcome on GitHub at https://github.com/masato-hi/mackerel-check-mdadm.


## License

The script is available as open source under the terms of the [MIT License](http://opensource.org/licenses/MIT).

