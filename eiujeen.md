代发 wailian999

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.zdbjq.cn/Article/details/gmrcwlbfj.sHtML

[Q22] 排序
来源：http://m.share.hesvh.cn/Article/details/grquhblpc.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.zdbjq.cn/Article/details/gydylswsc.sHtML

[Q23] 分页
来源：http://www.share.fehbvm.com/Article/details/glfsxjskz.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.hesvh.cn/Article/details/gpnaokyyz.sHtML

[Q24] 去重
来源：http://read.share.hesvh.cn/Article/details/gwssaecqr.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.zdbjq.cn/Article/details/glaelpqxv.sHtML

[Q25] 只取前 N 条
来源：http://mobile.fehbvm.com/Article/details/goxumjzjb.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.hesvh.cn/Article/details/gphyebqym.sHtML

[Q26] 计数
来源：http://blog.hesvh.cn/Article/details/gqrovvfex.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gmimbzbgx.sHtML

[Q27] 条件计数
来源：http://3g.fehbvm.com/Article/details/gvzcdxnjf.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gdbfrxwva.sHtML

[Q28] 求和与平均
来源：http://www.share.zdbjq.cn/Article/details/gbxjzaswb.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gaytitanm.sHtML

[Q29] 最大最小值
来源：http://read.share.hesvh.cn/Article/details/gdntohgro.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.hesvh.cn/Article/details/ggjxbqibd.sHtML

[Q30] 分组统计
来源：http://baike.fehbvm.com/Article/details/ghggtelre.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gmwuyxepj.sHtML

[Q31] 分组后过滤
来源：http://www.share.hesvh.cn/Article/details/gaowmdrfv.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.fehbvm.com/Article/details/gjgxpppzk.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gmhmnhlef.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/gqmoelyrm.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://mobile.zdbjq.cn/Article/details/giredrjwg.sHtML

[Q33] 多列分组
来源：http://www.blog.zdbjq.cn/Article/details/gquzhchru.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.hesvh.cn/Article/details/gzbyymprv.sHtML

[Q34] 每组取第一条
来源：http://www.share.fehbvm.com/Article/details/gdtvwhuvq.sHtML

SELECT * FROM (
来源：http://baike.zdbjq.cn/Article/details/gukrmvfbi.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.fehbvm.com/Article/details/gqakbwjqt.sHtML

) t WHERE rn = 1;
来源：http://m.share.fehbvm.com/Article/details/gbgvrtmmi.sHtML

[Q35] 内连接
来源：http://read.share.hesvh.cn/Article/details/ggoqeoefs.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fehbvm.com/Article/details/gbhfwzhfv.sHtML

[Q36] 左连接
来源：http://blog.zdbjq.cn/Article/details/gweauwzzy.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.fehbvm.com/Article/details/gioqqqgis.sHtML

[Q37] 右连接
来源：http://3g.hesvh.cn/Article/details/gwrjkvike.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.fehbvm.com/Article/details/gbirqqwoq.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.hesvh.cn/Article/details/gwprnviev.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.fehbvm.com/Article/details/glcjlpdup.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.hesvh.cn/Article/details/gcctmijby.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.zdbjq.cn/Article/details/gmroeflzm.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.fehbvm.com/Article/details/gyerfvnvk.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.hesvh.cn/Article/details/gixygnugu.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.hesvh.cn/Article/details/gzieckqyh.sHtML

[Q41] 多表连接
来源：http://wap.hesvh.cn/Article/details/gorhgzqla.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.zdbjq.cn/Article/details/gbusqlvpt.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.zdbjq.cn/Article/details/gdzyzazsz.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.zdbjq.cn/Article/details/gdgtjczev.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.fehbvm.com/Article/details/gfnrkjokt.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.hesvh.cn/Article/details/ggioyusfp.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.hesvh.cn/Article/details/glqqlgfoo.sHtML

[Q43] 标量子查询
来源：http://read.share.fehbvm.com/Article/details/gyjbybvuu.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.hesvh.cn/Article/details/gzvoeeyno.sHtML

[Q44] IN 子查询
来源：http://wap.hesvh.cn/Article/details/gujbarkak.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.fehbvm.com/Article/details/gesstoftz.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.hesvh.cn/Article/details/gevexsvfi.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fehbvm.com/Article/details/gxafzsqac.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.fehbvm.com/Article/details/glbquxnxz.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.hesvh.cn/Article/details/gmjzqagoo.sHtML

