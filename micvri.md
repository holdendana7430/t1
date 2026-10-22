代发 wailian999

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2swoijhhm.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2lvvhmdqe.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2ewqacbwg.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2tobcauni.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2lpxpmzfo.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2nqqrutrw.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ebawklou.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2zilxnyng.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2ehuydlyl.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2gjpkydcz.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2uxwsjyce.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2klqphmqk.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2deuglhzo.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2bjtiygzu.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xlqgjigf.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2wweidbxo.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2qpaqgqjg.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2xjnjygfh.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zxzieedo.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2eoksipoz.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ecvfyyth.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2qbbsmnve.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2pcqxbxqt.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2bizfqmtb.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tmontlmg.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2lreramab.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2sgzpgmtf.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2whcczsiy.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2mrgcrnon.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2vrpkorye.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2gdrzwoed.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2nnvigrsi.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2towpunkq.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2dlovztty.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2xbiyppaj.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2mpkvinjh.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2iksylsgx.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2oxnnclak.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2vzvndgfb.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2uwwgswge.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2mkgyuvgg.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ewamrcjh.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2kgydxybh.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2juyujsfm.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2ctejvsfh.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2zwgmpbju.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2cqekadgw.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2hodlfxyu.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2qtxrroor.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2pifgusup.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2gbloigfk.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2imwvjkqr.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2ubqtxjcr.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2epujyyma.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2rkvjkeht.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2yzzozdbt.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2veltndvc.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2toddphfe.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2mhzvqgel.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2aenoomhr.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2vqjvqgdj.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2wqqytuhj.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2uxbqgbhh.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2halyjjqa.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2kuqaibrg.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2ahwirqdx.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2evcnouez.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2sdmrlrup.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2mvzerpdf.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2wecgclan.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2eucsbwmz.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2tiooecub.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2bhmvagab.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2neeygnag.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2gpozibkd.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2zxihkibz.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ofrniecv.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2ejwmphmh.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2lmfdqxgv.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2lyjdtyqf.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2bnzfcbib.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2qjnvhhjb.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2cygoksbr.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2dshnxilf.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2tgukoanc.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2clxneony.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2qtpybxxh.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2fiwptqvy.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2iniwaauw.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2tseugqmr.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2mmvallfc.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2wccqudfh.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2jtjmokxj.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2qspgmmue.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2yzurlnmi.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2rejdflbt.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2fhvmmnqj.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2fidljqbp.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2jrpebowt.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2edguupsw.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2nmzvxbuq.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2fjusvowa.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2dhskatsl.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2ivluuhgd.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2fmqiedzv.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2qldzmock.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2dstwjwtm.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2ahhtifou.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2sheoemec.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2gjtaxroq.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2jnybczun.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2wmkdtetx.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2xqmmlcxv.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2vcwlffqs.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2hvlccvkq.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2qctqsoil.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2mvzawvbk.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2gudvjrvx.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2hjthluhk.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2rqdclcfd.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bojjanpy.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2aaprlvoq.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2hacebozx.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2gdvkchwj.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2equrfyis.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2hpjmqthe.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2icwfbvgp.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2rwrnlcse.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2aoptafgh.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2kqwhxyzl.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2onddfryr.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2obdsfonv.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2ivaninkw.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2yvongczq.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2hqxjdkaz.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2dzyisaro.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2kabrlmey.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2saivqwrn.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2fmsvwwzu.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zqvixmkx.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2jedadmze.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hrkujhch.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2usngoeqb.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jskujzlv.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2sunpvycb.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2yisskcsj.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2djxkcltt.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2sgdhncxg.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2bmckddup.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2aksmqkri.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2dyzttkby.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2qfwaywcg.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2qjytdonz.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2oyalltit.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rfjvkoye.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2lqtpzldf.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2ukpcwfek.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2epxrltjc.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2yvqdlyib.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wytjstyj.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2xztkjwzx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dqizsnia.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2ffpfaxjm.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2bkrqpibq.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2grlcaxji.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2baysjpnz.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2gbxsuioy.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2ndvmnrat.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2uxnewfpg.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2dqybegjy.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2iypvmwna.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2vsbiogfr.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2yqcshtqt.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2xunrjrno.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2ldxpclvf.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2efhikpnw.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2uxemaodb.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2hywrvkyk.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2gttztysd.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2fgrdiwxg.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2iikgvbnn.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2hidpfblz.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2kqyuicjm.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2cdtupbxq.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2xjtbpgfv.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2sqfoppwt.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2zglxktvx.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2qcyhetbb.html

esac
来源：http://www.52xcode.cn/Article/details/gt2viiiiyla.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2waevuzfl.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2impoauuq.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2jbzqmduk.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2idrihmex.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2wfmkzczi.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2xjipawdm.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2skpbdgrz.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2gtvlrivd.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2jnifdwqf.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2ciyqwexa.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2obbwnnpt.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2gutmmwbr.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2ittdlazy.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2bzfmugdi.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2kgmpoxyw.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2luamremt.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2zoloojcq.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2axrxkbov.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2cknxkzcm.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2pdkefygf.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2pevqbppa.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2dpwyxwzb.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2cphzbdyg.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2hmigkbsv.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2nfhiibeu.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2dokugbkf.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2egdzbyli.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2wrxkupvb.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2dsfixicf.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2igcvtxeg.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2bizernsd.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2bgesryap.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2ppbqdclp.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2xhfxttuz.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2hfnnoown.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2bzqfrbhr.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2rgvlqqqs.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2jezsftwa.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2ccmavccb.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2akgxxedx.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2fftwuwun.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2nbnmhvvr.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2rnchyugj.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2qidtyzlh.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2ujsterzf.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2abiaceta.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2sufkohow.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2cnjkysfy.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2ukzryebm.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2hjpfymla.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2mxqhrnwd.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2irdgpqfh.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2hyohyooc.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2pdmzcybf.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2uptmxpqu.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2tinqgsam.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2wybqyqua.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2ckfgydtv.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2qitdxuzc.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2gnmdeeeq.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2xcmqvxaa.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2pvpuarvs.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2itzyyonu.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2zdiunptt.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2ivtqzykw.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2jkmlpbec.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2qbcxvotb.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2iwpknkvq.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2cahapuyk.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2hqefsbwz.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2wkzvrzxi.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2bpbyncjn.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2outqmzco.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2yvsxbcwc.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2jgzyhhlx.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2twpuiojd.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2qexrysrr.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2zlusustg.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2szelmgrp.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2ecczbqir.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2lptavexz.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2aetnaozl.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2mcjvsrqw.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2kdyevbfq.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2amzcghxc.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2rtyconks.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2jzivtjcw.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2yztymezt.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2zwnsujjb.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2rffesmta.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2hhqfxcib.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2vsyredqa.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2lievvbhs.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2skvvwudi.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ntjcdgjg.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2vtloppbb.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2becqtrwo.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2sipbdwqs.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2xktgpall.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2ielockdw.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2dxsnsdfd.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2gkssrusa.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2mfawqvqb.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2qynwuwdz.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2coaycjkc.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2nfhlqdze.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2ilecaftb.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2tzmchtyh.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2tlijdako.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2iykbmkng.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2lrlsbgkk.html


<!-- 参考信息 -->