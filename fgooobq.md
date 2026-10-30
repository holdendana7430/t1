代发 wailian999

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.hesvh.cn/Article/details/gpqdjbxrj.sHtML

[Q26] 计数
来源：http://blog.fehbvm.com/Article/details/ghcuqtwjq.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gztitpkqb.sHtML

[Q27] 条件计数
来源：http://read.share.fehbvm.com/Article/details/gqujagyxu.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.fehbvm.com/Article/details/ggimbjhyy.sHtML

[Q28] 求和与平均
来源：http://m.share.fehbvm.com/Article/details/gdeltmrcf.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.fehbvm.com/Article/details/gfjldggyx.sHtML

[Q29] 最大最小值
来源：http://mobile.zdbjq.cn/Article/details/gonylphhi.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gpyihjwwe.sHtML

[Q30] 分组统计
来源：http://read.share.zdbjq.cn/Article/details/gvhfjrqsh.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gzsgrdisg.sHtML

[Q31] 分组后过滤
来源：http://read.share.zdbjq.cn/Article/details/gxgjtsqkh.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.fehbvm.com/Article/details/gqxopjmdo.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/gqualmzai.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/gjfmqqckn.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.zdbjq.cn/Article/details/gnpqawvhf.sHtML

[Q33] 多列分组
来源：http://read.share.hesvh.cn/Article/details/gnlbwyshk.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.fehbvm.com/Article/details/gygbxlqti.sHtML

[Q34] 每组取第一条
来源：http://blog.fehbvm.com/Article/details/gdxxzdpzc.sHtML

SELECT * FROM (
来源：http://blog.zdbjq.cn/Article/details/ggtdcxzxp.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.fehbvm.com/Article/details/gtnzgmjxa.sHtML

) t WHERE rn = 1;
来源：http://blog.zdbjq.cn/Article/details/gasktbzdw.sHtML

[Q35] 内连接
来源：http://m.share.fehbvm.com/Article/details/giareuhiv.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.hesvh.cn/Article/details/gcvrdbdqe.sHtML

[Q36] 左连接
来源：http://www.blog.hesvh.cn/Article/details/ghgulpbpf.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.zdbjq.cn/Article/details/gsfbchgis.sHtML

[Q37] 右连接
来源：http://read.share.zdbjq.cn/Article/details/gpajwniqw.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.hesvh.cn/Article/details/gbdhkvqqg.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.zdbjq.cn/Article/details/gpijiudxc.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.hesvh.cn/Article/details/guztndapy.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.fehbvm.com/Article/details/gzyeasdyl.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.fehbvm.com/Article/details/gzllddlrp.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.zdbjq.cn/Article/details/gnmdtqxat.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.zdbjq.cn/Article/details/gtkypobuc.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.zdbjq.cn/Article/details/guywlustw.sHtML

[Q41] 多表连接
来源：http://www.blog.fehbvm.com/Article/details/gsojuxgyw.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.fehbvm.com/Article/details/gkjvliynb.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.fehbvm.com/Article/details/gabduwnlr.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gggoahufw.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.fehbvm.com/Article/details/gufzwkean.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.hesvh.cn/Article/details/gasvxvgrj.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.zdbjq.cn/Article/details/gamobtuze.sHtML

[Q43] 标量子查询
来源：http://wap.hesvh.cn/Article/details/gcxurirfe.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.hesvh.cn/Article/details/gyvjmvnpk.sHtML

[Q44] IN 子查询
来源：http://blog.zdbjq.cn/Article/details/gaiahwfqc.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.zdbjq.cn/Article/details/gyliyahne.sHtML

[Q45] EXISTS 判断存在
来源：http://wap.hesvh.cn/Article/details/gordrhjwh.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.zdbjq.cn/Article/details/gwewyjxma.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.hesvh.cn/Article/details/gulvwpbkx.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.zdbjq.cn/Article/details/gzevhxhbd.sHtML

[Q47] 与平均值比较
来源：http://m.share.hesvh.cn/Article/details/gxulizyeq.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.hesvh.cn/Article/details/gloyokhjp.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.fehbvm.com/Article/details/gnpkdxmdm.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fehbvm.com/Article/details/gqefcbsak.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.zdbjq.cn/Article/details/gshlbfbne.sHtML

