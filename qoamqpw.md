代发 wailian999

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.fehbvm.com/Article/details/gskancafl.sHtML

[Q28] 求和与平均
来源：http://3g.hesvh.cn/Article/details/gnodeknuy.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gpgmjmztm.sHtML

[Q29] 最大最小值
来源：http://read.share.hesvh.cn/Article/details/gyncmcujv.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gbojbczbu.sHtML

[Q30] 分组统计
来源：http://3g.zdbjq.cn/Article/details/guzggyolr.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/grmxevubs.sHtML

[Q31] 分组后过滤
来源：http://wap.hesvh.cn/Article/details/gxqnqatqc.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.zdbjq.cn/Article/details/gviwjopha.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.hesvh.cn/Article/details/gaxqxfuvk.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/ghtaskooo.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.zdbjq.cn/Article/details/gvqvpiksj.sHtML

[Q33] 多列分组
来源：http://blog.hesvh.cn/Article/details/gjayccevr.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.zdbjq.cn/Article/details/gipwljmjg.sHtML

[Q34] 每组取第一条
来源：http://3g.zdbjq.cn/Article/details/gyosbnjgc.sHtML

SELECT * FROM (
来源：http://blog.hesvh.cn/Article/details/gxuypxibz.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.hesvh.cn/Article/details/glbhqotut.sHtML

) t WHERE rn = 1;
来源：http://baike.fehbvm.com/Article/details/govunknln.sHtML

[Q35] 内连接
来源：http://wap.fehbvm.com/Article/details/glcodlebj.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.hesvh.cn/Article/details/gojlpfstz.sHtML

[Q36] 左连接
来源：http://read.share.hesvh.cn/Article/details/gplykjzlx.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.hesvh.cn/Article/details/gcuxuuxrk.sHtML

[Q37] 右连接
来源：http://baike.hesvh.cn/Article/details/giifdqovb.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.fehbvm.com/Article/details/gkvjkyedu.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.hesvh.cn/Article/details/giopobnwh.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.hesvh.cn/Article/details/gcuxrhqtl.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.zdbjq.cn/Article/details/gkdabbthi.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.fehbvm.com/Article/details/glywcdxne.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.zdbjq.cn/Article/details/gsobqoief.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.fehbvm.com/Article/details/gqgktnubg.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.hesvh.cn/Article/details/geqcsquno.sHtML

[Q41] 多表连接
来源：http://3g.fehbvm.com/Article/details/gufcpmcdq.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.fehbvm.com/Article/details/gmnvtcxci.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.fehbvm.com/Article/details/gxzjggsgd.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gbbulmczn.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.zdbjq.cn/Article/details/gaemmtcaz.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.zdbjq.cn/Article/details/gpngngoyd.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.fehbvm.com/Article/details/ggfzpzklt.sHtML

[Q43] 标量子查询
来源：http://blog.hesvh.cn/Article/details/gvrbuxljt.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.fehbvm.com/Article/details/gzxbwscef.sHtML

[Q44] IN 子查询
来源：http://www.blog.fehbvm.com/Article/details/gquugvsiz.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.fehbvm.com/Article/details/gwdegtuog.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.zdbjq.cn/Article/details/gnvvddrbs.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.hesvh.cn/Article/details/gtpafwpnk.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.zdbjq.cn/Article/details/gzylwgsij.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.zdbjq.cn/Article/details/gmlkwaafg.sHtML

[Q47] 与平均值比较
来源：http://3g.fehbvm.com/Article/details/gohxrysgy.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.fehbvm.com/Article/details/gmwsumnsp.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.fehbvm.com/Article/details/geyhubetz.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.zdbjq.cn/Article/details/gckvptqzk.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.fehbvm.com/Article/details/gucvvburb.sHtML

[Q49] 更新单行
来源：http://mobile.hesvh.cn/Article/details/gqokokasd.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://baike.fehbvm.com/Article/details/ghvfmedoo.sHtML

[Q50] 批量更新
来源：http://blog.hesvh.cn/Article/details/gcnyqanpl.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.zdbjq.cn/Article/details/gkdpgmwcc.sHtML

[Q51] 用子查询更新
来源：http://mobile.zdbjq.cn/Article/details/gteuyaehs.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.hesvh.cn/Article/details/giduurecw.sHtML

