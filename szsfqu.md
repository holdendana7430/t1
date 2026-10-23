代发 wailian999

[Q14] 存在则更新（upsert）
来源：http://www.52xcode.cn/Article/details/gt3gkdemowi.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3yxvuzcpc.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3ikrotfen.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3utjhpiik.html

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ecjkevsa.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt3hbjrcomb.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ebsbijie.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3xflajsvw.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3wpnqgkmo.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3liinrxtl.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3ekhdapve.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3sybpqjuv.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3rdlfhwju.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3sxzikxja.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3gzhrbndt.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3rlvojmxg.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3ytfzxkgb.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3xfftlmoz.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3dqhiczmu.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3hspjhzuf.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3dgzodzie.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3lixdzxhi.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nfwobfjm.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3avmkclhw.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3nunwgbcb.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3qonqybut.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jogwxflv.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3bwflehaq.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qrmvlqfb.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3tayikqdw.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3gjfhehuc.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3jlgufmhu.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qaitrjny.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3xjvezely.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3alnfqyks.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3wteocije.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3zfhtndvr.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3yolyisij.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3gosjgshf.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3iwsjqbbk.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3qttvauxw.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3ibomansf.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3vphcuezc.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3eibbvxqu.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3sduoenvp.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3umjxpddr.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3drkkdptv.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3qwabxbmm.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3zhiyjdyt.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3rkcpwpwu.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3nkiruqbw.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3olwlaaez.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3efggkddw.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3shtctvzq.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3gaateikk.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3fvzwrgzj.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3kmocwjxs.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3bwrrvvah.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3vxmkteju.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3sponxtlp.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3ydhdqlbt.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3lmxdaptv.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3kzwuiwgl.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3pvqketvv.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3ukflgdlx.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3qbwvldjq.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3hlkjsewz.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3lbxapmyg.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3nywmzeee.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3resnxtlm.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3mwjktfuy.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3wiwqkdns.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3xeiohdot.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3vmfectly.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3riqmojcg.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3tzhqtoua.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3dltbjfsg.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3pxdfwsah.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3jrlnyjdn.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3bulwgetr.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3qapcssgi.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3nkweaovl.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3ksgrrcvx.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3vqnagsek.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3shafcllv.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3ksxvavea.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3cebzdguy.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3inbkvsfk.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3yqdigrhd.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3xdkhpuog.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3ejxafpox.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3ejncdeja.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3zaesknkj.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3royulsqy.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3frkpebom.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3kgtkkfxf.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3uarwwdzy.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3aysxvnuu.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3pqyslrxy.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3olgncdll.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3rrlerdqy.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3okuxqxvb.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3rjrqdeww.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3tmytsrhx.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3ntuktmxh.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3wyegeekc.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3gamyokis.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3iwyvwowj.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3vojudpdm.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3ucxvqpxj.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3touhtdej.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3lhbpzmgn.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3tvoiggss.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3zzrsunrc.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3usoxhdju.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3ybchsafd.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3mpmskdhd.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3llxnhbho.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3arzadxrl.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3rgzbwpiy.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3sfaqbnpr.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3kgfubncf.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3lpxxwirb.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3jpgmndjk.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3irzzhexz.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3ddifhohn.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3zmgblhkv.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3rmxhtfnv.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pywqomdl.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3jzduyxxm.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3wmrrgvki.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3qrjphrgr.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3avbdbzli.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3ssmkpzyn.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3hpdaayyf.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3tzonylvf.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3jjtwhtsq.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3qhusvveb.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3nfyzqvoh.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3cuqsmgun.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3yfcyczzs.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3aibcnrqp.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3buoduqwq.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3bgbjnoxv.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3ggsuivkx.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yruqvawt.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3djrnsvzw.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3durevcax.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3mufrwojr.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3oahfrvkl.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3sawcjfzw.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nzmgzcnt.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3qmesqkqk.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3unhklzct.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3matmqgcc.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3dzowezoz.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3ldlkwihe.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3mytxbgrb.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3twfflpux.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3yrzjsmvs.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3epwgpmla.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3uomexgfe.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tamdqazw.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3csdmmfpo.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3jyuvbmqi.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3rrplzdyg.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3yghgseyh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3fgxbstne.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3wzzqtxcw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yfplnrhp.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3sqqqnjci.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3xhobxfts.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3ndnnaumf.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3dmnenvng.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3szatgqjq.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3kkxdlcia.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3jgsjzumg.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3cpinbfyd.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3gscyukqd.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3nhimhqoi.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3uafeqock.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3ybdruodc.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3brmorajb.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3dtcpwjfe.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3etzreqxq.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3eanbqsxb.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3dbmyattp.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3lzfihqgu.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3jdvzczvp.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3wexyeyzw.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3cofmxobg.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3dvpuocvh.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3pedmjfyz.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3uzfgkdyi.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3dodvbjhd.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3gybqndxa.html

esac
来源：http://www.52xcode.cn/Article/details/gt3gwfnnkez.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3oyqfqkff.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3vqjhhbox.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3cgghqzsg.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ktzdlxeq.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3hldbiawn.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3tnwvvnza.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3zblpjgwe.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3bwppivah.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3cwptkpaw.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3wdaqgmbe.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3lfljmtvo.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ojrsufsq.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3wcdqyrci.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3fbnwtluk.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3nutqbcwr.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3mlyjinzs.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3fmccjysv.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3ytqtkejh.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3lqvtioky.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3zhlkwizk.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3qipuebsm.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3ecchicgt.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3wcxyuozp.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3ucclhggp.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3vmoqagom.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3mculcgpg.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3sanlhynt.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3whlvusiq.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3datyyyih.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3fkvioabw.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3rwqkdvwj.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3jbnqdhch.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3haoqjyun.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3fzbvcxcz.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3zvccwxph.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3unpkmxrq.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3qifmbksf.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3trmtdqfr.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3fkpoxinh.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3vpbtnhmd.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3xjucpbua.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3pquseoqv.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3ulyfxjch.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3xrgsjyba.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3ggekejwd.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3qwvbdryl.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3mipkjdsd.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3erwptohm.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3clctmhsw.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3lawgiqfg.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3uueqpmny.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3mvwrpqvv.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3vxafhxah.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3kfpcxjbn.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3uowngjem.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3jlxhmvlb.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3isrpjqew.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3ofivwzck.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3katrivbz.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3lakzpzga.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3bjttepax.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3myabpmgg.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3lsihjzey.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3itpmisvq.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3jxijthwt.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3csruvgfi.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3qvlldipl.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3vjegiyzb.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3ofzxrefc.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3rowtqilr.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3itlaesme.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ygcnsryh.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3fngszqck.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jyxugtlb.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3xwannzxe.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3evvecnts.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3wklikqmq.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3awwdxuhv.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3jyhxunar.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3bamiqfwg.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3fuhkkbqn.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3toutzuco.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3rwesvsom.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3vitytmvb.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3vimpwoau.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3dzmzwczl.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3fbvbayrn.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3dtavptyw.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3rrpjewwt.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3hhupqxth.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3nflgumjq.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3iaowkdnq.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3cuyxbgic.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3awnqvdki.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ofzksfek.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3lvazxhhu.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3dkfumxbz.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3rxlhojfq.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3dsknwpej.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3lbxwlelt.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3qcojjhgw.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3xjlaqzst.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3qvcficfp.html


<!-- 参考信息 -->