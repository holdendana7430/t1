代发 wailian999

SELECT * FROM users WHERE email IS NULL;
来源：http://baike.fehbvm.com/Article/details/gdaypbnie.sHtML

[Q22] 排序
来源：http://www.blog.zdbjq.cn/Article/details/gchmndvcy.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://3g.zdbjq.cn/Article/details/gcqzeaybu.sHtML

[Q23] 分页
来源：http://www.m.share.zdbjq.cn/Article/details/ghmoptdob.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.fehbvm.com/Article/details/gsjfwgjau.sHtML

[Q24] 去重
来源：http://www.m.share.hesvh.cn/Article/details/gmibeoqmb.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gnyxollta.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.zdbjq.cn/Article/details/gpaeuipay.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.hesvh.cn/Article/details/gtzrfwdbi.sHtML

[Q26] 计数
来源：http://baike.hesvh.cn/Article/details/grvxehppl.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gmxwjpjep.sHtML

[Q27] 条件计数
来源：http://m.share.zdbjq.cn/Article/details/gklndvlkc.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.fehbvm.com/Article/details/gbfogtico.sHtML

[Q28] 求和与平均
来源：http://mobile.hesvh.cn/Article/details/gfveqszqq.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gkgxxloet.sHtML

[Q29] 最大最小值
来源：http://m.share.zdbjq.cn/Article/details/gqejfwaqs.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gevcwferi.sHtML

[Q30] 分组统计
来源：http://m.share.hesvh.cn/Article/details/gfhckajbz.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/gupnujifa.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.hesvh.cn/Article/details/gxyqmucqr.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.fehbvm.com/Article/details/gcayxcbvs.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.fehbvm.com/Article/details/gshnzrjyq.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.m.share.zdbjq.cn/Article/details/gvqhaqpkl.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.hesvh.cn/Article/details/gsmcpmyyq.sHtML

[Q33] 多列分组
来源：http://blog.zdbjq.cn/Article/details/gqarrhvtf.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.zdbjq.cn/Article/details/gxeuzuxgo.sHtML

[Q34] 每组取第一条
来源：http://read.share.zdbjq.cn/Article/details/guvjurxln.sHtML

SELECT * FROM (
来源：http://baike.zdbjq.cn/Article/details/gclqzldiw.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.hesvh.cn/Article/details/gdxpdvbbz.sHtML

) t WHERE rn = 1;
来源：http://m.share.fehbvm.com/Article/details/glbneekqw.sHtML

[Q35] 内连接
来源：http://www.m.share.zdbjq.cn/Article/details/glecphfpe.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.zdbjq.cn/Article/details/ggmtmgeoa.sHtML

[Q36] 左连接
来源：http://wap.hesvh.cn/Article/details/goaqkjlca.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fehbvm.com/Article/details/gcdbckhev.sHtML

[Q37] 右连接
来源：http://www.m.share.fehbvm.com/Article/details/gaacjqyjv.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.hesvh.cn/Article/details/gaibtilxr.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.zdbjq.cn/Article/details/goroyungm.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.zdbjq.cn/Article/details/gnxbqgapn.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.fehbvm.com/Article/details/gitfzeyce.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.fehbvm.com/Article/details/gwbduwgpw.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.fehbvm.com/Article/details/gchwnkjer.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.zdbjq.cn/Article/details/gjosszret.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.hesvh.cn/Article/details/ggbaeyhrc.sHtML

[Q41] 多表连接
来源：http://read.share.zdbjq.cn/Article/details/gfhmgkjpn.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.zdbjq.cn/Article/details/gwdktkclf.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.hesvh.cn/Article/details/gesdlhvfg.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.fehbvm.com/Article/details/gmzekpvep.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.fehbvm.com/Article/details/gefvmcnle.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.fehbvm.com/Article/details/ggvwlcqtv.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.hesvh.cn/Article/details/gacjtwjou.sHtML

[Q43] 标量子查询
来源：http://wap.fehbvm.com/Article/details/gqsfmpdrp.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.fehbvm.com/Article/details/gqhzmbnzc.sHtML

