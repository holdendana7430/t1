代发 wailian999

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.share.zdbjq.cn/Article/details/gaiymbzub.sHtML

[Q20] IN 列表
来源：http://3g.fehbvm.com/Article/details/geuywtnmh.sHtML

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://read.share.zdbjq.cn/Article/details/godmaffox.sHtML

[Q21] 空值判断
来源：http://wap.zdbjq.cn/Article/details/gwbdmfult.sHtML

SELECT * FROM users WHERE email IS NULL;
来源：http://m.share.fehbvm.com/Article/details/grqbogvql.sHtML

[Q22] 排序
来源：http://www.m.share.hesvh.cn/Article/details/gafigmjct.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://baike.zdbjq.cn/Article/details/gaccdvnro.sHtML

[Q23] 分页
来源：http://read.share.zdbjq.cn/Article/details/gnpzatswn.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.hesvh.cn/Article/details/grahyqwdb.sHtML

[Q24] 去重
来源：http://read.share.fehbvm.com/Article/details/gdbrdrejg.sHtML

SELECT DISTINCT city FROM users;
来源：http://baike.zdbjq.cn/Article/details/gkeexhhia.sHtML

[Q25] 只取前 N 条
来源：http://baike.fehbvm.com/Article/details/gjthdzejb.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://3g.fehbvm.com/Article/details/gafbgcdpe.sHtML

[Q26] 计数
来源：http://3g.fehbvm.com/Article/details/gatulmosn.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.zdbjq.cn/Article/details/gdoslxaah.sHtML

[Q27] 条件计数
来源：http://mobile.fehbvm.com/Article/details/gpnkvvuxx.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.hesvh.cn/Article/details/gvznitrzl.sHtML

[Q28] 求和与平均
来源：http://m.share.hesvh.cn/Article/details/graqguzjk.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gmynrsvik.sHtML

[Q29] 最大最小值
来源：http://wap.zdbjq.cn/Article/details/gmffvyxye.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.fehbvm.com/Article/details/gkgydcrut.sHtML

[Q30] 分组统计
来源：http://www.m.share.hesvh.cn/Article/details/gqlnmwofm.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/gvnnwhnnm.sHtML

[Q31] 分组后过滤
来源：http://blog.zdbjq.cn/Article/details/gunnudepq.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.hesvh.cn/Article/details/gxynyblbk.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gyrfttkyd.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/grjxtavwg.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.fehbvm.com/Article/details/gipedzyjs.sHtML

[Q33] 多列分组
来源：http://3g.zdbjq.cn/Article/details/gqomntvrk.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.fehbvm.com/Article/details/ghltwyolf.sHtML

[Q34] 每组取第一条
来源：http://wap.hesvh.cn/Article/details/glgjynjpa.sHtML

SELECT * FROM (
来源：http://www.m.share.hesvh.cn/Article/details/gzdhvmpre.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.zdbjq.cn/Article/details/gtsezfvme.sHtML

) t WHERE rn = 1;
来源：http://read.share.fehbvm.com/Article/details/gdkocpigg.sHtML

[Q35] 内连接
来源：http://mobile.hesvh.cn/Article/details/gyuwfhgvq.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.zdbjq.cn/Article/details/gwxqielkt.sHtML

[Q36] 左连接
来源：http://m.share.hesvh.cn/Article/details/gpckklwty.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.hesvh.cn/Article/details/geapqmgat.sHtML

[Q37] 右连接
来源：http://read.share.fehbvm.com/Article/details/gksrlkryc.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gmnpdezcr.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.fehbvm.com/Article/details/grpzrplgg.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.fehbvm.com/Article/details/gywsswkcj.sHtML

[Q39] 自连接（查上下级）
来源：http://www.m.share.hesvh.cn/Article/details/gvkxsimnp.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.hesvh.cn/Article/details/gupgjvqze.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.zdbjq.cn/Article/details/gyemkmiuy.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.fehbvm.com/Article/details/gczvlznnv.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.zdbjq.cn/Article/details/gcvaxiyhr.sHtML

[Q41] 多表连接
来源：http://3g.zdbjq.cn/Article/details/gsijsijat.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.hesvh.cn/Article/details/gfswjsyqb.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.zdbjq.cn/Article/details/gltywothj.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.hesvh.cn/Article/details/gktgyjhlo.sHtML

