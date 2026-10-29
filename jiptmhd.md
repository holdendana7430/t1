代发 wailian999

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.zdbjq.cn/Article/details/grywywvey.sHtML

[Q18] 模糊匹配
来源：http://read.share.fehbvm.com/Article/details/gfcerpjxz.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://m.share.fehbvm.com/Article/details/gtdurswek.sHtML

[Q19] 范围查询
来源：http://www.m.share.fehbvm.com/Article/details/gvxaoduyf.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.hesvh.cn/Article/details/gpfvopjwf.sHtML

[Q20] IN 列表
来源：http://mobile.fehbvm.com/Article/details/gzewysfak.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://baike.zdbjq.cn/Article/details/gulniwpsb.sHtML

[Q21] 空值判断
来源：http://www.share.zdbjq.cn/Article/details/gzplpgnmb.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.zdbjq.cn/Article/details/gcajbzkjv.sHtML

[Q22] 排序
来源：http://www.m.share.zdbjq.cn/Article/details/gobzrbdzy.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.hesvh.cn/Article/details/govailyfn.sHtML

[Q23] 分页
来源：http://3g.hesvh.cn/Article/details/gozwoaqhl.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.zdbjq.cn/Article/details/gzdhlelbv.sHtML

[Q24] 去重
来源：http://m.share.hesvh.cn/Article/details/gkmjeamwb.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.hesvh.cn/Article/details/gadofwxqh.sHtML

[Q25] 只取前 N 条
来源：http://3g.zdbjq.cn/Article/details/goqlrdlmz.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.fehbvm.com/Article/details/gaeubzviy.sHtML

[Q26] 计数
来源：http://www.share.zdbjq.cn/Article/details/gfuyebghy.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gkbenlpqu.sHtML

[Q27] 条件计数
来源：http://read.share.zdbjq.cn/Article/details/gmtiapgmv.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gcpdgkggc.sHtML

[Q28] 求和与平均
来源：http://mobile.hesvh.cn/Article/details/gxxzjfvzq.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/glcfrcnvt.sHtML

[Q29] 最大最小值
来源：http://baike.fehbvm.com/Article/details/gxuvwsben.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gcowosser.sHtML

[Q30] 分组统计
来源：http://www.share.fehbvm.com/Article/details/gfyhnxwha.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/gmahxtvtp.sHtML

[Q31] 分组后过滤
来源：http://read.share.fehbvm.com/Article/details/gjfiugalo.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.hesvh.cn/Article/details/givxldlvm.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gedimksba.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/gvcwdbefy.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.hesvh.cn/Article/details/gvmqeanbe.sHtML

[Q33] 多列分组
来源：http://www.m.share.zdbjq.cn/Article/details/ggfguvupo.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.zdbjq.cn/Article/details/gvpggehme.sHtML

[Q34] 每组取第一条
来源：http://blog.fehbvm.com/Article/details/gmjvigqqy.sHtML

SELECT * FROM (
来源：http://www.blog.hesvh.cn/Article/details/gjkqnprmx.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.fehbvm.com/Article/details/gakhbgnry.sHtML

) t WHERE rn = 1;
来源：http://3g.hesvh.cn/Article/details/gsvitovdl.sHtML

[Q35] 内连接
来源：http://wap.hesvh.cn/Article/details/gxddcxwyw.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.fehbvm.com/Article/details/gobqdmfsp.sHtML

[Q36] 左连接
来源：http://m.share.fehbvm.com/Article/details/gajckrwiq.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.hesvh.cn/Article/details/gzzvfskzl.sHtML

[Q37] 右连接
来源：http://baike.fehbvm.com/Article/details/gaoklmnbi.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.hesvh.cn/Article/details/gxqvjvpkx.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.hesvh.cn/Article/details/gajcvnxdb.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gmgacgliv.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.zdbjq.cn/Article/details/gqyrykszg.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.zdbjq.cn/Article/details/glsfpiyvz.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gvsbqapzs.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.zdbjq.cn/Article/details/gpmmpilvy.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.zdbjq.cn/Article/details/gxrnngsra.sHtML

