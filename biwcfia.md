代发 wailian999

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.fehbvm.com/Article/details/gdtfqmair.sHtML

[Q22] 排序
来源：http://wap.fehbvm.com/Article/details/gvcnpvpyz.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.m.share.hesvh.cn/Article/details/gvqtsrayg.sHtML

[Q23] 分页
来源：http://mobile.zdbjq.cn/Article/details/gaxxpblyu.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.hesvh.cn/Article/details/gxxtahoea.sHtML

[Q24] 去重
来源：http://www.share.fehbvm.com/Article/details/gmzjzofgh.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.share.hesvh.cn/Article/details/gumhwnkom.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.fehbvm.com/Article/details/gwffpqkpy.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.hesvh.cn/Article/details/gxdbntgck.sHtML

[Q26] 计数
来源：http://wap.zdbjq.cn/Article/details/gvkdmirst.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gvnryctmz.sHtML

[Q27] 条件计数
来源：http://blog.zdbjq.cn/Article/details/giuozglgo.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.hesvh.cn/Article/details/gcrrmihps.sHtML

[Q28] 求和与平均
来源：http://read.share.fehbvm.com/Article/details/gtvkxudqn.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.hesvh.cn/Article/details/gabtkbovy.sHtML

[Q29] 最大最小值
来源：http://www.share.hesvh.cn/Article/details/gddlunfoj.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.fehbvm.com/Article/details/ghjmmesij.sHtML

[Q30] 分组统计
来源：http://read.share.hesvh.cn/Article/details/gkgvuwwos.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/glewfqulc.sHtML

[Q31] 分组后过滤
来源：http://3g.zdbjq.cn/Article/details/ggfzmsplh.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.hesvh.cn/Article/details/gcmovmhbg.sHtML

[Q32] 分组拼接字符串
来源：http://wap.hesvh.cn/Article/details/gjuntueoh.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/gpfsmznoe.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.hesvh.cn/Article/details/gluixrksd.sHtML

[Q33] 多列分组
来源：http://www.share.hesvh.cn/Article/details/gmwnnemol.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.zdbjq.cn/Article/details/gwyadxakr.sHtML

[Q34] 每组取第一条
来源：http://read.share.hesvh.cn/Article/details/gqzpexioe.sHtML

