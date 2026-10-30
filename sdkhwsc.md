代发 wailian999

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.zdbjq.cn/Article/details/gdbpofuzh.sHtML

[Q20] IN 列表
来源：http://read.share.hesvh.cn/Article/details/ggppqtemn.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.share.zdbjq.cn/Article/details/gblvdbfib.sHtML

[Q21] 空值判断
来源：http://wap.zdbjq.cn/Article/details/gkycsmmhw.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://mobile.zdbjq.cn/Article/details/gfxssahpw.sHtML

[Q22] 排序
来源：http://www.blog.hesvh.cn/Article/details/ghmkeniad.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.hesvh.cn/Article/details/ghzbowlnu.sHtML

[Q23] 分页
来源：http://read.share.hesvh.cn/Article/details/gwhhdrgfn.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.fehbvm.com/Article/details/gtylcpdwt.sHtML

[Q24] 去重
来源：http://mobile.hesvh.cn/Article/details/gujfswdwb.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.fehbvm.com/Article/details/gnmbvhesa.sHtML

[Q25] 只取前 N 条
来源：http://www.share.zdbjq.cn/Article/details/gqsoiuwbk.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.zdbjq.cn/Article/details/grmjunexf.sHtML

[Q26] 计数
来源：http://3g.fehbvm.com/Article/details/gxaanjqnq.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.hesvh.cn/Article/details/ghpgrirda.sHtML

[Q27] 条件计数
来源：http://baike.fehbvm.com/Article/details/ghsakzqcj.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.hesvh.cn/Article/details/gkzkfbgsk.sHtML

[Q28] 求和与平均
来源：http://read.share.fehbvm.com/Article/details/glhutoihp.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/ggxzzrbvd.sHtML

[Q29] 最大最小值
来源：http://www.m.share.hesvh.cn/Article/details/gtfutiran.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gxuvfvfdf.sHtML

[Q30] 分组统计
来源：http://www.m.share.zdbjq.cn/Article/details/gggvwkqro.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/gcdtniafe.sHtML

[Q31] 分组后过滤
来源：http://www.blog.hesvh.cn/Article/details/gnljqnlfs.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.fehbvm.com/Article/details/gqgiqirlh.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gkeicyvfv.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/gmdtucoth.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.zdbjq.cn/Article/details/gfftipjsy.sHtML

[Q33] 多列分组
来源：http://www.blog.zdbjq.cn/Article/details/gewypkpam.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.zdbjq.cn/Article/details/gwwbcswsu.sHtML

[Q34] 每组取第一条
来源：http://read.share.hesvh.cn/Article/details/gtejupvhj.sHtML

SELECT * FROM (
来源：http://mobile.zdbjq.cn/Article/details/gztepwndq.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.hesvh.cn/Article/details/gbpvelewn.sHtML

) t WHERE rn = 1;
来源：http://m.share.fehbvm.com/Article/details/gtjooiokx.sHtML

[Q35] 内连接
来源：http://blog.hesvh.cn/Article/details/gxeqdszgb.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.fehbvm.com/Article/details/ghlbjhiyb.sHtML

[Q36] 左连接
来源：http://www.share.hesvh.cn/Article/details/gzkzpuihg.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.zdbjq.cn/Article/details/ghegzcfdl.sHtML

[Q37] 右连接
来源：http://read.share.hesvh.cn/Article/details/gbccghclb.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.hesvh.cn/Article/details/gvjrhppoo.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.hesvh.cn/Article/details/gogtckdyg.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.fehbvm.com/Article/details/gsbprluav.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.hesvh.cn/Article/details/gfdoydoyb.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.hesvh.cn/Article/details/gpnlfhltb.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.zdbjq.cn/Article/details/gmfrnljik.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.fehbvm.com/Article/details/garkhrooh.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.fehbvm.com/Article/details/gettbiydn.sHtML

[Q41] 多表连接
来源：http://blog.zdbjq.cn/Article/details/gjkfxqmiq.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.hesvh.cn/Article/details/gwwndvfcr.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.zdbjq.cn/Article/details/gxwnmphtp.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.zdbjq.cn/Article/details/gzomhqeqj.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.zdbjq.cn/Article/details/gheffonsb.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.zdbjq.cn/Article/details/gnjgnhyix.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.hesvh.cn/Article/details/gqpypafuo.sHtML

