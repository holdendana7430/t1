代发 wailian999

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2utudnuii.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2fjgcgrmj.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2ohjuvwlr.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2gemcnwcn.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2vmwvejqh.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2ltvejxje.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2gocrikxc.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2iffqlbsi.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2gwdrvelz.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2ffyvgbpb.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wlmvwlph.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2dyijmuqa.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2ckhvaprj.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2bjmohlla.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zqshdbhm.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2ddsvuvrf.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mcjfjxbl.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2swdagnva.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2vtyduviz.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2goirllkg.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2misvzoet.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2yvsdarxa.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2pqbifbis.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2ncrkzbxv.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2lqugbffg.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2rqabfokm.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2mhoyqfiz.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2veyapbgg.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2dprgsiys.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2kjezzief.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2ivdzltnw.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2rfiywcjx.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2nssjwdfw.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2lmhoxyct.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2kegkrstz.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2blmlenhs.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2yqqqjwjb.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2dbdvqwyq.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2ulgqbyxq.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2pvkocecm.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2yagkxbch.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2wicoefvj.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2lodcexxt.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2tfkloqnz.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2dzhjuzyh.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2fwvethsw.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2frhettnu.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2gehgasrl.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2kcsucygu.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2ewxavilk.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2upfzxvei.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2onkjifkk.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2glhutkdd.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2kwlcfepn.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2juhknqin.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2zzncixvn.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2orjhqiui.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2flnrueaf.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2cwlcshga.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2ncrmadvj.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2hvrakoat.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2xahvhbpj.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2tiuigien.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2qivtrhkj.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2vlvhhjip.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2thxeuxtn.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2ywklolgi.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2mydihwlq.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2aoonqhzn.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2bmnhahar.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2imquloax.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2lfuuopzi.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2eotphkte.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2tmlxwzgj.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2hpehwize.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2ivvaailh.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2gkhikcys.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2lgerrzur.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2dsteciqm.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2jrujqcfn.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2kfpahvjp.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2hdmblnpe.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2ufzhhsjw.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2coukxdke.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2guqrdluu.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2eyziyigd.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2loxcyhbz.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2vmfxdfig.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2nadebyjp.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2hjqqldvp.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2ibcxthbx.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2sgopqwff.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2qosiwqnk.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2fsnunkya.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2pznrclcl.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2uprcmngq.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2pxechkbf.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2yspxfpav.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2ezctgaar.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2ucummnkw.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2cgpsigbf.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2ajgnyljh.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2byphlqqk.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2wunigoyf.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2lwtwodds.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2bcjdrwhx.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2nctylwoc.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2bxriggxs.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2waafsunc.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2fvqjsyyd.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2avcfavuz.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2sgmgkfqx.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2cvqoleji.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2hcyeqeql.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2wbzatdvo.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2wwrwritk.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lezgjhvp.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2igaiqfjg.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2guvetccn.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2waqtcwko.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2nsafgjnn.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2qdbjfyuc.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2aqoodlpg.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2anpjcxos.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2aoudszjg.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2wcmelqrt.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2tyvsgjcx.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2hfmmfvdy.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2dzawvvjv.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2gaxacpux.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2zabutymz.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2etjikhrj.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2iiifqxzl.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2phtthfui.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2pseindyc.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ukscfnxv.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2jtjbiwdf.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jyzmdxkc.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2cgusnqvy.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qwziupfu.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2poregyzi.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2knllnnow.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2kcjazgwt.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2vhnjhssr.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2kjicaons.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2uwibodmf.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2dxnhrrpk.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2uazrfrow.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2pwapwthj.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2yangseyp.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pftypqdu.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2wofxzzlx.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2lfavkzkt.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2ldqnkrcb.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2gdmauvfp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hjcnfqjd.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2tkobvlwl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vvrefqlm.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2hmazxoyl.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2afcwottz.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2pcgatfob.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2gfszftws.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2iqquolsq.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2xjrdptmo.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2bxqurcwc.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2mlvdzkmu.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2hwvaaqoo.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2rwaqolru.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2kpeogued.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2cqvomhcj.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2fosxlisu.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2xomzexfj.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2axarcsqd.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2ypbctalz.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2zlnfbdeh.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2isiymsxl.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2otffqahb.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2bohcaytk.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2cylvznfb.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2lpvamhan.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2dfzsoqom.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2jueersie.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2ftzoshpw.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2rnooatew.html

esac
来源：http://www.52xcode.cn/Article/details/gt2rdxohpgp.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2mcdayghv.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2rgkoppor.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2ajpxdmau.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2kytpudrk.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2fuxlygxn.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2asztjgmb.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2dcmwhnix.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2anizuxdk.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2uqpvailx.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2uwvgnzho.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2zhckldtu.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2wvyykkpe.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2qljcqdkc.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2qqaglniu.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2smrsmfkg.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2kqbeqakq.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2wrwqggbk.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2drdeptdg.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2mhtqimfq.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2wmxmxgdg.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2vjjqbbht.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2umwkiuyi.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2zyuunfxe.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2btcfohtv.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2naqppmfd.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2ksyyiwhx.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2bugzoiff.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2qpefgmtg.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2mbmxfrhi.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2bfjdvvan.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2puwjjgcc.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2yklxwgze.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2umwkomfz.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2udgqhnyb.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2crvbefxw.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2rbggklsg.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2thlkpcdg.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2zazpyzby.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2uvhwpaxr.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2hcqpilhr.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2imzhusxj.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2aakfjthi.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2zpnrququ.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2ozzkdocp.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2gluucbah.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2mapytmdf.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2jujmzgsh.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2piqxofuv.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2akyrfgaj.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2ipuyrier.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2aoserzit.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2axrirhxp.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2msvpyokt.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2vmcolfwv.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2cbeoscds.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2ntbydhnc.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2zkjxgjsj.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2njogcmow.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2ylizqaaq.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2cuozlkwf.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2pbyheiew.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rkmilhjt.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2rzesiilo.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2epazsxic.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2jueztelt.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2aykakayi.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2rtgbbtpc.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2xkugowaw.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2bvjuuums.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2womwmczo.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2gxidsont.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2aiabvywp.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2svuooasx.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2mgpeqdoi.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2iewbcqxe.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2oojdyjmx.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2itwrrmhe.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2wwtgmqcd.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2wmttyldr.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2tymtnlzm.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2bcavvrtv.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2sjughcag.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2ixhgpfwk.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2lxggfexq.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2dyuxgdii.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2korymasi.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2paxhzdlv.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2lwwotkls.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2mkofgvkf.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2yldzsvjq.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2xeelnzcq.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2uwuzrakq.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2swbfecxb.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2lisumzrv.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2qgpkdvlh.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2plsppizt.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2wphpbohr.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2yftvvukw.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2bgmjgifd.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2otsyqpip.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2wvnpvkio.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2tybmahrq.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2cazdjzqu.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2bsspuhnr.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2myrixaun.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2wqdnhoys.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2fvpcmwyi.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2lwlxilzp.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2mqumwyvb.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2rtytybqo.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2sxykxtzb.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2udmyjjkv.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2rzdfzwan.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2barhmowm.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2xmhbvrhx.html


<!-- 参考信息 -->