SELECT * FROM (
来源：http://mobile.zdbjq.cn/Article/details/gcwjlrerf.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.hesvh.cn/Article/details/gqgezgswa.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.fehbvm.com/Article/details/grwnsyvbd.sHtML

[Q35] 内连接
来源：http://www.blog.zdbjq.cn/Article/details/gvbisxdhg.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.fehbvm.com/Article/details/gkqukdoqe.sHtML

[Q36] 左连接
来源：http://www.share.hesvh.cn/Article/details/grltbhujp.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.fehbvm.com/Article/details/gvduoesis.sHtML

[Q37] 右连接
来源：http://www.share.fehbvm.com/Article/details/gfaavhpdv.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.hesvh.cn/Article/details/ghpolqrbm.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.hesvh.cn/Article/details/gwlckhzge.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.zdbjq.cn/Article/details/gohxfrwhj.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.zdbjq.cn/Article/details/gohurcsmi.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.zdbjq.cn/Article/details/gtaxnnory.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.hesvh.cn/Article/details/gjpwrfteb.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.zdbjq.cn/Article/details/ggaropzgi.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.fehbvm.com/Article/details/gpebrbwsz.sHtML

[Q41] 多表连接
来源：http://wap.fehbvm.com/Article/details/gsmklpaeq.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.fehbvm.com/Article/details/ghojlqkoy.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.zdbjq.cn/Article/details/gjvjhmyop.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.hesvh.cn/Article/details/ggiqlpino.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.zdbjq.cn/Article/details/gcharxxxh.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.hesvh.cn/Article/details/gvdckvbsv.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.fehbvm.com/Article/details/gmwqskjnf.sHtML

[Q43] 标量子查询
来源：http://blog.hesvh.cn/Article/details/gioretqif.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.hesvh.cn/Article/details/gggibndet.sHtML

[Q44] IN 子查询
来源：http://blog.hesvh.cn/Article/details/grcrxmdra.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.hesvh.cn/Article/details/goryfvoii.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.fehbvm.com/Article/details/gwwbtnouz.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fehbvm.com/Article/details/ghipjhcso.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.hesvh.cn/Article/details/gjtgtprkr.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.hesvh.cn/Article/details/ghueoqzbl.sHtML

[Q47] 与平均值比较
来源：http://read.share.fehbvm.com/Article/details/gaesbvhie.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.zdbjq.cn/Article/details/gyoosiion.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.hesvh.cn/Article/details/glindcomh.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.zdbjq.cn/Article/details/glmxundnp.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.zdbjq.cn/Article/details/gepcfwfnn.sHtML

[Q49] 更新单行
来源：http://www.blog.hesvh.cn/Article/details/gkcvhhlqi.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.fehbvm.com/Article/details/gjicshrhv.sHtML

[Q50] 批量更新
来源：http://baike.fehbvm.com/Article/details/gfiksuwge.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.zdbjq.cn/Article/details/gdqbzirhv.sHtML

[Q51] 用子查询更新
来源：http://m.share.zdbjq.cn/Article/details/gjjjzbfgf.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.hesvh.cn/Article/details/gdyordgrh.sHtML

[Q52] 删除指定行
来源：http://baike.zdbjq.cn/Article/details/ghglecabh.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.fehbvm.com/Article/details/gdqwzorod.sHtML

[Q53] 按条件删除
来源：http://wap.fehbvm.com/Article/details/gqxetltws.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.fehbvm.com/Article/details/gkmfbvjhd.sHtML

[Q54] 清空表
来源：http://baike.fehbvm.com/Article/details/gpqgiscrf.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.hesvh.cn/Article/details/gkzqjsszz.sHtML

[Q55] 排名（并列占位）
来源：http://blog.zdbjq.cn/Article/details/gojjxctmz.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.hesvh.cn/Article/details/goqedozgn.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.hesvh.cn/Article/details/gstionmuc.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.fehbvm.com/Article/details/gfenfbpiv.sHtML

[Q57] 行号
来源：http://www.m.share.zdbjq.cn/Article/details/gkjpkxasl.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.fehbvm.com/Article/details/gpmfoihcm.sHtML

[Q58] 累计求和
来源：http://baike.hesvh.cn/Article/details/gmzeeurge.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gyswigzxq.sHtML

[Q59] 分组内累计
来源：http://mobile.fehbvm.com/Article/details/ggsbrquvl.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gmlityttz.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.zdbjq.cn/Article/details/gdjnwjnkl.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.hesvh.cn/Article/details/gijbedwtb.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fehbvm.com/Article/details/gblqofwec.sHtML

[Q61] 移动平均
来源：http://www.m.share.zdbjq.cn/Article/details/gezblncsb.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/ggjzorzmb.sHtML

[Q62] 分组占比
来源：http://mobile.fehbvm.com/Article/details/gwqefjtse.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/ghdqhntey.sHtML

[Q63] 开启事务
来源：http://mobile.hesvh.cn/Article/details/gdlhuohfd.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.fehbvm.com/Article/details/gjlwfkbjq.sHtML

[Q64] 提交事务
来源：http://www.m.share.fehbvm.com/Article/details/gltyoscug.sHtML

COMMIT;
来源：http://blog.zdbjq.cn/Article/details/gkwvwyluc.sHtML

[Q65] 回滚事务
来源：http://www.share.zdbjq.cn/Article/details/govleezls.sHtML

ROLLBACK;
来源：http://baike.hesvh.cn/Article/details/gwtuepkkd.sHtML

[Q66] 行锁查询
来源：http://www.blog.hesvh.cn/Article/details/gewprdmde.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fehbvm.com/Article/details/gygcbkkli.sHtML

[Q67] 设置隔离级别
来源：http://www.share.zdbjq.cn/Article/details/gvrlpcrvo.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.zdbjq.cn/Article/details/gzmhfjdct.sHtML

[Q68] 保存点
来源：http://blog.zdbjq.cn/Article/details/ggolufyit.sHtML

SAVEPOINT sp1;
来源：http://blog.hesvh.cn/Article/details/gyjpaegfb.sHtML

ROLLBACK TO sp1;
来源：http://m.share.hesvh.cn/Article/details/gzwyfntgc.sHtML

[Q69] 查看执行计划
来源：http://wap.hesvh.cn/Article/details/gisnqqgnx.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.hesvh.cn/Article/details/glxlnbcpo.sHtML

[Q70] 更新统计信息
来源：http://3g.zdbjq.cn/Article/details/gqijnokiq.sHtML

ANALYZE TABLE users;
来源：http://www.blog.fehbvm.com/Article/details/glkydxthv.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.zdbjq.cn/Article/details/gjsytziup.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.hesvh.cn/Article/details/gydozppnt.sHtML

[Q72] 查看索引
来源：http://3g.hesvh.cn/Article/details/gzvfpasmq.sHtML

SHOW INDEX FROM users;
来源：http://3g.fehbvm.com/Article/details/grshuvnya.sHtML

[Q73] 查看表状态
来源：http://mobile.fehbvm.com/Article/details/gmvvntdxe.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.fehbvm.com/Article/details/grrobkmwi.sHtML

[Q74] 强制使用索引
来源：http://baike.zdbjq.cn/Article/details/gxizzlnsq.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.zdbjq.cn/Article/details/gdpkeuqtj.sHtML

[Q75] 日期格式化
来源：http://mobile.hesvh.cn/Article/details/glyhuuhyq.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gqkqpctxi.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.fehbvm.com/Article/details/gdzcqonzq.sHtML

[Q76] 按天统计
来源：http://m.share.zdbjq.cn/Article/details/gzmammyqb.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.hesvh.cn/Article/details/gszzqqsac.sHtML

[Q77] 时间加减
来源：http://mobile.fehbvm.com/Article/details/genwtevnu.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.zdbjq.cn/Article/details/gfhuubklg.sHtML

[Q78] 当前时间
来源：http://baike.fehbvm.com/Article/details/gosohqjvy.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.fehbvm.com/Article/details/gukysanun.sHtML

[Q79] 字符串拼接
来源：http://blog.zdbjq.cn/Article/details/gzzjficgx.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.zdbjq.cn/Article/details/gbymlyuyi.sHtML

[Q80] 字符串截取
来源：http://blog.hesvh.cn/Article/details/gzzjqouzz.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.hesvh.cn/Article/details/grpmjqnfp.sHtML

[Q81] 字符串替换
来源：http://blog.hesvh.cn/Article/details/gcppwzgng.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.zdbjq.cn/Article/details/gxfysuoqs.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.fehbvm.com/Article/details/gmjovymhm.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/gnxdneozb.sHtML

[Q83] 大小写转换
来源：http://www.blog.zdbjq.cn/Article/details/gorozazkb.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gbrfvnluz.sHtML

[Q84] 去除首尾空格
来源：http://m.share.zdbjq.cn/Article/details/gqqqzoegk.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/guelvdevn.sHtML

[Q85] 数值取整
来源：http://baike.hesvh.cn/Article/details/gjrsbhzyy.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.zdbjq.cn/Article/details/gzwxohzpx.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.hesvh.cn/Article/details/gbcugkewl.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fehbvm.com/Article/details/gdyzcouth.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fehbvm.com/Article/details/gjxnsgkef.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.zdbjq.cn/Article/details/gecfgbdmi.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fehbvm.com/Article/details/gxeaaotob.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.hesvh.cn/Article/details/gdmhhcnmb.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gctlegawd.sHtML

[Q89] 判断表是否存在
来源：http://m.share.zdbjq.cn/Article/details/gvszzxdhb.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.hesvh.cn/Article/details/gikyqneeb.sHtML

[Q90] 生成序号列
来源：http://baike.fehbvm.com/Article/details/gstezxcmt.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.zdbjq.cn/Article/details/grzvoxifn.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gssbckdgg.sHtML

R. Bash 专题
来源：http://read.share.zdbjq.cn/Article/details/gdguedrpy.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gbkqjbyrh.sHtML

[R01] shebang 与严格模式
来源：http://blog.zdbjq.cn/Article/details/gfqnjihvs.sHtML

#!/usr/bin/env bash
来源：http://baike.zdbjq.cn/Article/details/gqgiogdlb.sHtML

set -euo pipefail
来源：http://www.share.zdbjq.cn/Article/details/gkeggbuqr.sHtML

[R02] 变量赋值与使用
来源：http://mobile.hesvh.cn/Article/details/gtyqnjsrq.sHtML

name="Tom"; echo "$name"
来源：http://3g.hesvh.cn/Article/details/gdkjhawra.sHtML

[R03] 只读变量
来源：http://wap.zdbjq.cn/Article/details/govdmbjqx.sHtML

readonly PI=3.14
来源：http://baike.fehbvm.com/Article/details/gtwoucabv.sHtML

[R04] 位置参数
来源：http://www.share.zdbjq.cn/Article/details/gbnbvopmk.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.hesvh.cn/Article/details/gvfxpeusm.sHtML

[R05] 参数默认值
来源：http://www.blog.hesvh.cn/Article/details/ggqnvjqns.sHtML

name="${1:-default}"
来源：http://mobile.hesvh.cn/Article/details/gjzkdrobd.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gnecwhmjm.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/gnygbrmjh.sHtML

[R07] if 判断文件
来源：http://www.m.share.hesvh.cn/Article/details/gmhihugwm.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.zdbjq.cn/Article/details/gjmwwpozg.sHtML

[R08] 数值比较
来源：http://m.share.hesvh.cn/Article/details/gkcesehep.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gquctfdnp.sHtML

[R09] 字符串比较
来源：http://read.share.zdbjq.cn/Article/details/gtcdrewud.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fehbvm.com/Article/details/gpwozyyah.sHtML

[R10] 正则匹配
来源：http://blog.zdbjq.cn/Article/details/guuwfevyo.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.zdbjq.cn/Article/details/gglorojme.sHtML

[R11] case 多分支
来源：http://3g.fehbvm.com/Article/details/gxpjpfwnm.sHtML

case "$1" in
来源：http://www.share.hesvh.cn/Article/details/gowddlcsb.sHtML

start) echo "启动" ;;
来源：http://m.share.hesvh.cn/Article/details/gcpjthema.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fehbvm.com/Article/details/ghbmbjyem.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.zdbjq.cn/Article/details/gqwuytzom.sHtML

