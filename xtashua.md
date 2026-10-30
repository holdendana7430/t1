代发 wailian999

[Q33] 多列分组
来源：http://m.share.fanxiaobao.xyz/Article/details/ggqboxhwi.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.fanxiaobao.xyz/Article/details/gzaztimat.sHtML

[Q34] 每组取第一条
来源：http://read.share.fanxiaobao.xyz/Article/details/gqozcqbnd.sHtML

SELECT * FROM (
来源：http://blog.fanxiaobao.xyz/Article/details/gujllxmna.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.fanxiaobao.xyz/Article/details/gpcwoflcv.sHtML

) t WHERE rn = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gciixuokv.sHtML

[Q35] 内连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gszcobjpe.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmyleyogx.sHtML

[Q36] 左连接
来源：http://read.share.fanxiaobao.xyz/Article/details/gwjlbfybm.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkorwooim.sHtML

[Q37] 右连接
来源：http://blog.fanxiaobao.xyz/Article/details/gzgqrcbag.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.fanxiaobao.xyz/Article/details/gvpgygljc.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.fanxiaobao.xyz/Article/details/gpznfjjvn.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqwcnbwai.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfkqzfakz.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.fanxiaobao.xyz/Article/details/gtyslfmwi.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.fanxiaobao.xyz/Article/details/getldmpgu.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzsxtqgkw.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.fanxiaobao.xyz/Article/details/gbnribatl.sHtML

[Q41] 多表连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gtsqzpxvh.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.fanxiaobao.xyz/Article/details/gegjmyoeg.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.fanxiaobao.xyz/Article/details/gkoycluwg.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.fanxiaobao.xyz/Article/details/ggcmnqyss.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gmoktixtl.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdshshlcw.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwmiidnfn.sHtML

[Q43] 标量子查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnlumwktp.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvagtvkxz.sHtML

[Q44] IN 子查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/glippcjdg.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.fanxiaobao.xyz/Article/details/gcgimfqsv.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gunsmbjeu.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fanxiaobao.xyz/Article/details/gjtdkkrrk.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gwzixykgh.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fanxiaobao.xyz/Article/details/guxmngzkl.sHtML

[Q47] 与平均值比较
来源：http://blog.fanxiaobao.xyz/Article/details/gnwahhddr.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.fanxiaobao.xyz/Article/details/godmfkecm.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmcefjild.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.fanxiaobao.xyz/Article/details/glcjtdueh.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtujwqkft.sHtML

[Q49] 更新单行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvsbclbah.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gsvnaqzyj.sHtML

[Q50] 批量更新
来源：http://read.share.fanxiaobao.xyz/Article/details/gbjndbyub.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fanxiaobao.xyz/Article/details/gxgtfrygb.sHtML

[Q51] 用子查询更新
来源：http://m.share.fanxiaobao.xyz/Article/details/gbxhprxnb.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gslurbmjm.sHtML

[Q52] 删除指定行
来源：http://m.share.fanxiaobao.xyz/Article/details/gtnefbjvr.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gsuqldlgm.sHtML

[Q53] 按条件删除
来源：http://blog.fanxiaobao.xyz/Article/details/gmnbeytyj.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghssjgryl.sHtML

[Q54] 清空表
来源：http://wap.fanxiaobao.xyz/Article/details/gunkwxhln.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkspblmkj.sHtML

[Q55] 排名（并列占位）
来源：http://baike.fanxiaobao.xyz/Article/details/gvbfxmimn.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gydfqxszh.sHtML

[Q56] 密集排名（并列不占位）
来源：http://blog.fanxiaobao.xyz/Article/details/gyemjxrqu.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.fanxiaobao.xyz/Article/details/gypcedwdh.sHtML

[Q57] 行号
来源：http://read.share.fanxiaobao.xyz/Article/details/gophlrgmn.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/grmyrkxyr.sHtML

[Q58] 累计求和
来源：http://wap.fanxiaobao.xyz/Article/details/ggsvnwhfg.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gvyqsvlpx.sHtML

