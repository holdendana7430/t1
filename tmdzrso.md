代发 wailian999

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://m.share.zdbjq.cn/Article/details/graonrmyj.sHtML

[Q20] IN 列表
来源：http://read.share.fehbvm.com/Article/details/gtogxsztq.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://m.share.zdbjq.cn/Article/details/gunxmtbzf.sHtML

[Q21] 空值判断
来源：http://m.share.hesvh.cn/Article/details/gjlyoermn.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.hesvh.cn/Article/details/gvppfxuyp.sHtML

[Q22] 排序
来源：http://3g.hesvh.cn/Article/details/gogofoaam.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.hesvh.cn/Article/details/gtjhkxkvy.sHtML

[Q23] 分页
来源：http://blog.zdbjq.cn/Article/details/gzmgwopyw.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.hesvh.cn/Article/details/gzzmcwrpr.sHtML

[Q24] 去重
来源：http://www.share.hesvh.cn/Article/details/gbihqtaeo.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.hesvh.cn/Article/details/gdqaxyohb.sHtML

[Q25] 只取前 N 条
来源：http://baike.hesvh.cn/Article/details/gpntomopg.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.fehbvm.com/Article/details/gvhkoylof.sHtML

[Q26] 计数
来源：http://wap.zdbjq.cn/Article/details/gonwgsdqj.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gvklzqkxm.sHtML

[Q27] 条件计数
来源：http://wap.fehbvm.com/Article/details/geongmmrm.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gyapoisyb.sHtML

[Q28] 求和与平均
来源：http://www.m.share.fehbvm.com/Article/details/gyxnhvlgr.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gkpyleicm.sHtML

[Q29] 最大最小值
来源：http://mobile.hesvh.cn/Article/details/gxffyzfjd.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.zdbjq.cn/Article/details/grdpdcyzy.sHtML

[Q30] 分组统计
来源：http://mobile.fehbvm.com/Article/details/gwafamfqm.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/ggjitcvmd.sHtML

[Q31] 分组后过滤
来源：http://mobile.fehbvm.com/Article/details/gcurbywyr.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.zdbjq.cn/Article/details/gcolwpylg.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gkrdhfmgq.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/gtsiozcoo.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.fehbvm.com/Article/details/gkffxkvsz.sHtML

[Q33] 多列分组
来源：http://blog.hesvh.cn/Article/details/glbrlwibp.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.zdbjq.cn/Article/details/gjnqkxnru.sHtML

[Q34] 每组取第一条
来源：http://baike.zdbjq.cn/Article/details/guwbgzflp.sHtML

