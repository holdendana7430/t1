代发 wailian999

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.fanxiaobao.xyz/Article/details/ghovtmzkc.sHtML

[Q26] 计数
来源：http://m.share.fanxiaobao.xyz/Article/details/gyuhlszer.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjcrpixet.sHtML

[Q27] 条件计数
来源：http://wap.fanxiaobao.xyz/Article/details/gasfdarhd.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gaodtgysc.sHtML

[Q28] 求和与平均
来源：http://baike.fanxiaobao.xyz/Article/details/gizgczvyd.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/genangjpk.sHtML

[Q29] 最大最小值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkshvxeog.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqxxjdpwe.sHtML

[Q30] 分组统计
来源：http://3g.fanxiaobao.xyz/Article/details/gysncvpeb.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.fanxiaobao.xyz/Article/details/gsnorygzp.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grchvtppj.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqnlfiddu.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwssldgpq.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.fanxiaobao.xyz/Article/details/gfvyjhdcd.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.fanxiaobao.xyz/Article/details/gwrafczjd.sHtML

[Q33] 多列分组
来源：http://www.share.fanxiaobao.xyz/Article/details/ggcdhnyzb.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.fanxiaobao.xyz/Article/details/gpielemrs.sHtML

[Q34] 每组取第一条
来源：http://www.share.fanxiaobao.xyz/Article/details/gnvoycfxf.sHtML

SELECT * FROM (
来源：http://3g.fanxiaobao.xyz/Article/details/gxhtkhvkb.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.fanxiaobao.xyz/Article/details/gmdowduvb.sHtML

) t WHERE rn = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gjykwhspn.sHtML

[Q35] 内连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gcgaovulk.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjmvxnaqt.sHtML

[Q36] 左连接
来源：http://wap.fanxiaobao.xyz/Article/details/glysbwrpt.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.fanxiaobao.xyz/Article/details/gsvthglel.sHtML

[Q37] 右连接
来源：http://blog.fanxiaobao.xyz/Article/details/gqxbnuoxv.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwhbzuwlt.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.fanxiaobao.xyz/Article/details/grkpdvqui.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.fanxiaobao.xyz/Article/details/gwmvsjgxk.sHtML

[Q39] 自连接（查上下级）
来源：http://baike.fanxiaobao.xyz/Article/details/gtupdswfg.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.fanxiaobao.xyz/Article/details/ggbejiunx.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkypytjai.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.fanxiaobao.xyz/Article/details/gfeopsrbe.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.fanxiaobao.xyz/Article/details/gogodwkkp.sHtML

[Q41] 多表连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gvfvfdiek.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.fanxiaobao.xyz/Article/details/gpsdvzpfz.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.fanxiaobao.xyz/Article/details/grpmfutme.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqpuacewo.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gyyfjjyfg.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.fanxiaobao.xyz/Article/details/gsdqbvnoy.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.fanxiaobao.xyz/Article/details/ghdtxiufd.sHtML

[Q43] 标量子查询
来源：http://3g.fanxiaobao.xyz/Article/details/gvjjdjyqq.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gztvbkngf.sHtML

[Q44] IN 子查询
来源：http://blog.fanxiaobao.xyz/Article/details/gdxydyvvm.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtgvehrlk.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkxfspigs.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fanxiaobao.xyz/Article/details/gazovrrhu.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.fanxiaobao.xyz/Article/details/gtsotbapm.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fanxiaobao.xyz/Article/details/glwqxfrhe.sHtML

[Q47] 与平均值比较
来源：http://blog.fanxiaobao.xyz/Article/details/gllzjlgor.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grupgslye.sHtML

[Q48] CTE 公用表表达式
来源：http://wap.fanxiaobao.xyz/Article/details/ghlqdtflk.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.fanxiaobao.xyz/Article/details/gfcenridp.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqbseqhbl.sHtML

[Q49] 更新单行
来源：http://mobile.fanxiaobao.xyz/Article/details/gxxeunzmd.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gulsplhip.sHtML

[Q50] 批量更新
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gozvuuuxd.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.fanxiaobao.xyz/Article/details/gpytpusoq.sHtML

[Q51] 用子查询更新
来源：http://www.blog.fanxiaobao.xyz/Article/details/gemsjpvzb.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gbyntdnen.sHtML

[Q52] 删除指定行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwlpmjswa.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwebhxgul.sHtML

