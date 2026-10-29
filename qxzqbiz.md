代发 wailian999

SELECT * FROM users;
来源：http://blog.fehbvm.com/Article/details/gumnrurec.sHtML

[Q16] 查询指定列
来源：http://wap.hesvh.cn/Article/details/gmdenirvd.sHtML

SELECT id, name FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gksfckaah.sHtML

[Q17] 条件查询
来源：http://www.m.share.zdbjq.cn/Article/details/getczmjdv.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.hesvh.cn/Article/details/gdmxocsgb.sHtML

[Q18] 模糊匹配
来源：http://www.share.zdbjq.cn/Article/details/gkdaotepw.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.blog.fehbvm.com/Article/details/gwnchufsx.sHtML

[Q19] 范围查询
来源：http://wap.fehbvm.com/Article/details/gwnjqunpa.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.m.share.hesvh.cn/Article/details/gdtgzzxhm.sHtML

[Q20] IN 列表
来源：http://blog.zdbjq.cn/Article/details/gmbxiumax.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.zdbjq.cn/Article/details/ggohxlvir.sHtML

[Q21] 空值判断
来源：http://3g.fehbvm.com/Article/details/gnfukplwv.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://read.share.hesvh.cn/Article/details/gqgehwomh.sHtML

[Q22] 排序
来源：http://read.share.fehbvm.com/Article/details/gnobobaev.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.zdbjq.cn/Article/details/gbstvifwh.sHtML

[Q23] 分页
来源：http://baike.zdbjq.cn/Article/details/gizjrrkgv.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://baike.zdbjq.cn/Article/details/ggwnadazi.sHtML

[Q24] 去重
来源：http://m.share.zdbjq.cn/Article/details/gjgygkeuj.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.hesvh.cn/Article/details/gytitwivb.sHtML

[Q25] 只取前 N 条
来源：http://baike.zdbjq.cn/Article/details/gmetizaea.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.fehbvm.com/Article/details/gapcwxrup.sHtML

[Q26] 计数
来源：http://blog.hesvh.cn/Article/details/geagxxgnh.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.hesvh.cn/Article/details/glaxebmzi.sHtML

[Q27] 条件计数
来源：http://m.share.fehbvm.com/Article/details/gwbcwgvzx.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.zdbjq.cn/Article/details/gshyvqinr.sHtML

[Q28] 求和与平均
来源：http://www.m.share.fehbvm.com/Article/details/gskpszsuj.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gnuduouih.sHtML

[Q29] 最大最小值
来源：http://www.blog.hesvh.cn/Article/details/gbqhltjvm.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gthvkfrfd.sHtML

[Q30] 分组统计
来源：http://blog.fehbvm.com/Article/details/gptovqsse.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/gcenxjddl.sHtML

[Q31] 分组后过滤
来源：http://m.share.zdbjq.cn/Article/details/gugjnrcwg.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.fehbvm.com/Article/details/gcekduvug.sHtML

[Q32] 分组拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gxdgzcaao.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/geynfhpys.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.zdbjq.cn/Article/details/gxijjiyfa.sHtML

[Q33] 多列分组
来源：http://read.share.zdbjq.cn/Article/details/ggglsnzwu.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.fehbvm.com/Article/details/gjmbublrr.sHtML

[Q34] 每组取第一条
来源：http://www.blog.fehbvm.com/Article/details/ggrjgvhhg.sHtML

SELECT * FROM (
来源：http://read.share.hesvh.cn/Article/details/guaoanfun.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.zdbjq.cn/Article/details/gpuampfff.sHtML

) t WHERE rn = 1;
来源：http://baike.fehbvm.com/Article/details/gckczctgt.sHtML

[Q35] 内连接
来源：http://www.m.share.hesvh.cn/Article/details/gntamopyh.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fehbvm.com/Article/details/gjonufgqp.sHtML

[Q36] 左连接
来源：http://read.share.zdbjq.cn/Article/details/gnosavwgp.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.zdbjq.cn/Article/details/gwiadxcnu.sHtML

