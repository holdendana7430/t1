代发 wailian999

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://wap.zdbjq.cn/Article/details/grohtunfa.sHtML

[Q24] 去重
来源：http://mobile.zdbjq.cn/Article/details/grnisjnzb.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gzrvssjui.sHtML

[Q25] 只取前 N 条
来源：http://mobile.hesvh.cn/Article/details/gyhlhkefw.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://m.share.fehbvm.com/Article/details/gxazzxvmm.sHtML

[Q26] 计数
来源：http://blog.hesvh.cn/Article/details/gpyrdhmam.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gvateivzj.sHtML

[Q27] 条件计数
来源：http://www.m.share.hesvh.cn/Article/details/gpfyqznab.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gxpetdaem.sHtML

[Q28] 求和与平均
来源：http://www.m.share.fehbvm.com/Article/details/gzvkupvbm.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.hesvh.cn/Article/details/goevinpre.sHtML

[Q29] 最大最小值
来源：http://www.share.fehbvm.com/Article/details/gxzxinpgf.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gznleogup.sHtML

[Q30] 分组统计
来源：http://wap.zdbjq.cn/Article/details/gytivtbso.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/gbhvxtwup.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.hesvh.cn/Article/details/gmcdrkguw.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.hesvh.cn/Article/details/gjibzlmka.sHtML

[Q32] 分组拼接字符串
来源：http://baike.hesvh.cn/Article/details/gqlqdfese.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/galmvzuom.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.hesvh.cn/Article/details/gnhalqvto.sHtML

[Q33] 多列分组
来源：http://3g.zdbjq.cn/Article/details/grxcvtmpb.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.zdbjq.cn/Article/details/gbsqdcske.sHtML

[Q34] 每组取第一条
来源：http://www.blog.zdbjq.cn/Article/details/ghvijdsnt.sHtML

SELECT * FROM (
来源：http://3g.zdbjq.cn/Article/details/ghvvhfudq.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.zdbjq.cn/Article/details/ggqbblghr.sHtML

) t WHERE rn = 1;
来源：http://m.share.hesvh.cn/Article/details/gqrtchkif.sHtML

[Q35] 内连接
来源：http://m.share.zdbjq.cn/Article/details/gwwqtjyfy.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.zdbjq.cn/Article/details/gadluaosb.sHtML

[Q36] 左连接
来源：http://blog.zdbjq.cn/Article/details/gqtreubyo.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.hesvh.cn/Article/details/gqnujkjpc.sHtML

[Q37] 右连接
来源：http://www.m.share.hesvh.cn/Article/details/glevfrlgk.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.fehbvm.com/Article/details/gnkmadtny.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.fehbvm.com/Article/details/gdemutefx.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.zdbjq.cn/Article/details/gvqjbhust.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.hesvh.cn/Article/details/gvlisarzr.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.zdbjq.cn/Article/details/gjjisknfq.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.fehbvm.com/Article/details/gpoxabocb.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.zdbjq.cn/Article/details/gmpcyvmmz.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.zdbjq.cn/Article/details/gwxyhbkmq.sHtML

[Q41] 多表连接
来源：http://read.share.hesvh.cn/Article/details/gvlykhyqn.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.zdbjq.cn/Article/details/gcfbtvfkn.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.zdbjq.cn/Article/details/ginzbloit.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.hesvh.cn/Article/details/gphqtmwpb.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.fehbvm.com/Article/details/gtvtwllpx.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.zdbjq.cn/Article/details/gilsmigwz.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.hesvh.cn/Article/details/gxacxlrnl.sHtML

[Q43] 标量子查询
来源：http://3g.hesvh.cn/Article/details/gzizzvohi.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.zdbjq.cn/Article/details/gcakgpdyp.sHtML

[Q44] IN 子查询
来源：http://read.share.fehbvm.com/Article/details/goxuazijb.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.hesvh.cn/Article/details/gnnbynqzp.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.zdbjq.cn/Article/details/gctqucilj.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fehbvm.com/Article/details/gggtkpurz.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.zdbjq.cn/Article/details/gecxushdt.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.zdbjq.cn/Article/details/gukdccszz.sHtML

[Q47] 与平均值比较
来源：http://wap.fehbvm.com/Article/details/gxynolsiy.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.hesvh.cn/Article/details/gbewjwkoa.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gqfemslna.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.hesvh.cn/Article/details/gwivdmjav.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.fehbvm.com/Article/details/gloesthjn.sHtML

