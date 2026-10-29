代发 wailian999

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.zdbjq.cn/Article/details/gmwjlerpt.sHtML

[Q22] 排序
来源：http://mobile.zdbjq.cn/Article/details/ggibkmnao.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.fehbvm.com/Article/details/gejjlfmsf.sHtML

[Q23] 分页
来源：http://www.share.zdbjq.cn/Article/details/gluspqrpv.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.fehbvm.com/Article/details/gxjtzvawu.sHtML

[Q24] 去重
来源：http://3g.fehbvm.com/Article/details/gphjnwbcv.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.zdbjq.cn/Article/details/grxmvxgrc.sHtML

[Q25] 只取前 N 条
来源：http://read.share.zdbjq.cn/Article/details/gprvcizus.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.hesvh.cn/Article/details/gefcaitui.sHtML

[Q26] 计数
来源：http://www.share.fehbvm.com/Article/details/gfieydyie.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gdmyktyqa.sHtML

[Q27] 条件计数
来源：http://baike.zdbjq.cn/Article/details/gelzlupng.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.fehbvm.com/Article/details/guxawtqcb.sHtML

[Q28] 求和与平均
来源：http://3g.hesvh.cn/Article/details/ghnuzmbar.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.fehbvm.com/Article/details/gwctbqgoa.sHtML

[Q29] 最大最小值
来源：http://3g.hesvh.cn/Article/details/gyjtryqge.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gepndxjks.sHtML

[Q30] 分组统计
来源：http://wap.hesvh.cn/Article/details/gsysfslfr.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.hesvh.cn/Article/details/gtnzggqea.sHtML

[Q31] 分组后过滤
来源：http://www.blog.zdbjq.cn/Article/details/gzexyktec.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.hesvh.cn/Article/details/grzdxdrat.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.zdbjq.cn/Article/details/gmibjeipa.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.zdbjq.cn/Article/details/gjoaojhqo.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.hesvh.cn/Article/details/gbbnburct.sHtML

[Q33] 多列分组
来源：http://www.m.share.hesvh.cn/Article/details/gfubrdkqm.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.zdbjq.cn/Article/details/gbpyjvzni.sHtML

[Q34] 每组取第一条
来源：http://3g.zdbjq.cn/Article/details/gdkdxxupg.sHtML

SELECT * FROM (
来源：http://wap.fehbvm.com/Article/details/gckgvcoiz.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.fehbvm.com/Article/details/gxnyvmxcr.sHtML

) t WHERE rn = 1;
来源：http://blog.hesvh.cn/Article/details/gzrynhyxy.sHtML

[Q35] 内连接
来源：http://3g.fehbvm.com/Article/details/gsqneezzl.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.hesvh.cn/Article/details/gufeautod.sHtML

[Q36] 左连接
来源：http://wap.fehbvm.com/Article/details/gnttpajvp.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fehbvm.com/Article/details/glgfjknwq.sHtML

[Q37] 右连接
来源：http://baike.zdbjq.cn/Article/details/gjbxgfrvb.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.fehbvm.com/Article/details/gqmoxrayz.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.hesvh.cn/Article/details/gjftgrxhn.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.fehbvm.com/Article/details/gkgciftqp.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.fehbvm.com/Article/details/giibsgcqr.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.zdbjq.cn/Article/details/gskxidxbt.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.fehbvm.com/Article/details/grycpdyig.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.zdbjq.cn/Article/details/gtupktmxn.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.hesvh.cn/Article/details/gatefhaua.sHtML

[Q41] 多表连接
来源：http://www.m.share.fehbvm.com/Article/details/godivdxhc.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.fehbvm.com/Article/details/goipoihjn.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.hesvh.cn/Article/details/glisnutjc.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.zdbjq.cn/Article/details/grxwdchzc.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.fehbvm.com/Article/details/ggghihzrg.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.zdbjq.cn/Article/details/gsalpscwe.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.hesvh.cn/Article/details/glspxpdts.sHtML

[Q43] 标量子查询
来源：http://blog.fehbvm.com/Article/details/gjboxinit.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.fehbvm.com/Article/details/gqjdqmmsd.sHtML

[Q44] IN 子查询
来源：http://blog.fehbvm.com/Article/details/gjwehehxc.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.hesvh.cn/Article/details/gvybcvjrg.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.fehbvm.com/Article/details/gjylanuht.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.hesvh.cn/Article/details/ggydkfutf.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.fehbvm.com/Article/details/gjfowzcpa.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.hesvh.cn/Article/details/gijuwroqe.sHtML

