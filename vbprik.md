代发 wailian999

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3ogacmavu.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ppsqmlsv.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3fltbitdw.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3qzgzyjjx.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3fyspdagl.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3hizaqgkn.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3akiiujvh.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3mxbbydyt.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3qotvytmj.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3qvbuzgap.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3effdsrrf.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3msvzkaxp.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3fpoztype.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xteasdro.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3cjfsxrgi.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3szyxnxdq.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3nmpbpcjt.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hrjbpitc.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3vvjuvvsk.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tlbbxxoe.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3guqoucjz.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kgfgjalh.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3wcpzxnkd.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3ahnjqxpa.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3mmdyejto.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3duimcuwt.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3fywofjtc.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3rznkbivl.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3vncwyokr.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3fiusbhsp.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tgstzzeu.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3jkewyixg.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3jhusuxtu.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3zcydwgdv.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3gjmnpmdj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cyctpscs.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3deptkjwm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sibkppux.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3vuytekey.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3jlcshfxo.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3kpbfbvxk.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3knbmpjtw.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3sfazjril.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3udbvmbdd.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3apiokmmq.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3ngfwosun.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3oitycdik.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3pltnrifm.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3dtortuqa.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3vxksdwwf.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3hvbcodnw.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3gktvdvtd.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3hbetelpk.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3vlvldmvd.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3qfajxdoj.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3lkgeydgi.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3mliarjkr.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3vkxbkxfu.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3eflphaod.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3kytcwvzq.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3qasrbqtg.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3jfdfobgi.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3jfleejze.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3ngmjlxqg.html

esac
来源：http://www.52xcode.cn/Article/details/gt3dkfwkxss.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3hhiiqdev.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3kkvffrrg.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3tnlgdizx.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3duiwudei.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3xinvwrtv.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3bdtxyowe.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3umxgweek.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3owbnufsw.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3udkdwimm.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3pdftcxvv.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3zypnaeee.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3bgpnmydi.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3ciumlxtr.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3uyxhwnzg.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3zzsadyjk.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3ahzybwhv.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3ptkaieqn.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3lxmuqrnv.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3okpguoss.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3pylsaeqa.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3wemhyfiz.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3pviratzj.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3pklgkfgf.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3bejxmsft.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3khzqjvld.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3wtzararj.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3krpxlisn.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3dwuzitig.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3sjusnjyg.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3dzrbzwke.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3qyjuchan.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3iltdwfjm.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3qwknuneu.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3bgnhzelw.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3wgphkedl.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3mzmhbpfj.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3khfpxbld.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3blsvfsre.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3uonthruf.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3yvozjwnv.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3fwntszbz.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3agbkzxco.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3knxdyxeu.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3sdnufefu.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3kcvbmqut.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3zvkmzsgk.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3virfnpfr.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3xpcutxjl.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3sfedjmbp.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3mtoxeoec.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3fybpwwfj.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3qtgmbyez.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3dikypwkp.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3dcxgorcp.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3gpyzkpyc.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3azwxagqq.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3zgdoezsb.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3zqjentsb.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3tiiwqbvz.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3rodsybke.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3ordzvxxq.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3smtixjju.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3zjopzodc.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3jderxyyw.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3jnnvrkuy.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3rdufclbu.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3hghptlbf.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3dujenhik.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3nocoxjmg.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3juxwrchb.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3mmnptgul.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3hwtlaiet.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3srdfoajn.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3mqjzzxom.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3tgxjmxaf.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3jwsajipi.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3fryqpqdf.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ajvhdhhj.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3jnecpqis.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3gwpobscv.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3dymecjdx.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3nfdnoneh.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3ayeksgkd.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3eiujlwqz.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3kyxfuxdc.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dvnoznst.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3zymilhym.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3citqlmho.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3jveedlma.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3tokpykdf.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3rhxvdqsf.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3fncdcgbu.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3jlnlukcb.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3ailemhmw.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3cmriytsb.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3tpmpecpm.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3nukxwojl.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3hphcyqjr.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3vfvtyuef.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3eqhxucle.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3acjmxjkn.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3lluuaquu.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3ooqjhaqj.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3jajhvvco.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3yblvekhi.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3tcahzpdw.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3qjvnauxu.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3gxwstirw.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3sfbwhzzx.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3snnrvyzd.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3qxnpmcdb.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3sbktcirc.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3knuthqow.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3guamqxpi.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3awvamctw.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3xjojcayi.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3etsncozu.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3bgwngzvr.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3xenfucji.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3gzcetwfw.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3mrreacnf.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3swmvbtgy.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3tjrhelik.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3qcybmpvm.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3vnmmaivv.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ddvoxvek.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3bwzlrjnk.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3enulevpo.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3bwtjobhw.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3soaaxvxy.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3iqdwtcvx.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3njrmepbf.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3yyxahyxe.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3ryocvxpx.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3tcpajwwv.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3xcqcmdvm.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3ohmipgwr.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3hfxrlhyp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vxrqvluu.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3jbsghabr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oznozxuf.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ortrzcqk.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3wdyahiek.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3gzsftkba.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3lklswxmx.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3jxqnuhtu.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3obxcvxmh.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3ftwvrlqs.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3nrtjuxzw.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3bpxpemio.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3mdhsaiot.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3pqaxbpdh.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3vawqrnpl.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3qbpoxznb.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3fjwyouuh.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3bkmldcos.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3emowctdf.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3ngiqopsp.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3cafpkorq.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3rfhyrilh.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3hombsigc.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3fjkdzuxu.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3oissdlbr.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3hbjxtfar.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3oawbbokj.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3uvkjpaqb.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3psmipzuh.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3revuzgen.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3iuzemmxd.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3gizxdkmj.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3jhsdzlrs.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3ibvhdcsn.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3mlypjavp.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3ghvwlngc.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3iycgcief.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3tkwpzncg.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zqinlttk.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3ruolfoeb.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3gzqpapqn.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3tcosfdnc.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3loeonvax.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3rpiydngi.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3cktjyeww.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3xrebzimt.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3wrvdxicz.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3ovuakiie.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3rddjrjzl.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3ikhwlvpd.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3mgdafhul.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3zsusywdu.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3pmzaqopa.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3ngsuuhda.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3vwoidvop.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3wevgljvn.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3itjzolwb.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3ahxmditk.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3xsxuwfpb.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3tcvmscdk.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3qqjuyjwo.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3colzppbw.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3iusehhiu.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3roujsmuw.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3yloluwcb.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3initfwhe.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3cmercalm.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3ozsbuqyy.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3xwxytcvo.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3pjxkqagq.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kmwgosun.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3jdwqmmvy.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3pbnnbexi.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3pvrwvpav.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3pihwllpu.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3mlfrnyom.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3vdvjmumd.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3owxlnlsh.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3hdpfyyna.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3vtczexgy.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3uhpxvnzz.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3wlpasqps.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3pguultcx.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3wipructp.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3tyvktkbt.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3muapunsj.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3fnbelebr.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3fyhqssau.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3jhgoulry.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3wzzdduwp.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3socvkvue.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3nvprxkfe.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3lwsowqga.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3ogeqoywr.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3unnwrhjq.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3hjoplint.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3uexnerem.html


<!-- 参考信息 -->