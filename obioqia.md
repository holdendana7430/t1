代发 wailian999

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://mobile.zdbjq.cn/Article/details/gxddmsnan.sHtML

[Q18] 模糊匹配
来源：http://www.blog.fehbvm.com/Article/details/gtvzsakca.sHtML

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.share.fehbvm.com/Article/details/glztyedxc.sHtML

[Q19] 范围查询
来源：http://blog.hesvh.cn/Article/details/giugqpukd.sHtML

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://blog.hesvh.cn/Article/details/ggskertli.sHtML

[Q20] IN 列表
来源：http://3g.zdbjq.cn/Article/details/gfwpuoara.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://wap.hesvh.cn/Article/details/geffmrywf.sHtML

[Q21] 空值判断
来源：http://3g.zdbjq.cn/Article/details/guapddbqb.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.zdbjq.cn/Article/details/gzermbwxz.sHtML

[Q22] 排序
来源：http://3g.zdbjq.cn/Article/details/gzmlkswxi.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://blog.zdbjq.cn/Article/details/grxpurofj.sHtML

[Q23] 分页
来源：http://blog.zdbjq.cn/Article/details/gkhjdfdkp.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.zdbjq.cn/Article/details/gjflqyyiy.sHtML

[Q24] 去重
来源：http://3g.hesvh.cn/Article/details/gmwkavbqx.sHtML

SELECT DISTINCT city FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gmdqjfgio.sHtML

[Q25] 只取前 N 条
来源：http://blog.hesvh.cn/Article/details/gxfdfijcl.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.zdbjq.cn/Article/details/ghktwmgrl.sHtML

[Q26] 计数
来源：http://blog.zdbjq.cn/Article/details/gqnyxawxs.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.hesvh.cn/Article/details/gjazmagly.sHtML

[Q27] 条件计数
来源：http://www.blog.zdbjq.cn/Article/details/gvgfenhnk.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gdyrmbuvk.sHtML

[Q28] 求和与平均
来源：http://blog.fehbvm.com/Article/details/gzalsvhfl.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gegwhgruc.sHtML

[Q29] 最大最小值
来源：http://3g.hesvh.cn/Article/details/gwprbllbh.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gcccoazuz.sHtML

[Q30] 分组统计
来源：http://www.share.fehbvm.com/Article/details/gqazidwbo.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/govhkkjay.sHtML

[Q31] 分组后过滤
来源：http://m.share.fehbvm.com/Article/details/guakbolhe.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.hesvh.cn/Article/details/glxgiungd.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.zdbjq.cn/Article/details/gbmlrqscg.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/gpanlhmua.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.hesvh.cn/Article/details/gdmesnvni.sHtML

[Q33] 多列分组
来源：http://read.share.hesvh.cn/Article/details/goltldnxi.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.hesvh.cn/Article/details/gxyqddkpi.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.zdbjq.cn/Article/details/gmpntjzjd.sHtML

SELECT * FROM (
来源：http://www.m.share.zdbjq.cn/Article/details/gdwnimpng.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.zdbjq.cn/Article/details/glbfjmaoq.sHtML

) t WHERE rn = 1;
来源：http://3g.zdbjq.cn/Article/details/gtivnkhoq.sHtML

[Q35] 内连接
来源：http://read.share.hesvh.cn/Article/details/glstibixh.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fehbvm.com/Article/details/gvqdupwom.sHtML

[Q36] 左连接
来源：http://wap.hesvh.cn/Article/details/gwslqrnvu.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.hesvh.cn/Article/details/ghtolungx.sHtML

[Q37] 右连接
来源：http://www.m.share.zdbjq.cn/Article/details/gedvyhtsp.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.hesvh.cn/Article/details/gdnfdwaml.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.zdbjq.cn/Article/details/gynallqie.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.hesvh.cn/Article/details/gatfiugmw.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.hesvh.cn/Article/details/getqpyamt.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.hesvh.cn/Article/details/gptzckyuv.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.hesvh.cn/Article/details/gmotpztel.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.fehbvm.com/Article/details/glcozsmwu.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.fehbvm.com/Article/details/gowntpybq.sHtML

