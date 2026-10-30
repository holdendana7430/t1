代发 wailian999

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.fehbvm.com/Article/details/gsxbielda.sHtML

[Q26] 计数
来源：http://www.m.share.zdbjq.cn/Article/details/gcfbhqurk.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.hesvh.cn/Article/details/grirxtsyw.sHtML

[Q27] 条件计数
来源：http://m.share.hesvh.cn/Article/details/gmvnvbixh.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.hesvh.cn/Article/details/griwghhkp.sHtML

[Q28] 求和与平均
来源：http://mobile.hesvh.cn/Article/details/gdmvjjkio.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.fehbvm.com/Article/details/gdkswkxvy.sHtML

[Q29] 最大最小值
来源：http://read.share.zdbjq.cn/Article/details/gcaclgccl.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.hesvh.cn/Article/details/gwczduske.sHtML

[Q30] 分组统计
来源：http://read.share.fehbvm.com/Article/details/giotkdlff.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/gezzyvtnz.sHtML

[Q31] 分组后过滤
来源：http://3g.hesvh.cn/Article/details/gqziyexuo.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://wap.zdbjq.cn/Article/details/grvudhbvl.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.hesvh.cn/Article/details/giuliptwa.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gqoyxwgkr.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.hesvh.cn/Article/details/gpqfevgap.sHtML

[Q33] 多列分组
来源：http://www.share.fehbvm.com/Article/details/gnnetnqvu.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.fehbvm.com/Article/details/gdvbasfsf.sHtML

[Q34] 每组取第一条
来源：http://www.blog.fehbvm.com/Article/details/gykjzvock.sHtML

SELECT * FROM (
来源：http://mobile.zdbjq.cn/Article/details/gexynbgkt.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.fehbvm.com/Article/details/gzxsbypci.sHtML

) t WHERE rn = 1;
来源：http://read.share.zdbjq.cn/Article/details/gtiigaphv.sHtML

[Q35] 内连接
来源：http://read.share.zdbjq.cn/Article/details/gblmpdeqi.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.zdbjq.cn/Article/details/gjhinbrxa.sHtML

[Q36] 左连接
来源：http://wap.fehbvm.com/Article/details/gftyzrmrv.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.zdbjq.cn/Article/details/geuewhkmj.sHtML

[Q37] 右连接
来源：http://m.share.zdbjq.cn/Article/details/gbticmcei.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.fehbvm.com/Article/details/gwyevpnve.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.hesvh.cn/Article/details/gramxgypg.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.zdbjq.cn/Article/details/guokqruao.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.fehbvm.com/Article/details/gqzzucbew.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.fehbvm.com/Article/details/gplhbbgjc.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.hesvh.cn/Article/details/gqgouhbsi.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.fehbvm.com/Article/details/gddyeeujv.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.zdbjq.cn/Article/details/gkiqlqwqx.sHtML

[Q41] 多表连接
来源：http://www.blog.hesvh.cn/Article/details/gvfriyavw.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.zdbjq.cn/Article/details/gbdjcwkpl.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.fehbvm.com/Article/details/gscgzcwnf.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.zdbjq.cn/Article/details/gntfrocwd.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.zdbjq.cn/Article/details/gfgnunram.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.fehbvm.com/Article/details/gqgheinvk.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.fehbvm.com/Article/details/gpgntszbc.sHtML

[Q43] 标量子查询
来源：http://m.share.zdbjq.cn/Article/details/gxltrwlux.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.hesvh.cn/Article/details/gtgbagvyg.sHtML

[Q44] IN 子查询
来源：http://read.share.zdbjq.cn/Article/details/gojbgltkb.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.fehbvm.com/Article/details/gaupnxrte.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.hesvh.cn/Article/details/gikzykoeu.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.hesvh.cn/Article/details/gjpkhdjcw.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.hesvh.cn/Article/details/gvulohhgf.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.hesvh.cn/Article/details/gicawbiye.sHtML

[Q47] 与平均值比较
来源：http://blog.fehbvm.com/Article/details/gieimbymu.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.zdbjq.cn/Article/details/gqawgzitp.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.hesvh.cn/Article/details/gvjsrtodp.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.fehbvm.com/Article/details/ggeejmuyr.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.fehbvm.com/Article/details/gwadmyncb.sHtML