SELECT * FROM (
来源：http://www.blog.zdbjq.cn/Article/details/gowsqwlte.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.zdbjq.cn/Article/details/gajejfvzw.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gswdrbtyk.sHtML

[Q35] 内连接
来源：http://m.share.zdbjq.cn/Article/details/gbwxbykyy.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.hesvh.cn/Article/details/gwjudsefq.sHtML

[Q36] 左连接
来源：http://m.share.fehbvm.com/Article/details/ggqbaeywy.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.zdbjq.cn/Article/details/gzmcqaqbi.sHtML

[Q37] 右连接
来源：http://www.share.fehbvm.com/Article/details/grpunyfic.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.zdbjq.cn/Article/details/gyaudxdpn.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.hesvh.cn/Article/details/glpyrrzae.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://read.share.hesvh.cn/Article/details/gjrrbqkyz.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.hesvh.cn/Article/details/gzhabhcwc.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.zdbjq.cn/Article/details/gybpctxrn.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.zdbjq.cn/Article/details/gaphewswr.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.fehbvm.com/Article/details/gofcgljvt.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.hesvh.cn/Article/details/guiydfcmw.sHtML

[Q41] 多表连接
来源：http://wap.fehbvm.com/Article/details/gqeaiowxt.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.hesvh.cn/Article/details/gczikdqvm.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.fehbvm.com/Article/details/gcboqniuw.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.hesvh.cn/Article/details/glkkpaesv.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.fehbvm.com/Article/details/gotkijeag.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.zdbjq.cn/Article/details/gsfzqvfyv.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.zdbjq.cn/Article/details/gnlrusvqs.sHtML

[Q43] 标量子查询
来源：http://read.share.zdbjq.cn/Article/details/gtnvtvqtm.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.zdbjq.cn/Article/details/gpzsbzcaa.sHtML

[Q44] IN 子查询
来源：http://read.share.zdbjq.cn/Article/details/gzvcppuod.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.fehbvm.com/Article/details/gipkkozbm.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.fehbvm.com/Article/details/guthrjmza.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.hesvh.cn/Article/details/gisuyaboz.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.zdbjq.cn/Article/details/gxqakvlws.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.hesvh.cn/Article/details/gjltqsidd.sHtML

[Q47] 与平均值比较
来源：http://www.blog.zdbjq.cn/Article/details/gaetdyzyb.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.hesvh.cn/Article/details/guunbmrrn.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.hesvh.cn/Article/details/gtnxioyst.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.fehbvm.com/Article/details/gehyvlayb.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.hesvh.cn/Article/details/glptyfjqk.sHtML

[Q49] 更新单行
来源：http://read.share.fehbvm.com/Article/details/gypdybyna.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.hesvh.cn/Article/details/gyonlfwfa.sHtML

[Q50] 批量更新
来源：http://3g.zdbjq.cn/Article/details/giixkoowv.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.hesvh.cn/Article/details/gkqrtuceg.sHtML

[Q51] 用子查询更新
来源：http://blog.hesvh.cn/Article/details/guwvarzbj.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.hesvh.cn/Article/details/ghboyxdap.sHtML

[Q52] 删除指定行
来源：http://blog.hesvh.cn/Article/details/gfmhteznd.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.zdbjq.cn/Article/details/glhwjubrk.sHtML

[Q53] 按条件删除
来源：http://www.share.hesvh.cn/Article/details/gmyfuznnv.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.zdbjq.cn/Article/details/gshfiqrgd.sHtML

[Q54] 清空表
来源：http://read.share.fehbvm.com/Article/details/gvvjiqvyd.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.hesvh.cn/Article/details/geqwzvhoy.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.fehbvm.com/Article/details/gikjfyucd.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.fehbvm.com/Article/details/ghqzbycuz.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.hesvh.cn/Article/details/glyordcgu.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.zdbjq.cn/Article/details/grwyddajm.sHtML

[Q57] 行号
来源：http://read.share.fehbvm.com/Article/details/giwlnawhz.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gbhslytmx.sHtML

[Q58] 累计求和
来源：http://www.m.share.zdbjq.cn/Article/details/gbtwqicuc.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.hesvh.cn/Article/details/gxjtvtott.sHtML

[Q59] 分组内累计
来源：http://mobile.hesvh.cn/Article/details/gncdbwydf.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gidscsaxb.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.hesvh.cn/Article/details/gmbiqdqwe.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.zdbjq.cn/Article/details/gzbthdyri.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.zdbjq.cn/Article/details/glkncvqsz.sHtML

[Q61] 移动平均
来源：http://read.share.fehbvm.com/Article/details/goypdbysx.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/ggzqcopps.sHtML

[Q62] 分组占比
来源：http://www.blog.hesvh.cn/Article/details/guwoliuqr.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gwtzyvjlv.sHtML

[Q63] 开启事务
来源：http://wap.zdbjq.cn/Article/details/gfvvvnvqq.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.hesvh.cn/Article/details/gxopvnfyg.sHtML

[Q64] 提交事务
来源：http://3g.zdbjq.cn/Article/details/goijyeqtz.sHtML

COMMIT;
来源：http://baike.hesvh.cn/Article/details/guqlgeogy.sHtML

[Q65] 回滚事务
来源：http://www.share.hesvh.cn/Article/details/gieimrxcv.sHtML

ROLLBACK;
来源：http://www.share.zdbjq.cn/Article/details/gapzxconq.sHtML

[Q66] 行锁查询
来源：http://baike.zdbjq.cn/Article/details/grgogdjtv.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.hesvh.cn/Article/details/gvefhumkc.sHtML

[Q67] 设置隔离级别
来源：http://baike.hesvh.cn/Article/details/gmapnbjzg.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.hesvh.cn/Article/details/gqgnjkbem.sHtML

[Q68] 保存点
来源：http://read.share.zdbjq.cn/Article/details/ghgxgxmjc.sHtML

SAVEPOINT sp1;
来源：http://3g.fehbvm.com/Article/details/gaoirtuoh.sHtML

ROLLBACK TO sp1;
来源：http://baike.hesvh.cn/Article/details/gmdvrbhpb.sHtML

[Q69] 查看执行计划
来源：http://m.share.hesvh.cn/Article/details/gkrdkciwi.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.fehbvm.com/Article/details/gcezpnvix.sHtML

[Q70] 更新统计信息
来源：http://www.share.fehbvm.com/Article/details/gbfkdvbar.sHtML

ANALYZE TABLE users;
来源：http://mobile.fehbvm.com/Article/details/gefpbitsp.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fehbvm.com/Article/details/gtofmseuw.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.zdbjq.cn/Article/details/gnyysqsmy.sHtML

[Q72] 查看索引
来源：http://www.share.zdbjq.cn/Article/details/gfjekvrls.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gxmzeoqcj.sHtML

[Q73] 查看表状态
来源：http://3g.fehbvm.com/Article/details/gmvqiecyy.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.zdbjq.cn/Article/details/gsdieokvc.sHtML

[Q74] 强制使用索引
来源：http://read.share.fehbvm.com/Article/details/gzxcgvjgh.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fehbvm.com/Article/details/gbabwwcya.sHtML

[Q75] 日期格式化
来源：http://3g.fehbvm.com/Article/details/gplpdhelt.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fehbvm.com/Article/details/ggqjwgawa.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.zdbjq.cn/Article/details/grlltqtua.sHtML

[Q76] 按天统计
来源：http://3g.hesvh.cn/Article/details/gksslcsip.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.zdbjq.cn/Article/details/gsiowuiax.sHtML

[Q77] 时间加减
来源：http://wap.zdbjq.cn/Article/details/gkblatmsd.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.hesvh.cn/Article/details/giwjfczpx.sHtML

[Q78] 当前时间
来源：http://3g.fehbvm.com/Article/details/gunzqxkfy.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.hesvh.cn/Article/details/gnqqncctu.sHtML

[Q79] 字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/gjhkdtqde.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fehbvm.com/Article/details/gsdkumepq.sHtML

[Q80] 字符串截取
来源：http://www.share.zdbjq.cn/Article/details/gswqdwctf.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.fehbvm.com/Article/details/ghfclmjea.sHtML

[Q81] 字符串替换
来源：http://wap.fehbvm.com/Article/details/gsmacwvce.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gkkpruilv.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.zdbjq.cn/Article/details/gxvvkvyyg.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gxunwxtbg.sHtML

[Q83] 大小写转换
来源：http://www.blog.fehbvm.com/Article/details/gmhwhjvne.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gfqczxcvi.sHtML

[Q84] 去除首尾空格
来源：http://m.share.zdbjq.cn/Article/details/gbvtmtyns.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gskyfkixj.sHtML

[Q85] 数值取整
来源：http://wap.fehbvm.com/Article/details/ggdqdfflv.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.zdbjq.cn/Article/details/gjhvnqcjz.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.fehbvm.com/Article/details/grppcvwok.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.hesvh.cn/Article/details/gzdxdvxly.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.hesvh.cn/Article/details/gxqudhrdh.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.hesvh.cn/Article/details/gfyshbdcr.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.hesvh.cn/Article/details/gfoufirih.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.zdbjq.cn/Article/details/guezvibdv.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fehbvm.com/Article/details/goindzenw.sHtML

[Q89] 判断表是否存在
来源：http://blog.zdbjq.cn/Article/details/gahfksotk.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.hesvh.cn/Article/details/gtodvdxkh.sHtML

[Q90] 生成序号列
来源：http://3g.zdbjq.cn/Article/details/gheudhrwh.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.hesvh.cn/Article/details/gscmymenh.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gllmbgvew.sHtML

R. Bash 专题
来源：http://mobile.fehbvm.com/Article/details/gcznmpebc.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gijvwxojz.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fehbvm.com/Article/details/gwigtrylc.sHtML

#!/usr/bin/env bash
来源：http://mobile.fehbvm.com/Article/details/gsiazdegu.sHtML

set -euo pipefail
来源：http://www.blog.fehbvm.com/Article/details/gscyllcye.sHtML

[R02] 变量赋值与使用
来源：http://3g.hesvh.cn/Article/details/gzrypvtcv.sHtML

name="Tom"; echo "$name"
来源：http://wap.fehbvm.com/Article/details/ggtyqcxei.sHtML

[R03] 只读变量
来源：http://read.share.hesvh.cn/Article/details/gwigahtyu.sHtML

readonly PI=3.14
来源：http://read.share.zdbjq.cn/Article/details/giliijxdp.sHtML

[R04] 位置参数
来源：http://www.share.fehbvm.com/Article/details/gjrmvvoct.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.hesvh.cn/Article/details/guhnjugpq.sHtML

[R05] 参数默认值
来源：http://blog.fehbvm.com/Article/details/gtxtuudaz.sHtML

name="${1:-default}"
来源：http://www.blog.zdbjq.cn/Article/details/golzugeeu.sHtML

[R06] 判断命令是否存在
来源：http://m.share.fehbvm.com/Article/details/gxsgcfyfz.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.zdbjq.cn/Article/details/gwgrialab.sHtML

[R07] if 判断文件
来源：http://mobile.fehbvm.com/Article/details/giurtpljh.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.hesvh.cn/Article/details/gggktemiq.sHtML

[R08] 数值比较
来源：http://m.share.fehbvm.com/Article/details/gjdzdmpuu.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gkyxuspqm.sHtML

[R09] 字符串比较
来源：http://read.share.hesvh.cn/Article/details/gfiqwztbo.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.hesvh.cn/Article/details/gznnnfzpr.sHtML

[R10] 正则匹配
来源：http://read.share.zdbjq.cn/Article/details/ggvmufrxu.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.fehbvm.com/Article/details/gimevayhu.sHtML

[R11] case 多分支
来源：http://www.m.share.fehbvm.com/Article/details/gnrzoocuj.sHtML

case "$1" in
来源：http://read.share.zdbjq.cn/Article/details/gmsjcdibi.sHtML

start) echo "启动" ;;
来源：http://www.blog.fehbvm.com/Article/details/gkfgolmcn.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fehbvm.com/Article/details/gfawsphft.sHtML

