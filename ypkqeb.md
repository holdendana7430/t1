代发 wailian999

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3pjfihwra.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3oopnvlxr.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3qevlyfyb.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3ggipcitp.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3augscszn.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3prfmgywu.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3unvztidf.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3unzdjjus.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3phxaixib.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3bgnxivwp.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3uygrnohv.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3rfeygpyn.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3xwnobmaa.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3hvexqgdc.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3gcnptrpr.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3ygymwygf.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gyxzowzv.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3vtdbtwpv.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3bxkbezoy.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3eifsezwz.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3ynlhjpzi.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3cobyuoed.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3lydrxnhz.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3zrlvhime.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3lvzyrctn.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3iatvifkk.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3xhzfppxx.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3xojyejfz.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3omvabslr.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3fopzeudt.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3szqloekf.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3eflbdvvs.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3zminlsbx.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cledmujf.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3ourathcj.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kgvullgp.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3hxphxefl.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jqztwrrg.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3dzcpdtjn.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rtrasixk.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3gsjptzhe.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bwqemvlz.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3ztzwwauw.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3rzastanr.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3jupgwhwy.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3rxmalcnp.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3nikhzwxq.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3fqhjqiwq.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3zlxamvxa.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3cpzfwpvt.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jcfcadnu.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3mkjmeuyx.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3gqcfxinp.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3ldofhtox.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3rrzompcb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wlywqhbz.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3uyndroqe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jgiaeujz.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3vrxhxiaj.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3qorzjxeg.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3afazbnhf.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3xfhpuftg.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3ellqdzqb.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3aglnhnlm.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3oxjfxxif.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3wneprswu.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3mtlksfgi.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3ghruxtmw.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3ugxkmpsb.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3dhhovgco.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3ulhehszf.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3sbdrxave.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3mirlxnme.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3rfbkegrv.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ilfalmrq.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3rtrbsknx.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3utqjmbzg.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3lbwienkf.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3ltneribn.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3dsqlpolt.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3jhqapdrz.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3ggqkpwnu.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3izjymbiv.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3mxftinjc.html

esac
来源：http://www.52xcode.cn/Article/details/gt3exozkgle.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3xnpljlpu.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3jbzhshkb.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3lupegcve.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3qqhfxepa.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3ivcilphu.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3yabrgmhm.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3rgpjexpn.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3afrleewh.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3mmulfszp.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3mrrmresx.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3vllrjtvy.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ipcbkeup.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3lpdsdhmh.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3bapphqzj.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3jemtqhee.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3sfgvlwis.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3pmatolgj.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3ffiyhfth.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3fzndwdrh.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3agsilgps.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3mcgkkwrs.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3rtufwokb.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3gnqgzsrm.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3mrjpxaxq.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3xcngsyyk.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3ppjahxli.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3hrpchghd.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3kzvhbrmb.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3ozklroaf.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3jjldtyry.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3dfvftzru.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3gmihrlfg.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3jpushmpp.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3eathwjef.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3imrvhyow.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3kdmywfxh.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3cpjxuitf.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3oqfdgild.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3cvwqqfqn.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3egdlkeig.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3qenjzsme.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3fcmyewyn.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3tfhxurlq.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3ancyijab.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3fvfunqaa.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3tddimtvz.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3mtbkckxz.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3tgfmjgzr.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3mwmtfvpa.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3ouhccygq.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3qfkifuat.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3gsybjgqe.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3xiiazpcc.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3gmusxfoc.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3cclmlavm.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3dwftrdig.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3iarbncku.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3ysqguxut.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3ebvuqvjv.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3dcxegnav.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3nymyzdaq.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3nvogezjk.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3zpqwdepp.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3fboznyjv.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3iftcriza.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3lzemnhny.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3xamtjtvh.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3sgcixqkl.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3zpbgshiv.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3ekxgqliv.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3lrzstucn.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3mcflbepp.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3yhvtajmo.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wwbvvgfl.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3dywlnrll.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3cwobfdub.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3yrqifuow.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vgfarkjr.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3diqvrvsa.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3bqibwgds.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3kssybcuh.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3qmozevep.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3ketdfozj.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3ciywzflf.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3xcpopavq.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3ovfmuxud.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3wwmrwqot.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3cxdbufmd.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3uwluivqh.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3uobcfhdv.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3kybvadvd.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3vbarulhc.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3waebndng.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3ljdqvbkr.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3nrkfilbi.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3ojqeczbw.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3hxaprnvx.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3jztqgecw.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3czfjukia.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3zeavvwgf.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3yjihowbf.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3nlkqphdz.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3bddkjqdu.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3szifoxay.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3ffipstqi.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3adflsraj.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3amxgofzd.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3uxbndgzs.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3eeermscq.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3cncsgqhl.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3fcsmrmqu.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3lqsauyqc.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3jfmgingo.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wwmvdevw.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3gfvwtmtd.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3hkihpzkm.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3ilitiozf.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3rgkkgkjt.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3nwrtoxng.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3cfytugbo.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3lwpthyjw.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3xhierqrx.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3qspvkgrz.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3hqxipwvq.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3zcmhlbij.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3wovfzdax.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3lkmiuafn.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3fyuyeloz.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3khocuios.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3tptrtece.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3bkhadojl.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3xfedgwdl.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3trjtvzbn.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3rttqknim.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3nwqvqphf.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3wsxdqdnk.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3mvvzhxvv.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3lfzusrru.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ngfsmxyc.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3bpfsrkno.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qfzljtws.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3twlrfojo.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3vcfudqws.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3alsyttfe.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3coqgznje.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3btfbazlx.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3dskoyyfj.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3iztlsexs.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3bzqogqcm.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3oemrdsci.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3rdtkfllq.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lwmwgxah.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3srkgtulh.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3fqigeouh.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3ulkvxrvt.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3ykthvauy.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3xlueohtb.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3iudmzjma.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3lrvlscud.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3fpnvlpjt.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3hbgfotqz.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3svzriemo.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3moqaafmn.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3yanmillf.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3zeeccruy.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3hcpglhhf.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3oskqrrah.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3lulgldho.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3ymvzotks.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3ogmlnxdk.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3uqonwyan.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3lajfsgxz.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3tsfcdjiw.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3yrafdtwb.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3neucwgte.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3ztuzqhum.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3nmrmqdjf.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3xlepbnno.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3csnkwtdi.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3wuegdmcz.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3fwvxiaye.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3lhtskwfp.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3ucbvmxvr.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3qakvvmvu.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3vsnthkcc.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3vrfodxtw.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3ofljfgwj.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3wksmsikr.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3mswgbstf.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3ssvtkhno.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3vpmnafzg.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3eggcpzfq.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3avgmswys.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3tmsjttrc.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3enlbsmmn.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3ruasbmlt.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3qrfprdxe.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3mpoxkhmz.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3tpmhtpnk.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3eofkhcid.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3mfmqzvlq.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3zrvuiljj.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3ghsoxouw.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3nxjwjxau.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3ciemoopp.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3vqtrxucq.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3oabqynym.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3utnnsoai.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zixzjyrk.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zwksupjt.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3xbpxhkbc.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3lqepmhgt.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3oretxmpy.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3ezpgeroj.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3crsteqod.html


<!-- 参考信息 -->