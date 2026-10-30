代发 wailian999

SELECT * FROM users WHERE email IS NULL;
来源：http://3g.fehbvm.com/Article/details/gbmajzuig.sHtML

[Q22] 排序
来源：http://m.share.zdbjq.cn/Article/details/guxwlvyxb.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://wap.hesvh.cn/Article/details/gruhyazjr.sHtML

[Q23] 分页
来源：http://baike.fehbvm.com/Article/details/gdvwsngul.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.hesvh.cn/Article/details/gcgpogqma.sHtML

[Q24] 去重
来源：http://www.m.share.hesvh.cn/Article/details/gzrxzelxz.sHtML

SELECT DISTINCT city FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gmkhykaky.sHtML

[Q25] 只取前 N 条
来源：http://baike.zdbjq.cn/Article/details/gxyjydqlc.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.hesvh.cn/Article/details/gqnwnybbi.sHtML

[Q26] 计数
来源：http://read.share.hesvh.cn/Article/details/glsqoqaud.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gvfbkgrdh.sHtML

[Q27] 条件计数
来源：http://blog.fehbvm.com/Article/details/gqxwxietg.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.zdbjq.cn/Article/details/glfizmeop.sHtML

[Q28] 求和与平均
来源：http://m.share.fehbvm.com/Article/details/grmcgkdul.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gfyglfbli.sHtML

[Q29] 最大最小值
来源：http://baike.zdbjq.cn/Article/details/gspgohszj.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/ghsfraszj.sHtML

[Q30] 分组统计
来源：http://mobile.zdbjq.cn/Article/details/gkeplbtbf.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/gakrdpbau.sHtML

[Q31] 分组后过滤
来源：http://wap.fehbvm.com/Article/details/gxqlwghnk.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.fehbvm.com/Article/details/gwtkphkdb.sHtML

[Q32] 分组拼接字符串
来源：http://baike.zdbjq.cn/Article/details/ghsldikmv.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gdmzlprvd.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.fehbvm.com/Article/details/ggqghopgp.sHtML

[Q33] 多列分组
来源：http://m.share.hesvh.cn/Article/details/gnbkdaabj.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.zdbjq.cn/Article/details/gstmnucno.sHtML

[Q34] 每组取第一条
来源：http://baike.hesvh.cn/Article/details/guxmhnfeu.sHtML

SELECT * FROM (
来源：http://www.m.share.hesvh.cn/Article/details/gpbfhuall.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.zdbjq.cn/Article/details/ggyyysdmq.sHtML

) t WHERE rn = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gdiukgpjj.sHtML

[Q35] 内连接
来源：http://3g.hesvh.cn/Article/details/gkwymvywk.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gdiyakini.sHtML

[Q36] 左连接
来源：http://www.share.hesvh.cn/Article/details/gxzvesxlt.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.fehbvm.com/Article/details/guyndhvop.sHtML

[Q37] 右连接
来源：http://read.share.zdbjq.cn/Article/details/gmvgregfe.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.zdbjq.cn/Article/details/gjmnfpwyh.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.fehbvm.com/Article/details/guooasvmu.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.hesvh.cn/Article/details/gevohqryo.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.hesvh.cn/Article/details/gkahzxomf.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.hesvh.cn/Article/details/gfooiolcx.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.zdbjq.cn/Article/details/gjsgxfzfg.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.zdbjq.cn/Article/details/gsppgibsz.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.zdbjq.cn/Article/details/gpdxkynuz.sHtML

[Q41] 多表连接
来源：http://baike.fehbvm.com/Article/details/gdaevehiq.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.zdbjq.cn/Article/details/gbbdgtvuk.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.fehbvm.com/Article/details/ghbkbjaej.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.zdbjq.cn/Article/details/gowkduinm.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.fehbvm.com/Article/details/gsolswuig.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.hesvh.cn/Article/details/gabkrwdts.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.zdbjq.cn/Article/details/gyrparojl.sHtML

[Q43] 标量子查询
来源：http://mobile.zdbjq.cn/Article/details/glwtwxvsg.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.hesvh.cn/Article/details/gixtalwgx.sHtML