*)     echo "未知命令" ;;
来源：http://3g.hesvh.cn/Article/details/ggbkkqsfv.sHtML

esac
来源：http://www.m.share.zdbjq.cn/Article/details/gyfkpugsb.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fehbvm.com/Article/details/gurscotzt.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.zdbjq.cn/Article/details/gkrfotbpa.sHtML

[R13] for 计数循环
来源：http://baike.hesvh.cn/Article/details/gkatqvbve.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/gqfhtssug.sHtML

[R14] C 风格 for
来源：http://m.share.fehbvm.com/Article/details/gqbsifpsd.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.hesvh.cn/Article/details/gfbjlsgzo.sHtML

[R15] while 逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gsjpchczi.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fehbvm.com/Article/details/ggchhskto.sHtML

[R16] until 等待条件
来源：http://www.m.share.fehbvm.com/Article/details/gjpgxnatu.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.hesvh.cn/Article/details/gcjmaicxu.sHtML

[R17] 数组定义与取值
来源：http://blog.fehbvm.com/Article/details/gxdqkiwlu.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.fehbvm.com/Article/details/gswuxtjeh.sHtML

[R18] 遍历数组
来源：http://www.m.share.fehbvm.com/Article/details/gckzqndhw.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.hesvh.cn/Article/details/gsudowoxm.sHtML