[Q52] 删除指定行
来源：http://www.m.share.zdbjq.cn/Article/details/gtzdudwvj.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.zdbjq.cn/Article/details/gdgbdzeob.sHtML

[Q53] 按条件删除
来源：http://blog.fehbvm.com/Article/details/gddtlqttu.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.fehbvm.com/Article/details/gbfgnmjxa.sHtML

[Q54] 清空表
来源：http://m.share.zdbjq.cn/Article/details/goafoxofp.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.fehbvm.com/Article/details/gzmjviyfm.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.zdbjq.cn/Article/details/gxeenrsml.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.hesvh.cn/Article/details/gbhkfmnjx.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.hesvh.cn/Article/details/glqoojmcq.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.hesvh.cn/Article/details/gjeafgnpo.sHtML

[Q57] 行号
来源：http://www.blog.fehbvm.com/Article/details/gfwimyink.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.fehbvm.com/Article/details/gzxwuahiv.sHtML

[Q58] 累计求和
来源：http://mobile.zdbjq.cn/Article/details/gfnfebeva.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gvgqfsyka.sHtML

[Q59] 分组内累计
来源：http://www.share.zdbjq.cn/Article/details/gplkhcaoj.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gdeoqrnzp.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.fehbvm.com/Article/details/gcnogmthb.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.fehbvm.com/Article/details/gfvubvivy.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gfldidmvi.sHtML

[Q61] 移动平均
来源：http://baike.hesvh.cn/Article/details/gsxgkpxfq.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gcnchxnnu.sHtML

[Q62] 分组占比
来源：http://m.share.hesvh.cn/Article/details/gnqjkqvug.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gwqqbhzlg.sHtML

[Q63] 开启事务
来源：http://m.share.hesvh.cn/Article/details/gtnfyzbvj.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.hesvh.cn/Article/details/gvhyuayud.sHtML

[Q64] 提交事务
来源：http://baike.hesvh.cn/Article/details/gwtphthlq.sHtML

COMMIT;
来源：http://mobile.zdbjq.cn/Article/details/gwwwzctmq.sHtML

[Q65] 回滚事务
来源：http://3g.zdbjq.cn/Article/details/gmmmgccrf.sHtML

ROLLBACK;
来源：http://www.blog.zdbjq.cn/Article/details/gxbwxsfks.sHtML

[Q66] 行锁查询
来源：http://blog.fehbvm.com/Article/details/gugtzfszb.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.hesvh.cn/Article/details/gqbevzfdu.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.hesvh.cn/Article/details/ggtfocedy.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.zdbjq.cn/Article/details/gxgdeufri.sHtML

[Q68] 保存点
来源：http://mobile.hesvh.cn/Article/details/gthgoqemo.sHtML

SAVEPOINT sp1;
来源：http://www.share.hesvh.cn/Article/details/gdltpfgfc.sHtML

ROLLBACK TO sp1;
来源：http://m.share.hesvh.cn/Article/details/gvmpaiavo.sHtML

[Q69] 查看执行计划
来源：http://www.share.zdbjq.cn/Article/details/gnlkwxfcm.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.hesvh.cn/Article/details/gitgospjl.sHtML

[Q70] 更新统计信息
来源：http://wap.fehbvm.com/Article/details/gwxgxecwo.sHtML

ANALYZE TABLE users;
来源：http://m.share.zdbjq.cn/Article/details/grikcwbag.sHtML

[Q71] 查看建表语句
来源：http://blog.fehbvm.com/Article/details/gujteqpgs.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.hesvh.cn/Article/details/gdaicmcho.sHtML

[Q72] 查看索引
来源：http://read.share.zdbjq.cn/Article/details/guohlyebt.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gyduuedtr.sHtML

[Q73] 查看表状态
来源：http://blog.zdbjq.cn/Article/details/grujmhfua.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fehbvm.com/Article/details/gxgvyyfzj.sHtML

[Q74] 强制使用索引
来源：http://www.share.fehbvm.com/Article/details/ghyozxhtt.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.fehbvm.com/Article/details/gqnwwrxnk.sHtML

[Q75] 日期格式化
来源：http://read.share.zdbjq.cn/Article/details/ghqejnovl.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gwvdoghse.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fehbvm.com/Article/details/gfcxndfbh.sHtML

