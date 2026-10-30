代发 wailian999

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.fehbvm.com/Article/details/gnudxubaa.sHtML

[Q26] 计数
来源：http://read.share.hesvh.cn/Article/details/gsvebozwt.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.hesvh.cn/Article/details/gvuigsjgf.sHtML

[Q27] 条件计数
来源：http://wap.fehbvm.com/Article/details/giyeuoktr.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gydypiwno.sHtML

[Q28] 求和与平均
来源：http://3g.hesvh.cn/Article/details/gvefwezkl.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gkjsgxhjq.sHtML

[Q29] 最大最小值
来源：http://m.share.hesvh.cn/Article/details/gnbvlbtln.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gspkmlymy.sHtML

[Q30] 分组统计
来源：http://www.share.zdbjq.cn/Article/details/gjfnpdiau.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.hesvh.cn/Article/details/gdjjuxfyx.sHtML

[Q31] 分组后过滤
来源：http://3g.fehbvm.com/Article/details/gbwvwaqjh.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.hesvh.cn/Article/details/gziyszstk.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gyeanagkl.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/gjwgtkfhc.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.hesvh.cn/Article/details/gpaiimflm.sHtML

[Q33] 多列分组
来源：http://wap.fehbvm.com/Article/details/gixrvfsbh.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.hesvh.cn/Article/details/grkatvvjl.sHtML

[Q34] 每组取第一条
来源：http://m.share.fehbvm.com/Article/details/gaxfrcxpt.sHtML

SELECT * FROM (
来源：http://blog.zdbjq.cn/Article/details/gmrgvrzeo.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.hesvh.cn/Article/details/grrzrxznp.sHtML

) t WHERE rn = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gaglykcih.sHtML

[Q35] 内连接
来源：http://www.m.share.fehbvm.com/Article/details/glajrgkic.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.fehbvm.com/Article/details/gbfemnxjp.sHtML

[Q36] 左连接
来源：http://www.share.fehbvm.com/Article/details/gdwzuceeo.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.fehbvm.com/Article/details/gidxgjiwl.sHtML

[Q37] 右连接
来源：http://www.share.fehbvm.com/Article/details/gffdfwlmj.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.zdbjq.cn/Article/details/glgznxmny.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.fehbvm.com/Article/details/gansrnzsi.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.hesvh.cn/Article/details/gfwzzgtan.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.zdbjq.cn/Article/details/gdaljktor.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.fehbvm.com/Article/details/gtohznmyn.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.fehbvm.com/Article/details/gbkisqzsn.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.zdbjq.cn/Article/details/gdllcferu.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.zdbjq.cn/Article/details/gpglbngun.sHtML

[Q41] 多表连接
来源：http://www.m.share.zdbjq.cn/Article/details/gdohfydxh.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.hesvh.cn/Article/details/gopwhkqdh.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.hesvh.cn/Article/details/gfeoepwdr.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.fehbvm.com/Article/details/gglbqorss.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.hesvh.cn/Article/details/gicksiwvw.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.zdbjq.cn/Article/details/gvamkigfh.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.hesvh.cn/Article/details/gkudyimuw.sHtML

[Q43] 标量子查询
来源：http://mobile.zdbjq.cn/Article/details/gyqqatkuh.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.fehbvm.com/Article/details/gwynbfnxz.sHtML

[Q44] IN 子查询
来源：http://mobile.zdbjq.cn/Article/details/gafeqzmqd.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.fehbvm.com/Article/details/gfphdglcu.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.zdbjq.cn/Article/details/gfeletmkn.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.hesvh.cn/Article/details/gxysmskeo.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.hesvh.cn/Article/details/gjheitlez.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fehbvm.com/Article/details/gxnwgdgwi.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.fehbvm.com/Article/details/gxezeqtml.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.zdbjq.cn/Article/details/gsqbuzetz.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.hesvh.cn/Article/details/gzlnlbfua.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.hesvh.cn/Article/details/gvybbxxjp.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.zdbjq.cn/Article/details/gnynlnjrq.sHtML

[Q49] 更新单行
来源：http://mobile.hesvh.cn/Article/details/gtlwwjqej.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.fehbvm.com/Article/details/gesbwyyvp.sHtML