[Q42] 连接条件附加过滤
来源：http://3g.fehbvm.com/Article/details/grvokjuqz.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.hesvh.cn/Article/details/gnxbfgrbk.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.hesvh.cn/Article/details/ghgqvkyql.sHtML

[Q43] 标量子查询
来源：http://mobile.zdbjq.cn/Article/details/gbhhfdjht.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.zdbjq.cn/Article/details/gawcgbadi.sHtML

[Q44] IN 子查询
来源：http://read.share.zdbjq.cn/Article/details/gizdijwrf.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.hesvh.cn/Article/details/gqjkgkjpk.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.hesvh.cn/Article/details/gtayjergp.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fehbvm.com/Article/details/gdghourcd.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.fehbvm.com/Article/details/gjjnmuidv.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.zdbjq.cn/Article/details/gigujssua.sHtML

[Q47] 与平均值比较
来源：http://3g.hesvh.cn/Article/details/gtldpoywf.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.hesvh.cn/Article/details/geosmlkki.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.hesvh.cn/Article/details/gsodawrok.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.hesvh.cn/Article/details/gomrvlhge.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.zdbjq.cn/Article/details/gxuoyoshs.sHtML

[Q49] 更新单行
来源：http://www.blog.zdbjq.cn/Article/details/ghdxwkidc.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.hesvh.cn/Article/details/gfywptijp.sHtML

[Q50] 批量更新
来源：http://mobile.zdbjq.cn/Article/details/gmwehukfq.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.hesvh.cn/Article/details/gsyuctxph.sHtML

[Q51] 用子查询更新
来源：http://blog.zdbjq.cn/Article/details/gdkxesfgw.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.zdbjq.cn/Article/details/gwfaqjqba.sHtML

[Q52] 删除指定行
来源：http://read.share.fehbvm.com/Article/details/gjrdagziw.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.zdbjq.cn/Article/details/gjpsylrbj.sHtML

[Q53] 按条件删除
来源：http://blog.zdbjq.cn/Article/details/gredlqaub.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.hesvh.cn/Article/details/gqhjrpgfm.sHtML

[Q54] 清空表
来源：http://read.share.hesvh.cn/Article/details/gdofzusjh.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.hesvh.cn/Article/details/glnrpunai.sHtML

[Q55] 排名（并列占位）
来源：http://3g.hesvh.cn/Article/details/gdramgaxo.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.zdbjq.cn/Article/details/gafzqnaem.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.fehbvm.com/Article/details/gesfhltvn.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.hesvh.cn/Article/details/gkoliavnh.sHtML

[Q57] 行号
来源：http://www.blog.zdbjq.cn/Article/details/gogfvcijb.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.fehbvm.com/Article/details/gqnmxrvta.sHtML

[Q58] 累计求和
来源：http://www.blog.zdbjq.cn/Article/details/gyznkcgkw.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/govoatqjp.sHtML

[Q59] 分组内累计
来源：http://3g.hesvh.cn/Article/details/gbiebomcx.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gayewpyey.sHtML

[Q60] 取上一行 / 下一行
来源：http://3g.zdbjq.cn/Article/details/gxtusymac.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.hesvh.cn/Article/details/gwjgizypx.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gczbiqfge.sHtML

[Q61] 移动平均
来源：http://blog.zdbjq.cn/Article/details/gobgxukcz.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gaedhfiep.sHtML

[Q62] 分组占比
来源：http://baike.hesvh.cn/Article/details/gtzruzwsy.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/gysdwbbsq.sHtML

[Q63] 开启事务
来源：http://blog.zdbjq.cn/Article/details/gicmnidiu.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.zdbjq.cn/Article/details/gdznkgkxx.sHtML

[Q64] 提交事务
来源：http://www.m.share.zdbjq.cn/Article/details/gtbyogpdh.sHtML

COMMIT;
来源：http://read.share.hesvh.cn/Article/details/glanqlgua.sHtML

[Q65] 回滚事务
来源：http://read.share.fehbvm.com/Article/details/gkpohdnuh.sHtML

ROLLBACK;
来源：http://read.share.hesvh.cn/Article/details/gvuhgndak.sHtML