[Q43] 标量子查询
来源：http://mobile.zdbjq.cn/Article/details/gjshiqdzf.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.zdbjq.cn/Article/details/gyrhdsstd.sHtML

[Q44] IN 子查询
来源：http://baike.fehbvm.com/Article/details/gswjcuanq.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.fehbvm.com/Article/details/gbmdtuwwo.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.fehbvm.com/Article/details/gpfwfvqqf.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fehbvm.com/Article/details/gsrolicou.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.fehbvm.com/Article/details/gairgpoxh.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.hesvh.cn/Article/details/gpeiuwtsk.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.hesvh.cn/Article/details/gjvtsfwqr.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.zdbjq.cn/Article/details/gyhtiakem.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.fehbvm.com/Article/details/gnawtpcgp.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.fehbvm.com/Article/details/gafsssvqf.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.zdbjq.cn/Article/details/gplpmvvrj.sHtML

[Q49] 更新单行
来源：http://mobile.fehbvm.com/Article/details/gddqeraus.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.fehbvm.com/Article/details/gpnhwtdqt.sHtML

[Q50] 批量更新
来源：http://baike.zdbjq.cn/Article/details/gouvutxbo.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.hesvh.cn/Article/details/gxxyezglz.sHtML

[Q51] 用子查询更新
来源：http://m.share.fehbvm.com/Article/details/gedqxeptf.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.fehbvm.com/Article/details/gdencfmlh.sHtML

[Q52] 删除指定行
来源：http://www.blog.hesvh.cn/Article/details/gpvinlaum.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.hesvh.cn/Article/details/grqiionas.sHtML

[Q53] 按条件删除
来源：http://www.m.share.fehbvm.com/Article/details/gefslqlhb.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.hesvh.cn/Article/details/gcigtqwou.sHtML

[Q54] 清空表
来源：http://read.share.zdbjq.cn/Article/details/gjvukwyhp.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.hesvh.cn/Article/details/gwetgkdks.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.hesvh.cn/Article/details/ghojhcryd.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.hesvh.cn/Article/details/gsfbhfamw.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.fehbvm.com/Article/details/gmqmstddy.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.hesvh.cn/Article/details/gfrzfpmya.sHtML

[Q57] 行号
来源：http://www.m.share.hesvh.cn/Article/details/godcznksv.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.hesvh.cn/Article/details/giggyzqoo.sHtML

[Q58] 累计求和
来源：http://wap.fehbvm.com/Article/details/gcudllktq.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.fehbvm.com/Article/details/gkyydlwxb.sHtML

[Q59] 分组内累计
来源：http://m.share.fehbvm.com/Article/details/gmqlkslfl.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gkimrottv.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.hesvh.cn/Article/details/gjqvyylzf.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fehbvm.com/Article/details/gjyeaogpa.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gmdavbick.sHtML

[Q61] 移动平均
来源：http://www.blog.zdbjq.cn/Article/details/guxfgojvm.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.hesvh.cn/Article/details/gdfjnnfxv.sHtML

[Q62] 分组占比
来源：http://blog.hesvh.cn/Article/details/gxgeudqeg.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.fehbvm.com/Article/details/guzrgpdku.sHtML

[Q63] 开启事务
来源：http://www.blog.zdbjq.cn/Article/details/gxomfwqgp.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.fehbvm.com/Article/details/gbehambxr.sHtML

[Q64] 提交事务
来源：http://mobile.zdbjq.cn/Article/details/gdgqfdcaj.sHtML

COMMIT;
来源：http://baike.fehbvm.com/Article/details/grhxmexdc.sHtML

[Q65] 回滚事务
来源：http://www.m.share.zdbjq.cn/Article/details/gkvmubxdx.sHtML

ROLLBACK;
来源：http://www.share.zdbjq.cn/Article/details/gnlldoqrf.sHtML

[Q66] 行锁查询
来源：http://m.share.hesvh.cn/Article/details/gzjjeflup.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.hesvh.cn/Article/details/gtonremju.sHtML

[Q67] 设置隔离级别
来源：http://mobile.zdbjq.cn/Article/details/gwidrtvxa.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.fehbvm.com/Article/details/gafgmhqum.sHtML

[Q68] 保存点
来源：http://m.share.fehbvm.com/Article/details/ggrnflixv.sHtML