[Q50] 批量更新
来源：http://www.m.share.hesvh.cn/Article/details/gekleoekh.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.hesvh.cn/Article/details/ghohehxmx.sHtML

[Q51] 用子查询更新
来源：http://m.share.fehbvm.com/Article/details/gaqxrmdrc.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.zdbjq.cn/Article/details/gggxtpnct.sHtML

[Q52] 删除指定行
来源：http://blog.zdbjq.cn/Article/details/gqeghdpgl.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.fehbvm.com/Article/details/gfovkhxkz.sHtML

[Q53] 按条件删除
来源：http://www.blog.zdbjq.cn/Article/details/ghaahcnkc.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.hesvh.cn/Article/details/gnzklwbrt.sHtML

[Q54] 清空表
来源：http://m.share.hesvh.cn/Article/details/gpqrrkvib.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.fehbvm.com/Article/details/gfeplqvwm.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.zdbjq.cn/Article/details/gxaiwxmym.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.hesvh.cn/Article/details/gnpxyspqm.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.fehbvm.com/Article/details/goaelhchq.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.fehbvm.com/Article/details/gfadlrzcr.sHtML

[Q57] 行号
来源：http://m.share.hesvh.cn/Article/details/giqlaibvk.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gbtrmqxfq.sHtML

[Q58] 累计求和
来源：http://baike.fehbvm.com/Article/details/ghyqpxuiy.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gtgkccxfy.sHtML

[Q59] 分组内累计
来源：http://www.share.fehbvm.com/Article/details/gjrbcntbd.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gnngraeku.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.zdbjq.cn/Article/details/gcsmrvsiy.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.fehbvm.com/Article/details/gmcvetbgq.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gcudsjmiz.sHtML

[Q61] 移动平均
来源：http://www.blog.hesvh.cn/Article/details/grsagonia.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gtyutilbb.sHtML

[Q62] 分组占比
来源：http://www.share.zdbjq.cn/Article/details/gugvkciur.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/gprhkrhjj.sHtML

[Q63] 开启事务
来源：http://www.blog.hesvh.cn/Article/details/gmhzkwgyw.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.fehbvm.com/Article/details/gmjxbmdkd.sHtML

[Q64] 提交事务
来源：http://wap.zdbjq.cn/Article/details/ghkgfhdth.sHtML

COMMIT;
来源：http://www.share.hesvh.cn/Article/details/glqrvblwu.sHtML

[Q65] 回滚事务
来源：http://baike.fehbvm.com/Article/details/ghyznjibo.sHtML

ROLLBACK;
来源：http://mobile.zdbjq.cn/Article/details/gshnkkmyw.sHtML

[Q66] 行锁查询
来源：http://baike.fehbvm.com/Article/details/giqsbiyho.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.zdbjq.cn/Article/details/gzjoezzpz.sHtML

[Q67] 设置隔离级别
来源：http://wap.zdbjq.cn/Article/details/gjiqnirnl.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.zdbjq.cn/Article/details/gmbzejclq.sHtML

[Q68] 保存点
来源：http://blog.hesvh.cn/Article/details/gsoqtgewm.sHtML

SAVEPOINT sp1;
来源：http://www.share.fehbvm.com/Article/details/guqccibqn.sHtML

ROLLBACK TO sp1;
来源：http://blog.hesvh.cn/Article/details/ggyqlavvz.sHtML

[Q69] 查看执行计划
来源：http://read.share.hesvh.cn/Article/details/gkckziciv.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.fehbvm.com/Article/details/gtmaosatp.sHtML

[Q70] 更新统计信息
来源：http://3g.hesvh.cn/Article/details/gegxfqkrg.sHtML

ANALYZE TABLE users;
来源：http://wap.fehbvm.com/Article/details/gfroxnfir.sHtML

[Q71] 查看建表语句
来源：http://mobile.hesvh.cn/Article/details/gtcbmqxck.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.fehbvm.com/Article/details/gpflehthd.sHtML

[Q72] 查看索引
来源：http://m.share.zdbjq.cn/Article/details/giinvzssb.sHtML

SHOW INDEX FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gtdacwoia.sHtML