esac
来源：http://mobile.hesvh.cn/Article/details/gcxqcjcqe.sHtML

[R12] for 遍历文件
来源：http://www.blog.zdbjq.cn/Article/details/glwsabgtj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.zdbjq.cn/Article/details/ggixrmxbk.sHtML

[R13] for 计数循环
来源：http://baike.fehbvm.com/Article/details/gsaibngjt.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.hesvh.cn/Article/details/gafvultey.sHtML

[R14] C 风格 for
来源：http://baike.zdbjq.cn/Article/details/gprmtszyh.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.hesvh.cn/Article/details/gcruumupw.sHtML

[R15] while 逐行读文件
来源：http://baike.fehbvm.com/Article/details/gvzdwtyqy.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.hesvh.cn/Article/details/glfyhqism.sHtML

[R16] until 等待条件
来源：http://blog.hesvh.cn/Article/details/gqwtlfihs.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/gmxiddvbt.sHtML

[R17] 数组定义与取值
来源：http://www.share.zdbjq.cn/Article/details/gmwkpzejf.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.hesvh.cn/Article/details/gyssalvgo.sHtML

[R18] 遍历数组
来源：http://www.m.share.hesvh.cn/Article/details/gngamzhcc.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fehbvm.com/Article/details/ggqgkpefs.sHtML

