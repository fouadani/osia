
ID Usage
--------

Services
""""""""

.. py:function:: verifyIdentity(UIN, [IDAttribute])
    :noindex:

    Verify Identity based on UIN and set of Identity Attributes (biometric data, credential, etc.)

    **Authorization**: :todo:`To be defined`

    :param str UIN: The person's UIN
    :param list[str] IDAttribute: A list of list of pair (name,value) requested
    :return: Y or N
    
    In case of error (unknown attributes, unauthorized access, etc.) the value is replaced with an error

.. py:function:: identify([inIDAttribute], [outIDAttribute])
    :noindex:

    Identify a person based on a set of Identity Attributes (biometric data, credential, etc.)

    **Authorization**: :todo:`To be defined`

    :param list[str] inIDAttribute: A list of list of pair (name,value) requested
    :param list[str] outIDAttribute: A list of list of attribute names requested
    :return: Y or N
    
    In case of error (unknown attributes, unauthorized access, etc.) the value is replaced with an error

.. py:function:: readAttributes(UIN, names)
    :noindex:

    Read person attributes.

    **Authorization**: :todo:`To be defined`

    :param str UIN: The person's UIN
    :param list[str] names: The names of the attributes requested
    :return: a list of pair (name,value). In case of error (unknown attributes, unauthorized access, etc.)
        the value is replaced with an error

.. py:function:: readAttributeSet(UIN, setName)
    :noindex:

    Read person attributes corresponding to a predefined set name.

    **Authorization**: :todo:`To be defined`

    :param str UIN: The person's UIN
    :param str setName: The name of predefined attributes set name
    :return: a list of pair (name,value). In case of error (unknown attributes, unauthorized access, etc.)
        the value is replaced with an error

