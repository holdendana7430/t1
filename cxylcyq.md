代发 wailian999

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/giysnvyjn.sHtML

[Q28] 求和与平均
来源：http://3g.fanxiaobao.xyz/Article/details/gymhccaxr.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwzoalkln.sHtML

[Q29] 最大最小值
来源：http://blog.fanxiaobao.xyz/Article/details/gawwkberx.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/ghvgxyhyw.sHtML

[Q30] 分组统计
来源：http://read.share.fanxiaobao.xyz/Article/details/gbhfpdtpc.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkhofucqr.sHtML

[Q31] 分组后过滤
来源：http://wap.fanxiaobao.xyz/Article/details/giuzmusjb.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gofllzgoz.sHtML

[Q32] 分组拼接字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gjjnbmahs.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpzadxsxo.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gazurskev.sHtML

[Q33] 多列分组
来源：http://mobile.fanxiaobao.xyz/Article/details/giegudkfo.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.fanxiaobao.xyz/Article/details/ginzziyop.sHtML

[Q34] 每组取第一条
来源：http://www.share.fanxiaobao.xyz/Article/details/gbsxobjji.sHtML

SELECT * FROM (
来源：http://m.share.fanxiaobao.xyz/Article/details/gltlolttq.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.fanxiaobao.xyz/Article/details/gsqpruwyc.sHtML

) t WHERE rn = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggwvqnpkp.sHtML

[Q35] 内连接
来源：http://baike.fanxiaobao.xyz/Article/details/gbklaqvxx.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghyhorcvr.sHtML

[Q36] 左连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gtnotuyvc.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzxdqkjzh.sHtML

[Q37] 右连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grbdotbzs.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gakclfllw.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.fanxiaobao.xyz/Article/details/gunvjhqze.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.fanxiaobao.xyz/Article/details/grufatdcf.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.fanxiaobao.xyz/Article/details/gmzzwezug.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.fanxiaobao.xyz/Article/details/gckjmhxtp.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjniqvuyi.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdfnszsjd.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtufeusff.sHtML

[Q41] 多表连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggvzkanad.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.fanxiaobao.xyz/Article/details/gstntvutj.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.fanxiaobao.xyz/Article/details/gnqsawxuc.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjfquijvo.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gtziaumaw.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.fanxiaobao.xyz/Article/details/glrlqkujw.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gihqvkppg.sHtML

[Q43] 标量子查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghgmcaxld.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.fanxiaobao.xyz/Article/details/gtuwoudkx.sHtML

[Q44] IN 子查询
来源：http://www.share.fanxiaobao.xyz/Article/details/giniuptro.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.fanxiaobao.xyz/Article/details/ggftbauum.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/glfvrhpoe.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fanxiaobao.xyz/Article/details/gzhhmowxg.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.fanxiaobao.xyz/Article/details/gieknhdnq.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fanxiaobao.xyz/Article/details/gaatnohou.sHtML

[Q47] 与平均值比较
来源：http://mobile.fanxiaobao.xyz/Article/details/guqunsivh.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gamuxiafk.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gdgxwtkqs.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxjkxtcay.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/gncrkmech.sHtML

[Q49] 更新单行
来源：http://wap.fanxiaobao.xyz/Article/details/ghzsefrid.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gdoeojngk.sHtML

[Q50] 批量更新
来源：http://m.share.fanxiaobao.xyz/Article/details/gniyovvym.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaxolnvot.sHtML

[Q51] 用子查询更新
来源：http://m.share.fanxiaobao.xyz/Article/details/gwptabmxw.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gsuxxdrie.sHtML

[Q52] 删除指定行
来源：http://www.share.fanxiaobao.xyz/Article/details/gpyytjzcr.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvspnhyfg.sHtML

[Q53] 按条件删除
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxepdjwdc.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.fanxiaobao.xyz/Article/details/gkfldoyta.sHtML

[Q54] 清空表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gakmevrfh.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqvvbxzxv.sHtML

[Q55] 排名（并列占位）
来源：http://blog.fanxiaobao.xyz/Article/details/gxymxitov.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmebnfwlw.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.fanxiaobao.xyz/Article/details/gxbsogcqz.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.fanxiaobao.xyz/Article/details/gnptfeyvk.sHtML

