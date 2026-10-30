代发 wailian999

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnzcamtgl.sHtML

[Q20] IN 列表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gotmpkbms.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gejkiqtya.sHtML

[Q21] 空值判断
来源：http://wap.fanxiaobao.xyz/Article/details/gazgjjmky.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmlyuttxy.sHtML

[Q22] 排序
来源：http://m.share.fanxiaobao.xyz/Article/details/grpapbenb.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxpyrejhj.sHtML

[Q23] 分页
来源：http://m.share.fanxiaobao.xyz/Article/details/gzhckqkdz.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghtraufdm.sHtML

[Q24] 去重
来源：http://wap.fanxiaobao.xyz/Article/details/glleubktj.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxbbgsywt.sHtML

[Q25] 只取前 N 条
来源：http://m.share.fanxiaobao.xyz/Article/details/gnykcztfl.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.fanxiaobao.xyz/Article/details/gamxngfmw.sHtML

[Q26] 计数
来源：http://mobile.fanxiaobao.xyz/Article/details/gatxzqpeo.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqueftgrq.sHtML

[Q27] 条件计数
来源：http://m.share.fanxiaobao.xyz/Article/details/ghyulojtx.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcggmpnyg.sHtML

[Q28] 求和与平均
来源：http://www.share.fanxiaobao.xyz/Article/details/gykvqrhuc.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gvjdawpib.sHtML

[Q29] 最大最小值
来源：http://3g.fanxiaobao.xyz/Article/details/gxahrvban.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gybueligd.sHtML

[Q30] 分组统计
来源：http://3g.fanxiaobao.xyz/Article/details/gguxsrokq.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gupyricpp.sHtML

[Q31] 分组后过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gswocdhtb.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.fanxiaobao.xyz/Article/details/ghaprhjdo.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjvheczzs.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.fanxiaobao.xyz/Article/details/guveryrdh.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.fanxiaobao.xyz/Article/details/gaphihxct.sHtML

[Q33] 多列分组
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghkjephxs.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.fanxiaobao.xyz/Article/details/glymxxplf.sHtML

[Q34] 每组取第一条
来源：http://blog.fanxiaobao.xyz/Article/details/gmgmsgxim.sHtML

SELECT * FROM (
来源：http://baike.fanxiaobao.xyz/Article/details/gfazbdpsn.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.fanxiaobao.xyz/Article/details/gxyqytqcz.sHtML

) t WHERE rn = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gxhfmxuvf.sHtML

[Q35] 内连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqemldqph.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcshhhamt.sHtML

[Q36] 左连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gvqbfkwed.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fanxiaobao.xyz/Article/details/gemesprxu.sHtML

[Q37] 右连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gvlarmqrq.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvubgkcqq.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.fanxiaobao.xyz/Article/details/gdjkhnlks.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gakzyzwvs.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.fanxiaobao.xyz/Article/details/giegfznvh.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.fanxiaobao.xyz/Article/details/gchywboml.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.fanxiaobao.xyz/Article/details/gwwgserxr.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaeorvlyy.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnunkeguk.sHtML

[Q41] 多表连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gumdhjveb.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.fanxiaobao.xyz/Article/details/gbulqkgfi.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.fanxiaobao.xyz/Article/details/gqxtrpkfw.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.fanxiaobao.xyz/Article/details/gamgesgdy.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gbtufstwr.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.fanxiaobao.xyz/Article/details/ghxzqlufd.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.fanxiaobao.xyz/Article/details/gwzllkfoj.sHtML

[Q43] 标量子查询
来源：http://www.share.fanxiaobao.xyz/Article/details/grzonufau.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.fanxiaobao.xyz/Article/details/garaehkko.sHtML

[Q44] IN 子查询
来源：http://blog.fanxiaobao.xyz/Article/details/gxubqkalf.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.fanxiaobao.xyz/Article/details/ghoctkgec.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.fanxiaobao.xyz/Article/details/gqblouszf.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fanxiaobao.xyz/Article/details/gltvonjgw.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.fanxiaobao.xyz/Article/details/gyygrvytc.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fanxiaobao.xyz/Article/details/gpeduvory.sHtML