[Q49] 更新单行
来源：http://www.blog.fehbvm.com/Article/details/geyohipsy.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.hesvh.cn/Article/details/ghtqhakef.sHtML

[Q50] 批量更新
来源：http://www.blog.fehbvm.com/Article/details/gqjbguayx.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.fehbvm.com/Article/details/gsakpsybd.sHtML

[Q51] 用子查询更新
来源：http://blog.fehbvm.com/Article/details/gbdxckipg.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.fehbvm.com/Article/details/gxhkswblh.sHtML

[Q52] 删除指定行
来源：http://www.blog.hesvh.cn/Article/details/gmbbbrhmk.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.hesvh.cn/Article/details/gvtohffcn.sHtML

[Q53] 按条件删除
来源：http://mobile.zdbjq.cn/Article/details/gjyxgizon.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.hesvh.cn/Article/details/gfxwvoxhm.sHtML

[Q54] 清空表
来源：http://m.share.hesvh.cn/Article/details/gxntzmbjb.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.hesvh.cn/Article/details/gjlisyhwi.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.zdbjq.cn/Article/details/gokjvczug.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.zdbjq.cn/Article/details/gtqfkydzm.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.hesvh.cn/Article/details/gwjuflcck.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.hesvh.cn/Article/details/gatafwdik.sHtML

[Q57] 行号
来源：http://blog.hesvh.cn/Article/details/grlxmxfbo.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gmjkerfpb.sHtML

[Q58] 累计求和
来源：http://read.share.hesvh.cn/Article/details/gxwfylxux.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.hesvh.cn/Article/details/gyupzlybw.sHtML

[Q59] 分组内累计
来源：http://www.m.share.fehbvm.com/Article/details/gjpvvcnis.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.fehbvm.com/Article/details/gmgqosezc.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.hesvh.cn/Article/details/gkphvzlpd.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fehbvm.com/Article/details/grttjnlhg.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gsprycklh.sHtML

[Q61] 移动平均
来源：http://wap.zdbjq.cn/Article/details/gvmapezab.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gfcjgxpls.sHtML

[Q62] 分组占比
来源：http://www.blog.hesvh.cn/Article/details/gzvytdstw.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/gtscrqpyb.sHtML

[Q63] 开启事务
来源：http://www.blog.fehbvm.com/Article/details/gkjwsapif.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.fehbvm.com/Article/details/gaxttgdun.sHtML

[Q64] 提交事务
来源：http://read.share.fehbvm.com/Article/details/gwjqsiilj.sHtML

COMMIT;
来源：http://www.blog.zdbjq.cn/Article/details/gixqydpzv.sHtML

[Q65] 回滚事务
来源：http://www.blog.fehbvm.com/Article/details/gxinbhzhe.sHtML

ROLLBACK;
来源：http://mobile.zdbjq.cn/Article/details/gqaikuypb.sHtML

[Q66] 行锁查询
来源：http://www.m.share.hesvh.cn/Article/details/gvogidvsu.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.hesvh.cn/Article/details/gqehloguo.sHtML

[Q67] 设置隔离级别
来源：http://blog.zdbjq.cn/Article/details/gyhrekuxv.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.hesvh.cn/Article/details/ggbqovdxz.sHtML

[Q68] 保存点
来源：http://3g.hesvh.cn/Article/details/gntomrdyi.sHtML

SAVEPOINT sp1;
来源：http://blog.zdbjq.cn/Article/details/ghbajbhkl.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.fehbvm.com/Article/details/gpyooiysz.sHtML

[Q69] 查看执行计划
来源：http://blog.fehbvm.com/Article/details/gduymlgis.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.fehbvm.com/Article/details/ghavtqsvk.sHtML

[Q70] 更新统计信息
来源：http://wap.hesvh.cn/Article/details/gilrcuddg.sHtML

ANALYZE TABLE users;
来源：http://baike.hesvh.cn/Article/details/gqxacxkba.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fehbvm.com/Article/details/gkagtefpd.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://read.share.zdbjq.cn/Article/details/grxzmtgfy.sHtML

[Q72] 查看索引
来源：http://read.share.fehbvm.com/Article/details/gdddsxyiz.sHtML

SHOW INDEX FROM users;
来源：http://mobile.hesvh.cn/Article/details/grsxovguo.sHtML

