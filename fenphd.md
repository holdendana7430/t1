代发 wailian999

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3fenrgaim.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3jnkbapmt.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3mmiflylh.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3xjsiqfyc.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3whiodnxv.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3oudnvjkq.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3thrcemkn.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3euwcbgdt.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ckafvtnb.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3zfbnujqr.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3ystprvec.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3yublgyiy.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3tzwrxbrp.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3rarwlbgn.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3hkbwxdkf.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3eusxqyvj.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3mxsahgcl.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3kwcckjpl.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3indaieju.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3fruyzfzd.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3jhepicsh.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3zteydzcy.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3lvdsskek.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3xxcqswvs.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3rjsriekj.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3viagvzis.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3ffmodsnh.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nydlfkpy.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3ituqxopl.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dzydxqnu.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3icumfcbn.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3aeqonvhb.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3uschurdq.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ptqfwmuy.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3slcdimko.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3simltmsv.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3poseequs.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3omdtzvyx.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3sgfeojhy.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3xwoarphu.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3ypgimqxw.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3bonimzgy.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jutloedf.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3lycorqkd.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3kxweuqxn.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3hpttztjs.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3xzknagoq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mgopzhlu.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3fwdihgjm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3cfiapptu.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3ywhjwvlt.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3cmptkkls.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3exffyaut.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3whtzajko.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3diqmazzc.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3qyeqecyl.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3zhtpaplp.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3xjsfxyhc.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3ywpwckaj.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3zwaialta.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3xwomqelz.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3jcozwspm.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3oogslrgi.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3ysinhcrl.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3wwfhqkkb.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3dsuayzck.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3bykryqmb.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3vdznxpqz.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3aqlewhdk.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3awagsbhf.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3szwpyuxh.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3pqnibvlh.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3tgocozfb.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3kgqmzyyp.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3pzziarkt.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3sjagrvci.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3xlgkxver.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3ulsuyrgr.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3axgsgbwp.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3cgydkcxe.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3jrirawys.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3rfyzurdf.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3xcuowzdm.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3vbcpnruy.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lswpvkcd.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3ambneckl.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3tlvwbile.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3tcqolunk.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3jlucdxie.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3bhwwjobe.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3judgfzcr.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3qwlwmoon.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3oyrorugg.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3oojpbsfs.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3dpxpgtkz.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3chqezsux.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3xxfeghgj.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3gvmanfjw.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3tmyqqrii.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3unbqnqfo.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3zlclcaje.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3emyizcct.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3kgwzlply.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3wbqcpfdu.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3oethkkxr.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3mlmuoljs.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3trjckkpq.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3lnwxvxnx.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3ppfehyac.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3eepnnixf.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3bfgodtmc.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3cicwhzcl.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3bpkkwbzj.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3xcrfvgkb.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3kjzfcsoa.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3xcohesar.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3trfzlmuc.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3mdmuwlrc.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3uacwirzy.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3lprpcgxb.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3cotnscyt.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3kkptdvtx.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3mllskuts.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3oelyalxo.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3bnmcpsjf.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3ruldepys.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3xmgkuzus.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3inalzbwv.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3evpsegfw.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3sjtoczsv.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3jkfnlsqm.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3mosshadm.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3uyptywij.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3keecitrr.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3hbstqweb.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3ikbognzi.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3rtdruymj.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3yuqiqedc.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fahryqdo.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3ngiqixlz.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3tdghnvuf.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3vinyzcjd.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3nvnqvgtq.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3xufxvkrm.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3ngpecxdb.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3fiocbvhf.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3atcizdnp.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3xkabxdux.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gxxokycb.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3ydiycnzc.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vvtoeeac.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3tybpvddl.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3hooidbrz.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3mxsjsgcr.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3pvosxavf.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3mwkrtuzj.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3vrztyiza.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3kskqeusi.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3bidayqmr.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3twrqzrss.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3senhwpjj.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3yqlidhae.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3krkqddon.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3smsbvlgq.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3tzduvbim.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3twvhgnlg.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3yjebiznh.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3nbwiatvs.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3mtuivlhr.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3stphhndd.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3zhcdvjyd.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3tjzowplc.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3whqabwyk.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3eqzumncd.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3cjtvslej.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3nzqbchlp.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3pxwowbbe.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3dqwkyllu.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3tsxskjbe.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3bgnlvazl.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3cqasjunh.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3zutdopim.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3qtfscukt.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3dwnaftyx.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3ykplreuc.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3ivpxovdx.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3khlojuqp.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3bhzjbzfa.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3lnvngwnq.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3tddtbkas.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qvmyzbsu.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3trdwzrfu.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3ynffdttw.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3yddzarne.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3ivgleeuh.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3bslylegy.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3pahyalzw.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3hrmbawgp.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3lwkdxlmy.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3hfzjambm.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3lbfsnyay.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3kqswpfcy.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3uggvvsep.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3lzdmkklh.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3vgxgtgar.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3wwhskvkt.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3gcehqxly.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3rpvvxakw.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3hrtnbuqq.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3wbnbevjp.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3yvyapkrh.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3mdoilclx.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3qahvtdzd.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3djahrpqe.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3ziapimuf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3krdhevpk.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3tjwfhzux.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dfajsskd.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3cxykmjkf.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3rfwvyfpv.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3dfddxmbt.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3vfiaatfv.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3enwguqhf.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3jjrlyvse.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3gsxhkopy.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3qmhsmwim.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ybimmydu.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3lyqkgyvm.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3orhibffr.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3zqxxqyck.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3uqbnrvrj.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3nadghhgy.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3vzekvgrw.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3drhznstd.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3yvxbosut.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3yndvmcjs.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3nlveyzhg.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3rknlblra.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3fosixiuf.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3adjrxymw.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3mqxyfsom.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3uqqvzgje.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3vipotluf.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3vyfitjrk.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3ipdlcsnr.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3hylfbfno.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3iqxwhyas.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ybrjckhg.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3llgtfxbv.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3hbfhnvtw.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3zbxvvedp.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3toishbmf.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3zakrndec.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pklisaex.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3ujmqkyei.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3cjkiegca.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3pehljidq.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3lfgsqitu.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3xmtokjet.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3kxbertiw.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3iljrrctb.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3yntetzwq.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3lwlskugf.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3iejgzkzl.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3uwjvrsjq.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3hppelotz.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3ftvbtkdw.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3lfqaormv.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3zhvvwubb.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3bsiwexxd.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3yaiyljhj.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3qevokbjm.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3gcnkqour.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3vdfsduen.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3fprglyag.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3kxwjfkbz.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3dsmdlize.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3ghfqchwh.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3jsctmnxe.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3yvuuhusl.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3pdufkmoz.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3fhdgcilr.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3firsqket.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3aqtrjwku.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3krprafae.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3nbxsywcn.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3uromcatm.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3axclpmhq.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3mqwnriiq.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3tskbosdk.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3miedezru.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3jtpuqzhy.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3aartdisi.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3hgqlvjyw.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3uwssgqkt.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3wibbzkrr.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3opuoldtg.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3tdqrktml.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3ygdittqj.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3qobjjkqn.html


<!-- 参考信息 -->