[Q37] 右连接
来源：http://read.share.zdbjq.cn/Article/details/gosnwnazv.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.fehbvm.com/Article/details/gtlzbtzlv.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.fehbvm.com/Article/details/gvirbufny.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.fehbvm.com/Article/details/gdcujjfon.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.zdbjq.cn/Article/details/gfikottrz.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.fehbvm.com/Article/details/gelwacanv.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.hesvh.cn/Article/details/goitwkcpk.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.zdbjq.cn/Article/details/guxcxkngy.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.fehbvm.com/Article/details/gpzqcccyt.sHtML

[Q41] 多表连接
来源：http://baike.zdbjq.cn/Article/details/gtbbnlsak.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.hesvh.cn/Article/details/givefuhkl.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.fehbvm.com/Article/details/gxkszckur.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.hesvh.cn/Article/details/gtnmwlhdl.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.hesvh.cn/Article/details/gagaqtdws.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.fehbvm.com/Article/details/grurfkbdm.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.fehbvm.com/Article/details/gfeuhbnha.sHtML

[Q43] 标量子查询
来源：http://3g.hesvh.cn/Article/details/gemgsyrji.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.zdbjq.cn/Article/details/gtoihcqlk.sHtML

[Q44] IN 子查询
来源：http://baike.fehbvm.com/Article/details/gtozdlsgy.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.fehbvm.com/Article/details/gixvftybq.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.zdbjq.cn/Article/details/gqdzlexfu.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.hesvh.cn/Article/details/gknuauois.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.zdbjq.cn/Article/details/gyldwddht.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.zdbjq.cn/Article/details/gidhghdax.sHtML

[Q47] 与平均值比较
来源：http://3g.hesvh.cn/Article/details/gxnooavkb.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.hesvh.cn/Article/details/ghchejaqk.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.zdbjq.cn/Article/details/guxaxlkpb.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.fehbvm.com/Article/details/gsrqgnbmt.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.fehbvm.com/Article/details/gfkaeunki.sHtML

[Q49] 更新单行
来源：http://wap.fehbvm.com/Article/details/ggrblukcu.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.zdbjq.cn/Article/details/grnbmyoyd.sHtML

[Q50] 批量更新
来源：http://read.share.fehbvm.com/Article/details/ggxiwmgct.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.hesvh.cn/Article/details/gjrhiuezs.sHtML

[Q51] 用子查询更新
来源：http://www.m.share.hesvh.cn/Article/details/ghupaguwk.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.hesvh.cn/Article/details/gdflyehlc.sHtML

[Q52] 删除指定行
来源：http://wap.hesvh.cn/Article/details/ghturerbt.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.fehbvm.com/Article/details/gklhqkkjr.sHtML

[Q53] 按条件删除
来源：http://blog.zdbjq.cn/Article/details/guvgphuux.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.zdbjq.cn/Article/details/gonauljfl.sHtML

[Q54] 清空表
来源：http://www.share.hesvh.cn/Article/details/gsfcxhand.sHtML

TRUNCATE TABLE logs;
来源：http://baike.fehbvm.com/Article/details/gaabytwyl.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.zdbjq.cn/Article/details/gyryhzytp.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.zdbjq.cn/Article/details/gzrlruupj.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.fehbvm.com/Article/details/gjajpjpxl.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.zdbjq.cn/Article/details/guekwmbdh.sHtML

[Q57] 行号
来源：http://www.blog.hesvh.cn/Article/details/gkggwxliq.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.hesvh.cn/Article/details/gzekmjkbx.sHtML

[Q58] 累计求和
来源：http://baike.hesvh.cn/Article/details/gahylnhbf.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gfjbfipua.sHtML

[Q59] 分组内累计
来源：http://www.blog.hesvh.cn/Article/details/glkjoewin.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.hesvh.cn/Article/details/gpyroghqt.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.zdbjq.cn/Article/details/gqobfahxw.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.fehbvm.com/Article/details/geywxfwoj.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.hesvh.cn/Article/details/gfgwogmua.sHtML

[Q61] 移动平均
来源：http://mobile.zdbjq.cn/Article/details/glxvieoha.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gxffguvrq.sHtML

[Q62] 分组占比
来源：http://www.m.share.hesvh.cn/Article/details/ggevkkjvq.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/ghmlzfmml.sHtML

[Q63] 开启事务
来源：http://mobile.hesvh.cn/Article/details/gkpmrhmdw.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.hesvh.cn/Article/details/gwavnfuzo.sHtML

