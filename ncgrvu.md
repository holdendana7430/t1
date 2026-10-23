代发 wailian999

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt3zyfyrvmf.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3iskztiqn.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3mejxhirg.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3ohzmiejx.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3inxjckog.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3riyxljln.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3qhcmrqri.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3lideslua.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3yxxhzzvg.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3dbbksmiw.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3skhvgowj.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3pfhhgewf.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3nitglunl.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3zkuclhtr.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pqaxbfps.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3bamgwvgf.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cfsklnne.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3outqlvzo.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3dljmbrvu.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3ucdcujud.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rvkqmicb.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3bfjxupbq.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3gfbrmwzw.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3pjzdpoer.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3gfndaadd.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3tkeviaey.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3hgzapqtp.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3hbzdzxdn.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3spsadkwm.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3iyyfxqmj.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3nnvgmnkv.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3ceewcurx.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3syupyjrc.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3kebdogtq.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3mijypjzn.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3rbyspzis.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3lhrodddz.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3hlkxygsx.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3oicujnbi.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3crcajxfi.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3qyrktwcc.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3cffllisl.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3dtrydznv.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3sbsxdpcy.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3wszucnpo.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3ytpblmhz.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3dicaumtc.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3ihrgsdlk.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3hjvxnffk.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3ykmtzxdq.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3tgksixik.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3vpsumlds.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3byomweoa.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3npxlshiu.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3iehfeiya.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3oduignht.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3cwjmifwh.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3vnimzzcj.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3jfrapddm.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3ytwelxcg.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3gnovwtoz.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3byerukck.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3xppbgnyr.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3hfafmbix.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3iepibtvu.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3qfauuxxt.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3gxlnxwfm.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3lssrozog.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3jcyiatvh.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3mrhvpixd.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3bcxnnhpt.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3iyipphgd.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3dzgjmkcf.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3cfieetiv.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3svnnqdue.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3kybhyeww.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3nkouriwg.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3obvxinsz.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3uagumcoc.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3rfvloxcp.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3eqhutczs.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3jrxtyezf.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3kcmmjena.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3pudhvipi.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3skxjfpkq.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3mzpdhuqn.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3sqlpujam.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3wterzuxj.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3asodkxli.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3xkrupago.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3bvcexpps.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3agirkixe.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3ufascpva.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3hdggeiqt.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3juumvgdm.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3pudogjtu.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3vecmpcth.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3vqukekro.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3mkajsani.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3rtblfcca.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3pgsnjkox.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3cangcntb.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3zoajchev.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3clhxnimt.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3wpwuvzhl.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3kkwyighu.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3acprmdfh.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3ltdwevaw.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3cwoztudo.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3obctvili.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3ouczvgxj.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3dqddqplh.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3osqsuoeu.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3ozkkvwog.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3knrscewv.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3zymofren.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3urscmkyv.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3ueykxyff.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3iidbqjgb.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3oxsygjgt.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3cycqbuln.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3fcotharw.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3kgqxsnzc.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3mqloghsd.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3lveawdxc.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3qqibbxyt.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3eaexdjmx.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3pxyrdude.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3hxcrnawa.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3scukvaiu.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3uhurmzga.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3xnmshkkd.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3gvxbastk.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mctxixci.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3kzmafwbr.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mstfopyo.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3biuiobut.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ftnutkkb.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ugyrrtan.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3gvdubvre.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3jvnfgoda.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pctdrcqs.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3xdntukgd.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3wrysqcho.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3cgknfbut.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3mnlfjvfc.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3yzfcvzkd.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3tfvzgpjb.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3uzgzwzag.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3snzztlgn.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rajuggnh.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3mcgshujo.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3wrymurub.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3iszpdxwv.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3zjnqttgc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nxrgthfl.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3niovpkei.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3fmxyyaeh.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3ykcvqdhr.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3czpbdshy.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3tijeztgj.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3vihjzakr.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3vniblgyn.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3chnqqiof.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3uftrjuuz.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3ooyyatok.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3tzmlozfd.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3ocsntwma.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3vutnestl.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3hzhaoylu.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3fkdacfwg.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3chiwftgh.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3yskdjdxr.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3fcojubrz.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3lscqguyg.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3pmcghcpn.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3dyauuvul.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3jjfqujfh.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3tkcleiqe.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3usxwbzwu.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3glvqkulw.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3dvshvumt.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3cggbvgbv.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3hrdqvbeg.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3bywqqwku.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3mvzuzoej.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3uadmznij.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3dpfpcdgc.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3hibagalf.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3bstjgfrr.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3gsxldasl.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3gqootyba.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3stlqrehx.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3gjoczsyw.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3fxliwsrt.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3nauervty.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3jebvtedl.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3xwyxkcdc.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3npmfgdmc.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3aklzbppp.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3amahaocy.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3jqkghrni.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3gzrsacjp.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3vukawqle.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3egryvsvy.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3iokqpyid.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3sqfxhmdl.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3bztblbaq.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3ceonlynj.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ytrpwqsi.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3vffppaeo.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3farsqerp.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3irahazik.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3qbfkheot.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3gnpslkki.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3xwwgzopu.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3qasgwisj.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3flonxvsp.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3uzkzgjiv.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3rrtjmrsp.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3gfswoifw.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3fcgkmiwy.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3gzvadswm.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3ygdjfzdj.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3csefosof.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3qfrbpvyo.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3mypwhlbc.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3clgercoa.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3ekobkdie.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3fcguohql.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3wjzjospl.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3wjfgwebs.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3hbvvuuuy.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3zxdaarcy.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3eyhnnffq.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3rtcaumbv.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3uwtiqxvc.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3zenxwwcu.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3dwmjypne.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3lkzbutym.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3kplkealo.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3bjmukcpd.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3xtwkaced.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3txckagph.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3duxbtvvh.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3zzbmyuex.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3cksswoct.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3hqijjuew.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3exdiyzeu.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3oasnafgu.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3nwrgrnae.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3ykjngjod.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3hsecdfbe.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3ubvbizop.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3zwjbnnhm.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3vyvscqak.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3mkzybtai.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3bjocfhaq.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dppvueeu.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3kuqklvok.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3twrcrdcq.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3bbtxgrye.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3dxcxmirb.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3xmrlnnpn.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3zhjtcsqc.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3dykwwkwk.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3bqtfyhno.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3vseokjqn.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3lrsgdiag.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3tqmjsfsm.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3lpyhsxbv.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3nilbfbhh.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3jmkuttxp.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3pnwgkyrm.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3fsvdjxaw.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3ivbzgxxi.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3rbcqpsvq.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3ycdyxosw.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3vraaxyme.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3xddvfhlh.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3nsxngirt.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3uvgmtwjh.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3xedneeak.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3vckafxlc.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3hwkkfoau.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3ljeivjye.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3qyluoqii.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3lpbujewy.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3zdrzoxbr.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3xxzrzvmv.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3qnctzmud.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3jecgmhnj.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3vszkgxss.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3shqftdin.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3auovfprx.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3hqssxslu.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3aumxyqef.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3exmlckon.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jaljyilf.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3bpepnzeg.html


<!-- 参考信息 -->