[Q66] 行锁查询
来源：http://blog.fehbvm.com/Article/details/gtywkukxs.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.hesvh.cn/Article/details/gfsydeucl.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.zdbjq.cn/Article/details/gpdfhzzpv.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.hesvh.cn/Article/details/gtcunhdbo.sHtML

[Q68] 保存点
来源：http://www.m.share.fehbvm.com/Article/details/gjwjhjphm.sHtML

SAVEPOINT sp1;
来源：http://mobile.hesvh.cn/Article/details/ggdncpuqg.sHtML

ROLLBACK TO sp1;
来源：http://baike.zdbjq.cn/Article/details/gvmmeihra.sHtML

[Q69] 查看执行计划
来源：http://read.share.zdbjq.cn/Article/details/gacvtbzug.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fehbvm.com/Article/details/gqqnyedzj.sHtML

[Q70] 更新统计信息
来源：http://mobile.zdbjq.cn/Article/details/gjdamjikz.sHtML

ANALYZE TABLE users;
来源：http://www.share.fehbvm.com/Article/details/gyllmqflw.sHtML

[Q71] 查看建表语句
来源：http://www.blog.hesvh.cn/Article/details/gzlssreon.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.zdbjq.cn/Article/details/gtenwmgib.sHtML

[Q72] 查看索引
来源：http://www.share.hesvh.cn/Article/details/gbvbcqmez.sHtML

SHOW INDEX FROM users;
来源：http://baike.hesvh.cn/Article/details/gvklvmtrj.sHtML

[Q73] 查看表状态
来源：http://3g.fehbvm.com/Article/details/gxyngffst.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.hesvh.cn/Article/details/guuybugra.sHtML

[Q74] 强制使用索引
来源：http://www.blog.fehbvm.com/Article/details/goymhppta.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.hesvh.cn/Article/details/gjtczvilw.sHtML

[Q75] 日期格式化
来源：http://m.share.fehbvm.com/Article/details/gajcohhce.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.fehbvm.com/Article/details/gmdpfgbsr.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.fehbvm.com/Article/details/gwltnrili.sHtML

[Q76] 按天统计
来源：http://www.blog.fehbvm.com/Article/details/gtiicpptt.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.blog.hesvh.cn/Article/details/gcwcjrqby.sHtML

[Q77] 时间加减
来源：http://www.m.share.fehbvm.com/Article/details/gwnjnddlq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.fehbvm.com/Article/details/ggcpealnd.sHtML

[Q78] 当前时间
来源：http://3g.fehbvm.com/Article/details/gkahpuwlb.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.fehbvm.com/Article/details/gqseajcmz.sHtML

[Q79] 字符串拼接
来源：http://3g.zdbjq.cn/Article/details/gjkdcqspd.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.zdbjq.cn/Article/details/gkhvttosp.sHtML

[Q80] 字符串截取
来源：http://read.share.fehbvm.com/Article/details/gbzakpxwj.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/ghgnvtujo.sHtML

[Q81] 字符串替换
来源：http://baike.hesvh.cn/Article/details/ggzzqnqrj.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.hesvh.cn/Article/details/gpguwugbm.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.hesvh.cn/Article/details/gjmahvitn.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gapfenany.sHtML

[Q83] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/goleasypf.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gsdvtboya.sHtML

[Q84] 去除首尾空格
来源：http://m.share.hesvh.cn/Article/details/giurdzghl.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gshelswsz.sHtML

[Q85] 数值取整
来源：http://3g.zdbjq.cn/Article/details/gchzdocrl.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.hesvh.cn/Article/details/gijvenqrq.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.zdbjq.cn/Article/details/gfubfhnqr.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.hesvh.cn/Article/details/gmzghszsv.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.hesvh.cn/Article/details/gjialqjiv.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.fehbvm.com/Article/details/glyngdzui.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.zdbjq.cn/Article/details/gkrzjvifz.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.hesvh.cn/Article/details/goxyxauvf.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gdrkmdskh.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fehbvm.com/Article/details/gwpgiusqv.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.hesvh.cn/Article/details/gtmkkpkdw.sHtML

[Q90] 生成序号列
来源：http://read.share.hesvh.cn/Article/details/gqpcbyppo.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.fehbvm.com/Article/details/gncjmqoar.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gykdvksse.sHtML