[R19] 数组长度
来源：http://3g.fehbvm.com/Article/details/gnarnzkjk.sHtML

echo "${#arr[@]}"
来源：http://3g.hesvh.cn/Article/details/gbwrykgvx.sHtML

[R20] 关联数组（字典）
来源：http://blog.fehbvm.com/Article/details/gevchtjzz.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.zdbjq.cn/Article/details/guasysnqw.sHtML

[R21] 字符串长度
来源：http://www.blog.fehbvm.com/Article/details/gwwbbwchp.sHtML

echo "${#s}"
来源：http://www.share.zdbjq.cn/Article/details/gjioxutvy.sHtML

[R22] 截取子串
来源：http://m.share.fehbvm.com/Article/details/gkogazetj.sHtML

echo "${s:0:5}"
来源：http://read.share.zdbjq.cn/Article/details/gthxgarlq.sHtML

[R23] 字符串替换
来源：http://blog.zdbjq.cn/Article/details/gnrxuaevm.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.hesvh.cn/Article/details/gxivorlhu.sHtML

[R24] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/gwbgnxhaw.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.hesvh.cn/Article/details/geamadplz.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.zdbjq.cn/Article/details/gtyslvtsl.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fehbvm.com/Article/details/gobjihkwx.sHtML

[R26] 命令替换
来源：http://m.share.hesvh.cn/Article/details/gkyuuqjdx.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.zdbjq.cn/Article/details/gjitoihsj.sHtML

