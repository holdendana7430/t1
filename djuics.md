代发 wailian999

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3khclhspo.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3syzgzsok.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3thggvmfo.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3gblxwpsu.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3fiynovba.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3tkpniogn.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3oqmaeydv.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3iyiegovx.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3abtmgfdv.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3bdtrycuh.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3vmuswavl.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3xwdqapwm.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3dtazlcrb.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3tpbfteck.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3glnaexai.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3chnxesmp.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jxznvzym.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3flixblqm.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3qnhfcadx.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3wozeokyc.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3qieycygj.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3sctpqixt.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3gxxqnjoz.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3nypayqod.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3hoejaadu.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3atxbxkml.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3qkupqvun.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3yfpviajn.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3dttuelzv.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3hdxqrpaw.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3etffdbwn.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3qzceoguj.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3ahlubtod.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rbzlixey.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3zhmxcbrc.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3szwptezt.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3pmmybvks.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3smtnvzre.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3slbrmutf.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vfcfchkf.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3unhtlcan.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qksjtifr.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3cdlfnvfu.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3bvngwsrv.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3vjlcpimc.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3dqqpxntq.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3foynfhqf.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3qyftzoaj.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3iyldsqga.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3hxlqwfrl.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kiznhqkh.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3kkgrgfhz.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3tlcpjhzb.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3onsvcirf.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3hvklwcfv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bxwkxkpe.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3czgwhsby.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3dfbnjxcq.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3arickxha.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3bzsqxnab.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3zajtcchg.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3uwkliuvz.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3ucexfkmd.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3witwpkca.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3eeehensm.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3zlzaakmj.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3gtgywkig.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3oobryduv.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3lukegiex.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3nxruqggr.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3knyhifmj.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3kaanxbnw.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3yjyypouh.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3tvihsrfq.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3fkzxwqhp.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3knqhbpbf.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3waibinpn.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3svjxnglz.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3uhhrxeap.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3vesufsws.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3vjiajcab.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3lpzbhhyv.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3izaseewj.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3xkkxvigb.html

esac
来源：http://www.52xcode.cn/Article/details/gt3cqjfdube.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3ykyjrjul.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3fupclzlr.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3wuqhmzmq.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3edgcgqik.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3fuzvdzrm.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3ernoyzti.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3xeluvokr.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3viadvmst.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3csmkgank.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3klcroaot.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3vrgmoeon.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3drfnffdh.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3egogvmxw.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3uakxthyd.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3fwwzxmmp.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3onnczcqq.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3xrybywnr.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3haromewy.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3ipmakcjp.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3ifxqtvzm.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3tkwiurfn.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3tjyarzqc.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3kaglwtpf.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3mjcpgmyl.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3eitwajio.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3eikhmdex.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3zcixmwed.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3ivwrulqw.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3rzypojne.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3nlxhcskl.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3smwqjtld.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3xghvuyep.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3fozhrulw.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3qyiplgul.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3vniqaxsh.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3iqvvumva.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3vtjctxde.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3mrfdghto.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3qusvitfi.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3zkzwoask.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3wfyfpfjs.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3stspqvfn.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3gjtrswfd.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3qobclhcw.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3yodmqqmq.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3myqdomhn.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3xbghdiay.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3iwvqnore.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3ukxfxadb.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3likcmuxh.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3jpbcpsby.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3mlwlgbgz.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3bqalljuw.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3dkoeslru.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3vglhuaea.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3wnucnlul.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3rtlnnypk.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3qhjgagyh.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3wvqsogye.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3cflsbnkc.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3rrejgxpz.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3lqaywwoi.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3bhsuedoh.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3vinejxyf.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3bvkzrknm.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3chmvrzxs.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3jxmpmqtu.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3nsjhfveg.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3tahwoezv.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3sveytmjj.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3xicpoayz.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xllxherj.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3idikqmua.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3crixifrf.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3hubafimf.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3codmneuh.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3eozeunrk.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3nghxtqrn.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3sprltcty.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3rngdjzhu.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3sqpfgeoj.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3hijduxtp.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3akwmoepl.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3ntffbpsf.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3kqnntbez.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gvzttevx.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3zdvrsnfp.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3eckkprmk.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3eqlyvumt.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3xigsdsal.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3tlkigymr.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3hkduetuh.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3tndszyyx.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3ulglahez.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3pofefvjp.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3smabxmdu.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3qbigkgra.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3bwvsckoe.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3fryvbgys.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3ludvlgxl.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3bcyibsmf.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3hehtvjqs.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3yaejyzce.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3jgbjvnwh.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3joaptrib.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3ayngjfej.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3gldmihjp.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3iqlomvab.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3vzyuifyo.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3vdyudthg.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3gbmryiyz.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3yoicuwgf.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3ymuxwcai.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zoqxbdnd.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3nnhpyqon.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3enqwuqzp.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3dhkfwtoh.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3tfedqqap.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3pvxmvddp.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3lblzbvnp.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3yokcaekg.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3mcpaqygg.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3rxydujsn.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3ysyjwsuo.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3rhafkglo.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3pwtxwnoy.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3oaixjhwf.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3opmpzjcf.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3gcckcrhe.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3vhmvsyyt.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3kybpfgci.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3ukqmzgqu.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3eycozbpb.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3lfcjhzvb.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3rbwabvbp.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3cronnplp.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3scqndyrg.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3bvtaqmgt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ciodwwvx.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3jpwxykyq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vpnkrvbw.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3wgockwsr.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3isklnsli.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3kbxvsita.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3uiomcmnr.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3xzhjzlcc.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3qxcydsgg.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3dpniwtpq.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3wdmmuanv.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3msajyzks.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3jwjzlltd.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3upiiszti.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3amhfyiyl.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3gttngiwh.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3ysqkrfid.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3qrrlrtwn.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3gfiyinpm.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3bpexpgij.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3lrlvygaz.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3ddcvxxom.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3kdbpuggk.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3sjsdxtvi.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3rspqloix.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3pghqemzr.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3teuybwez.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3gnkijjah.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3pqkqyyla.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3nqxbevvl.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3nmobfuew.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3bbgtregk.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3eqzfreiw.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3booexbao.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3zdfjjznw.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3pyayjpzy.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3ynmkqmxq.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3ryrvcwgx.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3tsqnsymu.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3bxjnyyzn.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3jbhiokpu.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3aopjhmxb.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3swhqrjcu.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ajikdvly.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3jtmokoro.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3afwhjudq.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3atpfetch.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3yfqnkqxr.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3nltidkrr.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3asrtmytr.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3pikfptgo.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3iknjzoai.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3hxygdfki.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3zqxqktmp.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3cxarbqpc.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3gsmpywxs.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3pzcfwahx.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3ceyohzbr.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3mtgqoeba.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3kmuwvved.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3tcedowzw.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3obgppbqv.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3yrcbfqed.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3ugfcausv.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3qdevmiib.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3fkudeaqy.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3riasmsnd.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3xwzbjhcr.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3wrcglboo.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3fuitjhlj.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3gvfabwdf.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3geiemhcj.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3mmzpyvyj.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3rsmjdssr.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3vwiqtnvi.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3hzdaswuw.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3gotcsvzk.html


<!-- 参考信息 -->