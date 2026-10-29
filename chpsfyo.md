代发 wailian999

SELECT * FROM users;
来源：http://3g.zdbjq.cn/Article/details/gzppebjsa.sHtML

[Q16] 查询指定列
来源：http://mobile.hesvh.cn/Article/details/gczkysgmg.sHtML

SELECT id, name FROM users;
来源：http://www.share.fehbvm.com/Article/details/gjnbhrzal.sHtML

[Q17] 条件查询
来源：http://baike.hesvh.cn/Article/details/ggmpxheut.sHtML

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.share.fehbvm.com/Article/details/gdyrovrap.sHtML

[Q18] 模糊匹配
来源：http://read.share.hesvh.cn/Article/details/gnvhsfjre.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.m.share.hesvh.cn/Article/details/grrljayeg.sHtML

[Q19] 范围查询
来源：http://mobile.hesvh.cn/Article/details/gnjncsspk.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.zdbjq.cn/Article/details/gcarxudmx.sHtML

[Q20] IN 列表
来源：http://read.share.zdbjq.cn/Article/details/giwlhmgpp.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.blog.fehbvm.com/Article/details/gqydcqauz.sHtML

[Q21] 空值判断
来源：http://3g.hesvh.cn/Article/details/gbhzqrlnm.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.fehbvm.com/Article/details/gywoscxol.sHtML

[Q22] 排序
来源：http://blog.fehbvm.com/Article/details/gmlahuoku.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.zdbjq.cn/Article/details/ghbnsdkfc.sHtML

[Q23] 分页
来源：http://wap.zdbjq.cn/Article/details/gfetmpbck.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.zdbjq.cn/Article/details/gvnuyjeuh.sHtML

[Q24] 去重
来源：http://mobile.zdbjq.cn/Article/details/grwxkfygv.sHtML

SELECT DISTINCT city FROM users;
来源：http://3g.hesvh.cn/Article/details/gtqzmoohx.sHtML

[Q25] 只取前 N 条
来源：http://read.share.zdbjq.cn/Article/details/garlxtnor.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.hesvh.cn/Article/details/gorkzxeil.sHtML

[Q26] 计数
来源：http://m.share.hesvh.cn/Article/details/gmuwiiewp.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/grdtnpybf.sHtML

[Q27] 条件计数
来源：http://baike.zdbjq.cn/Article/details/ggeobhsld.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gxyvzhsfi.sHtML

[Q28] 求和与平均
来源：http://m.share.zdbjq.cn/Article/details/gekwcumnx.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/grgnlmjtq.sHtML

[Q29] 最大最小值
来源：http://baike.hesvh.cn/Article/details/guzwiwzsu.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.zdbjq.cn/Article/details/goahulyge.sHtML

[Q30] 分组统计
来源：http://blog.zdbjq.cn/Article/details/gnppnlvuy.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/gfzqletsv.sHtML

[Q31] 分组后过滤
来源：http://3g.zdbjq.cn/Article/details/ggxkymlee.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.zdbjq.cn/Article/details/ghdfmogfq.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.fehbvm.com/Article/details/glickiqqy.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gyvcvimis.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.zdbjq.cn/Article/details/gkahzaeyy.sHtML

[Q33] 多列分组
来源：http://m.share.fehbvm.com/Article/details/gsorohnak.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.hesvh.cn/Article/details/geebfrsyw.sHtML

[Q34] 每组取第一条
来源：http://wap.hesvh.cn/Article/details/gaflpqbqt.sHtML

SELECT * FROM (
来源：http://wap.zdbjq.cn/Article/details/gqtjdjxgh.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.fehbvm.com/Article/details/gdzjdsnet.sHtML

) t WHERE rn = 1;
来源：http://www.blog.hesvh.cn/Article/details/gveuucpea.sHtML

[Q35] 内连接
来源：http://www.m.share.fehbvm.com/Article/details/gaonyrsrx.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.fehbvm.com/Article/details/gefklenud.sHtML

[Q36] 左连接
来源：http://wap.hesvh.cn/Article/details/gzxrdyudr.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.fehbvm.com/Article/details/gipvjhnsa.sHtML

