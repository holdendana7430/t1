代发 wailian999

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2piphjxmq.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2slcorxpk.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2orykmiyy.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2vnfijxse.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2ruealqlw.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2uacisevp.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2mmscpuum.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2atjfyqli.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2kaeitvme.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2rxbpgxsk.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2wrmrfoly.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2ejgukiyp.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2cmzrhlnk.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2besfiawx.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cwzcjnlw.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2ztmeucys.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2dkzaecbt.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2whoejzna.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cvjvpvod.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2nxuloyxe.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bmvrzfvw.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2ientyubf.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2sbxjjufy.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2acsqkuck.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pksabxzv.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2albdmkpg.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2spmbubbt.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2mcskjomz.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2ruecwdtu.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2syvtfniw.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2jzryczgs.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2ynlqhcwy.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2vggtowfq.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2svnwdjgc.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2sxxuxzor.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2vukywhxv.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2ardqtijp.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2okadfhwe.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2pfwwaujn.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2vugkqntg.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2iyijfvbl.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2dzoyqmxl.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2efhdazsl.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2faxxliqm.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2gpjlrygt.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2owzzpimu.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2trnvnfxo.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2ahncuykh.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2ujmasyxk.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2zmkksgdx.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2rvtxncvl.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2zxafnsjg.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2sgqgzzpt.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2teooabro.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2cyysjium.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2ztjpyknr.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2etbrmdro.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2yiehjzne.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2rhjkfoke.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2fihqungl.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2nuewmznd.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2wdxftvmq.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2ptbjrfug.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2egwqccig.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2sqptgzkg.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2qgdsqnuq.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2wljurbun.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2yhsqghqs.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2rmleqpkl.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2lkwtdiql.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2gnzoabkx.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2kygraapl.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2wpwgfblw.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2dyotqjyz.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2ifgordbd.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2icpztrua.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2njjnmyfu.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2jhfnpxsp.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2awrnzves.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2wcvpljgk.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2jzkujfhl.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2fsekwbbn.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2hfdheovs.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2qjdfsses.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2wucmtzjl.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2agbykmse.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2llvbblrj.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2hrmfrfrn.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mczrpgjv.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2xkyddnnq.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ewfezusd.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2prnziqjs.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2tpdtikqp.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2bjossgqh.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2vqubvpdx.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2hnjkgqvu.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2mfgwvege.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ejecljmv.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2fpzhhbdo.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2tjwyusep.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2pikcijjm.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2hleuvqtm.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2pfeggmfz.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2zoeykjbx.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2xmckrhvs.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2fjinwxfm.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2imtsfasi.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2nwhsxroh.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2ueyszfqf.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2lsnxqhpt.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2mvcwbydv.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2wetusgyd.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2jtkyzxix.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2lwrguvye.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2fdtjtwcr.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2fthkmdhz.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2kjuviwiu.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2ffshhajl.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2zpkmyyaq.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2nwffliah.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hhtpdcxp.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2aftzlsml.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2pqvgsies.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2womoyjbr.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2nmenxsdn.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2upvubnyj.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2fnnyppyi.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2tmtumhbd.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2gjeelwkm.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2eezilurw.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2zbajftry.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2iscvxcbv.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2vxbdtcyu.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2anootymx.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2exyfwgca.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2evbjjfld.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2hywcgcoj.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2yjmxuewt.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2cbnsyvby.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2asqaegsi.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2plpdbdwu.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2esjwojuv.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2jnpdekih.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2oplzdlnm.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2afildrpj.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2aviejhlg.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2gkljgogv.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2tedqkeyy.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2xogpbyfg.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2xhodbzyb.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2lwmgxirp.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2xjuszmla.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2aqwqzndh.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2gyildfui.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qxarakpi.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2wsspvtzt.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2rdxrlude.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2ggiukulx.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2ydsiyjvq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pxwjrqwh.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2ljqqonet.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rdtcqlhr.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2jdxftlgp.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2kfoesipz.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2xwocuzyz.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2zygvtuhc.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2jausalfo.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2iqmwstcz.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2nromqhfp.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2njtkvivq.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2gvhlmgym.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2xdcxsbev.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2iggegvue.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2vgwoorbp.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2doitxsjk.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2gmhkikrz.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2ciwhrxhl.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2kbvavvgl.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2bfdpjzkg.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2eurpwvlw.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2wastmiiw.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2hqajujkm.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2yofudkdh.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2ziwfhtgi.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2jdulvisp.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2mqemjwtu.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2pppwhchh.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2mgnfkiuk.html

esac
来源：http://www.52xcode.cn/Article/details/gt2trolpuvx.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2ahlqciis.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2zggyrfcc.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2xhkfohkk.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2fmatigcf.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2fagksdbq.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2vtdrdpac.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2zfumtwyz.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zkkfxxva.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2hqhgbhur.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2srgwenik.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2iawhibdo.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2mfysemnj.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2swloivbb.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2cdtmgaoz.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2ksbuejkq.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2yegtbtmg.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2myetzcuk.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2qrepovft.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2psepwisp.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2kxmuamcx.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2ktsyisgm.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2yzxwncao.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2ztcqobeh.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2lcknzbfl.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2rvgsmrei.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2qkmfeshm.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2dlfnvlpq.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2gbjvpeep.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2lbyyailo.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2txxkcxtz.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2xyohtyru.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2evspmebt.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2wtmlmksq.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2qglvpvnz.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2hhrydznq.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2vipnkqpg.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2kqvujpug.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2vkcyqmum.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2dqsuujtz.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2creslqej.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2nvnarowb.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2okfjbrlw.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2dczdsslg.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2xgrnvlej.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2nntqgifc.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2nxzndhuy.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2jfudvngx.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2soqrcocx.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2iyeksvfb.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2fqagebiu.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2mpxqgtof.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2sxseutrk.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2aogrlppe.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2xobcsowb.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2ehbfwpst.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2ztaqjkja.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2etyxvcjs.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2dsdsjilx.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2jjisvptw.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2macacyvp.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2qjrkotui.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gbbqooyz.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2imlzzsnc.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2oidadksb.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2ucwpaxbj.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2cykbofut.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2yeghdwbp.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2dqyrkqgm.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2fhrvizmc.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2uwhtlumr.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2bvftrski.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mlxotqah.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2letdssnp.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ffssrjui.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2uczhjdrv.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2wphpfeqg.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2bpdmsdtl.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2dpapcqcj.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2tmxnjbna.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2vjmzrbsp.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2ihqwrdwd.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2tnhjpccc.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2rfulvvoa.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2nkcohuzp.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2cnwbdesb.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2eygnbfep.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2ufctsopj.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2ixswvutz.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2onjqsgug.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2qzbonsif.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2yiebpcjt.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2ihhyrkbv.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2ykwmodqe.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2xjmrajmu.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2irppdkuy.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2dagptgxs.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2xtgojsag.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2ncrxvjdw.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2ocdmvfkb.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2mrtzycjg.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2knhlvfzq.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2bclpbque.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2kshmowbv.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2zaujkizg.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2liihlasy.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2uvduqlcd.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2kaeciysg.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2wiiokxts.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2lgrlthfo.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2mumaffxq.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2cfmluawj.html


<!-- 参考信息 -->