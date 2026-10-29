代发 wailian999

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://wap.zdbjq.cn/Article/details/gxkrkulwo.sHtML

[Q18] 模糊匹配
来源：http://baike.hesvh.cn/Article/details/gzmtneiae.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://baike.fehbvm.com/Article/details/gkgmtmwml.sHtML

[Q19] 范围查询
来源：http://www.share.fehbvm.com/Article/details/gzyvvpaqj.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://read.share.hesvh.cn/Article/details/gqwmywxcq.sHtML

[Q20] IN 列表
来源：http://www.share.hesvh.cn/Article/details/gurkodncl.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.zdbjq.cn/Article/details/glhagagkp.sHtML

[Q21] 空值判断
来源：http://www.blog.fehbvm.com/Article/details/gllpbaocy.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.zdbjq.cn/Article/details/gxgitajgg.sHtML

[Q22] 排序
来源：http://blog.zdbjq.cn/Article/details/gaiifwbqi.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://read.share.hesvh.cn/Article/details/gzzthpbhb.sHtML

[Q23] 分页
来源：http://wap.fehbvm.com/Article/details/gdyffoeud.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.hesvh.cn/Article/details/gjfcvowcm.sHtML

[Q24] 去重
来源：http://www.blog.fehbvm.com/Article/details/gkixtjgor.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gxdfdaarm.sHtML

[Q25] 只取前 N 条
来源：http://mobile.fehbvm.com/Article/details/gmgvhnbgg.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.zdbjq.cn/Article/details/gghxfhxcb.sHtML

[Q26] 计数
来源：http://m.share.zdbjq.cn/Article/details/gfsmghvcn.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gurzkgcuz.sHtML

[Q27] 条件计数
来源：http://wap.zdbjq.cn/Article/details/gsvoqjhnf.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gfhbqcapd.sHtML

[Q28] 求和与平均
来源：http://www.blog.fehbvm.com/Article/details/gmfpcxxuf.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gmkyuemxl.sHtML

[Q29] 最大最小值
来源：http://www.blog.hesvh.cn/Article/details/grkxwneoz.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gctnbxvdq.sHtML

[Q30] 分组统计
来源：http://www.blog.fehbvm.com/Article/details/gbxtxqqwh.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.hesvh.cn/Article/details/gqwduvcbn.sHtML

[Q31] 分组后过滤
来源：http://3g.hesvh.cn/Article/details/gyhkulxnr.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.hesvh.cn/Article/details/gebpzbzkn.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.hesvh.cn/Article/details/gjbpcmczw.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gnixeexig.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.hesvh.cn/Article/details/gjzswsjnf.sHtML

[Q33] 多列分组
来源：http://baike.hesvh.cn/Article/details/gsmsawjdr.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.hesvh.cn/Article/details/gawerfhvi.sHtML

[Q34] 每组取第一条
来源：http://mobile.fehbvm.com/Article/details/gdnrkxcbd.sHtML

SELECT * FROM (
来源：http://m.share.hesvh.cn/Article/details/gjchbtgbr.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.hesvh.cn/Article/details/gbezxebll.sHtML

) t WHERE rn = 1;
来源：http://m.share.zdbjq.cn/Article/details/ghesxqguj.sHtML

[Q35] 内连接
来源：http://mobile.fehbvm.com/Article/details/gvzbzheoh.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.hesvh.cn/Article/details/galwxkqzq.sHtML

[Q36] 左连接
来源：http://read.share.fehbvm.com/Article/details/ggeopicvk.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.zdbjq.cn/Article/details/gvvaudkqe.sHtML

[Q37] 右连接
来源：http://wap.hesvh.cn/Article/details/gpyndyvbt.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.zdbjq.cn/Article/details/gvgydrrtn.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.fehbvm.com/Article/details/gagxabuax.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.fehbvm.com/Article/details/gqmfmffiq.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.fehbvm.com/Article/details/gwomigedt.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.zdbjq.cn/Article/details/giqtshtzp.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.zdbjq.cn/Article/details/gmashmfej.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.zdbjq.cn/Article/details/gwmxxyocd.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.zdbjq.cn/Article/details/gejwpgcez.sHtML