[Q49] 更新单行
来源：http://read.share.hesvh.cn/Article/details/gmuhvndmy.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.zdbjq.cn/Article/details/gdlpleozq.sHtML

[Q50] 批量更新
来源：http://www.blog.fehbvm.com/Article/details/gbkmlinju.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.hesvh.cn/Article/details/gxcpdyrcc.sHtML

[Q51] 用子查询更新
来源：http://www.share.hesvh.cn/Article/details/gbezgdcbx.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.zdbjq.cn/Article/details/gufecbwmf.sHtML

[Q52] 删除指定行
来源：http://www.blog.hesvh.cn/Article/details/gzcynhqzg.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.zdbjq.cn/Article/details/ghlbzqqln.sHtML

[Q53] 按条件删除
来源：http://wap.fehbvm.com/Article/details/gtcrkbjse.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.hesvh.cn/Article/details/gkcfnzjve.sHtML

[Q54] 清空表
来源：http://read.share.zdbjq.cn/Article/details/gdvcwvaim.sHtML

TRUNCATE TABLE logs;
来源：http://3g.fehbvm.com/Article/details/grxryeoov.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.zdbjq.cn/Article/details/gvabqkcts.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.hesvh.cn/Article/details/gdlccycfd.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.fehbvm.com/Article/details/gaglaggsv.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.zdbjq.cn/Article/details/gavrqtfhu.sHtML

[Q57] 行号
来源：http://wap.fehbvm.com/Article/details/gpoqeizmm.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.zdbjq.cn/Article/details/gqiqypetz.sHtML

[Q58] 累计求和
来源：http://blog.hesvh.cn/Article/details/gafutvyjm.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gtupbripj.sHtML

[Q59] 分组内累计
来源：http://mobile.hesvh.cn/Article/details/gshmhnequ.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gbtbodemm.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.fehbvm.com/Article/details/greyghbqa.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.zdbjq.cn/Article/details/gmzqyfitt.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gzhmofkzi.sHtML

[Q61] 移动平均
来源：http://wap.zdbjq.cn/Article/details/gugydoeuw.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.hesvh.cn/Article/details/gubjtnfcz.sHtML

[Q62] 分组占比
来源：http://www.share.fehbvm.com/Article/details/gotzpuxuo.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gsrqsanrc.sHtML

[Q63] 开启事务
来源：http://m.share.zdbjq.cn/Article/details/grzkbkmrh.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.zdbjq.cn/Article/details/gniwhxjlj.sHtML

[Q64] 提交事务
来源：http://baike.zdbjq.cn/Article/details/gnclsceyq.sHtML

COMMIT;
来源：http://mobile.fehbvm.com/Article/details/gwwegaymo.sHtML

[Q65] 回滚事务
来源：http://blog.fehbvm.com/Article/details/gbdjezgcj.sHtML

ROLLBACK;
来源：http://www.m.share.fehbvm.com/Article/details/gaqecliyy.sHtML

[Q66] 行锁查询
来源：http://www.blog.fehbvm.com/Article/details/gqhbawttu.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.hesvh.cn/Article/details/giuuhijyh.sHtML

[Q67] 设置隔离级别
来源：http://m.share.zdbjq.cn/Article/details/gtkxucvgz.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.hesvh.cn/Article/details/gxgrrjagu.sHtML

[Q68] 保存点
来源：http://www.m.share.zdbjq.cn/Article/details/gmwjszqor.sHtML

SAVEPOINT sp1;
来源：http://www.blog.hesvh.cn/Article/details/grlfsbohm.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.hesvh.cn/Article/details/gggmawxbk.sHtML

[Q69] 查看执行计划
来源：http://www.blog.fehbvm.com/Article/details/gvuimjpri.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.zdbjq.cn/Article/details/grhjcssap.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.hesvh.cn/Article/details/gnoxpuxox.sHtML

ANALYZE TABLE users;
来源：http://www.blog.zdbjq.cn/Article/details/ghxlyaorp.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fehbvm.com/Article/details/gyiihstmw.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.zdbjq.cn/Article/details/gtiejctog.sHtML

[Q72] 查看索引
来源：http://read.share.hesvh.cn/Article/details/gczifuqmj.sHtML

