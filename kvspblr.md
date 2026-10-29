代发 wailian999

SELECT * FROM users WHERE email IS NULL;
来源：http://blog.fehbvm.com/Article/details/gfftzkajm.sHtML

[Q22] 排序
来源：http://m.share.hesvh.cn/Article/details/gtpsvsqwl.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.hesvh.cn/Article/details/giwplwwch.sHtML

[Q23] 分页
来源：http://read.share.hesvh.cn/Article/details/gmwkasakq.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.zdbjq.cn/Article/details/gbxjwpagz.sHtML

[Q24] 去重
来源：http://read.share.zdbjq.cn/Article/details/gmdidffut.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.hesvh.cn/Article/details/gbcdvysef.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.hesvh.cn/Article/details/gqrqldhob.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.zdbjq.cn/Article/details/gzoriimsm.sHtML

[Q26] 计数
来源：http://baike.zdbjq.cn/Article/details/gznbjvltp.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gqvzgrpum.sHtML

[Q27] 条件计数
来源：http://read.share.hesvh.cn/Article/details/guaaweusp.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.fehbvm.com/Article/details/gaxxepmuj.sHtML

[Q28] 求和与平均
来源：http://blog.zdbjq.cn/Article/details/ggtqsyaby.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gwhugapzd.sHtML

[Q29] 最大最小值
来源：http://www.share.hesvh.cn/Article/details/gyqetfeel.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/glryhcfat.sHtML

[Q30] 分组统计
来源：http://www.share.zdbjq.cn/Article/details/gwwtkrhpz.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/gkahpnbsw.sHtML

[Q31] 分组后过滤
来源：http://baike.zdbjq.cn/Article/details/gpvgpsdyp.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.fehbvm.com/Article/details/gryygmzqm.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.fehbvm.com/Article/details/guhbtirtp.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/gjnefakzk.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.zdbjq.cn/Article/details/giaziontg.sHtML

[Q33] 多列分组
来源：http://www.share.zdbjq.cn/Article/details/gqzqkxpah.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.hesvh.cn/Article/details/gdzwpcrct.sHtML

[Q34] 每组取第一条
来源：http://mobile.hesvh.cn/Article/details/gxqausbcx.sHtML

SELECT * FROM (
来源：http://mobile.fehbvm.com/Article/details/guzxfwolp.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.zdbjq.cn/Article/details/gfrhvedjv.sHtML

) t WHERE rn = 1;
来源：http://mobile.zdbjq.cn/Article/details/gurbefyau.sHtML

[Q35] 内连接
来源：http://www.blog.fehbvm.com/Article/details/gwdsiwtel.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.zdbjq.cn/Article/details/gwftykyjv.sHtML

[Q36] 左连接
来源：http://read.share.zdbjq.cn/Article/details/gvspmphck.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.hesvh.cn/Article/details/gmshkuvay.sHtML

[Q37] 右连接
来源：http://wap.hesvh.cn/Article/details/grcpxjlmw.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.fehbvm.com/Article/details/gtsqjdxco.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.zdbjq.cn/Article/details/gtgjcrbnt.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.hesvh.cn/Article/details/gqacdbmjx.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.zdbjq.cn/Article/details/gwbtadicg.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.fehbvm.com/Article/details/gifzumjjw.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.fehbvm.com/Article/details/gfmnmcwza.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.zdbjq.cn/Article/details/gsgmwfunn.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.hesvh.cn/Article/details/geiwrrguf.sHtML

[Q41] 多表连接
来源：http://www.share.fehbvm.com/Article/details/gejhdwgdc.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.zdbjq.cn/Article/details/glocnfwkb.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.hesvh.cn/Article/details/gbdmixhmz.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.hesvh.cn/Article/details/gchrryvoc.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.hesvh.cn/Article/details/gmxiuwgti.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.fehbvm.com/Article/details/gjfsrmmxh.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.hesvh.cn/Article/details/glbdiqzxd.sHtML

[Q43] 标量子查询
来源：http://wap.fehbvm.com/Article/details/gjjuwvcko.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.fehbvm.com/Article/details/gqawymham.sHtML