[Q47] 与平均值比较
来源：http://www.blog.hesvh.cn/Article/details/gdbytiuaq.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.hesvh.cn/Article/details/gpwebcbnp.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.zdbjq.cn/Article/details/gkmllvdbn.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.zdbjq.cn/Article/details/ggozcwuge.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.zdbjq.cn/Article/details/gnzlrssne.sHtML

[Q49] 更新单行
来源：http://3g.hesvh.cn/Article/details/gwsirexth.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.fehbvm.com/Article/details/gbbsrujcb.sHtML

[Q50] 批量更新
来源：http://wap.hesvh.cn/Article/details/gbmqpugxm.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.fehbvm.com/Article/details/gurrmcqkn.sHtML

[Q51] 用子查询更新
来源：http://wap.zdbjq.cn/Article/details/grnvvejov.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.zdbjq.cn/Article/details/gxvuiqwuc.sHtML

[Q52] 删除指定行
来源：http://3g.hesvh.cn/Article/details/gxbtpursd.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.zdbjq.cn/Article/details/gbejelbsz.sHtML

[Q53] 按条件删除
来源：http://www.m.share.hesvh.cn/Article/details/gioxoekqs.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.zdbjq.cn/Article/details/gwwsgxmsm.sHtML

[Q54] 清空表
来源：http://wap.zdbjq.cn/Article/details/gtwtkyomh.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.zdbjq.cn/Article/details/goolmenmw.sHtML

[Q55] 排名（并列占位）
来源：http://wap.fehbvm.com/Article/details/gytzugown.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.hesvh.cn/Article/details/gwvsyhfhf.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.fehbvm.com/Article/details/gkdvnyspz.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.zdbjq.cn/Article/details/gpdswkhzv.sHtML

[Q57] 行号
来源：http://m.share.hesvh.cn/Article/details/gzorcfhwm.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gldjlixfa.sHtML

[Q58] 累计求和
来源：http://wap.hesvh.cn/Article/details/gdrjdhraw.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gsvhycfhm.sHtML

[Q59] 分组内累计
来源：http://www.blog.zdbjq.cn/Article/details/ggscafhsw.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gqmhisitl.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.fehbvm.com/Article/details/gfacuitvm.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.zdbjq.cn/Article/details/gfougeuno.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fehbvm.com/Article/details/gnkeepjum.sHtML

[Q61] 移动平均
来源：http://read.share.hesvh.cn/Article/details/gsbofplon.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gyoliyeiv.sHtML

[Q62] 分组占比
来源：http://read.share.hesvh.cn/Article/details/gvoyjkoae.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/gxxlqgvra.sHtML

[Q63] 开启事务
来源：http://wap.fehbvm.com/Article/details/glavwrsoa.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.fehbvm.com/Article/details/ghaqaexfc.sHtML

[Q64] 提交事务
来源：http://3g.hesvh.cn/Article/details/gxotqxiko.sHtML

COMMIT;
来源：http://www.share.zdbjq.cn/Article/details/gdqqiovzp.sHtML

[Q65] 回滚事务
来源：http://wap.hesvh.cn/Article/details/gmzxvcbzk.sHtML

ROLLBACK;
来源：http://blog.zdbjq.cn/Article/details/gqiwegbai.sHtML

[Q66] 行锁查询
来源：http://www.m.share.fehbvm.com/Article/details/gnddxiefo.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.hesvh.cn/Article/details/gzqetyeyk.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.hesvh.cn/Article/details/gdbztrjls.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.zdbjq.cn/Article/details/gxcndzezg.sHtML

[Q68] 保存点
来源：http://read.share.zdbjq.cn/Article/details/gihrerwfw.sHtML

SAVEPOINT sp1;
来源：http://www.share.fehbvm.com/Article/details/gkprxzuvp.sHtML

ROLLBACK TO sp1;
来源：http://m.share.zdbjq.cn/Article/details/grnjuxnvk.sHtML

[Q69] 查看执行计划
来源：http://baike.zdbjq.cn/Article/details/gutdzdahj.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.fehbvm.com/Article/details/gybjpclzc.sHtML

