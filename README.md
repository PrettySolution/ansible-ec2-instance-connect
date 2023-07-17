1. install asdf https://asdf-vm.com/guide/getting-started.html
2. `git clone https://github.com/PrettySolution/ansible-ec2-instance-connect.git && cd ansible-ec2-instance-connect`
3. `asdf install`
2. `python3 -m venv venv && source venv/bin/activate`
2. `pip install ansible boto3`
3. `ansible-galaxy collection install amazon.aws`
```shell
export AWS_ACCESS_KEY_ID="AWS_ACCESS_KEY_ID"
export AWS_SECRET_ACCESS_KEY="AWS_SECRET_ACCESS_KEY"
export AWS_SESSION_TOKEN="TOKEN"
export AWS_REGION="us-east-1"
```
3. `ansible all -i inventory -m ping -u ubuntu`
4. `ansible all -i aws_ec2.yml -m ping -u ubuntu`