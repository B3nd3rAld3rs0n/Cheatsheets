# Bash Cheatsheet

## Special Arguments

<table style="text-align:center">
    <tr>
        <th>Argument</th>
        <th>Explanation</th>
    </tr>
    <tr>
        <td>
            $#
        </td>
        <td>
            Number of arguments
        </td>
    </tr>
    <tr>
        <td>
            $*
        </td>
        <td>
            All arguments
        </td>
    </tr>
    <tr>
        </tr>
        <td>
            $@
        </td>
        <td>
            All arguments, starting from first
        </td>
    </tr>
    <tr>
        </tr>
        <td>
            $1
        </td>
        <td>
            First argument
        </td>
    </tr>
    <tr>
        </tr>
        <td>
            $_
        </td>
        <td>
            Last argument of previous command
        </td>
    </tr>
</table>

See: [Bash Hackers Wiki](https://wiki.bash-hackers.org/syntax/shellvars#special_parameters_and_shell_variables)

## Special Characters

<table style="text-align:center">
    <tr>
        <th>Character</th>
        <th>Explanation</th>
    </tr>
    <tr>
        <td>
            " "
        </td>
        <td>
            Whitespace
        </td>
    </tr>
    <tr>
        <td>
            $var, ${var}
        </td>
        <td>
            Variable expansion
        </td>
    </tr>
    <tr>
        <td>
            $(cmd)
        </td>
        <td>
            Command substitution, returns command output
        </td>
    </tr>
    <tr>
        <td>
            $((expression))
        </td>
        <td>
            Arithmetic expansion
        </td>
    </tr>
    <tr>
        <td>
            ''
        </td>
        <td>
            Literal string, special chars are ignored
        </td>
    </tr>
    <tr>
        </tr>
        <td>
            ""
        </td>
        <td>
            String, special chars are evaluated
        </td>
    </tr>
    <tr>
        <td>
            \
        </td>
        <td>
            Escape special chars
        </td>
    </tr>
    <tr>
        <td>
            #
        </td>
        <td>
            Comment
        </td>
    </tr>
    <tr>
        <td>
            =
        </td>
        <td>
            Variable Assignment
        </td>
    </tr>
    <tr>
        <td>
            [[ ]]
        </td>
        <td>
            Evaluate conditional expression
        </td>
    </tr>
    <tr>
        <td>
            !
        </td>
        <td>
            Negate test or exit status
        </td>
    </tr>
    <tr>
        <td>
            >, >>, <
        </td>
        <td>
            Redirection
        </td>
    </tr>
    <tr>
        <td>
            |
        </td>
        <td>
            Pipe output to another command
        </td>
    </tr>
    <tr>
        <td>
            ;
        </td>
        <td>
            Command separator
        </td>
    </tr>
    <tr>
        <td>
            { }
        </td>
        <td>
            Inline group, commands inside are treated as one command
        </td>
    </tr>
    <tr>
        <td>
            ( )
        </td>
        <td>
            Subshell group, commands are executed in a new process
        </td>
    </tr>
    <tr>
        <td>
            (( ))
        </td>
        <td>
            Arithmetic expression, returns result
        </td>
    </tr>
    <tr>
        <td>
            *, ?
        </td>
        <td>
            Globs, wildcard matches
        </td>
    </tr>
    <tr>
        <td>
            ~
        </td>
        <td>
            Home directory
        </td>
    </tr>
    <tr>
        <td>
            &
        </td>
        <td>
            Background command
        </td>
    </tr>
</table>

See: [Bash Guide](http://mywiki.wooledge.org/BashGuide/SpecialCharacters)

## Loops

<table>
    <tr>
        <th>Loop</th>
        <th>Multi-Line</th>
        <th>One-Liner</th>
    </tr>
    <tr>
        <td>For</td>
        <td>
            <pre lang="bash">
for i in list; do
    cmd
done
            </pre>
        </td>
        <td>
            <pre lang="bash" style="text-align:center">
for i in list; do cmd; done
            </pre>
        </td>
    </tr>
    <tr>
        <td>If-Else</td>
        <td>
            <pre lang="bash">
if [ condition ]; do
    cmd
elif [condition ]; do
    cmd
else cmd
fi
            </pre>
        </td>
        <td>
            <pre lang="bash" style="text-align:center">
if [ condition ]; do cmd; else cmd; fi
            </pre>
        </td>
    </tr>
    <tr>
        <td>While</td>
        <td>
            <pre lang="bash">
while [ condition ]; do
    cmd
done
            </pre>
        </td>
        <td>
            <pre lang="bash" style="text-align:center">
while [ condition ]; do cmd; done
            </pre>
        </td>
    </tr>
</table>

## Text Manipulation

<table>
    <tr>
        <th>Command</th>
        <th>Explanation</th>
        <th>Usage</th>
    </tr>
    <tr>
        <td style="text-align:center">Sed</td>
        <td style="text-align:center">Stream Editor - transform text</td>
        <td>
            <pre lang="bash" style="text-align:center">
sed -i "s/to replace/replacement/g"
            </pre>
        </td>
    </tr>
    <tr>
        <td style="text-align:center">Cut</td>
        <td style="text-align:center">Cut fields using delimiter</td>
        <td>
            <pre lang="bash" style="text-align:center">
cut -d "&ltdelimiter&gt" -f "&ltfield # to cut&GT"
            </pre>
        </td>
    </tr>
</table>

## Colorization/Formatting

See: [Bash tips: Colors and formatting](https://misc.flogisoft.com/bash/tip_colors_and_formatting)

## Resources

[]()
[]()