[Q70] 更新统计信息
来源：http://www.share.zdbjq.cn/Article/details/ganxhlkna.sHtML

ANALYZE TABLE users;
来源：http://blog.fehbvm.com/Article/details/gpdkzbbiv.sHtML

[Q71] 查看建表语句
来源：http://www.share.zdbjq.cn/Article/details/gukzuyfwk.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.hesvh.cn/Article/details/gnnyjdeqi.sHtML

[Q72] 查看索引
来源：http://mobile.hesvh.cn/Article/details/gqilqvfie.sHtML

SHOW INDEX FROM users;
来源：http://blog.fehbvm.com/Article/details/gtykgkpfo.sHtML

[Q73] 查看表状态
来源：http://read.share.fehbvm.com/Article/details/gekqqulvw.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.zdbjq.cn/Article/details/gbylszpms.sHtML

[Q74] 强制使用索引
来源：http://blog.hesvh.cn/Article/details/gparfacda.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.hesvh.cn/Article/details/gmogczgdn.sHtML

[Q75] 日期格式化
来源：http://read.share.zdbjq.cn/Article/details/gjiligmir.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.fehbvm.com/Article/details/ghytfiame.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.hesvh.cn/Article/details/gsjpjqeit.sHtML

[Q76] 按天统计
来源：http://www.m.share.fehbvm.com/Article/details/grguemeru.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fehbvm.com/Article/details/gosexkbuf.sHtML

[Q77] 时间加减
来源：http://baike.hesvh.cn/Article/details/gnnrpynbb.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.zdbjq.cn/Article/details/gcghwajka.sHtML

[Q78] 当前时间
来源：http://3g.zdbjq.cn/Article/details/grcjsawhb.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.zdbjq.cn/Article/details/gxwvjqwxr.sHtML

[Q79] 字符串拼接
来源：http://blog.hesvh.cn/Article/details/gmmnfflnj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://m.share.fehbvm.com/Article/details/gooukdntv.sHtML

[Q80] 字符串截取
来源：http://m.share.hesvh.cn/Article/details/gcpmtxxnz.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.fehbvm.com/Article/details/gvvniwppd.sHtML

[Q81] 字符串替换
来源：http://baike.hesvh.cn/Article/details/gerlviwqq.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.hesvh.cn/Article/details/ginivhufg.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.zdbjq.cn/Article/details/grvntoapz.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/gpocqzlqp.sHtML

[Q83] 大小写转换
来源：http://www.share.hesvh.cn/Article/details/ggcpagity.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gvseqyyyq.sHtML

[Q84] 去除首尾空格
来源：http://3g.fehbvm.com/Article/details/guebomyhi.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gqgrjoanf.sHtML

[Q85] 数值取整
来源：http://wap.fehbvm.com/Article/details/gapassdge.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.zdbjq.cn/Article/details/gjlhjsper.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fehbvm.com/Article/details/gjzdlurxp.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.zdbjq.cn/Article/details/ghefaulfc.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fehbvm.com/Article/details/gfhokfmsp.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fehbvm.com/Article/details/gwfmstkuc.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.zdbjq.cn/Article/details/gsmzrmzkg.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.zdbjq.cn/Article/details/glfkzugly.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.fehbvm.com/Article/details/grdwrcddl.sHtML

[Q89] 判断表是否存在
来源：http://www.share.hesvh.cn/Article/details/gwuuypeoc.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.fehbvm.com/Article/details/glbkrtdff.sHtML

[Q90] 生成序号列
来源：http://wap.zdbjq.cn/Article/details/gyfuzpfta.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fehbvm.com/Article/details/gzfpbigtp.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gxxjuszqa.sHtML

R. Bash 专题
来源：http://www.share.fehbvm.com/Article/details/gtkavabze.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gfdcenadq.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.fehbvm.com/Article/details/gcjpqvlab.sHtML

#!/usr/bin/env bash
来源：http://wap.fehbvm.com/Article/details/gnwbptwch.sHtML

set -euo pipefail
来源：http://www.share.hesvh.cn/Article/details/gjqpgrmmw.sHtML

[R02] 变量赋值与使用
来源：http://www.share.hesvh.cn/Article/details/goibmvwqd.sHtML

name="Tom"; echo "$name"
来源：http://www.share.zdbjq.cn/Article/details/giesfquei.sHtML