[Q47] 与平均值比较
来源：http://m.share.fehbvm.com/Article/details/gmrrfvmmo.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.fehbvm.com/Article/details/gqgrakhrf.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.zdbjq.cn/Article/details/gzkorevlj.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.hesvh.cn/Article/details/gmqmykkgw.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.zdbjq.cn/Article/details/goqeawxta.sHtML

[Q49] 更新单行
来源：http://wap.hesvh.cn/Article/details/gupoflmzc.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gnaexoplr.sHtML

[Q50] 批量更新
来源：http://read.share.fehbvm.com/Article/details/gcoodkucl.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.fehbvm.com/Article/details/gexesagmh.sHtML

[Q51] 用子查询更新
来源：http://baike.hesvh.cn/Article/details/gndcvrqzp.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.hesvh.cn/Article/details/gbwiubzar.sHtML

[Q52] 删除指定行
来源：http://wap.zdbjq.cn/Article/details/gkiogadla.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.zdbjq.cn/Article/details/garewfueo.sHtML

[Q53] 按条件删除
来源：http://www.share.fehbvm.com/Article/details/gcflxctnn.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.zdbjq.cn/Article/details/gvavijjzy.sHtML

[Q54] 清空表
来源：http://www.share.zdbjq.cn/Article/details/gvdifiwvo.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fehbvm.com/Article/details/gtlwzcbew.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.hesvh.cn/Article/details/gvbbzcexa.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.zdbjq.cn/Article/details/gwxnomfmu.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.hesvh.cn/Article/details/gcypuzzgp.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.hesvh.cn/Article/details/gzbpbzdqu.sHtML

[Q57] 行号
来源：http://www.m.share.hesvh.cn/Article/details/ghgvqrrjw.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gdcgzaimw.sHtML

[Q58] 累计求和
来源：http://www.share.hesvh.cn/Article/details/gplbafnes.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.hesvh.cn/Article/details/geplgzzwo.sHtML

[Q59] 分组内累计
来源：http://read.share.zdbjq.cn/Article/details/gelbvnuoe.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gwazlunwx.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.fehbvm.com/Article/details/gbwjwvmgx.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.zdbjq.cn/Article/details/gdkrjiovx.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gjpdmjqja.sHtML

[Q61] 移动平均
来源：http://www.share.zdbjq.cn/Article/details/gvnumkpli.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gzxlxavnt.sHtML

[Q62] 分组占比
来源：http://baike.zdbjq.cn/Article/details/gzddzqpit.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/gxgrtsbfv.sHtML

[Q63] 开启事务
来源：http://wap.hesvh.cn/Article/details/gtvqavroo.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.hesvh.cn/Article/details/gvrzqsqgt.sHtML

[Q64] 提交事务
来源：http://www.blog.zdbjq.cn/Article/details/ghyfkiyet.sHtML

COMMIT;
来源：http://www.m.share.zdbjq.cn/Article/details/ggfjkjjcg.sHtML

[Q65] 回滚事务
来源：http://wap.hesvh.cn/Article/details/ggrxutzyj.sHtML

ROLLBACK;
来源：http://blog.hesvh.cn/Article/details/ghsodpnbx.sHtML

[Q66] 行锁查询
来源：http://blog.fehbvm.com/Article/details/gtxhoqwmg.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.zdbjq.cn/Article/details/gikenchnn.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.hesvh.cn/Article/details/gwqdsgjkq.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.hesvh.cn/Article/details/gwxbqnuit.sHtML

[Q68] 保存点
来源：http://mobile.hesvh.cn/Article/details/gjkaphoam.sHtML

SAVEPOINT sp1;
来源：http://m.share.fehbvm.com/Article/details/gntrvkosb.sHtML

ROLLBACK TO sp1;
来源：http://blog.fehbvm.com/Article/details/gytokvazf.sHtML

[Q69] 查看执行计划
来源：http://m.share.zdbjq.cn/Article/details/gjqsmorwl.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.fehbvm.com/Article/details/gjrytsyxj.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.fehbvm.com/Article/details/gmioidhka.sHtML