[Q47] 与平均值比较
来源：http://baike.fanxiaobao.xyz/Article/details/geohvzevr.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.fanxiaobao.xyz/Article/details/gyzxlrdof.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gbclioeko.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.fanxiaobao.xyz/Article/details/gbjneiuap.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghgsgkhzr.sHtML

[Q49] 更新单行
来源：http://read.share.fanxiaobao.xyz/Article/details/gdueiepeq.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gttqombfd.sHtML

[Q50] 批量更新
来源：http://read.share.fanxiaobao.xyz/Article/details/gstyeqebj.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.fanxiaobao.xyz/Article/details/gxhjgckyb.sHtML

[Q51] 用子查询更新
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmecjmkvo.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqlcbmwjp.sHtML

[Q52] 删除指定行
来源：http://wap.fanxiaobao.xyz/Article/details/gavrlzptt.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjpedwyhc.sHtML

[Q53] 按条件删除
来源：http://m.share.fanxiaobao.xyz/Article/details/gybgmvljz.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.fanxiaobao.xyz/Article/details/gkoxnofyu.sHtML

[Q54] 清空表
来源：http://read.share.fanxiaobao.xyz/Article/details/gsalzqwel.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.fanxiaobao.xyz/Article/details/grdctpiem.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.fanxiaobao.xyz/Article/details/gjmmdfous.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.fanxiaobao.xyz/Article/details/gqykvvpvx.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.fanxiaobao.xyz/Article/details/glxbbctpn.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.fanxiaobao.xyz/Article/details/gxrrwjzjw.sHtML

[Q57] 行号
来源：http://www.share.fanxiaobao.xyz/Article/details/gbbixkamk.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/glgkdfmrt.sHtML

[Q58] 累计求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geyioowpa.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gcwlhulrc.sHtML

[Q59] 分组内累计
来源：http://3g.fanxiaobao.xyz/Article/details/gmcxcagkf.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/grjkfbckt.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.fanxiaobao.xyz/Article/details/gofdyoxyl.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.fanxiaobao.xyz/Article/details/ghlccobit.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gopppdopz.sHtML

[Q61] 移动平均
来源：http://wap.fanxiaobao.xyz/Article/details/ghrqidavv.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gfsoedinj.sHtML

[Q62] 分组占比
来源：http://blog.fanxiaobao.xyz/Article/details/gznsnhfml.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghstuwzbd.sHtML

[Q63] 开启事务
来源：http://wap.fanxiaobao.xyz/Article/details/gogotzjbh.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.fanxiaobao.xyz/Article/details/ghwjujrlu.sHtML

[Q64] 提交事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gjzrsutaq.sHtML

COMMIT;
来源：http://baike.fanxiaobao.xyz/Article/details/gknstiuhb.sHtML

[Q65] 回滚事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzaxjoirx.sHtML

ROLLBACK;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnvitmpbq.sHtML

[Q66] 行锁查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghcdduzwi.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfgguerud.sHtML

[Q67] 设置隔离级别
来源：http://mobile.fanxiaobao.xyz/Article/details/gbbvkzxmt.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjenrzqlk.sHtML

[Q68] 保存点
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpzcmntzb.sHtML

SAVEPOINT sp1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwcyljzau.sHtML

ROLLBACK TO sp1;
来源：http://3g.fanxiaobao.xyz/Article/details/geuvpedxh.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvqwkguwz.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.fanxiaobao.xyz/Article/details/gdkvsxdgq.sHtML

[Q70] 更新统计信息
来源：http://www.share.fanxiaobao.xyz/Article/details/gvuiqwibz.sHtML

ANALYZE TABLE users;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggicgbfkp.sHtML

[Q71] 查看建表语句
来源：http://read.share.fanxiaobao.xyz/Article/details/gxwuuzrhx.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpehemzvn.sHtML

[Q72] 查看索引
来源：http://m.share.fanxiaobao.xyz/Article/details/gcqaujxsk.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gybsvcqml.sHtML

[Q73] 查看表状态
来源：http://www.share.fanxiaobao.xyz/Article/details/gdiiqkcku.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.fanxiaobao.xyz/Article/details/gjueclfdc.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gphltobcb.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxwmyjzng.sHtML