[Q57] 行号
来源：http://wap.fanxiaobao.xyz/Article/details/grhkmdljk.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gavppqfya.sHtML

[Q58] 累计求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzvsrhblu.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gosgbgcwd.sHtML

[Q59] 分组内累计
来源：http://blog.fanxiaobao.xyz/Article/details/gcpdxevyd.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjuecjxla.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.fanxiaobao.xyz/Article/details/gjeehvxxy.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.fanxiaobao.xyz/Article/details/gachdhsgo.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/giksdlkrl.sHtML

[Q61] 移动平均
来源：http://wap.fanxiaobao.xyz/Article/details/grvoshiuw.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbmsxzasx.sHtML

[Q62] 分组占比
来源：http://3g.fanxiaobao.xyz/Article/details/gnnkaafen.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.fanxiaobao.xyz/Article/details/gvzityrez.sHtML

[Q63] 开启事务
来源：http://3g.fanxiaobao.xyz/Article/details/grdvtyyww.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.fanxiaobao.xyz/Article/details/gmiathytq.sHtML

[Q64] 提交事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gwowsgydg.sHtML

COMMIT;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbelwgxhm.sHtML

[Q65] 回滚事务
来源：http://baike.fanxiaobao.xyz/Article/details/gxklzoskj.sHtML

ROLLBACK;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwapfrwog.sHtML

[Q66] 行锁查询
来源：http://blog.fanxiaobao.xyz/Article/details/gvkubcrkn.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.fanxiaobao.xyz/Article/details/gktnfyfja.sHtML

[Q67] 设置隔离级别
来源：http://3g.fanxiaobao.xyz/Article/details/gwgydxzek.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.fanxiaobao.xyz/Article/details/gykocbkvx.sHtML

[Q68] 保存点
来源：http://read.share.fanxiaobao.xyz/Article/details/gqhftfrlg.sHtML

SAVEPOINT sp1;
来源：http://m.share.fanxiaobao.xyz/Article/details/glmvxykdm.sHtML

ROLLBACK TO sp1;
来源：http://3g.fanxiaobao.xyz/Article/details/giyqpodrc.sHtML

[Q69] 查看执行计划
来源：http://blog.fanxiaobao.xyz/Article/details/glpwpchri.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.fanxiaobao.xyz/Article/details/gortwbuoh.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnvsxdyez.sHtML

ANALYZE TABLE users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gqxsuhpdt.sHtML

[Q71] 查看建表语句
来源：http://m.share.fanxiaobao.xyz/Article/details/gmqojigja.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.fanxiaobao.xyz/Article/details/gzlnedmwz.sHtML

[Q72] 查看索引
来源：http://m.share.fanxiaobao.xyz/Article/details/gywwafrzf.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gssjyczzb.sHtML

[Q73] 查看表状态
来源：http://wap.fanxiaobao.xyz/Article/details/gkiexmicm.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.share.fanxiaobao.xyz/Article/details/gugqynmjq.sHtML

[Q74] 强制使用索引
来源：http://read.share.fanxiaobao.xyz/Article/details/gaqlbwleu.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.fanxiaobao.xyz/Article/details/glsaeqqcu.sHtML

[Q75] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gyajibilc.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/glriegxew.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.fanxiaobao.xyz/Article/details/gakahqzfg.sHtML

[Q76] 按天统计
来源：http://3g.fanxiaobao.xyz/Article/details/gbidxqiip.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.fanxiaobao.xyz/Article/details/gsxoonplv.sHtML

[Q77] 时间加减
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxmowklug.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.fanxiaobao.xyz/Article/details/gawchztiy.sHtML

[Q78] 当前时间
来源：http://baike.fanxiaobao.xyz/Article/details/gjfulzlwz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.fanxiaobao.xyz/Article/details/gkfqftsrg.sHtML

[Q79] 字符串拼接
来源：http://wap.fanxiaobao.xyz/Article/details/gtizaiymj.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.fanxiaobao.xyz/Article/details/gzyasxfyg.sHtML

[Q80] 字符串截取
来源：http://wap.fanxiaobao.xyz/Article/details/gvtuvdndi.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/glqwxjluo.sHtML

[Q81] 字符串替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gxqbupmie.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/geolnkaul.sHtML

