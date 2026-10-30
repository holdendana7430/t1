代发 wailian999

SELECT * FROM users WHERE email IS NULL;
来源：http://www.blog.fehbvm.com/Article/details/gxizjbzti.sHtML

[Q22] 排序
来源：http://www.share.fehbvm.com/Article/details/gjgivjvbu.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://mobile.zdbjq.cn/Article/details/goiavenkq.sHtML

[Q23] 分页
来源：http://mobile.fehbvm.com/Article/details/gxayafycc.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.fehbvm.com/Article/details/gfnngpjag.sHtML

[Q24] 去重
来源：http://blog.zdbjq.cn/Article/details/glcmsqbfh.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.hesvh.cn/Article/details/giyedrqso.sHtML

[Q25] 只取前 N 条
来源：http://blog.fehbvm.com/Article/details/gpclgtarr.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.zdbjq.cn/Article/details/gludnozel.sHtML

[Q26] 计数
来源：http://www.share.hesvh.cn/Article/details/gxfxoznud.sHtML

SELECT COUNT(*) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gsswkmgea.sHtML

[Q27] 条件计数
来源：http://www.share.hesvh.cn/Article/details/gnmduvymp.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.zdbjq.cn/Article/details/gxzubqqtz.sHtML

[Q28] 求和与平均
来源：http://3g.zdbjq.cn/Article/details/gonragxgx.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.fehbvm.com/Article/details/gozymyicu.sHtML

[Q29] 最大最小值
来源：http://blog.fehbvm.com/Article/details/gjcmiumgm.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.fehbvm.com/Article/details/gvvcttpeb.sHtML

[Q30] 分组统计
来源：http://baike.zdbjq.cn/Article/details/gncfapjan.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/gvkwwvrfg.sHtML

[Q31] 分组后过滤
来源：http://mobile.fehbvm.com/Article/details/gicljelny.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.hesvh.cn/Article/details/gzoxdbysk.sHtML

[Q32] 分组拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gfnfowvid.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/giwlhrmol.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.fehbvm.com/Article/details/gtdhmebhr.sHtML

[Q33] 多列分组
来源：http://www.m.share.hesvh.cn/Article/details/gdygxsbgi.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://blog.zdbjq.cn/Article/details/gtozmiksh.sHtML

[Q34] 每组取第一条
来源：http://baike.fehbvm.com/Article/details/gwdetudjs.sHtML

SELECT * FROM (
来源：http://baike.hesvh.cn/Article/details/gwwuobboi.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://3g.zdbjq.cn/Article/details/gughvqvit.sHtML

) t WHERE rn = 1;
来源：http://3g.zdbjq.cn/Article/details/gsryizviq.sHtML

[Q35] 内连接
来源：http://www.blog.hesvh.cn/Article/details/gqgcaefsv.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.fehbvm.com/Article/details/gwxfjyumi.sHtML

[Q36] 左连接
来源：http://mobile.hesvh.cn/Article/details/goupbzdsl.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.hesvh.cn/Article/details/gmxhdhoil.sHtML

[Q37] 右连接
来源：http://3g.hesvh.cn/Article/details/glcjdchau.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.zdbjq.cn/Article/details/gavklslaj.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.fehbvm.com/Article/details/gangpjlzu.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.hesvh.cn/Article/details/gfvumiswm.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.hesvh.cn/Article/details/gzwoiusdj.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.hesvh.cn/Article/details/gbhqfalsc.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.fehbvm.com/Article/details/ggjzmjepw.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.zdbjq.cn/Article/details/grbdtfrxb.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.hesvh.cn/Article/details/gyhovouzj.sHtML

[Q41] 多表连接
来源：http://mobile.zdbjq.cn/Article/details/govxelnlw.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.fehbvm.com/Article/details/gfqzbrnnd.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.hesvh.cn/Article/details/guiskwvzk.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.hesvh.cn/Article/details/gfdhwlrxf.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.hesvh.cn/Article/details/gelvfndtn.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.fehbvm.com/Article/details/gowoxfzxa.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.zdbjq.cn/Article/details/gvptaiaxz.sHtML

[Q43] 标量子查询
来源：http://baike.fehbvm.com/Article/details/gfsolnmww.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.hesvh.cn/Article/details/gufcolaih.sHtML