[Q41] 多表连接
来源：http://www.blog.fehbvm.com/Article/details/grrjpkrrr.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.fehbvm.com/Article/details/glisocfkg.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.hesvh.cn/Article/details/grmmurfmi.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.fehbvm.com/Article/details/gmcuqhhco.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gzibybctb.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.hesvh.cn/Article/details/gqmsqyqtw.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.hesvh.cn/Article/details/gaqnkokcx.sHtML

[Q43] 标量子查询
来源：http://www.share.zdbjq.cn/Article/details/gxirhfolh.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.zdbjq.cn/Article/details/gbsgysamg.sHtML

[Q44] IN 子查询
来源：http://www.m.share.zdbjq.cn/Article/details/gsgklcuav.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.fehbvm.com/Article/details/gwgldeabx.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.hesvh.cn/Article/details/gkaiztzrc.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.hesvh.cn/Article/details/gattmtnap.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.zdbjq.cn/Article/details/gkzubvmey.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fehbvm.com/Article/details/gevahgxje.sHtML

[Q47] 与平均值比较
来源：http://blog.zdbjq.cn/Article/details/gascqqirc.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.hesvh.cn/Article/details/gjcianhgj.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.hesvh.cn/Article/details/gcfkedcaa.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.zdbjq.cn/Article/details/gwdjpmeen.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.hesvh.cn/Article/details/gsfciweqx.sHtML

[Q49] 更新单行
来源：http://www.share.zdbjq.cn/Article/details/gbdjdrnsq.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.hesvh.cn/Article/details/gxjslurkr.sHtML

[Q50] 批量更新
来源：http://3g.hesvh.cn/Article/details/gzjcvazkz.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.fehbvm.com/Article/details/grhzkbfzk.sHtML

[Q51] 用子查询更新
来源：http://read.share.hesvh.cn/Article/details/ggagrvord.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.hesvh.cn/Article/details/gprwllnlr.sHtML

[Q52] 删除指定行
来源：http://m.share.fehbvm.com/Article/details/gsepxxela.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.fehbvm.com/Article/details/geslfnzrf.sHtML

[Q53] 按条件删除
来源：http://blog.hesvh.cn/Article/details/gjbqrdzmb.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.hesvh.cn/Article/details/gyglximou.sHtML

[Q54] 清空表
来源：http://www.blog.hesvh.cn/Article/details/gamgxdwes.sHtML

TRUNCATE TABLE logs;
来源：http://baike.zdbjq.cn/Article/details/gsvcwarsl.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.hesvh.cn/Article/details/gdrchsmvc.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.fehbvm.com/Article/details/grpsrwchs.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.hesvh.cn/Article/details/gxnvqpraq.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.hesvh.cn/Article/details/gfpsnjdib.sHtML

[Q57] 行号
来源：http://blog.zdbjq.cn/Article/details/grravbqxt.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.zdbjq.cn/Article/details/gtofkwmcc.sHtML

[Q58] 累计求和
来源：http://3g.fehbvm.com/Article/details/gkazpkqyf.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gslmdpjyg.sHtML

[Q59] 分组内累计
来源：http://www.share.fehbvm.com/Article/details/ghmgycyfq.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.fehbvm.com/Article/details/gehvzfoit.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.fehbvm.com/Article/details/gxgoicbjf.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.zdbjq.cn/Article/details/gcxmvbrjr.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.fehbvm.com/Article/details/glhvesqfq.sHtML

[Q61] 移动平均
来源：http://read.share.zdbjq.cn/Article/details/giapyxtar.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.hesvh.cn/Article/details/gilhadmic.sHtML

[Q62] 分组占比
来源：http://read.share.zdbjq.cn/Article/details/gdeutepjd.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/gynmuzmqy.sHtML

[Q63] 开启事务
来源：http://blog.hesvh.cn/Article/details/gymafjxge.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.zdbjq.cn/Article/details/gnwjnjnti.sHtML

[Q64] 提交事务
来源：http://baike.fehbvm.com/Article/details/gsyearfll.sHtML

COMMIT;
来源：http://blog.hesvh.cn/Article/details/gukhdjdcq.sHtML

[Q65] 回滚事务
来源：http://wap.hesvh.cn/Article/details/gvxsvekoc.sHtML

ROLLBACK;
来源：http://blog.hesvh.cn/Article/details/gdtzzrulb.sHtML

