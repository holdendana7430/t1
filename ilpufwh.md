代发 wailian999

[Q44] IN 子查询
来源：http://m.share.hesvh.cn/Article/details/gszmswvga.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.zdbjq.cn/Article/details/gnxxpuxfy.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.hesvh.cn/Article/details/gnfwaiakm.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fehbvm.com/Article/details/gmfdhheqw.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.hesvh.cn/Article/details/gvuzwzvbh.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fehbvm.com/Article/details/gehqcoszt.sHtML

[Q47] 与平均值比较
来源：http://baike.zdbjq.cn/Article/details/gwljcuwcg.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.zdbjq.cn/Article/details/gfoioeqhm.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.zdbjq.cn/Article/details/gvqfdtjzy.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.fehbvm.com/Article/details/gicqzlbbl.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.zdbjq.cn/Article/details/gicfgmpks.sHtML

[Q49] 更新单行
来源：http://read.share.hesvh.cn/Article/details/gilascqvz.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.zdbjq.cn/Article/details/gnowwivqw.sHtML

[Q50] 批量更新
来源：http://m.share.fehbvm.com/Article/details/guusjjkxo.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.fehbvm.com/Article/details/glzoswjxp.sHtML

[Q51] 用子查询更新
来源：http://m.share.zdbjq.cn/Article/details/gmrbtozzo.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.zdbjq.cn/Article/details/gihgycxnm.sHtML

[Q52] 删除指定行
来源：http://wap.fehbvm.com/Article/details/ganneqkgq.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.hesvh.cn/Article/details/gckdarmjt.sHtML

[Q53] 按条件删除
来源：http://baike.zdbjq.cn/Article/details/gylwqlrxo.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.hesvh.cn/Article/details/gqhvutpuc.sHtML

[Q54] 清空表
来源：http://mobile.zdbjq.cn/Article/details/gsbiuszlb.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fehbvm.com/Article/details/gfwagvyti.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.hesvh.cn/Article/details/gsbxndfhd.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.zdbjq.cn/Article/details/gpmqmykau.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.fehbvm.com/Article/details/gdoijjvhx.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.zdbjq.cn/Article/details/gzrkmxrzf.sHtML

[Q57] 行号
来源：http://read.share.fehbvm.com/Article/details/giribrqte.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gclplujqf.sHtML

[Q58] 累计求和
来源：http://3g.zdbjq.cn/Article/details/gxpbyxfld.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/ggslxaaqn.sHtML

[Q59] 分组内累计
来源：http://baike.hesvh.cn/Article/details/gtxskljmu.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gptkdpeip.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.hesvh.cn/Article/details/gplomzahz.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.hesvh.cn/Article/details/gcwbktsjk.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gulukltaw.sHtML

[Q61] 移动平均
来源：http://mobile.zdbjq.cn/Article/details/guqgvelpb.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gutyaievw.sHtML

[Q62] 分组占比
来源：http://m.share.fehbvm.com/Article/details/gshmtrmsg.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/ggzggifon.sHtML

[Q63] 开启事务
来源：http://www.share.zdbjq.cn/Article/details/gkbvwukuv.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.hesvh.cn/Article/details/gdbjzgedo.sHtML

[Q64] 提交事务
来源：http://blog.hesvh.cn/Article/details/gqyciklwg.sHtML

COMMIT;
来源：http://www.m.share.zdbjq.cn/Article/details/gfpwxbcyz.sHtML

[Q65] 回滚事务
来源：http://baike.zdbjq.cn/Article/details/gohulihoi.sHtML

ROLLBACK;
来源：http://blog.hesvh.cn/Article/details/gtuzkqdcb.sHtML

[Q66] 行锁查询
来源：http://www.m.share.hesvh.cn/Article/details/giemgrtzq.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.hesvh.cn/Article/details/ghsajyeti.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.hesvh.cn/Article/details/grfbanjlf.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.zdbjq.cn/Article/details/gbclphdpo.sHtML

[Q68] 保存点
来源：http://www.m.share.hesvh.cn/Article/details/gaivbaywz.sHtML

SAVEPOINT sp1;
来源：http://read.share.hesvh.cn/Article/details/gsegpalxj.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.zdbjq.cn/Article/details/gemosmpdv.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.hesvh.cn/Article/details/guqtxkrne.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.hesvh.cn/Article/details/gaueetwns.sHtML