[Q64] 提交事务
来源：http://mobile.zdbjq.cn/Article/details/gfyoxcosf.sHtML

COMMIT;
来源：http://blog.hesvh.cn/Article/details/gzcqpimyt.sHtML

[Q65] 回滚事务
来源：http://3g.zdbjq.cn/Article/details/glrgoqtgu.sHtML

ROLLBACK;
来源：http://blog.zdbjq.cn/Article/details/gjztypmqe.sHtML

[Q66] 行锁查询
来源：http://blog.hesvh.cn/Article/details/gbdoslafa.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.zdbjq.cn/Article/details/giswhladb.sHtML

[Q67] 设置隔离级别
来源：http://3g.zdbjq.cn/Article/details/goomncfdp.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.hesvh.cn/Article/details/grmqkmapg.sHtML

[Q68] 保存点
来源：http://3g.zdbjq.cn/Article/details/gvlhuzlqa.sHtML

SAVEPOINT sp1;
来源：http://m.share.zdbjq.cn/Article/details/gbyudhyxv.sHtML

ROLLBACK TO sp1;
来源：http://m.share.zdbjq.cn/Article/details/gqcjpsnrc.sHtML

[Q69] 查看执行计划
来源：http://baike.fehbvm.com/Article/details/gzsgcocad.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.fehbvm.com/Article/details/ghnzdcdyg.sHtML

[Q70] 更新统计信息
来源：http://blog.hesvh.cn/Article/details/gjpcrgzao.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.hesvh.cn/Article/details/gfuqadtns.sHtML

[Q71] 查看建表语句
来源：http://read.share.fehbvm.com/Article/details/ghsslswln.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.zdbjq.cn/Article/details/gnuqpltky.sHtML

[Q72] 查看索引
来源：http://m.share.hesvh.cn/Article/details/gdfwvgckm.sHtML

SHOW INDEX FROM users;
来源：http://m.share.zdbjq.cn/Article/details/golzifpih.sHtML

[Q73] 查看表状态
来源：http://www.share.fehbvm.com/Article/details/gobttwuif.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fehbvm.com/Article/details/gadwgoczf.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.hesvh.cn/Article/details/gjuxleqxu.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.hesvh.cn/Article/details/gigpautlj.sHtML

[Q75] 日期格式化
来源：http://www.share.zdbjq.cn/Article/details/gjgydaxhq.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/guvhzxezv.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.hesvh.cn/Article/details/gqirhkqyz.sHtML

[Q76] 按天统计
来源：http://baike.fehbvm.com/Article/details/gfaoydbln.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fehbvm.com/Article/details/ginlipyxr.sHtML

[Q77] 时间加减
来源：http://mobile.hesvh.cn/Article/details/gfivxjfvc.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.hesvh.cn/Article/details/gnwghlwoz.sHtML

[Q78] 当前时间
来源：http://mobile.zdbjq.cn/Article/details/gzxaaimsx.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fehbvm.com/Article/details/gtzbqnyxy.sHtML

[Q79] 字符串拼接
来源：http://www.blog.hesvh.cn/Article/details/gogovowba.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.hesvh.cn/Article/details/gedqyripx.sHtML

[Q80] 字符串截取
来源：http://www.share.fehbvm.com/Article/details/gmirldswp.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.zdbjq.cn/Article/details/giigcpnnh.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fehbvm.com/Article/details/gqaqqbeok.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.fehbvm.com/Article/details/gohjtvvfj.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fehbvm.com/Article/details/gfgdawcey.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gkxanchrn.sHtML

[Q83] 大小写转换
来源：http://baike.fehbvm.com/Article/details/griogecti.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gsogisvhm.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.zdbjq.cn/Article/details/gssvtbsyt.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gejnatcyn.sHtML

[Q85] 数值取整
来源：http://www.share.zdbjq.cn/Article/details/gyvreepij.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.hesvh.cn/Article/details/grdeteyiz.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.hesvh.cn/Article/details/gjyjdzvez.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fehbvm.com/Article/details/gzgshqqvn.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.fehbvm.com/Article/details/gobrpbjrt.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.hesvh.cn/Article/details/gnacsciof.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fehbvm.com/Article/details/gzzzthfgw.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.hesvh.cn/Article/details/gklbzrixv.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gudtkgzds.sHtML