[Q44] IN 子查询
来源：http://read.share.fehbvm.com/Article/details/gsrfqmfzs.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.hesvh.cn/Article/details/ghopzktsy.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.hesvh.cn/Article/details/gcmyyggpr.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.zdbjq.cn/Article/details/ghpesyczk.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.zdbjq.cn/Article/details/gfzzdfgak.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.hesvh.cn/Article/details/gvrgjrjbb.sHtML

[Q47] 与平均值比较
来源：http://blog.hesvh.cn/Article/details/gtyydxfwd.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.zdbjq.cn/Article/details/gpvvsigjc.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.hesvh.cn/Article/details/gkvmlfowc.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.hesvh.cn/Article/details/ghkanerbj.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.zdbjq.cn/Article/details/geiizrnbi.sHtML

[Q49] 更新单行
来源：http://read.share.zdbjq.cn/Article/details/gndvkcbry.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.hesvh.cn/Article/details/gmxbzawxr.sHtML

[Q50] 批量更新
来源：http://www.blog.fehbvm.com/Article/details/gmcvgabap.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.zdbjq.cn/Article/details/gkwfjqlqr.sHtML

[Q51] 用子查询更新
来源：http://blog.fehbvm.com/Article/details/gmvdrdpnq.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.hesvh.cn/Article/details/gbwvmnnyi.sHtML

[Q52] 删除指定行
来源：http://mobile.hesvh.cn/Article/details/gklhaepno.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.fehbvm.com/Article/details/ggelwwfii.sHtML

[Q53] 按条件删除
来源：http://m.share.zdbjq.cn/Article/details/gwacabpeo.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.fehbvm.com/Article/details/gixpajahz.sHtML

[Q54] 清空表
来源：http://www.m.share.fehbvm.com/Article/details/gnuzyhsjb.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.zdbjq.cn/Article/details/gjrxpttex.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.fehbvm.com/Article/details/gfiftlmkq.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.zdbjq.cn/Article/details/gfloggmou.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.fehbvm.com/Article/details/gkctgmbiz.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.hesvh.cn/Article/details/gjvpcjusu.sHtML

[Q57] 行号
来源：http://www.share.hesvh.cn/Article/details/gnihtmgtq.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/grkmkswjx.sHtML

[Q58] 累计求和
来源：http://baike.hesvh.cn/Article/details/gktcvgzyu.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gcotqbzll.sHtML

[Q59] 分组内累计
来源：http://www.share.fehbvm.com/Article/details/gyfsgavwc.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/geegzzhmh.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.fehbvm.com/Article/details/gkncflewx.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.fehbvm.com/Article/details/gzmicrbdh.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fehbvm.com/Article/details/gzjpplxgi.sHtML

[Q61] 移动平均
来源：http://m.share.zdbjq.cn/Article/details/girgiqxfi.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.hesvh.cn/Article/details/gzpvwdhva.sHtML

[Q62] 分组占比
来源：http://www.blog.hesvh.cn/Article/details/gcpiaysgz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/ghgmjhwtb.sHtML

[Q63] 开启事务
来源：http://wap.zdbjq.cn/Article/details/gemdntvij.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.zdbjq.cn/Article/details/gjmimqpem.sHtML

[Q64] 提交事务
来源：http://wap.fehbvm.com/Article/details/gepkrnguh.sHtML

COMMIT;
来源：http://mobile.hesvh.cn/Article/details/geguutsne.sHtML

[Q65] 回滚事务
来源：http://www.m.share.fehbvm.com/Article/details/gmzetktri.sHtML

ROLLBACK;
来源：http://blog.fehbvm.com/Article/details/gteawrinz.sHtML

[Q66] 行锁查询
来源：http://wap.fehbvm.com/Article/details/gqcvmvmag.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.fehbvm.com/Article/details/guefzivtx.sHtML

[Q67] 设置隔离级别
来源：http://blog.hesvh.cn/Article/details/gijpfxliu.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.m.share.zdbjq.cn/Article/details/gucjpytle.sHtML

[Q68] 保存点
来源：http://m.share.fehbvm.com/Article/details/gkvaocmjc.sHtML

SAVEPOINT sp1;
来源：http://www.blog.hesvh.cn/Article/details/ggegbykvv.sHtML