[Q76] 按天统计
来源：http://baike.hesvh.cn/Article/details/grjbqfldq.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.fehbvm.com/Article/details/gafxyxtab.sHtML

[Q77] 时间加减
来源：http://read.share.fehbvm.com/Article/details/guteaclwl.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.hesvh.cn/Article/details/gfxnlelps.sHtML

[Q78] 当前时间
来源：http://baike.fehbvm.com/Article/details/gloasngls.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.zdbjq.cn/Article/details/gvhhmnlej.sHtML

[Q79] 字符串拼接
来源：http://read.share.hesvh.cn/Article/details/glvisekqx.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.hesvh.cn/Article/details/gtrqqxduk.sHtML

[Q80] 字符串截取
来源：http://www.m.share.fehbvm.com/Article/details/gpvzprwvp.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.hesvh.cn/Article/details/gdxruryby.sHtML

[Q81] 字符串替换
来源：http://www.share.hesvh.cn/Article/details/gxccdptjt.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.zdbjq.cn/Article/details/gbdagzyqm.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fehbvm.com/Article/details/gnntmgtiv.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gpibbxzum.sHtML

[Q83] 大小写转换
来源：http://www.m.share.zdbjq.cn/Article/details/gohfjwbit.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gljstikhy.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fehbvm.com/Article/details/gvohfaxan.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gsswynyvq.sHtML

[Q85] 数值取整
来源：http://www.m.share.fehbvm.com/Article/details/gagtosqcj.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.fehbvm.com/Article/details/gevkwaozx.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fehbvm.com/Article/details/gzinuxscu.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fehbvm.com/Article/details/gifuxcwhr.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.hesvh.cn/Article/details/gwnnrdsop.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.zdbjq.cn/Article/details/gpnayelrr.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.hesvh.cn/Article/details/gnyidebay.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.hesvh.cn/Article/details/gqurxgnzh.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gjcikggul.sHtML

[Q89] 判断表是否存在
来源：http://www.share.fehbvm.com/Article/details/gxmmuhhfi.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.zdbjq.cn/Article/details/gahgrikrw.sHtML

[Q90] 生成序号列
来源：http://www.share.hesvh.cn/Article/details/gbngiseun.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.hesvh.cn/Article/details/gnoyrjoxt.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/guejzxgwn.sHtML

R. Bash 专题
来源：http://baike.zdbjq.cn/Article/details/gyxpqkysv.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gfpgpbnvo.sHtML

[R01] shebang 与严格模式
来源：http://baike.hesvh.cn/Article/details/gvkktncpl.sHtML

#!/usr/bin/env bash
来源：http://www.blog.zdbjq.cn/Article/details/gutnpkikm.sHtML

set -euo pipefail
来源：http://3g.hesvh.cn/Article/details/gkqjqyrqk.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fehbvm.com/Article/details/gvjgsvvdx.sHtML

name="Tom"; echo "$name"
来源：http://3g.hesvh.cn/Article/details/gqldpzhmc.sHtML

[R03] 只读变量
来源：http://blog.hesvh.cn/Article/details/gvjuxnkrr.sHtML

readonly PI=3.14
来源：http://blog.zdbjq.cn/Article/details/gujvdgldv.sHtML

[R04] 位置参数
来源：http://www.m.share.hesvh.cn/Article/details/geuknspqq.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fehbvm.com/Article/details/gpremcuvi.sHtML

[R05] 参数默认值
来源：http://read.share.zdbjq.cn/Article/details/gfmiyanef.sHtML

name="${1:-default}"
来源：http://blog.hesvh.cn/Article/details/gzuyksfac.sHtML

[R06] 判断命令是否存在
来源：http://baike.fehbvm.com/Article/details/gfxcmxspq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fehbvm.com/Article/details/gjfgwdmnv.sHtML

[R07] if 判断文件
来源：http://www.blog.hesvh.cn/Article/details/gpuydpopq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.hesvh.cn/Article/details/gjmuwbadz.sHtML

[R08] 数值比较
来源：http://blog.hesvh.cn/Article/details/gtgloulbu.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.zdbjq.cn/Article/details/ghzurksfg.sHtML

[R09] 字符串比较
来源：http://wap.hesvh.cn/Article/details/gqlmrmqum.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.zdbjq.cn/Article/details/geihwkiyw.sHtML

