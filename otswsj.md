代发 wailian999

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2jwsdjipp.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2jvgudgxt.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2iwpvkxau.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2vyhjvrvn.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2zxqrnhbe.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2ttmlqevx.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2loxjkjov.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2wowztvtj.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2olaofekz.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2mblpnslm.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ezjfsemr.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2qjnfvijn.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2suzqhuby.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2mdplaakc.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2blihdlyk.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2fwiovryj.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2sojpjctt.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2gdheluzt.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2xjnbsedr.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ryyozeoq.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2hlkoaqch.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2juxnohyg.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2blxeytud.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2rzvikhmk.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2wzdavnov.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2cpwmhnng.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2ojcazire.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2kxsldpaj.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2ndczrejz.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2adtkpxpe.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2wsxtbsri.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2mpqsvpaf.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2uwzqkzxp.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ykfqxyrc.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2dlmskxwk.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2chvpyhsx.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2aqwormfq.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2pbjdntbx.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2hitodsaf.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2ntsuapib.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2afaxadht.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2bvtstouo.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2cedtzrgy.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2hmrwagkl.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2zywyllgw.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2cmxmainy.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2znrswahd.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2wjntqccx.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2lkgajmmc.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2jwlzevqu.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2avlchvou.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2gwkqxavm.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2bdhvrqhg.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2opcnjpde.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2ghmayxmk.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2iypruyfj.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2atyaahap.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2ojakgukg.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2hacmuchx.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2qidrsyym.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2xvbkgapo.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2kesowusb.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2kjveynhc.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2ypwsnzke.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2exlvdrfp.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2nfvciijv.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2abugowqs.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2xnwyawsf.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2invbksuo.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2lcnevscz.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2vgadngxz.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2ielcxndg.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2ntfumpst.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2trrujwdk.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2rqatqhdz.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2pggfjnhb.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2tryuthkd.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2nprozfbn.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2pteikhlk.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2kxllrbxp.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hmgxosfo.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2vpfbllxz.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2dmvjundo.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2fkoyxeim.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2djltyatl.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2zcblbirs.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2jxknohex.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2vvltkhqg.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2hgkzdtvw.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2arnlleub.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2sanxefaz.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2fldumoyf.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2iaetvhfs.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2flczbtof.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2krwepqfp.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2svzkzcjm.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2zjpxcqur.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2ztxuwcuh.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2cwlvzewh.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2rowhgtvk.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2lmsqsolr.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2hllksamh.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2djhknsab.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2dzdrfujt.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2tkqizmtw.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2qloncgdr.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2wvdcpgcw.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2infxvzng.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2ythhlatx.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2geffxlbm.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2shazyddl.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2nivijlkq.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2knjfzjqe.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2whzqdxqd.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2qafqrpuk.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2rzgxxtye.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2izjicffv.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2oqyuvmjq.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2gzgoaqxv.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2yyngnneg.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2pbpoestm.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2fabnkwqc.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2ewczliyh.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2zsocbjjm.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2tihmgrdu.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2paothllu.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2xhyoukqh.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2nenlozxg.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2grhwxsoz.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xprvmydr.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2ojbcfvhx.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jqpryhkx.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2wvlfhwxp.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hxdimash.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2rxhscbmw.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dqjpxkja.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2qjutjpqy.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vlxitems.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2bngzqrpt.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2saejmbel.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2xefkasuj.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2difhviee.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2lzuiddpt.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2tijfuecn.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2hluqvrdk.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2udzrnwni.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bsciykta.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2fzcwetff.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2opksyzdq.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2svbrnqmr.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2ixuqbksb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wtldqmys.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2tyhncfsp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xwhdllsz.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2acmkkcwt.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2trqkkgru.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2iqxzbrmt.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2jakslvwk.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2stcwhjxb.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2jyttfmho.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2nsjqabiw.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2asoparme.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2uiufixgc.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2ohilvcdj.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2fjdvmjck.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2sxcjjdkm.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2zbclpgfy.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2uxiedxwg.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2zeuwlbzb.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2wqyzarun.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2kadukwdr.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2jzxekhwf.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2gmpvrcwf.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2oiheoydn.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2mimnduiv.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2fvykkfph.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2yxqbcanl.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ujuvcmkr.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2lukylugw.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2lciujhnn.html

esac
来源：http://www.52xcode.cn/Article/details/gt2lhfejcdv.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2qwaxzfyv.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ppkkexox.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2fwmkwhlo.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2wlqntyrg.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2ksfkcfso.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2uqeodhnw.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2nylsukuq.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2mtphytky.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2dwfjkosu.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2rzgclnar.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2vfbktsfg.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2jndpdkcg.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2ejrjihze.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2wnsbqcvs.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2jkbobjmh.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2xmhjdzni.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2nptcppyo.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2lzlfdavx.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2jturbkbe.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2nvgguwwn.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2kikojuba.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2oqgkoqfv.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2emysgnzu.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2wdynbwdg.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2fqinvszo.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2lftetmue.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2pjojlehc.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2jfsngwzu.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2fttcqafg.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2rppyblpw.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2xiyulvow.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2xvpoaiil.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2tidpyulr.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2cxfenqcw.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2yzijtouo.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2dfazcdim.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2lccyiypg.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2fswqznqs.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2orrlmsvx.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2efqdgray.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2rangnvle.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2hzrcvwgg.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2tcgaygds.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2kkkiuzml.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2qrutdogb.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2bbryxuld.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2wdjjwbia.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2wkchaywj.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2zttjlnkk.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2bznoqqgv.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2nryoqkql.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2ovleukrd.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2ztcmauks.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2bhzpozoj.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2gzoquatd.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2aoykfhda.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2vuovwjtn.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2knatpwep.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2cirtlwyr.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2ipuarucv.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2furfptat.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2rznilmvf.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2ujohsowk.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2ckrdnnqw.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2mylvdqai.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2xzsjnjbg.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2bqljoowq.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2glvakfud.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2qjbszpdc.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2wrnptdww.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2lbowjzvw.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fwhssulf.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2ndqcvoow.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2yhbarbgx.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2yurezkcx.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2jfhvdsba.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2kbvbgcly.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2lgelipnc.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2cumbgqnm.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2sykartzx.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2zzbkxdkq.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2eoiwzfnb.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2sogpmoax.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2imfibdwt.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2gyiyiypu.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2newaosup.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2ierzfmyl.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2arsciivd.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2zunhpqay.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2eymolqjq.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2ajnvonot.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2fojxncqv.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2dwgfxqwp.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2xixfsdnn.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2kurqbasz.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2ihcuvbfb.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2cxccuovp.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2fdkqovmq.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2gzfdulbv.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2nlesrwxa.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2swdwtwtd.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2iqhendcu.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2jhvttwgk.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2xizgxerk.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2jkyzdocj.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2lgmvosey.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2xqwwwuwt.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2givdjbbe.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2ktsvpipl.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2ummqzxja.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2xxextlpm.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2ivlknvvi.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2iccqjekm.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2xejoejto.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2fxhmamdl.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2gurwrjov.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2brgzmpjw.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2vjdbdliv.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2btkclkvo.html


<!-- 参考信息 -->