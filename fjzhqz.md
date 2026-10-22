代发 wailian999

INSERT INTO users (name) VALUES ('C');
来源：http://www.52xcode.cn/Article/details/gt2kukpdzho.html

SELECT LAST_INSERT_ID();          -- PostgreSQL: INSERT ... RETURNING id
来源：http://www.ydjk.org.cn/Article/details/gt2hmujgllg.html

[Q13] 忽略重复插入
来源：http://www.52xcode.cn/Article/details/gt2afuycgzd.html

INSERT IGNORE INTO users (email) VALUES ('a@a.com');
来源：http://www.ydjk.org.cn/Article/details/gt2iixoxxpi.html

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt2zmudjavz.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2lkvraodk.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt2owfzynae.html

[Q15] 查询全部
来源：http://www.ydjk.org.cn/Article/details/gt2wqrzzwqd.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mqesozsf.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2mirgpyoy.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2leociqol.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2goexhemu.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2uqbzsxnl.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2aniikqzu.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2loqjvpxv.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2lrmrabyl.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2peveatuj.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2whgruqph.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2aldztwng.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2taaeatwl.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2mdkxegwk.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2njkzsojb.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2hwesgqcs.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2tmsxnvuk.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2mzrvkcdr.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2rgfitxux.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mzrcmyog.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2upkckxyu.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2yxgtncel.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2nvapilfh.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qfwiuhvy.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2psojlyua.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fzkusgyy.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2elnhankq.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2iqvfagwb.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2rrypjdue.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vzxqndtf.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2movfnntf.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2jsqtoqgx.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2ufprgvqf.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2tvtxpdie.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2aouynmrc.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2shppxrrx.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2vhhkwhyv.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2jaugsorn.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2gbpyxxwt.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2yipuosip.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2dqygugwf.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2fzqayeww.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2xuyaeaua.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2lssmzqsp.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2iykazsdj.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2nbbciibc.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2wdaylgjc.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2vlwuehby.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2viinhmhw.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2ffkjnujm.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2jvwaiqaz.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2lnjuzmcz.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2qzvavkmo.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2sobykzin.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2rfpjmblc.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2puvrqjku.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2hpcnenve.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2fxblovtm.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2ymlgpmoz.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2ttmjddah.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ydqdabqf.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2ehyzeclw.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2dexitixi.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2hjdfdcnp.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2ukxpgefl.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2hzzsithu.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2nyvakcyj.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2adhevclq.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2cfentacw.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2aczimxks.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2pnkdmkxq.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2ghasdmtp.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2aaczsvgz.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2zpiupakc.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2zadktcjs.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2wvdvfxsu.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2vfiyqzhe.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2hmdixpit.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2rsbddzaj.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2gxrefevv.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2zhtasxlj.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2nfayvixi.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2owgjlerd.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2fbzcgbqm.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2wdupobrj.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2maqtkvxp.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2dgptpnug.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2izulyinh.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2zmyrrbdh.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2bjtxjkhx.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2spsbwoek.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2tvkrpnyw.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2zbrcrlcf.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qttrdqxs.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2wvacdllq.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ziliehjx.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2urzunalo.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2jlugainw.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2qnclrcbg.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2fnvetuwk.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2swrciuws.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2bfoodvpw.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2hmxghges.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2itmspdfb.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2ncvkhkdy.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2llboyqmy.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2aaeyqctp.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2nlqbmkoo.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2ongvwmwq.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2gohnrttq.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2mxwkylgy.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2wbrnxlev.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2btmovnxj.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2itgppqrp.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2ruszrvbl.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2bgvvnxry.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2aaowmkac.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2lmxoiubu.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2zjazbcbz.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2sgaxrqwb.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2kgwsxvmg.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2ovzbddgi.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2yfhghusf.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2ukisnlzh.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2gpdghjrc.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zsfuxldi.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2fxqdtudg.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2kygzpwqy.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2dhpmridh.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2slvombjg.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2zahaicia.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2djwtxkve.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2puhtldfj.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2scxvpsep.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2jnneivlq.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2eislwqte.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2rpnbapho.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2peojoeyu.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2icnqgjob.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2unziqkcy.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2gdwzubeh.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2urjbeler.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cwdowzuq.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2zbmxmhgu.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mizijpkp.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2canlcupn.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ntprxmsl.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2hjdoytvq.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bqzwiprv.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2figdkfvt.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2harebuii.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2ymazyftl.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2oldcqpwz.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2meglzsul.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2pwswupjd.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2urenzfce.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2dnwcrthj.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2yyhkikqy.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2ujoszaxb.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dwzpiaiq.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2mospwyba.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2deylohau.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2befngrlv.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2yynwbsmp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2thawrkbl.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2bpeegmrq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fhfezgbp.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2ykbjtbmk.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2jayobyxe.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2atzcyuef.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2xnzvxnxy.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2mrenftcq.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2izdrglyu.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2hsenmoli.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2npwxnzdc.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2muvygdon.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2yaxdjolp.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2uikkvwzp.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2htgmxgzg.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2ofsxvumx.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2wynjqzgu.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2augqaoxf.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2stthvbks.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2juqtherg.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2sawyholr.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2iczsvcrd.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2eheiqvbb.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2kwnlsiod.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2pagzphbo.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2firiykuk.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2jsxrespf.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2obxippte.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2dccfjzfa.html