[Q82] 字符长度与字节长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gvmmmmsvj.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gusfwuskc.sHtML

[Q83] 大小写转换
来源：http://baike.fanxiaobao.xyz/Article/details/ghewjmfbm.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkjvphzcc.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fanxiaobao.xyz/Article/details/girzxlzwl.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfladsfoz.sHtML

[Q85] 数值取整
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gckkhrlbf.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.fanxiaobao.xyz/Article/details/gobjsjefk.sHtML

[Q86] 读取 JSON 字段
来源：http://m.share.fanxiaobao.xyz/Article/details/gicdtxpzy.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fanxiaobao.xyz/Article/details/ghqbisdgh.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fanxiaobao.xyz/Article/details/glzzusfhd.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpqxrhjzn.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.fanxiaobao.xyz/Article/details/gwjasdfpp.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.fanxiaobao.xyz/Article/details/gpsobsjms.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gyxydfskc.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtzpqpmzb.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.fanxiaobao.xyz/Article/details/gxxebisxu.sHtML

[Q90] 生成序号列
来源：http://m.share.fanxiaobao.xyz/Article/details/gkuiqemvt.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.fanxiaobao.xyz/Article/details/gmavjfhwd.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gpgoyrsux.sHtML

R. Bash 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/geszurqjt.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxylurums.sHtML

[R01] shebang 与严格模式
来源：http://blog.fanxiaobao.xyz/Article/details/gzxsbtfrp.sHtML

#!/usr/bin/env bash
来源：http://baike.fanxiaobao.xyz/Article/details/gyprvygdd.sHtML

set -euo pipefail
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnupcbwsd.sHtML

[R02] 变量赋值与使用
来源：http://wap.fanxiaobao.xyz/Article/details/gqjymeicq.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gabmsltur.sHtML

[R03] 只读变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzsnuiqno.sHtML

readonly PI=3.14
来源：http://wap.fanxiaobao.xyz/Article/details/gtrmkjaug.sHtML

[R04] 位置参数
来源：http://baike.fanxiaobao.xyz/Article/details/gulbomumj.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fanxiaobao.xyz/Article/details/ghuhlfroz.sHtML

[R05] 参数默认值
来源：http://baike.fanxiaobao.xyz/Article/details/ggmrjbxij.sHtML

name="${1:-default}"
来源：http://wap.fanxiaobao.xyz/Article/details/gvvynuzkt.sHtML

[R06] 判断命令是否存在
来源：http://m.share.fanxiaobao.xyz/Article/details/gelqfursl.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnnnwruyo.sHtML

[R07] if 判断文件
来源：http://baike.fanxiaobao.xyz/Article/details/gpwlsewko.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/ghmxjazid.sHtML

[R08] 数值比较
来源：http://blog.fanxiaobao.xyz/Article/details/ggiecglpp.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqiihqhvn.sHtML

[R09] 字符串比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gohesjoly.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gyqiqmomu.sHtML

[R10] 正则匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gullileil.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmcgasxko.sHtML

[R11] case 多分支
来源：http://blog.fanxiaobao.xyz/Article/details/grepzxasm.sHtML

case "$1" in
来源：http://mobile.fanxiaobao.xyz/Article/details/gniidwnlf.sHtML

start) echo "启动" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqwugurrc.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gppborvlx.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbviaduwx.sHtML

esac
来源：http://mobile.fanxiaobao.xyz/Article/details/gyxpppjbj.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnsysabvi.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gebntwnhw.sHtML

[R13] for 计数循环
来源：http://3g.fanxiaobao.xyz/Article/details/ggpuvelnz.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gkdlvatrd.sHtML

[R14] C 风格 for
来源：http://wap.fanxiaobao.xyz/Article/details/gdmiceddo.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gxvjrxxqo.sHtML

[R15] while 逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gsbslcocs.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gxdmqtgyw.sHtML

[R16] until 等待条件
来源：http://wap.fanxiaobao.xyz/Article/details/gjjudnfxt.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gfgdoymri.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glcwvmzjx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gtilbwnyl.sHtML

[R18] 遍历数组
来源：http://blog.fanxiaobao.xyz/Article/details/goljytfjx.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gnmbcspmc.sHtML

