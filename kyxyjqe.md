代发 wailian999

[Q33] 多列分组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxnpjicio.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.fanxiaobao.xyz/Article/details/gtpanvgfv.sHtML

[Q34] 每组取第一条
来源：http://mobile.fanxiaobao.xyz/Article/details/gwdkpnqlg.sHtML

SELECT * FROM (
来源：http://3g.fanxiaobao.xyz/Article/details/gtnkbosaf.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.fanxiaobao.xyz/Article/details/gdozzjlni.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfxdmjjve.sHtML

[Q35] 内连接
来源：http://wap.fanxiaobao.xyz/Article/details/gvaucybbk.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkrzkfohp.sHtML

[Q36] 左连接
来源：http://baike.fanxiaobao.xyz/Article/details/grtjtszvv.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggcgbpadv.sHtML

[Q37] 右连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gsmynqhdx.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gauadzlnb.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.fanxiaobao.xyz/Article/details/gpvtbnmms.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwtmnjfcf.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaorezpvt.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.fanxiaobao.xyz/Article/details/gztxbgopv.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcovcfoxa.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbuqqqlrd.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjybpgxyx.sHtML

[Q41] 多表连接
来源：http://wap.fanxiaobao.xyz/Article/details/govggcmzd.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcvbafkal.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.fanxiaobao.xyz/Article/details/gmbwprmpu.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.fanxiaobao.xyz/Article/details/gjvvktraq.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.fanxiaobao.xyz/Article/details/glmeguzfw.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.fanxiaobao.xyz/Article/details/gigkvurga.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.fanxiaobao.xyz/Article/details/gtomolhln.sHtML

[Q43] 标量子查询
来源：http://blog.fanxiaobao.xyz/Article/details/gxwlcvvke.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvdwqvpfv.sHtML

[Q44] IN 子查询
来源：http://wap.fanxiaobao.xyz/Article/details/gegmvywbr.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.fanxiaobao.xyz/Article/details/gmlnqigks.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.fanxiaobao.xyz/Article/details/guykpofsn.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjzqvtkwr.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gjialsasz.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fanxiaobao.xyz/Article/details/gvylpdnpt.sHtML

[Q47] 与平均值比较
来源：http://3g.fanxiaobao.xyz/Article/details/ghxasescd.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.fanxiaobao.xyz/Article/details/glriuwpec.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyrvkfcin.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtyarirty.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.fanxiaobao.xyz/Article/details/gbvedgdpw.sHtML

[Q49] 更新单行
来源：http://wap.fanxiaobao.xyz/Article/details/gexbzqnke.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/giqpkuvrr.sHtML

[Q50] 批量更新
来源：http://mobile.fanxiaobao.xyz/Article/details/gbtwgceoy.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.fanxiaobao.xyz/Article/details/gqmvzpvmy.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqcrqwsak.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gyhcjvujv.sHtML

[Q52] 删除指定行
来源：http://baike.fanxiaobao.xyz/Article/details/gpelnxlet.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gumofuxqj.sHtML

[Q53] 按条件删除
来源：http://read.share.fanxiaobao.xyz/Article/details/gbifwcvcj.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.fanxiaobao.xyz/Article/details/gzuaiecdt.sHtML

[Q54] 清空表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsnkreqgw.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.fanxiaobao.xyz/Article/details/gfipcbnam.sHtML

[Q55] 排名（并列占位）
来源：http://3g.fanxiaobao.xyz/Article/details/gidakkbih.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.fanxiaobao.xyz/Article/details/gazdztjfi.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.fanxiaobao.xyz/Article/details/gjwtfwrqe.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.fanxiaobao.xyz/Article/details/gnqzadqpr.sHtML

[Q57] 行号
来源：http://3g.fanxiaobao.xyz/Article/details/grmtirejp.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzdqnqzbp.sHtML

[Q58] 累计求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gskptkjmi.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/gwljsgkqi.sHtML

[Q59] 分组内累计
来源：http://3g.fanxiaobao.xyz/Article/details/gvzonehdg.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gnlvxohit.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.fanxiaobao.xyz/Article/details/gppdwwhzt.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fanxiaobao.xyz/Article/details/guurqnaxy.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtajlqtgn.sHtML

[Q61] 移动平均
来源：http://baike.fanxiaobao.xyz/Article/details/gupqbvjfm.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtjunlrxd.sHtML

[Q62] 分组占比
来源：http://3g.fanxiaobao.xyz/Article/details/gkaridflr.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcyyejmmb.sHtML

[Q63] 开启事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gkqrfjxjz.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.fanxiaobao.xyz/Article/details/gelsjbens.sHtML

[Q64] 提交事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gtwwplihp.sHtML

COMMIT;
来源：http://read.share.fanxiaobao.xyz/Article/details/grggdoyld.sHtML

[Q65] 回滚事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gdetmlvqk.sHtML

ROLLBACK;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghviohypw.sHtML

[Q66] 行锁查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gfiekakio.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.fanxiaobao.xyz/Article/details/gkpsbhdwn.sHtML

[Q67] 设置隔离级别
来源：http://www.share.fanxiaobao.xyz/Article/details/gpvvoohcp.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.fanxiaobao.xyz/Article/details/gddvemsrw.sHtML

[Q68] 保存点
来源：http://baike.fanxiaobao.xyz/Article/details/govrwnnmt.sHtML

SAVEPOINT sp1;
来源：http://3g.fanxiaobao.xyz/Article/details/gqjxainet.sHtML

ROLLBACK TO sp1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwmjxspeo.sHtML

[Q69] 查看执行计划
来源：http://baike.fanxiaobao.xyz/Article/details/glkpcjfiu.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.fanxiaobao.xyz/Article/details/gnthruhsn.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gicknstjm.sHtML

ANALYZE TABLE users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpimordgj.sHtML

[Q71] 查看建表语句
来源：http://read.share.fanxiaobao.xyz/Article/details/gbvhgawgq.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gijzjggfi.sHtML

[Q72] 查看索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gayznlmhq.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdscejxwe.sHtML

[Q73] 查看表状态
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyxefufkm.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.fanxiaobao.xyz/Article/details/gyohwbisi.sHtML

[Q74] 强制使用索引
来源：http://blog.fanxiaobao.xyz/Article/details/gecreorlp.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.fanxiaobao.xyz/Article/details/gmsygrukd.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpcucrmhy.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtqhdmens.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.fanxiaobao.xyz/Article/details/gflhjcyjq.sHtML

[Q76] 按天统计
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtasnnjcb.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.fanxiaobao.xyz/Article/details/gksjushpu.sHtML

[Q77] 时间加减
来源：http://blog.fanxiaobao.xyz/Article/details/gwpkzpljr.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.fanxiaobao.xyz/Article/details/gyrlznfbi.sHtML

[Q78] 当前时间
来源：http://m.share.fanxiaobao.xyz/Article/details/guqirilwp.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fanxiaobao.xyz/Article/details/gesmwrbrh.sHtML

[Q79] 字符串拼接
来源：http://wap.fanxiaobao.xyz/Article/details/gfyaumokr.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyngtuwln.sHtML

[Q80] 字符串截取
来源：http://3g.fanxiaobao.xyz/Article/details/ghsokyzim.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcnbskbei.sHtML

[Q81] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gszpnhsjp.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtykualqs.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.fanxiaobao.xyz/Article/details/gyeztvvjq.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/glckevlsl.sHtML

[Q83] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/gwcqymhdu.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzskliuoh.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwjlkbupw.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/grfxqmaol.sHtML

[Q85] 数值取整
来源：http://wap.fanxiaobao.xyz/Article/details/gddhafqfs.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gplhotdwz.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fanxiaobao.xyz/Article/details/gvanzqykp.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fanxiaobao.xyz/Article/details/gxvdktutb.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gcbpvjdzx.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.fanxiaobao.xyz/Article/details/gxfhuevnk.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fanxiaobao.xyz/Article/details/gurprqsay.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzvilnmye.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gurvbtgto.sHtML

[Q89] 判断表是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gjepjqzwj.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.fanxiaobao.xyz/Article/details/guvymtgzs.sHtML

[Q90] 生成序号列
来源：http://mobile.fanxiaobao.xyz/Article/details/gcfzikpoo.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghvsjrlpf.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggantefik.sHtML

R. Bash 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gukqzggwh.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gjdcbfsjx.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fanxiaobao.xyz/Article/details/gdncohloa.sHtML

#!/usr/bin/env bash
来源：http://read.share.fanxiaobao.xyz/Article/details/gjplnhvdy.sHtML

set -euo pipefail
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbcmssosd.sHtML

[R02] 变量赋值与使用
来源：http://baike.fanxiaobao.xyz/Article/details/gpaooodlv.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gruzlpuwf.sHtML

[R03] 只读变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwkauwxba.sHtML

readonly PI=3.14
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtoznokuj.sHtML

[R04] 位置参数
来源：http://wap.fanxiaobao.xyz/Article/details/gmnsdqpbv.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glrfexang.sHtML

[R05] 参数默认值
来源：http://wap.fanxiaobao.xyz/Article/details/gbfvjnaxw.sHtML

name="${1:-default}"
来源：http://blog.fanxiaobao.xyz/Article/details/gqcosdlhq.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbqlvsabp.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gohxrgnbj.sHtML

[R07] if 判断文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gieafnqvb.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gjbgzaulp.sHtML

[R08] 数值比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gkewehmee.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gbfoflvid.sHtML

[R09] 字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/grlfrrokt.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/grdtzzrbh.sHtML

[R10] 正则匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gonufpxro.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gixrbldoz.sHtML

[R11] case 多分支
来源：http://3g.fanxiaobao.xyz/Article/details/gbydzwzdv.sHtML

case "$1" in
来源：http://m.share.fanxiaobao.xyz/Article/details/gkewoinnb.sHtML

start) echo "启动" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwnxawysg.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/glznsacfh.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gwmexmpsp.sHtML