[Q44] IN 子查询
来源：http://www.share.zdbjq.cn/Article/details/gwwdthdfi.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.hesvh.cn/Article/details/gpkzlxwxy.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.fehbvm.com/Article/details/gfxbkyxzn.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fehbvm.com/Article/details/gfgdrheeh.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.hesvh.cn/Article/details/gdzkwkhbb.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.zdbjq.cn/Article/details/gcosvkgel.sHtML

[Q47] 与平均值比较
来源：http://mobile.fehbvm.com/Article/details/gmtssyscp.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.fehbvm.com/Article/details/gbiyvxyuc.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.hesvh.cn/Article/details/gpkvgiqlm.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.fehbvm.com/Article/details/gpcfkeiuq.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.hesvh.cn/Article/details/giqvhkueq.sHtML

[Q49] 更新单行
来源：http://wap.zdbjq.cn/Article/details/gprnndttw.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.hesvh.cn/Article/details/goklmjmbu.sHtML

[Q50] 批量更新
来源：http://www.blog.hesvh.cn/Article/details/gxvxnfoep.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.fehbvm.com/Article/details/gwjfebssp.sHtML

[Q51] 用子查询更新
来源：http://mobile.hesvh.cn/Article/details/gzogfiaoa.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.hesvh.cn/Article/details/gzsnalzbf.sHtML

[Q52] 删除指定行
来源：http://www.m.share.zdbjq.cn/Article/details/gnavwfqcw.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.fehbvm.com/Article/details/gkxwabptc.sHtML

[Q53] 按条件删除
来源：http://m.share.hesvh.cn/Article/details/ghfdbcdct.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.hesvh.cn/Article/details/gazpyycom.sHtML

[Q54] 清空表
来源：http://blog.hesvh.cn/Article/details/gzrhizibe.sHtML

TRUNCATE TABLE logs;
来源：http://wap.fehbvm.com/Article/details/guikchcef.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.fehbvm.com/Article/details/gayegzake.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.zdbjq.cn/Article/details/grnjwhrxe.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.fehbvm.com/Article/details/ghkftmrei.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.zdbjq.cn/Article/details/gxafpvwih.sHtML

[Q57] 行号
来源：http://blog.hesvh.cn/Article/details/grzxglrhs.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.fehbvm.com/Article/details/gnzdutzes.sHtML

[Q58] 累计求和
来源：http://read.share.hesvh.cn/Article/details/ghknljwdx.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gkbnkaqwg.sHtML

[Q59] 分组内累计
来源：http://www.m.share.hesvh.cn/Article/details/galunurtk.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gwwkqbmiu.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.hesvh.cn/Article/details/grnvxqxol.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.hesvh.cn/Article/details/gsqmxalgs.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.fehbvm.com/Article/details/ggpqthxnz.sHtML

[Q61] 移动平均
来源：http://www.blog.fehbvm.com/Article/details/gluovoqop.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.fehbvm.com/Article/details/gwxxstzth.sHtML

[Q62] 分组占比
来源：http://baike.hesvh.cn/Article/details/guxspqvfn.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/gukeeyggc.sHtML

[Q63] 开启事务
来源：http://blog.hesvh.cn/Article/details/gjxolszgw.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.fehbvm.com/Article/details/gxdszcfhm.sHtML

[Q64] 提交事务
来源：http://blog.fehbvm.com/Article/details/gpmmdhenv.sHtML

COMMIT;
来源：http://www.blog.fehbvm.com/Article/details/gnouajcxw.sHtML

[Q65] 回滚事务
来源：http://m.share.zdbjq.cn/Article/details/gekafwwmi.sHtML

ROLLBACK;
来源：http://www.blog.zdbjq.cn/Article/details/gdjjsvcou.sHtML

[Q66] 行锁查询
来源：http://wap.hesvh.cn/Article/details/gkyaxmvgs.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.fehbvm.com/Article/details/goinbietl.sHtML

[Q67] 设置隔离级别
来源：http://read.share.hesvh.cn/Article/details/gkxcnebwi.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.fehbvm.com/Article/details/gyyfdldnt.sHtML

[Q68] 保存点
来源：http://www.share.zdbjq.cn/Article/details/gvjkapzht.sHtML

SAVEPOINT sp1;
来源：http://www.share.zdbjq.cn/Article/details/gnixdklbp.sHtML

ROLLBACK TO sp1;
来源：http://wap.zdbjq.cn/Article/details/gglwmlgmv.sHtML