[Q44] IN 子查询
来源：http://3g.hesvh.cn/Article/details/gnyjiqtrs.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.fehbvm.com/Article/details/gqyxyqyqk.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.fehbvm.com/Article/details/ggmyonkfw.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.hesvh.cn/Article/details/gdluvdwre.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.hesvh.cn/Article/details/gfmlbohem.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fehbvm.com/Article/details/grehvlwxa.sHtML

[Q47] 与平均值比较
来源：http://mobile.zdbjq.cn/Article/details/grljabpap.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.zdbjq.cn/Article/details/gvornzqjt.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.zdbjq.cn/Article/details/gngitkqbj.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.fehbvm.com/Article/details/gitwmcpcl.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.fehbvm.com/Article/details/gerizsngt.sHtML

[Q49] 更新单行
来源：http://www.m.share.hesvh.cn/Article/details/gkxgcsven.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.zdbjq.cn/Article/details/grzcdazpe.sHtML

[Q50] 批量更新
来源：http://www.blog.fehbvm.com/Article/details/gyvtxdble.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.zdbjq.cn/Article/details/gngkbwhtw.sHtML

[Q51] 用子查询更新
来源：http://m.share.zdbjq.cn/Article/details/gfzxhmozn.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gbwnorhah.sHtML

[Q52] 删除指定行
来源：http://wap.hesvh.cn/Article/details/gmbyjtqck.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.zdbjq.cn/Article/details/gmegsuegi.sHtML

[Q53] 按条件删除
来源：http://www.m.share.fehbvm.com/Article/details/gdmoixncc.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.zdbjq.cn/Article/details/gypqbmysm.sHtML

[Q54] 清空表
来源：http://baike.zdbjq.cn/Article/details/gbklgkowg.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.zdbjq.cn/Article/details/grjzzhoki.sHtML

[Q55] 排名（并列占位）
来源：http://baike.fehbvm.com/Article/details/geftpjalp.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.zdbjq.cn/Article/details/geadmqaxw.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.fehbvm.com/Article/details/gplavlqvt.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.zdbjq.cn/Article/details/goxplmzbh.sHtML

[Q57] 行号
来源：http://baike.fehbvm.com/Article/details/gtmohqttk.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gbkuputmt.sHtML

[Q58] 累计求和
来源：http://baike.fehbvm.com/Article/details/gzhspzmpq.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gzifztdef.sHtML

[Q59] 分组内累计
来源：http://blog.fehbvm.com/Article/details/gyoppzcxn.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gqfvgdrkn.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.hesvh.cn/Article/details/gswxtrkex.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.fehbvm.com/Article/details/gznbfzszm.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gcpqcznym.sHtML

[Q61] 移动平均
来源：http://mobile.hesvh.cn/Article/details/ghohpccpr.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gpxqkdnmy.sHtML

[Q62] 分组占比
来源：http://mobile.zdbjq.cn/Article/details/gqeaaxorf.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/grfajtqne.sHtML

[Q63] 开启事务
来源：http://www.share.zdbjq.cn/Article/details/gnzrrxnlp.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.fehbvm.com/Article/details/gthrdottj.sHtML

[Q64] 提交事务
来源：http://baike.hesvh.cn/Article/details/glsecyodu.sHtML

COMMIT;
来源：http://wap.fehbvm.com/Article/details/gbxltstgt.sHtML

[Q65] 回滚事务
来源：http://blog.fehbvm.com/Article/details/gazhtnkji.sHtML

ROLLBACK;
来源：http://mobile.fehbvm.com/Article/details/gpduzpsqj.sHtML

[Q66] 行锁查询
来源：http://3g.hesvh.cn/Article/details/gwieqrggn.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.hesvh.cn/Article/details/gbzehfurf.sHtML

[Q67] 设置隔离级别
来源：http://www.share.hesvh.cn/Article/details/gjkshzdbq.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.hesvh.cn/Article/details/gpzxqdqac.sHtML

[Q68] 保存点
来源：http://blog.zdbjq.cn/Article/details/gywbvkqdd.sHtML

SAVEPOINT sp1;
来源：http://m.share.zdbjq.cn/Article/details/grzxwjdua.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.fehbvm.com/Article/details/goukmwqua.sHtML

[Q69] 查看执行计划
来源：http://www.share.fehbvm.com/Article/details/gkvlzbvkw.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.fehbvm.com/Article/details/gitiyrsfm.sHtML