[Q59] 分组内累计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyeipfbfi.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gksrzjfgr.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.fanxiaobao.xyz/Article/details/gykajxkjf.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.fanxiaobao.xyz/Article/details/ggutzyjbv.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gfxelqryh.sHtML

[Q61] 移动平均
来源：http://www.share.fanxiaobao.xyz/Article/details/gpqbtmglc.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gptkduetl.sHtML

[Q62] 分组占比
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbaaawneo.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.fanxiaobao.xyz/Article/details/gboxrrgkz.sHtML

[Q63] 开启事务
来源：http://wap.fanxiaobao.xyz/Article/details/gyiegnvis.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkxwcwkrz.sHtML

[Q64] 提交事务
来源：http://3g.fanxiaobao.xyz/Article/details/gmquxezfz.sHtML

COMMIT;
来源：http://www.blog.fanxiaobao.xyz/Article/details/goztglxnq.sHtML

[Q65] 回滚事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gpttvwacr.sHtML

ROLLBACK;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghsnrcbbz.sHtML

[Q66] 行锁查询
来源：http://3g.fanxiaobao.xyz/Article/details/gfrgqiakx.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.fanxiaobao.xyz/Article/details/gnjbfivyx.sHtML

[Q67] 设置隔离级别
来源：http://read.share.fanxiaobao.xyz/Article/details/gvzauvxcb.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gszsmjjsz.sHtML

[Q68] 保存点
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbyxhtyyg.sHtML

SAVEPOINT sp1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjbdhqyxx.sHtML

ROLLBACK TO sp1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gepeqsfpa.sHtML

[Q69] 查看执行计划
来源：http://www.share.fanxiaobao.xyz/Article/details/gvnbrmnge.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.fanxiaobao.xyz/Article/details/gdxrdqbib.sHtML

[Q70] 更新统计信息
来源：http://mobile.fanxiaobao.xyz/Article/details/gfpgpqfzl.sHtML

ANALYZE TABLE users;
来源：http://3g.fanxiaobao.xyz/Article/details/ggijmxtjr.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmtwenmqw.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdozwbwxt.sHtML

[Q72] 查看索引
来源：http://www.share.fanxiaobao.xyz/Article/details/gxnnpjsev.sHtML

SHOW INDEX FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwhqjkqrl.sHtML

[Q73] 查看表状态
来源：http://blog.fanxiaobao.xyz/Article/details/gzocmqpxo.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.fanxiaobao.xyz/Article/details/ghgcgworp.sHtML

[Q74] 强制使用索引
来源：http://3g.fanxiaobao.xyz/Article/details/gkxhktvwz.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fanxiaobao.xyz/Article/details/ghkozeirs.sHtML

[Q75] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/glcynbumy.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gzyjlzgwi.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fanxiaobao.xyz/Article/details/gcijewewt.sHtML

[Q76] 按天统计
来源：http://read.share.fanxiaobao.xyz/Article/details/grelumxam.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fanxiaobao.xyz/Article/details/gntnwzzoc.sHtML

[Q77] 时间加减
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmpphojfq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.fanxiaobao.xyz/Article/details/gewzqwlol.sHtML

[Q78] 当前时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxzrtqsyy.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghjkglhsf.sHtML

[Q79] 字符串拼接
来源：http://3g.fanxiaobao.xyz/Article/details/gaplibomz.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.fanxiaobao.xyz/Article/details/grrfbdwtt.sHtML

[Q80] 字符串截取
来源：http://mobile.fanxiaobao.xyz/Article/details/gahrqyviu.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gnhdaywrf.sHtML

[Q81] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gwyxigwde.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gocyezwxj.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gemvrwfib.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gzfbkuzcy.sHtML

[Q83] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqdkgkqii.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gxymjopfi.sHtML

[Q84] 去除首尾空格
来源：http://blog.fanxiaobao.xyz/Article/details/gfpolqczr.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpjbchxlu.sHtML

[Q85] 数值取整
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjrzfyuin.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.fanxiaobao.xyz/Article/details/gvldmdiry.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnvfhrfbz.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://mobile.fanxiaobao.xyz/Article/details/gvbalxxrm.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fanxiaobao.xyz/Article/details/gmohtuxts.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guwhlzeci.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fanxiaobao.xyz/Article/details/gdxxzeoap.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.fanxiaobao.xyz/Article/details/guqoneruh.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnwhionqm.sHtML