[R27] 算术展开
来源：http://read.share.zdbjq.cn/Article/details/gocurxula.sHtML

echo $((1 + 2 * 3))
来源：http://baike.hesvh.cn/Article/details/gkqaukewy.sHtML

[R28] 浮点运算
来源：http://wap.hesvh.cn/Article/details/giiomeqoh.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.hesvh.cn/Article/details/gbyspgqbr.sHtML

[R29] 定义函数
来源：http://wap.zdbjq.cn/Article/details/gwcphcmsa.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fehbvm.com/Article/details/goginnnnr.sHtML

[R30] 函数返回状态码
来源：http://read.share.zdbjq.cn/Article/details/gjhxljhfc.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.zdbjq.cn/Article/details/gaigkvvvm.sHtML

[R31] 局部变量
来源：http://www.blog.zdbjq.cn/Article/details/gukekyasd.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fehbvm.com/Article/details/gcoxngskp.sHtML

[R32] 参数个数校验
来源：http://wap.hesvh.cn/Article/details/gqosjpcgf.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.zdbjq.cn/Article/details/gmqthlwrk.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.hesvh.cn/Article/details/gvrqtjvev.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.zdbjq.cn/Article/details/grkuritpw.sHtML

[R34] 退出时清理
来源：http://read.share.hesvh.cn/Article/details/gxkncfiet.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.hesvh.cn/Article/details/gtkcxwefl.sHtML

[R35] 后台执行并等待
来源：http://www.blog.zdbjq.cn/Article/details/gdhqqyidq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.zdbjq.cn/Article/details/guzhuowoh.sHtML

[R36] 并发执行多个任务
来源：http://www.share.zdbjq.cn/Article/details/gfhksvumd.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.zdbjq.cn/Article/details/ghpjhwcte.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.zdbjq.cn/Article/details/gzpzyhiaz.sHtML

files=$(ls -1)
来源：http://baike.hesvh.cn/Article/details/gasiqejhi.sHtML

[R38] 管道串联
来源：http://blog.hesvh.cn/Article/details/gtquhpzqs.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.hesvh.cn/Article/details/guscfaifr.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fehbvm.com/Article/details/gapmyamen.sHtML

cmd > out.log 2>&1
来源：http://read.share.fehbvm.com/Article/details/geuwxdkpo.sHtML

[R40] 追加写日志
来源：http://m.share.fehbvm.com/Article/details/gdtvtiewv.sHtML

echo "log" >> out.log
来源：http://www.share.fehbvm.com/Article/details/gqisjozel.sHtML

[R41] 丢弃输出
来源：http://read.share.hesvh.cn/Article/details/gnssqqbfo.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.hesvh.cn/Article/details/gffphuukq.sHtML

[R42] 输入重定向
来源：http://blog.zdbjq.cn/Article/details/gelhtoqkj.sHtML

wc -l < a.txt
来源：http://blog.zdbjq.cn/Article/details/gerrmtvfn.sHtML

[R43] 按名字查找文件
来源：http://wap.zdbjq.cn/Article/details/gvfmyvhnt.sHtML

find . -name "*.log" -type f
来源：http://blog.fehbvm.com/Article/details/grsigfiyk.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fehbvm.com/Article/details/gnavltegl.sHtML

find . -mtime -7 -type f
来源：http://wap.hesvh.cn/Article/details/gavqrisda.sHtML