[Q70] 更新统计信息
来源：http://wap.zdbjq.cn/Article/details/guvlwcbww.sHtML

ANALYZE TABLE users;
来源：http://blog.fehbvm.com/Article/details/gyazdexag.sHtML

[Q71] 查看建表语句
来源：http://wap.fehbvm.com/Article/details/gmjqcjzwm.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.zdbjq.cn/Article/details/gijligrwz.sHtML

[Q72] 查看索引
来源：http://www.m.share.zdbjq.cn/Article/details/gqwsxynye.sHtML

SHOW INDEX FROM users;
来源：http://baike.fehbvm.com/Article/details/gxehdzqle.sHtML

[Q73] 查看表状态
来源：http://www.blog.hesvh.cn/Article/details/gbluitscq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.fehbvm.com/Article/details/gejieblkz.sHtML

[Q74] 强制使用索引
来源：http://baike.hesvh.cn/Article/details/gonikiimg.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.hesvh.cn/Article/details/gynezeiny.sHtML

[Q75] 日期格式化
来源：http://wap.hesvh.cn/Article/details/gkotpguuf.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gattrvslc.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.hesvh.cn/Article/details/gzuopwadf.sHtML

[Q76] 按天统计
来源：http://wap.hesvh.cn/Article/details/gcooodybr.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fehbvm.com/Article/details/gaixhmcnq.sHtML

[Q77] 时间加减
来源：http://mobile.zdbjq.cn/Article/details/gukjtwguu.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.hesvh.cn/Article/details/geqbwaqkg.sHtML

[Q78] 当前时间
来源：http://m.share.fehbvm.com/Article/details/ghnubgbps.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.zdbjq.cn/Article/details/gteiebjsc.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.zdbjq.cn/Article/details/grxafghdk.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.zdbjq.cn/Article/details/gmpegjwem.sHtML

[Q80] 字符串截取
来源：http://www.m.share.fehbvm.com/Article/details/gkiuogpyy.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gzzktuyrs.sHtML

[Q81] 字符串替换
来源：http://www.share.hesvh.cn/Article/details/gwmjqkojf.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.hesvh.cn/Article/details/gptfwvlbf.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fehbvm.com/Article/details/gmehdqnjk.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gvvjyxjsg.sHtML

[Q83] 大小写转换
来源：http://blog.fehbvm.com/Article/details/gdfwufxzm.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/goycripen.sHtML

[Q84] 去除首尾空格
来源：http://m.share.hesvh.cn/Article/details/gkvpftwvo.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gltdejoad.sHtML

[Q85] 数值取整
来源：http://www.m.share.fehbvm.com/Article/details/gqpyltvzj.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.zdbjq.cn/Article/details/gnztsexqc.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.hesvh.cn/Article/details/gtfnwtyvq.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.zdbjq.cn/Article/details/gxmvzirej.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.fehbvm.com/Article/details/gphbvihdg.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fehbvm.com/Article/details/gofowizxy.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fehbvm.com/Article/details/gtvebkzjk.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.zdbjq.cn/Article/details/gyjuxgumc.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.hesvh.cn/Article/details/gfdywqmpq.sHtML

[Q89] 判断表是否存在
来源：http://m.share.zdbjq.cn/Article/details/gfhmgqswx.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.fehbvm.com/Article/details/gogndyzdl.sHtML

[Q90] 生成序号列
来源：http://baike.fehbvm.com/Article/details/ghfkrsgqj.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.zdbjq.cn/Article/details/gqirtraij.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gjlusuhse.sHtML

R. Bash 专题
来源：http://blog.hesvh.cn/Article/details/gyouhgumr.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/glrmpquzi.sHtML

[R01] shebang 与严格模式
来源：http://3g.zdbjq.cn/Article/details/gokxjoynd.sHtML

#!/usr/bin/env bash
来源：http://m.share.zdbjq.cn/Article/details/goykqcxnh.sHtML

set -euo pipefail
来源：http://mobile.hesvh.cn/Article/details/grqtmkfku.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.zdbjq.cn/Article/details/gabmmfbzf.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.hesvh.cn/Article/details/gianntjhq.sHtML

[R03] 只读变量
来源：http://www.share.zdbjq.cn/Article/details/gfqsroeki.sHtML

