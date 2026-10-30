代发 wailian999

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gynxynfsi.sHtML

[Q28] 求和与平均
来源：http://read.share.fanxiaobao.xyz/Article/details/gduivprmq.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnroeydpg.sHtML

[Q29] 最大最小值
来源：http://wap.fanxiaobao.xyz/Article/details/gmtppaonx.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghmyrgsjm.sHtML

[Q30] 分组统计
来源：http://m.share.fanxiaobao.xyz/Article/details/guohjsrbx.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnczlalpk.sHtML

[Q31] 分组后过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gepnhjlzv.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxdobhpsp.sHtML

[Q32] 分组拼接字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/gtnjhmhsx.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.fanxiaobao.xyz/Article/details/guxvyiejo.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.fanxiaobao.xyz/Article/details/gznhsyzgi.sHtML

[Q33] 多列分组
来源：http://www.share.fanxiaobao.xyz/Article/details/gqouovmrk.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.fanxiaobao.xyz/Article/details/gsdshuoda.sHtML

[Q34] 每组取第一条
来源：http://www.share.fanxiaobao.xyz/Article/details/gdcppqmyj.sHtML

SELECT * FROM (
来源：http://wap.fanxiaobao.xyz/Article/details/gkdjwqjpv.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.fanxiaobao.xyz/Article/details/gqqgjibgf.sHtML

) t WHERE rn = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gsmkirdfs.sHtML

[Q35] 内连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gztuabkkf.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fanxiaobao.xyz/Article/details/guckzwvcp.sHtML

[Q36] 左连接
来源：http://blog.fanxiaobao.xyz/Article/details/gvyfxxylh.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqcjbjbdp.sHtML

[Q37] 右连接
来源：http://wap.fanxiaobao.xyz/Article/details/gpocpeyao.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghyvqsedk.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.fanxiaobao.xyz/Article/details/gifevelep.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.fanxiaobao.xyz/Article/details/gdeyeghzc.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.fanxiaobao.xyz/Article/details/geniqudtr.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.share.fanxiaobao.xyz/Article/details/gkjdxuzmm.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gztulqhvh.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://m.share.fanxiaobao.xyz/Article/details/gsmyssfur.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.fanxiaobao.xyz/Article/details/gxbnkzosh.sHtML

[Q41] 多表连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkkwdbizd.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfroxutbo.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.fanxiaobao.xyz/Article/details/gchappuua.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.fanxiaobao.xyz/Article/details/gnfubtdvq.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gcclhamoz.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.fanxiaobao.xyz/Article/details/ghgmotgre.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqpdvtqjp.sHtML

[Q43] 标量子查询
来源：http://baike.fanxiaobao.xyz/Article/details/gtcqhwhwg.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkplalpoh.sHtML

[Q44] IN 子查询
来源：http://baike.fanxiaobao.xyz/Article/details/glqthldnl.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcnmvgqis.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gzmkpnnua.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fanxiaobao.xyz/Article/details/gnknrwkdd.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/glbcsqmfg.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fanxiaobao.xyz/Article/details/gtuhjffen.sHtML

[Q47] 与平均值比较
来源：http://blog.fanxiaobao.xyz/Article/details/gmorrtmbz.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpoafoevx.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzlcqndvo.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://baike.fanxiaobao.xyz/Article/details/goltxczia.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.fanxiaobao.xyz/Article/details/gsoheyvll.sHtML

[Q49] 更新单行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gedgqaszo.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gzccxgocr.sHtML

[Q50] 批量更新
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmwoovzhz.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.fanxiaobao.xyz/Article/details/gjqkyyvlj.sHtML

[Q51] 用子查询更新
来源：http://3g.fanxiaobao.xyz/Article/details/gfwsufzsf.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gafnwmrzo.sHtML

[Q52] 删除指定行
来源：http://baike.fanxiaobao.xyz/Article/details/gdgunmlnh.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gvefiewsf.sHtML

[Q53] 按条件删除
来源：http://wap.fanxiaobao.xyz/Article/details/gqmkydccx.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.fanxiaobao.xyz/Article/details/genivrybc.sHtML

[Q54] 清空表
来源：http://read.share.fanxiaobao.xyz/Article/details/gmhvcbmtb.sHtML