[R10] 正则匹配
来源：http://www.m.share.hesvh.cn/Article/details/gycrycgyy.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gcqxygjzp.sHtML

[R11] case 多分支
来源：http://m.share.fehbvm.com/Article/details/gltoizvqk.sHtML

case "$1" in
来源：http://mobile.zdbjq.cn/Article/details/gwxvgobog.sHtML

start) echo "启动" ;;
来源：http://www.share.zdbjq.cn/Article/details/gftnglgws.sHtML

stop)  echo "停止" ;;
来源：http://3g.hesvh.cn/Article/details/gbmfcnabz.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.hesvh.cn/Article/details/gwtdwuiaf.sHtML

esac
来源：http://m.share.fehbvm.com/Article/details/gccwbydyu.sHtML

[R12] for 遍历文件
来源：http://www.m.share.hesvh.cn/Article/details/gqzasfsmj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.hesvh.cn/Article/details/ghvwlgjjb.sHtML

[R13] for 计数循环
来源：http://3g.zdbjq.cn/Article/details/gpujbozwu.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.zdbjq.cn/Article/details/gvhtfhmbr.sHtML

[R14] C 风格 for
来源：http://3g.zdbjq.cn/Article/details/gtrwxonbh.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/gtqwbyifo.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gdviedjbm.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fehbvm.com/Article/details/ggpxnzipp.sHtML

[R16] until 等待条件
来源：http://3g.hesvh.cn/Article/details/gelhkbucu.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fehbvm.com/Article/details/goephflsr.sHtML

[R17] 数组定义与取值
来源：http://3g.fehbvm.com/Article/details/gqolzrceq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fehbvm.com/Article/details/gsezbxnsw.sHtML

[R18] 遍历数组
来源：http://3g.zdbjq.cn/Article/details/ghemnkplr.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.zdbjq.cn/Article/details/ggbkaefnr.sHtML

[R19] 数组长度
来源：http://m.share.hesvh.cn/Article/details/gxuohwgbl.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fehbvm.com/Article/details/gsyqjgcgg.sHtML

[R20] 关联数组（字典）
来源：http://m.share.zdbjq.cn/Article/details/glvbvwnit.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fehbvm.com/Article/details/gjxsuvagx.sHtML

[R21] 字符串长度
来源：http://www.share.zdbjq.cn/Article/details/gzbnkrpik.sHtML

echo "${#s}"
来源：http://read.share.fehbvm.com/Article/details/gylbpbjef.sHtML

[R22] 截取子串
来源：http://mobile.zdbjq.cn/Article/details/geoaxjwbr.sHtML

echo "${s:0:5}"
来源：http://blog.fehbvm.com/Article/details/gdzzptfqj.sHtML

[R23] 字符串替换
来源：http://3g.zdbjq.cn/Article/details/gldhrcmxt.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fehbvm.com/Article/details/ggjldfmhv.sHtML

[R24] 大小写转换
来源：http://www.share.fehbvm.com/Article/details/gqumlgsgj.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.hesvh.cn/Article/details/gbpkhtvrk.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.zdbjq.cn/Article/details/gmcysyvua.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.hesvh.cn/Article/details/gfftfffuq.sHtML

[R26] 命令替换
来源：http://www.blog.hesvh.cn/Article/details/gxipfbprr.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fehbvm.com/Article/details/gtxbrljid.sHtML

[R27] 算术展开
来源：http://baike.hesvh.cn/Article/details/gwqgnyvzz.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.zdbjq.cn/Article/details/gthdoswal.sHtML

[R28] 浮点运算
来源：http://www.share.zdbjq.cn/Article/details/gljbvqtox.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.zdbjq.cn/Article/details/gizpfttjj.sHtML

[R29] 定义函数
来源：http://www.m.share.hesvh.cn/Article/details/gzfqiqidt.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fehbvm.com/Article/details/gmvpmowzy.sHtML

[R30] 函数返回状态码
来源：http://www.blog.zdbjq.cn/Article/details/gqoblgsew.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.hesvh.cn/Article/details/gwwhoiuzo.sHtML

[R31] 局部变量
来源：http://www.blog.zdbjq.cn/Article/details/gcazaorvb.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.fehbvm.com/Article/details/gzohfenqh.sHtML