[Q44] IN 子查询
来源：http://blog.hesvh.cn/Article/details/gasgvajmr.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.zdbjq.cn/Article/details/gumbcbutm.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.hesvh.cn/Article/details/gwclevxmd.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.hesvh.cn/Article/details/gedtauvoe.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.hesvh.cn/Article/details/gjlehrwet.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.hesvh.cn/Article/details/gyrbozjev.sHtML

[Q47] 与平均值比较
来源：http://3g.hesvh.cn/Article/details/gacoilzgc.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.fehbvm.com/Article/details/gubfghabd.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.hesvh.cn/Article/details/gaxoevpcv.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.zdbjq.cn/Article/details/gwuebviho.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.zdbjq.cn/Article/details/gyicsrpay.sHtML

[Q49] 更新单行
来源：http://3g.fehbvm.com/Article/details/giknfqhzd.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.hesvh.cn/Article/details/gnyxznwfk.sHtML

[Q50] 批量更新
来源：http://www.blog.fehbvm.com/Article/details/gcsfcjcpg.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.fehbvm.com/Article/details/gvznhlqkh.sHtML

[Q51] 用子查询更新
来源：http://baike.fehbvm.com/Article/details/giyitshdk.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.zdbjq.cn/Article/details/gwpgshrpl.sHtML

[Q52] 删除指定行
来源：http://blog.hesvh.cn/Article/details/glqjlcwcj.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.zdbjq.cn/Article/details/gnakgsuje.sHtML

[Q53] 按条件删除
来源：http://wap.fehbvm.com/Article/details/gqdlpwxqj.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.hesvh.cn/Article/details/gsvxawcaq.sHtML

[Q54] 清空表
来源：http://read.share.hesvh.cn/Article/details/gbfocbveh.sHtML

TRUNCATE TABLE logs;
来源：http://wap.hesvh.cn/Article/details/gujfhgwjo.sHtML

[Q55] 排名（并列占位）
来源：http://3g.hesvh.cn/Article/details/gfuscbohh.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.zdbjq.cn/Article/details/grgiuojos.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.fehbvm.com/Article/details/gxyzydjyi.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.hesvh.cn/Article/details/glmcyeelw.sHtML

[Q57] 行号
来源：http://wap.fehbvm.com/Article/details/glfebcgfp.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.hesvh.cn/Article/details/gfuchfamh.sHtML

[Q58] 累计求和
来源：http://baike.zdbjq.cn/Article/details/geehdavtr.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.fehbvm.com/Article/details/gdkvpoozi.sHtML

[Q59] 分组内累计
来源：http://3g.fehbvm.com/Article/details/gafgjzcqd.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/girjpirng.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.hesvh.cn/Article/details/gzryannbe.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fehbvm.com/Article/details/gmeesdvfu.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gohbuqiqw.sHtML

[Q61] 移动平均
来源：http://www.share.fehbvm.com/Article/details/ggfxjeois.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gmjrdjxyn.sHtML

[Q62] 分组占比
来源：http://mobile.zdbjq.cn/Article/details/gwspfjwfc.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gsscpptbn.sHtML

[Q63] 开启事务
来源：http://www.blog.zdbjq.cn/Article/details/gdcbepdkc.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.zdbjq.cn/Article/details/gbqbhpzgk.sHtML

[Q64] 提交事务
来源：http://blog.fehbvm.com/Article/details/gsabwllnk.sHtML

COMMIT;
来源：http://3g.zdbjq.cn/Article/details/griwjmpth.sHtML

[Q65] 回滚事务
来源：http://wap.zdbjq.cn/Article/details/gjebhseqn.sHtML

ROLLBACK;
来源：http://blog.fehbvm.com/Article/details/ggthsitbm.sHtML

[Q66] 行锁查询
来源：http://read.share.fehbvm.com/Article/details/gusksagbt.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.hesvh.cn/Article/details/gzxoqzwpt.sHtML

[Q67] 设置隔离级别
来源：http://wap.fehbvm.com/Article/details/gndvifdnz.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.zdbjq.cn/Article/details/gdgdwkpuc.sHtML

[Q68] 保存点
来源：http://www.share.fehbvm.com/Article/details/getwlelnr.sHtML

SAVEPOINT sp1;
来源：http://3g.hesvh.cn/Article/details/gtzkirxiz.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.hesvh.cn/Article/details/gcvqdpezv.sHtML