[Q73] 查看表状态
来源：http://3g.zdbjq.cn/Article/details/gxklnvkvp.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.zdbjq.cn/Article/details/gzdoewmoi.sHtML

[Q74] 强制使用索引
来源：http://www.share.fehbvm.com/Article/details/gcunnecbm.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.zdbjq.cn/Article/details/gvyyyxjbf.sHtML

[Q75] 日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/gvbbgotgu.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.hesvh.cn/Article/details/gkrhcyagy.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fehbvm.com/Article/details/gfwetcbxu.sHtML

[Q76] 按天统计
来源：http://www.m.share.fehbvm.com/Article/details/greonwswb.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.zdbjq.cn/Article/details/gwttywgnc.sHtML

[Q77] 时间加减
来源：http://www.share.fehbvm.com/Article/details/guhkknijn.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.hesvh.cn/Article/details/gasczfbjy.sHtML

[Q78] 当前时间
来源：http://3g.hesvh.cn/Article/details/gjxmslwpe.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.hesvh.cn/Article/details/grjntoydy.sHtML

[Q79] 字符串拼接
来源：http://www.blog.fehbvm.com/Article/details/ghpthlywt.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.hesvh.cn/Article/details/gfkkvtiow.sHtML

[Q80] 字符串截取
来源：http://m.share.fehbvm.com/Article/details/gvnwopjgu.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.fehbvm.com/Article/details/gmuvybruw.sHtML

[Q81] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/ghqrniwxx.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.hesvh.cn/Article/details/gbtanrbfi.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.zdbjq.cn/Article/details/glxqerits.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.zdbjq.cn/Article/details/golblmdaq.sHtML

[Q83] 大小写转换
来源：http://wap.fehbvm.com/Article/details/gxsbskpap.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gyejjvmte.sHtML

[Q84] 去除首尾空格
来源：http://read.share.hesvh.cn/Article/details/gzknkifqf.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gcdhxijzb.sHtML

[Q85] 数值取整
来源：http://m.share.fehbvm.com/Article/details/gobbbqdhq.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.zdbjq.cn/Article/details/gswvtcimi.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.zdbjq.cn/Article/details/gfyvkvnjx.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.zdbjq.cn/Article/details/grjrfqgox.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.hesvh.cn/Article/details/geqdgbhig.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.fehbvm.com/Article/details/gpyjclojk.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fehbvm.com/Article/details/gmwaqunrl.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.hesvh.cn/Article/details/gacrvuens.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fehbvm.com/Article/details/ggfgtaxcs.sHtML

[Q89] 判断表是否存在
来源：http://m.share.hesvh.cn/Article/details/gjdsdvjtm.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.zdbjq.cn/Article/details/gjvblxhqg.sHtML

[Q90] 生成序号列
来源：http://wap.fehbvm.com/Article/details/ghaoxyvcl.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.zdbjq.cn/Article/details/gbugdkktb.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gauhcmsip.sHtML

R. Bash 专题
来源：http://www.share.hesvh.cn/Article/details/gawrqqccl.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gxwrzhfht.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.fehbvm.com/Article/details/gjuvsuive.sHtML

#!/usr/bin/env bash
来源：http://www.blog.hesvh.cn/Article/details/glyaeexof.sHtML

set -euo pipefail
来源：http://mobile.hesvh.cn/Article/details/gxzdxhiap.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fehbvm.com/Article/details/gjcmaknnk.sHtML

name="Tom"; echo "$name"
来源：http://www.share.hesvh.cn/Article/details/gdwdjpwte.sHtML

[R03] 只读变量
来源：http://m.share.hesvh.cn/Article/details/gqclgctiq.sHtML

readonly PI=3.14
来源：http://read.share.hesvh.cn/Article/details/gifvhoyps.sHtML

[R04] 位置参数
来源：http://wap.fehbvm.com/Article/details/gzautsyyz.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.blog.hesvh.cn/Article/details/gfiqcvyku.sHtML

[R05] 参数默认值
来源：http://www.m.share.zdbjq.cn/Article/details/gigdumzqg.sHtML

name="${1:-default}"
来源：http://m.share.hesvh.cn/Article/details/gtsbxhfud.sHtML