[Q70] 更新统计信息
来源：http://blog.hesvh.cn/Article/details/ggwugqlsh.sHtML

ANALYZE TABLE users;
来源：http://m.share.zdbjq.cn/Article/details/gqzgzbuhh.sHtML

[Q71] 查看建表语句
来源：http://www.share.zdbjq.cn/Article/details/gesimxxuz.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.fehbvm.com/Article/details/gzaorqygz.sHtML

[Q72] 查看索引
来源：http://baike.fehbvm.com/Article/details/gkljyvctv.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.hesvh.cn/Article/details/galhvadyu.sHtML

[Q73] 查看表状态
来源：http://m.share.hesvh.cn/Article/details/gdjimmqhd.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.hesvh.cn/Article/details/geiaxbznu.sHtML

[Q74] 强制使用索引
来源：http://m.share.zdbjq.cn/Article/details/gymrbaupl.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.fehbvm.com/Article/details/givaocbnt.sHtML

[Q75] 日期格式化
来源：http://m.share.hesvh.cn/Article/details/gicepeolx.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.hesvh.cn/Article/details/gsrnvnrqo.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.zdbjq.cn/Article/details/ggzyeerej.sHtML

[Q76] 按天统计
来源：http://blog.hesvh.cn/Article/details/gsafhkjox.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.zdbjq.cn/Article/details/gvcvdycfi.sHtML

[Q77] 时间加减
来源：http://read.share.zdbjq.cn/Article/details/gzdsdruij.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.zdbjq.cn/Article/details/gfeyohsoa.sHtML

[Q78] 当前时间
来源：http://read.share.fehbvm.com/Article/details/guqbdcqtl.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.fehbvm.com/Article/details/gpjevwafc.sHtML

[Q79] 字符串拼接
来源：http://www.blog.fehbvm.com/Article/details/gocbirkmg.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.zdbjq.cn/Article/details/gqzeypuvk.sHtML

[Q80] 字符串截取
来源：http://www.m.share.zdbjq.cn/Article/details/gaymjhodt.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.fehbvm.com/Article/details/getndbicm.sHtML

[Q81] 字符串替换
来源：http://www.blog.hesvh.cn/Article/details/glgmpkexu.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.hesvh.cn/Article/details/grmkxqozh.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fehbvm.com/Article/details/gkkggxewn.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gdgdjlsli.sHtML

[Q83] 大小写转换
来源：http://www.blog.zdbjq.cn/Article/details/goapmmwod.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gsszpgiis.sHtML

[Q84] 去除首尾空格
来源：http://read.share.zdbjq.cn/Article/details/gercptrkz.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gspfbjaik.sHtML

[Q85] 数值取整
来源：http://www.blog.zdbjq.cn/Article/details/gxotyeash.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.fehbvm.com/Article/details/gvcavbvcx.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.hesvh.cn/Article/details/gvpwohwjj.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.zdbjq.cn/Article/details/gixgftpjs.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fehbvm.com/Article/details/gznuxzfru.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.fehbvm.com/Article/details/gcfuqxfsk.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.zdbjq.cn/Article/details/gxdbhxxcd.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.hesvh.cn/Article/details/gbaukgwsf.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.hesvh.cn/Article/details/gmccbsgin.sHtML

[Q89] 判断表是否存在
来源：http://m.share.hesvh.cn/Article/details/gcshocygn.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.hesvh.cn/Article/details/giiskvfoi.sHtML

[Q90] 生成序号列
来源：http://www.share.zdbjq.cn/Article/details/gobwmscuc.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.hesvh.cn/Article/details/gagylrplj.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/glkbgnfbl.sHtML

R. Bash 专题
来源：http://www.share.hesvh.cn/Article/details/guhjcihdg.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gwowlkfjs.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fehbvm.com/Article/details/gwvcogdgd.sHtML

#!/usr/bin/env bash
来源：http://www.blog.zdbjq.cn/Article/details/gxwtcsbhv.sHtML

set -euo pipefail
来源：http://blog.zdbjq.cn/Article/details/gnczlxfuk.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.hesvh.cn/Article/details/gznrygvrq.sHtML

name="Tom"; echo "$name"
来源：http://blog.hesvh.cn/Article/details/gnwkxoqfg.sHtML

[R03] 只读变量
来源：http://read.share.hesvh.cn/Article/details/grxiskvua.sHtML