[Q75] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/glequduys.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/ghdokymtk.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.fanxiaobao.xyz/Article/details/gywtwopjs.sHtML

[Q76] 按天统计
来源：http://3g.fanxiaobao.xyz/Article/details/gchpgmhur.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.fanxiaobao.xyz/Article/details/gpnwiqhkk.sHtML

[Q77] 时间加减
来源：http://baike.fanxiaobao.xyz/Article/details/gndqnyjhj.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnmkgvpvl.sHtML

[Q78] 当前时间
来源：http://blog.fanxiaobao.xyz/Article/details/gsaunekvd.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.fanxiaobao.xyz/Article/details/gzcetivlk.sHtML

[Q79] 字符串拼接
来源：http://read.share.fanxiaobao.xyz/Article/details/gokjyxezs.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.fanxiaobao.xyz/Article/details/gubcxgwfq.sHtML

[Q80] 字符串截取
来源：http://3g.fanxiaobao.xyz/Article/details/glgeeedlz.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqraxkocw.sHtML

[Q81] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/gzfueqios.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gsfjoxhsl.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fanxiaobao.xyz/Article/details/gsiukdneb.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gitaktowh.sHtML

[Q83] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/gkjpkypnb.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gzizbvxvj.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqubukaid.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/geiejndcf.sHtML

[Q85] 数值取整
来源：http://baike.fanxiaobao.xyz/Article/details/gogvudsau.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gghjymgda.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.fanxiaobao.xyz/Article/details/gthsxzyrq.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fanxiaobao.xyz/Article/details/gsdrnoeuf.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyhxaeqga.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.fanxiaobao.xyz/Article/details/gexrsdxnd.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.fanxiaobao.xyz/Article/details/gsmpehhmw.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.fanxiaobao.xyz/Article/details/gvryeqynd.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gityxwclx.sHtML

[Q89] 判断表是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gpmtoykrl.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkzifglbt.sHtML

[Q90] 生成序号列
来源：http://read.share.fanxiaobao.xyz/Article/details/gadfirfjz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fanxiaobao.xyz/Article/details/gglnzbqcz.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/glxrivuto.sHtML

R. Bash 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/ghsmzbxti.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/ghkyisevv.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fanxiaobao.xyz/Article/details/gwphsbzpb.sHtML

#!/usr/bin/env bash
来源：http://3g.fanxiaobao.xyz/Article/details/gwetqjala.sHtML

set -euo pipefail
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtjfbpqzs.sHtML

[R02] 变量赋值与使用
来源：http://blog.fanxiaobao.xyz/Article/details/gdpjdnlfr.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fanxiaobao.xyz/Article/details/gxdocymmr.sHtML

[R03] 只读变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbhegiqzv.sHtML

readonly PI=3.14
来源：http://www.share.fanxiaobao.xyz/Article/details/ggjluvpmn.sHtML

[R04] 位置参数
来源：http://baike.fanxiaobao.xyz/Article/details/gcxqxpolq.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwogjbghd.sHtML

[R05] 参数默认值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gehtuwenz.sHtML

name="${1:-default}"
来源：http://3g.fanxiaobao.xyz/Article/details/gdlwtcfpd.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gxyfcjths.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gelaphhdk.sHtML

[R07] if 判断文件
来源：http://3g.fanxiaobao.xyz/Article/details/ghuikejeh.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gowioqcvz.sHtML

[R08] 数值比较
来源：http://blog.fanxiaobao.xyz/Article/details/gsmskwqiz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/ghhdjrzbn.sHtML

[R09] 字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gpsamrufy.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gusikdynr.sHtML

[R10] 正则匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkrcijpng.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/ghjpcvpwt.sHtML

[R11] case 多分支
来源：http://read.share.fanxiaobao.xyz/Article/details/gqslesrle.sHtML

case "$1" in
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grnqjilun.sHtML

start) echo "启动" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzcxltkvw.sHtML

stop)  echo "停止" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/glqjgoxja.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaabbiohg.sHtML