[R19] 数组长度
来源：http://mobile.fehbvm.com/Article/details/glcbxmqry.sHtML

echo "${#arr[@]}"
来源：http://www.share.hesvh.cn/Article/details/gwgewmump.sHtML

[R20] 关联数组（字典）
来源：http://read.share.zdbjq.cn/Article/details/gdawttexe.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.hesvh.cn/Article/details/gcrpexacz.sHtML

[R21] 字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/gnuxmbrab.sHtML

echo "${#s}"
来源：http://read.share.zdbjq.cn/Article/details/gfypolnle.sHtML

[R22] 截取子串
来源：http://www.share.hesvh.cn/Article/details/gkmnaehhr.sHtML

echo "${s:0:5}"
来源：http://read.share.hesvh.cn/Article/details/gnmvrhfma.sHtML

[R23] 字符串替换
来源：http://3g.fehbvm.com/Article/details/gxlafifkq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fehbvm.com/Article/details/gdzjmhihn.sHtML

[R24] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/ggexrwxkz.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fehbvm.com/Article/details/gswnugymj.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fehbvm.com/Article/details/gdjrnhekl.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.hesvh.cn/Article/details/grwwomqrr.sHtML

[R26] 命令替换
来源：http://www.blog.fehbvm.com/Article/details/geerwdazt.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.hesvh.cn/Article/details/gfkffhopu.sHtML