[Q89] 判断表是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gwfzujrhj.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fanxiaobao.xyz/Article/details/gnyufohfx.sHtML

[Q90] 生成序号列
来源：http://m.share.fanxiaobao.xyz/Article/details/ggtmrkiaj.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.fanxiaobao.xyz/Article/details/gibqcvlfi.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gcbrfzdke.sHtML

R. Bash 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/goyhwwptz.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdvqqxoqw.sHtML

[R01] shebang 与严格模式
来源：http://blog.fanxiaobao.xyz/Article/details/gwrzsaztn.sHtML

#!/usr/bin/env bash
来源：http://3g.fanxiaobao.xyz/Article/details/gzunbpito.sHtML

set -euo pipefail
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzfhepmmm.sHtML

[R02] 变量赋值与使用
来源：http://baike.fanxiaobao.xyz/Article/details/gstmhuefr.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fanxiaobao.xyz/Article/details/gwjtchoqt.sHtML

[R03] 只读变量
来源：http://m.share.fanxiaobao.xyz/Article/details/grftykmpz.sHtML

readonly PI=3.14
来源：http://read.share.fanxiaobao.xyz/Article/details/gjtvccdjx.sHtML

[R04] 位置参数
来源：http://baike.fanxiaobao.xyz/Article/details/gkzuqicng.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fanxiaobao.xyz/Article/details/gqvedjyxx.sHtML

[R05] 参数默认值
来源：http://wap.fanxiaobao.xyz/Article/details/gybrxobgp.sHtML

name="${1:-default}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gzgjvyykp.sHtML

[R06] 判断命令是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gjgthvsdi.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gbntrumyk.sHtML

[R07] if 判断文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gifwwfbhf.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gjporntpw.sHtML

[R08] 数值比较
来源：http://3g.fanxiaobao.xyz/Article/details/gwbtwuuzq.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gbciyziek.sHtML

[R09] 字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gjoxakube.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glqtudgkp.sHtML

[R10] 正则匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gwnxrasuo.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gcmoouvrr.sHtML

[R11] case 多分支
来源：http://read.share.fanxiaobao.xyz/Article/details/gfjyuabmn.sHtML

case "$1" in
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnxovwxxu.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvucpqgfy.sHtML

stop)  echo "停止" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gtdyfdnrp.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcukesjyp.sHtML

esac
来源：http://read.share.fanxiaobao.xyz/Article/details/grmkodhnl.sHtML

[R12] for 遍历文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gyyrnelit.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/graielrue.sHtML

[R13] for 计数循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmnpmfpgn.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/ggnmbeyxp.sHtML

[R14] C 风格 for
来源：http://mobile.fanxiaobao.xyz/Article/details/gbyxuxtiy.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/ggwfwsdkk.sHtML

[R15] while 逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gtqhyuchv.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gkgriftid.sHtML

[R16] until 等待条件
来源：http://baike.fanxiaobao.xyz/Article/details/gihfgdugn.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdgxtjbmp.sHtML

[R17] 数组定义与取值
来源：http://m.share.fanxiaobao.xyz/Article/details/gvebilcho.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gcqvfwipz.sHtML

[R18] 遍历数组
来源：http://3g.fanxiaobao.xyz/Article/details/gjdryspai.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/grukjgtbx.sHtML

[R19] 数组长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gdrqwtbdi.sHtML

echo "${#arr[@]}"
来源：http://baike.fanxiaobao.xyz/Article/details/ggnayqdyd.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fanxiaobao.xyz/Article/details/ganvyxojz.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gcshoeglx.sHtML

[R21] 字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gfkeqpfkl.sHtML

echo "${#s}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqccszmdv.sHtML

[R22] 截取子串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpgdesgsk.sHtML

echo "${s:0:5}"
来源：http://3g.fanxiaobao.xyz/Article/details/gcabkwory.sHtML

[R23] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/gqdiwngao.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fanxiaobao.xyz/Article/details/gjxlekkgz.sHtML