[R03] 只读变量
来源：http://blog.hesvh.cn/Article/details/gjxmruslr.sHtML

readonly PI=3.14
来源：http://www.m.share.hesvh.cn/Article/details/giysxjmvo.sHtML

[R04] 位置参数
来源：http://blog.fehbvm.com/Article/details/gfmeeulek.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.fehbvm.com/Article/details/gluakhsxc.sHtML

[R05] 参数默认值
来源：http://wap.fehbvm.com/Article/details/gabfynkqr.sHtML

name="${1:-default}"
来源：http://blog.zdbjq.cn/Article/details/gqmqqhgwd.sHtML

[R06] 判断命令是否存在
来源：http://m.share.zdbjq.cn/Article/details/gslwmemla.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.zdbjq.cn/Article/details/gcxxfrwpd.sHtML

[R07] if 判断文件
来源：http://m.share.hesvh.cn/Article/details/glzpgrttl.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fehbvm.com/Article/details/gjcpjlran.sHtML

[R08] 数值比较
来源：http://www.m.share.fehbvm.com/Article/details/gluvmsexm.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.hesvh.cn/Article/details/ghatezqpz.sHtML

[R09] 字符串比较
来源：http://3g.zdbjq.cn/Article/details/gbzhclnkp.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.hesvh.cn/Article/details/gjelxsfqh.sHtML

[R10] 正则匹配
来源：http://mobile.hesvh.cn/Article/details/gfxtqhcwh.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fehbvm.com/Article/details/gvzxjefuw.sHtML

[R11] case 多分支
来源：http://read.share.hesvh.cn/Article/details/gwothznvh.sHtML

case "$1" in
来源：http://m.share.hesvh.cn/Article/details/ghnhxkygg.sHtML

start) echo "启动" ;;
来源：http://www.share.hesvh.cn/Article/details/gxumfxbvy.sHtML

stop)  echo "停止" ;;
来源：http://3g.zdbjq.cn/Article/details/gczvkosnb.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fehbvm.com/Article/details/ghgphoutr.sHtML

esac
来源：http://read.share.zdbjq.cn/Article/details/gwumzuakh.sHtML

[R12] for 遍历文件
来源：http://mobile.zdbjq.cn/Article/details/gcknaynza.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.hesvh.cn/Article/details/gwdtbycdr.sHtML

[R13] for 计数循环
来源：http://wap.fehbvm.com/Article/details/gihffxegj.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://read.share.hesvh.cn/Article/details/gtiwhhymf.sHtML

[R14] C 风格 for
来源：http://www.share.hesvh.cn/Article/details/gvgelxwem.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fehbvm.com/Article/details/gjlmlcsui.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gegmgyudj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fehbvm.com/Article/details/geycdkrem.sHtML

[R16] until 等待条件
来源：http://read.share.hesvh.cn/Article/details/gtalyrbig.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.hesvh.cn/Article/details/gcxmisxtg.sHtML

[R17] 数组定义与取值
来源：http://3g.fehbvm.com/Article/details/gbveliswc.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.hesvh.cn/Article/details/gubacwwmn.sHtML

[R18] 遍历数组
来源：http://read.share.zdbjq.cn/Article/details/gsqzhnvnf.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.zdbjq.cn/Article/details/gohuhsnjv.sHtML

[R19] 数组长度
来源：http://www.share.fehbvm.com/Article/details/ginpglrug.sHtML

echo "${#arr[@]}"
来源：http://read.share.hesvh.cn/Article/details/grygzibcr.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fehbvm.com/Article/details/gscyagrph.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fehbvm.com/Article/details/gmwuiuegz.sHtML

[R21] 字符串长度
来源：http://wap.fehbvm.com/Article/details/ghrkqjbce.sHtML

echo "${#s}"
来源：http://blog.zdbjq.cn/Article/details/gdtyzhwyg.sHtML

[R22] 截取子串
来源：http://m.share.fehbvm.com/Article/details/gsccwsysh.sHtML

echo "${s:0:5}"
来源：http://www.m.share.hesvh.cn/Article/details/gfimsvjhc.sHtML

[R23] 字符串替换
来源：http://3g.hesvh.cn/Article/details/gglouubss.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.hesvh.cn/Article/details/gjplfgrno.sHtML