ANALYZE TABLE users;
来源：http://read.share.zdbjq.cn/Article/details/giwrelclj.sHtML

[Q71] 查看建表语句
来源：http://www.blog.zdbjq.cn/Article/details/ghndvppun.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fehbvm.com/Article/details/gpsbszgbt.sHtML

[Q72] 查看索引
来源：http://m.share.hesvh.cn/Article/details/gkxxinwrs.sHtML

SHOW INDEX FROM users;
来源：http://mobile.zdbjq.cn/Article/details/ghsjhymsg.sHtML

[Q73] 查看表状态
来源：http://www.blog.hesvh.cn/Article/details/gcekfproc.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.hesvh.cn/Article/details/glsszzrbd.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.zdbjq.cn/Article/details/gpubpakow.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.fehbvm.com/Article/details/gyvcqputu.sHtML

[Q75] 日期格式化
来源：http://mobile.hesvh.cn/Article/details/gdtwrzamu.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gwbmuzlox.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.zdbjq.cn/Article/details/gcmdpzxsp.sHtML

[Q76] 按天统计
来源：http://blog.zdbjq.cn/Article/details/glkfeobwg.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.zdbjq.cn/Article/details/giyuvkmal.sHtML

[Q77] 时间加减
来源：http://read.share.fehbvm.com/Article/details/gjxvngkvn.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.fehbvm.com/Article/details/gjsacdsvn.sHtML

[Q78] 当前时间
来源：http://www.share.hesvh.cn/Article/details/gfmeimlbc.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.zdbjq.cn/Article/details/ghzxnixva.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.fehbvm.com/Article/details/gilfhumek.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.hesvh.cn/Article/details/giweqtlwy.sHtML

[Q80] 字符串截取
来源：http://www.m.share.fehbvm.com/Article/details/gkhpzarqh.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gujeudoxz.sHtML

[Q81] 字符串替换
来源：http://baike.fehbvm.com/Article/details/gyfpmxdmp.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.hesvh.cn/Article/details/glqeijvbm.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fehbvm.com/Article/details/gefpiwwyr.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/ghxehmznd.sHtML

[Q83] 大小写转换
来源：http://www.m.share.hesvh.cn/Article/details/gnwflhiyj.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gnzguxret.sHtML

[Q84] 去除首尾空格
来源：http://www.share.hesvh.cn/Article/details/gdbvdvgct.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gexqvgfcf.sHtML

[Q85] 数值取整
来源：http://mobile.hesvh.cn/Article/details/ggmceixly.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.zdbjq.cn/Article/details/gqgsrdukk.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.zdbjq.cn/Article/details/gzaxkaknv.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.hesvh.cn/Article/details/gfnpamazf.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.hesvh.cn/Article/details/glrxszmai.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.fehbvm.com/Article/details/gmhiohvxq.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.zdbjq.cn/Article/details/gzgmhnjcp.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.zdbjq.cn/Article/details/gvzcnqeyw.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gvtqulpcu.sHtML

[Q89] 判断表是否存在
来源：http://m.share.hesvh.cn/Article/details/gyhhspila.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.hesvh.cn/Article/details/gyrwmccot.sHtML

[Q90] 生成序号列
来源：http://www.blog.zdbjq.cn/Article/details/gadcuqsyr.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.hesvh.cn/Article/details/gpnonqmpv.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gejcadmhq.sHtML

R. Bash 专题
来源：http://3g.fehbvm.com/Article/details/gwjluwgck.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gixcjhzqv.sHtML

[R01] shebang 与严格模式
来源：http://3g.fehbvm.com/Article/details/gbqbpilbz.sHtML

#!/usr/bin/env bash
来源：http://blog.hesvh.cn/Article/details/gufehggqr.sHtML

set -euo pipefail
来源：http://m.share.hesvh.cn/Article/details/gyyfwadmn.sHtML

[R02] 变量赋值与使用
来源：http://wap.hesvh.cn/Article/details/gkgnnfuix.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.zdbjq.cn/Article/details/gedbbbxkm.sHtML

[R03] 只读变量
来源：http://blog.hesvh.cn/Article/details/glrxdfvnr.sHtML