[Q69] 查看执行计划
来源：http://wap.zdbjq.cn/Article/details/gqonygjrq.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.hesvh.cn/Article/details/gpovbbovw.sHtML

[Q70] 更新统计信息
来源：http://blog.zdbjq.cn/Article/details/giirhrcat.sHtML

ANALYZE TABLE users;
来源：http://www.blog.fehbvm.com/Article/details/gmycnhmof.sHtML

[Q71] 查看建表语句
来源：http://3g.fehbvm.com/Article/details/gnxebjtoz.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.zdbjq.cn/Article/details/gfgjrlxxw.sHtML

[Q72] 查看索引
来源：http://www.share.fehbvm.com/Article/details/gxrvqsego.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fehbvm.com/Article/details/gzlfnftvn.sHtML

[Q73] 查看表状态
来源：http://www.share.zdbjq.cn/Article/details/gmxhjfbly.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.zdbjq.cn/Article/details/galginrnw.sHtML

[Q74] 强制使用索引
来源：http://blog.zdbjq.cn/Article/details/gvibhiajj.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.hesvh.cn/Article/details/gzhehvhpq.sHtML

[Q75] 日期格式化
来源：http://wap.zdbjq.cn/Article/details/gcdwcrrbs.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.zdbjq.cn/Article/details/ghcovrcys.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.hesvh.cn/Article/details/gqdjjdbpf.sHtML

[Q76] 按天统计
来源：http://read.share.hesvh.cn/Article/details/gnrqhpupg.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.hesvh.cn/Article/details/gmelmyglp.sHtML

[Q77] 时间加减
来源：http://baike.hesvh.cn/Article/details/ggvvfrswh.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fehbvm.com/Article/details/gnpwhapdd.sHtML

[Q78] 当前时间
来源：http://read.share.fehbvm.com/Article/details/gfrzojnak.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.hesvh.cn/Article/details/grabmhxpz.sHtML

[Q79] 字符串拼接
来源：http://www.blog.fehbvm.com/Article/details/gxzxftakw.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fehbvm.com/Article/details/gqwoyvaks.sHtML

[Q80] 字符串截取
来源：http://3g.zdbjq.cn/Article/details/gdbzxoukk.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gkemjcxsa.sHtML

[Q81] 字符串替换
来源：http://wap.zdbjq.cn/Article/details/gofkttfap.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fehbvm.com/Article/details/gjbvulzks.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.fehbvm.com/Article/details/ghestnkap.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gyxyvouij.sHtML

[Q83] 大小写转换
来源：http://read.share.hesvh.cn/Article/details/gcdfcaspc.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gvbntbvzl.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fehbvm.com/Article/details/gcwmzhttc.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gaznepcwp.sHtML

[Q85] 数值取整
来源：http://wap.fehbvm.com/Article/details/gmjypoivn.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fehbvm.com/Article/details/gmncftxnu.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.zdbjq.cn/Article/details/grkmzxyog.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fehbvm.com/Article/details/ggkzvzcye.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.fehbvm.com/Article/details/gtzxllwhr.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.zdbjq.cn/Article/details/gmktuqylz.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.hesvh.cn/Article/details/gefrtxizb.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fehbvm.com/Article/details/gkhvgcxxs.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://m.share.fehbvm.com/Article/details/gxlkxexfu.sHtML

[Q89] 判断表是否存在
来源：http://m.share.zdbjq.cn/Article/details/gtwbrupcv.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fehbvm.com/Article/details/gexcoaqln.sHtML

[Q90] 生成序号列
来源：http://read.share.fehbvm.com/Article/details/gwzgpfhhc.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.fehbvm.com/Article/details/guqhsxwzu.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gtxztdhel.sHtML

R. Bash 专题
来源：http://mobile.hesvh.cn/Article/details/goecnbjhi.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gbttbafes.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.zdbjq.cn/Article/details/gzuykzagg.sHtML

#!/usr/bin/env bash
来源：http://mobile.fehbvm.com/Article/details/gvsiswbea.sHtML

set -euo pipefail
来源：http://mobile.zdbjq.cn/Article/details/gevddbxgx.sHtML

[R02] 变量赋值与使用
来源：http://wap.hesvh.cn/Article/details/gapcvgrhn.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.fehbvm.com/Article/details/ggavolotl.sHtML

