代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghhwnckmy.sHtML

[Q52] 删除指定行
来源：http://blog.fanxiaobao.xyz/Article/details/gsorklavy.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwqzuessg.sHtML

[Q53] 按条件删除
来源：http://mobile.fanxiaobao.xyz/Article/details/gttrkdkea.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.fanxiaobao.xyz/Article/details/grbbifyvt.sHtML

[Q54] 清空表
来源：http://read.share.fanxiaobao.xyz/Article/details/gsbrblakq.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghwlgsjnf.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.fanxiaobao.xyz/Article/details/gptrdqmkd.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbxhzzrcl.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.fanxiaobao.xyz/Article/details/gvgixxxpv.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.fanxiaobao.xyz/Article/details/gwvpcjcrt.sHtML

[Q57] 行号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gulrxpnpl.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfkivkcud.sHtML

[Q58] 累计求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghxrzrnoj.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmkjjyfen.sHtML

[Q59] 分组内累计
来源：http://mobile.fanxiaobao.xyz/Article/details/gnfdikplu.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gzichshys.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.fanxiaobao.xyz/Article/details/grqakpzcq.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.fanxiaobao.xyz/Article/details/gdsxoajsl.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtbteucjh.sHtML

[Q61] 移动平均
来源：http://3g.fanxiaobao.xyz/Article/details/gsolrpqdk.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gqcszbkmn.sHtML

[Q62] 分组占比
来源：http://www.blog.fanxiaobao.xyz/Article/details/gntxpcyah.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvtpurpad.sHtML

[Q63] 开启事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzvrpehva.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.fanxiaobao.xyz/Article/details/gskszmyew.sHtML

[Q64] 提交事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gpdtpfnrp.sHtML

COMMIT;
来源：http://wap.fanxiaobao.xyz/Article/details/glbujkrbs.sHtML

[Q65] 回滚事务
来源：http://blog.fanxiaobao.xyz/Article/details/gdouwapkd.sHtML

ROLLBACK;
来源：http://www.blog.fanxiaobao.xyz/Article/details/galxpftbp.sHtML

[Q66] 行锁查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gozbazfxj.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.fanxiaobao.xyz/Article/details/gedoalvgf.sHtML

[Q67] 设置隔离级别
来源：http://www.share.fanxiaobao.xyz/Article/details/gvjiaxhxs.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.fanxiaobao.xyz/Article/details/gbpesqqzz.sHtML

[Q68] 保存点
来源：http://read.share.fanxiaobao.xyz/Article/details/gukzbgyue.sHtML

SAVEPOINT sp1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gibrlmfme.sHtML

ROLLBACK TO sp1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gyohtokrr.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnnymyygb.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.fanxiaobao.xyz/Article/details/gewdqpgeq.sHtML

[Q70] 更新统计信息
来源：http://mobile.fanxiaobao.xyz/Article/details/gdwprehka.sHtML

ANALYZE TABLE users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbmgbtvpt.sHtML

[Q71] 查看建表语句
来源：http://m.share.fanxiaobao.xyz/Article/details/gijmisjmg.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fanxiaobao.xyz/Article/details/gbyxhumsm.sHtML

[Q72] 查看索引
来源：http://3g.fanxiaobao.xyz/Article/details/glahdrwur.sHtML

SHOW INDEX FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gkcpejhww.sHtML

[Q73] 查看表状态
来源：http://m.share.fanxiaobao.xyz/Article/details/gxjqrjkvw.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gveprxgai.sHtML

[Q74] 强制使用索引
来源：http://mobile.fanxiaobao.xyz/Article/details/gyrgextlo.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.fanxiaobao.xyz/Article/details/gzqllmlyf.sHtML

[Q75] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/giwtpvzne.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gsgusqxrh.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fanxiaobao.xyz/Article/details/ggdwgzpjk.sHtML

[Q76] 按天统计
来源：http://read.share.fanxiaobao.xyz/Article/details/gmzgqkpuk.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggpbakduh.sHtML

[Q77] 时间加减
来源：http://wap.fanxiaobao.xyz/Article/details/gnkwlopgd.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzysznbpt.sHtML

[Q78] 当前时间
来源：http://read.share.fanxiaobao.xyz/Article/details/giptokexh.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fanxiaobao.xyz/Article/details/gjdjntljd.sHtML

