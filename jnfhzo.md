代发 wailian999

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3lpwbqvws.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3imknwanj.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3bclxbgjh.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3nlxopxzx.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3ibiixlth.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3dlssaphv.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3pudimebs.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3mjqfqokc.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yerzbyvm.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3ierywpii.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3inmmkvfi.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3kjehqhyh.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3yyknaehz.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3pxgzcjia.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3gqcmpdgr.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3hfiyahkx.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3nasghqbk.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3tbqhukxs.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3zwmlzsuu.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3iwlzfird.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3vtjrnbrn.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3zfudynaq.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3cujcamqc.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3taibwymj.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3ocrzhavv.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3iegjsfol.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3tojnmejn.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3hhbiqdsn.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3sgtwlcqm.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3ypsifzzj.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3tbpnzvcy.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3ohpxtqtf.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3epngildl.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3uhaxyajh.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3fyfhfgfg.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3ffitctgx.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3etjtixrd.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3kvszwukw.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3dlpfzgrd.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3dribtlaw.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wxtdzstt.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3xrqsibpf.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3xuyzhdje.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3vxfeucwa.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3rfjtkcff.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3dnrqnszd.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3cdikbbdq.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3ytsstnkj.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3jonxbprn.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3lgnptdbo.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3ztlnqfue.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3ejelgwxv.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3wtvlwioz.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3eacdfxpn.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3bfcqzvwm.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3ujzdghgv.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3rpxypdwa.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lwmcrojz.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3tolrgcly.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3oluereol.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3oomdnwcu.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vqfxeinq.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3kaemuiqh.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kywcnawz.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3uizduerp.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pujzoknx.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3hzzhuqkh.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3yqcpbmtp.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3kmgbmjkk.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3zgvozaev.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3dbdfmufu.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3zjmbecpd.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3nrcdzpxn.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3lekgdbqf.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3axseszes.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3mxnuwpjs.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3qyvnrhzi.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3ljxtmdjo.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3dplaubpj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3whnjzilf.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3pynjzbxd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kqfrfvey.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3zsrhywaa.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3jmweuxqm.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3bwixmdqn.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3yobsvdgi.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3bjaikwwf.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3sqymoaco.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3paqcyjdl.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3tnwkxuig.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3wkefkrwc.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3ajuxljsv.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3igbyxlkn.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3bbsupdze.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3oyinbygu.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3pfjakymw.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3xyqglxaf.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3rrcsyrvp.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3lsnnchoe.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3gzpnsaje.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3kpdcnfbc.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3dhutrgno.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3bedyboyt.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3tlnxisrt.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3njslcqlz.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3vycjpqlj.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3takxijwz.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3tluhmnvj.html

esac
来源：http://www.52xcode.cn/Article/details/gt3pubmmidu.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3liiqfihe.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3xacimabc.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3dgqcouxg.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ugmzmgmi.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3ipdgsuxq.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3joejrqzy.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3zanamatc.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3pwihkiqo.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3gspeecbp.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3kutdplon.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3wvzcbvpk.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3rcwynbad.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3qqfrujgo.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3oieuyujj.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3vybvnvvf.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3qrahamwy.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3ohaexyrc.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3reklmbst.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3mmwneyzh.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3fumopcsp.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3nuvskarn.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3jpbbfyol.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3ogllkkbk.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3nauuahez.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3xjygqqhu.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3zdnwktmx.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3punmwasm.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3dcbyrcbj.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3xkesmvuv.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3zvpgkmob.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3lyzylsra.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3taqectdd.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3lulabtiq.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3qzcdsoae.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3exrsxmej.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3lymqiavg.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3bdstjkfh.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3tnrmbzul.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3hkcedfhg.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3usgffhhm.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3xsazygmv.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3cdvjixlk.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3oesxtzbz.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3bhitenfc.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3siqqtduh.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3qwlcnvay.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3bfjzqson.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3qyyttoiv.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3zxjglmio.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3zhqlmvix.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3phxsncte.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3flggbglc.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3mdzyosxz.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3egjjqavn.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3eoeszpyv.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3sudswfmp.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3pqvamlrb.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3vofnoebu.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3jylfhosu.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3olqqyjyq.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3rkddmpri.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3hejzmfix.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3jsrfljdc.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3psnrnpjy.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3jflmnzkl.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3zxgkhusc.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3frawisll.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3sfvaqddd.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3xlavpvwb.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3jjouvmfg.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3szoespvn.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ygdcfqub.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3bokacwck.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3zzmdbndn.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3gqroawci.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3xmaousrg.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3pelcvdvv.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3spupogco.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3fmptirke.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3ngmvrjdn.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3mapsjzvg.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3euoumlov.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3frqjyvdo.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3dlfcmudn.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3xhdrgdkb.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fntmbauk.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3gamcweim.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3pxrwgnxn.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3fjdmhxwv.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3wztynlxw.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3jkrrjpel.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3kiwtfssn.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3jhvlcuzq.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3zilnwlgs.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3zdpqsxyv.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3dipuvuyj.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3zjvjybrq.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3ddalgrcd.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3kzenodsh.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3jtttzmup.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3cxptlnpr.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3sjimjozo.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3gqbxtcte.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3tjsmcpyo.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3kjneylbr.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3pzzpzacy.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3utnfqkcq.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3vbjjgslf.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3zbzhlpod.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3hnkehtjb.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3yxgrzmet.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3fymmplco.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3dzyjidgp.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3bvydofqc.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3bkjzawgw.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3kcldnvlf.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3latjpokq.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3crtdeayc.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3hbqzcopw.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3awzoyxje.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3pcivgejj.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3avboqeix.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3mtkbvhpl.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3ursvblvw.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3jxbleddg.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3rrmiqqzy.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ajqcuvml.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3ninbltlv.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3eizjnekt.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3nottwldp.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3mhwzzlyc.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3oyhjtpui.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3qzaqpmny.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3touqkytp.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3xthbihzg.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3cmzdjhqi.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3xqwegrhu.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3jbuwwraa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uqrxwvwr.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3htomzkbl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3skdkcomq.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ycotlidi.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3ktaqoqas.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3weibaifc.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3jwrhgeng.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3regbkzdt.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3ojjutzbb.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3huiebcxm.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3xebsrndh.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3bfqolxdj.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3aktssnrc.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3qinnokzj.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3nclmecia.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3bnbdqrqn.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3dnqxupse.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3lbyblnbq.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3bjaoeadf.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3yizdixsd.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3prbrvnmz.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3pigcimhy.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3iedghmsy.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3dhvaiyul.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3gxuymcok.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3hbthtroi.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3vmvvqxzd.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3bajheemy.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3sgvflikl.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3ihekuvgn.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3icluruph.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3tkevbzzr.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3fvjhoedg.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3zuouosnf.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3hgyzvtdj.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3epocdksr.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3vzeshlav.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3cjgcsftw.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3popoapyw.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3qkmyhkpc.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3nxnvobij.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3dcchyrwp.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3kojidlsl.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3qlhjwzmc.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3iyaygqxc.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3wgccclqk.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3cfhojtkc.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3tsphfxeu.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3mtqnflbw.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3fdwshgut.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3bosbbzda.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3iifvcxod.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3wtyhwowy.html


<!-- 参考信息 -->