[R27] 算术展开
来源：http://wap.zdbjq.cn/Article/details/gyjmikqsm.sHtML

echo $((1 + 2 * 3))
来源：http://3g.hesvh.cn/Article/details/gunukebpg.sHtML

[R28] 浮点运算
来源：http://mobile.fehbvm.com/Article/details/gfewnmile.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.zdbjq.cn/Article/details/gswfcmocy.sHtML

[R29] 定义函数
来源：http://mobile.hesvh.cn/Article/details/gipguotjb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.zdbjq.cn/Article/details/ghmlzpoid.sHtML

[R30] 函数返回状态码
来源：http://read.share.fehbvm.com/Article/details/gjvwcldti.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.hesvh.cn/Article/details/gbylecqqc.sHtML

[R31] 局部变量
来源：http://m.share.fehbvm.com/Article/details/gnvzynfer.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.hesvh.cn/Article/details/gmmpvcyrt.sHtML

[R32] 参数个数校验
来源：http://www.share.fehbvm.com/Article/details/goryagieu.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.hesvh.cn/Article/details/gzrursumj.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.hesvh.cn/Article/details/gzpwxqhrk.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.hesvh.cn/Article/details/ghhsmsddw.sHtML

[R34] 退出时清理
来源：http://baike.hesvh.cn/Article/details/gtojwltot.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/gykgfidzy.sHtML

[R35] 后台执行并等待
来源：http://wap.zdbjq.cn/Article/details/ghvhtiwyb.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.zdbjq.cn/Article/details/gszfjaipq.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.hesvh.cn/Article/details/gwyrlkdqj.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.hesvh.cn/Article/details/gmohdruyc.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.hesvh.cn/Article/details/gwrjrohdx.sHtML

files=$(ls -1)
来源：http://blog.zdbjq.cn/Article/details/gtpzugbfj.sHtML

[R38] 管道串联
来源：http://www.m.share.fehbvm.com/Article/details/gmptptcwv.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.hesvh.cn/Article/details/gipkomusc.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.hesvh.cn/Article/details/goucjupdh.sHtML

cmd > out.log 2>&1
来源：http://m.share.zdbjq.cn/Article/details/gwajzlekx.sHtML

[R40] 追加写日志
来源：http://mobile.zdbjq.cn/Article/details/gwoyqpbzi.sHtML

echo "log" >> out.log
来源：http://blog.zdbjq.cn/Article/details/gdoccwmpx.sHtML

[R41] 丢弃输出
来源：http://www.share.zdbjq.cn/Article/details/gdosbkawv.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.hesvh.cn/Article/details/gxnqgykll.sHtML

[R42] 输入重定向
来源：http://www.m.share.hesvh.cn/Article/details/gsuymmlww.sHtML

wc -l < a.txt
来源：http://baike.hesvh.cn/Article/details/gygbminok.sHtML

[R43] 按名字查找文件
来源：http://read.share.fehbvm.com/Article/details/gvrzumfmi.sHtML

find . -name "*.log" -type f
来源：http://blog.hesvh.cn/Article/details/gaiezbhzr.sHtML

[R44] 按修改时间查找
来源：http://mobile.fehbvm.com/Article/details/gowcpyymx.sHtML

find . -mtime -7 -type f
来源：http://baike.zdbjq.cn/Article/details/gkrvwpuqj.sHtML

[R45] 批量删除
来源：http://www.blog.fehbvm.com/Article/details/gcxwosmoc.sHtML

find . -name "*.tmp" -delete
来源：http://wap.hesvh.cn/Article/details/gtsqnjiko.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fehbvm.com/Article/details/gintbnezf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fehbvm.com/Article/details/gmqnxngcg.sHtML

[R47] sed 单行替换
来源：http://blog.zdbjq.cn/Article/details/gqqldmwdg.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.hesvh.cn/Article/details/gqntaxnof.sHtML

[R48] awk 取指定列
来源：http://read.share.zdbjq.cn/Article/details/gnhvzwojm.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.hesvh.cn/Article/details/ghvxalvee.sHtML