[Q79] 字符串拼接
来源：http://www.share.fanxiaobao.xyz/Article/details/gghulefsi.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.fanxiaobao.xyz/Article/details/gopnzzqve.sHtML

[Q80] 字符串截取
来源：http://www.blog.fanxiaobao.xyz/Article/details/gswzrqzyt.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmhqfdpfh.sHtML

[Q81] 字符串替换
来源：http://read.share.fanxiaobao.xyz/Article/details/grtcdmvth.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gsqzlsnxj.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gnkrgxtaj.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/guubkwhhu.sHtML

[Q83] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gvpeghoeu.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gsmnxyauf.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fanxiaobao.xyz/Article/details/gytolcewo.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gqnfubbek.sHtML

[Q85] 数值取整
来源：http://wap.fanxiaobao.xyz/Article/details/gtxaaywfv.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.fanxiaobao.xyz/Article/details/gbyyzkaaj.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.fanxiaobao.xyz/Article/details/gmxzmklqb.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fanxiaobao.xyz/Article/details/gxmlepltd.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gzxsdtfia.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfwhiejhq.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fanxiaobao.xyz/Article/details/gjqlyloty.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.fanxiaobao.xyz/Article/details/gwbyavwic.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gqjpukykb.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gldrftjof.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.fanxiaobao.xyz/Article/details/gyqlwunof.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzjbtwqpo.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.fanxiaobao.xyz/Article/details/gzlrsnhfu.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gmmbgosmn.sHtML

R. Bash 专题
来源：http://wap.fanxiaobao.xyz/Article/details/gckxbsaea.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gzyqlkyjv.sHtML

[R01] shebang 与严格模式
来源：http://wap.fanxiaobao.xyz/Article/details/gvtbemnbi.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkoirpkhj.sHtML

set -euo pipefail
来源：http://www.share.fanxiaobao.xyz/Article/details/gobyssaev.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gprvsyziz.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmgpgyjhd.sHtML

[R03] 只读变量
来源：http://3g.fanxiaobao.xyz/Article/details/ghnafqnpc.sHtML

readonly PI=3.14
来源：http://baike.fanxiaobao.xyz/Article/details/gwdfceozk.sHtML

[R04] 位置参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gwnresdjk.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fanxiaobao.xyz/Article/details/gyzwamxez.sHtML

[R05] 参数默认值
来源：http://blog.fanxiaobao.xyz/Article/details/geqxtltua.sHtML

name="${1:-default}"
来源：http://mobile.fanxiaobao.xyz/Article/details/grswbuljd.sHtML

[R06] 判断命令是否存在
来源：http://3g.fanxiaobao.xyz/Article/details/gtzmleabt.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcciexhyy.sHtML

[R07] if 判断文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxkbzimfj.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gfouhmleb.sHtML

[R08] 数值比较
来源：http://baike.fanxiaobao.xyz/Article/details/gqnswuyca.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gpdqkapox.sHtML

[R09] 字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gwozmlhye.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/grilpuqci.sHtML

[R10] 正则匹配
来源：http://blog.fanxiaobao.xyz/Article/details/guhvnyxox.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnllzkogf.sHtML

[R11] case 多分支
来源：http://wap.fanxiaobao.xyz/Article/details/ggobgmvca.sHtML

case "$1" in
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gggrjaiuj.sHtML

start) echo "启动" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gcpzuhjpo.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghnbnowxq.sHtML

*)     echo "未知命令" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gshhxvuln.sHtML

esac
来源：http://m.share.fanxiaobao.xyz/Article/details/guybvbwje.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmlaawanq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/giyeyjrmz.sHtML

[R13] for 计数循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdaleetzh.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gjnytrbuv.sHtML

[R14] C 风格 for
来源：http://baike.fanxiaobao.xyz/Article/details/gsiegemnu.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gyolrhfam.sHtML

[R15] while 逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/geecqyzye.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gegujagdd.sHtML

[R16] until 等待条件
来源：http://wap.fanxiaobao.xyz/Article/details/gnxynmzhc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/grlipllur.sHtML

[R17] 数组定义与取值
来源：http://read.share.fanxiaobao.xyz/Article/details/geymhxaqk.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gzeuybtfw.sHtML