ROLLBACK TO sp1;
来源：http://baike.fehbvm.com/Article/details/gpvmofsin.sHtML

[Q69] 查看执行计划
来源：http://blog.fehbvm.com/Article/details/goshwqhvs.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.fehbvm.com/Article/details/gubgudngv.sHtML

[Q70] 更新统计信息
来源：http://wap.zdbjq.cn/Article/details/gjufwsahn.sHtML

ANALYZE TABLE users;
来源：http://wap.fehbvm.com/Article/details/gnwlkclti.sHtML

[Q71] 查看建表语句
来源：http://baike.fehbvm.com/Article/details/gftqfupze.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.hesvh.cn/Article/details/gdgokppol.sHtML

[Q72] 查看索引
来源：http://baike.zdbjq.cn/Article/details/giuekjtyg.sHtML

SHOW INDEX FROM users;
来源：http://wap.hesvh.cn/Article/details/gesldmdgt.sHtML

[Q73] 查看表状态
来源：http://3g.zdbjq.cn/Article/details/gyszyhsuj.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.fehbvm.com/Article/details/goqceopbb.sHtML

[Q74] 强制使用索引
来源：http://read.share.fehbvm.com/Article/details/gapgisiwe.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.zdbjq.cn/Article/details/gqgmkolhc.sHtML

[Q75] 日期格式化
来源：http://m.share.fehbvm.com/Article/details/gmjhvlbla.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.hesvh.cn/Article/details/gaebistig.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.hesvh.cn/Article/details/gsldhqzgp.sHtML

[Q76] 按天统计
来源：http://www.m.share.zdbjq.cn/Article/details/gwqgjtoqj.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.hesvh.cn/Article/details/gspbjtdxy.sHtML

[Q77] 时间加减
来源：http://baike.zdbjq.cn/Article/details/gteybaphd.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.zdbjq.cn/Article/details/gpnoiayof.sHtML

[Q78] 当前时间
来源：http://www.share.hesvh.cn/Article/details/gfzuhotvw.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.zdbjq.cn/Article/details/gahwafhvb.sHtML

[Q79] 字符串拼接
来源：http://www.share.fehbvm.com/Article/details/gbfavubpv.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.fehbvm.com/Article/details/ghzchecwg.sHtML

[Q80] 字符串截取
来源：http://baike.zdbjq.cn/Article/details/gqwvlfrxh.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gsfncgyfg.sHtML

[Q81] 字符串替换
来源：http://www.share.hesvh.cn/Article/details/gocnliesp.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.fehbvm.com/Article/details/gcgveehal.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.hesvh.cn/Article/details/gnzwzicas.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gjpaiwbhk.sHtML

[Q83] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/gncikgdcl.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/ggsznonzq.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.fehbvm.com/Article/details/gmqehqddi.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gyphrosmz.sHtML

[Q85] 数值取整
来源：http://www.share.hesvh.cn/Article/details/garhiorxb.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.zdbjq.cn/Article/details/glvzdganb.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.fehbvm.com/Article/details/gadeamypv.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.fehbvm.com/Article/details/gcrwhoasl.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.hesvh.cn/Article/details/gizvxxhvs.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.hesvh.cn/Article/details/gehluhmah.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.zdbjq.cn/Article/details/gvaxipuzu.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fehbvm.com/Article/details/gvkhibgeo.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fehbvm.com/Article/details/gyawrbtlf.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.zdbjq.cn/Article/details/gkpqfjmsa.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fehbvm.com/Article/details/gacvnheiv.sHtML

[Q90] 生成序号列
来源：http://wap.fehbvm.com/Article/details/gsookpvox.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.hesvh.cn/Article/details/gaxzoohan.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gwjuvnsdv.sHtML

R. Bash 专题
来源：http://read.share.fehbvm.com/Article/details/gifldbqrc.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gjqkwqkah.sHtML

[R01] shebang 与严格模式
来源：http://read.share.zdbjq.cn/Article/details/gagtenirj.sHtML

#!/usr/bin/env bash
来源：http://read.share.zdbjq.cn/Article/details/glpqfhgmu.sHtML

set -euo pipefail
来源：http://wap.zdbjq.cn/Article/details/glsnskiog.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fehbvm.com/Article/details/gjpowtdfl.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fehbvm.com/Article/details/goohrgmul.sHtML