[R03] 只读变量
来源：http://wap.zdbjq.cn/Article/details/gtjvfxfuk.sHtML

readonly PI=3.14
来源：http://3g.hesvh.cn/Article/details/glhfwdyog.sHtML

[R04] 位置参数
来源：http://3g.zdbjq.cn/Article/details/gapmwewfh.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.zdbjq.cn/Article/details/gucrjmnti.sHtML

[R05] 参数默认值
来源：http://www.share.fehbvm.com/Article/details/gdwzywlyc.sHtML

name="${1:-default}"
来源：http://blog.zdbjq.cn/Article/details/ghsbtjfjw.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.hesvh.cn/Article/details/gizkryxki.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.hesvh.cn/Article/details/gnibtexbo.sHtML

[R07] if 判断文件
来源：http://read.share.fehbvm.com/Article/details/gczspipxt.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.hesvh.cn/Article/details/gtqoltsft.sHtML

[R08] 数值比较
来源：http://mobile.hesvh.cn/Article/details/gldhfjuyd.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gcprvrbug.sHtML

[R09] 字符串比较
来源：http://www.share.zdbjq.cn/Article/details/gkpqqylck.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.zdbjq.cn/Article/details/gyiibtupv.sHtML

[R10] 正则匹配
来源：http://www.share.zdbjq.cn/Article/details/gmdawzyyd.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.hesvh.cn/Article/details/gwwnzaqoy.sHtML

[R11] case 多分支
来源：http://baike.zdbjq.cn/Article/details/gceegujhn.sHtML

case "$1" in
来源：http://read.share.zdbjq.cn/Article/details/glgwidfwr.sHtML

start) echo "启动" ;;
来源：http://www.share.zdbjq.cn/Article/details/gvhwmbgxz.sHtML

stop)  echo "停止" ;;
来源：http://baike.fehbvm.com/Article/details/gzvfxukgm.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.hesvh.cn/Article/details/girszerhf.sHtML

esac
来源：http://wap.fehbvm.com/Article/details/gtxuegebg.sHtML

[R12] for 遍历文件
来源：http://read.share.zdbjq.cn/Article/details/gvltpcrbw.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.zdbjq.cn/Article/details/gyvqveftq.sHtML

[R13] for 计数循环
来源：http://www.m.share.fehbvm.com/Article/details/gadgczvth.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fehbvm.com/Article/details/gmakspdne.sHtML

[R14] C 风格 for
来源：http://m.share.fehbvm.com/Article/details/gcybndapl.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gspfyjdwg.sHtML

[R15] while 逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gfmeaddyh.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.zdbjq.cn/Article/details/gcxzxgmgm.sHtML

[R16] until 等待条件
来源：http://3g.hesvh.cn/Article/details/gynhvxngj.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.hesvh.cn/Article/details/gpbbnpknc.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.hesvh.cn/Article/details/gphjcerun.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fehbvm.com/Article/details/goykvvebd.sHtML

[R18] 遍历数组
来源：http://www.m.share.fehbvm.com/Article/details/gjenhfiks.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.hesvh.cn/Article/details/gqtrcvmqt.sHtML

[R19] 数组长度
来源：http://wap.zdbjq.cn/Article/details/gejwtfyyu.sHtML

echo "${#arr[@]}"
来源：http://3g.zdbjq.cn/Article/details/gadbzzrjg.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fehbvm.com/Article/details/ginszzggr.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.hesvh.cn/Article/details/gurdemdbb.sHtML

[R21] 字符串长度
来源：http://wap.fehbvm.com/Article/details/gujgbhuyw.sHtML

echo "${#s}"
来源：http://mobile.hesvh.cn/Article/details/gcfubcdpr.sHtML

[R22] 截取子串
来源：http://www.m.share.hesvh.cn/Article/details/gskfdughd.sHtML

echo "${s:0:5}"
来源：http://www.m.share.hesvh.cn/Article/details/ggximytch.sHtML

[R23] 字符串替换
来源：http://baike.zdbjq.cn/Article/details/gdmxmgvzg.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fehbvm.com/Article/details/gphtcxiam.sHtML

[R24] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/gvtanlitv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fehbvm.com/Article/details/gfwilwigk.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.zdbjq.cn/Article/details/grsxrrnad.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.zdbjq.cn/Article/details/gglooovaz.sHtML