[R06] 判断命令是否存在
来源：http://3g.zdbjq.cn/Article/details/gvqrhibwo.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.hesvh.cn/Article/details/gercxoqyo.sHtML

[R07] if 判断文件
来源：http://read.share.zdbjq.cn/Article/details/gsovjsbnr.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fehbvm.com/Article/details/gguxnulih.sHtML

[R08] 数值比较
来源：http://baike.zdbjq.cn/Article/details/gjouoyvrx.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.hesvh.cn/Article/details/gecvispha.sHtML

[R09] 字符串比较
来源：http://blog.zdbjq.cn/Article/details/gaqpxfdai.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.zdbjq.cn/Article/details/gkptvuexk.sHtML

[R10] 正则匹配
来源：http://3g.fehbvm.com/Article/details/gkpkectqy.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gjruimcht.sHtML

[R11] case 多分支
来源：http://baike.fehbvm.com/Article/details/gcnuctimq.sHtML

case "$1" in
来源：http://blog.fehbvm.com/Article/details/giipdrbfa.sHtML

start) echo "启动" ;;
来源：http://read.share.hesvh.cn/Article/details/ggzrifmgh.sHtML

stop)  echo "停止" ;;
来源：http://m.share.zdbjq.cn/Article/details/gmfftgtyk.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.hesvh.cn/Article/details/gexwolebb.sHtML

esac
来源：http://m.share.fehbvm.com/Article/details/gzwmwtyia.sHtML

[R12] for 遍历文件
来源：http://3g.fehbvm.com/Article/details/gjzakujwz.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.zdbjq.cn/Article/details/gacfeelel.sHtML

[R13] for 计数循环
来源：http://mobile.fehbvm.com/Article/details/gkzdwdifp.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/gnwxecavb.sHtML

[R14] C 风格 for
来源：http://mobile.zdbjq.cn/Article/details/gyjonqjwu.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.zdbjq.cn/Article/details/gklzkqqcp.sHtML

[R15] while 逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gguegodfn.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fehbvm.com/Article/details/gjpovakwa.sHtML

[R16] until 等待条件
来源：http://mobile.zdbjq.cn/Article/details/gktfnyuxv.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/gggqpfimk.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.zdbjq.cn/Article/details/gtutgewrp.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fehbvm.com/Article/details/grpstlgcc.sHtML

[R18] 遍历数组
来源：http://www.share.fehbvm.com/Article/details/gepbaqwet.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.zdbjq.cn/Article/details/gerazplaz.sHtML

[R19] 数组长度
来源：http://www.m.share.zdbjq.cn/Article/details/gnaystkxw.sHtML

echo "${#arr[@]}"
来源：http://www.share.fehbvm.com/Article/details/gxmywumru.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fehbvm.com/Article/details/gfgduqqfp.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fehbvm.com/Article/details/gzkfnhyog.sHtML

[R21] 字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/gttusdmhd.sHtML

echo "${#s}"
来源：http://www.share.hesvh.cn/Article/details/gxggvzrmy.sHtML

[R22] 截取子串
来源：http://blog.fehbvm.com/Article/details/gxryulzkn.sHtML

echo "${s:0:5}"
来源：http://read.share.fehbvm.com/Article/details/gjzdvjrms.sHtML

[R23] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/ggdtoackn.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fehbvm.com/Article/details/govrqnxgx.sHtML

[R24] 大小写转换
来源：http://www.share.hesvh.cn/Article/details/gthqchltr.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fehbvm.com/Article/details/gowpbxprl.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.hesvh.cn/Article/details/grqqegljo.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.hesvh.cn/Article/details/gglcubmdl.sHtML

[R26] 命令替换
来源：http://baike.fehbvm.com/Article/details/gptjrcves.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.zdbjq.cn/Article/details/gobplekly.sHtML

[R27] 算术展开
来源：http://read.share.zdbjq.cn/Article/details/gqpoltfzy.sHtML

echo $((1 + 2 * 3))
来源：http://wap.zdbjq.cn/Article/details/gqodhssla.sHtML

[R28] 浮点运算
来源：http://blog.fehbvm.com/Article/details/gdzcrqmmx.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.hesvh.cn/Article/details/gryuldjne.sHtML