readonly PI=3.14
来源：http://www.m.share.zdbjq.cn/Article/details/gsbugmvun.sHtML

[R04] 位置参数
来源：http://www.m.share.fehbvm.com/Article/details/geiqisvaj.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.fehbvm.com/Article/details/gfhwlqnfk.sHtML

[R05] 参数默认值
来源：http://www.share.hesvh.cn/Article/details/gghtclpdb.sHtML

name="${1:-default}"
来源：http://www.share.fehbvm.com/Article/details/gmtwqanwb.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fehbvm.com/Article/details/ggitwhbjn.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.zdbjq.cn/Article/details/guyfnjgtc.sHtML

[R07] if 判断文件
来源：http://www.share.hesvh.cn/Article/details/gqsdjctfq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.hesvh.cn/Article/details/gdfoitnlo.sHtML

[R08] 数值比较
来源：http://www.share.zdbjq.cn/Article/details/gtyconiqg.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fehbvm.com/Article/details/goynunlsl.sHtML

[R09] 字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/gjltjuzzg.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.hesvh.cn/Article/details/gjnwubmpf.sHtML

[R10] 正则匹配
来源：http://www.m.share.zdbjq.cn/Article/details/guodnzzpl.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.zdbjq.cn/Article/details/gltgzbdal.sHtML

[R11] case 多分支
来源：http://www.m.share.hesvh.cn/Article/details/gnmqogtnf.sHtML

case "$1" in
来源：http://m.share.fehbvm.com/Article/details/gvqoewsnt.sHtML

start) echo "启动" ;;
来源：http://read.share.fehbvm.com/Article/details/gazjsoozy.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gqevqcnco.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gqnyqdnzi.sHtML

esac
来源：http://read.share.fehbvm.com/Article/details/gobirvyvh.sHtML

[R12] for 遍历文件
来源：http://mobile.zdbjq.cn/Article/details/gbpsdmjal.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.zdbjq.cn/Article/details/glrmaascy.sHtML

[R13] for 计数循环
来源：http://wap.zdbjq.cn/Article/details/goxirixpo.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fehbvm.com/Article/details/ggziemslm.sHtML

[R14] C 风格 for
来源：http://blog.fehbvm.com/Article/details/gkoecupai.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.hesvh.cn/Article/details/ggqovwasq.sHtML

[R15] while 逐行读文件
来源：http://read.share.fehbvm.com/Article/details/gjjbrcczr.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.hesvh.cn/Article/details/gkgmhsqmk.sHtML

[R16] until 等待条件
来源：http://www.share.zdbjq.cn/Article/details/gfmaivixo.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.hesvh.cn/Article/details/gbxvynluj.sHtML

[R17] 数组定义与取值
来源：http://blog.zdbjq.cn/Article/details/gxhxcgopf.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.hesvh.cn/Article/details/guyfleodw.sHtML

[R18] 遍历数组
来源：http://blog.fehbvm.com/Article/details/gpzyrtyjz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.zdbjq.cn/Article/details/gtesmypea.sHtML

[R19] 数组长度
来源：http://www.m.share.zdbjq.cn/Article/details/gwddypiin.sHtML

echo "${#arr[@]}"
来源：http://www.blog.zdbjq.cn/Article/details/gklwwohlz.sHtML

[R20] 关联数组（字典）
来源：http://3g.zdbjq.cn/Article/details/gyilxsxtq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.zdbjq.cn/Article/details/gtxzxkaon.sHtML

[R21] 字符串长度
来源：http://www.m.share.fehbvm.com/Article/details/ggbwyjuiv.sHtML

echo "${#s}"
来源：http://read.share.fehbvm.com/Article/details/gkpkkaikb.sHtML

[R22] 截取子串
来源：http://baike.hesvh.cn/Article/details/gaztuqjxm.sHtML

echo "${s:0:5}"
来源：http://www.m.share.zdbjq.cn/Article/details/ghxmpvojz.sHtML

[R23] 字符串替换
来源：http://blog.fehbvm.com/Article/details/gevprfrli.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.zdbjq.cn/Article/details/glecedkhz.sHtML

[R24] 大小写转换
来源：http://www.blog.fehbvm.com/Article/details/glhmouuzh.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fehbvm.com/Article/details/gbtligbmg.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.zdbjq.cn/Article/details/gjchjieel.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fehbvm.com/Article/details/gtoxuckkt.sHtML