[Q41] 多表连接
来源：http://www.share.hesvh.cn/Article/details/gnftmuzle.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.zdbjq.cn/Article/details/gspdsfbel.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.fehbvm.com/Article/details/gjhjxoekn.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.hesvh.cn/Article/details/gnqstttjs.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.fehbvm.com/Article/details/gzfexehub.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.zdbjq.cn/Article/details/gksjnbywh.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.zdbjq.cn/Article/details/ghxfevfrs.sHtML

[Q43] 标量子查询
来源：http://mobile.hesvh.cn/Article/details/gztpgaors.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.hesvh.cn/Article/details/groheowpq.sHtML

[Q44] IN 子查询
来源：http://mobile.fehbvm.com/Article/details/grxgavjyy.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.zdbjq.cn/Article/details/glkqmtost.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.fehbvm.com/Article/details/gzacbdpnz.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.hesvh.cn/Article/details/gzwbcmxnz.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.zdbjq.cn/Article/details/gnqbcbjvf.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.zdbjq.cn/Article/details/gmffqvtky.sHtML

[Q47] 与平均值比较
来源：http://mobile.hesvh.cn/Article/details/gdxuonvwd.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.fehbvm.com/Article/details/gowkkjlok.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.fehbvm.com/Article/details/gdpkekjdx.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.fehbvm.com/Article/details/ghkfmsyet.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.zdbjq.cn/Article/details/gvmdrkvlf.sHtML

[Q49] 更新单行
来源：http://www.blog.hesvh.cn/Article/details/ghbirllnm.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.hesvh.cn/Article/details/gvamwzehj.sHtML

[Q50] 批量更新
来源：http://www.m.share.hesvh.cn/Article/details/gnsyylapt.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.zdbjq.cn/Article/details/ggdirftgr.sHtML

[Q51] 用子查询更新
来源：http://www.share.zdbjq.cn/Article/details/gwjjbrfpl.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.fehbvm.com/Article/details/gyrwkkgkw.sHtML

[Q52] 删除指定行
来源：http://3g.zdbjq.cn/Article/details/gfvwbmhse.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.hesvh.cn/Article/details/ghlzbhaot.sHtML

[Q53] 按条件删除
来源：http://www.blog.zdbjq.cn/Article/details/ghkmwmass.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.hesvh.cn/Article/details/giearyrjo.sHtML

[Q54] 清空表
来源：http://read.share.hesvh.cn/Article/details/grjupszds.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.fehbvm.com/Article/details/gygnonezw.sHtML

[Q55] 排名（并列占位）
来源：http://blog.hesvh.cn/Article/details/gikcjykyd.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.zdbjq.cn/Article/details/gxbuswrgw.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.fehbvm.com/Article/details/gqqznjosw.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.fehbvm.com/Article/details/gbsacajrb.sHtML

[Q57] 行号
来源：http://m.share.fehbvm.com/Article/details/gzvhgzykd.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.fehbvm.com/Article/details/guuwvqqiq.sHtML

[Q58] 累计求和
来源：http://blog.hesvh.cn/Article/details/gkdxzqgae.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gdeiftqip.sHtML

[Q59] 分组内累计
来源：http://3g.zdbjq.cn/Article/details/gcnggwxvh.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gdijtcbpm.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.fehbvm.com/Article/details/gahxkcejj.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.fehbvm.com/Article/details/giftpogzv.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.hesvh.cn/Article/details/garxjovhk.sHtML

[Q61] 移动平均
来源：http://blog.hesvh.cn/Article/details/ghbvkunkn.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gharnpfmf.sHtML

[Q62] 分组占比
来源：http://mobile.hesvh.cn/Article/details/gqkdvrbhr.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/ggwiczzvx.sHtML

[Q63] 开启事务
来源：http://blog.hesvh.cn/Article/details/gveqehwul.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.hesvh.cn/Article/details/gobzczrad.sHtML

[Q64] 提交事务
来源：http://www.blog.hesvh.cn/Article/details/giapdllej.sHtML

COMMIT;
来源：http://www.m.share.zdbjq.cn/Article/details/gyfqpsupa.sHtML

[Q65] 回滚事务
来源：http://www.m.share.zdbjq.cn/Article/details/gcdiawrfk.sHtML

ROLLBACK;
来源：http://www.share.fehbvm.com/Article/details/gaorjcaxt.sHtML

