代发 wailian999

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ysttjxdt.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2inezudhe.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pwhgcfag.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2msrgywul.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2rtquabvg.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2rmsqsuog.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2fjdkqfkt.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2ludwzchv.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2ggpejmxa.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2crgawqod.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qziscexl.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2izofpiay.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2icmeqhtb.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2xzrfsbde.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2nfchjkce.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2qysgrjka.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2uuahckem.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2pscycuiy.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bsvefuoy.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2dltfhvfc.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2xgqdvhnh.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2mkdhbdlj.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dlhcibtx.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2wuiyjngz.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gjhnkpxn.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2emeuduck.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ngrrzbub.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2mnqhlyzl.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zgbioggr.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2relnehsr.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2wwlbjjbd.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2qbpflmtt.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2zuhpwpyw.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2ejedrrzl.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2dehztlrw.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2ajotvbij.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2oieeqyvd.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2nbshdawz.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2byuedpzq.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2amxqpaor.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2qcuqhtti.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2cxbhwoor.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2gpsdndit.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2emperbri.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2cklinmpl.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2xnihchcw.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2yekvdwsn.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2ucornpgv.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2qmlcauyc.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2ewydivet.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2wdegjkij.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2vmpcepjg.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2gcigorfh.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2waspciuc.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2yeydnrkt.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2tnvhpgvu.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2umukaolr.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2irmskzqt.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2wablmbne.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2ixycpwfu.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2oemchcsf.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2cktqtfvq.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2cgxuaqpm.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2jvowimqf.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2hkjviszs.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2eqikljtt.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2ntgmqjel.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2vdmdxhty.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2kkuipspn.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2urltnxyr.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2hjjrnwff.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2fgrtmxer.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2wuqdoleo.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2ugncmypn.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2mlelxwzd.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2njfgedjv.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2scsxbbdz.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2vrfovbxd.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2tqnhlpgf.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2sppurdtk.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2batvjbok.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2zqaxoicm.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2btvkjqxj.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2nhgrkhrt.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2tkeldhrg.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2trmieteh.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2fezjkcrj.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2bbfrphgl.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2gvxfnizg.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2gnephkpx.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2bufohdsd.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2kwfszisj.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gcxegrax.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2latjenax.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2wfrqzqch.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2bfdjamlb.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2hyqbyuuq.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2maluoplc.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2nbivkfuc.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2uolviluy.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2zcpuajms.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ydoxyqrl.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2qvarvcpd.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2pcuooxzw.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2ajgtmbgp.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2loysemyx.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2veljvpdi.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2fdwqdeyv.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2mliecnrb.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2cpblbzlq.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2iuxiqhdz.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2tvsqbpki.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2yurvutla.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2oydeqntv.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2jzuffdma.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2azbwvmtn.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2ulticcoc.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2yrhthkbs.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2rksnmwgy.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2mznmpupz.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2lxwsojew.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2kzgfyink.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2pzmcdesc.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2vaobdduy.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vxncrgii.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2xggmdwot.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2zfgcokwa.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2skyvnedc.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2meyikvzz.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2hhflbcuo.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2xjuevszu.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2debhczfb.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2pkdaxqgj.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2jrunlmgs.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2ojwppccl.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2vzptczvb.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2tgmhqytd.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2ptpcfbso.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2dbmhftxr.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2oqretxzq.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2iycjisxo.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lyztendr.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2xrrnszzo.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pbxssxgl.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2bfulssms.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qxclavqr.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2drqdgmez.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vovkgbqv.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2zkfbqtya.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jmolfmyj.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2gifplfdq.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2zsxwvmbr.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2cyylsspp.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2xbhikduy.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2xixvezym.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2ontwnnrx.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2rjpxrqsj.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2zbafopmc.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2caqfmmzb.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2qhbpwzvn.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2mydjxpvz.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2ywbutepg.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2octazbcc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ittrrpvi.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2ufnadafb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2crfqxodr.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2gbxghbcu.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2itkmnnkl.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2tcewjfeb.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2vimakrgd.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2zszmdgmf.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2wpvkrrqe.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2tksshern.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2ouiviyge.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2yziwjece.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2xvpqvvmd.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2sxubredd.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2khyocqff.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2mvwevllb.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2aweauvlz.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2yfzfasau.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2emzzzerb.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2wucidcry.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2qmpqtdgg.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2jglxblmd.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2bjymhkkp.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2evlxzybo.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2krnpoxwr.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2bqrtgkih.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2cxjcgdky.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2jilzokxf.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2yospqlht.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2kmcifcrk.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2pbrgyasx.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2dedadofz.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2ynsfvymo.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2vtrmgydl.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2aojvkjsz.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2cyvxldcd.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2knkdsfqv.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2feasbumd.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2lmndodeb.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2gesdvxky.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2esdtuvpw.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2nimfjmil.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2beabpwrh.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2eyixikrk.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2svxxsqst.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2dlfpqloh.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2cvfugcjf.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2dofhrbgv.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2fyueauem.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2xxueewxg.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2ksqrgvzs.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2nvoebqzs.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2xoyizveo.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2kmdutubn.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2zgurxoxr.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2rssslxmn.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2jdnyldmk.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2aswdrbbt.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2tmldtzsd.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2ylvfgtjq.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2pbjucpjh.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2szfmlvkm.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2jqknraeo.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2cktudxng.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2mxzttnsl.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2umlwiukg.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2kzqmxpyd.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2aelsepfx.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2gmvgktyf.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2xijanhyb.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2gecqvgoi.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2kkqymvyf.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2bjoiiulx.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2hkbrvfhi.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2ymmdsurw.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2flpyuveh.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2pdezmbcc.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2eilqctcp.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2lbqlgjfl.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2ulhhtdvs.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2cnwzydfv.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2gdppalzj.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2mnpnbqgx.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2lzvdrbdt.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2ocvdguhe.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2kqyqcovj.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2baddnhgk.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2wpxduahs.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2hlwtfjll.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2kapzfzzj.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2ztlquwyy.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fssvnpic.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2upxvtdux.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2zukttadj.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2nhjvygpt.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2hovmjqde.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2zjfggess.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2kmoecctu.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2mlmgzkqp.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2anuagzwa.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2gckwjhiy.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wqvaejwc.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2kqkqzihk.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2milaypmy.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2iglbvnvj.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2hkzntbvj.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2tyfsbkku.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ppbvlhgy.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2urtvqcoi.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2hsrtgmgf.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2seeheknd.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2fbfomynx.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2nacskawk.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2wrxyiyeb.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2kbuvwejp.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2osbdaxyj.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2exeoovnl.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2psralywa.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2sgjhfulv.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2pkgqibtg.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2xazrwuyk.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2vdxlfcya.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2zpmmymyt.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2vvcapnhr.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2qlkogouu.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2qrxsutts.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2wyauhiwj.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2kbflxocy.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2iocmhldz.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2iqpycqcq.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2qxlivxtm.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2jjhttztl.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2iuirspij.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2kmyjpwpz.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2ynuqkvdt.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2yckxcnoq.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2trouleec.html


<!-- 参考信息 -->