[R29] 定义函数
来源：http://blog.hesvh.cn/Article/details/gbfsbgixe.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.hesvh.cn/Article/details/gxkdrfkxa.sHtML

[R30] 函数返回状态码
来源：http://blog.zdbjq.cn/Article/details/gdkvaneao.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fehbvm.com/Article/details/gfoqxosiv.sHtML

[R31] 局部变量
来源：http://read.share.zdbjq.cn/Article/details/gaqendkkz.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.zdbjq.cn/Article/details/gumpjqgds.sHtML

[R32] 参数个数校验
来源：http://baike.fehbvm.com/Article/details/gmgofuoes.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/grxrwrtqm.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fehbvm.com/Article/details/gjsyhobmo.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.hesvh.cn/Article/details/gqiiiecsk.sHtML

[R34] 退出时清理
来源：http://www.share.fehbvm.com/Article/details/giovtooyb.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.hesvh.cn/Article/details/glbfhvsza.sHtML

[R35] 后台执行并等待
来源：http://baike.hesvh.cn/Article/details/giajfhzin.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.zdbjq.cn/Article/details/gerkvojgs.sHtML

[R36] 并发执行多个任务
来源：http://mobile.hesvh.cn/Article/details/glpgbymat.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.hesvh.cn/Article/details/gctxyzqrd.sHtML

[R37] 把输出赋给变量
来源：http://mobile.zdbjq.cn/Article/details/grxhgwbsy.sHtML

files=$(ls -1)
来源：http://mobile.hesvh.cn/Article/details/gybckizik.sHtML

[R38] 管道串联
来源：http://www.blog.hesvh.cn/Article/details/gwwpezqpk.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.zdbjq.cn/Article/details/ghttcbngr.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.hesvh.cn/Article/details/gghekegnf.sHtML

cmd > out.log 2>&1
来源：http://www.share.hesvh.cn/Article/details/ggyinufkd.sHtML

[R40] 追加写日志
来源：http://3g.zdbjq.cn/Article/details/ghxsipvwy.sHtML

echo "log" >> out.log
来源：http://m.share.hesvh.cn/Article/details/ghfumuepn.sHtML

[R41] 丢弃输出
来源：http://blog.hesvh.cn/Article/details/groffmaba.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fehbvm.com/Article/details/ggnxtjrgi.sHtML

[R42] 输入重定向
来源：http://blog.zdbjq.cn/Article/details/glxhrpczj.sHtML

wc -l < a.txt
来源：http://m.share.fehbvm.com/Article/details/ggpmsjrgj.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fehbvm.com/Article/details/gdfkzgval.sHtML

find . -name "*.log" -type f
来源：http://m.share.hesvh.cn/Article/details/gvydqnltg.sHtML

[R44] 按修改时间查找
来源：http://baike.hesvh.cn/Article/details/gerfmzgel.sHtML

find . -mtime -7 -type f
来源：http://3g.fehbvm.com/Article/details/gpeixubyg.sHtML

[R45] 批量删除
来源：http://read.share.zdbjq.cn/Article/details/gjniwlxeh.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.hesvh.cn/Article/details/gpavaxiaz.sHtML

[R46] 递归替换文件内容
来源：http://m.share.zdbjq.cn/Article/details/gyqvlypvd.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.zdbjq.cn/Article/details/gliouragf.sHtML

[R47] sed 单行替换
来源：http://www.blog.fehbvm.com/Article/details/gkbstvpgl.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gielkvxof.sHtML

[R48] awk 取指定列
来源：http://m.share.zdbjq.cn/Article/details/gnhuzzosf.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gyyegtlfx.sHtML

[R49] awk 带条件
来源：http://www.share.fehbvm.com/Article/details/grdoolusb.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.zdbjq.cn/Article/details/glefoebiv.sHtML

[R50] awk 求和
来源：http://baike.hesvh.cn/Article/details/gxqxnzzqe.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.zdbjq.cn/Article/details/gsjeqhjnh.sHtML

[R51] 排序去重取前几
来源：http://3g.fehbvm.com/Article/details/gbkcttpib.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.hesvh.cn/Article/details/glulnugev.sHtML

[R52] 统计行数
来源：http://www.m.share.hesvh.cn/Article/details/gtureuqsd.sHtML