[Q73] 查看表状态
来源：http://www.m.share.zdbjq.cn/Article/details/gromahuty.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.hesvh.cn/Article/details/gzlaxcfbu.sHtML

[Q74] 强制使用索引
来源：http://www.share.fehbvm.com/Article/details/gvuoymjih.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.zdbjq.cn/Article/details/gyerlnfpc.sHtML

[Q75] 日期格式化
来源：http://mobile.hesvh.cn/Article/details/giskytngq.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.hesvh.cn/Article/details/gagnzywsh.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.zdbjq.cn/Article/details/gzvpqdbys.sHtML

[Q76] 按天统计
来源：http://www.m.share.zdbjq.cn/Article/details/giueacdjb.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.fehbvm.com/Article/details/grauupsuc.sHtML

[Q77] 时间加减
来源：http://www.m.share.zdbjq.cn/Article/details/gqztsmfgk.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.zdbjq.cn/Article/details/glcwlltze.sHtML

[Q78] 当前时间
来源：http://wap.hesvh.cn/Article/details/gxzxbxfsa.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.hesvh.cn/Article/details/gcpchluyc.sHtML

[Q79] 字符串拼接
来源：http://mobile.hesvh.cn/Article/details/gniialfws.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.zdbjq.cn/Article/details/gtpugexts.sHtML

[Q80] 字符串截取
来源：http://www.share.hesvh.cn/Article/details/gebtdoxyz.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gpzaohdii.sHtML

[Q81] 字符串替换
来源：http://3g.fehbvm.com/Article/details/gteytpssn.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gnjdmrftu.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.hesvh.cn/Article/details/grcxvcilw.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/ghajetbco.sHtML

[Q83] 大小写转换
来源：http://blog.hesvh.cn/Article/details/gxnjwrehw.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/ghkpvagxo.sHtML

[Q84] 去除首尾空格
来源：http://mobile.hesvh.cn/Article/details/gxbiwsetw.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gwedlwjvp.sHtML

[Q85] 数值取整
来源：http://m.share.fehbvm.com/Article/details/gqvmcpvyi.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.hesvh.cn/Article/details/gqjqbbvfv.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.hesvh.cn/Article/details/gcvykgvak.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.hesvh.cn/Article/details/glxurtfbh.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.zdbjq.cn/Article/details/gyfebpehe.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.fehbvm.com/Article/details/gxpsqtezg.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.hesvh.cn/Article/details/gewrztqhm.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.hesvh.cn/Article/details/gnbziytdh.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gznviifvp.sHtML

[Q89] 判断表是否存在
来源：http://blog.fehbvm.com/Article/details/gudebdeyv.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.hesvh.cn/Article/details/gziuqyxvf.sHtML

[Q90] 生成序号列
来源：http://3g.zdbjq.cn/Article/details/gjbmdlwuc.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.hesvh.cn/Article/details/gosdyujbf.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gnyhhfomi.sHtML

R. Bash 专题
来源：http://blog.zdbjq.cn/Article/details/ggkdmsulj.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/grgcabujr.sHtML

[R01] shebang 与严格模式
来源：http://read.share.zdbjq.cn/Article/details/gbeenxmtp.sHtML

#!/usr/bin/env bash
来源：http://wap.zdbjq.cn/Article/details/grkqouqja.sHtML

set -euo pipefail
来源：http://baike.hesvh.cn/Article/details/gycsjzkil.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fehbvm.com/Article/details/gekbxgrya.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fehbvm.com/Article/details/gugendiiy.sHtML

[R03] 只读变量
来源：http://m.share.zdbjq.cn/Article/details/gjfpkuhzq.sHtML

readonly PI=3.14
来源：http://baike.zdbjq.cn/Article/details/gksavjudo.sHtML

[R04] 位置参数
来源：http://www.m.share.fehbvm.com/Article/details/gyepgbsyp.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.zdbjq.cn/Article/details/gwdblfbzd.sHtML

[R05] 参数默认值
来源：http://m.share.fehbvm.com/Article/details/gylroibcw.sHtML

name="${1:-default}"
来源：http://read.share.hesvh.cn/Article/details/gkmnecxfy.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fehbvm.com/Article/details/gdbjxnpfo.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/gckjpgyme.sHtML

