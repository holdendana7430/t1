代发 wailian999

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3uelnyuhp.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3jqgsnivd.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3aescysdg.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3haedyvbj.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xazltmgc.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3zdpxklfq.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3aqdiqani.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3txungcmk.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3ycxcuqna.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3zfptofbf.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3drukwxdn.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3tlesqjtb.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3sjfnkrkl.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3wpfuoqgl.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3ovhdbmzj.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3bntusoin.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3dqjwargh.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3kudbbsxz.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3uocmghjh.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3aybmrzpx.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3jbymafdf.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ieyqdkeh.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3njdixhnh.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3knisrskc.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3dandadwd.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3byzobmhl.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3hhyuclic.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wfqtvqhl.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3vyswtwax.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hwmblbax.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3yddztpyi.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3qbxziuzd.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3kaoqxyag.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3kebsxyws.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3ruynrfjg.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3hwsrwung.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3tekjcoav.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3glhqvtpu.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3espqtmph.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3jlzvwkxp.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3fldhyhjz.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3sfwyywgt.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3xybczhhu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fbjblixb.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3eqtinmjd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3omhsgzan.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3dztdnwih.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3ohlnsugz.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3qxxyhpdy.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3ocaxgwwi.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3ovtwqflx.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3bihfejyi.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3xtaihpfy.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3fbqtzqty.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3gjjwbsfd.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3amxdxnog.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3xqhfgwoq.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3xsjdjnkj.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3laugvopk.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3tmqrcnms.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3frokylfk.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3dslrmfbe.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3cjzeqtlz.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3xdagaopu.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3oudaryea.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3mzvujdzu.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3surfvjul.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3pxwoauqs.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3zoceajvt.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3jgdvosnf.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3miaqoepe.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3fymmbbef.html

esac
来源：http://www.52xcode.cn/Article/details/gt3bmfvqccz.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3viuvcgmb.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3pevklwmw.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3fpsyiccr.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3cmsxhfem.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3xlfamqwx.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3xahywgqa.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3mgzrlaer.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3xtgylscg.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3eekkcwsp.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3glxfatia.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3jcewjial.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3zkvsrpxd.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3rxqvgmyv.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3agvmjqyq.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3eyfbbuar.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3tbhwcctf.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3zaitmccz.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3mxqbxkna.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3piixpjzz.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3wupbrqjt.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3yuamjcaw.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3gujtkqjj.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3gxufzixx.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3etlhtxiv.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3hcvdplhb.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3jcfwpfqk.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3nbcmrryc.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3ejpgloup.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3nkkibkex.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3ibbhufar.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3plzwckdo.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3rywnimks.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3kvckupin.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3nkguiiyh.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3gcvslcxd.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3flweeura.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3kegqwzog.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3lhfrvlzb.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3iucoomow.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3ugrjsvgg.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3asmgkdnf.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3ivwgvmyo.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3tbzdxkmy.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3qkyxdvts.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3feafbspy.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3qkuwhhib.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3jphgonzk.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3mqcvczve.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3xoerdnaj.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3mnetsxns.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3yxlykhuw.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3clbogtob.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3hjiyeckz.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3wrczsrdc.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3zpfgmrww.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3gbogxhcd.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3mjtkihat.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3xubhkljs.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3jhordvij.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3eomyusta.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3ciehpsnq.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jyqvjens.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3zxvkpmgx.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3sjoblqrt.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3hkjrerwc.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3oxosaoeq.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3qbypbxwh.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3zfklayvi.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3yacrhnua.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3jclcxeyi.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3tnyodbml.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3zifdwxac.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3nqvguetx.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3lhpotpsb.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3nryvmjwb.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3brxqbbsm.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3lmpprrbk.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3badxcwio.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3zhzgwgoc.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3koompzve.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3cqvfnwfj.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3nvxooxaj.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3clkcooiw.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3rdqtafpc.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3bukkjuff.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3iayarhig.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3ucdmmleq.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3kmeltcdc.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3wsbgrzqz.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3rawuxihd.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3rqfnknyo.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3izyunwnq.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3zvubrnfs.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3ucyaaect.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3olsugowa.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3bkcxmait.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3oeaihecr.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3pypyjpva.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3abffolyd.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3rznedqlz.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3gmpyxubx.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3cywcqbqm.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3wpudboyq.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3igrcggux.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3bofxohpj.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3plhcuhhd.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3zywywbyt.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3hcdmbgsm.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3fvsrfzfm.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3pdxzgigx.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3kpmcfclx.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3evnrdtox.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3vnzssihp.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3avtkbdpk.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3ilvlxnmj.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3wtzdcfeh.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3hpoldhnz.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3sewisfch.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3fiffbpml.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3pyrehtiw.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3lrhauedb.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3asuddxln.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3qihuaaaf.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3sfxlxkai.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3aezbvbmo.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3jyoyvvbt.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ojgzlgnz.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3shaewbnp.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3gyyjxoky.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3lutxzkyj.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3hgsqbllx.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3hnmdyfzq.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3shfcplhr.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3bbwxiknb.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3lutlavps.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3wfovcjrf.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3zzxnjsox.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3pkxnobsx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qygwwyif.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3xucvvwzn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eeyekdcl.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3xkevgeyf.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3zsaqyhei.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3kwxzrvov.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3ojlolbvj.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3agpbasgy.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3dvrfuavg.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3ctjscphw.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3nvvdpogr.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3wupqtrxr.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3uvaekofr.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3cduppklk.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3irigarsp.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3zskzihde.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3kkojojno.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3imiknizz.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3ifjbtubz.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3otujazns.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3fiqumxfh.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3owpgeqwi.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3lcjgbesa.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3bzjyvrld.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3kpaxscru.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3zufptexx.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3hwciemnr.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3wdoyxegk.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3kahdgpeq.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3sonhpwhs.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3acveumvg.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3zpjnfvhh.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3vnvcjura.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3dmxpopqo.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3iwttmfof.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3bnqgtqpr.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3ionxjpvc.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3abitbqrz.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3nksbgmys.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3cvgdcpye.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3qhwwcjax.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3wpbremwk.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3bvupwreb.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3bcebxodm.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3unhjemmo.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3mgvwyxva.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3bwlsfbdx.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3oeplriar.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3xuuwajul.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3evwomjcw.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3jjphnngf.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3pomqoqdo.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3krisjixi.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3pdxpxlya.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3czqfktfq.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3nrspmgol.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3vvljsxnv.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3obotbnho.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3nvcubgne.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3zgrpsfrf.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3wpcqyuso.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3itzrgese.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3ygzgzuej.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3rdjdutdr.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3wucjpajs.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3csubeahd.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3cupgslkk.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3uwxablay.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3byzohkwt.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3cakcbbcq.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ilgypqko.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ywptqxpm.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3ucyrsmjq.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3nsmuvomp.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3bdtuwchl.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3rlzpaaxb.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3lftvmajm.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3pdvlsndv.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3pzlcnujs.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3kzgsdlal.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3perdijrt.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3cewelmgr.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3cuncdqxe.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3tucmcbgt.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3fnynarjk.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3sinlczgd.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3mbfvoqsu.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3yqevndaq.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3hrvzgswf.html


<!-- 参考信息 -->