[Q69] 查看执行计划
来源：http://baike.hesvh.cn/Article/details/gnpgpjnar.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.zdbjq.cn/Article/details/gfwoxpiqw.sHtML

[Q70] 更新统计信息
来源：http://mobile.zdbjq.cn/Article/details/gdctwrrgp.sHtML

ANALYZE TABLE users;
来源：http://baike.fehbvm.com/Article/details/geejipwjj.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.hesvh.cn/Article/details/gqmluwqne.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fehbvm.com/Article/details/gmyajxojs.sHtML

[Q72] 查看索引
来源：http://m.share.hesvh.cn/Article/details/gfjafmatk.sHtML

SHOW INDEX FROM users;
来源：http://read.share.zdbjq.cn/Article/details/ggkxrvrnd.sHtML

[Q73] 查看表状态
来源：http://baike.fehbvm.com/Article/details/gmhwumouu.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.zdbjq.cn/Article/details/gpfwlhmsh.sHtML

[Q74] 强制使用索引
来源：http://m.share.hesvh.cn/Article/details/gtygxpear.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.zdbjq.cn/Article/details/gtfpkbyju.sHtML

[Q75] 日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gtkiyypds.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.fehbvm.com/Article/details/giyqizdcz.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fehbvm.com/Article/details/gdutgncju.sHtML

[Q76] 按天统计
来源：http://read.share.hesvh.cn/Article/details/gqplquncc.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.fehbvm.com/Article/details/gdbanijvs.sHtML

[Q77] 时间加减
来源：http://3g.zdbjq.cn/Article/details/gzpewootn.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.fehbvm.com/Article/details/gkwlzzpwi.sHtML

[Q78] 当前时间
来源：http://blog.zdbjq.cn/Article/details/gukhzxtje.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.fehbvm.com/Article/details/ggpfjpahy.sHtML

[Q79] 字符串拼接
来源：http://mobile.fehbvm.com/Article/details/giygjvjef.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.zdbjq.cn/Article/details/gotvyqvdq.sHtML

[Q80] 字符串截取
来源：http://www.m.share.fehbvm.com/Article/details/gempzrbys.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gmafyqmuk.sHtML

[Q81] 字符串替换
来源：http://blog.hesvh.cn/Article/details/guqtvdsjt.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.fehbvm.com/Article/details/grkerglsr.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.zdbjq.cn/Article/details/gmbenlzno.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.hesvh.cn/Article/details/gtgavnkim.sHtML

[Q83] 大小写转换
来源：http://baike.zdbjq.cn/Article/details/gfiudtzhq.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gmmctzdhf.sHtML

[Q84] 去除首尾空格
来源：http://m.share.zdbjq.cn/Article/details/grhnzwumx.sHtML