[R18] 遍历数组
来源：http://www.share.fanxiaobao.xyz/Article/details/gqsviyncx.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gboxoqfjy.sHtML

[R19] 数组长度
来源：http://3g.fanxiaobao.xyz/Article/details/gqdkyovin.sHtML

echo "${#arr[@]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gbmqfcuav.sHtML

[R20] 关联数组（字典）
来源：http://wap.fanxiaobao.xyz/Article/details/gpjyufxfj.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gzcqerfco.sHtML

[R21] 字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/guliuwezx.sHtML

echo "${#s}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glhglghso.sHtML

[R22] 截取子串
来源：http://read.share.fanxiaobao.xyz/Article/details/gidptxkwv.sHtML

echo "${s:0:5}"
来源：http://blog.fanxiaobao.xyz/Article/details/gvdrtvqbz.sHtML

[R23] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/gjwezvewh.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fanxiaobao.xyz/Article/details/glkwsnoin.sHtML

[R24] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gvzmzwrdy.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fanxiaobao.xyz/Article/details/guiwjxnhq.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fanxiaobao.xyz/Article/details/gyywzgmuh.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fanxiaobao.xyz/Article/details/ghibzebpx.sHtML

[R26] 命令替换
来源：http://mobile.fanxiaobao.xyz/Article/details/griorvwiv.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fanxiaobao.xyz/Article/details/gjtmjmgsm.sHtML

[R27] 算术展开
来源：http://blog.fanxiaobao.xyz/Article/details/ghdhcdzml.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghytckpio.sHtML

[R28] 浮点运算
来源：http://m.share.fanxiaobao.xyz/Article/details/ghlwgssei.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fanxiaobao.xyz/Article/details/ghbqsyuno.sHtML

[R29] 定义函数
来源：http://wap.fanxiaobao.xyz/Article/details/guefjwffu.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gaiorscfn.sHtML

[R30] 函数返回状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gcbdyiele.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fanxiaobao.xyz/Article/details/gmerlugxz.sHtML

[R31] 局部变量
来源：http://read.share.fanxiaobao.xyz/Article/details/glwzymcao.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gycdfcooh.sHtML

[R32] 参数个数校验
来源：http://blog.fanxiaobao.xyz/Article/details/gfdjszjhk.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gjurmpqoj.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdwidzehm.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fanxiaobao.xyz/Article/details/gkmxvskgu.sHtML

[R34] 退出时清理
来源：http://wap.fanxiaobao.xyz/Article/details/gipjrvarb.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/giuqcgrkq.sHtML

[R35] 后台执行并等待
来源：http://baike.fanxiaobao.xyz/Article/details/guuxklyzy.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gussciuhg.sHtML

[R36] 并发执行多个任务
来源：http://baike.fanxiaobao.xyz/Article/details/gttgrtctd.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fanxiaobao.xyz/Article/details/gfvxwkkcw.sHtML

[R37] 把输出赋给变量
来源：http://3g.fanxiaobao.xyz/Article/details/grmhcrtay.sHtML

files=$(ls -1)
来源：http://wap.fanxiaobao.xyz/Article/details/gmsbxuxxn.sHtML

[R38] 管道串联
来源：http://3g.fanxiaobao.xyz/Article/details/gtxcffkxt.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gfewpdzkj.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzwvmqzly.sHtML

cmd > out.log 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/gqajyxyod.sHtML

[R40] 追加写日志
来源：http://blog.fanxiaobao.xyz/Article/details/grlpuhzwv.sHtML

echo "log" >> out.log
来源：http://www.share.fanxiaobao.xyz/Article/details/ghucwzwlz.sHtML

[R41] 丢弃输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gpnewwmjz.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gklxzonnv.sHtML

[R42] 输入重定向
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grnrtdjgk.sHtML

wc -l < a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gvjvptraa.sHtML

[R43] 按名字查找文件
来源：http://wap.fanxiaobao.xyz/Article/details/gotplbabp.sHtML

find . -name "*.log" -type f
来源：http://baike.fanxiaobao.xyz/Article/details/givriihvy.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gehgreqgc.sHtML

find . -mtime -7 -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/gnuamzzzj.sHtML