[R49] awk 带条件
来源：http://www.blog.hesvh.cn/Article/details/gkpwxrtjs.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.hesvh.cn/Article/details/gttspjxin.sHtML

[R50] awk 求和
来源：http://mobile.fehbvm.com/Article/details/gdckwhdhk.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.hesvh.cn/Article/details/gehtzevlm.sHtML

[R51] 排序去重取前几
来源：http://3g.fehbvm.com/Article/details/gtvglpshb.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.zdbjq.cn/Article/details/grmdhskmz.sHtML

[R52] 统计行数
来源：http://www.blog.hesvh.cn/Article/details/gfjbxrumn.sHtML

wc -l a.txt
来源：http://www.share.fehbvm.com/Article/details/gjjtpsein.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.zdbjq.cn/Article/details/gatwflkjm.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.hesvh.cn/Article/details/guqmsxscr.sHtML

[R54] 比较两个文件
来源：http://www.m.share.hesvh.cn/Article/details/gbxdswsfr.sHtML

diff a.txt b.txt
来源：http://3g.fehbvm.com/Article/details/ghaidosmg.sHtML

[R55] 压缩与解压
来源：http://blog.fehbvm.com/Article/details/goaowrpsw.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.zdbjq.cn/Article/details/gtywqdqgx.sHtML

[R56] 远程拷贝
来源：http://read.share.fehbvm.com/Article/details/guufqjqam.sHtML

scp file user@host:/path/
来源：http://read.share.fehbvm.com/Article/details/gebfcodtr.sHtML

[R57] 远程执行命令
来源：http://baike.hesvh.cn/Article/details/gjualwbgk.sHtML

ssh user@host 'uptime'
来源：http://mobile.hesvh.cn/Article/details/gmadlovmh.sHtML

[R58] 下载文件
来源：http://3g.zdbjq.cn/Article/details/gjgiteqrv.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fehbvm.com/Article/details/gvvhifxyb.sHtML

[R59] 发 POST JSON
来源：http://www.blog.zdbjq.cn/Article/details/gdqfyuunx.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fehbvm.com/Article/details/gdipflndh.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fehbvm.com/Article/details/gaabmjktr.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.zdbjq.cn/Article/details/gjbxrmevq.sHtML

[R61] 磁盘占用
来源：http://baike.fehbvm.com/Article/details/gxzffneiq.sHtML

df -h;  du -sh *
来源：http://mobile.fehbvm.com/Article/details/gjkyycxqy.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fehbvm.com/Article/details/gnqvfwbag.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.zdbjq.cn/Article/details/gfpzwupeb.sHtML

[R63] 内存与进程
来源：http://www.share.fehbvm.com/Article/details/gdrevehbk.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.hesvh.cn/Article/details/gvgrecqbn.sHtML

[R64] 结束进程
来源：http://wap.zdbjq.cn/Article/details/gxmoxzxty.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.zdbjq.cn/Article/details/gaeouijsp.sHtML

[R65] 查看端口占用
来源：http://mobile.fehbvm.com/Article/details/gboogpmwp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.zdbjq.cn/Article/details/gobqcyqah.sHtML

[R66] 定时任务
来源：http://3g.hesvh.cn/Article/details/gsyfdvhhs.sHtML

crontab -e;  crontab -l
来源：http://mobile.zdbjq.cn/Article/details/gbpuphvwd.sHtML

[R67] 生成随机十六进制串
来源：http://baike.hesvh.cn/Article/details/geakqzqvu.sHtML

openssl rand -hex 16
来源：http://blog.hesvh.cn/Article/details/galdxixab.sHtML

[R68] 计算文件校验值
来源：http://read.share.hesvh.cn/Article/details/gifdxkoyg.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fehbvm.com/Article/details/girbjdfet.sHtML

[R69] 生成随机密码
来源：http://www.m.share.zdbjq.cn/Article/details/gpebxfczt.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.zdbjq.cn/Article/details/gmzvpbktz.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fehbvm.com/Article/details/gwqfphrmd.sHtML

date +%s;  date -d @1700000000
来源：http://3g.hesvh.cn/Article/details/gqayogcfs.sHtML

[R71] 日期格式化
来源：http://read.share.zdbjq.cn/Article/details/ggailmtel.sHtML


<!-- 参考信息 -->