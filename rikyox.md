代发 wailian999

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lvbbccul.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2dtvdhqrh.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2plbfxetv.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2qsfiawgm.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2xggdenjf.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2dbcfypou.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2teifzevg.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2jojrrabw.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2xmbdnctg.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2lsvsdyqm.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qnykjfok.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2uedcayaf.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2zlvtnmek.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2lycikort.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2gznmlcjb.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2bgcpeovt.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2szcpdqym.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2qqgljptb.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jtypejsi.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2lbwjqyyo.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2wjrjddia.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2xvuetrvb.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hxcwinfo.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2hdcsionn.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2glwarmdk.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2unnsfcyr.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2mkxjszms.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2bmlyrrgo.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jpmnzekj.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2wnapnhbp.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2mcjgrjsa.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2eiwrduuz.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2mhbalddb.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2bwveiqzv.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2jigbslem.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2wtaemnby.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2dvstznvn.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2fbhjylrl.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2ggopevqs.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2lxudzzki.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2mdrwxsda.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2frihpesm.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2inpwgwrb.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2pzbnizuc.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2rcgeaeie.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2sptkkgap.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2etabbyrc.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2cxrfujss.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2ilgdwfcb.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2vjgwkvak.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2nlclndiv.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2usqjjjji.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2mdnztqsa.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2tjmcllgo.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2eaqpbrgq.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2gcqkqsmq.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2upjsqycc.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2iktsurvz.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2pizcvlnt.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2amrjdrvi.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2gagrniyb.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2lghyieja.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2xhskvwxy.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2incenxze.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2ofjbwews.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2bieayomf.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2ukujlqxg.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2anldejwy.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2uxijfljf.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2timicozv.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2lhpxxrqm.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2dioklery.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2bozdndsl.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2cbkeppam.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2cxziopdo.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2lftghwlp.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2ilwaoadj.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2obxwfdie.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2tyqphxsh.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2yylhhwwa.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2fiiebwuc.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2bvsrsbmr.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2giiodurx.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2wltphhuv.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2mdvqjopj.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2qpmbzrlh.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2wlmnpnrb.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2tntwyasx.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2txjftuex.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2pfwbzprz.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2wilalsqs.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2xwoxmdjo.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fxewifwo.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2ndgxlehk.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2nidisaor.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2twjbnyfz.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2pjaqkgzy.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2lasyytbq.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2scvewqrj.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2odrkmrli.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2gkhxgbjg.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2pfgrtvju.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2mvdigtjj.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2qvmnrffu.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2lmpwnvnn.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2faxjzbgk.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2pjtkicyx.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2lahsyrwi.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2rblcqphv.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2cmmobnqx.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2uwpwhghs.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2asgesnjj.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2uzktamlg.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2vjklytqv.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2kaauyemr.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2qrujnpjg.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2xabipsqz.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2ackskpqf.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2gmncezkl.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2kqcreavf.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2regiepij.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2pymfzxoe.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2adypickc.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2pxkqxorl.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2txfhrwyu.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2pqnigdnc.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2narrpokw.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2zdwezelr.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2tasmwwep.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ifzqgxnk.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2plswtrll.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2bxrrznuu.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2qadblnem.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2lbrrrczz.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2uavdwkbp.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2xbflaeoq.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2owchcmif.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2jdhoauog.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2levggoas.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2tiphmmkv.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2ftejywuz.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2umqcnlas.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2mnwnhnje.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wksssarn.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2ehthtxmy.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lsoouxcl.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2awnviquo.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lebhqcwa.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2fbbtvlql.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lmrjnfto.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2modhqzhh.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2ktorxzpl.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2pwjoasci.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2nwutniwi.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2lssfmxqa.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2pphtjkwr.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2bdzpaqgz.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2kvqefwtu.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cmgogadc.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2hcdhowwz.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2axrsysaz.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2ykliwvkl.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2izpnxxac.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2inkvtbxa.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2yvykwlsh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cvmbwrau.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2ubcvgxcf.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2usmqagdr.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2plferxea.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2saqtithe.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2sjnbggxp.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2adhkushk.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2emdevfsj.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2zkscbzpv.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2coibwlkm.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2uymaduab.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2fghtzdcs.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2xaeinphn.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2thuydgzs.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2ndzchzxh.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ccotuocv.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2gsbvbovp.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2cfgujcaw.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2ykyjflkn.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2sswawzir.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2bhxuxtmi.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2kigzbbqi.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2mlhnzsrq.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2ubfhkatj.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2brwwrhjq.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2wlpkksor.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2eoxldwob.html

esac
来源：http://www.52xcode.cn/Article/details/gt2ezcrbwlj.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2saumiqdf.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2usdsialw.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2hysqdyey.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2xiqjoqfo.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2rlxsuiud.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2ojbuemsw.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2kzqhhmiw.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2uonhmkcd.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2anwjtuib.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2icdaznmf.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2itgkwdsa.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2byaggdww.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2lhftaphu.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2peijucrp.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2vrxlfasz.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2ijoitcuc.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2binfeevy.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2cmcmxgoc.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2dqqvujsc.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2tigvatbd.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2bjftcmov.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2isinhuja.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2iucqodyu.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2kkurkqyy.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2thwfgzbf.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2apjulfqv.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2angekglx.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2fxtbcdfr.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2ethhkwbm.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2sqdspvjx.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2dsvfpbsp.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2zpwboslk.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2olzeyxws.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2mkgvsbte.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2uaarofcu.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2nwaadrct.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2swcmhuug.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2plonfmlm.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2rmnzganj.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2kcufedig.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2prqvjdsy.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2ezbcswpd.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2vtwgcszi.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2xyldqoer.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2kzwuxuof.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2klljipzn.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2tcscfixk.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2zoewaxte.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2pohjlzad.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2yhyqevab.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2hfkpauof.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2uhmrevzb.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2flkzvdfr.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2hblklbyf.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2agpvwgli.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2xwvyqpmk.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2ncnsibbs.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2uupfwcly.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2efcuqgcf.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2naqwgapx.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2oxopqkyc.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2tczurzqm.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2nywksvhv.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2ojljtrkr.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2uvrranny.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2ttzjlxwx.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2zqnudqyy.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2vzozriga.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2ipfufkht.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2swlvhjsn.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2oocwpzbq.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2hoxxifpz.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2rmpirstc.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2dumouwyr.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2ncocovbn.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2znqdmgry.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2swocssua.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vakskpuc.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2erasonzj.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2ehvyvysw.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2wofwciez.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2llrbtbuq.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2abazhixm.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2jxclozpa.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2dnhznbsl.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vlayifnt.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2qdplkkrh.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2fknrvino.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2kzgcedqj.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2zcknfube.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2njrojnxh.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2kefaekbj.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2xxrcqyfm.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2ccuoyemz.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2yutnsajp.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2uearvrfx.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2fkjpyzgk.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2jhyjjnch.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2humrvrbn.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2xufbcuyu.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2juyvyfxg.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2welkutio.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2bkceokgy.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2zowiosbd.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2wqkskdcn.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2nwmglnza.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2beqpgpag.html


<!-- 参考信息 -->