SHOW INDEX FROM users;
来源：http://mobile.hesvh.cn/Article/details/ghckdprae.sHtML

[Q73] 查看表状态
来源：http://blog.zdbjq.cn/Article/details/gcubuatye.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.fehbvm.com/Article/details/ghlvejubt.sHtML

[Q74] 强制使用索引
来源：http://baike.hesvh.cn/Article/details/grnphossy.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.zdbjq.cn/Article/details/gsdmllbil.sHtML

[Q75] 日期格式化
来源：http://m.share.zdbjq.cn/Article/details/gfdeukllg.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.hesvh.cn/Article/details/gembpilbz.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.fehbvm.com/Article/details/gkxpkfueo.sHtML

[Q76] 按天统计
来源：http://baike.fehbvm.com/Article/details/gatfvfnkc.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.hesvh.cn/Article/details/gzrzfdyol.sHtML

[Q77] 时间加减
来源：http://www.blog.zdbjq.cn/Article/details/ghoubzdum.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.zdbjq.cn/Article/details/gjisibbfc.sHtML

[Q78] 当前时间
来源：http://blog.hesvh.cn/Article/details/gtvzffhgl.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.hesvh.cn/Article/details/gibigoljp.sHtML

[Q79] 字符串拼接
来源：http://www.blog.zdbjq.cn/Article/details/goexjhyyn.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fehbvm.com/Article/details/gffberukm.sHtML

[Q80] 字符串截取
来源：http://wap.zdbjq.cn/Article/details/gwdalybbk.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gfotxyofa.sHtML

[Q81] 字符串替换
来源：http://www.share.hesvh.cn/Article/details/gqhvyeuza.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.hesvh.cn/Article/details/gxsfgnxyr.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.zdbjq.cn/Article/details/goctzbypp.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.fehbvm.com/Article/details/gifvxrwxh.sHtML

[Q83] 大小写转换
来源：http://read.share.hesvh.cn/Article/details/gtrogdvxf.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gkazqucvi.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.zdbjq.cn/Article/details/gphpvkjjo.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gtzxddbrs.sHtML

[Q85] 数值取整
来源：http://blog.hesvh.cn/Article/details/gfjrpyali.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.zdbjq.cn/Article/details/gqymxyfkp.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.zdbjq.cn/Article/details/gxacnxjmy.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.fehbvm.com/Article/details/gelbqgexe.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.zdbjq.cn/Article/details/glkkldnig.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.hesvh.cn/Article/details/glgtkdyqe.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.hesvh.cn/Article/details/gnxbdxzxf.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.zdbjq.cn/Article/details/gubbdnhms.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gmupundcu.sHtML

[Q89] 判断表是否存在
来源：http://m.share.fehbvm.com/Article/details/ghnenqcmz.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fehbvm.com/Article/details/gxganodht.sHtML

[Q90] 生成序号列
来源：http://mobile.zdbjq.cn/Article/details/gjpwxdafx.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.hesvh.cn/Article/details/gdiyduizd.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/ggjhznqfs.sHtML

R. Bash 专题
来源：http://wap.fehbvm.com/Article/details/gkefzatdu.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gteijpseh.sHtML

[R01] shebang 与严格模式
来源：http://blog.zdbjq.cn/Article/details/glvwvjqbs.sHtML

#!/usr/bin/env bash
来源：http://blog.fehbvm.com/Article/details/gdgrdchfm.sHtML

set -euo pipefail
来源：http://baike.zdbjq.cn/Article/details/gxedegxgq.sHtML

[R02] 变量赋值与使用
来源：http://read.share.hesvh.cn/Article/details/gwsfkunfj.sHtML

name="Tom"; echo "$name"
来源：http://wap.zdbjq.cn/Article/details/gbqhnitsl.sHtML

[R03] 只读变量
来源：http://blog.fehbvm.com/Article/details/gyxkwbsuz.sHtML

readonly PI=3.14
来源：http://www.blog.zdbjq.cn/Article/details/gzxiozscc.sHtML

[R04] 位置参数
来源：http://baike.fehbvm.com/Article/details/gziflrrgh.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.zdbjq.cn/Article/details/gwotbveyr.sHtML

[R05] 参数默认值
来源：http://www.m.share.fehbvm.com/Article/details/gwxmyutin.sHtML