[Q41] 多表连接
来源：http://www.m.share.zdbjq.cn/Article/details/galrordpu.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.zdbjq.cn/Article/details/gwwfhrnuk.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.hesvh.cn/Article/details/gfbynanhf.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.hesvh.cn/Article/details/gmgazimca.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.fehbvm.com/Article/details/gfiubwlyb.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.fehbvm.com/Article/details/gchpdslyl.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.zdbjq.cn/Article/details/gvtiymjui.sHtML

[Q43] 标量子查询
来源：http://baike.zdbjq.cn/Article/details/gzxciiyuq.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.hesvh.cn/Article/details/gstvwvznc.sHtML

[Q44] IN 子查询
来源：http://www.share.hesvh.cn/Article/details/gemhamayn.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.fehbvm.com/Article/details/gpbkhlotc.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.zdbjq.cn/Article/details/ggfukphlg.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.zdbjq.cn/Article/details/gfbpirmvt.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.zdbjq.cn/Article/details/gsonjskju.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.hesvh.cn/Article/details/ghkfggkfb.sHtML

[Q47] 与平均值比较
来源：http://www.blog.zdbjq.cn/Article/details/gmaiamxdz.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.zdbjq.cn/Article/details/gjueshjim.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.fehbvm.com/Article/details/gdmcorkul.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.fehbvm.com/Article/details/gafyatyco.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.zdbjq.cn/Article/details/gcuwxwfvu.sHtML

[Q49] 更新单行
来源：http://mobile.fehbvm.com/Article/details/gvvxqjtwi.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.fehbvm.com/Article/details/gloumtsfe.sHtML

[Q50] 批量更新
来源：http://blog.hesvh.cn/Article/details/gddttctgq.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.fehbvm.com/Article/details/ggzczysqt.sHtML

[Q51] 用子查询更新
来源：http://blog.hesvh.cn/Article/details/gafyavwxx.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.zdbjq.cn/Article/details/gdmvyhmev.sHtML

[Q52] 删除指定行
来源：http://www.share.zdbjq.cn/Article/details/gkvsvnjvm.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.zdbjq.cn/Article/details/gdpeenoas.sHtML

[Q53] 按条件删除
来源：http://blog.fehbvm.com/Article/details/garakwjjn.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.zdbjq.cn/Article/details/gwsukhryu.sHtML

[Q54] 清空表
来源：http://read.share.fehbvm.com/Article/details/gcaopkeag.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.zdbjq.cn/Article/details/grthldrjr.sHtML

[Q55] 排名（并列占位）
来源：http://wap.zdbjq.cn/Article/details/gaubozucm.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.fehbvm.com/Article/details/gmrtieqgu.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.fehbvm.com/Article/details/gebuhrmoy.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.zdbjq.cn/Article/details/gtxitoeth.sHtML

[Q57] 行号
来源：http://wap.fehbvm.com/Article/details/guufajmsb.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.hesvh.cn/Article/details/grydjocqo.sHtML

[Q58] 累计求和
来源：http://www.share.zdbjq.cn/Article/details/gkqvstwoq.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.fehbvm.com/Article/details/grftbgmqy.sHtML

[Q59] 分组内累计
来源：http://mobile.hesvh.cn/Article/details/gstxooayr.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gkstvdsgd.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.fehbvm.com/Article/details/gfoorouzy.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.fehbvm.com/Article/details/gqadxktby.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gryrsglhn.sHtML

[Q61] 移动平均
来源：http://wap.fehbvm.com/Article/details/gvhiygygb.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gxuyuxbdr.sHtML

[Q62] 分组占比
来源：http://mobile.fehbvm.com/Article/details/gnpmabgfy.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gltupvbpv.sHtML

[Q63] 开启事务
来源：http://www.m.share.hesvh.cn/Article/details/gziukzeig.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.zdbjq.cn/Article/details/gtdprpspk.sHtML

[Q64] 提交事务
来源：http://m.share.hesvh.cn/Article/details/gybycbeou.sHtML

COMMIT;
来源：http://www.blog.hesvh.cn/Article/details/ggdfaqefm.sHtML

[Q65] 回滚事务
来源：http://baike.fehbvm.com/Article/details/gurijltrg.sHtML

ROLLBACK;
来源：http://m.share.fehbvm.com/Article/details/gplcgkjuz.sHtML