SAVEPOINT sp1;
来源：http://blog.hesvh.cn/Article/details/gblfjmrey.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.hesvh.cn/Article/details/gicisifip.sHtML

[Q69] 查看执行计划
来源：http://m.share.zdbjq.cn/Article/details/gilnsarty.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.hesvh.cn/Article/details/glkyrknxj.sHtML

[Q70] 更新统计信息
来源：http://wap.zdbjq.cn/Article/details/ggqpbggmq.sHtML

ANALYZE TABLE users;
来源：http://wap.fehbvm.com/Article/details/gvtcwdbvg.sHtML

[Q71] 查看建表语句
来源：http://www.blog.hesvh.cn/Article/details/gvspxasmf.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.fehbvm.com/Article/details/gkkngpzxu.sHtML

[Q72] 查看索引
来源：http://blog.hesvh.cn/Article/details/gymcwzkhh.sHtML

SHOW INDEX FROM users;
来源：http://baike.fehbvm.com/Article/details/glzwenhcd.sHtML

[Q73] 查看表状态
来源：http://www.blog.fehbvm.com/Article/details/gejtvfaah.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.zdbjq.cn/Article/details/gjbiwtkht.sHtML

[Q74] 强制使用索引
来源：http://wap.zdbjq.cn/Article/details/gjogzxqwl.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.hesvh.cn/Article/details/gdpvgpcuc.sHtML

[Q75] 日期格式化
来源：http://read.share.hesvh.cn/Article/details/gyjcujhok.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.hesvh.cn/Article/details/guxreabaf.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.hesvh.cn/Article/details/gqtgieufw.sHtML

[Q76] 按天统计
来源：http://www.m.share.hesvh.cn/Article/details/gjlxtffrs.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.zdbjq.cn/Article/details/gqalakzqh.sHtML

[Q77] 时间加减
来源：http://baike.fehbvm.com/Article/details/gcedbkfye.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.hesvh.cn/Article/details/gjqbwdhyu.sHtML

[Q78] 当前时间
来源：http://mobile.fehbvm.com/Article/details/gwthiqxhf.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.zdbjq.cn/Article/details/gwbitftpk.sHtML

[Q79] 字符串拼接
来源：http://mobile.hesvh.cn/Article/details/grgbxdgwi.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.fehbvm.com/Article/details/ggeorkvoc.sHtML

[Q80] 字符串截取
来源：http://www.share.fehbvm.com/Article/details/gtzkiubec.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/glpfluebf.sHtML

[Q81] 字符串替换
来源：http://read.share.hesvh.cn/Article/details/gftjvknoj.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://blog.zdbjq.cn/Article/details/gwhfainxl.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.fehbvm.com/Article/details/gbttvraib.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gmzexzmvq.sHtML

[Q83] 大小写转换
来源：http://mobile.fehbvm.com/Article/details/gkxntlvss.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gafjhdfok.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.fehbvm.com/Article/details/gzsdgezqx.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gjikbligo.sHtML

[Q85] 数值取整
来源：http://www.share.fehbvm.com/Article/details/gswmdfioo.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.hesvh.cn/Article/details/gsoyapwmr.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.hesvh.cn/Article/details/gkkezdcid.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.zdbjq.cn/Article/details/gaflogcmh.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fehbvm.com/Article/details/gvnpztugl.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.hesvh.cn/Article/details/gnvcylkxp.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.zdbjq.cn/Article/details/gfsvazlam.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.zdbjq.cn/Article/details/gstiiztxq.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fehbvm.com/Article/details/gkyjtsjsf.sHtML

[Q89] 判断表是否存在
来源：http://m.share.zdbjq.cn/Article/details/gindhdlpq.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.zdbjq.cn/Article/details/gzvxfvkvz.sHtML

[Q90] 生成序号列
来源：http://m.share.zdbjq.cn/Article/details/glmkipcyz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.zdbjq.cn/Article/details/gudptnmce.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gcldciopq.sHtML

R. Bash 专题
来源：http://www.blog.zdbjq.cn/Article/details/gjyilpdzb.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gdsaygisl.sHtML

[R01] shebang 与严格模式
来源：http://mobile.hesvh.cn/Article/details/gmskkwkkq.sHtML