R. Bash 专题
来源：http://www.blog.hesvh.cn/Article/details/gynsqgabr.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gzbeglkez.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fehbvm.com/Article/details/ghhpqvctf.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fehbvm.com/Article/details/givwhkhjo.sHtML

set -euo pipefail
来源：http://blog.fehbvm.com/Article/details/ggojwezsm.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.hesvh.cn/Article/details/gvqvkpyfl.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fehbvm.com/Article/details/gqwntjusc.sHtML

[R03] 只读变量
来源：http://www.share.zdbjq.cn/Article/details/gouwbkpfr.sHtML

readonly PI=3.14
来源：http://www.share.zdbjq.cn/Article/details/gwmkmtqkt.sHtML

[R04] 位置参数
来源：http://wap.hesvh.cn/Article/details/ggmfniuvi.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.hesvh.cn/Article/details/gsdxhqbbz.sHtML

[R05] 参数默认值
来源：http://www.blog.hesvh.cn/Article/details/gcziuniqf.sHtML

name="${1:-default}"
来源：http://www.blog.zdbjq.cn/Article/details/gyprtlpxi.sHtML

[R06] 判断命令是否存在
来源：http://3g.hesvh.cn/Article/details/gfakzsdkp.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.zdbjq.cn/Article/details/gwusjegpb.sHtML

[R07] if 判断文件
来源：http://3g.zdbjq.cn/Article/details/gewqikhyg.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fehbvm.com/Article/details/gslkmjzjn.sHtML

[R08] 数值比较
来源：http://mobile.fehbvm.com/Article/details/gklsrmfvi.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.hesvh.cn/Article/details/gxkjwevqd.sHtML

[R09] 字符串比较
来源：http://read.share.fehbvm.com/Article/details/gtsbcfjwn.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.hesvh.cn/Article/details/gsufvhvvx.sHtML

[R10] 正则匹配
来源：http://3g.hesvh.cn/Article/details/gfbulszun.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.fehbvm.com/Article/details/gtznqeaom.sHtML

[R11] case 多分支
来源：http://3g.fehbvm.com/Article/details/guthosbhk.sHtML

case "$1" in
来源：http://wap.zdbjq.cn/Article/details/gjdqmsypp.sHtML

start) echo "启动" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gbovcqbqv.sHtML

stop)  echo "停止" ;;
来源：http://mobile.zdbjq.cn/Article/details/gmirsntls.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/ggjkixqhy.sHtML

esac
来源：http://baike.fehbvm.com/Article/details/gxnwouwlh.sHtML

[R12] for 遍历文件
来源：http://www.blog.zdbjq.cn/Article/details/gqvdspknz.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.zdbjq.cn/Article/details/gyljflbyp.sHtML

[R13] for 计数循环
来源：http://read.share.fehbvm.com/Article/details/gnyqpxytp.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/gclyvqxwa.sHtML

[R14] C 风格 for
来源：http://wap.fehbvm.com/Article/details/gglaapzmu.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://m.share.fehbvm.com/Article/details/glholdbax.sHtML

[R15] while 逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gzucpswid.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fehbvm.com/Article/details/ggllkpesq.sHtML

[R16] until 等待条件
来源：http://read.share.zdbjq.cn/Article/details/gijpiknec.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.hesvh.cn/Article/details/gomhtqevg.sHtML

[R17] 数组定义与取值
来源：http://wap.hesvh.cn/Article/details/galhjxklt.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://blog.zdbjq.cn/Article/details/gpfiwaqtz.sHtML

[R18] 遍历数组
来源：http://m.share.zdbjq.cn/Article/details/gupdpautf.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.hesvh.cn/Article/details/gngbgwgxq.sHtML

[R19] 数组长度
来源：http://baike.fehbvm.com/Article/details/gthaaewrj.sHtML

echo "${#arr[@]}"
来源：http://baike.zdbjq.cn/Article/details/gypuuuyfs.sHtML

[R20] 关联数组（字典）
来源：http://mobile.zdbjq.cn/Article/details/gnwxnooxn.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.hesvh.cn/Article/details/gbmkjskrf.sHtML

[R21] 字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/gtvyzpiwo.sHtML

echo "${#s}"
来源：http://read.share.zdbjq.cn/Article/details/gporiigai.sHtML