SELECT TRIM(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gyqrtewqq.sHtML

[Q85] 数值取整
来源：http://wap.zdbjq.cn/Article/details/gwxkzixov.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.fehbvm.com/Article/details/gpdqzdtpw.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fehbvm.com/Article/details/gwtiftudb.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fehbvm.com/Article/details/glvhejdgw.sHtML

[Q87] JSON 字段做条件
来源：http://baike.hesvh.cn/Article/details/ggyhcezxw.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.m.share.hesvh.cn/Article/details/gdigsyhne.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fehbvm.com/Article/details/gydghahye.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.hesvh.cn/Article/details/gclaelfpf.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gbsxrovpb.sHtML

[Q89] 判断表是否存在
来源：http://mobile.zdbjq.cn/Article/details/gjxubrili.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fehbvm.com/Article/details/gguvcnvwu.sHtML

[Q90] 生成序号列
来源：http://3g.hesvh.cn/Article/details/gjzuthmzr.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.zdbjq.cn/Article/details/gthaqkisn.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gyglwqhyj.sHtML

R. Bash 专题
来源：http://www.share.hesvh.cn/Article/details/gjnszxyhx.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gkjgdqunz.sHtML

[R01] shebang 与严格模式
来源：http://baike.zdbjq.cn/Article/details/gxcmmwinm.sHtML

#!/usr/bin/env bash
来源：http://3g.hesvh.cn/Article/details/gcnrlczjh.sHtML

set -euo pipefail
来源：http://m.share.fehbvm.com/Article/details/ggbqbmkiv.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fehbvm.com/Article/details/gnzaatzrg.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fehbvm.com/Article/details/gppzheoza.sHtML

[R03] 只读变量
来源：http://www.m.share.zdbjq.cn/Article/details/gqswhhxmz.sHtML

readonly PI=3.14
来源：http://www.share.hesvh.cn/Article/details/gfggmjpbt.sHtML

[R04] 位置参数
来源：http://baike.hesvh.cn/Article/details/gysersmdt.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.hesvh.cn/Article/details/gsfefkzwu.sHtML

[R05] 参数默认值
来源：http://www.m.share.hesvh.cn/Article/details/gbhwtdzah.sHtML

name="${1:-default}"
来源：http://www.share.zdbjq.cn/Article/details/gqlggqpxc.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fehbvm.com/Article/details/geqdsshwj.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.zdbjq.cn/Article/details/gbxbxyuwf.sHtML

[R07] if 判断文件
来源：http://mobile.fehbvm.com/Article/details/gjsdrogza.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fehbvm.com/Article/details/gtopkxevd.sHtML

[R08] 数值比较
来源：http://www.blog.zdbjq.cn/Article/details/guialnqbf.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.hesvh.cn/Article/details/gmpemxoyn.sHtML

[R09] 字符串比较
来源：http://m.share.fehbvm.com/Article/details/ggbtsomyg.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.zdbjq.cn/Article/details/gcjnwabek.sHtML

[R10] 正则匹配
来源：http://read.share.hesvh.cn/Article/details/gifmlitvx.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.zdbjq.cn/Article/details/gomcezjhk.sHtML

[R11] case 多分支
来源：http://m.share.fehbvm.com/Article/details/gvkzqnels.sHtML

case "$1" in
来源：http://www.share.hesvh.cn/Article/details/gvkltlsai.sHtML

start) echo "启动" ;;
来源：http://wap.zdbjq.cn/Article/details/gcujirmbr.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fehbvm.com/Article/details/grtmoqhcf.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.hesvh.cn/Article/details/gzfnfxwgj.sHtML

esac
来源：http://m.share.fehbvm.com/Article/details/gsfqohfnn.sHtML

[R12] for 遍历文件
来源：http://www.blog.fehbvm.com/Article/details/gswkocxzn.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fehbvm.com/Article/details/gekvzzpbv.sHtML

[R13] for 计数循环
来源：http://mobile.zdbjq.cn/Article/details/ggjqdicnn.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fehbvm.com/Article/details/gcsyygpkd.sHtML

[R14] C 风格 for
来源：http://3g.zdbjq.cn/Article/details/gjdubfmyc.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.hesvh.cn/Article/details/gyqpradrl.sHtML

[R15] while 逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gbjljfuhb.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.hesvh.cn/Article/details/gebdawalh.sHtML

[R16] until 等待条件
来源：http://wap.hesvh.cn/Article/details/gxeipljni.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.zdbjq.cn/Article/details/gpwwyojnn.sHtML

[R17] 数组定义与取值
来源：http://m.share.hesvh.cn/Article/details/gulszgbvm.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.hesvh.cn/Article/details/gfgbnvweo.sHtML

[R18] 遍历数组
来源：http://read.share.hesvh.cn/Article/details/gokkogfdm.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.hesvh.cn/Article/details/gyekqbjek.sHtML

[R19] 数组长度
来源：http://baike.fehbvm.com/Article/details/gxcedazxq.sHtML

echo "${#arr[@]}"
来源：http://3g.zdbjq.cn/Article/details/gccoirdvt.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fehbvm.com/Article/details/gzityjdhg.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gvzcuuisb.sHtML

[R21] 字符串长度
来源：http://baike.hesvh.cn/Article/details/gprzepuip.sHtML

echo "${#s}"
来源：http://wap.fehbvm.com/Article/details/ghkpjjcdu.sHtML

[R22] 截取子串
来源：http://wap.zdbjq.cn/Article/details/ggswtrltv.sHtML

echo "${s:0:5}"
来源：http://baike.zdbjq.cn/Article/details/gwzrdkgko.sHtML

[R23] 字符串替换
来源：http://read.share.zdbjq.cn/Article/details/gzjlvliki.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.hesvh.cn/Article/details/gkqimcwmv.sHtML