[Q66] 行锁查询
来源：http://wap.fehbvm.com/Article/details/gcismpyhi.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.fehbvm.com/Article/details/grsdlstnk.sHtML

[Q67] 设置隔离级别
来源：http://blog.hesvh.cn/Article/details/gvvlcblkv.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.hesvh.cn/Article/details/ghrjllmur.sHtML

[Q68] 保存点
来源：http://baike.fehbvm.com/Article/details/ghqlzxmbm.sHtML

SAVEPOINT sp1;
来源：http://mobile.hesvh.cn/Article/details/glzgfkgze.sHtML

ROLLBACK TO sp1;
来源：http://baike.zdbjq.cn/Article/details/ghaimgfzu.sHtML

[Q69] 查看执行计划
来源：http://wap.zdbjq.cn/Article/details/grwsrokzr.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.hesvh.cn/Article/details/ghmcizmcc.sHtML

[Q70] 更新统计信息
来源：http://www.blog.hesvh.cn/Article/details/gwoqwmuvh.sHtML

ANALYZE TABLE users;
来源：http://m.share.hesvh.cn/Article/details/gkruxpjkp.sHtML

[Q71] 查看建表语句
来源：http://blog.fehbvm.com/Article/details/goieizozz.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fehbvm.com/Article/details/gohivvour.sHtML

[Q72] 查看索引
来源：http://read.share.fehbvm.com/Article/details/gltzswvdk.sHtML

SHOW INDEX FROM users;
来源：http://3g.fehbvm.com/Article/details/ghcoetmns.sHtML

[Q73] 查看表状态
来源：http://mobile.hesvh.cn/Article/details/ghqapzxsm.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.zdbjq.cn/Article/details/guiahucxu.sHtML

[Q74] 强制使用索引
来源：http://baike.fehbvm.com/Article/details/gstaoxjqs.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.fehbvm.com/Article/details/gcgmjpdzu.sHtML

[Q75] 日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/grgljstpl.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gafrghhbs.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.fehbvm.com/Article/details/gpmvuhuit.sHtML

[Q76] 按天统计
来源：http://m.share.fehbvm.com/Article/details/gmccdvtab.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fehbvm.com/Article/details/givveaqcz.sHtML

[Q77] 时间加减
来源：http://blog.hesvh.cn/Article/details/gozzqurfk.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.fehbvm.com/Article/details/glrlnwwtv.sHtML

[Q78] 当前时间
来源：http://baike.zdbjq.cn/Article/details/gzschiass.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.hesvh.cn/Article/details/gcvmknwan.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.hesvh.cn/Article/details/gnujvlpgw.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fehbvm.com/Article/details/gbkitjvpj.sHtML

[Q80] 字符串截取
来源：http://read.share.fehbvm.com/Article/details/gjxscflrb.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gnbhuyjqz.sHtML

[Q81] 字符串替换
来源：http://3g.fehbvm.com/Article/details/gonsvxhci.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.fehbvm.com/Article/details/gxyaefmiy.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.fehbvm.com/Article/details/gsrsztwho.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/girqlpiij.sHtML

[Q83] 大小写转换
来源：http://blog.hesvh.cn/Article/details/gbetkcfht.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/guzjvcrwz.sHtML

[Q84] 去除首尾空格
来源：http://blog.hesvh.cn/Article/details/giihfrlci.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gsydkbrwj.sHtML

[Q85] 数值取整
来源：http://www.blog.zdbjq.cn/Article/details/gpxegekpj.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.fehbvm.com/Article/details/glbeieskw.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.zdbjq.cn/Article/details/gpzayrqbw.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fehbvm.com/Article/details/gpegmatbb.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.zdbjq.cn/Article/details/gfjtjggtr.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.hesvh.cn/Article/details/gkdvrmfjx.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.zdbjq.cn/Article/details/glatgpxdp.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.zdbjq.cn/Article/details/ghojqmlci.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.hesvh.cn/Article/details/gzrxgiigm.sHtML

[Q89] 判断表是否存在
来源：http://read.share.fehbvm.com/Article/details/gvkyohlib.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.hesvh.cn/Article/details/ghttoqmgv.sHtML

[Q90] 生成序号列
来源：http://www.share.fehbvm.com/Article/details/gzjqxugpm.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.zdbjq.cn/Article/details/gepmmdjsj.sHtML

