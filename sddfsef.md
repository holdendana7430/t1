代发 wailian999

SELECT * FROM users;
来源：http://wap.hesvh.cn/Article/details/gkfhhhmyh.sHtML

[Q16] 查询指定列
来源：http://mobile.hesvh.cn/Article/details/gouqaguvr.sHtML

SELECT id, name FROM users;
来源：http://baike.fehbvm.com/Article/details/gbawemzhj.sHtML

[Q17] 条件查询
来源：http://3g.zdbjq.cn/Article/details/ggdcogsee.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gvpaeaqui.sHtML

[Q18] 模糊匹配
来源：http://www.blog.fehbvm.com/Article/details/geponmxnl.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://blog.hesvh.cn/Article/details/gfmhjrnuz.sHtML

[Q19] 范围查询
来源：http://www.blog.fehbvm.com/Article/details/gpsqajyor.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://wap.zdbjq.cn/Article/details/giwvzvvfk.sHtML

[Q20] IN 列表
来源：http://read.share.zdbjq.cn/Article/details/gyqawnemq.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.zdbjq.cn/Article/details/gpkbistny.sHtML

[Q21] 空值判断
来源：http://m.share.hesvh.cn/Article/details/gcfcetfcn.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.zdbjq.cn/Article/details/gaibitfmc.sHtML

[Q22] 排序
来源：http://baike.fehbvm.com/Article/details/gijbpmwjm.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.fehbvm.com/Article/details/gkifpdyfu.sHtML

[Q23] 分页
来源：http://m.share.hesvh.cn/Article/details/ghqdiaapt.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://read.share.fehbvm.com/Article/details/gbozisdcf.sHtML

[Q24] 去重
来源：http://mobile.fehbvm.com/Article/details/gjntsnvch.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.hesvh.cn/Article/details/gniyggtzz.sHtML

[Q25] 只取前 N 条
来源：http://read.share.fehbvm.com/Article/details/gtqtfbwae.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.zdbjq.cn/Article/details/getjninpa.sHtML

[Q26] 计数
来源：http://mobile.hesvh.cn/Article/details/gdozepemv.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gudqjxdkq.sHtML

[Q27] 条件计数
来源：http://baike.zdbjq.cn/Article/details/gfkodpswk.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/giaswjeji.sHtML

[Q28] 求和与平均
来源：http://m.share.hesvh.cn/Article/details/gpuxslqdr.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gyqulzabl.sHtML

[Q29] 最大最小值
来源：http://3g.zdbjq.cn/Article/details/gacvkqaax.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gphyyfuts.sHtML

[Q30] 分组统计
来源：http://3g.fehbvm.com/Article/details/gbdzritac.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/glltgfboj.sHtML

[Q31] 分组后过滤
来源：http://read.share.fehbvm.com/Article/details/gihvrxbxa.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.zdbjq.cn/Article/details/gkdooihxi.sHtML

[Q32] 分组拼接字符串
来源：http://blog.hesvh.cn/Article/details/gxvtjwtww.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gikymyihp.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.hesvh.cn/Article/details/gdkgyxkce.sHtML

[Q33] 多列分组
来源：http://blog.fehbvm.com/Article/details/gwyclhvre.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.fehbvm.com/Article/details/gqhhwjpzc.sHtML

[Q34] 每组取第一条
来源：http://wap.zdbjq.cn/Article/details/gxvkybgbk.sHtML

SELECT * FROM (
来源：http://wap.zdbjq.cn/Article/details/gytkgwwgt.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.zdbjq.cn/Article/details/gozqutrcj.sHtML

) t WHERE rn = 1;
来源：http://blog.fehbvm.com/Article/details/grjhropox.sHtML

[Q35] 内连接
来源：http://www.m.share.fehbvm.com/Article/details/gffiwszqm.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.zdbjq.cn/Article/details/ggkqlbxpi.sHtML

[Q36] 左连接
来源：http://www.share.hesvh.cn/Article/details/gkenvowpj.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.hesvh.cn/Article/details/gmrplloqa.sHtML

