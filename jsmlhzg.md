代发 wailian999

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnbumqgrq.sHtML

[Q28] 求和与平均
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmfhvwlrm.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjeytpfmv.sHtML

[Q29] 最大最小值
来源：http://m.share.fanxiaobao.xyz/Article/details/gamfshbap.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdinzmohw.sHtML

[Q30] 分组统计
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghvmmxuhh.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.fanxiaobao.xyz/Article/details/gcpclwxer.sHtML

[Q31] 分组后过滤
来源：http://blog.fanxiaobao.xyz/Article/details/glthkfstb.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnfnlkvnl.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/goduvyzbp.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.fanxiaobao.xyz/Article/details/gwkvzhwom.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvfjvxjax.sHtML

[Q33] 多列分组
来源：http://baike.fanxiaobao.xyz/Article/details/gihupjjxb.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.fanxiaobao.xyz/Article/details/gknltzyww.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjujdhijr.sHtML

SELECT * FROM (
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpishxxfm.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsgvssuox.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtdlabrqx.sHtML

[Q35] 内连接
来源：http://baike.fanxiaobao.xyz/Article/details/gjnezlsvv.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gppfegegr.sHtML

[Q36] 左连接
来源：http://www.share.fanxiaobao.xyz/Article/details/ggywxyqjg.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gychgdxii.sHtML

[Q37] 右连接
来源：http://wap.fanxiaobao.xyz/Article/details/gxtfmzdyr.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtrigazlw.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.fanxiaobao.xyz/Article/details/gsegiomqu.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpzbtrmce.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.fanxiaobao.xyz/Article/details/gkjsddoif.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.fanxiaobao.xyz/Article/details/gzmwifctt.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.fanxiaobao.xyz/Article/details/gkpvgdmja.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.fanxiaobao.xyz/Article/details/ghdmzqaij.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.fanxiaobao.xyz/Article/details/gchioixcq.sHtML

[Q41] 多表连接
来源：http://3g.fanxiaobao.xyz/Article/details/gndgbhbyn.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gihoymsnv.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gisszscxc.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.fanxiaobao.xyz/Article/details/gyxkyivni.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gwkgzllsj.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.fanxiaobao.xyz/Article/details/gunqszajg.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbeqsguft.sHtML

[Q43] 标量子查询
来源：http://blog.fanxiaobao.xyz/Article/details/gytzhmmjk.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.fanxiaobao.xyz/Article/details/gwujabrxb.sHtML

[Q44] IN 子查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gcaxvywjy.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.fanxiaobao.xyz/Article/details/gpybgowsh.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.fanxiaobao.xyz/Article/details/gguphrkte.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fanxiaobao.xyz/Article/details/ggbggddye.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gznrxextr.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fanxiaobao.xyz/Article/details/ghjfjnzzd.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjmoucejj.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://3g.fanxiaobao.xyz/Article/details/gwxvlcijd.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.fanxiaobao.xyz/Article/details/gqjrxlkgh.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggexrhphr.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.fanxiaobao.xyz/Article/details/givztzchp.sHtML

[Q49] 更新单行
来源：http://m.share.fanxiaobao.xyz/Article/details/gymakfzka.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gleptpzwo.sHtML

[Q50] 批量更新
来源：http://wap.fanxiaobao.xyz/Article/details/gqspnhgey.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.fanxiaobao.xyz/Article/details/gcxhdqlqb.sHtML

[Q51] 用子查询更新
来源：http://mobile.fanxiaobao.xyz/Article/details/gmggpdokv.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gajwstiiz.sHtML

[Q52] 删除指定行
来源：http://wap.fanxiaobao.xyz/Article/details/ghturreee.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gpsrsbnyr.sHtML

[Q53] 按条件删除
来源：http://baike.fanxiaobao.xyz/Article/details/gywlpcjrb.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.fanxiaobao.xyz/Article/details/gvipyuyef.sHtML

[Q54] 清空表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjsjwfsns.sHtML

TRUNCATE TABLE logs;
来源：http://wap.fanxiaobao.xyz/Article/details/gxoaqvhlx.sHtML

[Q55] 排名（并列占位）
来源：http://blog.fanxiaobao.xyz/Article/details/gapeghyyg.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.fanxiaobao.xyz/Article/details/guarberfg.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gappcaiwr.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.fanxiaobao.xyz/Article/details/gaphwdqtg.sHtML

[Q57] 行号
来源：http://read.share.fanxiaobao.xyz/Article/details/gqjvoghhq.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gawvgfnzc.sHtML

[Q58] 累计求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gjqhspwxe.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/griotwnbh.sHtML

[Q59] 分组内累计
来源：http://3g.fanxiaobao.xyz/Article/details/gigiorkst.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/guetlniis.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.fanxiaobao.xyz/Article/details/gqaqesctx.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.fanxiaobao.xyz/Article/details/gabhqfigy.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/glryutpiw.sHtML

[Q61] 移动平均
来源：http://mobile.fanxiaobao.xyz/Article/details/grtqxkiib.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwsquumwv.sHtML

[Q62] 分组占比
来源：http://m.share.fanxiaobao.xyz/Article/details/gtmylqjcf.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.fanxiaobao.xyz/Article/details/glqicdqsg.sHtML

[Q63] 开启事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gchvsqesx.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://3g.fanxiaobao.xyz/Article/details/gisgequsk.sHtML

[Q64] 提交事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gnajfmerz.sHtML

COMMIT;
来源：http://wap.fanxiaobao.xyz/Article/details/gfcmmlsie.sHtML

[Q65] 回滚事务
来源：http://3g.fanxiaobao.xyz/Article/details/gplfnylho.sHtML

ROLLBACK;
来源：http://3g.fanxiaobao.xyz/Article/details/gsqyjovav.sHtML

[Q66] 行锁查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjtcbnsme.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.fanxiaobao.xyz/Article/details/gfwpekfjz.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.fanxiaobao.xyz/Article/details/gldkprmjx.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.fanxiaobao.xyz/Article/details/golcyycfo.sHtML

[Q68] 保存点
来源：http://blog.fanxiaobao.xyz/Article/details/guframsvm.sHtML

SAVEPOINT sp1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpixhitso.sHtML

ROLLBACK TO sp1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnxsdfphj.sHtML

[Q69] 查看执行计划
来源：http://wap.fanxiaobao.xyz/Article/details/geruzhepx.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.fanxiaobao.xyz/Article/details/gbcdcdubm.sHtML

[Q70] 更新统计信息
来源：http://www.share.fanxiaobao.xyz/Article/details/gaoinzjdv.sHtML

ANALYZE TABLE users;
来源：http://baike.fanxiaobao.xyz/Article/details/gguoeqxdn.sHtML

[Q71] 查看建表语句
来源：http://m.share.fanxiaobao.xyz/Article/details/gceovnyjr.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.fanxiaobao.xyz/Article/details/gotfnokgf.sHtML

[Q72] 查看索引
来源：http://mobile.fanxiaobao.xyz/Article/details/geyflpkwt.sHtML

SHOW INDEX FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gtvgqonqc.sHtML

[Q73] 查看表状态
来源：http://m.share.fanxiaobao.xyz/Article/details/gcttmzxyn.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.fanxiaobao.xyz/Article/details/gocsawrfv.sHtML

[Q74] 强制使用索引
来源：http://baike.fanxiaobao.xyz/Article/details/gybqymzeu.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.fanxiaobao.xyz/Article/details/gwehxejqj.sHtML

[Q75] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gxujoygpv.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gdyyblfce.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvgffhsbw.sHtML

[Q76] 按天统计
来源：http://baike.fanxiaobao.xyz/Article/details/gzgmvjcki.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fanxiaobao.xyz/Article/details/gufahxxfe.sHtML

[Q77] 时间加减
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpmshklxq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.fanxiaobao.xyz/Article/details/gobouopiv.sHtML

[Q78] 当前时间
来源：http://wap.fanxiaobao.xyz/Article/details/gxtrpkmls.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.fanxiaobao.xyz/Article/details/gwkvhaund.sHtML

[Q79] 字符串拼接
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggjzsqnyg.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.fanxiaobao.xyz/Article/details/gotkvwpiz.sHtML

[Q80] 字符串截取
来源：http://read.share.fanxiaobao.xyz/Article/details/gmkungvpi.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmvwjyhyy.sHtML

[Q81] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/ghuquriau.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gbyuhjgny.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gihdacepy.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/giituekcm.sHtML

[Q83] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/gezczuzqu.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/geenaenvi.sHtML

[Q84] 去除首尾空格
来源：http://baike.fanxiaobao.xyz/Article/details/glswhqkij.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvtcpvcjj.sHtML

[Q85] 数值取整
来源：http://m.share.fanxiaobao.xyz/Article/details/gambyopnn.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.fanxiaobao.xyz/Article/details/gwhunnrot.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fanxiaobao.xyz/Article/details/giglyzhft.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fanxiaobao.xyz/Article/details/ghkqmkzda.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdfkkecse.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaalynfmw.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggvimcehe.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fanxiaobao.xyz/Article/details/gowqbnemy.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gbsityzwd.sHtML

[Q89] 判断表是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gwhvgvlsu.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fanxiaobao.xyz/Article/details/gpdvifgqx.sHtML

[Q90] 生成序号列
来源：http://www.share.fanxiaobao.xyz/Article/details/gdwavskqk.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fanxiaobao.xyz/Article/details/gxiywvzsb.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gijviewze.sHtML

R. Bash 专题
来源：http://wap.fanxiaobao.xyz/Article/details/ghfsjwgcp.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/glrnpgtdi.sHtML

[R01] shebang 与严格模式
来源：http://blog.fanxiaobao.xyz/Article/details/goiirpsfe.sHtML

#!/usr/bin/env bash
来源：http://baike.fanxiaobao.xyz/Article/details/gtdzjrtwr.sHtML

set -euo pipefail
来源：http://read.share.fanxiaobao.xyz/Article/details/gdsraktim.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fanxiaobao.xyz/Article/details/ghhxwcufq.sHtML

name="Tom"; echo "$name"
来源：http://blog.fanxiaobao.xyz/Article/details/gduuobpaq.sHtML

[R03] 只读变量
来源：http://wap.fanxiaobao.xyz/Article/details/gnduzjhxn.sHtML

readonly PI=3.14
来源：http://wap.fanxiaobao.xyz/Article/details/gdaylnxcm.sHtML

[R04] 位置参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gqusotzsy.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.fanxiaobao.xyz/Article/details/gyuougzae.sHtML

[R05] 参数默认值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbkeviing.sHtML

name="${1:-default}"
来源：http://wap.fanxiaobao.xyz/Article/details/grjnmeyqz.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gboeaunpn.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geaosnwkn.sHtML

[R07] if 判断文件
来源：http://3g.fanxiaobao.xyz/Article/details/gysqrtcga.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gotbjykfj.sHtML

[R08] 数值比较
来源：http://baike.fanxiaobao.xyz/Article/details/gppynifls.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gwtngmakd.sHtML

[R09] 字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gbwnqypsk.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gwvuxbyel.sHtML

[R10] 正则匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gyfkkygum.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glyjogubp.sHtML

[R11] case 多分支
来源：http://m.share.fanxiaobao.xyz/Article/details/gepkanhaa.sHtML

case "$1" in
来源：http://www.share.fanxiaobao.xyz/Article/details/gdicyjzyw.sHtML

start) echo "启动" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/ghbihvrlc.sHtML

