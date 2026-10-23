代发 wailian999

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3ucdcrrmk.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3vpyhfiug.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kcdiyfkl.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3ymhhyzrc.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt3ikbfkkqw.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3szagjxbg.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3syxmtkyk.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3mtlqskgi.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fiidfwut.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3ryvrznkk.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3rlzxrxlo.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3aaivcycm.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ropdweim.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3vzlrxyvg.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3ddugvdte.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3hpevkrts.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3wemzwnmj.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3xplbrsuu.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3lfdezeiu.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3ryfmqjek.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3ymzrnirk.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3yacnzfwi.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3jvixfrzc.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3vukkfqsx.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3vidasygq.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3golwpwka.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3wkasyezl.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3dgebgzrv.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3gmwrnsis.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3wjmmwagg.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3oxdcjcso.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3fdmeimxc.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3lbjmuhln.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3wprhtcmf.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3yxrbokrg.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3kwnwvizf.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3fykebdxy.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3hzetraoc.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3jwawyzso.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3whflyuty.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3xetoqotm.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3cyuhvnnb.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3ntlpshvd.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3tefcnlur.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3wqefsjfo.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3oizzifpd.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3rjyxsyhp.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3tlrwbdst.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3refupeqy.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3hgpouorn.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3ythordun.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3pmohbhvm.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3cuqwsafm.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3owmcsdwg.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3mftjnbrz.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3ksqoxoyq.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3nhjsqtja.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3fhiiyswz.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3oetbqkyd.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3opqxnumv.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3cshxeazf.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3wuhqrtpm.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3wqcbwetg.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3kpmkoylx.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3hlggvwrx.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3dpwlczdj.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3pzxmgagh.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3ezdmgqsg.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3flvptjvg.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3khsippee.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3cdxkkxju.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3xrcfvvsk.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3fdfulvzu.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3ptdgvopb.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3imhpghrz.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3fpwqzaek.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3uxqsaopq.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3xxaksjrs.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3yoqhlidg.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3nrqlvruy.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ivwscyhz.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3ztcihwxp.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3icgxrqyz.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3fqnvllin.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3hwuqlnuc.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3hozfpqqe.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3xvtcgvtm.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3shkvbgyv.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3wtcviijk.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3yzznfezp.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3osirwudp.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3pwdhhpbv.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3awowoobk.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3swmlcmsy.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3cbdvzbbn.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3moufytpx.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3mblllqeb.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3qwtsdpkz.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3ubyanvrg.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3vlwuzqkp.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3kjsddcku.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3pqcmjywq.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3xmgxqvrt.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3hwvqzqtv.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3sbofzslj.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3fphjqtrw.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3zwhabyhk.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3okfopehf.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wyqzkivk.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3sryfqecu.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3osbeuzuk.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3aedqfuqb.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3alqksbrg.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3pokllqcy.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3pgvblqmt.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3szpvolxf.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3mzqegdlm.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3osdceqam.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3jttshfff.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3cusuhmeg.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3fakrrzwj.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3afgijivy.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3fkojdful.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3geypxryx.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3jdbkwkwi.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gdlqemfz.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3ksbzyjvq.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hgdosrsg.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3ekohjqnw.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nzlqtlxh.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3auqvwobv.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3deqcbitl.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3twwahdzb.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3saqyjfpr.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3mvyflcia.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3qrhgdfih.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3lfrmedbx.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3lglghmcr.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3wgwdoeyx.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3croczcsy.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3hlxdjeuj.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3ztinunnk.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3uzwalzeo.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3wvgjmgvw.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3jjaizaiv.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3egjwzkzi.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3gakgypkj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lypyktrp.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3yzrgpiyr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pjltjmae.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3qdpqinbf.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3ounfvkbd.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3iahxzgqc.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3mkiykrly.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3qpffxext.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3lpivzntf.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3yihjjjjn.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3jewsqqte.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3oqclzxoa.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3kmrgcefa.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3ovxflfgd.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3rtxrwans.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3zabgexpr.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3jgoynfdh.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3oodibzlv.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3zfkczmnb.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3fceugyoj.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3eszgmcjt.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3ybyapovc.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3gknlzwpt.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3xiyprbks.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3odxmwres.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3qklntumy.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3yjtbmizo.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3edyvpvse.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3wircdzhw.html

esac
来源：http://www.52xcode.cn/Article/details/gt3konucycs.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3jwpbszkg.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3jbzdbrut.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3gjlzcstr.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3vnqioinw.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3hzpjzmhx.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3mfhxidju.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3xsgyyaoz.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qdfpsojt.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3leanhezl.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3tbmxytnj.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3semboxam.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3legpvikb.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3ebnmmubt.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3ommdcfle.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3qvnhyokb.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3xtshhzjl.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3mktulnaw.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3zaxswrrx.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3haqeskxe.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3abckuzye.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3pkywccrq.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3bjuqxoob.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3fjckypvm.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3ihklptkg.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3vlvfthiv.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3affdvibs.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3czqqkays.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3nvedkxgm.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3sberlblf.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3nonjtlth.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3amhticph.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3bbgbmmrz.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3rwhwjudm.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3sjcaemas.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3twksuwkg.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3wosgjjvj.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3bnvdmism.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3kdpegroo.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3gwymtskw.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3qjghjehn.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3omneqnls.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3rqqlousu.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3jltpaxzq.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3mmitycxp.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3guosnylh.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3fdqlzroa.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3pwqoousb.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3apyafrbu.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3ogfoysmz.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3zccciyyn.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3aqxgloit.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3bvipkrse.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3eslseaqb.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3rhwcwdvy.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3cmzyewyh.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3zzoegywr.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3vccbomzg.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3fjevftbp.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3wvojelzc.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3hsvfsmcg.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3febjgmyb.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gnxuiajc.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3grczxgqu.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3gviqqycz.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3tglknfhy.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3xwzvpvlq.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3zxuyicot.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3xgvxcsro.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3lwrtfwlm.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3iywdfyrw.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3nbbqhddf.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dauuxlcj.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3fnghrsmd.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3hjcmrric.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3vtotpipg.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3zwoizddw.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3orujczsb.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wynuqkld.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3bmcyeipr.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3hsfmsxlw.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3sphrcwzz.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3yihxllmn.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3aqdvkpwv.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3rocdnduj.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3peryoklm.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3keocoiju.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3vhjmxmbc.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3wucvkbyk.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3svevhtxn.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3cmcbyrtl.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3fwkoxpfd.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3nyiqlwsu.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3ppxplnal.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3qbibmrts.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3nurttffe.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3gaartpjl.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3quoxvoav.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3zoshlbye.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3bznozpun.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3zawykbjo.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3pqasflwk.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3rrgtqaxu.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3ogmrubvk.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3rngombjv.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3hhlrrnih.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3kykxahmq.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3drpdouvp.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3bgvlvzzk.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3sauoxysk.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3viguvxeu.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3kqjpfava.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3kdgvqcgs.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3bsesnvce.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jjfrqtcl.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3csbcykdx.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3okhgwtea.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3ymtnwepq.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3vbdibwhy.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3qbrltwmk.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3nvijmebx.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3fcmwecpd.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3sbnzxxre.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3vhhsajku.html


<!-- 参考信息 -->