[R24] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/gwmcuuzfj.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gswaiyzzr.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fanxiaobao.xyz/Article/details/gibvpdkfa.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghjhbizqf.sHtML

[R26] 命令替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gbyszacqg.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.fanxiaobao.xyz/Article/details/gdunffnxf.sHtML

[R27] 算术展开
来源：http://3g.fanxiaobao.xyz/Article/details/gmnulpdft.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fanxiaobao.xyz/Article/details/gsorizsyp.sHtML

[R28] 浮点运算
来源：http://m.share.fanxiaobao.xyz/Article/details/gbifmyknj.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fanxiaobao.xyz/Article/details/godeuvqek.sHtML

[R29] 定义函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtvphcrtb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyajawpbx.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvrqnibtk.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fanxiaobao.xyz/Article/details/grsbsyuej.sHtML

[R31] 局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gugfnflpw.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fanxiaobao.xyz/Article/details/ggwbauzyp.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gipwastmi.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gcdexzwnu.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnputhjvc.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fanxiaobao.xyz/Article/details/ghkyffnlj.sHtML

[R34] 退出时清理
来源：http://3g.fanxiaobao.xyz/Article/details/gcqkcekvu.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/gmfziudsq.sHtML

[R35] 后台执行并等待
来源：http://mobile.fanxiaobao.xyz/Article/details/gnfghnpcm.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkutxqeyi.sHtML

[R36] 并发执行多个任务
来源：http://baike.fanxiaobao.xyz/Article/details/ggmbfkisc.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fanxiaobao.xyz/Article/details/gskhgoinz.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gevkkbfmt.sHtML

files=$(ls -1)
来源：http://3g.fanxiaobao.xyz/Article/details/guixcskwc.sHtML

[R38] 管道串联
来源：http://mobile.fanxiaobao.xyz/Article/details/gdbzqvyyv.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geeqtsgvu.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvbsbozfv.sHtML

cmd > out.log 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gsqowkcwv.sHtML

[R40] 追加写日志
来源：http://3g.fanxiaobao.xyz/Article/details/goqkdpksi.sHtML

echo "log" >> out.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gjpcpupuo.sHtML

[R41] 丢弃输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gqnarijlj.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfrkzzikl.sHtML

[R42] 输入重定向
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzybtmmvs.sHtML

wc -l < a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gedoakjre.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsbiopefn.sHtML

find . -name "*.log" -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/ghiesuthz.sHtML

[R44] 按修改时间查找
来源：http://m.share.fanxiaobao.xyz/Article/details/glngqeodz.sHtML

find . -mtime -7 -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gshntulmg.sHtML

[R45] 批量删除
来源：http://wap.fanxiaobao.xyz/Article/details/gpyftjaoz.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fanxiaobao.xyz/Article/details/gbdmvcgkg.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsdvfhbgz.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fanxiaobao.xyz/Article/details/guovsnxqa.sHtML

[R47] sed 单行替换
来源：http://3g.fanxiaobao.xyz/Article/details/gmwzghlpv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkvhazmfy.sHtML

[R48] awk 取指定列
来源：http://blog.fanxiaobao.xyz/Article/details/gztclvnlv.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmkigktvu.sHtML

[R49] awk 带条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gcywdhzyd.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fanxiaobao.xyz/Article/details/gjuxrwswx.sHtML

[R50] awk 求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gqgqtfvom.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grzknfxcn.sHtML

[R51] 排序去重取前几
来源：http://m.share.fanxiaobao.xyz/Article/details/gqdibpgej.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fanxiaobao.xyz/Article/details/gtxikopxm.sHtML

[R52] 统计行数
来源：http://read.share.fanxiaobao.xyz/Article/details/gmmihavdi.sHtML

wc -l a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/grasecgeb.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpzazqsoe.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gvfqutptm.sHtML

[R54] 比较两个文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gnskqbtxn.sHtML

diff a.txt b.txt
来源：http://blog.fanxiaobao.xyz/Article/details/ggotlrler.sHtML

