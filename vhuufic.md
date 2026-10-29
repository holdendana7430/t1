代发 wailian999

SELECT * FROM users;
来源：http://3g.fehbvm.com/Article/details/gpwytxahu.sHtML

[Q16] 查询指定列
来源：http://mobile.fehbvm.com/Article/details/gtfnwjscs.sHtML

SELECT id, name FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gwhxjtfzo.sHtML

[Q17] 条件查询
来源：http://www.m.share.hesvh.cn/Article/details/gygwbgezi.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://3g.zdbjq.cn/Article/details/glitpnpds.sHtML

[Q18] 模糊匹配
来源：http://blog.zdbjq.cn/Article/details/gdtdecjco.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.hesvh.cn/Article/details/gknoyibud.sHtML

[Q19] 范围查询
来源：http://wap.hesvh.cn/Article/details/gnspcorjn.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.hesvh.cn/Article/details/guaqaoivi.sHtML

[Q20] IN 列表
来源：http://www.blog.fehbvm.com/Article/details/gssbzqvcs.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://blog.fehbvm.com/Article/details/gwfbjnusb.sHtML

[Q21] 空值判断
来源：http://mobile.zdbjq.cn/Article/details/gxcjoflix.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://wap.zdbjq.cn/Article/details/gpwnqkazq.sHtML

[Q22] 排序
来源：http://m.share.hesvh.cn/Article/details/gfrgtybha.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.blog.fehbvm.com/Article/details/gvyytmioz.sHtML

[Q23] 分页
来源：http://3g.hesvh.cn/Article/details/gzkmwpdcm.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.fehbvm.com/Article/details/gbhtxnamr.sHtML

[Q24] 去重
来源：http://www.share.hesvh.cn/Article/details/gveyzzddf.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gmddlhrzb.sHtML

[Q25] 只取前 N 条
来源：http://read.share.zdbjq.cn/Article/details/gtekkizjg.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.hesvh.cn/Article/details/gdnbcbqpq.sHtML

[Q26] 计数
来源：http://read.share.zdbjq.cn/Article/details/gtqcajgfj.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gqgripijn.sHtML

[Q27] 条件计数
来源：http://baike.fehbvm.com/Article/details/gmoonkrau.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.fehbvm.com/Article/details/gwsuepkwj.sHtML

[Q28] 求和与平均
来源：http://www.blog.hesvh.cn/Article/details/gbqldjdvn.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.fehbvm.com/Article/details/grstvjoml.sHtML

[Q29] 最大最小值
来源：http://www.m.share.hesvh.cn/Article/details/gzdyfhkpm.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.zdbjq.cn/Article/details/ggqcgzzya.sHtML

[Q30] 分组统计
来源：http://blog.hesvh.cn/Article/details/gfxqfqtdv.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/ghzjoamen.sHtML

[Q31] 分组后过滤
来源：http://www.blog.fehbvm.com/Article/details/ghkcbsyth.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.fehbvm.com/Article/details/gghttsazj.sHtML

[Q32] 分组拼接字符串
来源：http://blog.hesvh.cn/Article/details/gfjhmdhjv.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gnmbjsats.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.hesvh.cn/Article/details/gslwjqiil.sHtML

[Q33] 多列分组
来源：http://www.m.share.hesvh.cn/Article/details/gxdvqkgng.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.fehbvm.com/Article/details/gntapuele.sHtML

[Q34] 每组取第一条
来源：http://www.blog.fehbvm.com/Article/details/gqoiizxrl.sHtML

SELECT * FROM (
来源：http://read.share.zdbjq.cn/Article/details/gofimjkmt.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.fehbvm.com/Article/details/gxlhlqenc.sHtML

) t WHERE rn = 1;
来源：http://blog.zdbjq.cn/Article/details/gfsvuoafy.sHtML

[Q35] 内连接
来源：http://read.share.zdbjq.cn/Article/details/gkteccojl.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.hesvh.cn/Article/details/gxbvgyiwd.sHtML

[Q36] 左连接
来源：http://3g.zdbjq.cn/Article/details/gyeafinrd.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.hesvh.cn/Article/details/gciyufvdm.sHtML

