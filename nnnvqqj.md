代发 wailian999

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.hesvh.cn/Article/details/gfgoysoid.sHtML

[Q26] 计数
来源：http://mobile.fehbvm.com/Article/details/gzefdlsgs.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.fehbvm.com/Article/details/gpzwphivm.sHtML

[Q27] 条件计数
来源：http://read.share.fehbvm.com/Article/details/gpjnpctvc.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.hesvh.cn/Article/details/gxnqtkqly.sHtML

[Q28] 求和与平均
来源：http://mobile.fehbvm.com/Article/details/gmuetkcsi.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.fehbvm.com/Article/details/gugkwpkez.sHtML

[Q29] 最大最小值
来源：http://wap.zdbjq.cn/Article/details/gdhhezvuc.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gyzrhuylo.sHtML

[Q30] 分组统计
来源：http://mobile.zdbjq.cn/Article/details/gcplumsza.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/gsxhcfdwj.sHtML

[Q31] 分组后过滤
来源：http://mobile.hesvh.cn/Article/details/gauuyjtbr.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.fehbvm.com/Article/details/gxhuqlrzy.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/glxmarata.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gfarhswhy.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.zdbjq.cn/Article/details/ghzriylzj.sHtML

[Q33] 多列分组
来源：http://m.share.hesvh.cn/Article/details/glhfsteti.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.hesvh.cn/Article/details/gutjvwuez.sHtML

[Q34] 每组取第一条
来源：http://wap.fehbvm.com/Article/details/gaohcmuoj.sHtML