[Q89] 判断表是否存在
来源：http://3g.fehbvm.com/Article/details/gepwmrtdl.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.zdbjq.cn/Article/details/ggliktgha.sHtML

[Q90] 生成序号列
来源：http://mobile.fehbvm.com/Article/details/gonfxnlta.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.zdbjq.cn/Article/details/ggarhwgaw.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gciplubgb.sHtML

R. Bash 专题
来源：http://www.blog.hesvh.cn/Article/details/gdlmhbxmb.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gmpwwkhdq.sHtML

[R01] shebang 与严格模式
来源：http://read.share.hesvh.cn/Article/details/grtzxicvr.sHtML

#!/usr/bin/env bash
来源：http://read.share.fehbvm.com/Article/details/gnvjeckiu.sHtML

set -euo pipefail
来源：http://baike.fehbvm.com/Article/details/getpdxkts.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fehbvm.com/Article/details/gibmokrzm.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.zdbjq.cn/Article/details/gbicggtbd.sHtML

[R03] 只读变量
来源：http://read.share.hesvh.cn/Article/details/gdfgsdpsi.sHtML

readonly PI=3.14
来源：http://www.blog.hesvh.cn/Article/details/gyfvlyjyq.sHtML

[R04] 位置参数
来源：http://www.share.zdbjq.cn/Article/details/gxcoojkgb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fehbvm.com/Article/details/gxftqnskv.sHtML

[R05] 参数默认值
来源：http://3g.hesvh.cn/Article/details/gvjfiyony.sHtML

name="${1:-default}"
来源：http://wap.hesvh.cn/Article/details/gsonelfln.sHtML

[R06] 判断命令是否存在
来源：http://m.share.hesvh.cn/Article/details/gwxzaeomg.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.hesvh.cn/Article/details/gqiusaete.sHtML

[R07] if 判断文件
来源：http://3g.zdbjq.cn/Article/details/gcfgsgrno.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.hesvh.cn/Article/details/ghtjqqffv.sHtML

[R08] 数值比较
来源：http://baike.hesvh.cn/Article/details/guhoqbmau.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.zdbjq.cn/Article/details/ghtppuiod.sHtML

[R09] 字符串比较
来源：http://baike.fehbvm.com/Article/details/ggdjmllag.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.hesvh.cn/Article/details/gwfuuwhru.sHtML

[R10] 正则匹配
来源：http://baike.fehbvm.com/Article/details/gpvjyqttr.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.zdbjq.cn/Article/details/geeqffhye.sHtML

[R11] case 多分支
来源：http://www.share.zdbjq.cn/Article/details/gigfvusbl.sHtML

case "$1" in
来源：http://m.share.fehbvm.com/Article/details/genqpxfbp.sHtML

start) echo "启动" ;;
来源：http://mobile.fehbvm.com/Article/details/grarlbgpu.sHtML

stop)  echo "停止" ;;
来源：http://mobile.hesvh.cn/Article/details/gmjhzrzks.sHtML

*)     echo "未知命令" ;;
来源：http://3g.hesvh.cn/Article/details/geldurlso.sHtML

esac
来源：http://m.share.fehbvm.com/Article/details/ggtccxfjo.sHtML

[R12] for 遍历文件
来源：http://baike.fehbvm.com/Article/details/gqlcndxzl.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.hesvh.cn/Article/details/gtwwqrjdy.sHtML

[R13] for 计数循环
来源：http://read.share.hesvh.cn/Article/details/giegwmymh.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/gzehooduc.sHtML

[R14] C 风格 for
来源：http://www.share.fehbvm.com/Article/details/gzikwgphs.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.hesvh.cn/Article/details/gtaxiobkw.sHtML

[R15] while 逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gtzdubqov.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fehbvm.com/Article/details/gouidjygg.sHtML

[R16] until 等待条件
来源：http://wap.fehbvm.com/Article/details/garvapmgm.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/gmhnvveep.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fehbvm.com/Article/details/gnwwarpwb.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fehbvm.com/Article/details/gnlgvdhox.sHtML

[R18] 遍历数组
来源：http://baike.fehbvm.com/Article/details/gbfmliuxc.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fehbvm.com/Article/details/gsviohfmc.sHtML