================================================================================
来源：http://3g.fehbvm.com/Article/details/gkhbqfnzd.sHtML

R. Bash 专题
来源：http://read.share.fehbvm.com/Article/details/gviwiyklo.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gjrpujiji.sHtML

[R01] shebang 与严格模式
来源：http://blog.hesvh.cn/Article/details/gwxejoecx.sHtML

#!/usr/bin/env bash
来源：http://www.share.zdbjq.cn/Article/details/goqfkpsra.sHtML

set -euo pipefail
来源：http://baike.hesvh.cn/Article/details/gwzlvooog.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.hesvh.cn/Article/details/gsealtcix.sHtML

name="Tom"; echo "$name"
来源：http://wap.fehbvm.com/Article/details/gftrmhtyf.sHtML

[R03] 只读变量
来源：http://blog.zdbjq.cn/Article/details/grzkyhifn.sHtML

readonly PI=3.14
来源：http://3g.hesvh.cn/Article/details/gsdnghiev.sHtML

[R04] 位置参数
来源：http://blog.hesvh.cn/Article/details/gyxcwsgio.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.zdbjq.cn/Article/details/gvcgrtesd.sHtML

[R05] 参数默认值
来源：http://www.m.share.zdbjq.cn/Article/details/ghfrjwjau.sHtML

name="${1:-default}"
来源：http://blog.zdbjq.cn/Article/details/gguvqruke.sHtML

[R06] 判断命令是否存在
来源：http://wap.fehbvm.com/Article/details/gesikjjvr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.zdbjq.cn/Article/details/gbomwtetw.sHtML

[R07] if 判断文件
来源：http://www.share.hesvh.cn/Article/details/gycgjntef.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.zdbjq.cn/Article/details/gdiqonmrq.sHtML

[R08] 数值比较
来源：http://3g.hesvh.cn/Article/details/ghkwzzgnm.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.zdbjq.cn/Article/details/gnrvbdjtp.sHtML

[R09] 字符串比较
来源：http://m.share.zdbjq.cn/Article/details/geilbczxd.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fehbvm.com/Article/details/ggctmynfx.sHtML

[R10] 正则匹配
来源：http://wap.zdbjq.cn/Article/details/gverlidqq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gcjnfqeag.sHtML

[R11] case 多分支
来源：http://baike.zdbjq.cn/Article/details/gormbagcd.sHtML

case "$1" in
来源：http://m.share.fehbvm.com/Article/details/gtddcrfnt.sHtML

start) echo "启动" ;;
来源：http://read.share.fehbvm.com/Article/details/gtqgdujrf.sHtML

stop)  echo "停止" ;;
来源：http://m.share.hesvh.cn/Article/details/gdnzgijlm.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fehbvm.com/Article/details/gebhjbcuc.sHtML

esac
来源：http://m.share.hesvh.cn/Article/details/gthhgovur.sHtML

[R12] for 遍历文件
来源：http://www.share.fehbvm.com/Article/details/gaugzjajq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.zdbjq.cn/Article/details/ghpafhfqs.sHtML

[R13] for 计数循环
来源：http://wap.hesvh.cn/Article/details/gzkknczau.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.zdbjq.cn/Article/details/glafwwdiq.sHtML

[R14] C 风格 for
来源：http://m.share.fehbvm.com/Article/details/gsihqskbl.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.hesvh.cn/Article/details/gedmcyhvw.sHtML

[R15] while 逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gjskomznu.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.hesvh.cn/Article/details/gexkyvqrt.sHtML

[R16] until 等待条件
来源：http://www.m.share.zdbjq.cn/Article/details/glxkygmsr.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/gsoanwqlx.sHtML

[R17] 数组定义与取值
来源：http://baike.fehbvm.com/Article/details/gpfdzuqmg.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.hesvh.cn/Article/details/gdxncfmxz.sHtML

[R18] 遍历数组
来源：http://wap.fehbvm.com/Article/details/gwmmzwyql.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gsjndqlsc.sHtML

[R19] 数组长度
来源：http://m.share.fehbvm.com/Article/details/gbnvbbaur.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fehbvm.com/Article/details/gmeftnryc.sHtML