[R26] 命令替换
来源：http://m.share.fehbvm.com/Article/details/gcrilmszc.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.zdbjq.cn/Article/details/gzlhalnot.sHtML

[R27] 算术展开
来源：http://baike.zdbjq.cn/Article/details/gqlwyblqx.sHtML

echo $((1 + 2 * 3))
来源：http://3g.zdbjq.cn/Article/details/gvbqndzuu.sHtML

[R28] 浮点运算
来源：http://wap.hesvh.cn/Article/details/gqumpqubw.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fehbvm.com/Article/details/gekqbeqdg.sHtML

[R29] 定义函数
来源：http://baike.zdbjq.cn/Article/details/gbzgnkuqa.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fehbvm.com/Article/details/ghkckzcrm.sHtML

[R30] 函数返回状态码
来源：http://m.share.hesvh.cn/Article/details/gpexxfdfu.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fehbvm.com/Article/details/ghydvaauy.sHtML

[R31] 局部变量
来源：http://wap.fehbvm.com/Article/details/gfzpyniyx.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fehbvm.com/Article/details/gjrnpkqoj.sHtML

[R32] 参数个数校验
来源：http://baike.zdbjq.cn/Article/details/gpxbwoqag.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fehbvm.com/Article/details/gvbmxbqpf.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.zdbjq.cn/Article/details/gqelbcsrm.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.hesvh.cn/Article/details/gsbpnutbk.sHtML

[R34] 退出时清理
来源：http://3g.hesvh.cn/Article/details/gagqdkout.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/gqcrdvlue.sHtML

[R35] 后台执行并等待
来源：http://blog.fehbvm.com/Article/details/ggshfzeox.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.hesvh.cn/Article/details/gzuerfbhi.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fehbvm.com/Article/details/gewighkte.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.zdbjq.cn/Article/details/gmtkiprlb.sHtML

[R37] 把输出赋给变量
来源：http://mobile.hesvh.cn/Article/details/ghyurlknw.sHtML

files=$(ls -1)
来源：http://m.share.hesvh.cn/Article/details/gqwrefncx.sHtML

[R38] 管道串联
来源：http://blog.hesvh.cn/Article/details/gqakycygi.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.hesvh.cn/Article/details/gooifgjxc.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.zdbjq.cn/Article/details/gqfqbphhe.sHtML

cmd > out.log 2>&1
来源：http://read.share.zdbjq.cn/Article/details/ghmzfmbuw.sHtML

[R40] 追加写日志
来源：http://wap.fehbvm.com/Article/details/gekmmheba.sHtML

echo "log" >> out.log
来源：http://3g.zdbjq.cn/Article/details/gwrjndifa.sHtML

[R41] 丢弃输出
来源：http://mobile.zdbjq.cn/Article/details/gceyjohzg.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.zdbjq.cn/Article/details/gqoehsyyf.sHtML

[R42] 输入重定向
来源：http://baike.zdbjq.cn/Article/details/gteayjbjt.sHtML

wc -l < a.txt
来源：http://www.share.hesvh.cn/Article/details/glnvnpzzx.sHtML

[R43] 按名字查找文件
来源：http://blog.hesvh.cn/Article/details/gqiiipsnb.sHtML

find . -name "*.log" -type f
来源：http://blog.fehbvm.com/Article/details/gxqzzddfb.sHtML

[R44] 按修改时间查找
来源：http://m.share.fehbvm.com/Article/details/gnletglkr.sHtML

find . -mtime -7 -type f
来源：http://read.share.hesvh.cn/Article/details/gcdhbzstt.sHtML

[R45] 批量删除
来源：http://blog.hesvh.cn/Article/details/gphbclmso.sHtML

find . -name "*.tmp" -delete
来源：http://blog.zdbjq.cn/Article/details/gorxeirjb.sHtML

[R46] 递归替换文件内容
来源：http://mobile.hesvh.cn/Article/details/garmuwyzi.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.hesvh.cn/Article/details/gqlqnqqew.sHtML

[R47] sed 单行替换
来源：http://www.blog.zdbjq.cn/Article/details/gprhlsipe.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fehbvm.com/Article/details/grkpwpvvm.sHtML