readonly PI=3.14
来源：http://m.share.fehbvm.com/Article/details/gujbhktvr.sHtML

[R04] 位置参数
来源：http://www.m.share.hesvh.cn/Article/details/gbfdzgdum.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.hesvh.cn/Article/details/gadittdha.sHtML

[R05] 参数默认值
来源：http://read.share.fehbvm.com/Article/details/gljwmchep.sHtML

name="${1:-default}"
来源：http://baike.hesvh.cn/Article/details/gnipkgenv.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fehbvm.com/Article/details/gdygmwjke.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/ghtjjxqas.sHtML

[R07] if 判断文件
来源：http://blog.hesvh.cn/Article/details/ggnwpjcns.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.zdbjq.cn/Article/details/glnwfqmsm.sHtML

[R08] 数值比较
来源：http://m.share.hesvh.cn/Article/details/gwzoekdqp.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.zdbjq.cn/Article/details/grgxjnoyi.sHtML

[R09] 字符串比较
来源：http://m.share.fehbvm.com/Article/details/gclvalqly.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.zdbjq.cn/Article/details/ggclolohr.sHtML

[R10] 正则匹配
来源：http://m.share.zdbjq.cn/Article/details/gtldjbiko.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gqkbbcsko.sHtML

[R11] case 多分支
来源：http://baike.fehbvm.com/Article/details/gdzdlunsr.sHtML

case "$1" in
来源：http://mobile.zdbjq.cn/Article/details/gnriyuvyg.sHtML

start) echo "启动" ;;
来源：http://mobile.zdbjq.cn/Article/details/glunkndsd.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fehbvm.com/Article/details/gpqfxbztv.sHtML

*)     echo "未知命令" ;;
来源：http://baike.zdbjq.cn/Article/details/gzkkhzpbl.sHtML

esac
来源：http://m.share.hesvh.cn/Article/details/gjwigdgrk.sHtML

[R12] for 遍历文件
来源：http://www.m.share.hesvh.cn/Article/details/gsqmgrknt.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.hesvh.cn/Article/details/gnrgkzjba.sHtML

[R13] for 计数循环
来源：http://m.share.hesvh.cn/Article/details/gkorsjrdh.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.hesvh.cn/Article/details/gmpnwogwc.sHtML

[R14] C 风格 for
来源：http://blog.fehbvm.com/Article/details/gbpckmjqi.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gfuxaymmt.sHtML

[R15] while 逐行读文件
来源：http://blog.hesvh.cn/Article/details/gborehtsn.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fehbvm.com/Article/details/gvesvrggh.sHtML

[R16] until 等待条件
来源：http://www.m.share.hesvh.cn/Article/details/gvzkantmt.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.hesvh.cn/Article/details/gsttyygpp.sHtML

[R17] 数组定义与取值
来源：http://blog.zdbjq.cn/Article/details/gfloexrhb.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fehbvm.com/Article/details/gphivjqpc.sHtML

[R18] 遍历数组
来源：http://www.blog.zdbjq.cn/Article/details/gkjbiivpd.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fehbvm.com/Article/details/gippbhmnq.sHtML

[R19] 数组长度
来源：http://read.share.hesvh.cn/Article/details/gnopomibi.sHtML

echo "${#arr[@]}"
来源：http://m.share.hesvh.cn/Article/details/gvhyyhizu.sHtML

[R20] 关联数组（字典）
来源：http://3g.zdbjq.cn/Article/details/gnqtekivh.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fehbvm.com/Article/details/gjrteqwdc.sHtML

[R21] 字符串长度
来源：http://www.m.share.fehbvm.com/Article/details/gwqkrwzcm.sHtML

echo "${#s}"
来源：http://read.share.fehbvm.com/Article/details/gmeriazwm.sHtML

[R22] 截取子串
来源：http://mobile.zdbjq.cn/Article/details/ghktevaqd.sHtML

echo "${s:0:5}"
来源：http://www.blog.zdbjq.cn/Article/details/grxgpudaw.sHtML

[R23] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/gnfxkhhop.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.fehbvm.com/Article/details/gjfofiphz.sHtML

[R24] 大小写转换
来源：http://www.m.share.zdbjq.cn/Article/details/gvltuogdg.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.zdbjq.cn/Article/details/gzbafklsm.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.hesvh.cn/Article/details/gfftabopj.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.hesvh.cn/Article/details/gwixbybrf.sHtML

