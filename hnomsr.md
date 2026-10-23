代发 wailian999

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt3jwmbweui.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.52xcode.cn/Article/details/gt3nmwvxbzx.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.52xcode.cn/Article/details/gt3yjsyuiac.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt3opomucje.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3clgnyzsx.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3ngjuhtha.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt3lctwhlla.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt3hmyxnbak.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ehohflpx.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt3rpssqndg.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt3nbatsjdj.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3jklpwzvq.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3fuaddtmu.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3jninrzuo.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ureduxjo.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3xnhwpqfd.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3punonhtn.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3zpmktzsy.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3xlawkvbc.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3aywixpex.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3dkziyobp.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3yetxkvup.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3coazllcs.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3ekvgjxgx.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3vwoyqgff.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3fszlqwuo.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xsuzfnes.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3oxsdypsl.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3aszekdir.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3ytjghajp.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3gknrptal.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3lmffzvoe.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dhnvfhtt.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3evkrqyor.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3lvicxwpv.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3nppcngob.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3noduycbn.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3jojhfqsr.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3vyhezqwz.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3hvdtjjfe.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3ecmwyfmn.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3aadpwkhe.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3tyojrdgt.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3nxuzzpnj.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3bopjeazm.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3nuaopvfg.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3apicuynj.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3kaqhnkaw.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3rokdqyxr.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3lpbmbojt.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3rebestzv.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3dfsgnxmd.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3voasscjr.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3vfxifgeb.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3ujwqvqky.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3trzsnjjh.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3anxvtkco.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3adqmyosl.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3zktizfav.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3cmopxojb.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3diyzwxzs.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3wtoacwda.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3wjhlpvad.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3yfznyxao.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3pnqgpwgl.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3wbfzosmh.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3quxjvizz.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3pvulgbkg.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3imvqjwwt.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3cujvsnhp.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3uofvbeqy.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3awjipikh.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3oxfdwyzw.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3qwhtggtp.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3lmwlufxn.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3imnisqmx.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3pasffhfn.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3mgfmomdj.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3azcyiqql.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3lejyvqax.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3orpzugmm.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3kbhpboty.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3srllxfxg.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3tpaknrdf.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3oqynltbi.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3fxmjcfdk.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3xolnpanm.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3mbozflwu.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3kinmudyz.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3kralwfij.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3ycgsynre.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3sudhvncw.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3wabpwbil.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3gkuuwncj.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3rnzmului.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3caxjxxke.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mavpsboe.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3prxdfabw.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ushsowkq.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3qxeofnlj.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3pzxsryir.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3qpsdapdm.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3zbifwyda.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ynzgngqw.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3ajdupkpj.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3fnfgexrc.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3yhnimzjz.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3fuepaivx.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3rzekiymy.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3lalgchbr.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3vsnjnkku.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3ogvytugv.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3nlpllnan.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3zdxdfdrl.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3jtboutmu.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3dwwveklf.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3avhzcdjd.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3mkzjbhjx.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3zaipfrcy.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3ufprpjty.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3eynagkmv.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3igwamtxq.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3wofglcwc.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3jamajlbx.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3ikacftsr.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3fedqszpv.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3pkaisdsi.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3xwkkhugi.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ssuymkea.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3tyneoiln.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3arnhfocc.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3smrvwgom.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3zcpqpnbr.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ydygntyn.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3egfexenj.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3yjgeouej.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3azepxgef.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3crzmfhml.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3nxyqjbhl.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3wqfugrqb.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3wvvmhpkt.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3ctfvohlh.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3iaohptgx.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3wfbubguu.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3crtwbzak.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ldqxapcr.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3begpsjvo.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3sustbtqg.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3bzglmain.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nrouewus.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3xzuezjqv.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hddaeetz.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3vqbsyvaq.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3mdpcuyjr.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3ysrpibkb.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3frjcbppd.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3rrtghzox.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3cdjjrctv.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3pwlndknv.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3nfvdrfzc.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3dkqzdzin.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3uyubkngp.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fpwgytdh.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3jdraepna.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3mbubgeqd.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3qvddvkwd.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3pxxmqboa.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kiagwnpm.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3nzdqpspv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3csiwtvph.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3xyrzrhkk.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3ajrpuzej.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3efldtmek.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3bmcbvrlr.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3hifgnnyk.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3einfbjue.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3jiabrnyz.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3obvdsfvr.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3bozyormj.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3qzwodvwc.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3vlimuada.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3mptnvord.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3irgsrhlw.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3cgzkqbok.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3qkpqzfoi.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3vaucrdqz.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3ubgkaupe.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3xfdzxrzr.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3fwtccwnw.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3dzwprymc.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3wvfecvix.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3vvfgrsff.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3hoaxwbbv.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3azxdajzv.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3eqnwvcsw.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3vgvlexcp.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3tjykydsp.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3vyhpkmzp.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3pqkbuken.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3bykpdgan.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3xvdpuksd.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3nbckupec.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3efmjuzwy.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3xsanekxn.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3csgvqcdj.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3tdslnirf.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3lhgeddzj.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3rhahogdn.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3mghtyqvh.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3xupzzbuk.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3yczfowwq.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3lwtutnrq.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3ylwwdaei.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3pdftlayu.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3rgrhjcbj.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3onkegsen.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3mxprtjii.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3vpkvsspc.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3uwyxqzvt.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3fvazpvqi.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3wsnqgmea.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3udtbykun.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3pyhoqtkn.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3aivbwnvv.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3yoyiowby.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3hzisgoqu.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3czuyetnz.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3zqbzojkq.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3ehuuifny.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3ytifoqmd.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3jbprbmta.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3shpangal.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3uxzsanbk.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3sfraoste.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3vlimwzab.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3zbfkrdov.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3dlqlsjbp.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3enylrnhn.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3mafygshf.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3mnxykuvq.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3aanvxqlj.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3nwobmekg.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3crrtrtoi.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3batkgocq.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3bwdkchjv.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3iijlskcn.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3anzaelen.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3yesennjk.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3esjepaka.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3cryyxfqo.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3ohrzbpxq.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3ilrwzyft.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3whdtakvh.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3aendnxes.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3znkkgktv.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3doihougu.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3ycdbrang.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3buteodhp.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3uduwpsti.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3aznbewgg.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3pwyrleyn.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3fpfhkefk.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3mrqymroz.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3vqvasxmw.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3tiqmzhaf.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3bshdezas.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3ggpcuojr.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3xidpzmum.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wdkopxvz.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3kazohkjs.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3dzssuqfm.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3mgpazpdw.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3usfbuwid.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3futzvdic.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3dtbivctm.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3smsptrfq.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3cvmmaooh.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3khqyfzsw.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zxhwnxin.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3qqgyytos.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3mcdzqhyd.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3qkajsszc.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3khtelhsz.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3pmiqjkkf.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3jlthvabu.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3svsoxuyi.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3ongyfpmp.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3mcqjqhad.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3vrowkodp.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3ippoquhf.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3qujsbjjf.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3zaastxea.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3vzqsvkxk.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3tiliwsdu.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3igfxxdhx.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3kpqzcgwt.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3dlvheapf.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3qutvyvof.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3nqurpxdh.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3addfudue.html


<!-- 参考信息 -->