[R32] 参数个数校验
来源：http://wap.zdbjq.cn/Article/details/gqgsrkudu.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.hesvh.cn/Article/details/ghtnocyqc.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.hesvh.cn/Article/details/gzefojxrk.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.zdbjq.cn/Article/details/gfzzveoax.sHtML

[R34] 退出时清理
来源：http://www.blog.fehbvm.com/Article/details/gkdzihpqv.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fehbvm.com/Article/details/gcbbdhlen.sHtML

[R35] 后台执行并等待
来源：http://wap.fehbvm.com/Article/details/gfiarwuem.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fehbvm.com/Article/details/groxyljsz.sHtML

[R36] 并发执行多个任务
来源：http://www.share.zdbjq.cn/Article/details/gzqmplmlb.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fehbvm.com/Article/details/gzwaaaqpe.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fehbvm.com/Article/details/gpvxoklfd.sHtML

files=$(ls -1)
来源：http://www.m.share.hesvh.cn/Article/details/gbmfiljei.sHtML

[R38] 管道串联
来源：http://www.blog.hesvh.cn/Article/details/gbakqwrtv.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fehbvm.com/Article/details/gopuuynvk.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.zdbjq.cn/Article/details/gznqhgloj.sHtML

cmd > out.log 2>&1
来源：http://m.share.fehbvm.com/Article/details/gzvxmblid.sHtML

[R40] 追加写日志
来源：http://mobile.hesvh.cn/Article/details/gdrdeqktv.sHtML

echo "log" >> out.log
来源：http://www.m.share.zdbjq.cn/Article/details/gdcogzgep.sHtML

[R41] 丢弃输出
来源：http://www.share.hesvh.cn/Article/details/gjtaexabu.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.zdbjq.cn/Article/details/gxvkgjpkf.sHtML

[R42] 输入重定向
来源：http://www.share.zdbjq.cn/Article/details/ghbmowlos.sHtML

wc -l < a.txt
来源：http://www.blog.fehbvm.com/Article/details/gspqgbcsy.sHtML

[R43] 按名字查找文件
来源：http://mobile.zdbjq.cn/Article/details/gqupnrfgp.sHtML

find . -name "*.log" -type f
来源：http://blog.fehbvm.com/Article/details/gqdaawndr.sHtML

[R44] 按修改时间查找
来源：http://wap.zdbjq.cn/Article/details/gpyurffmo.sHtML

find . -mtime -7 -type f
来源：http://www.blog.hesvh.cn/Article/details/ghofskseg.sHtML

[R45] 批量删除
来源：http://www.blog.hesvh.cn/Article/details/ghkboimtr.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.zdbjq.cn/Article/details/ggnprhgul.sHtML

[R46] 递归替换文件内容
来源：http://m.share.hesvh.cn/Article/details/gcufleubg.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.zdbjq.cn/Article/details/gfsybzipi.sHtML

[R47] sed 单行替换
来源：http://wap.hesvh.cn/Article/details/gjpgfxdja.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.zdbjq.cn/Article/details/gnrauwdqj.sHtML

[R48] awk 取指定列
来源：http://m.share.hesvh.cn/Article/details/gimqdbuig.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gfffdwvzi.sHtML

[R49] awk 带条件
来源：http://www.blog.zdbjq.cn/Article/details/gcgkjyfes.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.hesvh.cn/Article/details/gjhqkuisk.sHtML

[R50] awk 求和
来源：http://wap.fehbvm.com/Article/details/gwuuznhfz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gqywtssdv.sHtML

[R51] 排序去重取前几
来源：http://wap.hesvh.cn/Article/details/gjuanjniq.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fehbvm.com/Article/details/gbwufjzjx.sHtML

[R52] 统计行数
来源：http://m.share.hesvh.cn/Article/details/ggqjksvow.sHtML

wc -l a.txt
来源：http://www.blog.fehbvm.com/Article/details/gfwdhquom.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.hesvh.cn/Article/details/gylmoskfw.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.zdbjq.cn/Article/details/goqwwowot.sHtML

[R54] 比较两个文件
来源：http://www.share.zdbjq.cn/Article/details/gzthjlxfa.sHtML

diff a.txt b.txt
来源：http://m.share.fehbvm.com/Article/details/gnmbijnht.sHtML