name="${1:-default}"
来源：http://blog.fehbvm.com/Article/details/gqookzopg.sHtML

[R06] 判断命令是否存在
来源：http://m.share.zdbjq.cn/Article/details/gohjpjsrz.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.zdbjq.cn/Article/details/gzvhohipm.sHtML

[R07] if 判断文件
来源：http://www.share.zdbjq.cn/Article/details/gncrxtfth.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.zdbjq.cn/Article/details/gwqdpsrcd.sHtML

[R08] 数值比较
来源：http://read.share.hesvh.cn/Article/details/gluzugwru.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gmnptbswd.sHtML

[R09] 字符串比较
来源：http://m.share.zdbjq.cn/Article/details/gibaeiojz.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fehbvm.com/Article/details/gigkyqhtg.sHtML

[R10] 正则匹配
来源：http://m.share.hesvh.cn/Article/details/gedaywyuq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.zdbjq.cn/Article/details/gaagxxysb.sHtML

[R11] case 多分支
来源：http://3g.zdbjq.cn/Article/details/gxekhcsza.sHtML

case "$1" in
来源：http://www.share.zdbjq.cn/Article/details/gudybroao.sHtML

start) echo "启动" ;;
来源：http://www.blog.fehbvm.com/Article/details/gzomagxqr.sHtML

stop)  echo "停止" ;;
来源：http://blog.zdbjq.cn/Article/details/gmzohmzln.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.hesvh.cn/Article/details/gkmanstzn.sHtML

esac
来源：http://www.blog.zdbjq.cn/Article/details/ghqclqhzr.sHtML

[R12] for 遍历文件
来源：http://www.share.zdbjq.cn/Article/details/grcxtroko.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.hesvh.cn/Article/details/gblmrjvag.sHtML

[R13] for 计数循环
来源：http://www.m.share.zdbjq.cn/Article/details/gqbixvakr.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/gypqebxsc.sHtML

[R14] C 风格 for
来源：http://www.m.share.fehbvm.com/Article/details/garlsdgql.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.hesvh.cn/Article/details/ghtdyqqso.sHtML

[R15] while 逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gelovqhyo.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.zdbjq.cn/Article/details/gnofaebkc.sHtML

[R16] until 等待条件
来源：http://www.share.hesvh.cn/Article/details/gfxubywjn.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.fehbvm.com/Article/details/gzczcjmcs.sHtML

[R17] 数组定义与取值
来源：http://m.share.hesvh.cn/Article/details/gxongfutr.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.zdbjq.cn/Article/details/gfvttevme.sHtML

[R18] 遍历数组
来源：http://baike.hesvh.cn/Article/details/ghyerwpnd.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.hesvh.cn/Article/details/glzjscajd.sHtML

[R19] 数组长度
来源：http://www.m.share.hesvh.cn/Article/details/gviamzomw.sHtML

echo "${#arr[@]}"
来源：http://m.share.zdbjq.cn/Article/details/geztgadmv.sHtML

[R20] 关联数组（字典）
来源：http://wap.hesvh.cn/Article/details/gmucnzhcw.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fehbvm.com/Article/details/gcslgaqoq.sHtML

[R21] 字符串长度
来源：http://mobile.zdbjq.cn/Article/details/gpnhepnmr.sHtML

echo "${#s}"
来源：http://www.blog.fehbvm.com/Article/details/gezfgdfir.sHtML

[R22] 截取子串
来源：http://www.blog.zdbjq.cn/Article/details/gfcvhcrix.sHtML

echo "${s:0:5}"
来源：http://m.share.fehbvm.com/Article/details/grkufpotd.sHtML

[R23] 字符串替换
来源：http://read.share.zdbjq.cn/Article/details/gukdrvasy.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.zdbjq.cn/Article/details/gxqpmhbeq.sHtML

[R24] 大小写转换
来源：http://3g.fehbvm.com/Article/details/gjeeewqeo.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.hesvh.cn/Article/details/guacmbmrk.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.zdbjq.cn/Article/details/gxdowwdqj.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.hesvh.cn/Article/details/gkxcuufht.sHtML

[R26] 命令替换
来源：http://www.m.share.zdbjq.cn/Article/details/gmcwetuqj.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fehbvm.com/Article/details/gjxknkyzi.sHtML