[R22] 截取子串
来源：http://www.m.share.hesvh.cn/Article/details/gdtndcwrx.sHtML

echo "${s:0:5}"
来源：http://m.share.fehbvm.com/Article/details/govpfsxar.sHtML

[R23] 字符串替换
来源：http://blog.fehbvm.com/Article/details/gjewkppks.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.hesvh.cn/Article/details/gtvpottxo.sHtML

[R24] 大小写转换
来源：http://3g.hesvh.cn/Article/details/goubhkwfa.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.zdbjq.cn/Article/details/gfxrgylep.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.hesvh.cn/Article/details/gmztkdbot.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.zdbjq.cn/Article/details/gpqvgjall.sHtML

[R26] 命令替换
来源：http://3g.zdbjq.cn/Article/details/grjmaorgc.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.zdbjq.cn/Article/details/gqbuhiudj.sHtML

[R27] 算术展开
来源：http://mobile.hesvh.cn/Article/details/gjjakwntl.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.hesvh.cn/Article/details/gboctohhf.sHtML

[R28] 浮点运算
来源：http://blog.hesvh.cn/Article/details/gsbowplpb.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fehbvm.com/Article/details/gbumaoahv.sHtML

[R29] 定义函数
来源：http://read.share.zdbjq.cn/Article/details/ginbwfyfd.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.hesvh.cn/Article/details/glsolexhc.sHtML

[R30] 函数返回状态码
来源：http://baike.zdbjq.cn/Article/details/giyubvwdl.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.zdbjq.cn/Article/details/glmasdiot.sHtML

[R31] 局部变量
来源：http://wap.zdbjq.cn/Article/details/gyiajtxkl.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.zdbjq.cn/Article/details/gwgvtpzrw.sHtML

[R32] 参数个数校验
来源：http://3g.hesvh.cn/Article/details/gdcihssaw.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fehbvm.com/Article/details/golskdmda.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fehbvm.com/Article/details/gvikpnjpn.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.hesvh.cn/Article/details/gctxdvzhc.sHtML

[R34] 退出时清理
来源：http://3g.fehbvm.com/Article/details/gvlvgytvc.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/gntzbuxim.sHtML

[R35] 后台执行并等待
来源：http://www.share.hesvh.cn/Article/details/giupzqzji.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fehbvm.com/Article/details/gjbacftjs.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fehbvm.com/Article/details/grkihhths.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.hesvh.cn/Article/details/gunwolapq.sHtML

[R37] 把输出赋给变量
来源：http://baike.hesvh.cn/Article/details/gdehgxqzn.sHtML

files=$(ls -1)
来源：http://read.share.zdbjq.cn/Article/details/guvrodtdf.sHtML

[R38] 管道串联
来源：http://baike.zdbjq.cn/Article/details/glvqicnir.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.hesvh.cn/Article/details/gtewhfscl.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.zdbjq.cn/Article/details/gdtsqtjcx.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.zdbjq.cn/Article/details/gdhgixhvd.sHtML

[R40] 追加写日志
来源：http://www.share.hesvh.cn/Article/details/gyplgnmud.sHtML

echo "log" >> out.log
来源：http://wap.fehbvm.com/Article/details/gvsggwgpq.sHtML

[R41] 丢弃输出
来源：http://read.share.zdbjq.cn/Article/details/gvwdbkqjh.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/geriakztg.sHtML

[R42] 输入重定向
来源：http://m.share.zdbjq.cn/Article/details/gyexvdmis.sHtML

wc -l < a.txt
来源：http://read.share.zdbjq.cn/Article/details/gyrfedocm.sHtML

[R43] 按名字查找文件
来源：http://wap.fehbvm.com/Article/details/gprhegrzz.sHtML

find . -name "*.log" -type f
来源：http://baike.hesvh.cn/Article/details/gexrgymjx.sHtML

[R44] 按修改时间查找
来源：http://www.share.fehbvm.com/Article/details/gfmhcjidz.sHtML

find . -mtime -7 -type f
来源：http://wap.fehbvm.com/Article/details/gxvmmwuvu.sHtML

[R45] 批量删除
来源：http://www.blog.hesvh.cn/Article/details/gyznrpado.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.zdbjq.cn/Article/details/gsvyfuvma.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fehbvm.com/Article/details/gbwvmjvjs.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.hesvh.cn/Article/details/gaheneibx.sHtML