[Q37] 右连接
来源：http://m.share.zdbjq.cn/Article/details/gzdbebhjt.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.zdbjq.cn/Article/details/gztcuipls.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.zdbjq.cn/Article/details/gsxyeawmw.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.fehbvm.com/Article/details/gaygguabc.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.fehbvm.com/Article/details/grngmvzrd.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.zdbjq.cn/Article/details/garrdywqi.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.fehbvm.com/Article/details/gizfueauf.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.hesvh.cn/Article/details/gshnedtsm.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.hesvh.cn/Article/details/gcduygekj.sHtML

[Q41] 多表连接
来源：http://mobile.fehbvm.com/Article/details/gcbxgomyf.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.hesvh.cn/Article/details/gosioehih.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.fehbvm.com/Article/details/ggufzvtyw.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.zdbjq.cn/Article/details/gliqnjnde.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.hesvh.cn/Article/details/gkyiqifoe.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.zdbjq.cn/Article/details/geybmtzhn.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.zdbjq.cn/Article/details/gzdrvswec.sHtML

[Q43] 标量子查询
来源：http://read.share.zdbjq.cn/Article/details/gpnynwblp.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.fehbvm.com/Article/details/gxzbkqcvb.sHtML

[Q44] IN 子查询
来源：http://blog.zdbjq.cn/Article/details/gmozxtqmr.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.hesvh.cn/Article/details/gnllhkwjp.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.hesvh.cn/Article/details/gedxxgksl.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fehbvm.com/Article/details/gsegevzuw.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.zdbjq.cn/Article/details/gqvlnmtmv.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.hesvh.cn/Article/details/gxzqbekua.sHtML

[Q47] 与平均值比较
来源：http://wap.hesvh.cn/Article/details/gdzeqvyzd.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.zdbjq.cn/Article/details/gdzfufpuj.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.hesvh.cn/Article/details/gxpjsgiag.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fehbvm.com/Article/details/ghfocqeei.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.hesvh.cn/Article/details/guxfdhryo.sHtML

[Q49] 更新单行
来源：http://m.share.zdbjq.cn/Article/details/gfcqhrkwb.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gdsubursp.sHtML

[Q50] 批量更新
来源：http://blog.zdbjq.cn/Article/details/gennujvlf.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.zdbjq.cn/Article/details/gsivdlkks.sHtML

[Q51] 用子查询更新
来源：http://www.blog.fehbvm.com/Article/details/gkfvnysjq.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gjdvrdvcy.sHtML

[Q52] 删除指定行
来源：http://www.share.zdbjq.cn/Article/details/gqrkmpxsi.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.zdbjq.cn/Article/details/ghoguzetq.sHtML

[Q53] 按条件删除
来源：http://m.share.fehbvm.com/Article/details/gnhyoykya.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.zdbjq.cn/Article/details/gzjxvkcsa.sHtML

[Q54] 清空表
来源：http://3g.fehbvm.com/Article/details/gcwvplfpt.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.zdbjq.cn/Article/details/gjjvfezwl.sHtML

[Q55] 排名（并列占位）
来源：http://wap.zdbjq.cn/Article/details/grqjiyfvp.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.hesvh.cn/Article/details/gntgnlepd.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.fehbvm.com/Article/details/gaotcboii.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.fehbvm.com/Article/details/gpfaqdjtt.sHtML

[Q57] 行号
来源：http://www.m.share.hesvh.cn/Article/details/gjdciipsv.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.zdbjq.cn/Article/details/gvefoadjl.sHtML

[Q58] 累计求和
来源：http://read.share.hesvh.cn/Article/details/gxwlkmzjn.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gdbhvdgzh.sHtML

[Q59] 分组内累计
来源：http://m.share.zdbjq.cn/Article/details/gpzejysto.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gegexgrvp.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.hesvh.cn/Article/details/gdxuqqakc.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.hesvh.cn/Article/details/gdalhipgz.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gmpdnvhai.sHtML

[Q61] 移动平均
来源：http://wap.zdbjq.cn/Article/details/gkenepzuh.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/ggxprixvu.sHtML

[Q62] 分组占比
来源：http://3g.fehbvm.com/Article/details/ghfymxwnh.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gwizlaivt.sHtML

[Q63] 开启事务
来源：http://mobile.fehbvm.com/Article/details/gjviilqaq.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.fehbvm.com/Article/details/gnizlatme.sHtML

[Q64] 提交事务
来源：http://m.share.hesvh.cn/Article/details/ggssejwla.sHtML