[Q53] 按条件删除
来源：http://wap.fanxiaobao.xyz/Article/details/gpslbmfdg.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.fanxiaobao.xyz/Article/details/gayqfymeq.sHtML

[Q54] 清空表
来源：http://wap.fanxiaobao.xyz/Article/details/gqbhidkcm.sHtML

TRUNCATE TABLE logs;
来源：http://baike.fanxiaobao.xyz/Article/details/glgsiwizc.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.fanxiaobao.xyz/Article/details/gyvhswcbt.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/godaflxgw.sHtML

[Q56] 密集排名（并列不占位）
来源：http://baike.fanxiaobao.xyz/Article/details/gxshnlwwa.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.fanxiaobao.xyz/Article/details/gghbrambu.sHtML

[Q57] 行号
来源：http://mobile.fanxiaobao.xyz/Article/details/gwvoxdhix.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gcvbzuqsa.sHtML

[Q58] 累计求和
来源：http://blog.fanxiaobao.xyz/Article/details/ginlslylr.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gxfonuqhk.sHtML

[Q59] 分组内累计
来源：http://www.blog.fanxiaobao.xyz/Article/details/glurdqiou.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmdwaxkbk.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.fanxiaobao.xyz/Article/details/gcmhsyrts.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.fanxiaobao.xyz/Article/details/gfbjczadk.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gaypnjqrp.sHtML

[Q61] 移动平均
来源：http://baike.fanxiaobao.xyz/Article/details/gyfvtbhvq.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gzpehuknd.sHtML

[Q62] 分组占比
来源：http://3g.fanxiaobao.xyz/Article/details/gokuwavbr.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.fanxiaobao.xyz/Article/details/gijkjvuvu.sHtML

[Q63] 开启事务
来源：http://m.share.fanxiaobao.xyz/Article/details/gsgticfdq.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggvrbidor.sHtML

[Q64] 提交事务
来源：http://baike.fanxiaobao.xyz/Article/details/gfjememuw.sHtML

COMMIT;
来源：http://3g.fanxiaobao.xyz/Article/details/gzpdncfyq.sHtML

[Q65] 回滚事务
来源：http://baike.fanxiaobao.xyz/Article/details/gxjhbbgxz.sHtML

ROLLBACK;
来源：http://baike.fanxiaobao.xyz/Article/details/grfnloyoh.sHtML

[Q66] 行锁查询
来源：http://baike.fanxiaobao.xyz/Article/details/ggnysafid.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqlzistom.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.fanxiaobao.xyz/Article/details/glxavdelw.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.fanxiaobao.xyz/Article/details/gefzybdnp.sHtML

[Q68] 保存点
来源：http://blog.fanxiaobao.xyz/Article/details/gbexnvdmo.sHtML

SAVEPOINT sp1;
来源：http://m.share.fanxiaobao.xyz/Article/details/glkaiwmeo.sHtML

ROLLBACK TO sp1;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggijqawqs.sHtML

[Q69] 查看执行计划
来源：http://mobile.fanxiaobao.xyz/Article/details/gdeopboph.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.fanxiaobao.xyz/Article/details/gqtsghjja.sHtML

[Q70] 更新统计信息
来源：http://www.share.fanxiaobao.xyz/Article/details/gcagjzfzq.sHtML

ANALYZE TABLE users;
来源：http://baike.fanxiaobao.xyz/Article/details/gbyowgzga.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfhfcaapv.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.fanxiaobao.xyz/Article/details/gqkgggiyl.sHtML

[Q72] 查看索引
来源：http://www.share.fanxiaobao.xyz/Article/details/ghsueiayz.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gexeowkvg.sHtML

[Q73] 查看表状态
来源：http://3g.fanxiaobao.xyz/Article/details/guxhcpuse.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.fanxiaobao.xyz/Article/details/grnniznta.sHtML

[Q74] 强制使用索引
来源：http://read.share.fanxiaobao.xyz/Article/details/glrceblfd.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.fanxiaobao.xyz/Article/details/gjkyqvixs.sHtML

[Q75] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/ghxhhzwll.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzgorvrcm.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fanxiaobao.xyz/Article/details/gxxwcqxtc.sHtML

[Q76] 按天统计
来源：http://read.share.fanxiaobao.xyz/Article/details/gednomggh.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.fanxiaobao.xyz/Article/details/gujoaaxci.sHtML