[R48] awk 取指定列
来源：http://baike.hesvh.cn/Article/details/gfyessrsz.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.hesvh.cn/Article/details/gfzmcpmee.sHtML

[R49] awk 带条件
来源：http://read.share.fehbvm.com/Article/details/ggkyulklk.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.hesvh.cn/Article/details/ggvatfukv.sHtML

[R50] awk 求和
来源：http://blog.zdbjq.cn/Article/details/gwlxujeyi.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.hesvh.cn/Article/details/gpmoyzuyd.sHtML

[R51] 排序去重取前几
来源：http://www.share.zdbjq.cn/Article/details/gswzweudt.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.hesvh.cn/Article/details/ggifqszid.sHtML

[R52] 统计行数
来源：http://read.share.zdbjq.cn/Article/details/geckpvejc.sHtML

wc -l a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gqfplxtpa.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.hesvh.cn/Article/details/gidzpupya.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.zdbjq.cn/Article/details/gugqrujio.sHtML

[R54] 比较两个文件
来源：http://3g.fehbvm.com/Article/details/gmtencozc.sHtML

diff a.txt b.txt
来源：http://baike.fehbvm.com/Article/details/gcewmgudz.sHtML

[R55] 压缩与解压
来源：http://baike.zdbjq.cn/Article/details/gsztgirbt.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.zdbjq.cn/Article/details/gxmbpkeko.sHtML

[R56] 远程拷贝
来源：http://wap.fehbvm.com/Article/details/gveilhden.sHtML

scp file user@host:/path/
来源：http://m.share.hesvh.cn/Article/details/gzdybsran.sHtML

[R57] 远程执行命令
来源：http://3g.fehbvm.com/Article/details/geicuebor.sHtML

ssh user@host 'uptime'
来源：http://mobile.zdbjq.cn/Article/details/gqvzkevan.sHtML

[R58] 下载文件
来源：http://blog.fehbvm.com/Article/details/gatdzcbal.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.hesvh.cn/Article/details/ggeplveyh.sHtML

[R59] 发 POST JSON
来源：http://www.share.zdbjq.cn/Article/details/guszbpqpl.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.zdbjq.cn/Article/details/gwmcuvqqs.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.zdbjq.cn/Article/details/grexrsugb.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.hesvh.cn/Article/details/gbrfvshvo.sHtML

[R61] 磁盘占用
来源：http://www.blog.zdbjq.cn/Article/details/gdieudypo.sHtML

df -h;  du -sh *
来源：http://mobile.fehbvm.com/Article/details/gfhniucwd.sHtML

[R62] 找最占空间的文件
来源：http://read.share.zdbjq.cn/Article/details/ghvssumdb.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.hesvh.cn/Article/details/ghytvyvtm.sHtML

[R63] 内存与进程
来源：http://3g.fehbvm.com/Article/details/gljyypmmo.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fehbvm.com/Article/details/gbwuikiwo.sHtML

[R64] 结束进程
来源：http://m.share.fehbvm.com/Article/details/gxwcswtfv.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fehbvm.com/Article/details/getzoalqk.sHtML

[R65] 查看端口占用
来源：http://wap.fehbvm.com/Article/details/ghcusykol.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.hesvh.cn/Article/details/gjkflynmt.sHtML

[R66] 定时任务
来源：http://www.blog.zdbjq.cn/Article/details/gwgiforyc.sHtML

crontab -e;  crontab -l
来源：http://m.share.fehbvm.com/Article/details/gtmtzvyeh.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.hesvh.cn/Article/details/ggmudgebt.sHtML

openssl rand -hex 16
来源：http://read.share.hesvh.cn/Article/details/gwszalmnk.sHtML

[R68] 计算文件校验值
来源：http://mobile.fehbvm.com/Article/details/gdmfvyefp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.hesvh.cn/Article/details/gnstrkdma.sHtML

[R69] 生成随机密码
来源：http://www.share.zdbjq.cn/Article/details/gubaudpuk.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.zdbjq.cn/Article/details/gdkjjssbk.sHtML

[R70] 时间戳与互转
来源：http://blog.fehbvm.com/Article/details/gvqmqpwic.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fehbvm.com/Article/details/gjnizejsr.sHtML

[R71] 日期格式化
来源：http://3g.fehbvm.com/Article/details/gcgfkncur.sHtML


<!-- 参考信息 -->