[R07] if 判断文件
来源：http://www.blog.hesvh.cn/Article/details/gadxoenzc.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.fehbvm.com/Article/details/grukajhcl.sHtML

[R08] 数值比较
来源：http://mobile.hesvh.cn/Article/details/goerxsjeu.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.fehbvm.com/Article/details/gosmlfufa.sHtML

[R09] 字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/gedqnvpir.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.zdbjq.cn/Article/details/gbdwetqbv.sHtML

[R10] 正则匹配
来源：http://www.share.fehbvm.com/Article/details/gzlxaeifb.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/ggdywvewb.sHtML

[R11] case 多分支
来源：http://baike.zdbjq.cn/Article/details/gidchkqhd.sHtML

case "$1" in
来源：http://www.blog.fehbvm.com/Article/details/gwpapwhtj.sHtML

start) echo "启动" ;;
来源：http://read.share.hesvh.cn/Article/details/gmrxupqcw.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.zdbjq.cn/Article/details/gkcguxijd.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.zdbjq.cn/Article/details/gporsnszy.sHtML

esac
来源：http://www.blog.hesvh.cn/Article/details/gddpnqxem.sHtML

[R12] for 遍历文件
来源：http://3g.fehbvm.com/Article/details/gcjcdgpte.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fehbvm.com/Article/details/gzxbbmgve.sHtML

[R13] for 计数循环
来源：http://blog.fehbvm.com/Article/details/gsfakmzkq.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fehbvm.com/Article/details/gtpxjoaev.sHtML

[R14] C 风格 for
来源：http://read.share.fehbvm.com/Article/details/gdbplpdre.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gjbwbjikj.sHtML

[R15] while 逐行读文件
来源：http://blog.hesvh.cn/Article/details/gwsincokq.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.hesvh.cn/Article/details/gplmddffr.sHtML

[R16] until 等待条件
来源：http://www.share.zdbjq.cn/Article/details/gqtyscond.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.zdbjq.cn/Article/details/gaasveqpp.sHtML

[R17] 数组定义与取值
来源：http://mobile.hesvh.cn/Article/details/gywpetuxs.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fehbvm.com/Article/details/ggiaplleq.sHtML

[R18] 遍历数组
来源：http://www.blog.hesvh.cn/Article/details/gygdlqzga.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.hesvh.cn/Article/details/ggiyvxujg.sHtML

[R19] 数组长度
来源：http://m.share.fehbvm.com/Article/details/gyxidlkxa.sHtML

echo "${#arr[@]}"
来源：http://baike.hesvh.cn/Article/details/gvsdwyngn.sHtML

[R20] 关联数组（字典）
来源：http://read.share.hesvh.cn/Article/details/gbmxvyuqd.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fehbvm.com/Article/details/gfcpzwflt.sHtML

[R21] 字符串长度
来源：http://wap.hesvh.cn/Article/details/gvcfwqyaj.sHtML

echo "${#s}"
来源：http://blog.fehbvm.com/Article/details/guycecwxi.sHtML

[R22] 截取子串
来源：http://m.share.zdbjq.cn/Article/details/gazjdxaxd.sHtML

echo "${s:0:5}"
来源：http://blog.hesvh.cn/Article/details/garlqvgpt.sHtML

[R23] 字符串替换
来源：http://baike.fehbvm.com/Article/details/gmnrbxlxr.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.zdbjq.cn/Article/details/gyqzmbasv.sHtML

[R24] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/geygaelfm.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fehbvm.com/Article/details/gbyrtihsp.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fehbvm.com/Article/details/gmsjbnzez.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fehbvm.com/Article/details/gjdycwqul.sHtML

[R26] 命令替换
来源：http://3g.fehbvm.com/Article/details/galfhbxnx.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.zdbjq.cn/Article/details/glmsaszrh.sHtML

[R27] 算术展开
来源：http://m.share.hesvh.cn/Article/details/gzfmaotac.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.zdbjq.cn/Article/details/gkvtrstwk.sHtML

[R28] 浮点运算
来源：http://www.blog.fehbvm.com/Article/details/gzxukaeyb.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fehbvm.com/Article/details/guhczyklm.sHtML

[R29] 定义函数
来源：http://blog.fehbvm.com/Article/details/gbxmsdrol.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.zdbjq.cn/Article/details/gvhvfinyy.sHtML