[Q37] 右连接
来源：http://read.share.fehbvm.com/Article/details/gqrxknwge.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.zdbjq.cn/Article/details/ggnzurfyg.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.hesvh.cn/Article/details/gvkcmnnfs.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.hesvh.cn/Article/details/gipupqlcz.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.hesvh.cn/Article/details/gzjdlmnho.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.fehbvm.com/Article/details/gvszecdjk.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.hesvh.cn/Article/details/gmpsgixve.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.hesvh.cn/Article/details/glmlbluog.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.hesvh.cn/Article/details/grtunyyec.sHtML

[Q41] 多表连接
来源：http://blog.zdbjq.cn/Article/details/gfquayivo.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.zdbjq.cn/Article/details/gpfoilijc.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.zdbjq.cn/Article/details/gcuphbbck.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.zdbjq.cn/Article/details/gpzfjbhys.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.zdbjq.cn/Article/details/gpucfysxn.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.zdbjq.cn/Article/details/grjkobhtd.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.hesvh.cn/Article/details/gttxdlhnp.sHtML

[Q43] 标量子查询
来源：http://m.share.fehbvm.com/Article/details/gcxljbqds.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.hesvh.cn/Article/details/grakbnare.sHtML

[Q44] IN 子查询
来源：http://www.m.share.fehbvm.com/Article/details/gequklhgw.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.fehbvm.com/Article/details/giqrcdchy.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.zdbjq.cn/Article/details/gmafscrjq.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fehbvm.com/Article/details/glghxgrxe.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.hesvh.cn/Article/details/gcqzvpahw.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.hesvh.cn/Article/details/gjijjccsv.sHtML

[Q47] 与平均值比较
来源：http://blog.zdbjq.cn/Article/details/ggnoalxcx.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.fehbvm.com/Article/details/ghhfaeyyh.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.zdbjq.cn/Article/details/gigekoznn.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.hesvh.cn/Article/details/ghkszovbz.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.hesvh.cn/Article/details/gowslrpyd.sHtML

[Q49] 更新单行
来源：http://m.share.fehbvm.com/Article/details/gxzhdgzoj.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gheepahgv.sHtML

[Q50] 批量更新
来源：http://www.m.share.fehbvm.com/Article/details/gpubrcrwt.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.hesvh.cn/Article/details/gepknczyu.sHtML

[Q51] 用子查询更新
来源：http://wap.zdbjq.cn/Article/details/guwhljppq.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.fehbvm.com/Article/details/gpeatqgok.sHtML

[Q52] 删除指定行
来源：http://blog.zdbjq.cn/Article/details/gpjewgeqp.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.fehbvm.com/Article/details/giwolrhhp.sHtML

[Q53] 按条件删除
来源：http://mobile.zdbjq.cn/Article/details/ggfmjlsbp.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.hesvh.cn/Article/details/gfszddcdq.sHtML

[Q54] 清空表
来源：http://www.m.share.zdbjq.cn/Article/details/gwczjjzwe.sHtML

TRUNCATE TABLE logs;
来源：http://3g.hesvh.cn/Article/details/gtzviusfh.sHtML

[Q55] 排名（并列占位）
来源：http://3g.zdbjq.cn/Article/details/gxrukfigw.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.zdbjq.cn/Article/details/gicdkefqd.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.fehbvm.com/Article/details/gundrltll.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.fehbvm.com/Article/details/gkjbneiaf.sHtML

[Q57] 行号
来源：http://mobile.fehbvm.com/Article/details/gaejalfml.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.fehbvm.com/Article/details/glignznjy.sHtML

[Q58] 累计求和
来源：http://www.blog.fehbvm.com/Article/details/gjyiwxekw.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.fehbvm.com/Article/details/guovlfyfc.sHtML

[Q59] 分组内累计
来源：http://wap.zdbjq.cn/Article/details/ghbulndga.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gmjdxhpsb.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.hesvh.cn/Article/details/gaisxcmvb.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.hesvh.cn/Article/details/gqxjaocwt.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/ggqklhfuv.sHtML

[Q61] 移动平均
来源：http://mobile.fehbvm.com/Article/details/gfwxjudrh.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gozawpmxy.sHtML

[Q62] 分组占比
来源：http://www.blog.zdbjq.cn/Article/details/grffvjnry.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gjwcgrrop.sHtML

[Q63] 开启事务
来源：http://www.blog.hesvh.cn/Article/details/grxlhftcc.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.zdbjq.cn/Article/details/ghtoepcgd.sHtML