readonly PI=3.14
来源：http://www.blog.zdbjq.cn/Article/details/gclmfyoqn.sHtML

[R04] 位置参数
来源：http://www.blog.fehbvm.com/Article/details/gqwgcvyrn.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.zdbjq.cn/Article/details/gtefbgkuk.sHtML

[R05] 参数默认值
来源：http://m.share.fehbvm.com/Article/details/ghmuxqqzf.sHtML

name="${1:-default}"
来源：http://mobile.zdbjq.cn/Article/details/gbiihpoxx.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fehbvm.com/Article/details/giykzqdxd.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/gwdqvvckd.sHtML

[R07] if 判断文件
来源：http://www.share.hesvh.cn/Article/details/gmqoiuesz.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gpejsucuu.sHtML

[R08] 数值比较
来源：http://wap.zdbjq.cn/Article/details/gjsxffbok.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.hesvh.cn/Article/details/gczmjmoal.sHtML

[R09] 字符串比较
来源：http://m.share.hesvh.cn/Article/details/gnjexqald.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.hesvh.cn/Article/details/ggccaejom.sHtML

[R10] 正则匹配
来源：http://www.blog.fehbvm.com/Article/details/gmfirsmxq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fehbvm.com/Article/details/gyuabylbi.sHtML

[R11] case 多分支
来源：http://m.share.hesvh.cn/Article/details/ghbygelkz.sHtML

case "$1" in
来源：http://www.share.hesvh.cn/Article/details/gxovgdcpn.sHtML

start) echo "启动" ;;
来源：http://baike.hesvh.cn/Article/details/gszclfnbw.sHtML

stop)  echo "停止" ;;
来源：http://read.share.zdbjq.cn/Article/details/gfesuerlr.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gvorcypfo.sHtML

esac
来源：http://baike.hesvh.cn/Article/details/gtpaxfvlz.sHtML

[R12] for 遍历文件
来源：http://baike.fehbvm.com/Article/details/gjqtmyzrn.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.hesvh.cn/Article/details/gcauujigr.sHtML

[R13] for 计数循环
来源：http://mobile.zdbjq.cn/Article/details/gmeuppdhw.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.zdbjq.cn/Article/details/gzszrmcxe.sHtML

[R14] C 风格 for
来源：http://www.share.hesvh.cn/Article/details/gcsmhqjxt.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.zdbjq.cn/Article/details/gpwgrbiwa.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/giymegcbh.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.zdbjq.cn/Article/details/gyiumpftg.sHtML

[R16] until 等待条件
来源：http://3g.fehbvm.com/Article/details/gqgsxbejd.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.zdbjq.cn/Article/details/gpmjrmiax.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fehbvm.com/Article/details/gkqhxpfrf.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.hesvh.cn/Article/details/grtksysyl.sHtML

[R18] 遍历数组
来源：http://www.blog.zdbjq.cn/Article/details/geyjlyijp.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fehbvm.com/Article/details/gvzklbcin.sHtML

[R19] 数组长度
来源：http://blog.fehbvm.com/Article/details/ghahqjbok.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fehbvm.com/Article/details/gfukytouq.sHtML

[R20] 关联数组（字典）
来源：http://baike.zdbjq.cn/Article/details/gqiswfnpf.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.zdbjq.cn/Article/details/gioiagbfb.sHtML

[R21] 字符串长度
来源：http://mobile.fehbvm.com/Article/details/gaevmdhdp.sHtML

echo "${#s}"
来源：http://wap.hesvh.cn/Article/details/gjscmdbbi.sHtML

[R22] 截取子串
来源：http://www.share.hesvh.cn/Article/details/gvjehkoag.sHtML

echo "${s:0:5}"
来源：http://www.m.share.hesvh.cn/Article/details/geepyduod.sHtML

[R23] 字符串替换
来源：http://baike.hesvh.cn/Article/details/gweftxegu.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.zdbjq.cn/Article/details/gxrpcamax.sHtML

[R24] 大小写转换
来源：http://www.m.share.fehbvm.com/Article/details/gdkdqgply.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.hesvh.cn/Article/details/gsgjyfbic.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fehbvm.com/Article/details/gdqqjnupi.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.hesvh.cn/Article/details/gzyuodbsf.sHtML