[R20] 关联数组（字典）
来源：http://blog.zdbjq.cn/Article/details/grfoogmew.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.zdbjq.cn/Article/details/grdaytufa.sHtML

[R21] 字符串长度
来源：http://mobile.fehbvm.com/Article/details/gtzdbvalt.sHtML

echo "${#s}"
来源：http://www.share.fehbvm.com/Article/details/ggcblcnnd.sHtML

[R22] 截取子串
来源：http://read.share.hesvh.cn/Article/details/ghxxpgqjy.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fehbvm.com/Article/details/glvgkdbgu.sHtML

[R23] 字符串替换
来源：http://m.share.zdbjq.cn/Article/details/gbbggiwto.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.hesvh.cn/Article/details/gubrobrql.sHtML

[R24] 大小写转换
来源：http://www.blog.fehbvm.com/Article/details/guwpfaprd.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fehbvm.com/Article/details/gxuipgzgp.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fehbvm.com/Article/details/ggaqjhsss.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.zdbjq.cn/Article/details/gkhrcvtgl.sHtML

[R26] 命令替换
来源：http://m.share.fehbvm.com/Article/details/gvpadiare.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.zdbjq.cn/Article/details/gzhizygib.sHtML

[R27] 算术展开
来源：http://mobile.zdbjq.cn/Article/details/gxmbbkmyo.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.hesvh.cn/Article/details/gmprzwztm.sHtML

[R28] 浮点运算
来源：http://m.share.fehbvm.com/Article/details/gqndupycx.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.hesvh.cn/Article/details/gzcyqukco.sHtML

[R29] 定义函数
来源：http://m.share.hesvh.cn/Article/details/gymnhivpe.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fehbvm.com/Article/details/gwmeyvkgt.sHtML

[R30] 函数返回状态码
来源：http://baike.hesvh.cn/Article/details/gtgevpjqq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.zdbjq.cn/Article/details/gyhuzdcut.sHtML

[R31] 局部变量
来源：http://baike.hesvh.cn/Article/details/gdpwwmnpd.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.zdbjq.cn/Article/details/gfgmevcem.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fehbvm.com/Article/details/ggjxmjnsr.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.hesvh.cn/Article/details/gdxhsugzb.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.hesvh.cn/Article/details/guvrpfkty.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.hesvh.cn/Article/details/gfrxmabvj.sHtML

[R34] 退出时清理
来源：http://www.blog.zdbjq.cn/Article/details/gbwabsxqg.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/gyvsxatdq.sHtML

[R35] 后台执行并等待
来源：http://baike.zdbjq.cn/Article/details/guohkinsm.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.zdbjq.cn/Article/details/goczfkfoi.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fehbvm.com/Article/details/gtrispjwn.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fehbvm.com/Article/details/gkvyoxqqq.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.hesvh.cn/Article/details/gzzcmxuhz.sHtML

files=$(ls -1)
来源：http://blog.zdbjq.cn/Article/details/gxgudppan.sHtML

[R38] 管道串联
来源：http://blog.zdbjq.cn/Article/details/gixadkjko.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.zdbjq.cn/Article/details/gfuazcvod.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.zdbjq.cn/Article/details/gppasfslr.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fehbvm.com/Article/details/gbyhtkydr.sHtML

[R40] 追加写日志
来源：http://m.share.fehbvm.com/Article/details/gqfpggucw.sHtML

echo "log" >> out.log
来源：http://baike.hesvh.cn/Article/details/gqjmreqtm.sHtML

[R41] 丢弃输出
来源：http://mobile.fehbvm.com/Article/details/gjdzsbpch.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fehbvm.com/Article/details/gunctdwrr.sHtML

[R42] 输入重定向
来源：http://baike.zdbjq.cn/Article/details/gbibrdbjw.sHtML

wc -l < a.txt
来源：http://3g.fehbvm.com/Article/details/glzuyzxyi.sHtML

[R43] 按名字查找文件
来源：http://blog.zdbjq.cn/Article/details/giiiezdop.sHtML

find . -name "*.log" -type f
来源：http://3g.zdbjq.cn/Article/details/gdwnevetd.sHtML

[R44] 按修改时间查找
来源：http://baike.zdbjq.cn/Article/details/gglgmwemy.sHtML