[Q77] 时间加减
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmncslbjm.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fanxiaobao.xyz/Article/details/gobtvdqjp.sHtML

[Q78] 当前时间
来源：http://mobile.fanxiaobao.xyz/Article/details/gelqdcwgg.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.fanxiaobao.xyz/Article/details/gifhkozmc.sHtML

[Q79] 字符串拼接
来源：http://read.share.fanxiaobao.xyz/Article/details/gmdunqkmf.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxdjlxmpg.sHtML

[Q80] 字符串截取
来源：http://m.share.fanxiaobao.xyz/Article/details/gmraraszt.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwsooydpp.sHtML

[Q81] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gochptkgs.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gutltabcx.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.fanxiaobao.xyz/Article/details/grnvzyuik.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/ggwxhvwnh.sHtML

[Q83] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/gstkalzgk.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gflbrlvlx.sHtML

[Q84] 去除首尾空格
来源：http://m.share.fanxiaobao.xyz/Article/details/gxroabuyi.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/genqxuhda.sHtML

[Q85] 数值取整
来源：http://mobile.fanxiaobao.xyz/Article/details/gfsmgiubu.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.fanxiaobao.xyz/Article/details/gwgogltfz.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.fanxiaobao.xyz/Article/details/gnkmypqcz.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.fanxiaobao.xyz/Article/details/gbtalutnx.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gpznwfpvy.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwwkryvyc.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fanxiaobao.xyz/Article/details/grvysvaou.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.fanxiaobao.xyz/Article/details/gbcapdpha.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gejivazkx.sHtML

[Q89] 判断表是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gebrypbmo.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.fanxiaobao.xyz/Article/details/golavvhgk.sHtML

[Q90] 生成序号列
来源：http://baike.fanxiaobao.xyz/Article/details/gmgmobbyf.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.fanxiaobao.xyz/Article/details/gvvgvwynr.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gwvfewnwe.sHtML

R. Bash 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gikzfcwmy.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/ghhezzrwd.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fanxiaobao.xyz/Article/details/ginjphhue.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghsktucjz.sHtML

set -euo pipefail
来源：http://mobile.fanxiaobao.xyz/Article/details/gjbljsaed.sHtML

[R02] 变量赋值与使用
来源：http://3g.fanxiaobao.xyz/Article/details/ggkzuzouo.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fanxiaobao.xyz/Article/details/grvqtddvm.sHtML

[R03] 只读变量
来源：http://wap.fanxiaobao.xyz/Article/details/gdsmrlkdv.sHtML

readonly PI=3.14
来源：http://read.share.fanxiaobao.xyz/Article/details/gesunhzkv.sHtML

[R04] 位置参数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfuhctgxj.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fanxiaobao.xyz/Article/details/gkyrznqij.sHtML

[R05] 参数默认值
来源：http://wap.fanxiaobao.xyz/Article/details/gftohfxup.sHtML

name="${1:-default}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdgxjznrv.sHtML

[R06] 判断命令是否存在
来源：http://3g.fanxiaobao.xyz/Article/details/gnysgtdpg.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/giylzqmjk.sHtML

[R07] if 判断文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/getysrtah.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gefnmkjva.sHtML

[R08] 数值比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gmneqskqt.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbaicxkpp.sHtML

[R09] 字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gifrkwizo.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gwhqvftbo.sHtML

[R10] 正则匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gyfqrzzar.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gdepnidxc.sHtML

[R11] case 多分支
来源：http://m.share.fanxiaobao.xyz/Article/details/gyxzbrnyf.sHtML

case "$1" in
来源：http://baike.fanxiaobao.xyz/Article/details/goagzzwxt.sHtML

start) echo "启动" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/ghmicoimh.sHtML

stop)  echo "停止" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gozhsearw.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnvhmwzkt.sHtML

esac
来源：http://mobile.fanxiaobao.xyz/Article/details/goypslnup.sHtML

[R12] for 遍历文件
来源：http://baike.fanxiaobao.xyz/Article/details/gudvnbviw.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gxjptndwv.sHtML

[R13] for 计数循环
来源：http://wap.fanxiaobao.xyz/Article/details/gaqztdflq.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtuxvsrsp.sHtML

[R14] C 风格 for
来源：http://3g.fanxiaobao.xyz/Article/details/gfhywnvsu.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gtgpwcmub.sHtML