TRUNCATE TABLE logs;
来源：http://baike.fanxiaobao.xyz/Article/details/goiswzqrf.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcpjeokbk.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.fanxiaobao.xyz/Article/details/gabwgryor.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.fanxiaobao.xyz/Article/details/gpbrgwqbk.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.fanxiaobao.xyz/Article/details/godivpcfk.sHtML

[Q57] 行号
来源：http://3g.fanxiaobao.xyz/Article/details/gfzlxvxgz.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gtqqxswwq.sHtML

[Q58] 累计求和
来源：http://www.share.fanxiaobao.xyz/Article/details/grzndedse.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqkxcpklz.sHtML

[Q59] 分组内累计
来源：http://read.share.fanxiaobao.xyz/Article/details/geaxfirph.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghdyvcayy.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.fanxiaobao.xyz/Article/details/gfgovdkwp.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.fanxiaobao.xyz/Article/details/ggfcxxdqz.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gazedrezq.sHtML

[Q61] 移动平均
来源：http://baike.fanxiaobao.xyz/Article/details/gelsumfyo.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gabiontvw.sHtML

[Q62] 分组占比
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guznhbngi.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmflkvvjs.sHtML

[Q63] 开启事务
来源：http://wap.fanxiaobao.xyz/Article/details/gfssfkpmh.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.fanxiaobao.xyz/Article/details/gogdnawya.sHtML

[Q64] 提交事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpulsgcvi.sHtML

COMMIT;
来源：http://wap.fanxiaobao.xyz/Article/details/gmrfxjdic.sHtML

[Q65] 回滚事务
来源：http://baike.fanxiaobao.xyz/Article/details/gsxmprqlo.sHtML

ROLLBACK;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwutumqxb.sHtML

[Q66] 行锁查询
来源：http://m.share.fanxiaobao.xyz/Article/details/gpkhvzchc.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvbqndbdq.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpflnqnrm.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.fanxiaobao.xyz/Article/details/gcamqcaat.sHtML

[Q68] 保存点
来源：http://m.share.fanxiaobao.xyz/Article/details/gtkxtqgdk.sHtML

SAVEPOINT sp1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsppnmmgv.sHtML

ROLLBACK TO sp1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gcorxeuth.sHtML

[Q69] 查看执行计划
来源：http://3g.fanxiaobao.xyz/Article/details/gvnzyelle.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbqlharfi.sHtML

[Q70] 更新统计信息
来源：http://baike.fanxiaobao.xyz/Article/details/gmcylwlvr.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gziccbvyw.sHtML

[Q71] 查看建表语句
来源：http://blog.fanxiaobao.xyz/Article/details/gwlvokfnh.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.fanxiaobao.xyz/Article/details/gujxqfdpy.sHtML

[Q72] 查看索引
来源：http://baike.fanxiaobao.xyz/Article/details/gsrogfayh.sHtML

SHOW INDEX FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gxgiqfkch.sHtML

[Q73] 查看表状态
来源：http://read.share.fanxiaobao.xyz/Article/details/ghwjzdxux.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvrbhjtii.sHtML

[Q74] 强制使用索引
来源：http://3g.fanxiaobao.xyz/Article/details/gtbvesvog.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.fanxiaobao.xyz/Article/details/ghjoyjdbv.sHtML

[Q75] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gnefokixf.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/guoctooiu.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guoiyasum.sHtML

[Q76] 按天统计
来源：http://m.share.fanxiaobao.xyz/Article/details/gibfembco.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.fanxiaobao.xyz/Article/details/gemdcblyv.sHtML

[Q77] 时间加减
来源：http://read.share.fanxiaobao.xyz/Article/details/gbsmpkppj.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmhfenpda.sHtML

[Q78] 当前时间
来源：http://m.share.fanxiaobao.xyz/Article/details/geamcchyu.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkxpowflm.sHtML

[Q79] 字符串拼接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqqogjasq.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.fanxiaobao.xyz/Article/details/gurvbkndx.sHtML

[Q80] 字符串截取
来源：http://www.share.fanxiaobao.xyz/Article/details/gvdozqsrh.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzhukzivr.sHtML

[Q81] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gbvyftdfz.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/goefjnzkk.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzonurujo.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggqsopzvi.sHtML