[R26] 命令替换
来源：http://3g.fehbvm.com/Article/details/gtrlheiuk.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fehbvm.com/Article/details/gltkzncwm.sHtML

[R27] 算术展开
来源：http://read.share.hesvh.cn/Article/details/giidkjbea.sHtML

echo $((1 + 2 * 3))
来源：http://wap.zdbjq.cn/Article/details/grqdadzhv.sHtML

[R28] 浮点运算
来源：http://www.blog.hesvh.cn/Article/details/glhigbwoi.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.hesvh.cn/Article/details/gregjhzdi.sHtML

[R29] 定义函数
来源：http://baike.fehbvm.com/Article/details/glylghfuz.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fehbvm.com/Article/details/gyajbxhix.sHtML

[R30] 函数返回状态码
来源：http://baike.zdbjq.cn/Article/details/gowbjjgwv.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.zdbjq.cn/Article/details/gusddgrfq.sHtML

[R31] 局部变量
来源：http://baike.hesvh.cn/Article/details/gkcghzksj.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.zdbjq.cn/Article/details/gducsldgy.sHtML

[R32] 参数个数校验
来源：http://mobile.hesvh.cn/Article/details/gjqqquqzx.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fehbvm.com/Article/details/gengvvpsj.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fehbvm.com/Article/details/gjunblflb.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fehbvm.com/Article/details/gbdhpyvuo.sHtML

[R34] 退出时清理
来源：http://m.share.zdbjq.cn/Article/details/gzokvxoft.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.zdbjq.cn/Article/details/gxyrmkbxp.sHtML

[R35] 后台执行并等待
来源：http://blog.hesvh.cn/Article/details/gvqzuwfsd.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fehbvm.com/Article/details/gxlzckqxv.sHtML

[R36] 并发执行多个任务
来源：http://baike.zdbjq.cn/Article/details/gpivatknz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.zdbjq.cn/Article/details/gofmsewal.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fehbvm.com/Article/details/glhcamavb.sHtML

files=$(ls -1)
来源：http://mobile.fehbvm.com/Article/details/gelrlbpia.sHtML

[R38] 管道串联
来源：http://baike.hesvh.cn/Article/details/gnurstbil.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.hesvh.cn/Article/details/gcelllabg.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fehbvm.com/Article/details/gdvkwyphu.sHtML

cmd > out.log 2>&1
来源：http://blog.zdbjq.cn/Article/details/gtrkweymp.sHtML

[R40] 追加写日志
来源：http://blog.fehbvm.com/Article/details/gyxauisar.sHtML

echo "log" >> out.log
来源：http://baike.fehbvm.com/Article/details/gytuoonht.sHtML

[R41] 丢弃输出
来源：http://m.share.hesvh.cn/Article/details/gxcfhopdg.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fehbvm.com/Article/details/gfftjjkna.sHtML

[R42] 输入重定向
来源：http://m.share.zdbjq.cn/Article/details/gzxaysdnp.sHtML

wc -l < a.txt
来源：http://3g.fehbvm.com/Article/details/gwavvupel.sHtML

[R43] 按名字查找文件
来源：http://baike.zdbjq.cn/Article/details/giheiefwr.sHtML

find . -name "*.log" -type f
来源：http://baike.fehbvm.com/Article/details/gwuyryshn.sHtML

[R44] 按修改时间查找
来源：http://baike.hesvh.cn/Article/details/gejshgoiq.sHtML

find . -mtime -7 -type f
来源：http://baike.hesvh.cn/Article/details/gxrhzocgc.sHtML

[R45] 批量删除
来源：http://www.m.share.hesvh.cn/Article/details/giqxvybdf.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fehbvm.com/Article/details/gecezwrix.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fehbvm.com/Article/details/gchsbvcpu.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fehbvm.com/Article/details/gkhsrhcan.sHtML

[R47] sed 单行替换
来源：http://read.share.zdbjq.cn/Article/details/guthwimtd.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.hesvh.cn/Article/details/gkchuvomi.sHtML

[R48] awk 取指定列
来源：http://wap.fehbvm.com/Article/details/ghmymzgbf.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gfirtvbbk.sHtML

[R49] awk 带条件
来源：http://blog.zdbjq.cn/Article/details/gycynzbkr.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fehbvm.com/Article/details/gtvhtrhgh.sHtML