[Q64] 提交事务
来源：http://www.share.zdbjq.cn/Article/details/ghkospreo.sHtML

COMMIT;
来源：http://wap.hesvh.cn/Article/details/gpigazpjl.sHtML

[Q65] 回滚事务
来源：http://3g.hesvh.cn/Article/details/gvzcdgtai.sHtML

ROLLBACK;
来源：http://blog.zdbjq.cn/Article/details/gveniwwuu.sHtML

[Q66] 行锁查询
来源：http://www.share.hesvh.cn/Article/details/gxaeqjafv.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.hesvh.cn/Article/details/gcnbvvifh.sHtML

[Q67] 设置隔离级别
来源：http://baike.fehbvm.com/Article/details/gyafdvosk.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.hesvh.cn/Article/details/gcistzlbl.sHtML

[Q68] 保存点
来源：http://baike.hesvh.cn/Article/details/gslajflei.sHtML

SAVEPOINT sp1;
来源：http://www.share.zdbjq.cn/Article/details/gwxohkgmu.sHtML

ROLLBACK TO sp1;
来源：http://www.share.hesvh.cn/Article/details/gzdnhysdl.sHtML

[Q69] 查看执行计划
来源：http://mobile.hesvh.cn/Article/details/gtzfwcqzt.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.hesvh.cn/Article/details/gpitzpsbb.sHtML

[Q70] 更新统计信息
来源：http://www.share.hesvh.cn/Article/details/gpklrajxz.sHtML

ANALYZE TABLE users;
来源：http://www.blog.hesvh.cn/Article/details/gemgmsxkt.sHtML

[Q71] 查看建表语句
来源：http://baike.hesvh.cn/Article/details/gpfugzjct.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.hesvh.cn/Article/details/gpsdksqou.sHtML

[Q72] 查看索引
来源：http://m.share.hesvh.cn/Article/details/gfgwunmjh.sHtML

SHOW INDEX FROM users;
来源：http://baike.zdbjq.cn/Article/details/gjbihfddt.sHtML

[Q73] 查看表状态
来源：http://blog.fehbvm.com/Article/details/gnzuglssy.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.hesvh.cn/Article/details/gclglutdg.sHtML

[Q74] 强制使用索引
来源：http://mobile.zdbjq.cn/Article/details/gjkffbawk.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.hesvh.cn/Article/details/ghdlysswf.sHtML

[Q75] 日期格式化
来源：http://mobile.zdbjq.cn/Article/details/gdrwucqam.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gfhjfhaqt.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.zdbjq.cn/Article/details/grsxpuzhr.sHtML

[Q76] 按天统计
来源：http://mobile.fehbvm.com/Article/details/gylvwfbsg.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.hesvh.cn/Article/details/geakvlhpv.sHtML

[Q77] 时间加减
来源：http://mobile.hesvh.cn/Article/details/gpxjprnpn.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.hesvh.cn/Article/details/gakpoexca.sHtML

[Q78] 当前时间
来源：http://m.share.fehbvm.com/Article/details/gehlzrotw.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.fehbvm.com/Article/details/grelyaxht.sHtML

[Q79] 字符串拼接
来源：http://www.share.zdbjq.cn/Article/details/gntgsgmva.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fehbvm.com/Article/details/gnmqxqers.sHtML

[Q80] 字符串截取
来源：http://m.share.hesvh.cn/Article/details/gdpwnaihh.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gyaqvagmw.sHtML

[Q81] 字符串替换
来源：http://www.m.share.fehbvm.com/Article/details/gavjmgnrv.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.fehbvm.com/Article/details/gmvxnkyxn.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.hesvh.cn/Article/details/gwkgvskph.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gpvrzgmiy.sHtML

[Q83] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/gzzpywctk.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gddkisahf.sHtML

[Q84] 去除首尾空格
来源：http://baike.zdbjq.cn/Article/details/gnursxrtf.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/ginhrptcx.sHtML

[Q85] 数值取整
来源：http://www.m.share.zdbjq.cn/Article/details/gvzdgudyq.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.hesvh.cn/Article/details/gcdxuyeoi.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.zdbjq.cn/Article/details/gcdlggolq.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.hesvh.cn/Article/details/grqteewde.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.zdbjq.cn/Article/details/gtdasrdht.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.hesvh.cn/Article/details/gsjkwnpfm.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.hesvh.cn/Article/details/gqihzroti.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.fehbvm.com/Article/details/gbaaeyejc.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gsjsfcosv.sHtML