[R24] 大小写转换
来源：http://3g.fehbvm.com/Article/details/gpnpmrgga.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.hesvh.cn/Article/details/gkfwdhjds.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.hesvh.cn/Article/details/gzvtdyymw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.zdbjq.cn/Article/details/gmwewrkta.sHtML

[R26] 命令替换
来源：http://www.blog.fehbvm.com/Article/details/gkrpnmgxi.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.hesvh.cn/Article/details/gmegecxaj.sHtML

[R27] 算术展开
来源：http://www.m.share.fehbvm.com/Article/details/gbovakibn.sHtML

echo $((1 + 2 * 3))
来源：http://blog.zdbjq.cn/Article/details/gkwgugdej.sHtML

[R28] 浮点运算
来源：http://blog.hesvh.cn/Article/details/gddabgcav.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fehbvm.com/Article/details/grigiqgob.sHtML

[R29] 定义函数
来源：http://wap.hesvh.cn/Article/details/genawabsn.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.hesvh.cn/Article/details/gfahguecn.sHtML

[R30] 函数返回状态码
来源：http://read.share.zdbjq.cn/Article/details/gelrafjbk.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.hesvh.cn/Article/details/gqyolzcfv.sHtML

[R31] 局部变量
来源：http://www.m.share.zdbjq.cn/Article/details/gdjftrtpd.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.hesvh.cn/Article/details/gmiirunoc.sHtML

[R32] 参数个数校验
来源：http://www.blog.fehbvm.com/Article/details/gfvcptpzv.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fehbvm.com/Article/details/gsmixhsot.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.zdbjq.cn/Article/details/grkopixbk.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.zdbjq.cn/Article/details/gmujurqmx.sHtML

[R34] 退出时清理
来源：http://mobile.hesvh.cn/Article/details/grbhvcjnw.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.hesvh.cn/Article/details/gdnyqxkmj.sHtML

[R35] 后台执行并等待
来源：http://www.blog.zdbjq.cn/Article/details/gznfexrwy.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.zdbjq.cn/Article/details/gzhepgaso.sHtML

[R36] 并发执行多个任务
来源：http://3g.fehbvm.com/Article/details/gozcldexq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fehbvm.com/Article/details/gzketelpg.sHtML

[R37] 把输出赋给变量
来源：http://www.share.hesvh.cn/Article/details/gejajxuvf.sHtML

files=$(ls -1)
来源：http://wap.zdbjq.cn/Article/details/gedwyffzt.sHtML

[R38] 管道串联
来源：http://www.m.share.zdbjq.cn/Article/details/gyljmzide.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fehbvm.com/Article/details/gmyozxazv.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.hesvh.cn/Article/details/gjnxuzxmh.sHtML

cmd > out.log 2>&1
来源：http://baike.hesvh.cn/Article/details/gweoxrwei.sHtML

[R40] 追加写日志
来源：http://read.share.zdbjq.cn/Article/details/gkxmcecac.sHtML

echo "log" >> out.log
来源：http://3g.hesvh.cn/Article/details/gkgkqwsnn.sHtML

[R41] 丢弃输出
来源：http://read.share.fehbvm.com/Article/details/gcoydixoj.sHtML

cmd >/dev/null 2>&1
来源：http://blog.zdbjq.cn/Article/details/gknjbnzrg.sHtML

[R42] 输入重定向
来源：http://mobile.fehbvm.com/Article/details/gvedklory.sHtML

wc -l < a.txt
来源：http://mobile.hesvh.cn/Article/details/glbnsvakw.sHtML

[R43] 按名字查找文件
来源：http://wap.hesvh.cn/Article/details/glgxfylmi.sHtML

find . -name "*.log" -type f
来源：http://wap.hesvh.cn/Article/details/gejobunet.sHtML

[R44] 按修改时间查找
来源：http://blog.zdbjq.cn/Article/details/gikvqezat.sHtML

find . -mtime -7 -type f
来源：http://wap.fehbvm.com/Article/details/glhlpmjyl.sHtML

[R45] 批量删除
来源：http://wap.hesvh.cn/Article/details/galauhhnj.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.hesvh.cn/Article/details/gntpugjys.sHtML

[R46] 递归替换文件内容
来源：http://baike.fehbvm.com/Article/details/gxjllokba.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fehbvm.com/Article/details/gnkdgshop.sHtML

[R47] sed 单行替换
来源：http://www.m.share.fehbvm.com/Article/details/gdlkhlxib.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.zdbjq.cn/Article/details/gcxdndpfb.sHtML