SELECT * FROM (
来源：http://mobile.zdbjq.cn/Article/details/gnbujamnl.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.zdbjq.cn/Article/details/gllancycw.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gllynwtwx.sHtML

[Q35] 内连接
来源：http://m.share.hesvh.cn/Article/details/gwwnrnnzy.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.zdbjq.cn/Article/details/gmkftykuc.sHtML

[Q36] 左连接
来源：http://www.m.share.zdbjq.cn/Article/details/gbtlaleak.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fehbvm.com/Article/details/gewdawfro.sHtML

[Q37] 右连接
来源：http://www.share.hesvh.cn/Article/details/gihkrzacz.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.fehbvm.com/Article/details/gpbyhykbv.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.zdbjq.cn/Article/details/gwtobpmmo.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.fehbvm.com/Article/details/gkmkjodmq.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.fehbvm.com/Article/details/gisuixmze.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.hesvh.cn/Article/details/glwkawncz.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.hesvh.cn/Article/details/gdgrwonas.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.hesvh.cn/Article/details/gumnsiwiw.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.fehbvm.com/Article/details/ggahhoylk.sHtML

[Q41] 多表连接
来源：http://mobile.zdbjq.cn/Article/details/ghzuqwfod.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.zdbjq.cn/Article/details/gzobvrjlp.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.fehbvm.com/Article/details/gaeivsvzb.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.fehbvm.com/Article/details/glkzlkaly.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.hesvh.cn/Article/details/gapkxyqdk.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.zdbjq.cn/Article/details/gqywtwxsl.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.fehbvm.com/Article/details/gslrcocig.sHtML

[Q43] 标量子查询
来源：http://read.share.zdbjq.cn/Article/details/gxlrliwaz.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.fehbvm.com/Article/details/gfkutbqgk.sHtML

[Q44] IN 子查询
来源：http://read.share.zdbjq.cn/Article/details/ggarrxprj.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.fehbvm.com/Article/details/gncaomhqn.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.hesvh.cn/Article/details/gdxirahne.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.zdbjq.cn/Article/details/ghaqnbyoy.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.fehbvm.com/Article/details/goheuopmy.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.zdbjq.cn/Article/details/gmfozdhdr.sHtML

[Q47] 与平均值比较
来源：http://blog.fehbvm.com/Article/details/gtwlihjxw.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.fehbvm.com/Article/details/gmzaqipyf.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.hesvh.cn/Article/details/gdmyybmzr.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.zdbjq.cn/Article/details/gwxzpvbcx.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.fehbvm.com/Article/details/gzkomutru.sHtML

[Q49] 更新单行
来源：http://m.share.zdbjq.cn/Article/details/gjovgpyhi.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.zdbjq.cn/Article/details/gabdplkft.sHtML

[Q50] 批量更新
来源：http://www.blog.zdbjq.cn/Article/details/goomfaoki.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.hesvh.cn/Article/details/gdbkughqz.sHtML

[Q51] 用子查询更新
来源：http://blog.zdbjq.cn/Article/details/gmjfsedvt.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.hesvh.cn/Article/details/gtvortnbn.sHtML

[Q52] 删除指定行
来源：http://www.blog.hesvh.cn/Article/details/gnugzhynn.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.hesvh.cn/Article/details/glcchensc.sHtML

[Q53] 按条件删除
来源：http://m.share.fehbvm.com/Article/details/gzatcudag.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.zdbjq.cn/Article/details/gxygrpvef.sHtML

[Q54] 清空表
来源：http://blog.hesvh.cn/Article/details/gcfdxchiu.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.hesvh.cn/Article/details/gmjlqccts.sHtML

[Q55] 排名（并列占位）
来源：http://wap.fehbvm.com/Article/details/gxiqtzaec.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.hesvh.cn/Article/details/gnxpuqowz.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.zdbjq.cn/Article/details/glqfzblfz.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.fehbvm.com/Article/details/gdxbtnvfi.sHtML

[Q57] 行号
来源：http://www.share.fehbvm.com/Article/details/ghtkauqmw.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gefxptmrk.sHtML

[Q58] 累计求和
来源：http://www.m.share.zdbjq.cn/Article/details/gbggcyrqf.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.fehbvm.com/Article/details/ghrsvcjyh.sHtML

[Q59] 分组内累计
来源：http://m.share.hesvh.cn/Article/details/gkrmbivdt.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/ggrifzwkl.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.hesvh.cn/Article/details/gxhfvwhhr.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.zdbjq.cn/Article/details/grzqpxbti.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gsfygiais.sHtML

[Q61] 移动平均
来源：http://www.blog.hesvh.cn/Article/details/gijlmaqsa.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gbojbouhh.sHtML

[Q62] 分组占比
来源：http://www.blog.zdbjq.cn/Article/details/gsgixrlib.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/gwhkdhtby.sHtML

[Q63] 开启事务
来源：http://blog.zdbjq.cn/Article/details/gxgbgkzxp.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fehbvm.com/Article/details/gtpdmeeqi.sHtML

[Q64] 提交事务
来源：http://blog.zdbjq.cn/Article/details/gfgeciuqo.sHtML

COMMIT;
来源：http://mobile.zdbjq.cn/Article/details/gfnkvkefv.sHtML

[Q65] 回滚事务
来源：http://blog.zdbjq.cn/Article/details/gimlnvrua.sHtML

ROLLBACK;
来源：http://www.share.hesvh.cn/Article/details/gipenectv.sHtML

[Q66] 行锁查询
来源：http://baike.zdbjq.cn/Article/details/gfgqlpbbm.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.fehbvm.com/Article/details/gbjpaityw.sHtML

[Q67] 设置隔离级别
来源：http://read.share.fehbvm.com/Article/details/gaxyqubmr.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.hesvh.cn/Article/details/gaeenrvlq.sHtML

[Q68] 保存点
来源：http://www.share.fehbvm.com/Article/details/gjopmgqdt.sHtML

SAVEPOINT sp1;
来源：http://blog.fehbvm.com/Article/details/gtizpfdaq.sHtML

ROLLBACK TO sp1;
来源：http://mobile.fehbvm.com/Article/details/guuucbddm.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.hesvh.cn/Article/details/gwdsemzyq.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fehbvm.com/Article/details/gzmdeoooq.sHtML

[Q70] 更新统计信息
来源：http://www.blog.hesvh.cn/Article/details/gccrpyrfp.sHtML

ANALYZE TABLE users;
来源：http://www.blog.fehbvm.com/Article/details/gmauvzghf.sHtML

[Q71] 查看建表语句
来源：http://3g.fehbvm.com/Article/details/grkolkkej.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.fehbvm.com/Article/details/gygoyrpkm.sHtML

[Q72] 查看索引
来源：http://www.share.fehbvm.com/Article/details/gmnmorkzq.sHtML

SHOW INDEX FROM users;
来源：http://blog.zdbjq.cn/Article/details/gmzpgairv.sHtML

[Q73] 查看表状态
来源：http://3g.zdbjq.cn/Article/details/gqnmjxwkr.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.hesvh.cn/Article/details/gextqbyid.sHtML

[Q74] 强制使用索引
来源：http://www.blog.zdbjq.cn/Article/details/gqvqgpkla.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.hesvh.cn/Article/details/gzqwqyqfe.sHtML

[Q75] 日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gpeozstuf.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.fehbvm.com/Article/details/glrujezda.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.zdbjq.cn/Article/details/gxtxrgrni.sHtML

[Q76] 按天统计
来源：http://baike.fehbvm.com/Article/details/gpsstmjre.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.fehbvm.com/Article/details/gmlcegnex.sHtML

[Q77] 时间加减
来源：http://blog.fehbvm.com/Article/details/grtdmrmdt.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.zdbjq.cn/Article/details/ggjeekalj.sHtML

[Q78] 当前时间
来源：http://3g.fehbvm.com/Article/details/glwregpvy.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.zdbjq.cn/Article/details/gxtdusowr.sHtML

[Q79] 字符串拼接
来源：http://www.share.zdbjq.cn/Article/details/gvyhxgkzl.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.hesvh.cn/Article/details/gnomfaqlc.sHtML

[Q80] 字符串截取
来源：http://www.m.share.zdbjq.cn/Article/details/gkkyjniaf.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gcinbsffq.sHtML

[Q81] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/gknsraetv.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gwvuphzov.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.zdbjq.cn/Article/details/gydmrwvsm.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gyivsuqva.sHtML

[Q83] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/gbmwsocxs.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gwnkdvisk.sHtML

[Q84] 去除首尾空格
来源：http://wap.fehbvm.com/Article/details/gmdpjowwp.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/grpvqvnwe.sHtML

[Q85] 数值取整
来源：http://wap.zdbjq.cn/Article/details/gzwflulfl.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.hesvh.cn/Article/details/gczbkvcyp.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.zdbjq.cn/Article/details/gzwhfsrcp.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.zdbjq.cn/Article/details/gzeegoznz.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.fehbvm.com/Article/details/ggjjakaij.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.hesvh.cn/Article/details/gptoswnkj.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fehbvm.com/Article/details/gluffklqm.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fehbvm.com/Article/details/grqfekoou.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fehbvm.com/Article/details/giyvjdtim.sHtML

[Q89] 判断表是否存在
来源：http://3g.fehbvm.com/Article/details/gxuubsgqv.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.hesvh.cn/Article/details/ggoudxsrt.sHtML

[Q90] 生成序号列
来源：http://m.share.hesvh.cn/Article/details/gaejfbbkd.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fehbvm.com/Article/details/gevvkcqck.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gfwdcezit.sHtML

R. Bash 专题
来源：http://www.blog.hesvh.cn/Article/details/gskmcjdue.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gjqqtmwls.sHtML

[R01] shebang 与严格模式
来源：http://read.share.zdbjq.cn/Article/details/gtymwagpt.sHtML

#!/usr/bin/env bash
来源：http://www.share.zdbjq.cn/Article/details/gomfgeroo.sHtML

set -euo pipefail
来源：http://www.share.fehbvm.com/Article/details/gcxwjbjrc.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fehbvm.com/Article/details/gkudeefhq.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fehbvm.com/Article/details/glsjpbcuo.sHtML

[R03] 只读变量
来源：http://blog.hesvh.cn/Article/details/gaghnahux.sHtML

readonly PI=3.14
来源：http://www.m.share.zdbjq.cn/Article/details/gndrnocjj.sHtML

[R04] 位置参数
来源：http://blog.zdbjq.cn/Article/details/gwgynjxbf.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.hesvh.cn/Article/details/ggmshzylt.sHtML

[R05] 参数默认值
来源：http://www.share.fehbvm.com/Article/details/gmhbjbykq.sHtML

name="${1:-default}"
来源：http://www.blog.fehbvm.com/Article/details/giiqiwklz.sHtML

[R06] 判断命令是否存在
来源：http://3g.hesvh.cn/Article/details/gdqufrigf.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/gmajruppo.sHtML

[R07] if 判断文件
来源：http://wap.fehbvm.com/Article/details/gvklhkeqb.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fehbvm.com/Article/details/gezxohkwy.sHtML

[R08] 数值比较
来源：http://www.share.fehbvm.com/Article/details/giqufkyyg.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.zdbjq.cn/Article/details/gfhovszoy.sHtML

[R09] 字符串比较
来源：http://mobile.fehbvm.com/Article/details/gohhrhadz.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fehbvm.com/Article/details/gvsczaymi.sHtML

[R10] 正则匹配
来源：http://baike.hesvh.cn/Article/details/gijvrdjso.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.hesvh.cn/Article/details/gyinmymqn.sHtML

[R11] case 多分支
来源：http://www.m.share.zdbjq.cn/Article/details/gkzwclokr.sHtML

case "$1" in
来源：http://baike.hesvh.cn/Article/details/gzbcrklyy.sHtML

start) echo "启动" ;;
来源：http://www.blog.fehbvm.com/Article/details/guofvwril.sHtML