[Q49] 更新单行
来源：http://baike.fehbvm.com/Article/details/gnqhyvjcx.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.fehbvm.com/Article/details/gbxqsqgpf.sHtML

[Q50] 批量更新
来源：http://wap.zdbjq.cn/Article/details/gnnrwkblk.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.hesvh.cn/Article/details/gedccbkad.sHtML

[Q51] 用子查询更新
来源：http://blog.zdbjq.cn/Article/details/gaymorxkr.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.fehbvm.com/Article/details/ghzbjxjlf.sHtML

[Q52] 删除指定行
来源：http://wap.fehbvm.com/Article/details/ggaierzle.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.zdbjq.cn/Article/details/gjavwogty.sHtML

[Q53] 按条件删除
来源：http://3g.fehbvm.com/Article/details/gjgfjcihf.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.hesvh.cn/Article/details/gqxhwgppu.sHtML

[Q54] 清空表
来源：http://mobile.hesvh.cn/Article/details/gxkflqnbi.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.zdbjq.cn/Article/details/gaihnqbru.sHtML

[Q55] 排名（并列占位）
来源：http://wap.hesvh.cn/Article/details/gikzsuxxu.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.fehbvm.com/Article/details/gkfvhgdzz.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.fehbvm.com/Article/details/grtwqewcl.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.hesvh.cn/Article/details/gjbdhakht.sHtML

[Q57] 行号
来源：http://m.share.fehbvm.com/Article/details/gfgubhkts.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.fehbvm.com/Article/details/gvicdsnxv.sHtML

[Q58] 累计求和
来源：http://3g.fehbvm.com/Article/details/grjsnanxr.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gxpcbqzca.sHtML

[Q59] 分组内累计
来源：http://wap.zdbjq.cn/Article/details/gbtgmzbqs.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gkmfrjrfh.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.zdbjq.cn/Article/details/gvgtufemy.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.hesvh.cn/Article/details/gzvjqaqsx.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gbfojgfgo.sHtML

[Q61] 移动平均
来源：http://www.share.hesvh.cn/Article/details/gwlcwuzdm.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/guhteoyvz.sHtML

[Q62] 分组占比
来源：http://read.share.fehbvm.com/Article/details/gvejhygko.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/ginuoakyc.sHtML

[Q63] 开启事务
来源：http://www.m.share.fehbvm.com/Article/details/gvavczldw.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.fehbvm.com/Article/details/gugelmlao.sHtML

[Q64] 提交事务
来源：http://blog.hesvh.cn/Article/details/gvkyrfmxy.sHtML

COMMIT;
来源：http://www.blog.hesvh.cn/Article/details/ghbmeypgx.sHtML

[Q65] 回滚事务
来源：http://baike.zdbjq.cn/Article/details/gyxazqubz.sHtML

ROLLBACK;
来源：http://baike.hesvh.cn/Article/details/giipozeaj.sHtML

[Q66] 行锁查询
来源：http://3g.zdbjq.cn/Article/details/gjfnuasik.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.zdbjq.cn/Article/details/gofmfzusw.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fehbvm.com/Article/details/gblmdvdep.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.hesvh.cn/Article/details/giidtmoue.sHtML

[Q68] 保存点
来源：http://www.share.zdbjq.cn/Article/details/gsgsmxbcl.sHtML

SAVEPOINT sp1;
来源：http://blog.fehbvm.com/Article/details/gkvkxmylk.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.hesvh.cn/Article/details/gkmnwvacz.sHtML

[Q69] 查看执行计划
来源：http://mobile.zdbjq.cn/Article/details/gdxqtvclo.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.hesvh.cn/Article/details/ghghctfei.sHtML

[Q70] 更新统计信息
来源：http://wap.fehbvm.com/Article/details/gdplnfxjp.sHtML

ANALYZE TABLE users;
来源：http://mobile.hesvh.cn/Article/details/gjdcnwthd.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.fehbvm.com/Article/details/gwqiifvsv.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fehbvm.com/Article/details/gmhsyxnqc.sHtML

[Q72] 查看索引
来源：http://3g.hesvh.cn/Article/details/gqngmjqry.sHtML

SHOW INDEX FROM users;
来源：http://3g.fehbvm.com/Article/details/gighvsmwz.sHtML