[R30] 函数返回状态码
来源：http://3g.hesvh.cn/Article/details/glucfzjrv.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.zdbjq.cn/Article/details/gwvpfrciz.sHtML

[R31] 局部变量
来源：http://baike.fehbvm.com/Article/details/gmloqrkmf.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fehbvm.com/Article/details/gpvceuozq.sHtML

[R32] 参数个数校验
来源：http://www.m.share.hesvh.cn/Article/details/guaimjzbn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fehbvm.com/Article/details/grravqwql.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.hesvh.cn/Article/details/gyyqpuvvk.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fehbvm.com/Article/details/gclwemrwa.sHtML

[R34] 退出时清理
来源：http://m.share.zdbjq.cn/Article/details/gnxjibefd.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/gxzvpmpul.sHtML

[R35] 后台执行并等待
来源：http://www.share.fehbvm.com/Article/details/gataxdkjp.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.hesvh.cn/Article/details/gvbzibfrc.sHtML

[R36] 并发执行多个任务
来源：http://wap.hesvh.cn/Article/details/gkrkgqbec.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.zdbjq.cn/Article/details/gijarjfsw.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fehbvm.com/Article/details/gnyfibzsc.sHtML

files=$(ls -1)
来源：http://read.share.fehbvm.com/Article/details/gmqfvwwaz.sHtML

[R38] 管道串联
来源：http://blog.zdbjq.cn/Article/details/guthbwoos.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fehbvm.com/Article/details/gffesmzfy.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.hesvh.cn/Article/details/gustccbbm.sHtML

cmd > out.log 2>&1
来源：http://wap.zdbjq.cn/Article/details/gfkilhssc.sHtML

[R40] 追加写日志
来源：http://m.share.fehbvm.com/Article/details/giqxxxmkv.sHtML

echo "log" >> out.log
来源：http://3g.zdbjq.cn/Article/details/gqtydzcgw.sHtML

[R41] 丢弃输出
来源：http://baike.hesvh.cn/Article/details/gvfxtjcji.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fehbvm.com/Article/details/gcsqubjzi.sHtML

[R42] 输入重定向
来源：http://mobile.fehbvm.com/Article/details/gnsqffzhp.sHtML

wc -l < a.txt
来源：http://www.blog.hesvh.cn/Article/details/gmdqhsivq.sHtML

[R43] 按名字查找文件
来源：http://www.blog.hesvh.cn/Article/details/gvwzpxybt.sHtML

find . -name "*.log" -type f
来源：http://www.share.fehbvm.com/Article/details/gfkxheczz.sHtML

[R44] 按修改时间查找
来源：http://blog.zdbjq.cn/Article/details/gdouvdwou.sHtML

find . -mtime -7 -type f
来源：http://read.share.hesvh.cn/Article/details/giseqmbfx.sHtML

[R45] 批量删除
来源：http://baike.hesvh.cn/Article/details/gxpzllvkw.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.hesvh.cn/Article/details/gcuriatxo.sHtML

[R46] 递归替换文件内容
来源：http://wap.fehbvm.com/Article/details/giagfgoht.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.hesvh.cn/Article/details/gkfktxkbf.sHtML

[R47] sed 单行替换
来源：http://read.share.fehbvm.com/Article/details/gzedqqtrp.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gduhqvyvk.sHtML

[R48] awk 取指定列
来源：http://blog.zdbjq.cn/Article/details/gpycheibg.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.zdbjq.cn/Article/details/geajrmzqr.sHtML

[R49] awk 带条件
来源：http://read.share.fehbvm.com/Article/details/guspapvxu.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.hesvh.cn/Article/details/gutmaqkuk.sHtML

[R50] awk 求和
来源：http://www.m.share.fehbvm.com/Article/details/gwruuache.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gzrhueaui.sHtML

[R51] 排序去重取前几
来源：http://blog.hesvh.cn/Article/details/gczwjhdzl.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.hesvh.cn/Article/details/gezbfegeg.sHtML

[R52] 统计行数
来源：http://baike.hesvh.cn/Article/details/gtxtcymgv.sHtML