stop)  echo "停止" ;;
来源：http://read.share.zdbjq.cn/Article/details/gngzhzfvi.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fehbvm.com/Article/details/gwnvbndzl.sHtML

esac
来源：http://www.m.share.zdbjq.cn/Article/details/gfubdkjft.sHtML

[R12] for 遍历文件
来源：http://baike.zdbjq.cn/Article/details/ggclxador.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.zdbjq.cn/Article/details/gbqspmqhq.sHtML

[R13] for 计数循环
来源：http://m.share.zdbjq.cn/Article/details/gptnueefp.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.hesvh.cn/Article/details/guoyfvzmd.sHtML

[R14] C 风格 for
来源：http://wap.hesvh.cn/Article/details/gnnqkvoup.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.hesvh.cn/Article/details/gyvyouoqd.sHtML

[R15] while 逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gpqgxtfre.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fehbvm.com/Article/details/gajfmdfzu.sHtML

[R16] until 等待条件
来源：http://baike.zdbjq.cn/Article/details/ghwpjteoe.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gjakbnlip.sHtML

[R17] 数组定义与取值
来源：http://baike.hesvh.cn/Article/details/gzhzkyihf.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gdajdjhjv.sHtML

[R18] 遍历数组
来源：http://baike.fehbvm.com/Article/details/gcbnkhaln.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.zdbjq.cn/Article/details/gmpbrpjld.sHtML