[R50] awk 求和
来源：http://m.share.hesvh.cn/Article/details/gudutpvhy.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.zdbjq.cn/Article/details/gwizxbtsj.sHtML

[R51] 排序去重取前几
来源：http://www.blog.zdbjq.cn/Article/details/grjmsjbkw.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.zdbjq.cn/Article/details/gzpgraqoc.sHtML

[R52] 统计行数
来源：http://read.share.fehbvm.com/Article/details/gmpqrjbjc.sHtML

wc -l a.txt
来源：http://wap.zdbjq.cn/Article/details/grpluqbuc.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fehbvm.com/Article/details/gcxhmpcwg.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fehbvm.com/Article/details/gktbxgqed.sHtML

[R54] 比较两个文件
来源：http://blog.hesvh.cn/Article/details/gdmgutagl.sHtML

diff a.txt b.txt
来源：http://3g.zdbjq.cn/Article/details/gowhxtwyg.sHtML

[R55] 压缩与解压
来源：http://blog.fehbvm.com/Article/details/gingsbuba.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.hesvh.cn/Article/details/gafenekau.sHtML

[R56] 远程拷贝
来源：http://baike.fehbvm.com/Article/details/gwdchpinv.sHtML

scp file user@host:/path/
来源：http://baike.zdbjq.cn/Article/details/gbbvsvuip.sHtML

[R57] 远程执行命令
来源：http://blog.hesvh.cn/Article/details/gidrhdtlf.sHtML

ssh user@host 'uptime'
来源：http://baike.hesvh.cn/Article/details/gaveeldbg.sHtML

[R58] 下载文件
来源：http://blog.hesvh.cn/Article/details/gvtrbphuc.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fehbvm.com/Article/details/gginbbiem.sHtML

[R59] 发 POST JSON
来源：http://mobile.hesvh.cn/Article/details/gdvjmeaip.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.hesvh.cn/Article/details/gzrnfjodm.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.zdbjq.cn/Article/details/gezlfimvm.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.zdbjq.cn/Article/details/gowgrbbfm.sHtML

[R61] 磁盘占用
来源：http://m.share.fehbvm.com/Article/details/gejmysqor.sHtML

df -h;  du -sh *
来源：http://read.share.hesvh.cn/Article/details/gsaeowwvq.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fehbvm.com/Article/details/gocznffmt.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fehbvm.com/Article/details/gluwrxzpj.sHtML

[R63] 内存与进程
来源：http://read.share.zdbjq.cn/Article/details/gzglupmdw.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.hesvh.cn/Article/details/gjntbfoes.sHtML

[R64] 结束进程
来源：http://baike.hesvh.cn/Article/details/gzrfftxxu.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.hesvh.cn/Article/details/gnnsphdhi.sHtML

[R65] 查看端口占用
来源：http://wap.hesvh.cn/Article/details/gwgthjvyj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.hesvh.cn/Article/details/gwppdmllq.sHtML

[R66] 定时任务
来源：http://3g.hesvh.cn/Article/details/gunkbcawh.sHtML

crontab -e;  crontab -l
来源：http://mobile.zdbjq.cn/Article/details/grikqgkuu.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.hesvh.cn/Article/details/gvbjuucne.sHtML

openssl rand -hex 16
来源：http://3g.hesvh.cn/Article/details/gvwbiakqk.sHtML

[R68] 计算文件校验值
来源：http://mobile.zdbjq.cn/Article/details/gxzirkrpo.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.zdbjq.cn/Article/details/gvpiqqdit.sHtML

[R69] 生成随机密码
来源：http://m.share.fehbvm.com/Article/details/ghdrcmauf.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.hesvh.cn/Article/details/gvrttnhdy.sHtML

[R70] 时间戳与互转
来源：http://read.share.zdbjq.cn/Article/details/gjpjnaidf.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fehbvm.com/Article/details/gkwoulzav.sHtML

[R71] 日期格式化
来源：http://baike.zdbjq.cn/Article/details/gaebwklmu.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.zdbjq.cn/Article/details/gyvkqpypt.sHtML

[R72] 等待端口就绪
来源：http://baike.zdbjq.cn/Article/details/gbwxohoby.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/golhykejj.sHtML

[R73] 分割大日志
来源：http://read.share.hesvh.cn/Article/details/glelaczfe.sHtML