esac
来源：http://blog.fanxiaobao.xyz/Article/details/gxmuantjx.sHtML

[R12] for 遍历文件
来源：http://blog.fanxiaobao.xyz/Article/details/gaqivzmxm.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyykvcfdy.sHtML

[R13] for 计数循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gafrovvii.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gedpfvzth.sHtML

[R14] C 风格 for
来源：http://3g.fanxiaobao.xyz/Article/details/gupwjtzkd.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/ggntluggp.sHtML

[R15] while 逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gdpzownww.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gdupjzwzq.sHtML

[R16] until 等待条件
来源：http://blog.fanxiaobao.xyz/Article/details/gtcqfalzj.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gevodeaam.sHtML

[R17] 数组定义与取值
来源：http://baike.fanxiaobao.xyz/Article/details/ggqqccfic.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvurvbfhp.sHtML

[R18] 遍历数组
来源：http://read.share.fanxiaobao.xyz/Article/details/gakeqepjd.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gehmflzxy.sHtML

[R19] 数组长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gfkdzhfxo.sHtML

echo "${#arr[@]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gcjxoetwk.sHtML

[R20] 关联数组（字典）
来源：http://baike.fanxiaobao.xyz/Article/details/glzchqajy.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/ggamycnkk.sHtML

[R21] 字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/goegrjtaj.sHtML

