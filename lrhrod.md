代发 wailian999

[Q14] 存在则更新（upsert）
来源：http://www.ydjk.org.cn/Article/details/gt2yowvhafb.html

INSERT INTO users (email, name) VALUES ('a@a.com', 'A')
来源：http://www.ydjk.org.cn/Article/details/gt2bhkemtql.html

ON DUPLICATE KEY UPDATE name = VALUES(name);
来源：http://www.ydjk.org.cn/Article/details/gt2lzgyrnrm.html

[Q15] 查询全部
来源：http://www.52xcode.cn/Article/details/gt2alctwetc.html

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qmgumxxo.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2zegdypjk.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gxbqcwjs.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2viqadiug.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2dvwegybp.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2eoarrspd.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2oftegnlg.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2vmsdolqg.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2tmdijfgi.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2pgryzpgg.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2nnyxfepp.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2flnfaajl.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2qfdyxymq.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2ehryqcqx.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2rrczdygd.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2wisrxalx.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2ixexsqgy.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2huszleao.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2odpqnpiz.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2hhufubyq.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2pquiddpk.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2lnljadym.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hsfuhdib.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2hjfcjlne.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gjeslmxz.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2exfliwvj.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ocsbtgvx.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2kpyuayfy.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vmhnrybd.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2ottjentm.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2squdlwtz.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2olswburz.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2pzfwnucd.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2jhuihfte.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2zvwzohbe.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2inhwfqnf.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2shxkgvnk.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2zehwhevy.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2aitdxqjr.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2pzbqxkyg.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2zlbcftii.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2gdvxaigb.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2tlkjyafr.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2pianravo.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2swinozni.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2uctbksic.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2kydxuwxa.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2gaoyrogu.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2mbnwxdib.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2pezktyrj.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2xqjuohph.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2ygcohgky.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2bpzqrhoa.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2iwiabuue.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2iqwaittm.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2ylnetkkq.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2bwddpdbn.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2gdlonhny.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2qhzgzowr.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2ybbkdugs.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2oftdxyis.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2yffdkkso.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2trhaukpp.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2lfrorctu.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2mldgbtzj.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2hphuaree.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2eorhqlpz.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2oodkogpm.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2arrosnar.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2xyufvsfo.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2laoxvbzh.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2zckrzeih.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2gxbklekd.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2stcpnprb.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2xwdperzr.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2rousscmw.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2enfnrkvf.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2mfbaymej.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2bkddqiua.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2cocxodrw.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2oniicpdv.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2xnwmffmg.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2mvilzdza.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2aosenrke.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2zubzfapc.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2ztpgqvgb.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2mpajznfq.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2jgfwkzff.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2dnexlime.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2cxxokhfb.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2ilurckfx.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2rhiniumg.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bxjruzzt.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2zpfyitii.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2szjlnnqq.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2gzcdsgkk.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2kxadhaoi.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2dzjxfutn.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2ibsfdkcs.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2gxhxhqfp.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2gqjwbccd.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2mohtlwki.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2pjibpgvr.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2mruhewur.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2uondjcxs.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2ksbzdxgt.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2ujahherf.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2arrssmah.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2vcfksqql.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2kcqfoaua.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2cnqqcoec.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2ffavrdje.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2etapqsyh.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2ywsksqkj.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2aibvgpaa.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2jsokfbmc.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2kovqcrqf.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2nmyuulvc.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2hssisour.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2fibwkviz.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2fbuwtmib.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2vvwjknhb.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2euoiyrbb.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2sdopcnaf.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zsuxsbjv.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2moihykbh.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2nmmjajbv.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2cijznlfb.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2laahogqe.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ktlfwpfi.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2skufjmbd.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2qvqbmtom.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2mqpfkfdg.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2grbvaxqe.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2pffxwldo.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2qxagwaqc.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2hsbtgsep.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2wfejabts.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2qqowbcue.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2utkgbshy.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2zzscqaes.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zokitjln.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2mzwljusp.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lbumfyxo.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2buhchxwu.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ovyjbpqt.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2scdzodvw.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cnnlczic.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2euujaakk.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ctifgqep.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2seibqdec.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2jmphfzvw.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2pvhzpvau.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2xpdfibtt.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2zzkodfrj.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2eqmtxbfp.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2hurzekwy.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2cxwgwmwo.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kkbpfxhh.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2vysicvwg.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2elfvbzkz.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2ojyyjnao.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2jcfjqhzu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ufehvrms.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2nfzqgcii.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2erdsxasx.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2swohpwbc.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2plqitmph.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2hzgcvmmz.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2fautzthm.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2dgxfnqzz.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2ngwobbmk.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2egnnyxri.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2aecwintm.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2aerwekpx.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2crskfgnn.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2wiyuejow.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ckkllbjz.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2wwvtywvw.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2ulsuljgo.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2dbzwidrd.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2vuinvnxk.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2cpkbtxpe.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2uhcclzpn.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2xipvxymt.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2fuxpdlje.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2czhznkbb.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2sovwhlfq.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2zzltvgvw.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2miezveoj.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ijaohsgm.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2eqsamact.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2cpoapbtl.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2xptxudyn.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2icurncxs.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2tsyrvlmc.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2yowqfvng.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2ocoqzqia.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2soudekwt.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2jnfjzort.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2yyfeiaqv.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2zkotsiqo.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2zglffvuq.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2viftyssg.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2jktwijno.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2phdrtkie.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2cnztncaz.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2gvxxrciq.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2elqmsfxw.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2tgjkbndp.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2agoyxspu.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2ohfhtxnn.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2qylxtcac.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2yzjgmxse.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2zivgqqbi.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2lmvcvauj.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2pfdavwhj.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2jujspxle.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2hejmmdac.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2lzyoanad.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2vwrevfbz.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2jtrrtcpa.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2apwhlizd.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2bhnultda.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2pgtdlxho.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2mxeitygt.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2hgwbygfu.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2gkjyuwvl.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2fdwtirud.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2qfykgalu.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2rhgprapj.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2wdwsizvp.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2fqkfjqfx.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2jqxxeyed.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2nxlkkipu.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2jeqzxbmw.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2anvmuniu.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2ufkuljqu.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2sxixonwv.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2rwtqiprg.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2ssthuxqm.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2cquycbil.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2tatuebdv.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2zzsohlyx.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2stsqdaqs.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2gjyuoqrc.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2gtaukywb.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2cukgehox.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2aqscpyat.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2eribcyle.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2swwsrvur.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2dkfoxddp.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2iqwnvjww.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2okrnzvqk.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vgnwnygw.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2ceekdgpq.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2fsqesain.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2emieakvl.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2ezihpjfp.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2fpphdcxl.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2ajrdcqra.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2tnlvfulx.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2azwbvqnv.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2seymmbut.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zrtnubqq.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2injbarzu.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ecuymmzk.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2cuxohtrl.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2iwwfseoa.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2jgcguuun.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2dijdoxng.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2qtdenloi.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2mndzdyyg.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2udblnyls.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2icekkini.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2gnuysdox.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2kycgplgz.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2ibgqyvag.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2ykjljlcl.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2edcasuhy.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2vmdbvsqo.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2rofzexed.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2cqueydpr.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2mikbicdb.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2vhjuavzy.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2pkzlqqox.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2hxydseua.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2yborywko.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2tiaxctex.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2egyndpab.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2iwmvljsj.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2szlpjlae.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2yhgtikgm.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2ofbylhas.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2kdxgiwts.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2hbqacwvk.html


<!-- 参考信息 -->