[R19] 数组长度
来源：http://mobile.hesvh.cn/Article/details/gemdfjuhm.sHtML

echo "${#arr[@]}"
来源：http://www.share.hesvh.cn/Article/details/gjsyuudkq.sHtML

[R20] 关联数组（字典）
来源：http://3g.fehbvm.com/Article/details/gjybmrmpg.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.zdbjq.cn/Article/details/gttmxudnn.sHtML

[R21] 字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/gcaqhutza.sHtML

echo "${#s}"
来源：http://3g.hesvh.cn/Article/details/gnmjlmdfi.sHtML

[R22] 截取子串
来源：http://m.share.zdbjq.cn/Article/details/guvmdionz.sHtML

echo "${s:0:5}"
来源：http://wap.zdbjq.cn/Article/details/ggggiamtq.sHtML

[R23] 字符串替换
来源：http://www.share.hesvh.cn/Article/details/gedyoepgr.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.hesvh.cn/Article/details/goaxqljqw.sHtML

[R24] 大小写转换
来源：http://wap.fehbvm.com/Article/details/ghsuqinip.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fehbvm.com/Article/details/guzrgrhim.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fehbvm.com/Article/details/gccezhpcr.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.hesvh.cn/Article/details/glyklwanc.sHtML

[R26] 命令替换
来源：http://wap.fehbvm.com/Article/details/gcsgpzyhf.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.zdbjq.cn/Article/details/ggzijwdai.sHtML

[R27] 算术展开
来源：http://3g.fehbvm.com/Article/details/gjffvgydz.sHtML

echo $((1 + 2 * 3))
来源：http://baike.hesvh.cn/Article/details/gjtnujasu.sHtML

[R28] 浮点运算
来源：http://www.blog.fehbvm.com/Article/details/gqdefaekg.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.zdbjq.cn/Article/details/gwwtujalw.sHtML