#!/usr/bin/env bash
来源：http://www.share.hesvh.cn/Article/details/gvbzyjxod.sHtML

set -euo pipefail
来源：http://m.share.hesvh.cn/Article/details/gqqjzbjxl.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.zdbjq.cn/Article/details/gjjndjjjq.sHtML

name="Tom"; echo "$name"
来源：http://3g.hesvh.cn/Article/details/gilwelpja.sHtML

[R03] 只读变量
来源：http://www.blog.hesvh.cn/Article/details/gxclqrmkq.sHtML

readonly PI=3.14
来源：http://m.share.hesvh.cn/Article/details/gzelusaow.sHtML

[R04] 位置参数
来源：http://blog.hesvh.cn/Article/details/ghzuivovd.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.hesvh.cn/Article/details/gkazvjugi.sHtML

[R05] 参数默认值
来源：http://blog.zdbjq.cn/Article/details/gkxrqjwzf.sHtML

name="${1:-default}"
来源：http://mobile.zdbjq.cn/Article/details/gjvnvmrtd.sHtML

[R06] 判断命令是否存在
来源：http://read.share.hesvh.cn/Article/details/gkhhvxwuu.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.hesvh.cn/Article/details/guvepvzfv.sHtML

[R07] if 判断文件
来源：http://m.share.hesvh.cn/Article/details/gsnsjsjkn.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.hesvh.cn/Article/details/gqriqfneu.sHtML

[R08] 数值比较
来源：http://wap.hesvh.cn/Article/details/gbpjvekxx.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.zdbjq.cn/Article/details/gccmvqurh.sHtML

[R09] 字符串比较
来源：http://wap.fehbvm.com/Article/details/ghqxadzkj.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.zdbjq.cn/Article/details/gqoxeqvoo.sHtML

[R10] 正则匹配
来源：http://3g.zdbjq.cn/Article/details/givnqnhil.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.fehbvm.com/Article/details/gbchjflxx.sHtML

[R11] case 多分支
来源：http://mobile.zdbjq.cn/Article/details/gwusqpgel.sHtML

case "$1" in
来源：http://www.m.share.hesvh.cn/Article/details/gptmlulhy.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fehbvm.com/Article/details/guniekgsr.sHtML

stop)  echo "停止" ;;
来源：http://3g.fehbvm.com/Article/details/gnizaomjw.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fehbvm.com/Article/details/glwrtmvdx.sHtML

esac
来源：http://www.m.share.hesvh.cn/Article/details/grykfrdfp.sHtML

[R12] for 遍历文件
来源：http://wap.zdbjq.cn/Article/details/gxpuudekg.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.hesvh.cn/Article/details/ggmrvoabs.sHtML

[R13] for 计数循环
来源：http://blog.fehbvm.com/Article/details/ggwnoozkq.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.hesvh.cn/Article/details/ghiwbfdsn.sHtML

[R14] C 风格 for
来源：http://wap.hesvh.cn/Article/details/grhvhmhux.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.hesvh.cn/Article/details/ggyqfbnzd.sHtML

[R15] while 逐行读文件
来源：http://3g.fehbvm.com/Article/details/gyarfdbks.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.zdbjq.cn/Article/details/gxfmaoxxf.sHtML

[R16] until 等待条件
来源：http://www.share.hesvh.cn/Article/details/gsgzjenik.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gqeevyquf.sHtML

[R17] 数组定义与取值
来源：http://baike.zdbjq.cn/Article/details/glvfzpksg.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.hesvh.cn/Article/details/glmakzgan.sHtML

[R18] 遍历数组
来源：http://www.share.hesvh.cn/Article/details/gmmxotdit.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.hesvh.cn/Article/details/ggqqtwcbz.sHtML

[R19] 数组长度
来源：http://www.m.share.hesvh.cn/Article/details/gflotvaig.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fehbvm.com/Article/details/gmuszwtbe.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fehbvm.com/Article/details/gzswtceuw.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.zdbjq.cn/Article/details/gqlyjxssn.sHtML

[R21] 字符串长度
来源：http://blog.zdbjq.cn/Article/details/gnugivcwy.sHtML

echo "${#s}"
来源：http://read.share.fehbvm.com/Article/details/gynrynnqc.sHtML

[R22] 截取子串
来源：http://blog.fehbvm.com/Article/details/gayjzzwlx.sHtML