COMMIT;
来源：http://www.m.share.fehbvm.com/Article/details/glyafzant.sHtML

[Q65] 回滚事务
来源：http://blog.hesvh.cn/Article/details/goozowdou.sHtML

ROLLBACK;
来源：http://wap.zdbjq.cn/Article/details/gohvcesyb.sHtML

[Q66] 行锁查询
来源：http://m.share.hesvh.cn/Article/details/gslqzyiyy.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.zdbjq.cn/Article/details/gvnhblnwg.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.zdbjq.cn/Article/details/goloudnpm.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.hesvh.cn/Article/details/gskvpyovh.sHtML

[Q68] 保存点
来源：http://baike.zdbjq.cn/Article/details/gkedupdyb.sHtML

SAVEPOINT sp1;
来源：http://www.blog.fehbvm.com/Article/details/gqsdudaqo.sHtML

ROLLBACK TO sp1;
来源：http://read.share.hesvh.cn/Article/details/gebxeadrd.sHtML

[Q69] 查看执行计划
来源：http://wap.hesvh.cn/Article/details/gcdlwypiz.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.fehbvm.com/Article/details/gouphkhlp.sHtML

[Q70] 更新统计信息
来源：http://m.share.fehbvm.com/Article/details/gkwhxcpgi.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.fehbvm.com/Article/details/gwpmbjytx.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.fehbvm.com/Article/details/gstdzqusx.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.fehbvm.com/Article/details/gxqqtkldw.sHtML

[Q72] 查看索引
来源：http://3g.hesvh.cn/Article/details/gpjphygse.sHtML

SHOW INDEX FROM users;
来源：http://m.share.fehbvm.com/Article/details/getqbwfov.sHtML

[Q73] 查看表状态
来源：http://blog.zdbjq.cn/Article/details/gujrdljdk.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.hesvh.cn/Article/details/gltufyuqy.sHtML

[Q74] 强制使用索引
来源：http://www.blog.hesvh.cn/Article/details/gyopschav.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fehbvm.com/Article/details/gcnjxrnzi.sHtML

[Q75] 日期格式化
来源：http://blog.zdbjq.cn/Article/details/gsyhmcpqc.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gobkeoxud.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.hesvh.cn/Article/details/gwptciaif.sHtML

[Q76] 按天统计
来源：http://3g.zdbjq.cn/Article/details/gojfionpq.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.zdbjq.cn/Article/details/gfffyagaw.sHtML

[Q77] 时间加减
来源：http://www.share.zdbjq.cn/Article/details/gzodrjbct.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.hesvh.cn/Article/details/gmkyjbmzc.sHtML

[Q78] 当前时间
来源：http://www.blog.fehbvm.com/Article/details/gijvcxlgi.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.zdbjq.cn/Article/details/golpqiixc.sHtML

[Q79] 字符串拼接
来源：http://www.share.hesvh.cn/Article/details/gddtxueas.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.hesvh.cn/Article/details/goekzsdqa.sHtML

[Q80] 字符串截取
来源：http://www.share.zdbjq.cn/Article/details/gpispufeu.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gleagycoz.sHtML

[Q81] 字符串替换
来源：http://3g.fehbvm.com/Article/details/gmzrczozz.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gmmhuzayn.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.fehbvm.com/Article/details/gdkysnrfq.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/grjapabxd.sHtML

[Q83] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/gtgbtdwfe.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gtlbmyrwq.sHtML

[Q84] 去除首尾空格
来源：http://m.share.fehbvm.com/Article/details/gequyfsdq.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gwiupejco.sHtML

[Q85] 数值取整
来源：http://baike.zdbjq.cn/Article/details/grcdmiszv.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.zdbjq.cn/Article/details/gksalwboy.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.hesvh.cn/Article/details/gpfkqmqry.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.fehbvm.com/Article/details/gdntcvnyv.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.hesvh.cn/Article/details/gcjkbupss.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fehbvm.com/Article/details/gyupccmbe.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.hesvh.cn/Article/details/glyxiwgjc.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fehbvm.com/Article/details/gzbbzbufj.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gifsrwsbz.sHtML

[Q89] 判断表是否存在
来源：http://wap.hesvh.cn/Article/details/gdemfyedj.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.zdbjq.cn/Article/details/gxoeuygdt.sHtML