stop)  echo "停止" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gqjcitdlg.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gksfcmxiw.sHtML

esac
来源：http://mobile.fanxiaobao.xyz/Article/details/ggmelkoox.sHtML

[R12] for 遍历文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gsdofvmph.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdympyvtc.sHtML

[R13] for 计数循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gvxmwksqc.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gnaowknhf.sHtML

[R14] C 风格 for
来源：http://3g.fanxiaobao.xyz/Article/details/gijlkmsfd.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goueiqujr.sHtML

[R15] while 逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/giuelfwer.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gewjgqpuz.sHtML

[R16] until 等待条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gcmmmgbdi.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gebuxaubl.sHtML

[R17] 数组定义与取值
来源：http://blog.fanxiaobao.xyz/Article/details/gtxbtyprw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkrkrkrmz.sHtML

[R18] 遍历数组
来源：http://wap.fanxiaobao.xyz/Article/details/gnzomsjuz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gadnvucqq.sHtML

[R19] 数组长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gcqkhvwgy.sHtML

echo "${#arr[@]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gqcjdfbmt.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fanxiaobao.xyz/Article/details/gigbnepao.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gepmhjhzn.sHtML

[R21] 字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/ggqeapyqn.sHtML

echo "${#s}"
来源：http://m.share.fanxiaobao.xyz/Article/details/grncbcuvb.sHtML