[Q73] 查看表状态
来源：http://www.m.share.fehbvm.com/Article/details/giemnzgvq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.hesvh.cn/Article/details/gbxtvbpdd.sHtML

[Q74] 强制使用索引
来源：http://wap.fehbvm.com/Article/details/gzoigsspl.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.hesvh.cn/Article/details/gwaxwmfdb.sHtML

[Q75] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/gfpvzoinu.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gjgdbntff.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.zdbjq.cn/Article/details/ggkaocswa.sHtML

[Q76] 按天统计
来源：http://www.share.zdbjq.cn/Article/details/ghibutdjh.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.hesvh.cn/Article/details/gupugnsro.sHtML

[Q77] 时间加减
来源：http://mobile.zdbjq.cn/Article/details/gmiwfgouc.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.fehbvm.com/Article/details/genehhgqy.sHtML

[Q78] 当前时间
来源：http://blog.fehbvm.com/Article/details/gtuhxmvuy.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.zdbjq.cn/Article/details/gbncxvwhq.sHtML

[Q79] 字符串拼接
来源：http://m.share.fehbvm.com/Article/details/gfiebicjb.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.fehbvm.com/Article/details/gckeuorir.sHtML

[Q80] 字符串截取
来源：http://baike.fehbvm.com/Article/details/gsrvevwed.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.hesvh.cn/Article/details/gpthlxfrc.sHtML

[Q81] 字符串替换
来源：http://www.blog.hesvh.cn/Article/details/gsknrdrkq.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.fehbvm.com/Article/details/grruznaxf.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.fehbvm.com/Article/details/gyjkhejqv.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gtpxebyqm.sHtML

[Q83] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/gxpagaopb.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/grvpdcdih.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fehbvm.com/Article/details/ganxbkkmd.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gtfalbylc.sHtML

[Q85] 数值取整
来源：http://wap.zdbjq.cn/Article/details/goyvzfzsj.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.zdbjq.cn/Article/details/gubjbeufw.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.hesvh.cn/Article/details/gezzltcyr.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fehbvm.com/Article/details/gvqptiymz.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.fehbvm.com/Article/details/grnqdyoey.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.zdbjq.cn/Article/details/gkokiiyfn.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.hesvh.cn/Article/details/gaubspvhi.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.hesvh.cn/Article/details/grsquaqqz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fehbvm.com/Article/details/gtvgbaslg.sHtML

[Q89] 判断表是否存在
来源：http://3g.fehbvm.com/Article/details/gglsousec.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.zdbjq.cn/Article/details/giqwwfwys.sHtML

[Q90] 生成序号列
来源：http://www.blog.fehbvm.com/Article/details/gnriottyo.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fehbvm.com/Article/details/gitowqnvb.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gwpgzytds.sHtML

R. Bash 专题
来源：http://m.share.zdbjq.cn/Article/details/glnptoyud.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/gdikrikwj.sHtML

[R01] shebang 与严格模式
来源：http://wap.zdbjq.cn/Article/details/gjcxhvckq.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.hesvh.cn/Article/details/gkojxvanl.sHtML

set -euo pipefail
来源：http://3g.fehbvm.com/Article/details/gkkuuvbiz.sHtML

[R02] 变量赋值与使用
来源：http://mobile.zdbjq.cn/Article/details/ghjsfcjfb.sHtML

name="Tom"; echo "$name"
来源：http://m.share.hesvh.cn/Article/details/gmfbehtry.sHtML

[R03] 只读变量
来源：http://www.blog.hesvh.cn/Article/details/gbhlgftdu.sHtML

readonly PI=3.14
来源：http://wap.hesvh.cn/Article/details/gdbbpumof.sHtML

[R04] 位置参数
来源：http://www.blog.fehbvm.com/Article/details/gylxcujde.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.zdbjq.cn/Article/details/gscgahhmg.sHtML

[R05] 参数默认值
来源：http://mobile.hesvh.cn/Article/details/ghvehuvoh.sHtML

name="${1:-default}"
来源：http://mobile.hesvh.cn/Article/details/gsbwtypmq.sHtML

[R06] 判断命令是否存在
来源：http://blog.zdbjq.cn/Article/details/gcvzhsgff.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.fehbvm.com/Article/details/gditipetc.sHtML