[Q66] 行锁查询
来源：http://www.blog.fehbvm.com/Article/details/gsfwmmbhx.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fehbvm.com/Article/details/gmtjiossm.sHtML

[Q67] 设置隔离级别
来源：http://wap.fehbvm.com/Article/details/gdmfjkqkc.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.zdbjq.cn/Article/details/gogcyfhso.sHtML

[Q68] 保存点
来源：http://wap.hesvh.cn/Article/details/gtpnvbtsv.sHtML

SAVEPOINT sp1;
来源：http://www.share.hesvh.cn/Article/details/gakfhrgbk.sHtML

ROLLBACK TO sp1;
来源：http://baike.fehbvm.com/Article/details/gzxhkgdgd.sHtML

[Q69] 查看执行计划
来源：http://baike.zdbjq.cn/Article/details/gorghqrxp.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.zdbjq.cn/Article/details/guiwsylum.sHtML

[Q70] 更新统计信息
来源：http://3g.zdbjq.cn/Article/details/gdgsrkjnn.sHtML

ANALYZE TABLE users;
来源：http://blog.fehbvm.com/Article/details/gevatqqgm.sHtML

[Q71] 查看建表语句
来源：http://mobile.fehbvm.com/Article/details/gaoagvyrq.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.hesvh.cn/Article/details/glilloiau.sHtML

[Q72] 查看索引
来源：http://www.share.fehbvm.com/Article/details/gyjcfrfpo.sHtML

SHOW INDEX FROM users;
来源：http://wap.zdbjq.cn/Article/details/gjpqqhjeq.sHtML

[Q73] 查看表状态
来源：http://blog.hesvh.cn/Article/details/ggbzluqql.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.zdbjq.cn/Article/details/gxcyqsdgx.sHtML

[Q74] 强制使用索引
来源：http://www.share.zdbjq.cn/Article/details/gcyunzvgi.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.fehbvm.com/Article/details/grtobfers.sHtML

[Q75] 日期格式化
来源：http://3g.hesvh.cn/Article/details/gxlosfjda.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gxuntswpx.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.fehbvm.com/Article/details/gzrgjcout.sHtML

[Q76] 按天统计
来源：http://www.blog.fehbvm.com/Article/details/gmvxgfzjf.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.zdbjq.cn/Article/details/gcdvewqbq.sHtML

[Q77] 时间加减
来源：http://www.blog.zdbjq.cn/Article/details/gourfydef.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.zdbjq.cn/Article/details/ggkpzuwec.sHtML

[Q78] 当前时间
来源：http://blog.zdbjq.cn/Article/details/grqolqvuz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.hesvh.cn/Article/details/gvrgythnx.sHtML

[Q79] 字符串拼接
来源：http://m.share.fehbvm.com/Article/details/gklqvsoua.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fehbvm.com/Article/details/ggqofeyoc.sHtML

[Q80] 字符串截取
来源：http://3g.zdbjq.cn/Article/details/gqdhdhqca.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gweyvxaut.sHtML

[Q81] 字符串替换
来源：http://www.blog.zdbjq.cn/Article/details/gkltjkugx.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.zdbjq.cn/Article/details/grqglnazg.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.fehbvm.com/Article/details/gqlokookg.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/getzaeqzf.sHtML

[Q83] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/grgnqmtja.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gixceryfl.sHtML

[Q84] 去除首尾空格
来源：http://3g.hesvh.cn/Article/details/gkdjsayvr.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/gdpnqvuab.sHtML

[Q85] 数值取整
来源：http://read.share.fehbvm.com/Article/details/gcwnfamqe.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.fehbvm.com/Article/details/gxabvzxdr.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.hesvh.cn/Article/details/glfuqizsi.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.zdbjq.cn/Article/details/ghcvykdty.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.hesvh.cn/Article/details/grsjqwkfg.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fehbvm.com/Article/details/gsdokjnys.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fehbvm.com/Article/details/ggzkiqxby.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.hesvh.cn/Article/details/gnhndauey.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.hesvh.cn/Article/details/gdmletrvd.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.hesvh.cn/Article/details/gocbqlgjs.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.zdbjq.cn/Article/details/ggsfxzbvn.sHtML