echo "${#s}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gfeakxfly.sHtML

[R22] 截取子串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gifkksvut.sHtML

echo "${s:0:5}"
来源：http://3g.fanxiaobao.xyz/Article/details/gdigcaahw.sHtML

[R23] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gtprssxta.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gumfuybct.sHtML

[R24] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gghyiorub.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gmxavmsqd.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbebhihqm.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fanxiaobao.xyz/Article/details/gkyjkexzs.sHtML

[R26] 命令替换
来源：http://blog.fanxiaobao.xyz/Article/details/gsnbcyvli.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fanxiaobao.xyz/Article/details/gpmtsjajr.sHtML

[R27] 算术展开
来源：http://www.blog.fanxiaobao.xyz/Article/details/gesddupab.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzyuubxuj.sHtML

[R28] 浮点运算
来源：http://m.share.fanxiaobao.xyz/Article/details/gjaxrcvsy.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fanxiaobao.xyz/Article/details/gidftyufu.sHtML

[R29] 定义函数
来源：http://baike.fanxiaobao.xyz/Article/details/gujgoeukl.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fanxiaobao.xyz/Article/details/gbhvhwspi.sHtML

[R30] 函数返回状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gktsdxeas.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fanxiaobao.xyz/Article/details/gpglbbgcd.sHtML