wc -l a.txt
来源：http://mobile.fehbvm.com/Article/details/gtlqnrvdt.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.hesvh.cn/Article/details/gvvnngymj.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.hesvh.cn/Article/details/gdgrlrydd.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fehbvm.com/Article/details/gfckwluhq.sHtML

diff a.txt b.txt
来源：http://baike.zdbjq.cn/Article/details/gecrpfuua.sHtML

[R55] 压缩与解压
来源：http://mobile.fehbvm.com/Article/details/gshswocsu.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.hesvh.cn/Article/details/glvkddirm.sHtML

[R56] 远程拷贝
来源：http://baike.zdbjq.cn/Article/details/gwcmvrktj.sHtML

scp file user@host:/path/
来源：http://read.share.hesvh.cn/Article/details/gatczwuat.sHtML

[R57] 远程执行命令
来源：http://3g.fehbvm.com/Article/details/gbvzlfbme.sHtML

ssh user@host 'uptime'
来源：http://blog.fehbvm.com/Article/details/gvyfpujtw.sHtML

[R58] 下载文件
来源：http://www.share.hesvh.cn/Article/details/gzbmlgbhx.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.hesvh.cn/Article/details/goiyhqhst.sHtML

[R59] 发 POST JSON
来源：http://baike.fehbvm.com/Article/details/gcjjmztjq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.hesvh.cn/Article/details/gtlsnzxfm.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.hesvh.cn/Article/details/ggsjpotib.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fehbvm.com/Article/details/gppskfuer.sHtML

[R61] 磁盘占用
来源：http://blog.zdbjq.cn/Article/details/gsvufkvhr.sHtML

df -h;  du -sh *
来源：http://mobile.hesvh.cn/Article/details/gfswybane.sHtML

[R62] 找最占空间的文件
来源：http://baike.fehbvm.com/Article/details/gmhpdbbjm.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.hesvh.cn/Article/details/ggkhhaujs.sHtML

[R63] 内存与进程
来源：http://read.share.hesvh.cn/Article/details/gzcvbsuar.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.zdbjq.cn/Article/details/gapfyymkh.sHtML

[R64] 结束进程
来源：http://3g.fehbvm.com/Article/details/gqymqonpl.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.zdbjq.cn/Article/details/gfdopsosr.sHtML

[R65] 查看端口占用
来源：http://blog.fehbvm.com/Article/details/gzclfkong.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.hesvh.cn/Article/details/gbdebeatj.sHtML

[R66] 定时任务
来源：http://blog.zdbjq.cn/Article/details/goduzxupt.sHtML

crontab -e;  crontab -l
来源：http://baike.hesvh.cn/Article/details/ggnylgmdq.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.zdbjq.cn/Article/details/ghttqrljr.sHtML

openssl rand -hex 16
来源：http://wap.fehbvm.com/Article/details/gkntrtbug.sHtML

[R68] 计算文件校验值
来源：http://read.share.fehbvm.com/Article/details/geiukczxv.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fehbvm.com/Article/details/gawflcvia.sHtML

[R69] 生成随机密码
来源：http://www.m.share.zdbjq.cn/Article/details/gyotfypnn.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fehbvm.com/Article/details/guonwelki.sHtML

[R70] 时间戳与互转
来源：http://www.share.fehbvm.com/Article/details/ggjsfxqkw.sHtML

date +%s;  date -d @1700000000
来源：http://3g.hesvh.cn/Article/details/gjzgdqegg.sHtML

[R71] 日期格式化
来源：http://wap.hesvh.cn/Article/details/ggknqtmqz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fehbvm.com/Article/details/gxfjhirtp.sHtML

[R72] 等待端口就绪
来源：http://wap.zdbjq.cn/Article/details/gntpxeosu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.hesvh.cn/Article/details/gjbdllgzl.sHtML

[R73] 分割大日志
来源：http://www.blog.fehbvm.com/Article/details/gtqxlpjjc.sHtML

split -l 1000 big.log part_
来源：http://mobile.hesvh.cn/Article/details/gimtmtxkb.sHtML

[R74] 批量重命名
来源：http://wap.fehbvm.com/Article/details/gybwzmshu.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.hesvh.cn/Article/details/gtohvcpet.sHtML

[R75] 导出环境变量
来源：http://wap.zdbjq.cn/Article/details/gozeqacsk.sHtML


<!-- 参考信息 -->