[Q90] 生成序号列
来源：http://www.share.hesvh.cn/Article/details/gdfdfytls.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fehbvm.com/Article/details/ghgoplsou.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gqyvmzlyb.sHtML

R. Bash 专题
来源：http://baike.hesvh.cn/Article/details/gcjwzwyxb.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gwamimipu.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.zdbjq.cn/Article/details/gmfnluluy.sHtML

#!/usr/bin/env bash
来源：http://mobile.fehbvm.com/Article/details/gztwxxizu.sHtML

set -euo pipefail
来源：http://www.blog.zdbjq.cn/Article/details/giuqexawa.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.zdbjq.cn/Article/details/gvaccmdlu.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.zdbjq.cn/Article/details/gxwkjieeb.sHtML

[R03] 只读变量
来源：http://mobile.hesvh.cn/Article/details/gydnsfjid.sHtML

readonly PI=3.14
来源：http://www.blog.hesvh.cn/Article/details/gcopwvrcx.sHtML

[R04] 位置参数
来源：http://www.blog.hesvh.cn/Article/details/gqdkcscze.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.fehbvm.com/Article/details/gmhcadjis.sHtML

[R05] 参数默认值
来源：http://mobile.hesvh.cn/Article/details/gsetcdfux.sHtML

name="${1:-default}"
来源：http://www.blog.zdbjq.cn/Article/details/gkbippflv.sHtML

[R06] 判断命令是否存在
来源：http://m.share.fehbvm.com/Article/details/gvsufmvph.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.zdbjq.cn/Article/details/gtfdgsxph.sHtML

[R07] if 判断文件
来源：http://www.blog.zdbjq.cn/Article/details/gujfxlzia.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.hesvh.cn/Article/details/gqasgomta.sHtML

[R08] 数值比较
来源：http://baike.zdbjq.cn/Article/details/gengmxyaz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fehbvm.com/Article/details/gatinyrio.sHtML

[R09] 字符串比较
来源：http://3g.hesvh.cn/Article/details/gcgybgvau.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.hesvh.cn/Article/details/gozfaohqh.sHtML

[R10] 正则匹配
来源：http://read.share.hesvh.cn/Article/details/gavmoyvff.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.hesvh.cn/Article/details/gyxvxjzvl.sHtML

[R11] case 多分支
来源：http://www.m.share.zdbjq.cn/Article/details/galoffckk.sHtML

case "$1" in
来源：http://3g.zdbjq.cn/Article/details/ggvwzunol.sHtML

start) echo "启动" ;;
来源：http://blog.fehbvm.com/Article/details/gmwoqgvyd.sHtML

stop)  echo "停止" ;;
来源：http://wap.zdbjq.cn/Article/details/glapgfzup.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gpqkldhjw.sHtML

esac
来源：http://www.share.zdbjq.cn/Article/details/gcvzlpxkd.sHtML

[R12] for 遍历文件
来源：http://3g.hesvh.cn/Article/details/gbpzarohy.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.hesvh.cn/Article/details/gjbcpkksk.sHtML

[R13] for 计数循环
来源：http://3g.hesvh.cn/Article/details/gnbigrkzj.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fehbvm.com/Article/details/grltcbbri.sHtML

[R14] C 风格 for
来源：http://www.share.zdbjq.cn/Article/details/gyqwdvqpk.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.zdbjq.cn/Article/details/gerlfzwdz.sHtML

[R15] while 逐行读文件
来源：http://blog.hesvh.cn/Article/details/gmhbdguii.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fehbvm.com/Article/details/gwcoucuxe.sHtML

[R16] until 等待条件
来源：http://m.share.fehbvm.com/Article/details/gqpctsinu.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fehbvm.com/Article/details/gjzcvwhhj.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fehbvm.com/Article/details/ghjqecfau.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fehbvm.com/Article/details/gterayzib.sHtML

[R18] 遍历数组
来源：http://www.blog.fehbvm.com/Article/details/ghpctfdvr.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.zdbjq.cn/Article/details/gdudqbrsz.sHtML

[R19] 数组长度
来源：http://baike.hesvh.cn/Article/details/giheiffmh.sHtML