[R45] 批量删除
来源：http://read.share.fanxiaobao.xyz/Article/details/gjgaujymu.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fanxiaobao.xyz/Article/details/grpecxudu.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fanxiaobao.xyz/Article/details/gcuarjfmh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fanxiaobao.xyz/Article/details/grlplajau.sHtML

[R47] sed 单行替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqrvdkxmc.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gnnzvppcx.sHtML

[R48] awk 取指定列
来源：http://wap.fanxiaobao.xyz/Article/details/guyvjtgkj.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gaoptokox.sHtML

[R49] awk 带条件
来源：http://3g.fanxiaobao.xyz/Article/details/ggvqlkhip.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fanxiaobao.xyz/Article/details/geccncihn.sHtML

[R50] awk 求和
来源：http://wap.fanxiaobao.xyz/Article/details/gkhkkdcjh.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gacimvsws.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fanxiaobao.xyz/Article/details/gusajkzku.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fanxiaobao.xyz/Article/details/gfuggfasd.sHtML

[R52] 统计行数
来源：http://blog.fanxiaobao.xyz/Article/details/gfecyardd.sHtML

wc -l a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gwoppxjsm.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/gusvywmam.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gccrtyrgg.sHtML

[R54] 比较两个文件
来源：http://blog.fanxiaobao.xyz/Article/details/gsbthfltl.sHtML

diff a.txt b.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gshdtjwla.sHtML

[R55] 压缩与解压
来源：http://wap.fanxiaobao.xyz/Article/details/gglxxbezm.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fanxiaobao.xyz/Article/details/gepuurmwg.sHtML

[R56] 远程拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqajxgbpo.sHtML

scp file user@host:/path/
来源：http://3g.fanxiaobao.xyz/Article/details/gnmxqmzjw.sHtML

[R57] 远程执行命令
来源：http://baike.fanxiaobao.xyz/Article/details/gwbubszzm.sHtML

ssh user@host 'uptime'
来源：http://3g.fanxiaobao.xyz/Article/details/gklktiqod.sHtML

[R58] 下载文件
来源：http://blog.fanxiaobao.xyz/Article/details/gkmsgqueu.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fanxiaobao.xyz/Article/details/gxlozhakw.sHtML

[R59] 发 POST JSON
来源：http://m.share.fanxiaobao.xyz/Article/details/gwcwteguf.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fanxiaobao.xyz/Article/details/gucvknnai.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gjfsddwqq.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fanxiaobao.xyz/Article/details/gbcgaxxon.sHtML

[R61] 磁盘占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gifhiskrs.sHtML

df -h;  du -sh *
来源：http://3g.fanxiaobao.xyz/Article/details/gulxkrnvs.sHtML

[R62] 找最占空间的文件
来源：http://baike.fanxiaobao.xyz/Article/details/grxxssdah.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fanxiaobao.xyz/Article/details/gtcbkbrgm.sHtML

[R63] 内存与进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghzcuenfg.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvvvftskj.sHtML

[R64] 结束进程
来源：http://mobile.fanxiaobao.xyz/Article/details/ggbcmidtv.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fanxiaobao.xyz/Article/details/gykruivph.sHtML

[R65] 查看端口占用
来源：http://blog.fanxiaobao.xyz/Article/details/gltjkeauc.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fanxiaobao.xyz/Article/details/gkrmytpqd.sHtML

[R66] 定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/gctundceg.sHtML

crontab -e;  crontab -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gdvseelwu.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fanxiaobao.xyz/Article/details/ggarfgjcl.sHtML

openssl rand -hex 16
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdipahsyo.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcpwukoas.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gqjxaoxfj.sHtML

[R69] 生成随机密码
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghgmzemnj.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fanxiaobao.xyz/Article/details/ghsrzweoo.sHtML

[R70] 时间戳与互转
来源：http://wap.fanxiaobao.xyz/Article/details/gvpvyfutn.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fanxiaobao.xyz/Article/details/gmchiurfu.sHtML

[R71] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gbzmgwrbu.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fanxiaobao.xyz/Article/details/gewojcjuu.sHtML

[R72] 等待端口就绪
来源：http://www.share.fanxiaobao.xyz/Article/details/gvplhnnso.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/ggonfcbhg.sHtML

[R73] 分割大日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwyivlqdl.sHtML