[R26] 命令替换
来源：http://baike.zdbjq.cn/Article/details/gyfhimxly.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.zdbjq.cn/Article/details/gvnsystxa.sHtML

[R27] 算术展开
来源：http://www.share.zdbjq.cn/Article/details/gsqfzgzzi.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fehbvm.com/Article/details/glbpfkxcj.sHtML

[R28] 浮点运算
来源：http://baike.hesvh.cn/Article/details/gbmebthno.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.zdbjq.cn/Article/details/gfjkwccio.sHtML

[R29] 定义函数
来源：http://3g.fehbvm.com/Article/details/ghgkolfji.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fehbvm.com/Article/details/ggmqznija.sHtML

[R30] 函数返回状态码
来源：http://baike.fehbvm.com/Article/details/gpqpknxag.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.hesvh.cn/Article/details/gwjcfzobs.sHtML

[R31] 局部变量
来源：http://www.blog.hesvh.cn/Article/details/gwcufuafr.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.hesvh.cn/Article/details/gwylwhfdv.sHtML

[R32] 参数个数校验
来源：http://www.share.hesvh.cn/Article/details/gwxeeqyrn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fehbvm.com/Article/details/gavhhibed.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fehbvm.com/Article/details/gqikhtjll.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fehbvm.com/Article/details/gxhaxemzk.sHtML

[R34] 退出时清理
来源：http://blog.fehbvm.com/Article/details/gyivoglyk.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.zdbjq.cn/Article/details/gvrtdtvor.sHtML

[R35] 后台执行并等待
来源：http://blog.hesvh.cn/Article/details/gnaqlaxfq.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.hesvh.cn/Article/details/gyhlbpytz.sHtML

[R36] 并发执行多个任务
来源：http://www.share.hesvh.cn/Article/details/ghxcuylob.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.zdbjq.cn/Article/details/gorwrjbvw.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fehbvm.com/Article/details/gofzzyebt.sHtML

files=$(ls -1)
来源：http://3g.fehbvm.com/Article/details/gzjbncrfl.sHtML

[R38] 管道串联
来源：http://www.blog.hesvh.cn/Article/details/glvjnulan.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.zdbjq.cn/Article/details/glifjnyaq.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fehbvm.com/Article/details/gzxzwwgnp.sHtML

cmd > out.log 2>&1
来源：http://www.blog.hesvh.cn/Article/details/gatoaiuov.sHtML

[R40] 追加写日志
来源：http://baike.fehbvm.com/Article/details/gdcvaxnii.sHtML

echo "log" >> out.log
来源：http://m.share.zdbjq.cn/Article/details/grxazrqav.sHtML

[R41] 丢弃输出
来源：http://www.share.hesvh.cn/Article/details/gbmswikud.sHtML

cmd >/dev/null 2>&1
来源：http://blog.hesvh.cn/Article/details/gffqofocv.sHtML

[R42] 输入重定向
来源：http://baike.hesvh.cn/Article/details/gnklqualv.sHtML

wc -l < a.txt
来源：http://wap.fehbvm.com/Article/details/gmgegixru.sHtML

[R43] 按名字查找文件
来源：http://blog.fehbvm.com/Article/details/gsdmjxbfy.sHtML

find . -name "*.log" -type f
来源：http://www.share.hesvh.cn/Article/details/gczdqtbvo.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.zdbjq.cn/Article/details/gjarzqvxo.sHtML

find . -mtime -7 -type f
来源：http://read.share.zdbjq.cn/Article/details/gppqyjeuf.sHtML

[R45] 批量删除
来源：http://m.share.zdbjq.cn/Article/details/ggwfmboij.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.hesvh.cn/Article/details/gtctogmeo.sHtML

[R46] 递归替换文件内容
来源：http://baike.zdbjq.cn/Article/details/gkkiblrmg.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fehbvm.com/Article/details/gqanqdzde.sHtML

[R47] sed 单行替换
来源：http://www.share.hesvh.cn/Article/details/gwnmxmtdb.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.hesvh.cn/Article/details/gkpgomrtm.sHtML

[R48] awk 取指定列
来源：http://3g.zdbjq.cn/Article/details/gfbxuhlrg.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.hesvh.cn/Article/details/gwnuqgquz.sHtML