[R29] 定义函数
来源：http://read.share.zdbjq.cn/Article/details/gisccqnlj.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.zdbjq.cn/Article/details/gstyzfgns.sHtML

[R30] 函数返回状态码
来源：http://mobile.hesvh.cn/Article/details/gtgsixhqq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fehbvm.com/Article/details/gxxwfzvis.sHtML

[R31] 局部变量
来源：http://wap.zdbjq.cn/Article/details/gvkmwixrc.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.hesvh.cn/Article/details/gfltxbtdh.sHtML

[R32] 参数个数校验
来源：http://3g.hesvh.cn/Article/details/guadpvwkg.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.zdbjq.cn/Article/details/gjrsctmto.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.zdbjq.cn/Article/details/grdyefgsv.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fehbvm.com/Article/details/gqtrtwtgu.sHtML

[R34] 退出时清理
来源：http://baike.fehbvm.com/Article/details/gpljwxjio.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.hesvh.cn/Article/details/gryosojgw.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fehbvm.com/Article/details/gmmakwxau.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.hesvh.cn/Article/details/gvnwxemud.sHtML

[R36] 并发执行多个任务
来源：http://wap.zdbjq.cn/Article/details/gjnycgzgy.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.zdbjq.cn/Article/details/gechgtbhc.sHtML

[R37] 把输出赋给变量
来源：http://blog.hesvh.cn/Article/details/ghpbsdcvk.sHtML

files=$(ls -1)
来源：http://mobile.hesvh.cn/Article/details/gknpfzhgl.sHtML

[R38] 管道串联
来源：http://blog.hesvh.cn/Article/details/ggsacvynb.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.zdbjq.cn/Article/details/gkwklwokj.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.hesvh.cn/Article/details/gpyokgigx.sHtML

cmd > out.log 2>&1
来源：http://mobile.fehbvm.com/Article/details/geynyvmzw.sHtML

[R40] 追加写日志
来源：http://m.share.zdbjq.cn/Article/details/gzbutkgfc.sHtML

echo "log" >> out.log
来源：http://read.share.fehbvm.com/Article/details/guzvjhwvd.sHtML

[R41] 丢弃输出
来源：http://blog.zdbjq.cn/Article/details/gikmfpquu.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.zdbjq.cn/Article/details/gogzzzkqc.sHtML

[R42] 输入重定向
来源：http://wap.fehbvm.com/Article/details/gpmdsubot.sHtML

wc -l < a.txt
来源：http://m.share.fehbvm.com/Article/details/gavksdtrv.sHtML

[R43] 按名字查找文件
来源：http://baike.zdbjq.cn/Article/details/gsgpedwor.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.zdbjq.cn/Article/details/glthlvoww.sHtML

[R44] 按修改时间查找
来源：http://mobile.fehbvm.com/Article/details/ggxbhjlco.sHtML

find . -mtime -7 -type f
来源：http://baike.hesvh.cn/Article/details/gjvhkwidl.sHtML

[R45] 批量删除
来源：http://m.share.zdbjq.cn/Article/details/gmxozsweh.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.zdbjq.cn/Article/details/gibdivzkd.sHtML

[R46] 递归替换文件内容
来源：http://baike.fehbvm.com/Article/details/gwnbdpztl.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.hesvh.cn/Article/details/gapzuuwxm.sHtML

[R47] sed 单行替换
来源：http://www.share.fehbvm.com/Article/details/gzefveyop.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.zdbjq.cn/Article/details/ghrtjahhd.sHtML

[R48] awk 取指定列
来源：http://wap.fehbvm.com/Article/details/gsjkfagng.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fehbvm.com/Article/details/guytqdnto.sHtML

[R49] awk 带条件
来源：http://3g.zdbjq.cn/Article/details/gfzphkiad.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.hesvh.cn/Article/details/gwvehrqjf.sHtML

[R50] awk 求和
来源：http://m.share.hesvh.cn/Article/details/gazkvhpuw.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fehbvm.com/Article/details/gfxqcktkz.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fehbvm.com/Article/details/gnsfbkdjv.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fehbvm.com/Article/details/ggujxoadz.sHtML

[R52] 统计行数
来源：http://wap.fehbvm.com/Article/details/ghifbjehv.sHtML