[Q89] 判断表是否存在
来源：http://wap.zdbjq.cn/Article/details/gwgyopgjj.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.hesvh.cn/Article/details/ghovpdxhc.sHtML

[Q90] 生成序号列
来源：http://www.blog.zdbjq.cn/Article/details/gqdinxohg.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.zdbjq.cn/Article/details/gmxocutaj.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gkcgkrflm.sHtML

R. Bash 专题
来源：http://3g.hesvh.cn/Article/details/gwrgcgkmt.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gmltqnpgi.sHtML

[R01] shebang 与严格模式
来源：http://3g.zdbjq.cn/Article/details/gqybmizsa.sHtML

#!/usr/bin/env bash
来源：http://mobile.zdbjq.cn/Article/details/gganbtjre.sHtML

set -euo pipefail
来源：http://blog.fehbvm.com/Article/details/gkywmesyj.sHtML

[R02] 变量赋值与使用
来源：http://blog.fehbvm.com/Article/details/grzlerzai.sHtML

name="Tom"; echo "$name"
来源：http://read.share.zdbjq.cn/Article/details/gbrgldyxh.sHtML

[R03] 只读变量
来源：http://www.share.zdbjq.cn/Article/details/gywnpexfb.sHtML

readonly PI=3.14
来源：http://3g.hesvh.cn/Article/details/gnnofnkbp.sHtML

[R04] 位置参数
来源：http://www.m.share.hesvh.cn/Article/details/ghyejpgkq.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.zdbjq.cn/Article/details/gndvwahoo.sHtML

[R05] 参数默认值
来源：http://www.share.zdbjq.cn/Article/details/grsgjpqyk.sHtML

name="${1:-default}"
来源：http://blog.fehbvm.com/Article/details/gfirexnlc.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gofudyngg.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fehbvm.com/Article/details/gwbjncewb.sHtML

[R07] if 判断文件
来源：http://mobile.hesvh.cn/Article/details/gdhakbfdq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fehbvm.com/Article/details/gitevmaww.sHtML

[R08] 数值比较
来源：http://www.blog.fehbvm.com/Article/details/gfadtpiyd.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fehbvm.com/Article/details/gwiuzwuug.sHtML

[R09] 字符串比较
来源：http://mobile.zdbjq.cn/Article/details/gpaonerju.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fehbvm.com/Article/details/gcxcmjftw.sHtML

[R10] 正则匹配
来源：http://read.share.hesvh.cn/Article/details/gxtggbqdc.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.zdbjq.cn/Article/details/gmgpyyths.sHtML

[R11] case 多分支
来源：http://wap.hesvh.cn/Article/details/gmtchhqjb.sHtML

case "$1" in
来源：http://blog.zdbjq.cn/Article/details/gvymabunm.sHtML

start) echo "启动" ;;
来源：http://wap.fehbvm.com/Article/details/glpnbcnsc.sHtML

stop)  echo "停止" ;;
来源：http://mobile.zdbjq.cn/Article/details/gpitfqdik.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fehbvm.com/Article/details/gnjpzrpzd.sHtML

esac
来源：http://www.share.fehbvm.com/Article/details/gfgayycfo.sHtML

[R12] for 遍历文件
来源：http://wap.zdbjq.cn/Article/details/ghmzhgjfi.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fehbvm.com/Article/details/gnrhafyaw.sHtML

[R13] for 计数循环
来源：http://www.blog.fehbvm.com/Article/details/grjlccaxt.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gbwlljlwv.sHtML

[R14] C 风格 for
来源：http://3g.hesvh.cn/Article/details/geoswsssh.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.zdbjq.cn/Article/details/gdyofhexs.sHtML

[R15] while 逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gkiacyovo.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fehbvm.com/Article/details/grgcryybi.sHtML

[R16] until 等待条件
来源：http://m.share.fehbvm.com/Article/details/gkhvrlymp.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fehbvm.com/Article/details/gosfekvrt.sHtML

[R17] 数组定义与取值
来源：http://mobile.fehbvm.com/Article/details/gwabkzvjj.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.hesvh.cn/Article/details/guebnrgig.sHtML