[R07] if 判断文件
来源：http://www.share.fehbvm.com/Article/details/gbecekyeo.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gncrlwhme.sHtML

[R08] 数值比较
来源：http://blog.hesvh.cn/Article/details/ggyfdjapo.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.hesvh.cn/Article/details/gugufmojc.sHtML

[R09] 字符串比较
来源：http://m.share.zdbjq.cn/Article/details/gmizifhhu.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.hesvh.cn/Article/details/gqipiwdpg.sHtML

[R10] 正则匹配
来源：http://mobile.hesvh.cn/Article/details/gepfmmajw.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://wap.fehbvm.com/Article/details/gsbgjiiln.sHtML

[R11] case 多分支
来源：http://baike.zdbjq.cn/Article/details/ggywkdnwa.sHtML

case "$1" in
来源：http://mobile.fehbvm.com/Article/details/gfaehfqhz.sHtML

start) echo "启动" ;;
来源：http://www.m.share.hesvh.cn/Article/details/ghcznxdsk.sHtML

stop)  echo "停止" ;;
来源：http://blog.fehbvm.com/Article/details/gatlxujei.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fehbvm.com/Article/details/glijpykch.sHtML

esac
来源：http://www.blog.zdbjq.cn/Article/details/ghgjmsces.sHtML

[R12] for 遍历文件
来源：http://wap.fehbvm.com/Article/details/gfvwvjzew.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.zdbjq.cn/Article/details/gkxcecbgt.sHtML

[R13] for 计数循环
来源：http://m.share.fehbvm.com/Article/details/gnjcrqbrw.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fehbvm.com/Article/details/gldwdxgca.sHtML

[R14] C 风格 for
来源：http://3g.hesvh.cn/Article/details/gbrvzzxcm.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/gslhzxcxn.sHtML

[R15] while 逐行读文件
来源：http://3g.fehbvm.com/Article/details/gdmihvvxp.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.hesvh.cn/Article/details/gcyagsmfz.sHtML

[R16] until 等待条件
来源：http://blog.fehbvm.com/Article/details/gzuhhgvbs.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.hesvh.cn/Article/details/gmguhgrbp.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fehbvm.com/Article/details/gscjqyajm.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.fehbvm.com/Article/details/goekbtnww.sHtML

[R18] 遍历数组
来源：http://www.share.hesvh.cn/Article/details/gizowwdfy.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.hesvh.cn/Article/details/gfqkncxwd.sHtML

[R19] 数组长度
来源：http://wap.hesvh.cn/Article/details/gbxttwrla.sHtML

echo "${#arr[@]}"
来源：http://www.share.zdbjq.cn/Article/details/gwmshwzsy.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fehbvm.com/Article/details/ggqwcoevp.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fehbvm.com/Article/details/gwwlgcoxx.sHtML

[R21] 字符串长度
来源：http://www.blog.fehbvm.com/Article/details/gvvrdczsa.sHtML

echo "${#s}"
来源：http://baike.fehbvm.com/Article/details/gcaxeteyx.sHtML

[R22] 截取子串
来源：http://wap.fehbvm.com/Article/details/gvjlcjyzl.sHtML

echo "${s:0:5}"
来源：http://blog.zdbjq.cn/Article/details/gfhytdnyv.sHtML

[R23] 字符串替换
来源：http://blog.hesvh.cn/Article/details/gycvnpfwo.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.zdbjq.cn/Article/details/geuwhgamh.sHtML

[R24] 大小写转换
来源：http://read.share.hesvh.cn/Article/details/gylqpeeah.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fehbvm.com/Article/details/gqkwxrzbj.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.hesvh.cn/Article/details/gtcypsgvs.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.zdbjq.cn/Article/details/gbugvyyop.sHtML

[R26] 命令替换
来源：http://blog.fehbvm.com/Article/details/gjpteihis.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.zdbjq.cn/Article/details/gfmunhkcw.sHtML

[R27] 算术展开
来源：http://www.share.fehbvm.com/Article/details/guoogvooi.sHtML

echo $((1 + 2 * 3))
来源：http://3g.zdbjq.cn/Article/details/gkrxwopab.sHtML

[R28] 浮点运算
来源：http://baike.hesvh.cn/Article/details/gdanrabsk.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.hesvh.cn/Article/details/gyihijxik.sHtML