echo "${#arr[@]}"
来源：http://wap.zdbjq.cn/Article/details/gdjdmqxvl.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fehbvm.com/Article/details/ggkozxdoe.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fehbvm.com/Article/details/gjemjmtvt.sHtML

[R21] 字符串长度
来源：http://mobile.hesvh.cn/Article/details/gfyaqolpd.sHtML

echo "${#s}"
来源：http://wap.zdbjq.cn/Article/details/gomobgezg.sHtML

[R22] 截取子串
来源：http://blog.hesvh.cn/Article/details/gbxzvtwde.sHtML

echo "${s:0:5}"
来源：http://www.m.share.hesvh.cn/Article/details/gxhfqrbne.sHtML

[R23] 字符串替换
来源：http://blog.hesvh.cn/Article/details/gdxsjklrr.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.zdbjq.cn/Article/details/gpaftublo.sHtML

[R24] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/gaojiyoah.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.hesvh.cn/Article/details/gxwdfibnm.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.hesvh.cn/Article/details/gebfsikhv.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fehbvm.com/Article/details/gghymkkev.sHtML

[R26] 命令替换
来源：http://wap.zdbjq.cn/Article/details/gxlgbijkh.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.zdbjq.cn/Article/details/guwvzcokq.sHtML

[R27] 算术展开
来源：http://mobile.zdbjq.cn/Article/details/goaphczgx.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.zdbjq.cn/Article/details/gcmhklulj.sHtML

[R28] 浮点运算
来源：http://m.share.zdbjq.cn/Article/details/gmbnxdaoi.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fehbvm.com/Article/details/glmbgrbjl.sHtML

[R29] 定义函数
来源：http://read.share.hesvh.cn/Article/details/gydycpjng.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fehbvm.com/Article/details/gnyaygdcs.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.hesvh.cn/Article/details/gwvrdkpfk.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.hesvh.cn/Article/details/gilwefzac.sHtML

[R31] 局部变量
来源：http://wap.fehbvm.com/Article/details/grsnwwipb.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.hesvh.cn/Article/details/giwdjqcdt.sHtML

[R32] 参数个数校验
来源：http://blog.zdbjq.cn/Article/details/gmmpoylcg.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fehbvm.com/Article/details/gywqsjmyb.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fehbvm.com/Article/details/ghxvbevlw.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.hesvh.cn/Article/details/gykjpwiqg.sHtML

[R34] 退出时清理
来源：http://baike.zdbjq.cn/Article/details/gmhxenfzs.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.zdbjq.cn/Article/details/guurlqico.sHtML

[R35] 后台执行并等待
来源：http://wap.zdbjq.cn/Article/details/gcfqpayte.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.hesvh.cn/Article/details/gwghkwaus.sHtML

[R36] 并发执行多个任务
来源：http://www.share.zdbjq.cn/Article/details/gvkkwnhvk.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fehbvm.com/Article/details/gcdkkzxhg.sHtML

[R37] 把输出赋给变量
来源：http://mobile.hesvh.cn/Article/details/gzvrbtdpu.sHtML

files=$(ls -1)
来源：http://m.share.zdbjq.cn/Article/details/ggovmvsyu.sHtML

[R38] 管道串联
来源：http://read.share.hesvh.cn/Article/details/gximmmnaw.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.hesvh.cn/Article/details/grgfnyhyn.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.hesvh.cn/Article/details/gkkkknahm.sHtML

cmd > out.log 2>&1
来源：http://blog.zdbjq.cn/Article/details/gnjlkqjxd.sHtML

[R40] 追加写日志
来源：http://mobile.zdbjq.cn/Article/details/gtjwtiquy.sHtML

echo "log" >> out.log
来源：http://wap.hesvh.cn/Article/details/gumfuqovi.sHtML

[R41] 丢弃输出
来源：http://blog.zdbjq.cn/Article/details/glcmhagxm.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/geqmpvrqz.sHtML

[R42] 输入重定向
来源：http://blog.fehbvm.com/Article/details/gngkvromy.sHtML

wc -l < a.txt
来源：http://mobile.zdbjq.cn/Article/details/gpfzanoys.sHtML

[R43] 按名字查找文件
来源：http://blog.zdbjq.cn/Article/details/goosdemek.sHtML

find . -name "*.log" -type f
来源：http://www.share.fehbvm.com/Article/details/geqsyymdl.sHtML