[R22] 截取子串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guavbekkl.sHtML

echo "${s:0:5}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gfvesjvoa.sHtML

[R23] 字符串替换
来源：http://baike.fanxiaobao.xyz/Article/details/gdzrmnxwo.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fanxiaobao.xyz/Article/details/gjuceobhw.sHtML

[R24] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwakmgfqt.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gddawxtwg.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fanxiaobao.xyz/Article/details/gggqfkhvi.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fanxiaobao.xyz/Article/details/gvthabvlt.sHtML

[R26] 命令替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gesjwqesu.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fanxiaobao.xyz/Article/details/gemlawbnu.sHtML

[R27] 算术展开
来源：http://mobile.fanxiaobao.xyz/Article/details/gtrpscstz.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fanxiaobao.xyz/Article/details/ggrfevarr.sHtML

[R28] 浮点运算
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdzakvgvc.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fanxiaobao.xyz/Article/details/galgmepwe.sHtML

[R29] 定义函数
来源：http://wap.fanxiaobao.xyz/Article/details/ghoxofcdv.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fanxiaobao.xyz/Article/details/gyyqnuhfd.sHtML

[R30] 函数返回状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/gubniksbo.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fanxiaobao.xyz/Article/details/gliuvcpxj.sHtML

[R31] 局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gxujljmuq.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvjyeualr.sHtML