[R55] 压缩与解压
来源：http://m.share.zdbjq.cn/Article/details/gslxbvhlg.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.hesvh.cn/Article/details/gywxpizay.sHtML

[R56] 远程拷贝
来源：http://read.share.hesvh.cn/Article/details/gpmwivrsi.sHtML

scp file user@host:/path/
来源：http://blog.hesvh.cn/Article/details/gjtxwfktf.sHtML

[R57] 远程执行命令
来源：http://3g.fehbvm.com/Article/details/gbmnmouib.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fehbvm.com/Article/details/gzecpxybv.sHtML

[R58] 下载文件
来源：http://www.m.share.zdbjq.cn/Article/details/glfznxprt.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.zdbjq.cn/Article/details/gsfhweszj.sHtML

[R59] 发 POST JSON
来源：http://wap.zdbjq.cn/Article/details/gtmyneclw.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.zdbjq.cn/Article/details/gqtjvgjps.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fehbvm.com/Article/details/ghxqrstlu.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fehbvm.com/Article/details/gvtzxkzoa.sHtML

[R61] 磁盘占用
来源：http://read.share.hesvh.cn/Article/details/gdcbyzohz.sHtML

df -h;  du -sh *
来源：http://wap.hesvh.cn/Article/details/ghdecfwpe.sHtML

[R62] 找最占空间的文件
来源：http://wap.zdbjq.cn/Article/details/gjziljdqs.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.hesvh.cn/Article/details/gtnposnhs.sHtML

[R63] 内存与进程
来源：http://baike.zdbjq.cn/Article/details/gyfhpgtxw.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.hesvh.cn/Article/details/gzkprouqp.sHtML

[R64] 结束进程
来源：http://baike.fehbvm.com/Article/details/gpypjnxev.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.hesvh.cn/Article/details/gmlgcwuuc.sHtML

[R65] 查看端口占用
来源：http://mobile.fehbvm.com/Article/details/grocmzabk.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fehbvm.com/Article/details/gkwhpiqyx.sHtML

[R66] 定时任务
来源：http://m.share.zdbjq.cn/Article/details/gmkyojngl.sHtML

crontab -e;  crontab -l
来源：http://wap.zdbjq.cn/Article/details/gkxmfxynu.sHtML

[R67] 生成随机十六进制串
来源：http://blog.zdbjq.cn/Article/details/gevyixapy.sHtML

openssl rand -hex 16
来源：http://read.share.zdbjq.cn/Article/details/gcrepdlok.sHtML

[R68] 计算文件校验值
来源：http://wap.zdbjq.cn/Article/details/gpzwygcoo.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.zdbjq.cn/Article/details/gqugvvoqh.sHtML

[R69] 生成随机密码
来源：http://www.share.zdbjq.cn/Article/details/gdsrokctj.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fehbvm.com/Article/details/golmtgdzi.sHtML

[R70] 时间戳与互转
来源：http://blog.fehbvm.com/Article/details/gxpiehvsr.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.zdbjq.cn/Article/details/gkwpdyros.sHtML

[R71] 日期格式化
来源：http://blog.hesvh.cn/Article/details/gbmzoqmzr.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fehbvm.com/Article/details/gbybyxxvh.sHtML

[R72] 等待端口就绪
来源：http://www.share.hesvh.cn/Article/details/gljympfrm.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/gvnelsvkt.sHtML

[R73] 分割大日志
来源：http://baike.fehbvm.com/Article/details/gdcfkeudd.sHtML

split -l 1000 big.log part_
来源：http://mobile.hesvh.cn/Article/details/ghlossfwh.sHtML

[R74] 批量重命名
来源：http://www.blog.zdbjq.cn/Article/details/grrylxzdm.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.hesvh.cn/Article/details/givvplabb.sHtML

[R75] 导出环境变量
来源：http://baike.fehbvm.com/Article/details/guvpbqmbk.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.hesvh.cn/Article/details/ggwrgddql.sHtML

[R76] 使用临时文件
来源：http://baike.hesvh.cn/Article/details/ghfbwbrsg.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.zdbjq.cn/Article/details/gkhdpmkyh.sHtML

[R77] 读取用户输入
来源：http://m.share.hesvh.cn/Article/details/geuensdmf.sHtML


<!-- 参考信息 -->