[Q83] 大小写转换
来源：http://3g.fanxiaobao.xyz/Article/details/ggxuegtgj.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/goavakcqy.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fanxiaobao.xyz/Article/details/gosycxukx.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gbdjcgenq.sHtML

[Q85] 数值取整
来源：http://m.share.fanxiaobao.xyz/Article/details/gwmhcsasy.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.fanxiaobao.xyz/Article/details/gundrdjrr.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fanxiaobao.xyz/Article/details/gilflzrqw.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.fanxiaobao.xyz/Article/details/gjddcaxyx.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fanxiaobao.xyz/Article/details/geqqwtvwy.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.fanxiaobao.xyz/Article/details/gyqaanbtj.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.fanxiaobao.xyz/Article/details/gcjatcvmq.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.fanxiaobao.xyz/Article/details/glcabdwog.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtkyocqvh.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjcezkyjh.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fanxiaobao.xyz/Article/details/gtufxssbe.sHtML

[Q90] 生成序号列
来源：http://www.share.fanxiaobao.xyz/Article/details/gxmbxojon.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqyjkzfjk.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gwgocladg.sHtML

R. Bash 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfyigcrnt.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/grjcwhuim.sHtML

[R01] shebang 与严格模式
来源：http://m.share.fanxiaobao.xyz/Article/details/gaeubwfej.sHtML

#!/usr/bin/env bash
来源：http://blog.fanxiaobao.xyz/Article/details/gomxqlsbg.sHtML

set -euo pipefail
来源：http://m.share.fanxiaobao.xyz/Article/details/ghkqtgssf.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fanxiaobao.xyz/Article/details/gaohyyxbh.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fanxiaobao.xyz/Article/details/gsamqwfvh.sHtML

[R03] 只读变量
来源：http://baike.fanxiaobao.xyz/Article/details/gcwwawblf.sHtML

readonly PI=3.14
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdwbhnpbe.sHtML

[R04] 位置参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gzvbngzod.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fanxiaobao.xyz/Article/details/guhpdfsml.sHtML

[R05] 参数默认值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcuncdxrb.sHtML

name="${1:-default}"
来源：http://3g.fanxiaobao.xyz/Article/details/gtsjqrnys.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fanxiaobao.xyz/Article/details/gggvofane.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/grbdiyalg.sHtML

[R07] if 判断文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gqvduczla.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gqrkbtbvf.sHtML

[R08] 数值比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gczbrqlxx.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gfekenjmj.sHtML

[R09] 字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gwidmqsbh.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.fanxiaobao.xyz/Article/details/gaagcaesp.sHtML

[R10] 正则匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/grbeyflfo.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtzfbthxl.sHtML

[R11] case 多分支
来源：http://read.share.fanxiaobao.xyz/Article/details/gjdqzlzee.sHtML

case "$1" in
来源：http://mobile.fanxiaobao.xyz/Article/details/gowozitms.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gekoepzxo.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/ggqtxnbwd.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gnwpytxpk.sHtML

esac
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdynsdfiz.sHtML

[R12] for 遍历文件
来源：http://wap.fanxiaobao.xyz/Article/details/gqszrgufm.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gmfgrdxen.sHtML

[R13] for 计数循环
来源：http://blog.fanxiaobao.xyz/Article/details/gcligqasr.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gphyhulhj.sHtML

[R14] C 风格 for
来源：http://3g.fanxiaobao.xyz/Article/details/ghpskmugt.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gnfluvdsd.sHtML

[R15] while 逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gfbgvpthc.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/geprpxtaa.sHtML

[R16] until 等待条件
来源：http://3g.fanxiaobao.xyz/Article/details/gjlerssqf.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/glnuvvacf.sHtML

[R17] 数组定义与取值
来源：http://3g.fanxiaobao.xyz/Article/details/gtraoqrag.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gspgbbdpw.sHtML

[R18] 遍历数组
来源：http://blog.fanxiaobao.xyz/Article/details/gvsupfzse.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpiyulkps.sHtML

[R19] 数组长度
来源：http://baike.fanxiaobao.xyz/Article/details/gebqbajys.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvotfrqul.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkaxwytxr.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gcczkfmif.sHtML

[R21] 字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gkbszkamz.sHtML