[R32] 参数个数校验
来源：http://mobile.fanxiaobao.xyz/Article/details/gobwolczk.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gztaclyny.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fanxiaobao.xyz/Article/details/gocahxdjk.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fanxiaobao.xyz/Article/details/ggohppqwy.sHtML

[R34] 退出时清理
来源：http://m.share.fanxiaobao.xyz/Article/details/gfpebfopb.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/galxuduky.sHtML

[R35] 后台执行并等待
来源：http://read.share.fanxiaobao.xyz/Article/details/grfvpneur.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fanxiaobao.xyz/Article/details/gegklflzc.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gbqdsspfv.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fanxiaobao.xyz/Article/details/gmhtjigse.sHtML

[R37] 把输出赋给变量
来源：http://baike.fanxiaobao.xyz/Article/details/gcyyowrmp.sHtML

files=$(ls -1)
来源：http://baike.fanxiaobao.xyz/Article/details/gpmxyxtvz.sHtML

[R38] 管道串联
来源：http://www.share.fanxiaobao.xyz/Article/details/grqxfzoue.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gtvqhgpvc.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggfhtqnfn.sHtML

cmd > out.log 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gbohnrvqr.sHtML

[R40] 追加写日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gdiaixewn.sHtML

echo "log" >> out.log
来源：http://blog.fanxiaobao.xyz/Article/details/gmxvxdqzj.sHtML

[R41] 丢弃输出
来源：http://baike.fanxiaobao.xyz/Article/details/gakzlizzi.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcplaylva.sHtML

[R42] 输入重定向
来源：http://mobile.fanxiaobao.xyz/Article/details/gmrklttzn.sHtML

wc -l < a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gvlamibee.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnqzapzqk.sHtML

find . -name "*.log" -type f
来源：http://wap.fanxiaobao.xyz/Article/details/gqyafvyrn.sHtML

[R44] 按修改时间查找
来源：http://m.share.fanxiaobao.xyz/Article/details/ggdpuytrq.sHtML

find . -mtime -7 -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gikuibplt.sHtML

[R45] 批量删除
来源：http://3g.fanxiaobao.xyz/Article/details/gxwcnixsq.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fanxiaobao.xyz/Article/details/gryndaufe.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaxbmsitk.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fanxiaobao.xyz/Article/details/gpepswaru.sHtML

[R47] sed 单行替换
来源：http://wap.fanxiaobao.xyz/Article/details/gwjuzkuoh.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gdjqkhvzy.sHtML

[R48] awk 取指定列
来源：http://blog.fanxiaobao.xyz/Article/details/gobatnvlc.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gbesanmjt.sHtML