[R49] awk 带条件
来源：http://wap.hesvh.cn/Article/details/gyivepbvv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.zdbjq.cn/Article/details/gpltqvopu.sHtML

[R50] awk 求和
来源：http://m.share.zdbjq.cn/Article/details/gudgoioyf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.hesvh.cn/Article/details/gigsbqfyr.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fehbvm.com/Article/details/gxhksmjeb.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fehbvm.com/Article/details/gcqbthdfq.sHtML

[R52] 统计行数
来源：http://mobile.zdbjq.cn/Article/details/giknngbjf.sHtML

wc -l a.txt
来源：http://wap.zdbjq.cn/Article/details/glwwdzrig.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.hesvh.cn/Article/details/gidgmsgfr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.hesvh.cn/Article/details/gcvjvaoot.sHtML

[R54] 比较两个文件
来源：http://read.share.fehbvm.com/Article/details/gjgekiadh.sHtML

diff a.txt b.txt
来源：http://baike.zdbjq.cn/Article/details/goqbgnvjw.sHtML

[R55] 压缩与解压
来源：http://m.share.zdbjq.cn/Article/details/gtmskucpa.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.hesvh.cn/Article/details/gpvhlybfm.sHtML

[R56] 远程拷贝
来源：http://www.share.hesvh.cn/Article/details/gbrmvfcfa.sHtML

scp file user@host:/path/
来源：http://baike.hesvh.cn/Article/details/gqkgzgifh.sHtML

[R57] 远程执行命令
来源：http://www.m.share.hesvh.cn/Article/details/gitvnxunc.sHtML

ssh user@host 'uptime'
来源：http://read.share.fehbvm.com/Article/details/goycqzxsh.sHtML

[R58] 下载文件
来源：http://blog.zdbjq.cn/Article/details/ggiuteoau.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.hesvh.cn/Article/details/gkmhensva.sHtML

[R59] 发 POST JSON
来源：http://3g.fehbvm.com/Article/details/gijuecozf.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.zdbjq.cn/Article/details/gjthfztvm.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fehbvm.com/Article/details/gnkfkuuwf.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fehbvm.com/Article/details/goedplacr.sHtML

[R61] 磁盘占用
来源：http://read.share.fehbvm.com/Article/details/gkvwllgif.sHtML

df -h;  du -sh *
来源：http://3g.zdbjq.cn/Article/details/giblrwsgg.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.hesvh.cn/Article/details/givdyjcek.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.hesvh.cn/Article/details/gcezjeqsa.sHtML

[R63] 内存与进程
来源：http://wap.zdbjq.cn/Article/details/giohveudg.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.zdbjq.cn/Article/details/gitulzgny.sHtML

[R64] 结束进程
来源：http://mobile.hesvh.cn/Article/details/gpdwazokn.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.zdbjq.cn/Article/details/gyktyrkqd.sHtML

[R65] 查看端口占用
来源：http://www.blog.zdbjq.cn/Article/details/gwcletxnx.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fehbvm.com/Article/details/glaojectp.sHtML

[R66] 定时任务
来源：http://wap.hesvh.cn/Article/details/grcyhuohh.sHtML

crontab -e;  crontab -l
来源：http://mobile.fehbvm.com/Article/details/gwuyzsehd.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.zdbjq.cn/Article/details/gkvfolart.sHtML

openssl rand -hex 16
来源：http://m.share.zdbjq.cn/Article/details/gdgotjpdo.sHtML

[R68] 计算文件校验值
来源：http://wap.hesvh.cn/Article/details/gbfsrjzqe.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.hesvh.cn/Article/details/ggyocucog.sHtML

[R69] 生成随机密码
来源：http://3g.hesvh.cn/Article/details/gunwuykim.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fehbvm.com/Article/details/gtkjhghmq.sHtML

[R70] 时间戳与互转
来源：http://read.share.fehbvm.com/Article/details/golcjtwhi.sHtML

date +%s;  date -d @1700000000
来源：http://baike.hesvh.cn/Article/details/givhptisu.sHtML

[R71] 日期格式化
来源：http://www.share.hesvh.cn/Article/details/gjmpjxljm.sHtML


<!-- 参考信息 -->