wc -l a.txt
来源：http://www.share.hesvh.cn/Article/details/gmzbuoygy.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.hesvh.cn/Article/details/gccyrsylc.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.zdbjq.cn/Article/details/gzrbvdfly.sHtML

[R54] 比较两个文件
来源：http://www.blog.hesvh.cn/Article/details/gkhidznrz.sHtML

diff a.txt b.txt
来源：http://baike.zdbjq.cn/Article/details/gczvinsss.sHtML

[R55] 压缩与解压
来源：http://read.share.hesvh.cn/Article/details/glswrisog.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.hesvh.cn/Article/details/gkitfdayp.sHtML

[R56] 远程拷贝
来源：http://wap.fehbvm.com/Article/details/gehlhbfmz.sHtML

scp file user@host:/path/
来源：http://wap.hesvh.cn/Article/details/gskalfwfw.sHtML

[R57] 远程执行命令
来源：http://www.share.hesvh.cn/Article/details/ghmgoxeqj.sHtML

ssh user@host 'uptime'
来源：http://m.share.zdbjq.cn/Article/details/glemvnpbn.sHtML

[R58] 下载文件
来源：http://www.blog.fehbvm.com/Article/details/gynqqjvgq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.zdbjq.cn/Article/details/gnnucabpi.sHtML

[R59] 发 POST JSON
来源：http://wap.zdbjq.cn/Article/details/ghuxjbevw.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.zdbjq.cn/Article/details/gstjbkejb.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.hesvh.cn/Article/details/girwtgyxa.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.zdbjq.cn/Article/details/gpxmdgyff.sHtML

[R61] 磁盘占用
来源：http://mobile.fehbvm.com/Article/details/gcniklbxq.sHtML

df -h;  du -sh *
来源：http://wap.fehbvm.com/Article/details/gqluvcycq.sHtML

[R62] 找最占空间的文件
来源：http://blog.hesvh.cn/Article/details/gujbakyap.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.zdbjq.cn/Article/details/gcjusmmvj.sHtML

[R63] 内存与进程
来源：http://read.share.zdbjq.cn/Article/details/gahysepys.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fehbvm.com/Article/details/gpsgzujmm.sHtML

[R64] 结束进程
来源：http://read.share.zdbjq.cn/Article/details/ganrolksi.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.zdbjq.cn/Article/details/gpreeinxz.sHtML

[R65] 查看端口占用
来源：http://3g.hesvh.cn/Article/details/givjmoumc.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.zdbjq.cn/Article/details/giomfjshu.sHtML

[R66] 定时任务
来源：http://3g.hesvh.cn/Article/details/gpvimheqg.sHtML

crontab -e;  crontab -l
来源：http://read.share.fehbvm.com/Article/details/gsfoycknl.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fehbvm.com/Article/details/gwofssawv.sHtML

openssl rand -hex 16
来源：http://www.m.share.hesvh.cn/Article/details/gnbejubcx.sHtML

[R68] 计算文件校验值
来源：http://blog.fehbvm.com/Article/details/gfmfysejv.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fehbvm.com/Article/details/giygampbt.sHtML

[R69] 生成随机密码
来源：http://baike.fehbvm.com/Article/details/glqzovlwx.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.hesvh.cn/Article/details/gndaispjg.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.zdbjq.cn/Article/details/gnpntjzxv.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fehbvm.com/Article/details/ghflnzmey.sHtML

[R71] 日期格式化
来源：http://baike.hesvh.cn/Article/details/gndfwmnty.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.hesvh.cn/Article/details/gpxwcuocr.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.zdbjq.cn/Article/details/gllyjaxwd.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/gmhjynowm.sHtML

[R73] 分割大日志
来源：http://read.share.zdbjq.cn/Article/details/gvoodocpp.sHtML

split -l 1000 big.log part_
来源：http://m.share.hesvh.cn/Article/details/gvmbmsbau.sHtML

[R74] 批量重命名
来源：http://baike.hesvh.cn/Article/details/gfkmjmsbx.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fehbvm.com/Article/details/ggzutpdsx.sHtML

[R75] 导出环境变量
来源：http://wap.hesvh.cn/Article/details/gatdxmkdm.sHtML


<!-- 参考信息 -->