split -l 1000 big.log part_
来源：http://3g.fanxiaobao.xyz/Article/details/gzkkkjxrn.sHtML

[R74] 批量重命名
来源：http://m.share.fanxiaobao.xyz/Article/details/guqikdfol.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gskeijnon.sHtML

[R75] 导出环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/gzznnrrdx.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fanxiaobao.xyz/Article/details/gspozkmuv.sHtML

[R76] 使用临时文件
来源：http://www.share.fanxiaobao.xyz/Article/details/ghlibfvvn.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpcwgbyui.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzvorgevv.sHtML

read -rp "请输入: " ans
来源：http://m.share.fanxiaobao.xyz/Article/details/ghblxrfuu.sHtML

[R78] 交互式菜单
来源：http://baike.fanxiaobao.xyz/Article/details/gntwrudro.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gdsnchxhl.sHtML

[R79] 解析命令行选项
来源：http://mobile.fanxiaobao.xyz/Article/details/gmogviadt.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fanxiaobao.xyz/Article/details/gvdlwgfom.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fanxiaobao.xyz/Article/details/grzryzwgf.sHtML

time ./run.sh
来源：http://3g.fanxiaobao.xyz/Article/details/gidtxaaah.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gssimlgun.sHtML

S. C / C++ 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goovsjiqx.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gzzvfomxr.sHtML

[S01] C：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/glzplfpld.sHtML

#include <stdio.h>
来源：http://www.share.fanxiaobao.xyz/Article/details/gjbtxbfjf.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gumvasfzx.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gmjqmtpoq.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gruxzcusx.sHtML

[S03] C：读入整数
来源：http://mobile.fanxiaobao.xyz/Article/details/gvoldrbbi.sHtML

int x; scanf("%d", &x);
来源：http://wap.fanxiaobao.xyz/Article/details/gssbxojtx.sHtML

[S04] C：字符串复制
来源：http://blog.fanxiaobao.xyz/Article/details/glsvjdkid.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fanxiaobao.xyz/Article/details/ggyhcrhqe.sHtML

[S05] C：字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gvqahaiei.sHtML

strlen(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gsicasdss.sHtML

[S06] C：字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/glyzgdenb.sHtML

strcmp(a, b) == 0
来源：http://wap.fanxiaobao.xyz/Article/details/ghtuyrahk.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjsqmafbb.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wap.fanxiaobao.xyz/Article/details/gejyqjbkm.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fanxiaobao.xyz/Article/details/ggydagqne.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjpixtzdh.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fanxiaobao.xyz/Article/details/gyzzyoogd.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fanxiaobao.xyz/Article/details/gcujqopro.sHtML

[S10] C：指针与解引用
来源：http://baike.fanxiaobao.xyz/Article/details/gybwbxhbj.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpurnzmxz.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnempooah.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzoqcvhou.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gturhnjbp.sHtML

fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gscvmqnyb.sHtML

[S12] C：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gniwfsqat.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/ggtkfyvge.sHtML

[S13] C：宏定义
来源：http://m.share.fanxiaobao.xyz/Article/details/gxgfvhmll.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fanxiaobao.xyz/Article/details/gzokwrpxd.sHtML

[S14] C：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkzbrbwwo.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fanxiaobao.xyz/Article/details/gdnydlmcs.sHtML

[S15] C：类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gplcryiqj.sHtML

(double) a / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/giufppcnf.sHtML

[S16] C：位操作置位
来源：http://m.share.fanxiaobao.xyz/Article/details/gjgxeocur.sHtML

x |= (1 << 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gowfkhdfe.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gotygxbpx.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fanxiaobao.xyz/Article/details/gupybpdup.sHtML

[S18] C：命令行参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gjnacvffn.sHtML

int main(int argc, char **argv)
来源：http://3g.fanxiaobao.xyz/Article/details/gfogtucbw.sHtML

[S19] C：快速排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gyznlcziz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gkclpktkh.sHtML

[S20] C：二分查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gsyrjgtit.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gdidqaqra.sHtML

[S21] C：字符类别判断
来源：http://blog.fanxiaobao.xyz/Article/details/gyjynxhph.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gacfpqjwo.sHtML

[S22] C：字符串转数字
来源：http://3g.fanxiaobao.xyz/Article/details/gtpcugsnh.sHtML


<!-- 参考信息 -->