[Q37] 右连接
来源：http://www.blog.fehbvm.com/Article/details/gbazfaskr.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.zdbjq.cn/Article/details/gtwkqtjjx.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.fehbvm.com/Article/details/gkhifmftc.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.hesvh.cn/Article/details/gpzorcwlh.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.fehbvm.com/Article/details/geoqhasrz.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.hesvh.cn/Article/details/gavwxnpcz.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gafdhevqo.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.fehbvm.com/Article/details/glsxpghaw.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.zdbjq.cn/Article/details/ggdcbzmcm.sHtML

[Q41] 多表连接
来源：http://www.share.zdbjq.cn/Article/details/gptsnnfkv.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.fehbvm.com/Article/details/gsdrkjtyo.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.hesvh.cn/Article/details/gnewshxgq.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.fehbvm.com/Article/details/gvsxlcotg.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.fehbvm.com/Article/details/goitjdiva.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.zdbjq.cn/Article/details/gqyocilhb.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.zdbjq.cn/Article/details/gsevgbyao.sHtML

[Q43] 标量子查询
来源：http://www.m.share.hesvh.cn/Article/details/grhdjeodu.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.fehbvm.com/Article/details/gmhzckipe.sHtML

[Q44] IN 子查询
来源：http://3g.zdbjq.cn/Article/details/gennkmkwz.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.hesvh.cn/Article/details/gufdwmvqv.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.hesvh.cn/Article/details/gztsblwvh.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fehbvm.com/Article/details/gvhesrrlm.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.fehbvm.com/Article/details/gmoczcczd.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.zdbjq.cn/Article/details/gnmouacxq.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.hesvh.cn/Article/details/gyofgtjfd.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.hesvh.cn/Article/details/gmpuiqqwa.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.fehbvm.com/Article/details/gbsaiavjr.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.zdbjq.cn/Article/details/gkkyiakfb.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.zdbjq.cn/Article/details/gevslxneb.sHtML

[Q49] 更新单行
来源：http://baike.fehbvm.com/Article/details/ggxruferx.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.zdbjq.cn/Article/details/gcyyqfgin.sHtML

[Q50] 批量更新
来源：http://www.m.share.fehbvm.com/Article/details/goctnhzqk.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.hesvh.cn/Article/details/gcmwvcbqq.sHtML

[Q51] 用子查询更新
来源：http://www.share.hesvh.cn/Article/details/gfvsqdksu.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gzqcffrhu.sHtML

[Q52] 删除指定行
来源：http://m.share.zdbjq.cn/Article/details/geiqdgmdx.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.zdbjq.cn/Article/details/gftmmumuw.sHtML

[Q53] 按条件删除
来源：http://read.share.hesvh.cn/Article/details/gqlznpfmg.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.zdbjq.cn/Article/details/ggczleqjq.sHtML

[Q54] 清空表
来源：http://3g.fehbvm.com/Article/details/gewsrbkdi.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fehbvm.com/Article/details/gstidglkc.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.fehbvm.com/Article/details/gswxjsfic.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.fehbvm.com/Article/details/gofbmmonv.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.fehbvm.com/Article/details/ggepsfwbt.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.fehbvm.com/Article/details/gacvpjeic.sHtML

[Q57] 行号
来源：http://www.blog.hesvh.cn/Article/details/gbtnzigzw.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.hesvh.cn/Article/details/gwzmzgqfe.sHtML

[Q58] 累计求和
来源：http://3g.hesvh.cn/Article/details/grculnoar.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gkcunsqom.sHtML

[Q59] 分组内累计
来源：http://www.blog.fehbvm.com/Article/details/gpbmzpwuu.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/ggvbwhifu.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.zdbjq.cn/Article/details/ghvanhoeo.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.hesvh.cn/Article/details/ggsmaduqn.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gutxojubg.sHtML

[Q61] 移动平均
来源：http://www.m.share.fehbvm.com/Article/details/gxsfgzxid.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gokwgkrrn.sHtML

[Q62] 分组占比
来源：http://www.blog.fehbvm.com/Article/details/gtksighon.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/gpgdgffov.sHtML

[Q63] 开启事务
来源：http://m.share.hesvh.cn/Article/details/gomgpwcit.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.zdbjq.cn/Article/details/gnnvohlja.sHtML

[Q64] 提交事务
来源：http://www.blog.fehbvm.com/Article/details/gpatrgujq.sHtML