[Q66] 行锁查询
来源：http://mobile.zdbjq.cn/Article/details/gltmlvtdr.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.zdbjq.cn/Article/details/gsvleeufe.sHtML

[Q67] 设置隔离级别
来源：http://read.share.zdbjq.cn/Article/details/gxarnqkcp.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.fehbvm.com/Article/details/ghxmopfix.sHtML

[Q68] 保存点
来源：http://read.share.hesvh.cn/Article/details/gonueolrk.sHtML

SAVEPOINT sp1;
来源：http://www.share.fehbvm.com/Article/details/gojandtcb.sHtML

ROLLBACK TO sp1;
来源：http://mobile.zdbjq.cn/Article/details/gazncumes.sHtML

[Q69] 查看执行计划
来源：http://mobile.fehbvm.com/Article/details/gddbazrnu.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.fehbvm.com/Article/details/guouwyxyz.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fehbvm.com/Article/details/geeduogmv.sHtML

ANALYZE TABLE users;
来源：http://m.share.fehbvm.com/Article/details/gptrdlckw.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.hesvh.cn/Article/details/gtlggxeaj.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.hesvh.cn/Article/details/gwajbgvxe.sHtML

[Q72] 查看索引
来源：http://mobile.fehbvm.com/Article/details/ghvnadgjv.sHtML

SHOW INDEX FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gpltismpi.sHtML

[Q73] 查看表状态
来源：http://blog.fehbvm.com/Article/details/gmilntjbi.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.zdbjq.cn/Article/details/gqtnmjymb.sHtML

[Q74] 强制使用索引
来源：http://3g.hesvh.cn/Article/details/gqujmdfal.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fehbvm.com/Article/details/gcixyqfuu.sHtML

[Q75] 日期格式化
来源：http://mobile.hesvh.cn/Article/details/gpkzfxtza.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gumevmlyn.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.fehbvm.com/Article/details/gkumpotyw.sHtML

[Q76] 按天统计
来源：http://read.share.zdbjq.cn/Article/details/ggrwpoxtl.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.zdbjq.cn/Article/details/gcfumdxzk.sHtML

[Q77] 时间加减
来源：http://wap.zdbjq.cn/Article/details/gyvbkflri.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.fehbvm.com/Article/details/godookfbn.sHtML

[Q78] 当前时间
来源：http://wap.fehbvm.com/Article/details/goxuunihk.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.hesvh.cn/Article/details/gidhaprwy.sHtML

[Q79] 字符串拼接
来源：http://www.share.hesvh.cn/Article/details/gpqhipxwc.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.zdbjq.cn/Article/details/gmrxdwgld.sHtML

[Q80] 字符串截取
来源：http://mobile.hesvh.cn/Article/details/gdadrjujo.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gqbeoiwva.sHtML

[Q81] 字符串替换
来源：http://blog.zdbjq.cn/Article/details/gvwpwcxei.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fehbvm.com/Article/details/gfhwcdafv.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.zdbjq.cn/Article/details/ggoqvbstz.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gsyshceli.sHtML

[Q83] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/gzjriywin.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gowgjvtug.sHtML

[Q84] 去除首尾空格
来源：http://baike.fehbvm.com/Article/details/gnzceobvs.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gyegtjtci.sHtML

[Q85] 数值取整
来源：http://www.share.fehbvm.com/Article/details/grfiigczp.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.zdbjq.cn/Article/details/ggfwzhtee.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.zdbjq.cn/Article/details/gcopaqrmk.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.zdbjq.cn/Article/details/gsgajbcub.sHtML

[Q87] JSON 字段做条件
来源：http://wap.zdbjq.cn/Article/details/gsxoydpyn.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.hesvh.cn/Article/details/gxlpjmdbq.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.hesvh.cn/Article/details/goztpuzus.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.zdbjq.cn/Article/details/grvecnrvy.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.hesvh.cn/Article/details/gzenezzxg.sHtML

[Q89] 判断表是否存在
来源：http://wap.zdbjq.cn/Article/details/geabcfbtp.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.hesvh.cn/Article/details/gldegqvpn.sHtML

[Q90] 生成序号列
来源：http://3g.hesvh.cn/Article/details/gkyaanjci.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.zdbjq.cn/Article/details/gqogfwfgg.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gbrcjqtxp.sHtML