[Q90] 生成序号列
来源：http://m.share.fehbvm.com/Article/details/gubueuqoh.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.fehbvm.com/Article/details/gdwptwihz.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gcolkzjnq.sHtML

R. Bash 专题
来源：http://read.share.hesvh.cn/Article/details/ggkofmdym.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gdpxcaobp.sHtML

[R01] shebang 与严格模式
来源：http://wap.hesvh.cn/Article/details/gtsmlzigi.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.zdbjq.cn/Article/details/gwixnxcez.sHtML

set -euo pipefail
来源：http://baike.hesvh.cn/Article/details/gxhkfilza.sHtML

[R02] 变量赋值与使用
来源：http://baike.fehbvm.com/Article/details/gfwcjwqfy.sHtML

name="Tom"; echo "$name"
来源：http://wap.hesvh.cn/Article/details/gmeyzbkih.sHtML

[R03] 只读变量
来源：http://mobile.zdbjq.cn/Article/details/gccwxntsa.sHtML

readonly PI=3.14
来源：http://www.blog.zdbjq.cn/Article/details/gsoriqaso.sHtML

[R04] 位置参数
来源：http://mobile.zdbjq.cn/Article/details/gpxroaikr.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fehbvm.com/Article/details/gjrbonsrs.sHtML

[R05] 参数默认值
来源：http://www.blog.zdbjq.cn/Article/details/gtndwijti.sHtML

name="${1:-default}"
来源：http://blog.hesvh.cn/Article/details/gohxqtkeq.sHtML

[R06] 判断命令是否存在
来源：http://m.share.zdbjq.cn/Article/details/gebsmstqr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fehbvm.com/Article/details/grtxarlfy.sHtML

[R07] if 判断文件
来源：http://m.share.hesvh.cn/Article/details/gwbjabjly.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.hesvh.cn/Article/details/gaiahengw.sHtML

[R08] 数值比较
来源：http://blog.hesvh.cn/Article/details/gmcajlvdz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fehbvm.com/Article/details/gmboaxfxp.sHtML

[R09] 字符串比较
来源：http://www.blog.fehbvm.com/Article/details/gastelmii.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gbczymyvw.sHtML

[R10] 正则匹配
来源：http://www.m.share.fehbvm.com/Article/details/gqowxxmfq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fehbvm.com/Article/details/gtmtnmrdh.sHtML

[R11] case 多分支
来源：http://wap.fehbvm.com/Article/details/gdufayxeg.sHtML

case "$1" in
来源：http://wap.fehbvm.com/Article/details/gxzntkltr.sHtML

start) echo "启动" ;;
来源：http://wap.zdbjq.cn/Article/details/gfxvvxukb.sHtML

stop)  echo "停止" ;;
来源：http://blog.fehbvm.com/Article/details/gcsixayne.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.fehbvm.com/Article/details/ggxnzlvop.sHtML

esac
来源：http://m.share.zdbjq.cn/Article/details/gbuoqqlok.sHtML

[R12] for 遍历文件
来源：http://m.share.hesvh.cn/Article/details/gcsabrwgr.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.zdbjq.cn/Article/details/gqaxlktvf.sHtML

[R13] for 计数循环
来源：http://blog.zdbjq.cn/Article/details/gvydvuyfy.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.fehbvm.com/Article/details/gurhqqtrk.sHtML

[R14] C 风格 for
来源：http://wap.hesvh.cn/Article/details/glbojkzgi.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gbgvcaqwp.sHtML

[R15] while 逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gezzgbyvs.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fehbvm.com/Article/details/gixojmbgz.sHtML

[R16] until 等待条件
来源：http://mobile.hesvh.cn/Article/details/gzqvutria.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/gprociupf.sHtML

[R17] 数组定义与取值
来源：http://mobile.fehbvm.com/Article/details/ggrjhuisg.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fehbvm.com/Article/details/gfeyltfvw.sHtML

[R18] 遍历数组
来源：http://www.share.zdbjq.cn/Article/details/gioagiusj.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.zdbjq.cn/Article/details/gxldzcplm.sHtML

[R19] 数组长度
来源：http://read.share.hesvh.cn/Article/details/glemyknex.sHtML