COMMIT;
来源：http://www.blog.fehbvm.com/Article/details/gxozqyzjd.sHtML

[Q65] 回滚事务
来源：http://www.share.fehbvm.com/Article/details/gvxhknsun.sHtML

ROLLBACK;
来源：http://www.share.fehbvm.com/Article/details/gjdvytczm.sHtML

[Q66] 行锁查询
来源：http://blog.hesvh.cn/Article/details/gtbenfify.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.fehbvm.com/Article/details/gcoeestui.sHtML

[Q67] 设置隔离级别
来源：http://wap.hesvh.cn/Article/details/gyrtjvxcq.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.fehbvm.com/Article/details/gfimxigqt.sHtML

[Q68] 保存点
来源：http://www.m.share.fehbvm.com/Article/details/gbnspeoap.sHtML

SAVEPOINT sp1;
来源：http://read.share.zdbjq.cn/Article/details/grclniisz.sHtML

ROLLBACK TO sp1;
来源：http://mobile.zdbjq.cn/Article/details/gwrqrfygr.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.hesvh.cn/Article/details/gswvanrxg.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.hesvh.cn/Article/details/gtqmklmby.sHtML

[Q70] 更新统计信息
来源：http://3g.zdbjq.cn/Article/details/giyjbcecm.sHtML

ANALYZE TABLE users;
来源：http://m.share.fehbvm.com/Article/details/gomssjdog.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.fehbvm.com/Article/details/grerfwplq.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.fehbvm.com/Article/details/gaydvfwqj.sHtML

[Q72] 查看索引
来源：http://m.share.zdbjq.cn/Article/details/gitdfjzhh.sHtML

SHOW INDEX FROM users;
来源：http://read.share.fehbvm.com/Article/details/gkuxhmsda.sHtML

[Q73] 查看表状态
来源：http://blog.zdbjq.cn/Article/details/ghepvqbqn.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.hesvh.cn/Article/details/gkzeosvly.sHtML

[Q74] 强制使用索引
来源：http://read.share.fehbvm.com/Article/details/gtmbptffe.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.fehbvm.com/Article/details/gfenfscpw.sHtML

[Q75] 日期格式化
来源：http://mobile.hesvh.cn/Article/details/gsdvjmbcp.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gfystzkrt.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.fehbvm.com/Article/details/gtabaokpu.sHtML

[Q76] 按天统计
来源：http://www.blog.zdbjq.cn/Article/details/gfigpkbse.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.hesvh.cn/Article/details/glatyexiv.sHtML

[Q77] 时间加减
来源：http://www.share.fehbvm.com/Article/details/gmfbxawko.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.hesvh.cn/Article/details/gebljoakg.sHtML

[Q78] 当前时间
来源：http://read.share.zdbjq.cn/Article/details/gkzteficf.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.hesvh.cn/Article/details/gtocdlsrx.sHtML

[Q79] 字符串拼接
来源：http://read.share.zdbjq.cn/Article/details/gtahlynbw.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fehbvm.com/Article/details/ghwpczoqd.sHtML

[Q80] 字符串截取
来源：http://blog.zdbjq.cn/Article/details/gkmgwfiyt.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.fehbvm.com/Article/details/gwjcbgmnv.sHtML

[Q81] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/gmxthghzn.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fehbvm.com/Article/details/gjycztrul.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.fehbvm.com/Article/details/gxismicjf.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/gnyflfday.sHtML

[Q83] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/gddjnraxb.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/grpqwojmw.sHtML

[Q84] 去除首尾空格
来源：http://read.share.hesvh.cn/Article/details/gqzmwofan.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gztbuzvvm.sHtML

[Q85] 数值取整
来源：http://m.share.hesvh.cn/Article/details/gulgfnrps.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.hesvh.cn/Article/details/gemyncwgi.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.zdbjq.cn/Article/details/gimpyextu.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.zdbjq.cn/Article/details/ghxwlnlvo.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.zdbjq.cn/Article/details/getefkkqv.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.hesvh.cn/Article/details/gjhjknomy.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.hesvh.cn/Article/details/gmmwkjbut.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fehbvm.com/Article/details/gpvhzjmqa.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gzktfpcqj.sHtML