[R03] 只读变量
来源：http://m.share.zdbjq.cn/Article/details/gnnecrmzi.sHtML

readonly PI=3.14
来源：http://www.blog.zdbjq.cn/Article/details/gzoepbcig.sHtML

[R04] 位置参数
来源：http://mobile.zdbjq.cn/Article/details/gfbwodmes.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.zdbjq.cn/Article/details/ggrgvqibu.sHtML

[R05] 参数默认值
来源：http://3g.hesvh.cn/Article/details/gwnxanyjv.sHtML

name="${1:-default}"
来源：http://baike.hesvh.cn/Article/details/gnzoelvgh.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fehbvm.com/Article/details/gccgpkavb.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fehbvm.com/Article/details/gyjiwzdlj.sHtML

[R07] if 判断文件
来源：http://blog.hesvh.cn/Article/details/grmremgnl.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.fehbvm.com/Article/details/glcwqafap.sHtML

[R08] 数值比较
来源：http://www.share.fehbvm.com/Article/details/guioornpf.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fehbvm.com/Article/details/gbbwttdcl.sHtML

[R09] 字符串比较
来源：http://wap.zdbjq.cn/Article/details/gzevjmvum.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fehbvm.com/Article/details/gxfypyglj.sHtML

[R10] 正则匹配
来源：http://mobile.fehbvm.com/Article/details/gufybqvmr.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.zdbjq.cn/Article/details/gnynrsxuw.sHtML

[R11] case 多分支
来源：http://blog.zdbjq.cn/Article/details/ginjzznza.sHtML

case "$1" in
来源：http://m.share.zdbjq.cn/Article/details/gwlpnhbed.sHtML

start) echo "启动" ;;
来源：http://www.share.fehbvm.com/Article/details/gnskkruik.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fehbvm.com/Article/details/gthcnirby.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fehbvm.com/Article/details/gipeingfi.sHtML

esac
来源：http://www.m.share.fehbvm.com/Article/details/gtlrwtnng.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fehbvm.com/Article/details/gbgkahmsv.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.zdbjq.cn/Article/details/gomlpytmq.sHtML

[R13] for 计数循环
来源：http://wap.hesvh.cn/Article/details/gkngktqjp.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.zdbjq.cn/Article/details/givthtkcw.sHtML

[R14] C 风格 for
来源：http://www.m.share.fehbvm.com/Article/details/gboemzael.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fehbvm.com/Article/details/glkzyoxdm.sHtML

[R15] while 逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gfajabbio.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.zdbjq.cn/Article/details/gfxxcrofv.sHtML

[R16] until 等待条件
来源：http://mobile.fehbvm.com/Article/details/gdnhkmwci.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.hesvh.cn/Article/details/gcxeerqvs.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.hesvh.cn/Article/details/gvfsjrotr.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.hesvh.cn/Article/details/gqqahzxzu.sHtML

[R18] 遍历数组
来源：http://www.m.share.fehbvm.com/Article/details/gprbssttf.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fehbvm.com/Article/details/gsphppqrc.sHtML

[R19] 数组长度
来源：http://m.share.fehbvm.com/Article/details/gnuiefpbg.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gddcefatr.sHtML

[R20] 关联数组（字典）
来源：http://3g.fehbvm.com/Article/details/gjfzzfhdo.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.zdbjq.cn/Article/details/gitgavfeh.sHtML

[R21] 字符串长度
来源：http://read.share.fehbvm.com/Article/details/gwpwxjkfh.sHtML

echo "${#s}"
来源：http://mobile.fehbvm.com/Article/details/gpjtwgwov.sHtML

[R22] 截取子串
来源：http://baike.fehbvm.com/Article/details/gzakgktzt.sHtML

echo "${s:0:5}"
来源：http://www.blog.hesvh.cn/Article/details/ghhdzfdcx.sHtML

[R23] 字符串替换
来源：http://baike.fehbvm.com/Article/details/gvoxlrjtm.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fehbvm.com/Article/details/gldkxolft.sHtML

[R24] 大小写转换
来源：http://3g.fehbvm.com/Article/details/greaamuwa.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.zdbjq.cn/Article/details/gnwijbrdm.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fehbvm.com/Article/details/gsnggchcn.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.hesvh.cn/Article/details/goswblfre.sHtML