[R27] 算术展开
来源：http://www.blog.hesvh.cn/Article/details/gqbkeqwdm.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.zdbjq.cn/Article/details/gucfzviag.sHtML

[R28] 浮点运算
来源：http://mobile.hesvh.cn/Article/details/gkixalpog.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.zdbjq.cn/Article/details/gfzkwksdd.sHtML

[R29] 定义函数
来源：http://blog.hesvh.cn/Article/details/gvzvqveit.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.zdbjq.cn/Article/details/glrmnthwl.sHtML

[R30] 函数返回状态码
来源：http://www.share.fehbvm.com/Article/details/gobuytpnl.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fehbvm.com/Article/details/gdfhheeef.sHtML

[R31] 局部变量
来源：http://wap.hesvh.cn/Article/details/gyffjqhrg.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.hesvh.cn/Article/details/grikwvsjz.sHtML

[R32] 参数个数校验
来源：http://read.share.fehbvm.com/Article/details/gicpvtehl.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.zdbjq.cn/Article/details/gpkolvedd.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.hesvh.cn/Article/details/gcghflfdz.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.zdbjq.cn/Article/details/gsjzauuzh.sHtML

[R34] 退出时清理
来源：http://www.share.fehbvm.com/Article/details/gltjhszuz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gqicnhjaq.sHtML

[R35] 后台执行并等待
来源：http://baike.fehbvm.com/Article/details/gulxlekkr.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.zdbjq.cn/Article/details/gsnvtjtgd.sHtML

[R36] 并发执行多个任务
来源：http://mobile.zdbjq.cn/Article/details/gbduexdls.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.hesvh.cn/Article/details/gvzrctmyc.sHtML

[R37] 把输出赋给变量
来源：http://blog.fehbvm.com/Article/details/gheweflzz.sHtML

files=$(ls -1)
来源：http://3g.fehbvm.com/Article/details/gqatldkel.sHtML

[R38] 管道串联
来源：http://3g.hesvh.cn/Article/details/gybjrhcxh.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.hesvh.cn/Article/details/gvhlvlgnm.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fehbvm.com/Article/details/ggglyfvvn.sHtML

cmd > out.log 2>&1
来源：http://read.share.zdbjq.cn/Article/details/ggfxhknft.sHtML

[R40] 追加写日志
来源：http://baike.hesvh.cn/Article/details/gdupvxlas.sHtML

echo "log" >> out.log
来源：http://blog.hesvh.cn/Article/details/gdvvbewdk.sHtML

[R41] 丢弃输出
来源：http://www.m.share.zdbjq.cn/Article/details/glcshtwep.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.hesvh.cn/Article/details/gvkcfldwu.sHtML

[R42] 输入重定向
来源：http://read.share.fehbvm.com/Article/details/gbjhjdstp.sHtML

wc -l < a.txt
来源：http://wap.zdbjq.cn/Article/details/gyljrdaqz.sHtML

[R43] 按名字查找文件
来源：http://mobile.hesvh.cn/Article/details/ghtzckhft.sHtML

find . -name "*.log" -type f
来源：http://baike.hesvh.cn/Article/details/gxwznolux.sHtML

[R44] 按修改时间查找
来源：http://mobile.fehbvm.com/Article/details/goojkbsla.sHtML

find . -mtime -7 -type f
来源：http://read.share.fehbvm.com/Article/details/gwwoyfdnb.sHtML

[R45] 批量删除
来源：http://www.blog.hesvh.cn/Article/details/gjmwvddza.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fehbvm.com/Article/details/grpjpzmim.sHtML

[R46] 递归替换文件内容
来源：http://wap.zdbjq.cn/Article/details/gzniamyvg.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.hesvh.cn/Article/details/giptrkfjq.sHtML

[R47] sed 单行替换
来源：http://3g.fehbvm.com/Article/details/gqefbbpxg.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fehbvm.com/Article/details/ghjeumrlz.sHtML

[R48] awk 取指定列
来源：http://3g.hesvh.cn/Article/details/gtrpkxvqw.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fehbvm.com/Article/details/gkbohcuqr.sHtML

[R49] awk 带条件
来源：http://3g.hesvh.cn/Article/details/gxrbtqcam.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fehbvm.com/Article/details/gfsnsieqf.sHtML