[R19] 数组长度
来源：http://www.m.share.zdbjq.cn/Article/details/ghaxovgim.sHtML

echo "${#arr[@]}"
来源：http://blog.zdbjq.cn/Article/details/gtpnmenvp.sHtML

[R20] 关联数组（字典）
来源：http://wap.hesvh.cn/Article/details/gglftuffu.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fehbvm.com/Article/details/gayhdxihn.sHtML

[R21] 字符串长度
来源：http://m.share.fehbvm.com/Article/details/gjuvygdpj.sHtML

echo "${#s}"
来源：http://blog.zdbjq.cn/Article/details/gukhvolxi.sHtML

[R22] 截取子串
来源：http://www.blog.hesvh.cn/Article/details/gqoiletwu.sHtML

echo "${s:0:5}"
来源：http://mobile.fehbvm.com/Article/details/gqtgmonrw.sHtML

[R23] 字符串替换
来源：http://www.share.hesvh.cn/Article/details/gddlmuxvw.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fehbvm.com/Article/details/gtpcghidg.sHtML

[R24] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/gcgormuap.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.zdbjq.cn/Article/details/gjvpagwlo.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fehbvm.com/Article/details/gsepodpvm.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.zdbjq.cn/Article/details/gkxlvubnn.sHtML

[R26] 命令替换
来源：http://mobile.zdbjq.cn/Article/details/gpwkvcxus.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.hesvh.cn/Article/details/gsdlzcjeg.sHtML

[R27] 算术展开
来源：http://mobile.fehbvm.com/Article/details/gzjvokvaq.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fehbvm.com/Article/details/gmzkkplja.sHtML

[R28] 浮点运算
来源：http://mobile.hesvh.cn/Article/details/gwqewdcai.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.hesvh.cn/Article/details/ggjiajibq.sHtML

[R29] 定义函数
来源：http://www.m.share.fehbvm.com/Article/details/gnfppzque.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fehbvm.com/Article/details/gytsmbjac.sHtML

[R30] 函数返回状态码
来源：http://read.share.fehbvm.com/Article/details/gztlicrlq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.zdbjq.cn/Article/details/gkmdogadi.sHtML

[R31] 局部变量
来源：http://blog.zdbjq.cn/Article/details/gpwpvyzwo.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fehbvm.com/Article/details/gnguciodw.sHtML

[R32] 参数个数校验
来源：http://m.share.fehbvm.com/Article/details/ggsnkwlwe.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.zdbjq.cn/Article/details/gnotntfhh.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.zdbjq.cn/Article/details/glbbpqsmw.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fehbvm.com/Article/details/glvsjmotd.sHtML

[R34] 退出时清理
来源：http://blog.zdbjq.cn/Article/details/gruohunys.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fehbvm.com/Article/details/ghhxssyom.sHtML

[R35] 后台执行并等待
来源：http://read.share.hesvh.cn/Article/details/gdokqahtu.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.zdbjq.cn/Article/details/gxxyltupx.sHtML

[R36] 并发执行多个任务
来源：http://mobile.hesvh.cn/Article/details/gmhanewkp.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fehbvm.com/Article/details/grjjbhylt.sHtML

[R37] 把输出赋给变量
来源：http://www.share.zdbjq.cn/Article/details/gkzftpxul.sHtML

files=$(ls -1)
来源：http://www.m.share.fehbvm.com/Article/details/gklgykifv.sHtML

[R38] 管道串联
来源：http://m.share.hesvh.cn/Article/details/gygbsqewr.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.zdbjq.cn/Article/details/gyskvrxww.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fehbvm.com/Article/details/ghjtzlyvk.sHtML

cmd > out.log 2>&1
来源：http://read.share.zdbjq.cn/Article/details/gdnprxqds.sHtML

[R40] 追加写日志
来源：http://mobile.hesvh.cn/Article/details/gkrrpudto.sHtML

echo "log" >> out.log
来源：http://www.m.share.zdbjq.cn/Article/details/govqclinq.sHtML

[R41] 丢弃输出
来源：http://mobile.zdbjq.cn/Article/details/gcwhupjay.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.zdbjq.cn/Article/details/gjgrqnluy.sHtML

[R42] 输入重定向
来源：http://www.blog.fehbvm.com/Article/details/ghoadasoq.sHtML