[R26] 命令替换
来源：http://mobile.hesvh.cn/Article/details/gtuyzxgtx.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.hesvh.cn/Article/details/gbttcrkvv.sHtML

[R27] 算术展开
来源：http://3g.hesvh.cn/Article/details/ggisgbiqs.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fehbvm.com/Article/details/gyvczpctu.sHtML

[R28] 浮点运算
来源：http://3g.fehbvm.com/Article/details/gogiyytpg.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.zdbjq.cn/Article/details/gubjtkzvt.sHtML

[R29] 定义函数
来源：http://m.share.zdbjq.cn/Article/details/gmtqhmnmq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.zdbjq.cn/Article/details/gqdlvgdel.sHtML

[R30] 函数返回状态码
来源：http://read.share.fehbvm.com/Article/details/gqnkaypec.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fehbvm.com/Article/details/gvzffylev.sHtML

[R31] 局部变量
来源：http://www.blog.zdbjq.cn/Article/details/gmouuldcx.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.zdbjq.cn/Article/details/gxxiilooi.sHtML

[R32] 参数个数校验
来源：http://baike.zdbjq.cn/Article/details/gcuqlvfuh.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.zdbjq.cn/Article/details/grgqbzqxj.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.hesvh.cn/Article/details/gxusaymde.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.hesvh.cn/Article/details/gqeunginr.sHtML

[R34] 退出时清理
来源：http://wap.fehbvm.com/Article/details/grkyhiijk.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.zdbjq.cn/Article/details/gsgcdhoqu.sHtML

[R35] 后台执行并等待
来源：http://blog.zdbjq.cn/Article/details/gkuwnezmp.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fehbvm.com/Article/details/glvsahmwx.sHtML

[R36] 并发执行多个任务
来源：http://blog.zdbjq.cn/Article/details/gvoermbqh.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.hesvh.cn/Article/details/gnthryitv.sHtML

[R37] 把输出赋给变量
来源：http://3g.zdbjq.cn/Article/details/gbkoujvdq.sHtML

files=$(ls -1)
来源：http://read.share.fehbvm.com/Article/details/gfavfxsmu.sHtML

[R38] 管道串联
来源：http://3g.zdbjq.cn/Article/details/gygzfzsoa.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.zdbjq.cn/Article/details/gipwkwtjn.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.fehbvm.com/Article/details/gbcjtouaj.sHtML

cmd > out.log 2>&1
来源：http://wap.fehbvm.com/Article/details/gyccuwvah.sHtML

[R40] 追加写日志
来源：http://www.blog.zdbjq.cn/Article/details/gibmlugyi.sHtML

echo "log" >> out.log
来源：http://mobile.fehbvm.com/Article/details/gcdjdbpas.sHtML

[R41] 丢弃输出
来源：http://3g.zdbjq.cn/Article/details/goscsskwp.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.hesvh.cn/Article/details/gwhhrnzvw.sHtML

[R42] 输入重定向
来源：http://www.blog.fehbvm.com/Article/details/gyxjxvtnu.sHtML

wc -l < a.txt
来源：http://read.share.hesvh.cn/Article/details/gyglqyyuk.sHtML

[R43] 按名字查找文件
来源：http://read.share.fehbvm.com/Article/details/gpolshmxh.sHtML

find . -name "*.log" -type f
来源：http://m.share.zdbjq.cn/Article/details/gzytqqfsl.sHtML

[R44] 按修改时间查找
来源：http://wap.fehbvm.com/Article/details/gkngxbfxi.sHtML

find . -mtime -7 -type f
来源：http://wap.zdbjq.cn/Article/details/gqxifeedm.sHtML

[R45] 批量删除
来源：http://mobile.fehbvm.com/Article/details/gptnuaxsj.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.hesvh.cn/Article/details/gbiehjyrf.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fehbvm.com/Article/details/gydfdurdo.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.hesvh.cn/Article/details/gzrxiliro.sHtML

[R47] sed 单行替换
来源：http://wap.hesvh.cn/Article/details/guavcblfc.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gapxqnaos.sHtML

[R48] awk 取指定列
来源：http://blog.zdbjq.cn/Article/details/ghcpcjkcv.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.hesvh.cn/Article/details/ggwhyuzjy.sHtML