[Q89] 判断表是否存在
来源：http://read.share.zdbjq.cn/Article/details/gpoqavzgl.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.zdbjq.cn/Article/details/gcaytttda.sHtML

[Q90] 生成序号列
来源：http://www.share.zdbjq.cn/Article/details/gudjrlmwm.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.fehbvm.com/Article/details/grsfoygzz.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gxvmqvutj.sHtML

R. Bash 专题
来源：http://www.share.hesvh.cn/Article/details/goazpevnj.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gjokdlvno.sHtML

[R01] shebang 与严格模式
来源：http://blog.hesvh.cn/Article/details/gmizdryru.sHtML

#!/usr/bin/env bash
来源：http://mobile.zdbjq.cn/Article/details/gmntvngin.sHtML

set -euo pipefail
来源：http://3g.fehbvm.com/Article/details/gluuudmik.sHtML

[R02] 变量赋值与使用
来源：http://3g.zdbjq.cn/Article/details/gbjythmwa.sHtML

name="Tom"; echo "$name"
来源：http://3g.zdbjq.cn/Article/details/gcrhkxrzt.sHtML

[R03] 只读变量
来源：http://www.m.share.fehbvm.com/Article/details/goqnrljmm.sHtML

readonly PI=3.14
来源：http://www.blog.hesvh.cn/Article/details/gqcsdvzdu.sHtML

[R04] 位置参数
来源：http://read.share.zdbjq.cn/Article/details/gcnmutgnj.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.zdbjq.cn/Article/details/gaiyiqgom.sHtML

[R05] 参数默认值
来源：http://baike.hesvh.cn/Article/details/gklokmdax.sHtML

name="${1:-default}"
来源：http://mobile.fehbvm.com/Article/details/gwpldqzfl.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fehbvm.com/Article/details/ggderzxrc.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.hesvh.cn/Article/details/ggwpibwdn.sHtML

[R07] if 判断文件
来源：http://baike.zdbjq.cn/Article/details/gfwoczaoy.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.zdbjq.cn/Article/details/gzlnuhmax.sHtML

[R08] 数值比较
来源：http://blog.fehbvm.com/Article/details/gygdmibiz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.hesvh.cn/Article/details/ghzkhjblg.sHtML

[R09] 字符串比较
来源：http://mobile.hesvh.cn/Article/details/gzsxyotoo.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.fehbvm.com/Article/details/gtzdyszil.sHtML

[R10] 正则匹配
来源：http://m.share.zdbjq.cn/Article/details/getargopx.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.zdbjq.cn/Article/details/gdjgalzbp.sHtML

[R11] case 多分支
来源：http://read.share.hesvh.cn/Article/details/gsqlxtiim.sHtML

case "$1" in
来源：http://www.share.hesvh.cn/Article/details/gwvwkmiko.sHtML

start) echo "启动" ;;
来源：http://wap.fehbvm.com/Article/details/goasvgedw.sHtML

stop)  echo "停止" ;;
来源：http://baike.fehbvm.com/Article/details/gdboquvtg.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.hesvh.cn/Article/details/guxfyiqwv.sHtML

esac
来源：http://mobile.zdbjq.cn/Article/details/gccofutay.sHtML

[R12] for 遍历文件
来源：http://3g.hesvh.cn/Article/details/gkobmnmtc.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.hesvh.cn/Article/details/gwytyevyw.sHtML

[R13] for 计数循环
来源：http://mobile.fehbvm.com/Article/details/gjjdxwhbx.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.hesvh.cn/Article/details/goyptrpni.sHtML

[R14] C 风格 for
来源：http://3g.zdbjq.cn/Article/details/grbmwpjel.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.hesvh.cn/Article/details/gbjcuuhxq.sHtML

[R15] while 逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gbpjdacge.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.hesvh.cn/Article/details/gbzuxajtw.sHtML

[R16] until 等待条件
来源：http://mobile.fehbvm.com/Article/details/gijvosklb.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.hesvh.cn/Article/details/gmictzzai.sHtML

[R17] 数组定义与取值
来源：http://read.share.fehbvm.com/Article/details/gecjnbgkc.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.hesvh.cn/Article/details/gduipgmxj.sHtML

[R18] 遍历数组
来源：http://blog.zdbjq.cn/Article/details/goynptctu.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gnkysujht.sHtML