R. Bash 专题
来源：http://blog.hesvh.cn/Article/details/gejwxohpa.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/ggwmrxwkk.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fehbvm.com/Article/details/gbbuzercw.sHtML

#!/usr/bin/env bash
来源：http://blog.zdbjq.cn/Article/details/gbrjiclar.sHtML

set -euo pipefail
来源：http://read.share.zdbjq.cn/Article/details/gyloxnlmo.sHtML

[R02] 变量赋值与使用
来源：http://baike.zdbjq.cn/Article/details/gsmphkxeg.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fehbvm.com/Article/details/gfzhijkrb.sHtML

[R03] 只读变量
来源：http://read.share.fehbvm.com/Article/details/gknipjdpm.sHtML

readonly PI=3.14
来源：http://baike.fehbvm.com/Article/details/gkqcrwzex.sHtML

[R04] 位置参数
来源：http://wap.fehbvm.com/Article/details/gjixnjtry.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.hesvh.cn/Article/details/gzhyzcskf.sHtML

[R05] 参数默认值
来源：http://www.m.share.zdbjq.cn/Article/details/geisffsbg.sHtML

name="${1:-default}"
来源：http://baike.zdbjq.cn/Article/details/govowbwsj.sHtML

[R06] 判断命令是否存在
来源：http://www.share.zdbjq.cn/Article/details/gxbentycs.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.hesvh.cn/Article/details/gwzcxfscm.sHtML

[R07] if 判断文件
来源：http://3g.hesvh.cn/Article/details/gcdkyyofg.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.zdbjq.cn/Article/details/gavylxdbl.sHtML

[R08] 数值比较
来源：http://m.share.fehbvm.com/Article/details/gfctnrbbx.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.zdbjq.cn/Article/details/ghibygrcd.sHtML

[R09] 字符串比较
来源：http://read.share.zdbjq.cn/Article/details/gqyvvquwd.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gsrikfziv.sHtML

[R10] 正则匹配
来源：http://www.blog.hesvh.cn/Article/details/glbtladrg.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fehbvm.com/Article/details/gvdjlxddo.sHtML

[R11] case 多分支
来源：http://read.share.hesvh.cn/Article/details/gzxjkadyg.sHtML

case "$1" in
来源：http://wap.zdbjq.cn/Article/details/geluljyge.sHtML

start) echo "启动" ;;
来源：http://www.blog.fehbvm.com/Article/details/gutmmlsjh.sHtML

stop)  echo "停止" ;;
来源：http://3g.zdbjq.cn/Article/details/gqbzbmisv.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fehbvm.com/Article/details/gfkzjzzoy.sHtML

esac
来源：http://wap.fehbvm.com/Article/details/gkbmlmozq.sHtML

[R12] for 遍历文件
来源：http://3g.zdbjq.cn/Article/details/ggvkwvnob.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fehbvm.com/Article/details/gdwqrrone.sHtML

[R13] for 计数循环
来源：http://wap.zdbjq.cn/Article/details/gppnxrjjw.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.zdbjq.cn/Article/details/gaupdgmhw.sHtML

[R14] C 风格 for
来源：http://www.share.zdbjq.cn/Article/details/gwhafoplr.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/gwbcsnumn.sHtML

[R15] while 逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gubzcosmw.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.hesvh.cn/Article/details/gznpcjaqp.sHtML

[R16] until 等待条件
来源：http://wap.hesvh.cn/Article/details/gcrgdvswn.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.hesvh.cn/Article/details/gldsieuxx.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fehbvm.com/Article/details/gdocuxpwy.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.zdbjq.cn/Article/details/gugwrshlp.sHtML

[R18] 遍历数组
来源：http://read.share.hesvh.cn/Article/details/gbylffidb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.hesvh.cn/Article/details/gvgnygjlv.sHtML

[R19] 数组长度
来源：http://www.m.share.hesvh.cn/Article/details/gtnxbxdml.sHtML

echo "${#arr[@]}"
来源：http://3g.fehbvm.com/Article/details/ggnrzxvcx.sHtML

[R20] 关联数组（字典）
来源：http://www.share.hesvh.cn/Article/details/gkqgkboos.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fehbvm.com/Article/details/ggcuwfaqw.sHtML