echo "${s:0:5}"
来源：http://3g.fehbvm.com/Article/details/gzpawpvzc.sHtML

[R23] 字符串替换
来源：http://blog.zdbjq.cn/Article/details/gwbsgeaur.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fehbvm.com/Article/details/gpcercbac.sHtML

[R24] 大小写转换
来源：http://www.share.fehbvm.com/Article/details/gkfsortxe.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fehbvm.com/Article/details/gzbkqxpjm.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fehbvm.com/Article/details/gznrgcoun.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.hesvh.cn/Article/details/guwwhkbmp.sHtML

[R26] 命令替换
来源：http://3g.fehbvm.com/Article/details/goljzbwxp.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fehbvm.com/Article/details/gboxlftyc.sHtML

[R27] 算术展开
来源：http://3g.fehbvm.com/Article/details/grjjovoml.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.hesvh.cn/Article/details/guotfdnoo.sHtML

[R28] 浮点运算
来源：http://wap.fehbvm.com/Article/details/gtsnylcmn.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fehbvm.com/Article/details/gxbksxxzr.sHtML

[R29] 定义函数
来源：http://wap.hesvh.cn/Article/details/gydlvwsjj.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.zdbjq.cn/Article/details/grrulggll.sHtML

[R30] 函数返回状态码
来源：http://blog.zdbjq.cn/Article/details/ghsrjqwpo.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.hesvh.cn/Article/details/gdyatavph.sHtML

[R31] 局部变量
来源：http://mobile.zdbjq.cn/Article/details/gaqwfxznr.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.hesvh.cn/Article/details/gdtevsuey.sHtML

[R32] 参数个数校验
来源：http://m.share.fehbvm.com/Article/details/groazmfvs.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/gbigduhgq.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.zdbjq.cn/Article/details/guibtytae.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.fehbvm.com/Article/details/gbcqwutup.sHtML

[R34] 退出时清理
来源：http://mobile.zdbjq.cn/Article/details/gsleygwsb.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/gwhjmcllx.sHtML

[R35] 后台执行并等待
来源：http://read.share.zdbjq.cn/Article/details/grffupejy.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.hesvh.cn/Article/details/gwblhlsdl.sHtML

[R36] 并发执行多个任务
来源：http://baike.fehbvm.com/Article/details/geqkeujnj.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.hesvh.cn/Article/details/gnyvlmemo.sHtML

[R37] 把输出赋给变量
来源：http://baike.zdbjq.cn/Article/details/gchltpyhd.sHtML

files=$(ls -1)
来源：http://www.share.zdbjq.cn/Article/details/gvgtownft.sHtML

[R38] 管道串联
来源：http://3g.zdbjq.cn/Article/details/gciavsvet.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fehbvm.com/Article/details/goxzuzojr.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.zdbjq.cn/Article/details/gchfwlbyo.sHtML

cmd > out.log 2>&1
来源：http://m.share.hesvh.cn/Article/details/gyevfgneo.sHtML

[R40] 追加写日志
来源：http://www.blog.fehbvm.com/Article/details/grlgzabpi.sHtML

echo "log" >> out.log
来源：http://mobile.hesvh.cn/Article/details/gasugnyon.sHtML

[R41] 丢弃输出
来源：http://baike.hesvh.cn/Article/details/gxjmlhrdd.sHtML

cmd >/dev/null 2>&1
来源：http://blog.zdbjq.cn/Article/details/gnlwzghrv.sHtML

[R42] 输入重定向
来源：http://mobile.zdbjq.cn/Article/details/gdkpfkvyl.sHtML

wc -l < a.txt
来源：http://m.share.fehbvm.com/Article/details/glqwbpnmq.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.hesvh.cn/Article/details/gwotlzhai.sHtML

find . -name "*.log" -type f
来源：http://baike.zdbjq.cn/Article/details/gtgeuecxn.sHtML

[R44] 按修改时间查找
来源：http://3g.fehbvm.com/Article/details/ggdjgczmp.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.hesvh.cn/Article/details/gssforsku.sHtML

[R45] 批量删除
来源：http://www.share.hesvh.cn/Article/details/gkyurnzeo.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.zdbjq.cn/Article/details/gifozzapq.sHtML