[R50] awk 求和
来源：http://read.share.fehbvm.com/Article/details/glvgfosef.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.hesvh.cn/Article/details/glmgvbgpi.sHtML

[R51] 排序去重取前几
来源：http://blog.hesvh.cn/Article/details/gjaepbwws.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.zdbjq.cn/Article/details/gfjpyaeqg.sHtML

[R52] 统计行数
来源：http://www.m.share.zdbjq.cn/Article/details/gbqiybemt.sHtML

wc -l a.txt
来源：http://wap.fehbvm.com/Article/details/gvxhpttjo.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fehbvm.com/Article/details/grzreykdl.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.hesvh.cn/Article/details/gzoixzanh.sHtML

[R54] 比较两个文件
来源：http://baike.hesvh.cn/Article/details/gupchrorp.sHtML

diff a.txt b.txt
来源：http://www.blog.fehbvm.com/Article/details/gbjcoaeos.sHtML

[R55] 压缩与解压
来源：http://www.blog.hesvh.cn/Article/details/guvsbfmqc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.hesvh.cn/Article/details/ggvmrsupq.sHtML

[R56] 远程拷贝
来源：http://m.share.hesvh.cn/Article/details/gpkwfexfx.sHtML

scp file user@host:/path/
来源：http://3g.zdbjq.cn/Article/details/gamagvrqd.sHtML

[R57] 远程执行命令
来源：http://3g.zdbjq.cn/Article/details/gaggvxjfi.sHtML

ssh user@host 'uptime'
来源：http://read.share.hesvh.cn/Article/details/gbuwohrvj.sHtML

[R58] 下载文件
来源：http://3g.fehbvm.com/Article/details/gebqztrge.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.zdbjq.cn/Article/details/gonlfsilk.sHtML

[R59] 发 POST JSON
来源：http://blog.fehbvm.com/Article/details/gwdzzjcvv.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.hesvh.cn/Article/details/gjumwlaze.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.hesvh.cn/Article/details/gynpvjjxj.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fehbvm.com/Article/details/gjsjtbxdi.sHtML

[R61] 磁盘占用
来源：http://wap.zdbjq.cn/Article/details/gmplpyadh.sHtML

df -h;  du -sh *
来源：http://m.share.zdbjq.cn/Article/details/gqpximiia.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fehbvm.com/Article/details/gsweptwtj.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.zdbjq.cn/Article/details/gzcbbsamo.sHtML

[R63] 内存与进程
来源：http://www.blog.fehbvm.com/Article/details/geokygzym.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fehbvm.com/Article/details/gumtuoqid.sHtML

[R64] 结束进程
来源：http://mobile.fehbvm.com/Article/details/gcgfsucva.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fehbvm.com/Article/details/gyrhxxcfs.sHtML

[R65] 查看端口占用
来源：http://3g.fehbvm.com/Article/details/gmwqmqfch.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fehbvm.com/Article/details/gqxzjxeew.sHtML

[R66] 定时任务
来源：http://m.share.hesvh.cn/Article/details/gggeawqpg.sHtML

crontab -e;  crontab -l
来源：http://m.share.zdbjq.cn/Article/details/gjuafybak.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.zdbjq.cn/Article/details/grcxauxxf.sHtML

openssl rand -hex 16
来源：http://wap.hesvh.cn/Article/details/gjocozuxp.sHtML

[R68] 计算文件校验值
来源：http://blog.zdbjq.cn/Article/details/gpvlzanpy.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fehbvm.com/Article/details/gwswjcypk.sHtML

[R69] 生成随机密码
来源：http://wap.hesvh.cn/Article/details/ghbgboner.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.hesvh.cn/Article/details/gptxojqwp.sHtML

[R70] 时间戳与互转
来源：http://www.blog.zdbjq.cn/Article/details/gmsscrhvn.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.zdbjq.cn/Article/details/gkjnkptrl.sHtML

[R71] 日期格式化
来源：http://read.share.hesvh.cn/Article/details/gvxsxbzri.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.zdbjq.cn/Article/details/gmrihuzzq.sHtML

[R72] 等待端口就绪
来源：http://www.share.zdbjq.cn/Article/details/gyojfvzzb.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.hesvh.cn/Article/details/gexnqrcmr.sHtML

[R73] 分割大日志
来源：http://www.blog.hesvh.cn/Article/details/gxukadxxj.sHtML


<!-- 参考信息 -->