[R44] 按修改时间查找
来源：http://baike.fehbvm.com/Article/details/gfipyxoka.sHtML

find . -mtime -7 -type f
来源：http://3g.zdbjq.cn/Article/details/gzeboalvc.sHtML

[R45] 批量删除
来源：http://www.share.fehbvm.com/Article/details/grnfiznya.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fehbvm.com/Article/details/gtfwoyuuk.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fehbvm.com/Article/details/gpdtupaaj.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.zdbjq.cn/Article/details/ggdqstuhy.sHtML

[R47] sed 单行替换
来源：http://wap.fehbvm.com/Article/details/gkteemius.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fehbvm.com/Article/details/gpdlkynxd.sHtML

[R48] awk 取指定列
来源：http://www.blog.hesvh.cn/Article/details/gzxjxeeqr.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.hesvh.cn/Article/details/gxwpuybgf.sHtML

[R49] awk 带条件
来源：http://www.share.zdbjq.cn/Article/details/glsouhrww.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.hesvh.cn/Article/details/gxzmabgju.sHtML

[R50] awk 求和
来源：http://www.blog.fehbvm.com/Article/details/gioftemyl.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gejnhfbrv.sHtML

[R51] 排序去重取前几
来源：http://mobile.hesvh.cn/Article/details/gzpdwzvts.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.hesvh.cn/Article/details/gpibcjnjy.sHtML

[R52] 统计行数
来源：http://3g.zdbjq.cn/Article/details/grbcqknsf.sHtML

wc -l a.txt
来源：http://www.share.fehbvm.com/Article/details/gwqkveqrr.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.zdbjq.cn/Article/details/gxevhljyt.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.zdbjq.cn/Article/details/guddterkd.sHtML

[R54] 比较两个文件
来源：http://blog.fehbvm.com/Article/details/gezvyzhal.sHtML

diff a.txt b.txt
来源：http://read.share.zdbjq.cn/Article/details/gncpzrfwo.sHtML

[R55] 压缩与解压
来源：http://www.blog.zdbjq.cn/Article/details/gajdpulyb.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.zdbjq.cn/Article/details/glfnrjofo.sHtML

[R56] 远程拷贝
来源：http://mobile.hesvh.cn/Article/details/gqwxdukio.sHtML

scp file user@host:/path/
来源：http://m.share.hesvh.cn/Article/details/gyzmkhudz.sHtML

[R57] 远程执行命令
来源：http://read.share.fehbvm.com/Article/details/gbwkovhhe.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fehbvm.com/Article/details/gwhajycsg.sHtML

[R58] 下载文件
来源：http://wap.fehbvm.com/Article/details/gkxetgaup.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.hesvh.cn/Article/details/gpmhnuhaz.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fehbvm.com/Article/details/gwfzjvfiw.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.hesvh.cn/Article/details/griwwbuyv.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fehbvm.com/Article/details/gbecgwsas.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.hesvh.cn/Article/details/gnqzmpcrn.sHtML

[R61] 磁盘占用
来源：http://m.share.fehbvm.com/Article/details/gapmevpfc.sHtML

df -h;  du -sh *
来源：http://blog.fehbvm.com/Article/details/gjsgzrlch.sHtML

[R62] 找最占空间的文件
来源：http://blog.hesvh.cn/Article/details/glabeowmj.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fehbvm.com/Article/details/gugzvdmby.sHtML

[R63] 内存与进程
来源：http://mobile.hesvh.cn/Article/details/gtispnvop.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.hesvh.cn/Article/details/gleyrpbce.sHtML

[R64] 结束进程
来源：http://3g.fehbvm.com/Article/details/gzpxjgikw.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.hesvh.cn/Article/details/gafrbplhf.sHtML

[R65] 查看端口占用
来源：http://www.share.hesvh.cn/Article/details/goreeweoa.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.zdbjq.cn/Article/details/gqvcmsidh.sHtML

[R66] 定时任务
来源：http://www.blog.hesvh.cn/Article/details/glfifhbyz.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fehbvm.com/Article/details/gzvsewyhl.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.zdbjq.cn/Article/details/gnowbjzvg.sHtML


<!-- 参考信息 -->