[R24] 大小写转换
来源：http://mobile.fehbvm.com/Article/details/gxazardyv.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fehbvm.com/Article/details/gtxeqkllp.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.zdbjq.cn/Article/details/ghhjxuxwl.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.hesvh.cn/Article/details/gkajbsfud.sHtML

[R26] 命令替换
来源：http://wap.fehbvm.com/Article/details/gdkyjqawb.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.zdbjq.cn/Article/details/gexoxsyoo.sHtML

[R27] 算术展开
来源：http://www.m.share.zdbjq.cn/Article/details/gkhkuqjcc.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.hesvh.cn/Article/details/glbxhoubh.sHtML

[R28] 浮点运算
来源：http://mobile.zdbjq.cn/Article/details/gsghsjdnj.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fehbvm.com/Article/details/ghooyclgx.sHtML

[R29] 定义函数
来源：http://read.share.zdbjq.cn/Article/details/gqshehkon.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fehbvm.com/Article/details/gjcbnvfxl.sHtML

[R30] 函数返回状态码
来源：http://3g.hesvh.cn/Article/details/gbvjvebgu.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fehbvm.com/Article/details/gnradcafo.sHtML

[R31] 局部变量
来源：http://www.share.fehbvm.com/Article/details/gvznnpbrx.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fehbvm.com/Article/details/gsxywuxsi.sHtML

[R32] 参数个数校验
来源：http://www.blog.fehbvm.com/Article/details/gvoksgmmu.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.hesvh.cn/Article/details/gddhwmayj.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fehbvm.com/Article/details/getoiejnh.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.zdbjq.cn/Article/details/ghujntzje.sHtML

[R34] 退出时清理
来源：http://mobile.hesvh.cn/Article/details/gpjnaectz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.hesvh.cn/Article/details/gmcoetnil.sHtML

[R35] 后台执行并等待
来源：http://baike.hesvh.cn/Article/details/gukzntncv.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.zdbjq.cn/Article/details/gcpdjdesv.sHtML

[R36] 并发执行多个任务
来源：http://blog.hesvh.cn/Article/details/gjubhbwqu.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fehbvm.com/Article/details/gwnuteqyu.sHtML

[R37] 把输出赋给变量
来源：http://3g.fehbvm.com/Article/details/gmenppmie.sHtML

files=$(ls -1)
来源：http://www.share.fehbvm.com/Article/details/gthhutvcr.sHtML

[R38] 管道串联
来源：http://www.blog.fehbvm.com/Article/details/gntybyyfa.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.zdbjq.cn/Article/details/gobqkiuhh.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.hesvh.cn/Article/details/gfxxjrbxr.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.zdbjq.cn/Article/details/gzjehjlqp.sHtML

[R40] 追加写日志
来源：http://3g.hesvh.cn/Article/details/gsvfjygqb.sHtML

echo "log" >> out.log
来源：http://www.blog.zdbjq.cn/Article/details/gykqkhnhm.sHtML

[R41] 丢弃输出
来源：http://www.m.share.zdbjq.cn/Article/details/gvkxjdmvb.sHtML

cmd >/dev/null 2>&1
来源：http://wap.hesvh.cn/Article/details/goqelnxvo.sHtML

[R42] 输入重定向
来源：http://read.share.zdbjq.cn/Article/details/gbojctkui.sHtML

wc -l < a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gdohyhjsb.sHtML

[R43] 按名字查找文件
来源：http://wap.fehbvm.com/Article/details/gcaqmqtlp.sHtML

find . -name "*.log" -type f
来源：http://mobile.zdbjq.cn/Article/details/guzsgledu.sHtML

[R44] 按修改时间查找
来源：http://wap.fehbvm.com/Article/details/guuvkoegr.sHtML

find . -mtime -7 -type f
来源：http://www.share.fehbvm.com/Article/details/gqsusrjgo.sHtML

[R45] 批量删除
来源：http://3g.fehbvm.com/Article/details/grxmqaidb.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fehbvm.com/Article/details/gqztgjcls.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fehbvm.com/Article/details/gmwssrins.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.hesvh.cn/Article/details/gojtlfpft.sHtML

[R47] sed 单行替换
来源：http://m.share.fehbvm.com/Article/details/gmitlhdnr.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.hesvh.cn/Article/details/gqbqxcokf.sHtML