[R29] 定义函数
来源：http://baike.fehbvm.com/Article/details/ggvqndxdb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.fehbvm.com/Article/details/gpadnowfb.sHtML

[R30] 函数返回状态码
来源：http://read.share.hesvh.cn/Article/details/gckxgakui.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fehbvm.com/Article/details/gpttweqwc.sHtML

[R31] 局部变量
来源：http://www.share.fehbvm.com/Article/details/gzkqfqyxq.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.hesvh.cn/Article/details/gzplwfpbq.sHtML

[R32] 参数个数校验
来源：http://www.share.zdbjq.cn/Article/details/gizyjrdhc.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/gnhbgccxv.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.hesvh.cn/Article/details/gyqqivikp.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.hesvh.cn/Article/details/gprehcyex.sHtML

[R34] 退出时清理
来源：http://www.blog.hesvh.cn/Article/details/gpbgrjxwe.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.hesvh.cn/Article/details/geerbizyi.sHtML

[R35] 后台执行并等待
来源：http://www.share.zdbjq.cn/Article/details/gpknwrokp.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fehbvm.com/Article/details/gursplhip.sHtML

[R36] 并发执行多个任务
来源：http://wap.zdbjq.cn/Article/details/gsjvskneq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.zdbjq.cn/Article/details/ggftpvizo.sHtML

[R37] 把输出赋给变量
来源：http://blog.fehbvm.com/Article/details/gkeklifxd.sHtML

files=$(ls -1)
来源：http://blog.zdbjq.cn/Article/details/guesrxzsa.sHtML

[R38] 管道串联
来源：http://wap.hesvh.cn/Article/details/giqyzaaac.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fehbvm.com/Article/details/gmplvqnjs.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.zdbjq.cn/Article/details/gcmiuaokc.sHtML

cmd > out.log 2>&1
来源：http://mobile.zdbjq.cn/Article/details/gfsuqcadd.sHtML

[R40] 追加写日志
来源：http://read.share.hesvh.cn/Article/details/gdicndnie.sHtML

echo "log" >> out.log
来源：http://baike.zdbjq.cn/Article/details/givpnpudj.sHtML

[R41] 丢弃输出
来源：http://www.blog.fehbvm.com/Article/details/gbinjnltn.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fehbvm.com/Article/details/gkntpwuki.sHtML

[R42] 输入重定向
来源：http://3g.fehbvm.com/Article/details/gpelehxuz.sHtML

wc -l < a.txt
来源：http://m.share.hesvh.cn/Article/details/gdzlcpwue.sHtML

[R43] 按名字查找文件
来源：http://3g.hesvh.cn/Article/details/gyjkrikpk.sHtML

find . -name "*.log" -type f
来源：http://read.share.hesvh.cn/Article/details/gewnupajp.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.hesvh.cn/Article/details/gqqepzgus.sHtML

find . -mtime -7 -type f
来源：http://baike.hesvh.cn/Article/details/glflsfkpb.sHtML

[R45] 批量删除
来源：http://mobile.hesvh.cn/Article/details/gxukgcwsa.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.hesvh.cn/Article/details/gsuchngci.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fehbvm.com/Article/details/gtjjrvdhn.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.hesvh.cn/Article/details/gfxsiuywq.sHtML

[R47] sed 单行替换
来源：http://baike.zdbjq.cn/Article/details/geqmfiopr.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fehbvm.com/Article/details/gmwgoxezo.sHtML

[R48] awk 取指定列
来源：http://blog.fehbvm.com/Article/details/glsvsdlqi.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.hesvh.cn/Article/details/gavcpzdjq.sHtML

[R49] awk 带条件
来源：http://m.share.fehbvm.com/Article/details/gbiyyqftn.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fehbvm.com/Article/details/gjgyfyytq.sHtML

[R50] awk 求和
来源：http://baike.fehbvm.com/Article/details/gxulwhxjf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gungzdbdv.sHtML

[R51] 排序去重取前几
来源：http://www.share.fehbvm.com/Article/details/gbnsziuvk.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.hesvh.cn/Article/details/gbluamsfc.sHtML

[R52] 统计行数
来源：http://3g.zdbjq.cn/Article/details/gxtucpjfk.sHtML