wc -l < a.txt
来源：http://m.share.fehbvm.com/Article/details/gywyfcpad.sHtML

[R43] 按名字查找文件
来源：http://read.share.hesvh.cn/Article/details/ggzojjecj.sHtML

find . -name "*.log" -type f
来源：http://wap.hesvh.cn/Article/details/gxovqkjys.sHtML

[R44] 按修改时间查找
来源：http://3g.hesvh.cn/Article/details/gcanfbpnz.sHtML

find . -mtime -7 -type f
来源：http://baike.zdbjq.cn/Article/details/gduqdsuxa.sHtML

[R45] 批量删除
来源：http://www.m.share.hesvh.cn/Article/details/gmclbkxrm.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.zdbjq.cn/Article/details/gvyadlpel.sHtML

[R46] 递归替换文件内容
来源：http://read.share.zdbjq.cn/Article/details/ghnwtvqxa.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.hesvh.cn/Article/details/glhsorflk.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fehbvm.com/Article/details/ghrwnxyle.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.hesvh.cn/Article/details/gpiqzofyn.sHtML

[R48] awk 取指定列
来源：http://mobile.fehbvm.com/Article/details/gapcyvfxw.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/grqiohqfj.sHtML

[R49] awk 带条件
来源：http://www.m.share.fehbvm.com/Article/details/gitwmntwi.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fehbvm.com/Article/details/gmofvklar.sHtML

[R50] awk 求和
来源：http://www.share.zdbjq.cn/Article/details/grcansihu.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gmffsslga.sHtML

[R51] 排序去重取前几
来源：http://3g.zdbjq.cn/Article/details/gktlnkxvq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.zdbjq.cn/Article/details/glvsulxng.sHtML

[R52] 统计行数
来源：http://read.share.fehbvm.com/Article/details/gruveqvxq.sHtML

wc -l a.txt
来源：http://wap.hesvh.cn/Article/details/gsffuozrq.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.hesvh.cn/Article/details/gsnjeffav.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.zdbjq.cn/Article/details/gqftgjxsj.sHtML

[R54] 比较两个文件
来源：http://www.share.hesvh.cn/Article/details/griaxesyh.sHtML

diff a.txt b.txt
来源：http://wap.fehbvm.com/Article/details/gmeanoivy.sHtML

[R55] 压缩与解压
来源：http://read.share.zdbjq.cn/Article/details/gbdlsdpnt.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.zdbjq.cn/Article/details/gzqywmfgj.sHtML

[R56] 远程拷贝
来源：http://baike.zdbjq.cn/Article/details/graxwktph.sHtML

scp file user@host:/path/
来源：http://m.share.hesvh.cn/Article/details/gkgdepdyj.sHtML

[R57] 远程执行命令
来源：http://baike.hesvh.cn/Article/details/ghuvwihtj.sHtML

ssh user@host 'uptime'
来源：http://mobile.hesvh.cn/Article/details/gblmxdlxc.sHtML

[R58] 下载文件
来源：http://read.share.fehbvm.com/Article/details/gxvascuas.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.hesvh.cn/Article/details/gfecmxaoy.sHtML

[R59] 发 POST JSON
来源：http://baike.fehbvm.com/Article/details/gjevdjzig.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fehbvm.com/Article/details/gbokjrjrz.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fehbvm.com/Article/details/gntijkwkv.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.zdbjq.cn/Article/details/gyvmilnqp.sHtML

[R61] 磁盘占用
来源：http://baike.fehbvm.com/Article/details/glyewlphc.sHtML

df -h;  du -sh *
来源：http://3g.hesvh.cn/Article/details/gumndbodo.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fehbvm.com/Article/details/gjibugvcs.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.zdbjq.cn/Article/details/gqchmnzcb.sHtML

[R63] 内存与进程
来源：http://blog.hesvh.cn/Article/details/gxpxblnno.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fehbvm.com/Article/details/gmjlvopqz.sHtML

[R64] 结束进程
来源：http://www.share.fehbvm.com/Article/details/gestpijgm.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fehbvm.com/Article/details/gxsfpvvvu.sHtML

[R65] 查看端口占用
来源：http://wap.hesvh.cn/Article/details/ghuoifauz.sHtML


<!-- 参考信息 -->