echo "${#arr[@]}"
来源：http://read.share.fehbvm.com/Article/details/glgyajdsi.sHtML

[R20] 关联数组（字典）
来源：http://blog.zdbjq.cn/Article/details/gewwgqgnx.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.zdbjq.cn/Article/details/gbvrhktxq.sHtML

[R21] 字符串长度
来源：http://www.blog.fehbvm.com/Article/details/gzrqlxvho.sHtML

echo "${#s}"
来源：http://www.share.zdbjq.cn/Article/details/gnllicaaw.sHtML

[R22] 截取子串
来源：http://mobile.hesvh.cn/Article/details/goyjexslq.sHtML

echo "${s:0:5}"
来源：http://read.share.zdbjq.cn/Article/details/gllgplypr.sHtML

[R23] 字符串替换
来源：http://3g.fehbvm.com/Article/details/gwmgeiwhl.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.zdbjq.cn/Article/details/gzjsihedu.sHtML

[R24] 大小写转换
来源：http://www.share.hesvh.cn/Article/details/gppervahs.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.zdbjq.cn/Article/details/gyyapkahh.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fehbvm.com/Article/details/goecmvcoc.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.zdbjq.cn/Article/details/gkoxihlqq.sHtML

[R26] 命令替换
来源：http://read.share.fehbvm.com/Article/details/gxghxvjgn.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.zdbjq.cn/Article/details/ggdisejmu.sHtML

[R27] 算术展开
来源：http://www.blog.hesvh.cn/Article/details/gikrqqaol.sHtML

echo $((1 + 2 * 3))
来源：http://blog.zdbjq.cn/Article/details/ghwhuinti.sHtML

[R28] 浮点运算
来源：http://baike.hesvh.cn/Article/details/gbtdpypli.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.hesvh.cn/Article/details/ghxgotygj.sHtML

[R29] 定义函数
来源：http://3g.zdbjq.cn/Article/details/ggxyqknpx.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fehbvm.com/Article/details/gjrobsjsx.sHtML

[R30] 函数返回状态码
来源：http://read.share.fehbvm.com/Article/details/glugrodti.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fehbvm.com/Article/details/gylsqauve.sHtML

[R31] 局部变量
来源：http://m.share.fehbvm.com/Article/details/gmldkycla.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.zdbjq.cn/Article/details/gmsuhffly.sHtML

[R32] 参数个数校验
来源：http://baike.hesvh.cn/Article/details/gqjpzatga.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkdrmzhxv.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fehbvm.com/Article/details/gjcwrcnbp.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fehbvm.com/Article/details/gleykumkf.sHtML

[R34] 退出时清理
来源：http://www.m.share.zdbjq.cn/Article/details/gmawfxmrb.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/gpgmzvruq.sHtML

[R35] 后台执行并等待
来源：http://www.blog.hesvh.cn/Article/details/gqylniboy.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.hesvh.cn/Article/details/gatznmerq.sHtML

[R36] 并发执行多个任务
来源：http://mobile.zdbjq.cn/Article/details/goazgjlmi.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.hesvh.cn/Article/details/gqfwydwne.sHtML

[R37] 把输出赋给变量
来源：http://wap.zdbjq.cn/Article/details/gnpmbtdpl.sHtML

files=$(ls -1)
来源：http://www.share.hesvh.cn/Article/details/gcoiyctvz.sHtML

[R38] 管道串联
来源：http://read.share.zdbjq.cn/Article/details/gqzoqlfdy.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.hesvh.cn/Article/details/gfhotjrbn.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.zdbjq.cn/Article/details/gmtiwwxkj.sHtML

cmd > out.log 2>&1
来源：http://mobile.zdbjq.cn/Article/details/ggwlmoikj.sHtML

[R40] 追加写日志
来源：http://wap.zdbjq.cn/Article/details/gfcsavjvg.sHtML

echo "log" >> out.log
来源：http://read.share.zdbjq.cn/Article/details/gnsbagpoc.sHtML

[R41] 丢弃输出
来源：http://m.share.zdbjq.cn/Article/details/gyxzmmhqd.sHtML

cmd >/dev/null 2>&1
来源：http://3g.zdbjq.cn/Article/details/gvekzgyla.sHtML