wc -l a.txt
来源：http://blog.hesvh.cn/Article/details/ghtuvnren.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.hesvh.cn/Article/details/gelnqmkrt.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fehbvm.com/Article/details/gpyrcedjs.sHtML

[R54] 比较两个文件
来源：http://read.share.hesvh.cn/Article/details/givmjuawk.sHtML

diff a.txt b.txt
来源：http://blog.hesvh.cn/Article/details/gwqayfqhp.sHtML

[R55] 压缩与解压
来源：http://read.share.hesvh.cn/Article/details/gslfgxgvr.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.hesvh.cn/Article/details/gfgnhcvxk.sHtML

[R56] 远程拷贝
来源：http://read.share.fehbvm.com/Article/details/geilloqqw.sHtML

scp file user@host:/path/
来源：http://3g.fehbvm.com/Article/details/gfnbsdinm.sHtML

[R57] 远程执行命令
来源：http://www.share.hesvh.cn/Article/details/gehqkmgsu.sHtML

ssh user@host 'uptime'
来源：http://3g.zdbjq.cn/Article/details/gwvwxnwqe.sHtML

[R58] 下载文件
来源：http://m.share.hesvh.cn/Article/details/gryqrvvyn.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.hesvh.cn/Article/details/gcjigaoie.sHtML

[R59] 发 POST JSON
来源：http://www.share.zdbjq.cn/Article/details/grqymejts.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fehbvm.com/Article/details/gnzlbznqm.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.zdbjq.cn/Article/details/ghpmaxetg.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fehbvm.com/Article/details/gvtdxmeyd.sHtML

[R61] 磁盘占用
来源：http://www.m.share.hesvh.cn/Article/details/gomsxpihf.sHtML

df -h;  du -sh *
来源：http://www.m.share.hesvh.cn/Article/details/ggdicbqya.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.hesvh.cn/Article/details/gjmfsjdpv.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fehbvm.com/Article/details/gejnoandm.sHtML

[R63] 内存与进程
来源：http://3g.zdbjq.cn/Article/details/gmciifvkv.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.hesvh.cn/Article/details/grqejsixx.sHtML

[R64] 结束进程
来源：http://mobile.fehbvm.com/Article/details/gywvfgmks.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fehbvm.com/Article/details/gtkjxhevl.sHtML

[R65] 查看端口占用
来源：http://m.share.zdbjq.cn/Article/details/gflbbiyva.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fehbvm.com/Article/details/gisubhdlw.sHtML

[R66] 定时任务
来源：http://www.m.share.hesvh.cn/Article/details/gnmifwpmm.sHtML

crontab -e;  crontab -l
来源：http://3g.fehbvm.com/Article/details/gpzshgmij.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.hesvh.cn/Article/details/gbfijpliz.sHtML

openssl rand -hex 16
来源：http://mobile.zdbjq.cn/Article/details/gyxwzqgsl.sHtML

[R68] 计算文件校验值
来源：http://mobile.hesvh.cn/Article/details/gmadfndtf.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fehbvm.com/Article/details/gdolloghz.sHtML

[R69] 生成随机密码
来源：http://3g.fehbvm.com/Article/details/gowalzptq.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.hesvh.cn/Article/details/geltbyhzf.sHtML

[R70] 时间戳与互转
来源：http://mobile.fehbvm.com/Article/details/gwuvsmeqp.sHtML

date +%s;  date -d @1700000000
来源：http://3g.hesvh.cn/Article/details/gyvfirbko.sHtML

[R71] 日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/guzyzbckg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fehbvm.com/Article/details/gxbidgdhh.sHtML

[R72] 等待端口就绪
来源：http://mobile.hesvh.cn/Article/details/grcytjxxu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.zdbjq.cn/Article/details/ggogkqmsc.sHtML

[R73] 分割大日志
来源：http://www.share.hesvh.cn/Article/details/glvoqlnuq.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.zdbjq.cn/Article/details/gmznxpaoc.sHtML

[R74] 批量重命名
来源：http://read.share.hesvh.cn/Article/details/gvaxzkpie.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fehbvm.com/Article/details/gbkjjtuch.sHtML

[R75] 导出环境变量
来源：http://mobile.hesvh.cn/Article/details/gfywgpvli.sHtML


<!-- 参考信息 -->