wc -l a.txt
来源：http://3g.zdbjq.cn/Article/details/gheguughi.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.hesvh.cn/Article/details/gtpjznuna.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.hesvh.cn/Article/details/gnvmejdbg.sHtML

[R54] 比较两个文件
来源：http://www.m.share.zdbjq.cn/Article/details/gxflzupek.sHtML

diff a.txt b.txt
来源：http://mobile.zdbjq.cn/Article/details/gnzgwgmyl.sHtML

[R55] 压缩与解压
来源：http://3g.hesvh.cn/Article/details/gwxmjjgxi.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.zdbjq.cn/Article/details/gdlxphqlb.sHtML

[R56] 远程拷贝
来源：http://mobile.fehbvm.com/Article/details/ggsinodue.sHtML

scp file user@host:/path/
来源：http://blog.fehbvm.com/Article/details/gcgwszuti.sHtML

[R57] 远程执行命令
来源：http://www.share.zdbjq.cn/Article/details/ghuxaeyde.sHtML

ssh user@host 'uptime'
来源：http://3g.fehbvm.com/Article/details/gqpbzmsfe.sHtML

[R58] 下载文件
来源：http://m.share.hesvh.cn/Article/details/ggsiwehyy.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.hesvh.cn/Article/details/gfcdicjop.sHtML

[R59] 发 POST JSON
来源：http://wap.fehbvm.com/Article/details/gcvurhszp.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.hesvh.cn/Article/details/gazglklei.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.hesvh.cn/Article/details/gzcezgfnf.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.zdbjq.cn/Article/details/ghvzzcifm.sHtML

[R61] 磁盘占用
来源：http://m.share.hesvh.cn/Article/details/gmqslgddy.sHtML

df -h;  du -sh *
来源：http://www.m.share.hesvh.cn/Article/details/gfeppezys.sHtML

[R62] 找最占空间的文件
来源：http://3g.zdbjq.cn/Article/details/gtfnzgaih.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.zdbjq.cn/Article/details/gkbwukdhj.sHtML

[R63] 内存与进程
来源：http://mobile.hesvh.cn/Article/details/gfsgvckwp.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.zdbjq.cn/Article/details/gyrjctlyx.sHtML

[R64] 结束进程
来源：http://www.share.zdbjq.cn/Article/details/gmdnfoxgo.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fehbvm.com/Article/details/glxfrlwfy.sHtML

[R65] 查看端口占用
来源：http://blog.hesvh.cn/Article/details/gowegcteq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fehbvm.com/Article/details/gygvmxkgq.sHtML

[R66] 定时任务
来源：http://baike.hesvh.cn/Article/details/gkcmnquiq.sHtML

crontab -e;  crontab -l
来源：http://3g.fehbvm.com/Article/details/gxdqsjfky.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fehbvm.com/Article/details/gmwvdorxj.sHtML

openssl rand -hex 16
来源：http://read.share.zdbjq.cn/Article/details/gewjwkokm.sHtML

[R68] 计算文件校验值
来源：http://read.share.hesvh.cn/Article/details/gochixpab.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.fehbvm.com/Article/details/gdtmlmklu.sHtML

[R69] 生成随机密码
来源：http://www.share.zdbjq.cn/Article/details/gyqsfrexc.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fehbvm.com/Article/details/gfkdknovy.sHtML

[R70] 时间戳与互转
来源：http://3g.fehbvm.com/Article/details/gtfdpzueb.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.zdbjq.cn/Article/details/gpfuysqdz.sHtML

[R71] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/ghxvsmzlv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.zdbjq.cn/Article/details/gtqoiijnb.sHtML

[R72] 等待端口就绪
来源：http://baike.fehbvm.com/Article/details/gfxmvgkvi.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/gzatcpvje.sHtML

[R73] 分割大日志
来源：http://www.share.hesvh.cn/Article/details/gcvpagudr.sHtML

split -l 1000 big.log part_
来源：http://mobile.fehbvm.com/Article/details/gtuxfekoj.sHtML

[R74] 批量重命名
来源：http://read.share.hesvh.cn/Article/details/gnsrmfqce.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.hesvh.cn/Article/details/gdscvjgju.sHtML

[R75] 导出环境变量
来源：http://wap.hesvh.cn/Article/details/gqoxoefvc.sHtML


<!-- 参考信息 -->