[R19] 数组长度
来源：http://mobile.fanxiaobao.xyz/Article/details/ggsyzgvyg.sHtML

echo "${#arr[@]}"
来源：http://blog.fanxiaobao.xyz/Article/details/glarvyghx.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fanxiaobao.xyz/Article/details/grzmfhtdq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfxtbuxca.sHtML

[R21] 字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/gzeqwaldl.sHtML

echo "${#s}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gimxwfkzp.sHtML

[R22] 截取子串
来源：http://m.share.fanxiaobao.xyz/Article/details/gqdmyjqfm.sHtML

echo "${s:0:5}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxhwycyfg.sHtML

[R23] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyoxrhzli.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fanxiaobao.xyz/Article/details/gwbljaabb.sHtML

[R24] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gsaubcfta.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gnvtyvptz.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fanxiaobao.xyz/Article/details/gpbxyxrox.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.fanxiaobao.xyz/Article/details/gfybrhvxr.sHtML

[R26] 命令替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gegmzxxel.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfkkamtes.sHtML

[R27] 算术展开
来源：http://3g.fanxiaobao.xyz/Article/details/geyfsznix.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fanxiaobao.xyz/Article/details/ggiphblds.sHtML

[R28] 浮点运算
来源：http://www.share.fanxiaobao.xyz/Article/details/gmisztzzz.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fanxiaobao.xyz/Article/details/gxzdmwxnm.sHtML

[R29] 定义函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaviyityu.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gysbtgcjj.sHtML

[R30] 函数返回状态码
来源：http://blog.fanxiaobao.xyz/Article/details/gxjyevgel.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giqpwjipm.sHtML

[R31] 局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnmvatiph.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fanxiaobao.xyz/Article/details/grokbtrul.sHtML

[R32] 参数个数校验
来源：http://wap.fanxiaobao.xyz/Article/details/gsdbosrhl.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gatkwblig.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fanxiaobao.xyz/Article/details/gnvfjrrtn.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.fanxiaobao.xyz/Article/details/gmonyrcdt.sHtML

[R34] 退出时清理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gemlogtfl.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gmexionhf.sHtML

[R35] 后台执行并等待
来源：http://3g.fanxiaobao.xyz/Article/details/gfhhxynrz.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fanxiaobao.xyz/Article/details/gvclntspl.sHtML

[R36] 并发执行多个任务
来源：http://wap.fanxiaobao.xyz/Article/details/ghvdnjpzv.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fanxiaobao.xyz/Article/details/gtowyddod.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvlzltqpc.sHtML

files=$(ls -1)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqgjckcin.sHtML

[R38] 管道串联
来源：http://read.share.fanxiaobao.xyz/Article/details/gwliaewus.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fanxiaobao.xyz/Article/details/groenvfva.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcgwzfozi.sHtML

cmd > out.log 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gjwykwfgz.sHtML

[R40] 追加写日志
来源：http://blog.fanxiaobao.xyz/Article/details/gkshlgkxj.sHtML

echo "log" >> out.log
来源：http://m.share.fanxiaobao.xyz/Article/details/glqffrlrv.sHtML

[R41] 丢弃输出
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxciofmep.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gswvxmiqh.sHtML

[R42] 输入重定向
来源：http://m.share.fanxiaobao.xyz/Article/details/gucbqqfks.sHtML

wc -l < a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gqyrwqikq.sHtML

[R43] 按名字查找文件
来源：http://baike.fanxiaobao.xyz/Article/details/ggyzqbomr.sHtML

find . -name "*.log" -type f
来源：http://blog.fanxiaobao.xyz/Article/details/grmhqussg.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwwwmmfxq.sHtML

find . -mtime -7 -type f
来源：http://wap.fanxiaobao.xyz/Article/details/gsanwpxdu.sHtML

[R45] 批量删除
来源：http://3g.fanxiaobao.xyz/Article/details/gvaxpamys.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvlbrwqhx.sHtML

[R46] 递归替换文件内容
来源：http://baike.fanxiaobao.xyz/Article/details/gzdcxlvoi.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gklpddqzk.sHtML

[R47] sed 单行替换
来源：http://blog.fanxiaobao.xyz/Article/details/gvavephvu.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gemzvbuef.sHtML

[R48] awk 取指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/gsenrzpys.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gbrpwpryh.sHtML