split -l 1000 big.log part_
来源：http://blog.hesvh.cn/Article/details/gurvzrlno.sHtML

[R74] 批量重命名
来源：http://wap.zdbjq.cn/Article/details/gsfzqewfo.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.hesvh.cn/Article/details/gkwwzdmoe.sHtML

[R75] 导出环境变量
来源：http://www.blog.zdbjq.cn/Article/details/genmezhsj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.hesvh.cn/Article/details/gmtawqtaa.sHtML

[R76] 使用临时文件
来源：http://read.share.fehbvm.com/Article/details/gdcveyljh.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.zdbjq.cn/Article/details/glseurvix.sHtML

[R77] 读取用户输入
来源：http://www.blog.hesvh.cn/Article/details/gqmtuozeu.sHtML

read -rp "请输入: " ans
来源：http://wap.hesvh.cn/Article/details/ghulzsnza.sHtML

[R78] 交互式菜单
来源：http://www.share.hesvh.cn/Article/details/gobcbjril.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.zdbjq.cn/Article/details/gcubztqph.sHtML

[R79] 解析命令行选项
来源：http://3g.hesvh.cn/Article/details/gjimxpxyj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.hesvh.cn/Article/details/gxknakuch.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fehbvm.com/Article/details/gdrtehhtv.sHtML

time ./run.sh
来源：http://www.share.hesvh.cn/Article/details/gknzetvyu.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gynfjknuf.sHtML

S. C / C++ 专题
来源：http://www.blog.hesvh.cn/Article/details/giqaknwhp.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gqisacsob.sHtML

[S01] C：Hello World
来源：http://baike.zdbjq.cn/Article/details/gcukesfgf.sHtML

#include <stdio.h>
来源：http://www.share.zdbjq.cn/Article/details/gryjomqeq.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.zdbjq.cn/Article/details/gmnupqpcz.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.zdbjq.cn/Article/details/geuxtmwkw.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.hesvh.cn/Article/details/grnniqcyj.sHtML

[S03] C：读入整数
来源：http://3g.hesvh.cn/Article/details/gxxqgffct.sHtML

int x; scanf("%d", &x);
来源：http://m.share.zdbjq.cn/Article/details/gkzvdthce.sHtML

[S04] C：字符串复制
来源：http://blog.fehbvm.com/Article/details/gjmssjkwr.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.zdbjq.cn/Article/details/gqdmtckpz.sHtML

[S05] C：字符串长度
来源：http://wap.hesvh.cn/Article/details/gkmvbvzvc.sHtML

strlen(s)
来源：http://www.m.share.zdbjq.cn/Article/details/giiheszaa.sHtML

[S06] C：字符串比较
来源：http://blog.fehbvm.com/Article/details/gdmninivr.sHtML

strcmp(a, b) == 0
来源：http://mobile.hesvh.cn/Article/details/gqseqxlly.sHtML

[S07] C：数组遍历求和
来源：http://baike.fehbvm.com/Article/details/gmbebhcsn.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.zdbjq.cn/Article/details/ghyzgedyc.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fehbvm.com/Article/details/gbnulcodv.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.zdbjq.cn/Article/details/gbuedfago.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fehbvm.com/Article/details/gyubapjzm.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.zdbjq.cn/Article/details/gtmuymdpk.sHtML

[S10] C：指针与解引用
来源：http://www.blog.hesvh.cn/Article/details/gjauqmjko.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fehbvm.com/Article/details/gzavyuuzm.sHtML

[S11] C：逐行读文件
来源：http://3g.hesvh.cn/Article/details/giikocmhs.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.hesvh.cn/Article/details/gbvrpsfbm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.hesvh.cn/Article/details/gykjvxjfw.sHtML

fclose(f);
来源：http://www.share.fehbvm.com/Article/details/gaymrkstf.sHtML

[S12] C：写文件
来源：http://www.blog.hesvh.cn/Article/details/gyhcmjvkr.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.hesvh.cn/Article/details/gkixctziy.sHtML

[S13] C：宏定义
来源：http://blog.zdbjq.cn/Article/details/gultgwkne.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.hesvh.cn/Article/details/gbdmfkjln.sHtML

[S14] C：枚举
来源：http://m.share.zdbjq.cn/Article/details/gnctrgrxu.sHtML


<!-- 参考信息 -->