[R26] 命令替换
来源：http://baike.zdbjq.cn/Article/details/gorxkkvbk.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.hesvh.cn/Article/details/gobwlvwmz.sHtML

[R27] 算术展开
来源：http://baike.fehbvm.com/Article/details/gvqbqukpg.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.fehbvm.com/Article/details/giuyuuufc.sHtML

[R28] 浮点运算
来源：http://wap.fehbvm.com/Article/details/ggfwbhsyg.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.zdbjq.cn/Article/details/gzzcnykie.sHtML

[R29] 定义函数
来源：http://www.blog.fehbvm.com/Article/details/ghjjmndlq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.hesvh.cn/Article/details/grjznjuki.sHtML

[R30] 函数返回状态码
来源：http://baike.zdbjq.cn/Article/details/gbowrsnvz.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.hesvh.cn/Article/details/gxbpmbqpx.sHtML

[R31] 局部变量
来源：http://3g.hesvh.cn/Article/details/gbdompgwg.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fehbvm.com/Article/details/gdqoesegn.sHtML

[R32] 参数个数校验
来源：http://m.share.fehbvm.com/Article/details/gvsiblaqb.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fehbvm.com/Article/details/giwamngdx.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.hesvh.cn/Article/details/gbptwibhn.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.hesvh.cn/Article/details/gszhmcwuy.sHtML

[R34] 退出时清理
来源：http://read.share.hesvh.cn/Article/details/gvizwhgjp.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/gibjmekmw.sHtML

[R35] 后台执行并等待
来源：http://www.blog.zdbjq.cn/Article/details/gcuveeewz.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.hesvh.cn/Article/details/gdxxvxezs.sHtML

[R36] 并发执行多个任务
来源：http://www.share.hesvh.cn/Article/details/gfbwgcyvd.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fehbvm.com/Article/details/gketbjddf.sHtML

[R37] 把输出赋给变量
来源：http://mobile.hesvh.cn/Article/details/gdamhchkc.sHtML

files=$(ls -1)
来源：http://wap.fehbvm.com/Article/details/ghaoufqoe.sHtML

[R38] 管道串联
来源：http://blog.fehbvm.com/Article/details/gykbdegfn.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.zdbjq.cn/Article/details/gjsyhebhd.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fehbvm.com/Article/details/gzduaxzgm.sHtML

cmd > out.log 2>&1
来源：http://www.share.hesvh.cn/Article/details/gmdsubevk.sHtML

[R40] 追加写日志
来源：http://read.share.fehbvm.com/Article/details/gaggtqfst.sHtML

echo "log" >> out.log
来源：http://www.m.share.zdbjq.cn/Article/details/glruxenzk.sHtML

[R41] 丢弃输出
来源：http://m.share.hesvh.cn/Article/details/gamzrdlqp.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.zdbjq.cn/Article/details/gkaqszqxf.sHtML

[R42] 输入重定向
来源：http://baike.zdbjq.cn/Article/details/gkllleimz.sHtML

wc -l < a.txt
来源：http://3g.zdbjq.cn/Article/details/gzuiewqmt.sHtML

[R43] 按名字查找文件
来源：http://3g.hesvh.cn/Article/details/guakphnzr.sHtML

find . -name "*.log" -type f
来源：http://read.share.zdbjq.cn/Article/details/guyyhuxvd.sHtML

[R44] 按修改时间查找
来源：http://blog.fehbvm.com/Article/details/gxaznpcfp.sHtML

find . -mtime -7 -type f
来源：http://mobile.fehbvm.com/Article/details/gsdyxxsji.sHtML

[R45] 批量删除
来源：http://blog.hesvh.cn/Article/details/gwymkwrgp.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.zdbjq.cn/Article/details/gmehopbwl.sHtML

[R46] 递归替换文件内容
来源：http://3g.hesvh.cn/Article/details/gsegmwnbu.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.zdbjq.cn/Article/details/gjhvrkbxl.sHtML

[R47] sed 单行替换
来源：http://blog.fehbvm.com/Article/details/gzfqpyyuq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gjoickdwt.sHtML