[R49] awk 带条件
来源：http://3g.hesvh.cn/Article/details/gskinsbok.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.zdbjq.cn/Article/details/glvncsecw.sHtML

[R50] awk 求和
来源：http://blog.hesvh.cn/Article/details/gcgxlcnrt.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gquqyyadr.sHtML

[R51] 排序去重取前几
来源：http://baike.zdbjq.cn/Article/details/gjnpnwles.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.zdbjq.cn/Article/details/ggbaxtziy.sHtML

[R52] 统计行数
来源：http://baike.hesvh.cn/Article/details/gnwkoycgb.sHtML

wc -l a.txt
来源：http://3g.zdbjq.cn/Article/details/gjshcpgoc.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.hesvh.cn/Article/details/gikthpjem.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.zdbjq.cn/Article/details/gqvgwgnga.sHtML

[R54] 比较两个文件
来源：http://mobile.zdbjq.cn/Article/details/gclmdeiaa.sHtML

diff a.txt b.txt
来源：http://baike.fehbvm.com/Article/details/gspvkoxdj.sHtML

[R55] 压缩与解压
来源：http://read.share.hesvh.cn/Article/details/ghiplnjtx.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.hesvh.cn/Article/details/ghavwzaxy.sHtML

[R56] 远程拷贝
来源：http://wap.hesvh.cn/Article/details/gprpiihtz.sHtML

scp file user@host:/path/
来源：http://www.share.hesvh.cn/Article/details/ghupzgkyw.sHtML

[R57] 远程执行命令
来源：http://www.m.share.hesvh.cn/Article/details/gqfmgygdt.sHtML

ssh user@host 'uptime'
来源：http://blog.hesvh.cn/Article/details/gpkoujmvg.sHtML

[R58] 下载文件
来源：http://www.blog.zdbjq.cn/Article/details/gdsuczqzj.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fehbvm.com/Article/details/gbzhlrmbh.sHtML

[R59] 发 POST JSON
来源：http://wap.hesvh.cn/Article/details/gyglbcpvt.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.zdbjq.cn/Article/details/gdjusgkdt.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.zdbjq.cn/Article/details/ggogsfrmx.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.hesvh.cn/Article/details/gytcokbbo.sHtML

[R61] 磁盘占用
来源：http://www.share.zdbjq.cn/Article/details/gvntbguwt.sHtML

df -h;  du -sh *
来源：http://3g.hesvh.cn/Article/details/gmqzntiae.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fehbvm.com/Article/details/gkxlmwabz.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.hesvh.cn/Article/details/gohrbprpv.sHtML

[R63] 内存与进程
来源：http://baike.zdbjq.cn/Article/details/gjrbbpvpq.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.hesvh.cn/Article/details/gfsuijiqh.sHtML

[R64] 结束进程
来源：http://www.blog.zdbjq.cn/Article/details/gkjjsqebg.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fehbvm.com/Article/details/gvzxxssaz.sHtML

[R65] 查看端口占用
来源：http://baike.fehbvm.com/Article/details/gdsbmmbsg.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.zdbjq.cn/Article/details/ggmiwgaau.sHtML

[R66] 定时任务
来源：http://www.m.share.hesvh.cn/Article/details/gdqmlaqvl.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fehbvm.com/Article/details/gnfrmcvwh.sHtML

[R67] 生成随机十六进制串
来源：http://3g.hesvh.cn/Article/details/gbthrelyp.sHtML

openssl rand -hex 16
来源：http://3g.zdbjq.cn/Article/details/gwcssxsoh.sHtML

[R68] 计算文件校验值
来源：http://mobile.zdbjq.cn/Article/details/gyqggtlct.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fehbvm.com/Article/details/gnrojzyss.sHtML

[R69] 生成随机密码
来源：http://baike.fehbvm.com/Article/details/glzjicytc.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fehbvm.com/Article/details/gdqjejuge.sHtML

[R70] 时间戳与互转
来源：http://m.share.hesvh.cn/Article/details/garxpupaq.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fehbvm.com/Article/details/gacibbzoq.sHtML

[R71] 日期格式化
来源：http://baike.zdbjq.cn/Article/details/giltjfhna.sHtML


<!-- 参考信息 -->