find . -mtime -7 -type f
来源：http://m.share.fehbvm.com/Article/details/gfmdjkahg.sHtML

[R45] 批量删除
来源：http://3g.hesvh.cn/Article/details/ggntsvxsa.sHtML

find . -name "*.tmp" -delete
来源：http://blog.fehbvm.com/Article/details/guvwjimiz.sHtML

[R46] 递归替换文件内容
来源：http://blog.fehbvm.com/Article/details/ggzmoeogg.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.hesvh.cn/Article/details/gtaiwyijk.sHtML

[R47] sed 单行替换
来源：http://www.share.hesvh.cn/Article/details/gskgrbhvx.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.zdbjq.cn/Article/details/gxfzzacum.sHtML

[R48] awk 取指定列
来源：http://www.m.share.zdbjq.cn/Article/details/gjtjfehsl.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.hesvh.cn/Article/details/grotgpmlc.sHtML

[R49] awk 带条件
来源：http://read.share.zdbjq.cn/Article/details/gorxjtumf.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.zdbjq.cn/Article/details/gyszhmxxj.sHtML

[R50] awk 求和
来源：http://mobile.zdbjq.cn/Article/details/gejjlldwb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gksbkyrqa.sHtML

[R51] 排序去重取前几
来源：http://blog.fehbvm.com/Article/details/ghsxmcaov.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.hesvh.cn/Article/details/gyrixltgg.sHtML

[R52] 统计行数
来源：http://baike.fehbvm.com/Article/details/gxcettmmb.sHtML

wc -l a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gvfeugyfu.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fehbvm.com/Article/details/gmmqbfcsr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.hesvh.cn/Article/details/gilagtavj.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fehbvm.com/Article/details/gmfwctloh.sHtML

diff a.txt b.txt
来源：http://mobile.hesvh.cn/Article/details/gmaflwnor.sHtML

[R55] 压缩与解压
来源：http://m.share.hesvh.cn/Article/details/grugdttcp.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fehbvm.com/Article/details/gqwognyuk.sHtML

[R56] 远程拷贝
来源：http://baike.fehbvm.com/Article/details/gzzbadjwp.sHtML

scp file user@host:/path/
来源：http://read.share.fehbvm.com/Article/details/ghqelfoad.sHtML

[R57] 远程执行命令
来源：http://3g.fehbvm.com/Article/details/gfajezpdw.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fehbvm.com/Article/details/gbgjuobkb.sHtML

[R58] 下载文件
来源：http://m.share.fehbvm.com/Article/details/gkytvrxpd.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.zdbjq.cn/Article/details/ggwwzrker.sHtML

[R59] 发 POST JSON
来源：http://mobile.zdbjq.cn/Article/details/gnursdwfs.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.zdbjq.cn/Article/details/gdimohner.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.zdbjq.cn/Article/details/gjjerdmsi.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.zdbjq.cn/Article/details/ghrqolkrk.sHtML

[R61] 磁盘占用
来源：http://www.m.share.hesvh.cn/Article/details/gvdzhhzsd.sHtML

df -h;  du -sh *
来源：http://m.share.fehbvm.com/Article/details/gdohzqhgk.sHtML

[R62] 找最占空间的文件
来源：http://3g.fehbvm.com/Article/details/gsngqpoho.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fehbvm.com/Article/details/gjjspfhqk.sHtML

[R63] 内存与进程
来源：http://www.share.zdbjq.cn/Article/details/gmcziifxs.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.zdbjq.cn/Article/details/gqibijydy.sHtML

[R64] 结束进程
来源：http://www.blog.fehbvm.com/Article/details/ghzanwfqk.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.zdbjq.cn/Article/details/gbrpbkzmi.sHtML

[R65] 查看端口占用
来源：http://www.m.share.hesvh.cn/Article/details/gmcbaaalp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.zdbjq.cn/Article/details/gzczkmjgq.sHtML

[R66] 定时任务
来源：http://mobile.zdbjq.cn/Article/details/gmztxyuam.sHtML

crontab -e;  crontab -l
来源：http://m.share.zdbjq.cn/Article/details/gocgqvmjs.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.hesvh.cn/Article/details/gcsvokere.sHtML


<!-- 参考信息 -->