[R18] 遍历数组
来源：http://blog.zdbjq.cn/Article/details/gbwikdign.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.zdbjq.cn/Article/details/gwgowwuao.sHtML

[R19] 数组长度
来源：http://read.share.hesvh.cn/Article/details/gpzceoyfh.sHtML

echo "${#arr[@]}"
来源：http://blog.zdbjq.cn/Article/details/giewdcobf.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fehbvm.com/Article/details/gfucyurlc.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.hesvh.cn/Article/details/gydgfspiy.sHtML

[R21] 字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/gypzdjmkn.sHtML

echo "${#s}"
来源：http://m.share.fehbvm.com/Article/details/gpatjutqx.sHtML

[R22] 截取子串
来源：http://blog.fehbvm.com/Article/details/gmxqqmlex.sHtML

echo "${s:0:5}"
来源：http://m.share.fehbvm.com/Article/details/ggkprzsnd.sHtML

[R23] 字符串替换
来源：http://m.share.hesvh.cn/Article/details/glqetqalm.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fehbvm.com/Article/details/gnanmsoyc.sHtML

[R24] 大小写转换
来源：http://m.share.zdbjq.cn/Article/details/gprmmexfe.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fehbvm.com/Article/details/ghosztzmk.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.hesvh.cn/Article/details/gehokcakm.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fehbvm.com/Article/details/gnauhxpll.sHtML

[R26] 命令替换
来源：http://blog.fehbvm.com/Article/details/gyrtsugwx.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fehbvm.com/Article/details/gvukxdqxq.sHtML

[R27] 算术展开
来源：http://blog.fehbvm.com/Article/details/gfrkufvty.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.zdbjq.cn/Article/details/gwuhukbcj.sHtML

[R28] 浮点运算
来源：http://m.share.zdbjq.cn/Article/details/gmmhcsweg.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.zdbjq.cn/Article/details/gaxzdafuy.sHtML

[R29] 定义函数
来源：http://www.share.fehbvm.com/Article/details/gqsqjaqnl.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.hesvh.cn/Article/details/gymxctukn.sHtML

[R30] 函数返回状态码
来源：http://baike.hesvh.cn/Article/details/gwxqnepyw.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.hesvh.cn/Article/details/gzbjbdure.sHtML

[R31] 局部变量
来源：http://wap.fehbvm.com/Article/details/gtlphpedj.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.hesvh.cn/Article/details/gltunjamf.sHtML

[R32] 参数个数校验
来源：http://m.share.fehbvm.com/Article/details/gngwtalqc.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.zdbjq.cn/Article/details/gopdmbexf.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fehbvm.com/Article/details/gvwqhjvom.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fehbvm.com/Article/details/gpwfdnbpx.sHtML

[R34] 退出时清理
来源：http://www.m.share.hesvh.cn/Article/details/glscgbfob.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.hesvh.cn/Article/details/gmpygqpuq.sHtML

[R35] 后台执行并等待
来源：http://baike.fehbvm.com/Article/details/gszfgeszc.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fehbvm.com/Article/details/gnuemvitz.sHtML

[R36] 并发执行多个任务
来源：http://mobile.zdbjq.cn/Article/details/ghwdxofdu.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fehbvm.com/Article/details/goxuarcau.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.zdbjq.cn/Article/details/gtefbnkeo.sHtML

files=$(ls -1)
来源：http://www.m.share.zdbjq.cn/Article/details/gepmyczfu.sHtML

[R38] 管道串联
来源：http://wap.zdbjq.cn/Article/details/gydmwzzbw.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.hesvh.cn/Article/details/gtjbwjyuv.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fehbvm.com/Article/details/gkkdbkkvn.sHtML

cmd > out.log 2>&1
来源：http://www.blog.zdbjq.cn/Article/details/guexixcmt.sHtML

[R40] 追加写日志
来源：http://m.share.hesvh.cn/Article/details/gigbayrjd.sHtML

echo "log" >> out.log
来源：http://baike.hesvh.cn/Article/details/gdhdgufrf.sHtML

[R41] 丢弃输出
来源：http://read.share.fehbvm.com/Article/details/goejgurvg.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fehbvm.com/Article/details/gdumfvuws.sHtML

[R42] 输入重定向
来源：http://wap.hesvh.cn/Article/details/gjcfwugdp.sHtML