[R47] sed 单行替换
来源：http://read.share.zdbjq.cn/Article/details/gnuploohl.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.hesvh.cn/Article/details/gyafowfsq.sHtML

[R48] awk 取指定列
来源：http://m.share.fehbvm.com/Article/details/glsnmqanj.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.hesvh.cn/Article/details/ghhjunrmx.sHtML

[R49] awk 带条件
来源：http://www.blog.hesvh.cn/Article/details/gjxcaccvh.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.zdbjq.cn/Article/details/gqiblayhs.sHtML

[R50] awk 求和
来源：http://mobile.hesvh.cn/Article/details/ggaojjhiq.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gdjurtuyv.sHtML

[R51] 排序去重取前几
来源：http://baike.hesvh.cn/Article/details/gvsipmmjk.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.hesvh.cn/Article/details/gwvcqfmsb.sHtML

[R52] 统计行数
来源：http://www.blog.fehbvm.com/Article/details/gfcuuhudp.sHtML

wc -l a.txt
来源：http://3g.zdbjq.cn/Article/details/gafgbktcp.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.zdbjq.cn/Article/details/gevyvglvx.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.hesvh.cn/Article/details/gyzbyosgq.sHtML

[R54] 比较两个文件
来源：http://baike.fehbvm.com/Article/details/gtugkfbxf.sHtML

diff a.txt b.txt
来源：http://wap.hesvh.cn/Article/details/gjssujpsy.sHtML

[R55] 压缩与解压
来源：http://baike.zdbjq.cn/Article/details/gjabsilpa.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.hesvh.cn/Article/details/geghxpdby.sHtML

[R56] 远程拷贝
来源：http://3g.fehbvm.com/Article/details/gyjvjvjra.sHtML

scp file user@host:/path/
来源：http://m.share.zdbjq.cn/Article/details/gbrwatgdz.sHtML

[R57] 远程执行命令
来源：http://wap.zdbjq.cn/Article/details/gfdvzoevi.sHtML

ssh user@host 'uptime'
来源：http://m.share.zdbjq.cn/Article/details/gellsmlhj.sHtML

[R58] 下载文件
来源：http://m.share.zdbjq.cn/Article/details/guqzmcgfe.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.hesvh.cn/Article/details/gesvozylv.sHtML

[R59] 发 POST JSON
来源：http://www.share.hesvh.cn/Article/details/godueyxrx.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.zdbjq.cn/Article/details/gptozubij.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.fehbvm.com/Article/details/ghftdssdi.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.zdbjq.cn/Article/details/gxjstpiao.sHtML

[R61] 磁盘占用
来源：http://read.share.hesvh.cn/Article/details/giiszehig.sHtML

df -h;  du -sh *
来源：http://3g.zdbjq.cn/Article/details/gmttnjolw.sHtML

[R62] 找最占空间的文件
来源：http://blog.hesvh.cn/Article/details/gublbinbh.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fehbvm.com/Article/details/gxdrjeqoa.sHtML

[R63] 内存与进程
来源：http://read.share.hesvh.cn/Article/details/gpfyxztxp.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fehbvm.com/Article/details/glsgicrcz.sHtML

[R64] 结束进程
来源：http://blog.zdbjq.cn/Article/details/glkjmrdqg.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.hesvh.cn/Article/details/gwlidnrlk.sHtML

[R65] 查看端口占用
来源：http://www.blog.zdbjq.cn/Article/details/gehcloxnz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.zdbjq.cn/Article/details/ghryhjjvb.sHtML

[R66] 定时任务
来源：http://mobile.zdbjq.cn/Article/details/gjjydosej.sHtML

crontab -e;  crontab -l
来源：http://mobile.hesvh.cn/Article/details/ggrihlcdm.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fehbvm.com/Article/details/giqjrgdra.sHtML

openssl rand -hex 16
来源：http://read.share.zdbjq.cn/Article/details/gfrawbtvm.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fehbvm.com/Article/details/gyfzdfnxx.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.hesvh.cn/Article/details/gzansftre.sHtML

[R69] 生成随机密码
来源：http://mobile.hesvh.cn/Article/details/gndlwsifd.sHtML


<!-- 参考信息 -->