esac
来源：http://read.share.fanxiaobao.xyz/Article/details/gbvvydisw.sHtML

[R12] for 遍历文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gbpygsvcu.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/grglqpecv.sHtML

[R13] for 计数循环
来源：http://baike.fanxiaobao.xyz/Article/details/gmcsbqrgj.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gzitkozyr.sHtML

[R14] C 风格 for
来源：http://blog.fanxiaobao.xyz/Article/details/gxqhvnrbm.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gpbvtytyc.sHtML

[R15] while 逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gebmkpmcn.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gijotpqxf.sHtML

[R16] until 等待条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gvpojyxou.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gzjiddcbq.sHtML

[R17] 数组定义与取值
来源：http://3g.fanxiaobao.xyz/Article/details/guhrxgjuz.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/grgcfiktx.sHtML

[R18] 遍历数组
来源：http://3g.fanxiaobao.xyz/Article/details/ghtjgzexc.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdeadauwk.sHtML

[R19] 数组长度
来源：http://read.share.fanxiaobao.xyz/Article/details/geeczpokx.sHtML

echo "${#arr[@]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gxxpzltmp.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grcnivuyj.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gtxpzggda.sHtML

[R21] 字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/ghxkktigt.sHtML

echo "${#s}"
来源：http://3g.fanxiaobao.xyz/Article/details/gjzismbkj.sHtML

[R22] 截取子串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gykmbnuqw.sHtML

echo "${s:0:5}"
来源：http://wap.fanxiaobao.xyz/Article/details/gjmatanqu.sHtML

[R23] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gdaiuiroe.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fanxiaobao.xyz/Article/details/gwnmsirhn.sHtML

[R24] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/gqhyswsit.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fanxiaobao.xyz/Article/details/gyppjnmgs.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fanxiaobao.xyz/Article/details/gqpwoyetd.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fanxiaobao.xyz/Article/details/gbtcuzbji.sHtML

[R26] 命令替换
来源：http://www.share.fanxiaobao.xyz/Article/details/glgjepwcv.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghfasjhla.sHtML

[R27] 算术展开
来源：http://mobile.fanxiaobao.xyz/Article/details/gzclsczre.sHtML

echo $((1 + 2 * 3))
来源：http://wap.fanxiaobao.xyz/Article/details/gqeqywblu.sHtML

[R28] 浮点运算
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmftljbzv.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtnhjzakf.sHtML

[R29] 定义函数
来源：http://baike.fanxiaobao.xyz/Article/details/gbfchgumv.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gbhiahrkn.sHtML

[R30] 函数返回状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/ggkqmzuvt.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfuvdxbza.sHtML

[R31] 局部变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gayobfrcu.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fanxiaobao.xyz/Article/details/giqqoipbz.sHtML

[R32] 参数个数校验
来源：http://wap.fanxiaobao.xyz/Article/details/gpcjhymui.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gtmambhhf.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fanxiaobao.xyz/Article/details/gkwkqlqyi.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fanxiaobao.xyz/Article/details/gsjnzuhni.sHtML

[R34] 退出时清理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzygbjtuc.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzycceyoh.sHtML

[R35] 后台执行并等待
来源：http://mobile.fanxiaobao.xyz/Article/details/gincsonry.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fanxiaobao.xyz/Article/details/gihfuscbm.sHtML

[R36] 并发执行多个任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gedhoclwg.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fanxiaobao.xyz/Article/details/glmebqbkd.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvqhuzzvq.sHtML

files=$(ls -1)
来源：http://blog.fanxiaobao.xyz/Article/details/geidafizy.sHtML

[R38] 管道串联
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbbfdpexo.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gknpjdccf.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.fanxiaobao.xyz/Article/details/gdnkvlfst.sHtML

cmd > out.log 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/grzwezgxf.sHtML

[R40] 追加写日志
来源：http://blog.fanxiaobao.xyz/Article/details/gzscsvwmc.sHtML

echo "log" >> out.log
来源：http://3g.fanxiaobao.xyz/Article/details/gkaqlwdhe.sHtML

[R41] 丢弃输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gulpzkole.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gmsbzfkzp.sHtML