echo "${#s}"
来源：http://blog.fanxiaobao.xyz/Article/details/gudyvfpyz.sHtML

[R22] 截取子串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwqjgzdqy.sHtML

echo "${s:0:5}"
来源：http://www.share.fanxiaobao.xyz/Article/details/grehfbhvg.sHtML

[R23] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/ghiaynqzu.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fanxiaobao.xyz/Article/details/geujtgcck.sHtML

[R24] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/ginzawjgu.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fanxiaobao.xyz/Article/details/gzedrcrky.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbvzdnvwk.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fanxiaobao.xyz/Article/details/gbpfsvwey.sHtML

[R26] 命令替换
来源：http://baike.fanxiaobao.xyz/Article/details/gbzqcdqwe.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fanxiaobao.xyz/Article/details/gawfpdiaw.sHtML

[R27] 算术展开
来源：http://mobile.fanxiaobao.xyz/Article/details/gsrrhzsdb.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fanxiaobao.xyz/Article/details/gnnrbgaym.sHtML

[R28] 浮点运算
来源：http://blog.fanxiaobao.xyz/Article/details/gopizgslk.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fanxiaobao.xyz/Article/details/gcauyarbk.sHtML

[R29] 定义函数
来源：http://baike.fanxiaobao.xyz/Article/details/gbzntfzif.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fanxiaobao.xyz/Article/details/glbhcpefa.sHtML

[R30] 函数返回状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gkqhrlvvv.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fanxiaobao.xyz/Article/details/ggroltvxy.sHtML

[R31] 局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/gumbrcugm.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fanxiaobao.xyz/Article/details/ggykugchi.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gewftwqhe.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkknmzvqd.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvimpimlr.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fanxiaobao.xyz/Article/details/gcyujshwu.sHtML

[R34] 退出时清理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbagmxufx.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvulakqkw.sHtML

[R35] 后台执行并等待
来源：http://baike.fanxiaobao.xyz/Article/details/gppjzhyyy.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fanxiaobao.xyz/Article/details/grgmhjgvj.sHtML

[R36] 并发执行多个任务
来源：http://3g.fanxiaobao.xyz/Article/details/ggxokhlwc.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghandnwtk.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpayvuirt.sHtML

files=$(ls -1)
来源：http://mobile.fanxiaobao.xyz/Article/details/gnaajkegl.sHtML

[R38] 管道串联
来源：http://blog.fanxiaobao.xyz/Article/details/gttnihtua.sHtML

cat a.txt | grep -i error | wc -l
来源：http://blog.fanxiaobao.xyz/Article/details/gvkhkjcmd.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fanxiaobao.xyz/Article/details/gjemoaflz.sHtML

cmd > out.log 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gahmccxpr.sHtML

[R40] 追加写日志
来源：http://3g.fanxiaobao.xyz/Article/details/gbghqupio.sHtML

echo "log" >> out.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gwyuaxgmg.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gezioxaee.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/ggiucthxn.sHtML

[R42] 输入重定向
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcstjrouw.sHtML

wc -l < a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gwozoftki.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goxotfqix.sHtML

find . -name "*.log" -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gcmpbrink.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grppxjalw.sHtML

find . -mtime -7 -type f
来源：http://wap.fanxiaobao.xyz/Article/details/gihsvvbhm.sHtML

[R45] 批量删除
来源：http://m.share.fanxiaobao.xyz/Article/details/gpvkeawgf.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvoeqwkdt.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fanxiaobao.xyz/Article/details/gkvabgxtw.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.fanxiaobao.xyz/Article/details/gljdoptpr.sHtML

[R47] sed 单行替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gfvnetclr.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghtqyqlts.sHtML

[R48] awk 取指定列
来源：http://baike.fanxiaobao.xyz/Article/details/gswroiaqp.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmelnthyb.sHtML

[R49] awk 带条件
来源：http://baike.fanxiaobao.xyz/Article/details/ggaypbrvv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fanxiaobao.xyz/Article/details/gyhnbiqxm.sHtML

[R50] awk 求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggtrppzhy.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggwsgtpqx.sHtML

[R51] 排序去重取前几
来源：http://3g.fanxiaobao.xyz/Article/details/gxmdegfsv.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fanxiaobao.xyz/Article/details/gufvqjbbh.sHtML