[R49] awk 带条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gmdopomex.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.fanxiaobao.xyz/Article/details/gzzqtyvus.sHtML

[R50] awk 求和
来源：http://blog.fanxiaobao.xyz/Article/details/gmhpfzajx.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gxnjfnbra.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guqrwhrlr.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fanxiaobao.xyz/Article/details/gwiiifirk.sHtML

[R52] 统计行数
来源：http://m.share.fanxiaobao.xyz/Article/details/gjkzihrcp.sHtML

wc -l a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gzzczvoag.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fanxiaobao.xyz/Article/details/greqygias.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fanxiaobao.xyz/Article/details/gfvzfbwxt.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwhapyrwd.sHtML

diff a.txt b.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gzgslwbba.sHtML

[R55] 压缩与解压
来源：http://blog.fanxiaobao.xyz/Article/details/gevjjdkgm.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fanxiaobao.xyz/Article/details/gsbhkpxbg.sHtML

[R56] 远程拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkfzcinue.sHtML

scp file user@host:/path/
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfzybzbli.sHtML

[R57] 远程执行命令
来源：http://blog.fanxiaobao.xyz/Article/details/gpljfiftv.sHtML

ssh user@host 'uptime'
来源：http://3g.fanxiaobao.xyz/Article/details/grjpnuigd.sHtML

[R58] 下载文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gyaxmlksd.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fanxiaobao.xyz/Article/details/gibqgcbsa.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxfvnehrf.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fanxiaobao.xyz/Article/details/gxwgfrvgz.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzrnmwipp.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fanxiaobao.xyz/Article/details/gceaypkfv.sHtML

[R61] 磁盘占用
来源：http://3g.fanxiaobao.xyz/Article/details/goohrxckj.sHtML

df -h;  du -sh *
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkgddrpnl.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghwuyxehv.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fanxiaobao.xyz/Article/details/ghgfpkxnl.sHtML

[R63] 内存与进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaywwrdjw.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fanxiaobao.xyz/Article/details/gnggrkotx.sHtML

[R64] 结束进程
来源：http://3g.fanxiaobao.xyz/Article/details/gbdemxaus.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fanxiaobao.xyz/Article/details/gxgkqvrux.sHtML

[R65] 查看端口占用
来源：http://baike.fanxiaobao.xyz/Article/details/gizwfhaxq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fanxiaobao.xyz/Article/details/gphfzortd.sHtML

[R66] 定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gkplfqlss.sHtML

crontab -e;  crontab -l
来源：http://baike.fanxiaobao.xyz/Article/details/gullyfxps.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fanxiaobao.xyz/Article/details/gizntunqt.sHtML

openssl rand -hex 16
来源：http://baike.fanxiaobao.xyz/Article/details/gzjmucrui.sHtML

[R68] 计算文件校验值
来源：http://m.share.fanxiaobao.xyz/Article/details/giqbvhwav.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gugzqzqvz.sHtML

[R69] 生成随机密码
来源：http://www.share.fanxiaobao.xyz/Article/details/giuqbxrea.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fanxiaobao.xyz/Article/details/gbkjafucs.sHtML

[R70] 时间戳与互转
来源：http://www.share.fanxiaobao.xyz/Article/details/gwbestmth.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fanxiaobao.xyz/Article/details/gbjcyhgmv.sHtML

[R71] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gvjvtfzvn.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fanxiaobao.xyz/Article/details/guuiiewma.sHtML

[R72] 等待端口就绪
来源：http://baike.fanxiaobao.xyz/Article/details/gwaupgtih.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guuleixbb.sHtML

[R73] 分割大日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giesrhywk.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvsxqjurr.sHtML

[R74] 批量重命名
来源：http://www.share.fanxiaobao.xyz/Article/details/gikeorqzf.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gdfhmbqrz.sHtML

[R75] 导出环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/gbgvqwust.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fanxiaobao.xyz/Article/details/gfoequmrf.sHtML

[R76] 使用临时文件
来源：http://blog.fanxiaobao.xyz/Article/details/gmrgivdkp.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gwboxkcya.sHtML

[R77] 读取用户输入
来源：http://www.share.fanxiaobao.xyz/Article/details/grioqghos.sHtML


<!-- 参考信息 -->