[R31] 局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtindzohi.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gpmhcjuqq.sHtML

[R32] 参数个数校验
来源：http://mobile.fanxiaobao.xyz/Article/details/gvqplhsdq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gyxylsiag.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fanxiaobao.xyz/Article/details/gjxdorjbl.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjwpsaqgz.sHtML

[R34] 退出时清理
来源：http://baike.fanxiaobao.xyz/Article/details/gbhlefcoz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gnscdgzlo.sHtML

[R35] 后台执行并等待
来源：http://www.share.fanxiaobao.xyz/Article/details/geurubjlh.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fanxiaobao.xyz/Article/details/gzqwcnyvo.sHtML

[R36] 并发执行多个任务
来源：http://baike.fanxiaobao.xyz/Article/details/gcibojfcn.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.fanxiaobao.xyz/Article/details/gdaxgdylk.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjtrtvjxc.sHtML

files=$(ls -1)
来源：http://baike.fanxiaobao.xyz/Article/details/gsvaaiciu.sHtML

[R38] 管道串联
来源：http://mobile.fanxiaobao.xyz/Article/details/gihluunld.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fanxiaobao.xyz/Article/details/ghcdgzeqq.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmsjxrvxc.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdlbqnbcp.sHtML

[R40] 追加写日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjipnqeiy.sHtML

echo "log" >> out.log
来源：http://blog.fanxiaobao.xyz/Article/details/gmijlkmto.sHtML

[R41] 丢弃输出
来源：http://3g.fanxiaobao.xyz/Article/details/gewbgqgzl.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/ghswrjjoa.sHtML

[R42] 输入重定向
来源：http://blog.fanxiaobao.xyz/Article/details/gdkjrbpww.sHtML

wc -l < a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gfofrczpo.sHtML

[R43] 按名字查找文件
来源：http://3g.fanxiaobao.xyz/Article/details/gwylmbefw.sHtML

find . -name "*.log" -type f
来源：http://baike.fanxiaobao.xyz/Article/details/gracrfqsx.sHtML

[R44] 按修改时间查找
来源：http://m.share.fanxiaobao.xyz/Article/details/guivlanpq.sHtML

find . -mtime -7 -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/gqcirbyei.sHtML

[R45] 批量删除
来源：http://www.share.fanxiaobao.xyz/Article/details/gtmxrlrsv.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fanxiaobao.xyz/Article/details/gqqajtmve.sHtML

[R46] 递归替换文件内容
来源：http://www.share.fanxiaobao.xyz/Article/details/gbghohtba.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fanxiaobao.xyz/Article/details/gxmzvjlaz.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvddkeucy.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gitthfgnj.sHtML

[R48] awk 取指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/gfxopgqwh.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcyzknbkl.sHtML

[R49] awk 带条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gxcwterft.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fanxiaobao.xyz/Article/details/gczsatlov.sHtML

[R50] awk 求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geederzfd.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/grojsbvuw.sHtML

[R51] 排序去重取前几
来源：http://read.share.fanxiaobao.xyz/Article/details/gxbkswuon.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqquczyhr.sHtML

[R52] 统计行数
来源：http://blog.fanxiaobao.xyz/Article/details/gdrypbicm.sHtML

wc -l a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gqqmwfneg.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fanxiaobao.xyz/Article/details/gxcvadsdh.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gdwzamvek.sHtML

[R54] 比较两个文件
来源：http://3g.fanxiaobao.xyz/Article/details/gholmsaby.sHtML

diff a.txt b.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gtwdlbmav.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjkbujjda.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnuwcyhys.sHtML

[R56] 远程拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gutxbxuav.sHtML

scp file user@host:/path/
来源：http://www.blog.fanxiaobao.xyz/Article/details/gavqehaci.sHtML

[R57] 远程执行命令
来源：http://blog.fanxiaobao.xyz/Article/details/gorpugpzp.sHtML