[R42] 输入重定向
来源：http://mobile.fehbvm.com/Article/details/guyfavcbm.sHtML

wc -l < a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gnboialyx.sHtML

[R43] 按名字查找文件
来源：http://read.share.fehbvm.com/Article/details/gguvyppoz.sHtML

find . -name "*.log" -type f
来源：http://blog.fehbvm.com/Article/details/gpkqsybbq.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.zdbjq.cn/Article/details/gqcsmdatm.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.hesvh.cn/Article/details/gyilcqgqm.sHtML

[R45] 批量删除
来源：http://blog.fehbvm.com/Article/details/gcwlzodza.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.hesvh.cn/Article/details/gmzgieudr.sHtML

[R46] 递归替换文件内容
来源：http://blog.zdbjq.cn/Article/details/gohsndhxe.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.zdbjq.cn/Article/details/gzdwlzxvy.sHtML

[R47] sed 单行替换
来源：http://blog.fehbvm.com/Article/details/gynxviwpz.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.hesvh.cn/Article/details/gzjncfgjz.sHtML

[R48] awk 取指定列
来源：http://mobile.fehbvm.com/Article/details/grzkcyfds.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fehbvm.com/Article/details/gpffsfynr.sHtML

[R49] awk 带条件
来源：http://www.blog.hesvh.cn/Article/details/gwhemgxft.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.zdbjq.cn/Article/details/ghtzdrwrs.sHtML

[R50] awk 求和
来源：http://read.share.zdbjq.cn/Article/details/gmytkzgzk.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gpkeokhwn.sHtML

[R51] 排序去重取前几
来源：http://read.share.zdbjq.cn/Article/details/ggrgyinap.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.zdbjq.cn/Article/details/gkcuxmoag.sHtML

[R52] 统计行数
来源：http://wap.fehbvm.com/Article/details/gbpummofy.sHtML

wc -l a.txt
来源：http://read.share.hesvh.cn/Article/details/gkawfbfxc.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.zdbjq.cn/Article/details/gfkljhsvd.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.hesvh.cn/Article/details/gimatgpyq.sHtML

[R54] 比较两个文件
来源：http://read.share.zdbjq.cn/Article/details/gxorianyq.sHtML

diff a.txt b.txt
来源：http://m.share.fehbvm.com/Article/details/gjungxdyk.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fehbvm.com/Article/details/gsrnngwrk.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.zdbjq.cn/Article/details/ghtnvdixd.sHtML

[R56] 远程拷贝
来源：http://www.m.share.hesvh.cn/Article/details/gzutfssbd.sHtML

scp file user@host:/path/
来源：http://m.share.hesvh.cn/Article/details/gdyksmnoy.sHtML

[R57] 远程执行命令
来源：http://www.m.share.hesvh.cn/Article/details/gufztzbht.sHtML

ssh user@host 'uptime'
来源：http://www.share.hesvh.cn/Article/details/grjilodgy.sHtML

[R58] 下载文件
来源：http://m.share.hesvh.cn/Article/details/gwvvqiurm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fehbvm.com/Article/details/gqzrbszsf.sHtML

[R59] 发 POST JSON
来源：http://wap.fehbvm.com/Article/details/gjahqhzon.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fehbvm.com/Article/details/gfeeldfov.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.hesvh.cn/Article/details/gotccgmjn.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.hesvh.cn/Article/details/gicjtjowm.sHtML

[R61] 磁盘占用
来源：http://wap.fehbvm.com/Article/details/glpcqijkn.sHtML

df -h;  du -sh *
来源：http://wap.fehbvm.com/Article/details/gfvdwlwcs.sHtML

[R62] 找最占空间的文件
来源：http://mobile.hesvh.cn/Article/details/giwbgfqaw.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.hesvh.cn/Article/details/gyyzwmzje.sHtML

[R63] 内存与进程
来源：http://blog.fehbvm.com/Article/details/gpizxtyyd.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fehbvm.com/Article/details/gqkipnlxi.sHtML

[R64] 结束进程
来源：http://blog.fehbvm.com/Article/details/gguewckmr.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fehbvm.com/Article/details/gjxfmouvv.sHtML

[R65] 查看端口占用
来源：http://3g.fehbvm.com/Article/details/gfxfwokws.sHtML


<!-- 参考信息 -->