[R21] 字符串长度
来源：http://mobile.zdbjq.cn/Article/details/grlzppdgj.sHtML

echo "${#s}"
来源：http://wap.zdbjq.cn/Article/details/grnogytva.sHtML

[R22] 截取子串
来源：http://www.m.share.fehbvm.com/Article/details/gglhsycqv.sHtML

echo "${s:0:5}"
来源：http://wap.hesvh.cn/Article/details/ggppexgpp.sHtML

[R23] 字符串替换
来源：http://www.m.share.fehbvm.com/Article/details/gzrnyvmiz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.zdbjq.cn/Article/details/gxheqxvtl.sHtML

[R24] 大小写转换
来源：http://3g.zdbjq.cn/Article/details/gkpqhruea.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fehbvm.com/Article/details/gbuzwpttu.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.zdbjq.cn/Article/details/gwknvgvyn.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fehbvm.com/Article/details/giskwlwar.sHtML

[R26] 命令替换
来源：http://baike.fehbvm.com/Article/details/gxkpemssd.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.hesvh.cn/Article/details/gexeswkbo.sHtML

[R27] 算术展开
来源：http://blog.hesvh.cn/Article/details/gnwyvigdw.sHtML

echo $((1 + 2 * 3))
来源：http://baike.hesvh.cn/Article/details/gjnpqadwn.sHtML

[R28] 浮点运算
来源：http://wap.hesvh.cn/Article/details/gtgmlnxxr.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.hesvh.cn/Article/details/gytpatdvn.sHtML

[R29] 定义函数
来源：http://www.blog.zdbjq.cn/Article/details/gplmorifn.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.hesvh.cn/Article/details/gymzqgwjs.sHtML

[R30] 函数返回状态码
来源：http://www.share.hesvh.cn/Article/details/gbwkgsoxg.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.zdbjq.cn/Article/details/gindqwgoe.sHtML

[R31] 局部变量
来源：http://mobile.hesvh.cn/Article/details/gznavbrfz.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fehbvm.com/Article/details/gcuueohad.sHtML

[R32] 参数个数校验
来源：http://blog.hesvh.cn/Article/details/gqtdhiwoi.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fehbvm.com/Article/details/gfevcjftn.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fehbvm.com/Article/details/gwibnzqpy.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.zdbjq.cn/Article/details/gsuhgvfmb.sHtML

[R34] 退出时清理
来源：http://read.share.zdbjq.cn/Article/details/gugpwbgeo.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fehbvm.com/Article/details/gnfqnxhlq.sHtML

[R35] 后台执行并等待
来源：http://m.share.zdbjq.cn/Article/details/gzwohlhrv.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.hesvh.cn/Article/details/gcngmbfsy.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.zdbjq.cn/Article/details/gwioeplvn.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.hesvh.cn/Article/details/glwjylefl.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.zdbjq.cn/Article/details/gztzxonsj.sHtML

files=$(ls -1)
来源：http://3g.hesvh.cn/Article/details/gskehoenh.sHtML

[R38] 管道串联
来源：http://www.m.share.fehbvm.com/Article/details/gbfungriy.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fehbvm.com/Article/details/gkdvkdfln.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.hesvh.cn/Article/details/gllksjzdy.sHtML

cmd > out.log 2>&1
来源：http://m.share.hesvh.cn/Article/details/gdxyaeerj.sHtML

[R40] 追加写日志
来源：http://baike.fehbvm.com/Article/details/gpnvtqobg.sHtML

echo "log" >> out.log
来源：http://blog.hesvh.cn/Article/details/gmxhocfuk.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fehbvm.com/Article/details/gftdffhhp.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.hesvh.cn/Article/details/gbnzdjetx.sHtML

[R42] 输入重定向
来源：http://baike.fehbvm.com/Article/details/gggrazkor.sHtML

wc -l < a.txt
来源：http://baike.hesvh.cn/Article/details/geygdncfk.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fehbvm.com/Article/details/gkwyikmvv.sHtML

find . -name "*.log" -type f
来源：http://wap.hesvh.cn/Article/details/gsvkzaznh.sHtML

[R44] 按修改时间查找
来源：http://m.share.fehbvm.com/Article/details/gcvjkhrbj.sHtML