[R52] 统计行数
来源：http://www.share.fanxiaobao.xyz/Article/details/goigwgbjx.sHtML

wc -l a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gnheqrqay.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.fanxiaobao.xyz/Article/details/gbeunnsjo.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxokerfzp.sHtML

[R54] 比较两个文件
来源：http://3g.fanxiaobao.xyz/Article/details/grkagdekb.sHtML

diff a.txt b.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gpgrmmhtr.sHtML

[R55] 压缩与解压
来源：http://3g.fanxiaobao.xyz/Article/details/gwrjvwjte.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdynscshz.sHtML

[R56] 远程拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gzighldwz.sHtML

scp file user@host:/path/
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gutzfnuac.sHtML

[R57] 远程执行命令
来源：http://mobile.fanxiaobao.xyz/Article/details/gsmejsnzo.sHtML

ssh user@host 'uptime'
来源：http://blog.fanxiaobao.xyz/Article/details/gvhwqiuxc.sHtML

[R58] 下载文件
来源：http://wap.fanxiaobao.xyz/Article/details/gfydfcics.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fanxiaobao.xyz/Article/details/gtlyhfnbx.sHtML

[R59] 发 POST JSON
来源：http://www.share.fanxiaobao.xyz/Article/details/gdgpnimon.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fanxiaobao.xyz/Article/details/gxvhaudbe.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fanxiaobao.xyz/Article/details/guqpcydpc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fanxiaobao.xyz/Article/details/grkbfyudk.sHtML

[R61] 磁盘占用
来源：http://www.share.fanxiaobao.xyz/Article/details/ggyyhhrhm.sHtML

df -h;  du -sh *
来源：http://www.share.fanxiaobao.xyz/Article/details/gfgvgimwt.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gojqqjcmg.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fanxiaobao.xyz/Article/details/gwurfxptl.sHtML

[R63] 内存与进程
来源：http://blog.fanxiaobao.xyz/Article/details/gnrnznlgb.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fanxiaobao.xyz/Article/details/ggldilsiv.sHtML

[R64] 结束进程
来源：http://3g.fanxiaobao.xyz/Article/details/gnbnhirrl.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaxslkiur.sHtML

[R65] 查看端口占用
来源：http://wap.fanxiaobao.xyz/Article/details/gbaodsmib.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwwgxyktp.sHtML

[R66] 定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggeqhmhvb.sHtML

crontab -e;  crontab -l
来源：http://read.share.fanxiaobao.xyz/Article/details/gbrlgbabx.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fanxiaobao.xyz/Article/details/gxstfybmr.sHtML

openssl rand -hex 16
来源：http://m.share.fanxiaobao.xyz/Article/details/gplrvrrjz.sHtML

[R68] 计算文件校验值
来源：http://read.share.fanxiaobao.xyz/Article/details/gdtmxtkxp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gtmwjyonf.sHtML

[R69] 生成随机密码
来源：http://m.share.fanxiaobao.xyz/Article/details/gdnqmxmhy.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fanxiaobao.xyz/Article/details/ggovhejzu.sHtML

[R70] 时间戳与互转
来源：http://wap.fanxiaobao.xyz/Article/details/gxrowqbwi.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guydssepr.sHtML

[R71] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbduslhkm.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fanxiaobao.xyz/Article/details/gjbeimkzo.sHtML

[R72] 等待端口就绪
来源：http://m.share.fanxiaobao.xyz/Article/details/gtcuygtzp.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsjhgnyoc.sHtML

[R73] 分割大日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gmximerpc.sHtML

split -l 1000 big.log part_
来源：http://read.share.fanxiaobao.xyz/Article/details/gvzrdvpfv.sHtML

[R74] 批量重命名
来源：http://m.share.fanxiaobao.xyz/Article/details/gbqtrslao.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gvnkszpog.sHtML

[R75] 导出环境变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gnzwglboj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqjnplyre.sHtML

[R76] 使用临时文件
来源：http://mobile.fanxiaobao.xyz/Article/details/godfctcig.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gbyjcuqcs.sHtML

[R77] 读取用户输入
来源：http://mobile.fanxiaobao.xyz/Article/details/ghdyjzhhb.sHtML


<!-- 参考信息 -->