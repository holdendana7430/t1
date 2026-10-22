代发 wailian999

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2yiwwmxpk.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2tecnwbjb.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2huzgjzlu.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2jwkfapbd.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2ugtrpjao.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2juyjfgcx.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2dndimgcu.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2nggpdypj.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2wsbythgo.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2tlqfittp.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2epduljfm.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2pqessoph.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2ltnwizoe.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2hkfkoftq.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2fnzinpdf.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2pcoqlnsm.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2syylzvjp.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2jrarzkph.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xjnhgpdr.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2hgdvfhro.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xgxxyntw.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2wbvwxcxw.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2eqdzjvlw.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2fwfxvxpa.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2eckiakor.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2ltngtvtg.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2vyyxjmsk.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2bafxzxyh.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2ltvldgrq.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2tyfnjmwa.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2astycdjg.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2uhsbagsw.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2qoicnhit.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2xprjlkus.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2kdwyljtu.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2bfauvidk.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2okxehrxp.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2sgfbgzfn.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2aljhzems.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2xxbpgufh.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2nthagkzp.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2oiibwrkw.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2ozbdzric.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2hjqjjhfw.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2hffjkbag.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2vbjxurod.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2wqdbdrui.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2pjqcjwki.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2hcitxgqf.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2mhvniukr.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2fgliidyg.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2kinhlmxv.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2uynqrhzb.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2wqrhhcnp.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2wtrqqumy.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2lxyzvjee.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2vouxyaqu.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2cxfvwplk.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2chdismpl.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2xucjoyvj.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2ieddwleb.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2rxszhxfa.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2eakmmzev.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2qmgpiwtm.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2purhvaqq.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2tzxlhkhl.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2lhvsdsqt.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2sgflzovc.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2hyeiqxhg.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2uecrxkjv.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2chsedeti.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2rmpirsab.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2arbfddun.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2kqhrtruh.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2amjldlex.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2qmjeqncb.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2iwezdpfo.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2wnuxpcke.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2keqclirf.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2kamtwsiv.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2zmorrtas.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2nalnfjrg.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2episyqkz.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2srzatwmc.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2uryaygib.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2mhdkqpqq.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2glzglyiw.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2ecelxfbv.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hvxeqswu.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2qsksedkh.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2zuiojxzf.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2dvjanabk.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2rpkwyrqx.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2zpgmaumm.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2bnbeltqk.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2dmuzyhxz.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2vrvewsji.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2uxkuzncr.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2trrvfvow.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2cjwdemtm.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2tqbiflkl.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2pxvlwfti.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2kkymkkvl.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2sadcfkyh.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2sykosrvu.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2huycohyh.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2wztbqump.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2cqzcvkxa.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2zhawzzel.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2pmtziqst.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2xrmngthf.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2lkqdraqo.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2pfossgka.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2vsvtanju.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2dbyygked.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2bwiaydah.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2fkrhjtrr.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2wzojgyyf.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2vjbeiofr.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2sdvlrrqm.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zoufveyi.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2dkhsgmpe.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2opczzofg.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2bdlapkjq.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2earqvdsc.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2dcncdsau.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2oulqnxfs.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2etvmhjsc.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2csclstbm.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2yndbofoj.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2iskmanfn.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2ajngiehu.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2gjfphtxe.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2pstopaii.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2lmamjnoa.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2ccbpkhdu.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2qehutinr.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rjagmivu.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2wzakxqej.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2czaljdvb.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2pgwyevrq.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hiuhxenc.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2fhwspjhe.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ofslmnrn.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2zpqfshyy.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lomiuwid.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2qkuduiir.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2qmxrtfyu.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2fyzsrfah.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2mjaejizb.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2xvxqzhex.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2pksxkerr.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2ykiomuxe.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2lgizxadm.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2yzcdjobg.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2dmsbbqag.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2sikmumsu.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2opkdqzzc.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2wcrzxtog.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yvqivglx.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2isholqfu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cawlmalp.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2fzisxove.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2vfxvyuhk.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2vqzuhxiq.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2ecacecmg.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2okjuiasa.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2mewkjgzq.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2xunoujfm.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2ghvoztrq.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2zcatahil.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2bxdltftf.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2qvhebkii.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2pkwkgalh.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2kcdnsbuy.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2hmdnovrs.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2isuihbju.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2eddzbcqn.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2cycxfhdg.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2luqxtpfe.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2kvzgkxmp.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2rlinjjwc.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2shhdjxli.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2rxhgdivb.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2rkildxsw.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2cctidbli.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2dhksmxpu.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2vkkhnxjn.html

esac
来源：http://www.52xcode.cn/Article/details/gt2dobaldgg.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2bbouhlmw.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2jvcwgqws.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2qyreecjg.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2dznzkjor.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2rxpsjsuh.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2bscyagnz.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2jxubnzmg.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2eozwayii.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2zzqwende.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2rfoyuidj.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2qejrrksq.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2dukpcnmo.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2nhpwbdfj.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2stunitja.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2pundojdt.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2kvlvtkxb.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2kunhjxjo.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2ablacqsc.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2aecqrlrf.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2vhapgdij.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2uywvldcq.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2zshloncw.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2vxspwhld.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2qqphmpog.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2vfkhnyjo.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2jugeaomo.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2djdowbdb.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2sfsewkpm.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2izcpmgjb.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2pmodeojx.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2ahxswbka.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2vugyfjpb.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2vbbcltjx.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2gilztqza.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2koeunblf.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2pxuspxal.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2vxasmbxs.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2ytozdcdg.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2ngpiubbr.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2fyilnogy.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2noqgxyji.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2ubtfnjaw.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2qybhycbf.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2nueneiqs.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2bzeywobt.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2cdyymoho.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2epzpubpp.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2zbqxjnde.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2njtbieyx.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2zhlotahj.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2kcttrfes.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2libeazvv.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2xxeryxmi.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2hhhuzrcq.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2niiblkav.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2wgesapwp.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2bymeyslr.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2otncidkz.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2hwhijhuv.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2wikrdage.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2tpqcxwxm.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2xpnqzmnd.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2oqxlwyix.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2pfnhhnhh.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2njnreqkk.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2hxlygqin.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2urwgqysu.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2zvmqyzjj.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2txfytiky.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2qziyxgez.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2ggfhmjgd.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ugfkxctt.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2hsrgghdw.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2hwuqwygi.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2aeivfikl.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2phomvfcn.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2fsjoosgv.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vgayjjgk.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2mrrtbrfi.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2igtevopt.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2ppuonolm.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2kwotnymz.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2achdwima.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2rgazayzz.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2szxwhdcx.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2wwpicuvg.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2gclnqmln.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2dqmpkdda.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2lldscoez.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2ajvcrqgo.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2rtfrbfxe.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2lzimzxwz.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2uroqpumu.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2dtiuljco.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2vmuaovlw.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2zhfqqbxk.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2bivaafwr.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2tpxkvics.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2anguhhck.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2ngdllkno.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2vvdqlhew.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2rqqjdhso.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2sqbequyp.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2ygubbbht.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2zpjtihud.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2jgrqohnj.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2oexqmyvx.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2bxupdzvv.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2lshngqhs.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2sykgvovb.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2ncxpzhqn.html


<!-- 参考信息 -->