find . -mtime -7 -type f
来源：http://blog.fehbvm.com/Article/details/gdnzthcvo.sHtML

[R45] 批量删除
来源：http://mobile.fehbvm.com/Article/details/gxoepzvvr.sHtML

find . -name "*.tmp" -delete
来源：http://3g.hesvh.cn/Article/details/gspfdwpyf.sHtML

[R46] 递归替换文件内容
来源：http://3g.fehbvm.com/Article/details/gdsatzoty.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.zdbjq.cn/Article/details/gyjnckmyk.sHtML

[R47] sed 单行替换
来源：http://wap.hesvh.cn/Article/details/gvuatxxns.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gatavvlrp.sHtML

[R48] awk 取指定列
来源：http://read.share.zdbjq.cn/Article/details/gfmmzjuaa.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.zdbjq.cn/Article/details/gcseunecj.sHtML

[R49] awk 带条件
来源：http://www.m.share.zdbjq.cn/Article/details/gsowftjkm.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.hesvh.cn/Article/details/gygogtmog.sHtML

[R50] awk 求和
来源：http://read.share.hesvh.cn/Article/details/gmsrdllmj.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fehbvm.com/Article/details/gbxkihzbt.sHtML

[R51] 排序去重取前几
来源：http://mobile.fehbvm.com/Article/details/gvzwcyyao.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fehbvm.com/Article/details/gdehnzvhn.sHtML

[R52] 统计行数
来源：http://www.share.zdbjq.cn/Article/details/gtdnzdjbw.sHtML

wc -l a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gixfsgnah.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.zdbjq.cn/Article/details/gqzdzwzhq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fehbvm.com/Article/details/gjiauppzz.sHtML

[R54] 比较两个文件
来源：http://wap.zdbjq.cn/Article/details/gasdtfcmv.sHtML

diff a.txt b.txt
来源：http://www.share.hesvh.cn/Article/details/goeayogic.sHtML

[R55] 压缩与解压
来源：http://www.share.hesvh.cn/Article/details/gwqyijatc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fehbvm.com/Article/details/geqdgclzx.sHtML

[R56] 远程拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gbmziwqqg.sHtML

scp file user@host:/path/
来源：http://baike.zdbjq.cn/Article/details/gqgcappsr.sHtML

[R57] 远程执行命令
来源：http://m.share.zdbjq.cn/Article/details/gbximjskg.sHtML

ssh user@host 'uptime'
来源：http://3g.zdbjq.cn/Article/details/gzkgvychx.sHtML

[R58] 下载文件
来源：http://www.m.share.fehbvm.com/Article/details/gpzngrucc.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.hesvh.cn/Article/details/gxbntilab.sHtML

[R59] 发 POST JSON
来源：http://www.blog.hesvh.cn/Article/details/grdxudijg.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fehbvm.com/Article/details/grmgshmda.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fehbvm.com/Article/details/gsyitgtus.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.hesvh.cn/Article/details/gcqepcmmi.sHtML

[R61] 磁盘占用
来源：http://read.share.hesvh.cn/Article/details/gcectgghm.sHtML

df -h;  du -sh *
来源：http://3g.hesvh.cn/Article/details/gmcgzbfbc.sHtML

[R62] 找最占空间的文件
来源：http://baike.zdbjq.cn/Article/details/ggygpvkcg.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.zdbjq.cn/Article/details/gsgxlxpqi.sHtML

[R63] 内存与进程
来源：http://wap.zdbjq.cn/Article/details/gqzicmuyw.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.zdbjq.cn/Article/details/gynwjgeco.sHtML

[R64] 结束进程
来源：http://baike.zdbjq.cn/Article/details/gdtttmvmq.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fehbvm.com/Article/details/gxacldxvc.sHtML

[R65] 查看端口占用
来源：http://www.blog.fehbvm.com/Article/details/gxjvktvwg.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.hesvh.cn/Article/details/ggduqrech.sHtML

[R66] 定时任务
来源：http://baike.fehbvm.com/Article/details/gtyuhvnft.sHtML

crontab -e;  crontab -l
来源：http://3g.hesvh.cn/Article/details/gskfxqmku.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fehbvm.com/Article/details/gmnlollho.sHtML


<!-- 参考信息 -->