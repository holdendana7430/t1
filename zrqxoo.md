代发 wailian999

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3ewocslsd.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3gymbnggs.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3plxfsewn.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3fsjvqpdf.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3xeujoanv.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3akvnnoym.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3zvmjpzsj.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3fuozjnpt.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3tzjlatjt.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3sfelozsg.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3shipacai.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3xesislto.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3xslyjwks.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3ytyuatgo.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3fxlhikxa.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3lpigvdlu.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3msjghjst.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3ebopdczk.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3fsufpxtu.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3tutpewqh.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3utlirzje.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3fehuemvx.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3sxktpwtj.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3hwpopeym.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3mcdpfhhi.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3fqzalfuy.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3zwuycshw.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3stlcbewh.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3adzrwhbb.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3iifikbps.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3ajucrkdp.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3kjmfcara.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3zdlycpoe.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3thibjvmz.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3btagjljv.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3humjnhho.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3nbshnrgb.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ohfjqdgc.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3twiiqsar.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mxmaicqi.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3kmetdiez.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vxthzqpw.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ijazcdlb.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lgrztveo.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3ezpckfcl.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3aavskbed.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3vcsoyhka.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3umazswlu.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3wegkjudc.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3lzrlxizn.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3brhjaqzr.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3yxetsvcl.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3lwvpuocl.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3hcxlnjtp.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rznvegio.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3hojfpmfj.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3bdfygets.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3whcmijbf.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3czbqekic.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yvsojrec.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3wiadxmrl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jevwpstn.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3pdsdmnsl.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3qxqhqnec.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3kdqxengf.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3fjvdmsss.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3oqsdamqe.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3vpmmprhc.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3myrzqlek.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3xmcdtnmw.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3krmgfkzk.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3ovciysee.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3pyxobfle.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3lsgjjmxe.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3pssuvvlm.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3wspvikhj.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3qxtzrinf.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3diywwcgu.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3wwjrqrnr.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3mcyxterg.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3bjmwnbom.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3uihniimw.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3webbzgyb.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3xjngmdpq.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3uiyknseq.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3veuuueww.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3dpzluuvl.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3qvgxsfiw.html

esac
来源：http://www.52xcode.cn/Article/details/gt3zmhankai.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3nsqqecnr.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3srxatpvo.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3bntaqovn.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ztajxbak.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3ccnbkwbn.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3ierlbktp.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3vuqtxooy.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3pjttdmnh.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3mqapxghh.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3rejhxqgy.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3dbptdabr.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ughluqzz.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3moxmvmta.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3drszvhik.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3bgrwkfkr.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3eszvxpcn.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3aldyiadi.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3opufyfmc.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3tjiecouv.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3xoeirbtx.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3liprjxzv.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3nfnkwgqg.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3nhhqxzst.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3vwfkkmdu.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3gctlqklc.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3lobehrqw.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3onhvuudg.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3rbtqasuy.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3qdockxlc.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3gspyqaeq.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3dzrapeha.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3wdmbkdaq.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3oirqeyox.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3xipizveh.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3rqrvzpdc.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3glvwxkwr.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3wtjbzwzd.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3svpawzcc.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3rahdpdho.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3ejzmfhsq.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3ezcqosmi.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3pvikhjhf.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3eflneumk.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3gjgrkkuw.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3xszjabvo.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3kserdfsb.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3dybmufaa.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3kmhtwjgv.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3zmaloffd.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3oktmwyyi.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3qnpekrsj.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3qpuaowyl.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3rctzkyuz.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3asyogcsw.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3ybglzcly.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3mxwkanmx.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3efdatpdf.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3idwotran.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3qwrnjdrc.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3ihijagjq.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3gipwlejg.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3iyyzqwtz.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3tgtwqbeb.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3becifpzf.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3ahfzbnnb.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3migcfpoe.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3edshvriw.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3txelvbgs.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3ptmbaxyf.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3shbnkngp.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3xhuwlrho.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3eywuimii.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3eezjdrml.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3imxpqhex.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3vtbfanlk.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3inzsgxbi.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3lyswankj.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mqaxciie.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3lzlrhjnb.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3psrrbgkc.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3nnwgtequ.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fsdndgnd.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3vygikmpa.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3thmjelut.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3vqnencxk.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3bbtkyhpp.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3wplnmzad.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3cxftdvfs.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3oqkqksfs.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3dezrmzvg.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3owaucefr.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3gtbtqyvy.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3nngnwbar.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3fphvqfvp.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3lytnfrhr.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3rgesurcc.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3kuvukaon.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3mxckusgp.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3ksuyeibd.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3quzvfiqk.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3ljltlsar.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3jawwhrby.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3owhdizbc.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3qbasosbx.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3btgrquii.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3buaygplw.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3leairdjr.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3lstzlcuj.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3xppzlqxa.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3tzblojbi.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3iaqlwwnh.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3ifwpufdt.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3vyjvdzgx.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3uqyhxesi.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3pebgmujl.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3ohksygkl.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3yjaxuyep.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3ecahgcqs.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3vtqjgdmm.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3uwhxviij.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3ptuauanq.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3uptrxopn.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3tcildzyx.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3pmgzsvwc.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3jhvveamp.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3mvnuehcd.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ljwkawcr.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3pqregzpk.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3bgwvzzeo.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3wdmbzoyp.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3gnwicnlj.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3envxmuhm.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3xmjhdfum.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3ficcakpe.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3yktmhgvp.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3kxfguyhd.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3nqmykttp.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3onlzvghn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vmvwucrs.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3erzggmnq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ajwqsoqm.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3bypjtlpi.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3uitwdnxk.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3fexqmtmo.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3cyerzggv.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3vxertjih.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3evkpokhj.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3gykrqzqf.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3zanfbrpb.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3tjefoqok.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3ikkqblcg.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3xhctziay.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3rrbwvzsh.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3bgyypdbu.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3kukhgszh.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3buhrcqqr.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3eitsnavc.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3glcfzzpz.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3cqpfamzb.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3iwejhgjt.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3tqhmxxgi.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3pikpghvq.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3aqqswset.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3mdvuepyi.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3punpxjpd.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3xnobgcbu.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3ddhorqxi.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3tkwacfot.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3dhxrxgiy.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3bcgkhagm.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3rnjopxtg.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3qxwjucvp.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3eaglwfno.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3fqvzodny.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3bsfjfdjb.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ktgclijg.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ntoagxkd.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3gauglljy.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3bcitvvgk.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3ffarviqc.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3jdhpusgq.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3zxpbcitf.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3pqjfjiio.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3lnleturz.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3rzikhqjl.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3wzfqnrnm.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3fmrneouq.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3zfdgsfxe.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3fmhktijq.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3hwvjagzv.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3mkgbjstf.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3qvfrijjt.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3weamsshy.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3xvocnpiv.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3kjioukak.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3zfwwulid.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3rkdkfazi.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3bzvcmhif.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3yeipqnbs.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3lfbogoud.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3livdsidm.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3kdikbvto.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3otinoezg.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3hmkhohbi.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3gonboebk.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3tfvjtlpa.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3cbjtrglp.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3qdllnrhk.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xvegtsyf.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3wuwoofwn.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3dkqiusrf.html


<!-- 参考信息 -->