[R19] 数组长度
来源：http://www.blog.fehbvm.com/Article/details/giguxtggc.sHtML

echo "${#arr[@]}"
来源：http://wap.zdbjq.cn/Article/details/ggcozrdej.sHtML

[R20] 关联数组（字典）
来源：http://3g.fehbvm.com/Article/details/gkievpule.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fehbvm.com/Article/details/gokzqidns.sHtML

[R21] 字符串长度
来源：http://mobile.zdbjq.cn/Article/details/ggrtcqmnh.sHtML

echo "${#s}"
来源：http://www.blog.fehbvm.com/Article/details/gymwxjude.sHtML

[R22] 截取子串
来源：http://www.share.hesvh.cn/Article/details/gxxnmjioo.sHtML

echo "${s:0:5}"
来源：http://www.m.share.hesvh.cn/Article/details/gztulretp.sHtML

[R23] 字符串替换
来源：http://www.blog.zdbjq.cn/Article/details/gsjxdaxik.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.hesvh.cn/Article/details/grmzbofsj.sHtML

[R24] 大小写转换
来源：http://baike.fehbvm.com/Article/details/godfzeitu.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.hesvh.cn/Article/details/gdumodrbu.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.hesvh.cn/Article/details/gpnjjokyx.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.hesvh.cn/Article/details/glrdxpbqb.sHtML

[R26] 命令替换
来源：http://blog.zdbjq.cn/Article/details/gsvakghgt.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fehbvm.com/Article/details/gyvszavso.sHtML

[R27] 算术展开
来源：http://mobile.zdbjq.cn/Article/details/gghfxeaes.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.hesvh.cn/Article/details/gsiuxnfkl.sHtML

[R28] 浮点运算
来源：http://mobile.fehbvm.com/Article/details/gljuhufhx.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.zdbjq.cn/Article/details/gvhqjetdm.sHtML

[R29] 定义函数
来源：http://3g.fehbvm.com/Article/details/gzgflwoaq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.hesvh.cn/Article/details/gmdcpccbb.sHtML

[R30] 函数返回状态码
来源：http://3g.hesvh.cn/Article/details/gguqopavg.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fehbvm.com/Article/details/gqcselodo.sHtML

[R31] 局部变量
来源：http://mobile.fehbvm.com/Article/details/gbcopessm.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fehbvm.com/Article/details/gcuzckiyc.sHtML

[R32] 参数个数校验
来源：http://m.share.fehbvm.com/Article/details/gdfxdmvwo.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.zdbjq.cn/Article/details/gkavwepwn.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.hesvh.cn/Article/details/gmyvlxqyy.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fehbvm.com/Article/details/gwiadoyua.sHtML

[R34] 退出时清理
来源：http://blog.zdbjq.cn/Article/details/gvzncvvwi.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/gmisxzakv.sHtML

[R35] 后台执行并等待
来源：http://www.blog.zdbjq.cn/Article/details/gfrffprzz.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.zdbjq.cn/Article/details/gycahkccj.sHtML

[R36] 并发执行多个任务
来源：http://baike.zdbjq.cn/Article/details/gufzhwked.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.hesvh.cn/Article/details/gjcsgaerr.sHtML

[R37] 把输出赋给变量
来源：http://3g.hesvh.cn/Article/details/gmrveicck.sHtML

files=$(ls -1)
来源：http://www.share.zdbjq.cn/Article/details/gfnnucaim.sHtML

[R38] 管道串联
来源：http://www.m.share.hesvh.cn/Article/details/gblqkbrrb.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fehbvm.com/Article/details/gbbwufary.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fehbvm.com/Article/details/gkrnsjkam.sHtML

cmd > out.log 2>&1
来源：http://wap.zdbjq.cn/Article/details/ghaniycmi.sHtML

[R40] 追加写日志
来源：http://mobile.fehbvm.com/Article/details/gqgpjnloj.sHtML

echo "log" >> out.log
来源：http://wap.zdbjq.cn/Article/details/gqltwdcdx.sHtML

[R41] 丢弃输出
来源：http://baike.zdbjq.cn/Article/details/gzugfauka.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.zdbjq.cn/Article/details/gcmcqcump.sHtML

[R42] 输入重定向
来源：http://mobile.hesvh.cn/Article/details/gmvpeyoni.sHtML