wc -l < a.txt
来源：http://blog.zdbjq.cn/Article/details/gyjjmcphn.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.zdbjq.cn/Article/details/ghsmusfsp.sHtML

find . -name "*.log" -type f
来源：http://www.blog.zdbjq.cn/Article/details/gakbbvqed.sHtML

[R44] 按修改时间查找
来源：http://read.share.hesvh.cn/Article/details/guhlvkzzz.sHtML

find . -mtime -7 -type f
来源：http://www.share.hesvh.cn/Article/details/grsgsblkw.sHtML

[R45] 批量删除
来源：http://3g.hesvh.cn/Article/details/gpmfculai.sHtML

find . -name "*.tmp" -delete
来源：http://wap.zdbjq.cn/Article/details/grhmvmmqu.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.hesvh.cn/Article/details/gjteapsfq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fehbvm.com/Article/details/gpmzlyggl.sHtML

[R47] sed 单行替换
来源：http://3g.zdbjq.cn/Article/details/ghcjpeyzk.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gshzqrgpc.sHtML

[R48] awk 取指定列
来源：http://www.blog.zdbjq.cn/Article/details/gkwpnyols.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.zdbjq.cn/Article/details/gfeifvbyb.sHtML

[R49] awk 带条件
来源：http://read.share.fehbvm.com/Article/details/ggdtlvtfv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.hesvh.cn/Article/details/gmshddyzy.sHtML

[R50] awk 求和
来源：http://3g.fehbvm.com/Article/details/gadfcspij.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.hesvh.cn/Article/details/goddxsqvs.sHtML

[R51] 排序去重取前几
来源：http://read.share.hesvh.cn/Article/details/gmafktwll.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.zdbjq.cn/Article/details/gthoaeasy.sHtML

[R52] 统计行数
来源：http://wap.hesvh.cn/Article/details/gbklthcus.sHtML

wc -l a.txt
来源：http://www.blog.hesvh.cn/Article/details/gacihgvxt.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.hesvh.cn/Article/details/gibpxdusw.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.zdbjq.cn/Article/details/glctxspps.sHtML

[R54] 比较两个文件
来源：http://3g.hesvh.cn/Article/details/gwqdtnqtb.sHtML

diff a.txt b.txt
来源：http://3g.zdbjq.cn/Article/details/gywdptjmh.sHtML

[R55] 压缩与解压
来源：http://read.share.fehbvm.com/Article/details/gllxnaczo.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.hesvh.cn/Article/details/gofpbtqom.sHtML

[R56] 远程拷贝
来源：http://blog.fehbvm.com/Article/details/gcifapbop.sHtML

scp file user@host:/path/
来源：http://baike.zdbjq.cn/Article/details/gsgtggdgz.sHtML

[R57] 远程执行命令
来源：http://www.share.zdbjq.cn/Article/details/gpsnnsglt.sHtML

ssh user@host 'uptime'
来源：http://read.share.zdbjq.cn/Article/details/gchxuhogm.sHtML

[R58] 下载文件
来源：http://www.m.share.fehbvm.com/Article/details/gohdabflr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.zdbjq.cn/Article/details/gthxcefsd.sHtML

[R59] 发 POST JSON
来源：http://mobile.hesvh.cn/Article/details/giyucrucw.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.hesvh.cn/Article/details/gruubufxf.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.hesvh.cn/Article/details/gmxxujnmc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.hesvh.cn/Article/details/gnmpqdaew.sHtML

[R61] 磁盘占用
来源：http://www.share.fehbvm.com/Article/details/gncogwjva.sHtML

df -h;  du -sh *
来源：http://read.share.zdbjq.cn/Article/details/gwigecbhk.sHtML

[R62] 找最占空间的文件
来源：http://3g.zdbjq.cn/Article/details/gvqohnerk.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.hesvh.cn/Article/details/gyzzplrzj.sHtML

[R63] 内存与进程
来源：http://www.blog.zdbjq.cn/Article/details/gvaespcrl.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fehbvm.com/Article/details/gqeskkugp.sHtML

[R64] 结束进程
来源：http://read.share.zdbjq.cn/Article/details/gkvmyecww.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.hesvh.cn/Article/details/gtladaofs.sHtML

[R65] 查看端口占用
来源：http://www.share.zdbjq.cn/Article/details/gilyulgsh.sHtML


<!-- 参考信息 -->