ssh user@host 'uptime'
来源：http://m.share.fanxiaobao.xyz/Article/details/ghmzfwwcf.sHtML

[R58] 下载文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gyzmawjmi.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fanxiaobao.xyz/Article/details/ghyotytmp.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfngvlqbp.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fanxiaobao.xyz/Article/details/gvkbxohzy.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gyqyebbno.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fanxiaobao.xyz/Article/details/gmiyurpzg.sHtML

[R61] 磁盘占用
来源：http://blog.fanxiaobao.xyz/Article/details/gzcycaavx.sHtML

df -h;  du -sh *
来源：http://m.share.fanxiaobao.xyz/Article/details/gwbmbyzra.sHtML

[R62] 找最占空间的文件
来源：http://baike.fanxiaobao.xyz/Article/details/gukmowxac.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fanxiaobao.xyz/Article/details/gbsdrfrlx.sHtML

[R63] 内存与进程
来源：http://mobile.fanxiaobao.xyz/Article/details/ghbfyfxib.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fanxiaobao.xyz/Article/details/gfjupoiif.sHtML

[R64] 结束进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggxkfrfxc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fanxiaobao.xyz/Article/details/grcrbauvg.sHtML

[R65] 查看端口占用
来源：http://3g.fanxiaobao.xyz/Article/details/gfagadfly.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fanxiaobao.xyz/Article/details/glqblzzsl.sHtML

[R66] 定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/ghnbkvhdu.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghjmgcwmt.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fanxiaobao.xyz/Article/details/goqdkwcaf.sHtML

openssl rand -hex 16
来源：http://m.share.fanxiaobao.xyz/Article/details/gkzxknteg.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fanxiaobao.xyz/Article/details/glxaprbun.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gsuvuxkpz.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gngktyohm.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fanxiaobao.xyz/Article/details/gcgkzntsc.sHtML

[R70] 时间戳与互转
来源：http://read.share.fanxiaobao.xyz/Article/details/guvtmalcq.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fanxiaobao.xyz/Article/details/gzihvywnn.sHtML

[R71] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gixjipvoc.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fanxiaobao.xyz/Article/details/gnqbkjqpz.sHtML

[R72] 等待端口就绪
来源：http://read.share.fanxiaobao.xyz/Article/details/gplconzdq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/govqgtrjt.sHtML

[R73] 分割大日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gsnrzwzdo.sHtML

split -l 1000 big.log part_
来源：http://mobile.fanxiaobao.xyz/Article/details/gzfqiwwml.sHtML

[R74] 批量重命名
来源：http://wap.fanxiaobao.xyz/Article/details/gvfqmwvaf.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gstkisjfk.sHtML

[R75] 导出环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/ghsyuczwk.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://3g.fanxiaobao.xyz/Article/details/gbsfjlrpa.sHtML

[R76] 使用临时文件
来源：http://wap.fanxiaobao.xyz/Article/details/gnjonufqz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geuefnjoo.sHtML

[R77] 读取用户输入
来源：http://www.blog.fanxiaobao.xyz/Article/details/gannglkht.sHtML

read -rp "请输入: " ans
来源：http://www.share.fanxiaobao.xyz/Article/details/gftqjkckj.sHtML

[R78] 交互式菜单
来源：http://m.share.fanxiaobao.xyz/Article/details/grfmwygqw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gzjjaqlll.sHtML

[R79] 解析命令行选项
来源：http://baike.fanxiaobao.xyz/Article/details/gggtocsnf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fanxiaobao.xyz/Article/details/gbzoakmov.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fanxiaobao.xyz/Article/details/gkpmriytb.sHtML

time ./run.sh
来源：http://wap.fanxiaobao.xyz/Article/details/grnhxpxio.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/glrlzvufe.sHtML

S. C / C++ 专题
来源：http://baike.fanxiaobao.xyz/Article/details/gyjskbrwv.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gurvgxyin.sHtML

[S01] C：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gnfblabrf.sHtML

#include <stdio.h>
来源：http://mobile.fanxiaobao.xyz/Article/details/gzzgwpdxs.sHtML


<!-- 参考信息 -->