[R15] while 逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/guvovncwr.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/guexxixxm.sHtML

[R16] until 等待条件
来源：http://baike.fanxiaobao.xyz/Article/details/guoqhvsqq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvizchguv.sHtML

[R17] 数组定义与取值
来源：http://m.share.fanxiaobao.xyz/Article/details/gmnaqrewx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gypbefaak.sHtML

[R18] 遍历数组
来源：http://www.share.fanxiaobao.xyz/Article/details/gxombvpdh.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpxecsgdt.sHtML

[R19] 数组长度
来源：http://3g.fanxiaobao.xyz/Article/details/gjiqvbfgr.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbnoieloj.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fanxiaobao.xyz/Article/details/gogcfaxfj.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gbsbahlug.sHtML

[R21] 字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/garxuyrtq.sHtML

echo "${#s}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gputzhbgi.sHtML

[R22] 截取子串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gctttbiox.sHtML

echo "${s:0:5}"
来源：http://wap.fanxiaobao.xyz/Article/details/gholtvxcj.sHtML

[R23] 字符串替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gmxstvcua.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fanxiaobao.xyz/Article/details/gfyvadxms.sHtML

[R24] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/goxeqztwn.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fanxiaobao.xyz/Article/details/gebcxllac.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fanxiaobao.xyz/Article/details/ggkybkvlc.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsodxyoom.sHtML

[R26] 命令替换
来源：http://wap.fanxiaobao.xyz/Article/details/gdufpydmh.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fanxiaobao.xyz/Article/details/gxlvomztj.sHtML

[R27] 算术展开
来源：http://wap.fanxiaobao.xyz/Article/details/ggeakiahk.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fanxiaobao.xyz/Article/details/ghyoowzxt.sHtML

[R28] 浮点运算
来源：http://m.share.fanxiaobao.xyz/Article/details/gejjjrbpr.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fanxiaobao.xyz/Article/details/gbhxyrjqg.sHtML

[R29] 定义函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsnoiezof.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkqwfupkm.sHtML

[R30] 函数返回状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/giveblpmm.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggsydrxbz.sHtML

[R31] 局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gcpakvjrc.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gxncimtqk.sHtML

[R32] 参数个数校验
来源：http://read.share.fanxiaobao.xyz/Article/details/gjfmhmpyz.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gpzdhrnao.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.fanxiaobao.xyz/Article/details/gggiltqcj.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fanxiaobao.xyz/Article/details/gudfitred.sHtML

[R34] 退出时清理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaeaiyxxk.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gvlmasbuh.sHtML

[R35] 后台执行并等待
来源：http://3g.fanxiaobao.xyz/Article/details/gxkgrlhak.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fanxiaobao.xyz/Article/details/gxvybahgz.sHtML

[R36] 并发执行多个任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gztfelevj.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fanxiaobao.xyz/Article/details/gnuafgzlb.sHtML

[R37] 把输出赋给变量
来源：http://baike.fanxiaobao.xyz/Article/details/gmeyvwuhv.sHtML