[R55] 压缩与解压
来源：http://m.share.fanxiaobao.xyz/Article/details/gctouoahl.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxjaqoxzy.sHtML

[R56] 远程拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gtlrmugzd.sHtML

scp file user@host:/path/
来源：http://3g.fanxiaobao.xyz/Article/details/ggtnrqvrh.sHtML

[R57] 远程执行命令
来源：http://baike.fanxiaobao.xyz/Article/details/ggiabwtrj.sHtML

ssh user@host 'uptime'
来源：http://baike.fanxiaobao.xyz/Article/details/gorpmktfv.sHtML

[R58] 下载文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gtkenvjgp.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fanxiaobao.xyz/Article/details/glpogvtct.sHtML

[R59] 发 POST JSON
来源：http://wap.fanxiaobao.xyz/Article/details/gnofdmchv.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkqeqybgr.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gexuzhimq.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gmlccoumc.sHtML

[R61] 磁盘占用
来源：http://blog.fanxiaobao.xyz/Article/details/gyfgqjhag.sHtML

df -h;  du -sh *
来源：http://m.share.fanxiaobao.xyz/Article/details/gtdhdqhal.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gpqodevrx.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fanxiaobao.xyz/Article/details/gtlduubqj.sHtML

[R63] 内存与进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzovwqefq.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fanxiaobao.xyz/Article/details/gdainxjfk.sHtML

[R64] 结束进程
来源：http://read.share.fanxiaobao.xyz/Article/details/gvjjjgdry.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fanxiaobao.xyz/Article/details/gplkxyatt.sHtML

[R65] 查看端口占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gpwiympuw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxhstfkxn.sHtML

[R66] 定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/grvjboiyb.sHtML

crontab -e;  crontab -l
来源：http://wap.fanxiaobao.xyz/Article/details/gfzqrwrgw.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwjryhvur.sHtML

openssl rand -hex 16
来源：http://m.share.fanxiaobao.xyz/Article/details/glandujij.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkdrztale.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gthxidiwi.sHtML

[R69] 生成随机密码
来源：http://www.share.fanxiaobao.xyz/Article/details/gthmohiso.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fanxiaobao.xyz/Article/details/gejfdswwn.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvczzevdn.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjsvfjuwh.sHtML

[R71] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/glwcnpypt.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fanxiaobao.xyz/Article/details/gbeymmvbd.sHtML

[R72] 等待端口就绪
来源：http://m.share.fanxiaobao.xyz/Article/details/gbhrlvrce.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gauigesal.sHtML

[R73] 分割大日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gstqqeoru.sHtML

split -l 1000 big.log part_
来源：http://mobile.fanxiaobao.xyz/Article/details/gnvkxbjpj.sHtML

[R74] 批量重命名
来源：http://3g.fanxiaobao.xyz/Article/details/gtpvcyvog.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/grmnnjbru.sHtML

[R75] 导出环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/gafsjwrco.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fanxiaobao.xyz/Article/details/gbqicedtr.sHtML

[R76] 使用临时文件
来源：http://www.share.fanxiaobao.xyz/Article/details/giswcnean.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fanxiaobao.xyz/Article/details/gghncafbc.sHtML

[R77] 读取用户输入
来源：http://www.share.fanxiaobao.xyz/Article/details/gktlkhhtg.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyxpzsupo.sHtML

[R78] 交互式菜单
来源：http://read.share.fanxiaobao.xyz/Article/details/gzzzteycj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbeofcbud.sHtML

[R79] 解析命令行选项
来源：http://wap.fanxiaobao.xyz/Article/details/gvtuieora.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fanxiaobao.xyz/Article/details/gaofaghvp.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fanxiaobao.xyz/Article/details/gqaydmccf.sHtML

time ./run.sh
来源：http://blog.fanxiaobao.xyz/Article/details/gkkqlkqdw.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/ggfzuhprf.sHtML

S. C / C++ 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwikrrtlr.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gyhzdnmin.sHtML

[S01] C：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gaehwxutm.sHtML

#include <stdio.h>
来源：http://m.share.fanxiaobao.xyz/Article/details/gdmrxsujm.sHtML


<!-- 参考信息 -->