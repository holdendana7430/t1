代发 wailian999

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt2coxsktyk.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2uutjlowr.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dttqgzmb.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt2pewawdac.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2jsaipjzk.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2tymyyyva.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2nnfqqqab.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2xkkgvwhh.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2moijejaq.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2enilfpzz.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2llpeindj.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2dfbjuuvp.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2eofndkcd.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2bdodhskx.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2sblbdhcc.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2rsdmpzlg.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2qqhpulgb.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2hyuqqvit.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2yzuhcwig.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2badpyvmj.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2kkftnycy.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2uvcbnbyg.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jbintlog.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2cxstdxrl.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bededehv.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2qzyjdjum.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2mvaivqcq.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2uzmxhfhd.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fhwurvzu.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2czympctr.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2iqiqnfcl.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2wwoniaec.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2fvcfrchx.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2asbliwdv.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2snbhgkbc.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2tlavipal.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2pnehqocw.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2gaanoeto.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2irvjghfb.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2rsfngyjd.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2zmvgohgh.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2impuzuto.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2jmmxtllt.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2octiigdk.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2qyltoglw.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2yuaedtqm.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2knwdnwqk.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2akllkwif.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2qivmhplt.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2rqaiawen.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2eucloayn.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2hezkhogm.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2xdrymbhv.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2giecweuu.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2nghqwdeq.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2zwqugkdv.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2jrbbboxw.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2gpyaebdw.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2akhyrijt.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2uzwxoqvu.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2dhbkvetq.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2tjhzvivr.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2qshwizbr.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2viwyfyjw.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2otpmfepf.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2uyttxoca.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2vivzofad.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2lzovixao.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2gyzihsrn.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2figxovdz.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2bxnlnuma.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2idtutgdx.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2zwdvqcgx.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2dfzysqlk.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2wdserydl.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2rybeecyg.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2flwgamsz.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2nwbtdvwp.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2oavjnter.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2zyzkgfdb.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2wclonmlh.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2ybpbvbda.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2swjvcwja.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2glzcygup.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2ztncpoxc.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2hksvwmdk.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2dzpmiylb.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2mlkojoct.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2mvyeohmc.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2wwkklzpl.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2azinxbsi.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2wovwiryh.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ofcugxpd.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2mcjeugne.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2frylnmjn.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2vynwmgzp.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2zlkegrqp.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2qijmocot.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2bagqfpfh.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2heareolc.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2icojurca.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ipdtuzis.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2osfxggrm.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2hhyhywle.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2otboxkhe.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2vtkkkubi.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2qlisuidj.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2hcpavteo.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2puuyywij.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2angqnfcp.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2tlyfllvw.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2pwrohgxx.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2gurlgfgf.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2royxesgn.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2eacoitpl.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2nmktjqur.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2qgfclddn.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2oqgscmwp.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2xmkgavmi.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2jvrjryas.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2zvxcinjn.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2viyccqxc.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2ifqxzutx.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2ggkrcpua.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2yxxisifq.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2xpgvtcvw.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2ocmrqowk.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2qwmwpuhl.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2zigfqyga.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2zkbnktcl.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ygqmjrsw.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2khaeeehy.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2lfnzjrzh.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2bnjavnwe.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2mnfqawxp.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2akiayesg.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2njhrvxgi.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2leumwncm.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2swdhcoec.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2klqtcyat.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2axqnqiik.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qilyikdk.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2echigfam.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2sgfozmwn.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2vokwmdgf.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2espvwgff.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2zsgayfwx.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rkvanrtx.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2xzbrbikt.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gdkrutyd.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2ueadfxue.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2webtjpbu.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2vqfvcsxw.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2jbiktanm.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2cloovlvy.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2rojudmlf.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2rwhivqtp.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2wsexjqeo.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2oozdqjuw.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2pzcaaorx.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2ixeitatk.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2ibkfxvag.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2wqhssskm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yjdzergr.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2uspabzut.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yvzlmekq.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2lhbgkheu.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2jfyyinfa.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2ygzarhzi.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2fvambsms.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2tqcihsxe.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2xtimwesf.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2vmkrhjxn.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2xhecrzhw.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2avmhorix.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2tluhxoup.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2jlppgrzl.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2tzsofnjj.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2ctopwzjl.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2iacifmer.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2viuqjbru.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2pvwkafxc.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2emfwjhmu.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2mlcohghe.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2qszwotdr.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2qecedzch.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2rowwvkar.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2avsatnlg.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2wfjhppjc.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2wyourbnr.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2xvezlvnq.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2vqlejliu.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2kvkjemwd.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2aahbuagq.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2uabfbtbl.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2qiphgipu.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2khqonhzv.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2qtkcytnn.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2bmwbrylp.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2yyppbodr.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2ddqgxmax.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2ecksvbqg.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2pckiqjje.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2rikdmauc.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2gypeetej.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2esossinz.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2cwirklrd.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2olityigy.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2watiflwm.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2dfjufkck.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2hfutqnjj.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2ecqvjpfd.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2maiwvvle.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2inusvexk.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2tynncrvq.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2jowakcah.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2elttbaam.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2adpdhbhs.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2uusyrqvc.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2xjxnffnv.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2kocvyclk.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2tryscpds.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2pkgttuxe.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2wmnlkflt.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2ftvjnhmt.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2dorsqaay.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2dcfscppf.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2dqeqcyyr.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2stfreaox.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2sslekwtr.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2mlmwufoq.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2rzevtroi.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2xdliamyw.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2tkhqksbb.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2bkrruqjy.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2lklrqsdj.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2cdfiledf.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2rtqrvvsx.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2cowzadkv.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2aupshzbc.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2lcgfwjmm.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2ccjltozb.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2wrufltpk.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2gkmsszio.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2ucwjkqhz.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2jjlilemr.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2cxpjylce.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2oieeglbp.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2hwkxiqoo.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2znqmcvlg.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2iqrndife.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2wedqhzfm.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2xoomtgtq.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2pkdgklml.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2kbnreqtz.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2zaypazwp.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2jqmiblkz.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2hmjqhtpa.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2fdexyhkw.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2mvcnjpoz.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2lseswaya.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2mcdmsyti.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2pzfnplml.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2xmxbnmcf.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2abammqrt.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2ucmmnydr.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2rpfsutee.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2dhyimudn.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2zzcxuyfy.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2lmsmvpqz.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xnxswkgx.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2ncwxmxgk.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2iqvdnsit.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2vwuccngz.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2zdxykyvd.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2pfucsujx.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2kqwliwla.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2ojgitpsz.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zrcyirjw.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2hgdzcbvg.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2dcvltchd.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2loqimprh.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2kskvuqwm.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2ikkdhxsd.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2odgpvxpm.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2vnjdvlcy.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2ipkhdpct.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2oebfvtfg.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2zmqxcpoo.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2mpapfujx.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2ouhuiqws.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2nlscaiwe.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2acmdlhxt.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2zcyqnpxw.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2ejewqpim.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2mulmcdxz.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2rwmegecj.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2ppuxfhkc.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2fklvivua.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2xuaxiait.html


<!-- 参考信息 -->