[R49] awk 带条件
来源：http://3g.fanxiaobao.xyz/Article/details/gcfucobwc.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fanxiaobao.xyz/Article/details/gottdboom.sHtML

[R50] awk 求和
来源：http://blog.fanxiaobao.xyz/Article/details/gzgptocrp.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtkizrumv.sHtML

[R51] 排序去重取前几
来源：http://blog.fanxiaobao.xyz/Article/details/gmbodxyhg.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.fanxiaobao.xyz/Article/details/gnllnpekg.sHtML

[R52] 统计行数
来源：http://mobile.fanxiaobao.xyz/Article/details/gjsxlkcrx.sHtML

wc -l a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gdolgieon.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fanxiaobao.xyz/Article/details/gyujjjgfm.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fanxiaobao.xyz/Article/details/grqfhlrnz.sHtML

[R54] 比较两个文件
来源：http://wap.fanxiaobao.xyz/Article/details/ggbjbzcjo.sHtML

diff a.txt b.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpzuszhha.sHtML

[R55] 压缩与解压
来源：http://blog.fanxiaobao.xyz/Article/details/grsikixuv.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzhbblvdd.sHtML

[R56] 远程拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gjcjekwhq.sHtML

scp file user@host:/path/
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnvusqqxj.sHtML

[R57] 远程执行命令
来源：http://www.blog.fanxiaobao.xyz/Article/details/giyaliwei.sHtML

ssh user@host 'uptime'
来源：http://wap.fanxiaobao.xyz/Article/details/gropcxzgk.sHtML

[R58] 下载文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gkngvsvvx.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcbtwzvot.sHtML

[R59] 发 POST JSON
来源：http://baike.fanxiaobao.xyz/Article/details/gytmnbbps.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fanxiaobao.xyz/Article/details/gyyveapdv.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwvegfmhh.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fanxiaobao.xyz/Article/details/gbuljnloq.sHtML

[R61] 磁盘占用
来源：http://wap.fanxiaobao.xyz/Article/details/ghntrflrs.sHtML

df -h;  du -sh *
来源：http://blog.fanxiaobao.xyz/Article/details/guxwievqg.sHtML

[R62] 找最占空间的文件
来源：http://3g.fanxiaobao.xyz/Article/details/gwnfxplzp.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfyvmwmkx.sHtML

[R63] 内存与进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gqptobamw.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fanxiaobao.xyz/Article/details/gyakyhvgf.sHtML

[R64] 结束进程
来源：http://wap.fanxiaobao.xyz/Article/details/gkhjperpm.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpfhqpdgr.sHtML

[R65] 查看端口占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gpscaucca.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fanxiaobao.xyz/Article/details/guqrgttdc.sHtML

[R66] 定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gcgyrwopq.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbxxlncar.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fanxiaobao.xyz/Article/details/gvaazoxsd.sHtML

openssl rand -hex 16
来源：http://mobile.fanxiaobao.xyz/Article/details/ggsqghcnv.sHtML

[R68] 计算文件校验值
来源：http://mobile.fanxiaobao.xyz/Article/details/gpfchwiqx.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjktifbsm.sHtML

[R69] 生成随机密码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmixkvrzr.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grxaulkpp.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fanxiaobao.xyz/Article/details/gumnivbgm.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fanxiaobao.xyz/Article/details/gjsufslph.sHtML

[R71] 日期格式化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gozkeizou.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fanxiaobao.xyz/Article/details/gnsrcaxnv.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyreljayu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gjvggnuxe.sHtML

[R73] 分割大日志
来源：http://3g.fanxiaobao.xyz/Article/details/grreubehk.sHtML

split -l 1000 big.log part_
来源：http://www.share.fanxiaobao.xyz/Article/details/gzwhxjnqj.sHtML

[R74] 批量重命名
来源：http://www.blog.fanxiaobao.xyz/Article/details/gggbydoev.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gendrrceg.sHtML

[R75] 导出环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/grwilaxez.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyhiuprrv.sHtML

[R76] 使用临时文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmbxukqmm.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gqvgcesfx.sHtML

[R77] 读取用户输入
来源：http://wap.fanxiaobao.xyz/Article/details/ggmwjdhmy.sHtML


<!-- 参考信息 -->