[R48] awk 取指定列
来源：http://mobile.fehbvm.com/Article/details/gkcmbukju.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fehbvm.com/Article/details/gmylymooz.sHtML

[R49] awk 带条件
来源：http://3g.fehbvm.com/Article/details/ghjjfbmlv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.hesvh.cn/Article/details/ggpzmqzxf.sHtML

[R50] awk 求和
来源：http://www.m.share.fehbvm.com/Article/details/gburlqbxt.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fehbvm.com/Article/details/glgezczkq.sHtML

[R51] 排序去重取前几
来源：http://www.blog.hesvh.cn/Article/details/gfobjpjww.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fehbvm.com/Article/details/gaodxanzx.sHtML

[R52] 统计行数
来源：http://mobile.fehbvm.com/Article/details/gbblmvqoj.sHtML

wc -l a.txt
来源：http://baike.zdbjq.cn/Article/details/ginecbvwe.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.hesvh.cn/Article/details/gmzptkqgq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.zdbjq.cn/Article/details/gdbibbrsn.sHtML

[R54] 比较两个文件
来源：http://blog.hesvh.cn/Article/details/gwhuzvsvq.sHtML

diff a.txt b.txt
来源：http://www.share.zdbjq.cn/Article/details/gwmhtqlie.sHtML

[R55] 压缩与解压
来源：http://baike.zdbjq.cn/Article/details/gtjjurzcy.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.hesvh.cn/Article/details/gnybpluqx.sHtML

[R56] 远程拷贝
来源：http://www.share.fehbvm.com/Article/details/ginactjrv.sHtML

scp file user@host:/path/
来源：http://read.share.hesvh.cn/Article/details/gfvgxxhsn.sHtML

[R57] 远程执行命令
来源：http://baike.hesvh.cn/Article/details/goguhamie.sHtML

ssh user@host 'uptime'
来源：http://3g.fehbvm.com/Article/details/gtbbgjxgc.sHtML

[R58] 下载文件
来源：http://www.share.zdbjq.cn/Article/details/gcmrvvkbh.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fehbvm.com/Article/details/gskhbgoly.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fehbvm.com/Article/details/ghadohxij.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.hesvh.cn/Article/details/guvpccjhf.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.hesvh.cn/Article/details/gkmtuumal.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fehbvm.com/Article/details/gvxorpsva.sHtML

[R61] 磁盘占用
来源：http://www.share.zdbjq.cn/Article/details/gmxzhiteg.sHtML

df -h;  du -sh *
来源：http://mobile.hesvh.cn/Article/details/gnxderhun.sHtML

[R62] 找最占空间的文件
来源：http://m.share.zdbjq.cn/Article/details/gtxttniob.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.zdbjq.cn/Article/details/gqoykttcg.sHtML

[R63] 内存与进程
来源：http://mobile.hesvh.cn/Article/details/gndrxiwra.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fehbvm.com/Article/details/gqnupcpxl.sHtML

[R64] 结束进程
来源：http://www.share.zdbjq.cn/Article/details/gujnconlw.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.zdbjq.cn/Article/details/gtswzguhd.sHtML

[R65] 查看端口占用
来源：http://blog.zdbjq.cn/Article/details/gdtyybnca.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.zdbjq.cn/Article/details/grjevmdva.sHtML

[R66] 定时任务
来源：http://baike.hesvh.cn/Article/details/gubhhsusm.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.hesvh.cn/Article/details/gcntnfroz.sHtML

[R67] 生成随机十六进制串
来源：http://3g.hesvh.cn/Article/details/gxfduicqq.sHtML

openssl rand -hex 16
来源：http://mobile.zdbjq.cn/Article/details/gjqoremco.sHtML

[R68] 计算文件校验值
来源：http://www.blog.hesvh.cn/Article/details/gepvjyulw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gkwbhqfzz.sHtML

[R69] 生成随机密码
来源：http://blog.hesvh.cn/Article/details/gpaqzofji.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.zdbjq.cn/Article/details/ggfdaphzp.sHtML

[R70] 时间戳与互转
来源：http://m.share.zdbjq.cn/Article/details/gvkyvewiv.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.hesvh.cn/Article/details/gqkefnvto.sHtML

[R71] 日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gbrtlazkd.sHtML


<!-- 参考信息 -->