files=$(ls -1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gnlxhjevn.sHtML

[R38] 管道串联
来源：http://3g.fanxiaobao.xyz/Article/details/gjkoiivuf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fanxiaobao.xyz/Article/details/gvlvtivlm.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fanxiaobao.xyz/Article/details/gjvghfpok.sHtML

cmd > out.log 2>&1
来源：http://blog.fanxiaobao.xyz/Article/details/gvowxbtgy.sHtML

[R40] 追加写日志
来源：http://read.share.fanxiaobao.xyz/Article/details/grzesnvnp.sHtML

echo "log" >> out.log
来源：http://3g.fanxiaobao.xyz/Article/details/gavceyosn.sHtML

[R41] 丢弃输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gteqmvdeh.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gboprmlwu.sHtML

[R42] 输入重定向
来源：http://3g.fanxiaobao.xyz/Article/details/gowcptbzx.sHtML

wc -l < a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqqhgkksw.sHtML

[R43] 按名字查找文件
来源：http://baike.fanxiaobao.xyz/Article/details/gyiqgpuwc.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtxuowgsv.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gluyxffwe.sHtML

find . -mtime -7 -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gdgmwjwdc.sHtML

[R45] 批量删除
来源：http://blog.fanxiaobao.xyz/Article/details/geypvegca.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fanxiaobao.xyz/Article/details/gfilcawco.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fanxiaobao.xyz/Article/details/gyqhvbybi.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxiqzmtff.sHtML

[R47] sed 单行替换
来源：http://3g.fanxiaobao.xyz/Article/details/gcbumabkv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gnraukyxg.sHtML

[R48] awk 取指定列
来源：http://www.share.fanxiaobao.xyz/Article/details/gnqqanose.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gohqysyrq.sHtML

[R49] awk 带条件
来源：http://3g.fanxiaobao.xyz/Article/details/gbaoriebb.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fanxiaobao.xyz/Article/details/gaujprgkw.sHtML

[R50] awk 求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkxsmpama.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gldiauswc.sHtML

[R51] 排序去重取前几
来源：http://m.share.fanxiaobao.xyz/Article/details/gbhtdgcly.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fanxiaobao.xyz/Article/details/gkxeqsryw.sHtML

[R52] 统计行数
来源：http://baike.fanxiaobao.xyz/Article/details/gmceehcyz.sHtML

wc -l a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gnnuttgxl.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fanxiaobao.xyz/Article/details/gdixkagjp.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fanxiaobao.xyz/Article/details/guafaeayw.sHtML

[R54] 比较两个文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gcshvjdyy.sHtML

diff a.txt b.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gtihidgnc.sHtML

[R55] 压缩与解压
来源：http://m.share.fanxiaobao.xyz/Article/details/goborejzw.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fanxiaobao.xyz/Article/details/gaqtdljgm.sHtML

[R56] 远程拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzajuwykv.sHtML

scp file user@host:/path/
来源：http://baike.fanxiaobao.xyz/Article/details/gygqbatvo.sHtML

[R57] 远程执行命令
来源：http://wap.fanxiaobao.xyz/Article/details/gzyerkqbo.sHtML

ssh user@host 'uptime'
来源：http://3g.fanxiaobao.xyz/Article/details/ghbzjshxf.sHtML

[R58] 下载文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geqmksemc.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fanxiaobao.xyz/Article/details/glyhjctjh.sHtML

[R59] 发 POST JSON
来源：http://mobile.fanxiaobao.xyz/Article/details/gaptrpapw.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fanxiaobao.xyz/Article/details/gjvhihkpj.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gdxwolqpc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fanxiaobao.xyz/Article/details/gosjjofsz.sHtML

[R61] 磁盘占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjazavhad.sHtML

df -h;  du -sh *
来源：http://baike.fanxiaobao.xyz/Article/details/gwpcbpkme.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gezhqabfi.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fanxiaobao.xyz/Article/details/gnldretkr.sHtML

[R63] 内存与进程
来源：http://wap.fanxiaobao.xyz/Article/details/gwlfhtkhh.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fanxiaobao.xyz/Article/details/glfngyrpa.sHtML

[R64] 结束进程
来源：http://baike.fanxiaobao.xyz/Article/details/gqlvsfzgl.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fanxiaobao.xyz/Article/details/gmwjzxmzk.sHtML

[R65] 查看端口占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gzbsparoz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fanxiaobao.xyz/Article/details/gwgqbtyhn.sHtML

[R66] 定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gxmxxbsne.sHtML

crontab -e;  crontab -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gxeposbde.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fanxiaobao.xyz/Article/details/glfzymlwm.sHtML

openssl rand -hex 16
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtcstqudn.sHtML

[R68] 计算文件校验值
来源：http://www.share.fanxiaobao.xyz/Article/details/gemytfpnz.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/ghlphbqky.sHtML

[R69] 生成随机密码
来源：http://wap.fanxiaobao.xyz/Article/details/gqubpvmli.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fanxiaobao.xyz/Article/details/glkeoauht.sHtML

[R70] 时间戳与互转
来源：http://m.share.fanxiaobao.xyz/Article/details/glwdnugtb.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fanxiaobao.xyz/Article/details/gplsixfml.sHtML

[R71] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gynamcbhv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fanxiaobao.xyz/Article/details/gihxzpgca.sHtML

[R72] 等待端口就绪
来源：http://read.share.fanxiaobao.xyz/Article/details/gioutseob.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gjshemtmb.sHtML

[R73] 分割大日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxgajyogb.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gesieclog.sHtML

[R74] 批量重命名
来源：http://read.share.fanxiaobao.xyz/Article/details/gichkccaf.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/ganibyjqm.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gerewarwl.sHtML


<!-- 参考信息 -->