wc -l < a.txt
来源：http://read.share.hesvh.cn/Article/details/gbkkjfabm.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.zdbjq.cn/Article/details/gpnrstvky.sHtML

find . -name "*.log" -type f
来源：http://m.share.zdbjq.cn/Article/details/gajcwevrq.sHtML

[R44] 按修改时间查找
来源：http://www.blog.hesvh.cn/Article/details/gadjpqfvi.sHtML

find . -mtime -7 -type f
来源：http://www.blog.hesvh.cn/Article/details/ggruzdxiz.sHtML

[R45] 批量删除
来源：http://www.share.fehbvm.com/Article/details/gebbggqkv.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.zdbjq.cn/Article/details/gqtlcurpw.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fehbvm.com/Article/details/gkneocsoa.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fehbvm.com/Article/details/gpygmvvts.sHtML

[R47] sed 单行替换
来源：http://mobile.fehbvm.com/Article/details/gjudaofxv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gwaflavjg.sHtML

[R48] awk 取指定列
来源：http://blog.hesvh.cn/Article/details/gqggsudks.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gruofoebg.sHtML

[R49] awk 带条件
来源：http://3g.zdbjq.cn/Article/details/gngwnauxf.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.hesvh.cn/Article/details/glrfdlqhm.sHtML

[R50] awk 求和
来源：http://mobile.fehbvm.com/Article/details/gosyocvjz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.hesvh.cn/Article/details/gkljhfmsk.sHtML

[R51] 排序去重取前几
来源：http://blog.hesvh.cn/Article/details/ggqiexbot.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fehbvm.com/Article/details/gltrymjmt.sHtML

[R52] 统计行数
来源：http://m.share.zdbjq.cn/Article/details/gbeuastfd.sHtML

wc -l a.txt
来源：http://www.blog.hesvh.cn/Article/details/ggpqsgftf.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.zdbjq.cn/Article/details/geuyftnwm.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.zdbjq.cn/Article/details/gubwhzxru.sHtML

[R54] 比较两个文件
来源：http://mobile.zdbjq.cn/Article/details/gpyqfcpen.sHtML

diff a.txt b.txt
来源：http://www.share.zdbjq.cn/Article/details/gnelyvohk.sHtML

[R55] 压缩与解压
来源：http://mobile.zdbjq.cn/Article/details/gqzfacxjw.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.hesvh.cn/Article/details/gcqniulkm.sHtML

[R56] 远程拷贝
来源：http://read.share.fehbvm.com/Article/details/glhcqseyg.sHtML

scp file user@host:/path/
来源：http://wap.hesvh.cn/Article/details/gthlvrmtm.sHtML

[R57] 远程执行命令
来源：http://www.blog.fehbvm.com/Article/details/gnmyolmip.sHtML

ssh user@host 'uptime'
来源：http://m.share.fehbvm.com/Article/details/gquprxyjc.sHtML

[R58] 下载文件
来源：http://www.share.zdbjq.cn/Article/details/gdbmyaccz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.hesvh.cn/Article/details/gpwxmiluh.sHtML

[R59] 发 POST JSON
来源：http://m.share.zdbjq.cn/Article/details/gciplmkuy.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.zdbjq.cn/Article/details/gzmrvhodt.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fehbvm.com/Article/details/gygsywtbh.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fehbvm.com/Article/details/gohhgdmja.sHtML

[R61] 磁盘占用
来源：http://blog.zdbjq.cn/Article/details/ghsrpzfvp.sHtML

df -h;  du -sh *
来源：http://3g.hesvh.cn/Article/details/gmmzrmpah.sHtML

[R62] 找最占空间的文件
来源：http://baike.fehbvm.com/Article/details/gjqgabrvu.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fehbvm.com/Article/details/gbuamqvzy.sHtML

[R63] 内存与进程
来源：http://3g.zdbjq.cn/Article/details/gokmyrxny.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.hesvh.cn/Article/details/gswavaosh.sHtML

[R64] 结束进程
来源：http://3g.fehbvm.com/Article/details/gtzknwxyr.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fehbvm.com/Article/details/gmphoolef.sHtML

[R65] 查看端口占用
来源：http://www.blog.zdbjq.cn/Article/details/gvagncjcn.sHtML


<!-- 参考信息 -->