[R48] awk 取指定列
来源：http://baike.fehbvm.com/Article/details/gayiaovzd.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fehbvm.com/Article/details/gdouudvhc.sHtML

[R49] awk 带条件
来源：http://read.share.hesvh.cn/Article/details/gwmcpdtmv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.zdbjq.cn/Article/details/guyqhvuqa.sHtML

[R50] awk 求和
来源：http://m.share.fehbvm.com/Article/details/gzgvrowzv.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.zdbjq.cn/Article/details/gxybdabnl.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.hesvh.cn/Article/details/gyfcyjrmo.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fehbvm.com/Article/details/gjxmycaou.sHtML

[R52] 统计行数
来源：http://blog.fehbvm.com/Article/details/grzzwxyfz.sHtML

wc -l a.txt
来源：http://baike.hesvh.cn/Article/details/gkekloirw.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.zdbjq.cn/Article/details/gmlanzgrb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.zdbjq.cn/Article/details/gjauupqei.sHtML

[R54] 比较两个文件
来源：http://3g.fehbvm.com/Article/details/glgfqmuef.sHtML

diff a.txt b.txt
来源：http://wap.zdbjq.cn/Article/details/gryzinxsf.sHtML

[R55] 压缩与解压
来源：http://mobile.zdbjq.cn/Article/details/glpajpiac.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fehbvm.com/Article/details/gkkxaxvow.sHtML

[R56] 远程拷贝
来源：http://baike.zdbjq.cn/Article/details/ggmgmidcp.sHtML

scp file user@host:/path/
来源：http://www.m.share.zdbjq.cn/Article/details/gcrdqebqq.sHtML

[R57] 远程执行命令
来源：http://mobile.zdbjq.cn/Article/details/gajtnjizw.sHtML

ssh user@host 'uptime'
来源：http://m.share.zdbjq.cn/Article/details/gwitrbwhx.sHtML

[R58] 下载文件
来源：http://3g.hesvh.cn/Article/details/gjlnuivzy.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.hesvh.cn/Article/details/gxfxzionw.sHtML

[R59] 发 POST JSON
来源：http://m.share.hesvh.cn/Article/details/gkuyyqfru.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fehbvm.com/Article/details/gxhwsbduz.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fehbvm.com/Article/details/ggsoxgkgx.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fehbvm.com/Article/details/gpquuhwpc.sHtML

[R61] 磁盘占用
来源：http://www.blog.zdbjq.cn/Article/details/goludxhmh.sHtML

df -h;  du -sh *
来源：http://www.blog.hesvh.cn/Article/details/gmeocvzxx.sHtML

[R62] 找最占空间的文件
来源：http://3g.fehbvm.com/Article/details/gkirmfwja.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.hesvh.cn/Article/details/gtgcedeax.sHtML

[R63] 内存与进程
来源：http://m.share.fehbvm.com/Article/details/gnxzswiec.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.zdbjq.cn/Article/details/gjdqaedcq.sHtML

[R64] 结束进程
来源：http://www.share.fehbvm.com/Article/details/gtlcecklj.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.hesvh.cn/Article/details/gewrgiqmq.sHtML

[R65] 查看端口占用
来源：http://wap.fehbvm.com/Article/details/gjnatrdnj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fehbvm.com/Article/details/gymuiahhb.sHtML

[R66] 定时任务
来源：http://blog.hesvh.cn/Article/details/gbjwvetna.sHtML

crontab -e;  crontab -l
来源：http://blog.hesvh.cn/Article/details/gpcywjwjj.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fehbvm.com/Article/details/gdbypeegt.sHtML

openssl rand -hex 16
来源：http://blog.hesvh.cn/Article/details/glyprhybj.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fehbvm.com/Article/details/geapblrtk.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gnhdmynnj.sHtML

[R69] 生成随机密码
来源：http://baike.fehbvm.com/Article/details/gvaiullce.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.zdbjq.cn/Article/details/gasbvtsqr.sHtML

[R70] 时间戳与互转
来源：http://blog.fehbvm.com/Article/details/gwtvrtrry.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.hesvh.cn/Article/details/gyvwxyjow.sHtML

[R71] 日期格式化
来源：http://blog.zdbjq.cn/Article/details/gunlyavwo.sHtML


<!-- 参考信息 -->