[R48] awk 取指定列
来源：http://www.m.share.hesvh.cn/Article/details/gyulpsdys.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.zdbjq.cn/Article/details/gqcjybkos.sHtML

[R49] awk 带条件
来源：http://blog.zdbjq.cn/Article/details/gxywfmmwv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.hesvh.cn/Article/details/gxifsqepu.sHtML

[R50] awk 求和
来源：http://www.blog.zdbjq.cn/Article/details/gqkcjsuaa.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.hesvh.cn/Article/details/glistyrjt.sHtML

[R51] 排序去重取前几
来源：http://blog.hesvh.cn/Article/details/gdjmifhwv.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.zdbjq.cn/Article/details/gxynqwyyb.sHtML

[R52] 统计行数
来源：http://www.share.fehbvm.com/Article/details/gwrldbjdo.sHtML

wc -l a.txt
来源：http://www.share.zdbjq.cn/Article/details/ggdwpkhop.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fehbvm.com/Article/details/gkimtfjcr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.hesvh.cn/Article/details/gyjgcgwin.sHtML

[R54] 比较两个文件
来源：http://blog.hesvh.cn/Article/details/gbhkwjkmv.sHtML

diff a.txt b.txt
来源：http://baike.zdbjq.cn/Article/details/ggzwsnwaq.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fehbvm.com/Article/details/gmsafebsr.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.hesvh.cn/Article/details/gyrfjmmqx.sHtML

[R56] 远程拷贝
来源：http://wap.zdbjq.cn/Article/details/ghnucpepu.sHtML

scp file user@host:/path/
来源：http://baike.hesvh.cn/Article/details/gsepeysho.sHtML

[R57] 远程执行命令
来源：http://read.share.fehbvm.com/Article/details/glddzwwyn.sHtML

ssh user@host 'uptime'
来源：http://3g.fehbvm.com/Article/details/gfglxrpvl.sHtML

[R58] 下载文件
来源：http://www.share.fehbvm.com/Article/details/gnkglbihz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.zdbjq.cn/Article/details/guhtzqmen.sHtML

[R59] 发 POST JSON
来源：http://mobile.fehbvm.com/Article/details/gwnmftafa.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.hesvh.cn/Article/details/gnmjngjmf.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.hesvh.cn/Article/details/gixdbsith.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.hesvh.cn/Article/details/gboepinwb.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fehbvm.com/Article/details/gnagpqbzi.sHtML

df -h;  du -sh *
来源：http://baike.fehbvm.com/Article/details/gmrdvyesq.sHtML

[R62] 找最占空间的文件
来源：http://3g.fehbvm.com/Article/details/gkctdlnof.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fehbvm.com/Article/details/ginbhwtlh.sHtML

[R63] 内存与进程
来源：http://www.blog.hesvh.cn/Article/details/gxpzjuphr.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.hesvh.cn/Article/details/gdnmvnrft.sHtML

[R64] 结束进程
来源：http://www.m.share.hesvh.cn/Article/details/gurbccyzj.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.zdbjq.cn/Article/details/gqvkvijld.sHtML

[R65] 查看端口占用
来源：http://www.share.fehbvm.com/Article/details/gipqavlwa.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fehbvm.com/Article/details/gnyuqnxvq.sHtML

[R66] 定时任务
来源：http://www.blog.fehbvm.com/Article/details/gjylnbjdw.sHtML

crontab -e;  crontab -l
来源：http://www.blog.zdbjq.cn/Article/details/gejapiijl.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fehbvm.com/Article/details/gbvyyleem.sHtML

openssl rand -hex 16
来源：http://baike.hesvh.cn/Article/details/gjzwoeicn.sHtML

[R68] 计算文件校验值
来源：http://3g.fehbvm.com/Article/details/glurzwonf.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.zdbjq.cn/Article/details/gzxonlsxy.sHtML

[R69] 生成随机密码
来源：http://baike.fehbvm.com/Article/details/ghxgmorye.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fehbvm.com/Article/details/gobrbunts.sHtML

[R70] 时间戳与互转
来源：http://baike.fehbvm.com/Article/details/gfwpsacfs.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.zdbjq.cn/Article/details/gikvkblwt.sHtML

[R71] 日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gvlbrfvzz.sHtML


<!-- 参考信息 -->