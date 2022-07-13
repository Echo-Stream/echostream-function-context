# echostream-function-context

Micro library for typing function contexts in EchoStream functions
 
## Installation

### For production
```shell
pip install echostream-function-context
```

Production install has no requirements.

### For development
```shell
pip install echostream-function-context[dev]
```

Development install will also install `boto3-stubs[dynamodb]`.

## Usage
```python
def processor(*, context, message, source, **kwargs):

    from typing import cast

    from echostream_function_context import Context

    context = cast(Context, context)
```