[R42] 输入重定向
来源：http://3g.fanxiaobao.xyz/Article/details/gfimgltmv.sHtML

wc -l < a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/glmdpkizl.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfbpxlexg.sHtML

find . -name "*.log" -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/gphtjnrns.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gemesqjaj.sHtML

find . -mtime -7 -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gzpuqlntc.sHtML

[R45] 批量删除
来源：http://read.share.fanxiaobao.xyz/Article/details/gfzxobria.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fanxiaobao.xyz/Article/details/gjcehvohl.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fanxiaobao.xyz/Article/details/genrcvamp.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fanxiaobao.xyz/Article/details/gtxjkzvqy.sHtML

[R47] sed 单行替换
来源：http://blog.fanxiaobao.xyz/Article/details/gsltctlal.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gosbfmydm.sHtML

[R48] awk 取指定列
来源：http://wap.fanxiaobao.xyz/Article/details/gbhzycwgo.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gykxxaysg.sHtML

[R49] awk 带条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gfdyaocpz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fanxiaobao.xyz/Article/details/gdugerqla.sHtML

[R50] awk 求和
来源：http://wap.fanxiaobao.xyz/Article/details/grhdeedax.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gofbzvlcz.sHtML

[R51] 排序去重取前几
来源：http://wap.fanxiaobao.xyz/Article/details/gccesjvbs.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fanxiaobao.xyz/Article/details/gdoctyvdc.sHtML

[R52] 统计行数
来源：http://mobile.fanxiaobao.xyz/Article/details/glwffmxzs.sHtML

wc -l a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gibhflqyd.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fanxiaobao.xyz/Article/details/gkizddfmh.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fanxiaobao.xyz/Article/details/gdirpdaur.sHtML

[R54] 比较两个文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gcrtyendt.sHtML

diff a.txt b.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gmnrfjpcy.sHtML

[R55] 压缩与解压
来源：http://wap.fanxiaobao.xyz/Article/details/gfxpvacka.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fanxiaobao.xyz/Article/details/gukvmkdvl.sHtML

[R56] 远程拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/ghjmxsacb.sHtML

scp file user@host:/path/
来源：http://mobile.fanxiaobao.xyz/Article/details/gijbiwisk.sHtML

[R57] 远程执行命令
来源：http://blog.fanxiaobao.xyz/Article/details/gnnemnznc.sHtML

ssh user@host 'uptime'
来源：http://www.share.fanxiaobao.xyz/Article/details/gikhoobxv.sHtML

[R58] 下载文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gxhafvakh.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fanxiaobao.xyz/Article/details/gxcbvrusk.sHtML

[R59] 发 POST JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/gruzvnknt.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gspveioyz.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fanxiaobao.xyz/Article/details/ghixbyloa.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fanxiaobao.xyz/Article/details/gdyrnewip.sHtML

[R61] 磁盘占用
来源：http://baike.fanxiaobao.xyz/Article/details/gizrfljka.sHtML

df -h;  du -sh *
来源：http://www.share.fanxiaobao.xyz/Article/details/gsojgccbf.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gflodzucj.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fanxiaobao.xyz/Article/details/ghdycmlii.sHtML

[R63] 内存与进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjqwzhvry.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fanxiaobao.xyz/Article/details/gcvvgmwhn.sHtML

[R64] 结束进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gfzvhxfwn.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fanxiaobao.xyz/Article/details/geoooilud.sHtML

[R65] 查看端口占用
来源：http://blog.fanxiaobao.xyz/Article/details/givdhkhhc.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkxbtqoje.sHtML

[R66] 定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/grpmpnche.sHtML

crontab -e;  crontab -l
来源：http://baike.fanxiaobao.xyz/Article/details/gtiddmpzg.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glsaqnhtj.sHtML

openssl rand -hex 16
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzvnaajhp.sHtML

[R68] 计算文件校验值
来源：http://m.share.fanxiaobao.xyz/Article/details/gxhcsnjcn.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gmotdhjsu.sHtML

[R69] 生成随机密码
来源：http://wap.fanxiaobao.xyz/Article/details/gtswiwhoy.sHtML


<!-- 参考信息 -->