esac
来源：http://www.52xcode.cn/Article/details/gt2cngdgzsm.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2dnofjkcu.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2thnqnfrw.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2xcjfgzlx.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2vlmdixdz.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2kfwbgplj.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2ajgjnbie.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2fxvvmxwa.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2umgdirjd.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2lufgpqtd.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2pnzwnglv.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2jgqjayhd.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2ednseqml.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2xkiiuvzl.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2vhmdeigq.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2idxvotcc.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2gaewdqca.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2pdtcaret.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2zymjporh.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2woaewzbr.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2tnmkmvfm.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2qhvcruzt.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2xiqjtnnj.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2kmvgfjsn.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2eetsgrtj.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2wmitotvg.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2lfyphjmt.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2djvirrft.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2tkjqnueu.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2mtiikztm.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2kgwpwxnp.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2vvjzabtp.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2dgyiejjf.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2qhpbgiae.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2rjwvzsgi.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2slkxzuoy.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2nlqtszmw.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2qaxltmrq.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2yxlshfyu.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2wdtuqweq.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2juwvnpej.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2tbhnqzme.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2yufklhpu.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2udyodkpy.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2foajelqb.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2scanbkut.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2ysfminms.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2ahlxoncr.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2aeydjzbk.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2fjmgnvqo.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2gcetdbjf.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2lodjddob.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2camozmhk.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2dqtlqkxp.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2jkyrqlqf.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2tzosyuru.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2fjhbylpw.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2decwqysn.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2segqerat.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2txtjecgj.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2hetglqum.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2fuqjzqmt.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ezbjggvk.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2pobczxsr.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2yshamkiy.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2hefrufxz.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2eyhxgwwo.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2ccqfckpq.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2jyvlrrqo.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2olwkjkcm.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2kgncoqdg.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2guwjlowj.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2pmblcbqt.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2beyofpmk.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2rgisszcw.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2xgnxxoty.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2yswzhxss.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2pgeykjcr.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qjbkmfrr.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2xhpumssq.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2quzvcezc.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2hhbuiqvl.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2uznrkbum.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2yvsowhwc.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2zgrecfzv.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2jkumaysd.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2opijoigg.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2hhyykdvz.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2rcgshwoh.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2bfzfrbwz.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2cwznyhrg.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2ylvsbxrc.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2vkzjixrt.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2clupmhxg.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2uedjoumb.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2swgcxbep.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2qtuzjlhv.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2melxckcm.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2axwnwyty.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2msqqwmdm.html


<!-- 参考信息 -->