[R45] 批量删除
来源：http://read.share.zdbjq.cn/Article/details/gmjqfnfwj.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fehbvm.com/Article/details/gxsixyvrl.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.zdbjq.cn/Article/details/gbhptutfo.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.hesvh.cn/Article/details/gfnphhtnk.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fehbvm.com/Article/details/gbdqigegl.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.zdbjq.cn/Article/details/gbtljefbr.sHtML

[R48] awk 取指定列
来源：http://blog.hesvh.cn/Article/details/gbktxcabb.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.zdbjq.cn/Article/details/gwuxltoiq.sHtML

[R49] awk 带条件
来源：http://mobile.zdbjq.cn/Article/details/gpddsxagc.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fehbvm.com/Article/details/gkdhtjpud.sHtML

[R50] awk 求和
来源：http://baike.zdbjq.cn/Article/details/ggbqlyqrj.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.zdbjq.cn/Article/details/gdcbruuby.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fehbvm.com/Article/details/gmdpgqamj.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.zdbjq.cn/Article/details/gggpwstop.sHtML

[R52] 统计行数
来源：http://www.share.zdbjq.cn/Article/details/gtsqhzkxb.sHtML

wc -l a.txt
来源：http://mobile.zdbjq.cn/Article/details/gebwivial.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fehbvm.com/Article/details/ggqjftwss.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fehbvm.com/Article/details/gftuuuocr.sHtML

[R54] 比较两个文件
来源：http://blog.zdbjq.cn/Article/details/gnpjbnisu.sHtML

diff a.txt b.txt
来源：http://m.share.fehbvm.com/Article/details/gpwrpnetw.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fehbvm.com/Article/details/ggexvzzyj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.hesvh.cn/Article/details/giabfigne.sHtML

[R56] 远程拷贝
来源：http://www.blog.fehbvm.com/Article/details/gypydkgxl.sHtML

scp file user@host:/path/
来源：http://www.m.share.zdbjq.cn/Article/details/gihlqalnw.sHtML

[R57] 远程执行命令
来源：http://baike.zdbjq.cn/Article/details/gytlsabpk.sHtML

ssh user@host 'uptime'
来源：http://blog.fehbvm.com/Article/details/gisfrknrp.sHtML

[R58] 下载文件
来源：http://3g.zdbjq.cn/Article/details/gczutvbfw.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.zdbjq.cn/Article/details/ghslbqlrm.sHtML

[R59] 发 POST JSON
来源：http://www.blog.zdbjq.cn/Article/details/glkoqugtw.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fehbvm.com/Article/details/gxwkwemcb.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.hesvh.cn/Article/details/gjqvtresd.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.hesvh.cn/Article/details/gajddhukj.sHtML

[R61] 磁盘占用
来源：http://www.share.hesvh.cn/Article/details/gachvxtmb.sHtML

df -h;  du -sh *
来源：http://baike.fehbvm.com/Article/details/gnadhptas.sHtML

[R62] 找最占空间的文件
来源：http://3g.fehbvm.com/Article/details/gyxqcdccg.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fehbvm.com/Article/details/gwqyejhmk.sHtML

[R63] 内存与进程
来源：http://mobile.fehbvm.com/Article/details/giweykqkd.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.zdbjq.cn/Article/details/glvjcbrju.sHtML

[R64] 结束进程
来源：http://3g.hesvh.cn/Article/details/gjxuhniyn.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fehbvm.com/Article/details/goyiljpop.sHtML

[R65] 查看端口占用
来源：http://mobile.zdbjq.cn/Article/details/gdesghoao.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fehbvm.com/Article/details/glqasaxov.sHtML

[R66] 定时任务
来源：http://www.blog.hesvh.cn/Article/details/gzzlvznji.sHtML

crontab -e;  crontab -l
来源：http://www.share.zdbjq.cn/Article/details/gyvnyskyu.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fehbvm.com/Article/details/gxuvdcgcq.sHtML

openssl rand -hex 16
来源：http://www.share.fehbvm.com/Article/details/gqyohemuf.sHtML

[R68] 计算文件校验值
来源：http://www.share.fehbvm.com/Article/details/gudgfffdn.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fehbvm.com/Article/details/gaptrwlfb.sHtML

[R69] 生成随机密码
来源：http://read.share.hesvh.cn/Article/details/gdyfhmofv.sHtML


<!-- 参考信息 -->