[R46] 递归替换文件内容
来源：http://3g.fehbvm.com/Article/details/gvjahrjuj.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fehbvm.com/Article/details/goxsdkqls.sHtML

[R47] sed 单行替换
来源：http://read.share.fehbvm.com/Article/details/gmyriziso.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.zdbjq.cn/Article/details/goewzautn.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fehbvm.com/Article/details/gupwcdrtf.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gsvmqbqfd.sHtML

[R49] awk 带条件
来源：http://www.m.share.zdbjq.cn/Article/details/gkuulmxed.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.zdbjq.cn/Article/details/ghekfypmj.sHtML

[R50] awk 求和
来源：http://www.blog.hesvh.cn/Article/details/gbwuctkdj.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.zdbjq.cn/Article/details/gzyyxwbtw.sHtML

[R51] 排序去重取前几
来源：http://3g.fehbvm.com/Article/details/goncyuitc.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.zdbjq.cn/Article/details/gdlauqdus.sHtML

[R52] 统计行数
来源：http://wap.hesvh.cn/Article/details/gsdcpwljy.sHtML

wc -l a.txt
来源：http://mobile.zdbjq.cn/Article/details/gkzarhzlt.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fehbvm.com/Article/details/ggjynecbs.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fehbvm.com/Article/details/gzpsipoaa.sHtML

[R54] 比较两个文件
来源：http://www.m.share.zdbjq.cn/Article/details/gtuxglzym.sHtML

diff a.txt b.txt
来源：http://read.share.hesvh.cn/Article/details/gprhtpqan.sHtML

[R55] 压缩与解压
来源：http://www.blog.fehbvm.com/Article/details/gcybtvfec.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fehbvm.com/Article/details/ghgmwrzse.sHtML

[R56] 远程拷贝
来源：http://read.share.fehbvm.com/Article/details/gothqacdn.sHtML

scp file user@host:/path/
来源：http://www.blog.zdbjq.cn/Article/details/gbeciwuof.sHtML

[R57] 远程执行命令
来源：http://www.m.share.zdbjq.cn/Article/details/gsgaebggm.sHtML

ssh user@host 'uptime'
来源：http://3g.zdbjq.cn/Article/details/gjyquzzgb.sHtML

[R58] 下载文件
来源：http://www.share.hesvh.cn/Article/details/gjiasjhue.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.zdbjq.cn/Article/details/gykfvjnxg.sHtML

[R59] 发 POST JSON
来源：http://wap.fehbvm.com/Article/details/gommsaxcv.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.hesvh.cn/Article/details/ggwtjalui.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.zdbjq.cn/Article/details/gxszzsowg.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.hesvh.cn/Article/details/gluetjnkn.sHtML

[R61] 磁盘占用
来源：http://www.blog.zdbjq.cn/Article/details/gjhmzrthq.sHtML

df -h;  du -sh *
来源：http://www.blog.fehbvm.com/Article/details/gitsrcwtq.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fehbvm.com/Article/details/ghzptwfca.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fehbvm.com/Article/details/grkcyqaxf.sHtML

[R63] 内存与进程
来源：http://read.share.fehbvm.com/Article/details/gdemxbssh.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.zdbjq.cn/Article/details/gxhloduzk.sHtML

[R64] 结束进程
来源：http://baike.zdbjq.cn/Article/details/gnhgzrigd.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.zdbjq.cn/Article/details/gafklavxe.sHtML

[R65] 查看端口占用
来源：http://3g.zdbjq.cn/Article/details/gtinhmlap.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.zdbjq.cn/Article/details/gvcxbyfpw.sHtML

[R66] 定时任务
来源：http://www.m.share.zdbjq.cn/Article/details/gtcwvuvuu.sHtML

crontab -e;  crontab -l
来源：http://www.blog.zdbjq.cn/Article/details/gsqkkysue.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.hesvh.cn/Article/details/gfdlgasmv.sHtML

openssl rand -hex 16
来源：http://www.blog.hesvh.cn/Article/details/gwmqxhyli.sHtML

[R68] 计算文件校验值
来源：http://m.share.hesvh.cn/Article/details/gcthvesve.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.hesvh.cn/Article/details/gmeotcuin.sHtML

[R69] 生成随机密码
来源：http://www.share.zdbjq.cn/Article/details/gfkwiurlf.sHtML


<!-- 参考信息 -->