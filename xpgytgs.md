代发 wailian999

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.hesvh.cn/Article/details/glmomxple.sHtML

[Q26] 计数
来源：http://3g.zdbjq.cn/Article/details/grieklgdd.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gzrgclsvi.sHtML

[Q27] 条件计数
来源：http://blog.fehbvm.com/Article/details/gilyzvdqr.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.zdbjq.cn/Article/details/geaabyidu.sHtML

[Q28] 求和与平均
来源：http://read.share.fehbvm.com/Article/details/ggjynyerc.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/guiaagqkr.sHtML

[Q29] 最大最小值
来源：http://www.blog.hesvh.cn/Article/details/gqdegnjna.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gzymxwojw.sHtML

[Q30] 分组统计
来源：http://www.blog.hesvh.cn/Article/details/gaxrmgruw.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gjzszybsm.sHtML

[Q31] 分组后过滤
来源：http://wap.hesvh.cn/Article/details/gxrxdkvit.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.zdbjq.cn/Article/details/gkrjahzoq.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gtuoibesd.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/gptagsnby.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.hesvh.cn/Article/details/gnuelmlmi.sHtML

[Q33] 多列分组
来源：http://blog.zdbjq.cn/Article/details/gstcgkpwl.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.zdbjq.cn/Article/details/ghairdbuu.sHtML

[Q34] 每组取第一条
来源：http://read.share.zdbjq.cn/Article/details/gzkxbcsyn.sHtML

SELECT * FROM (
来源：http://wap.hesvh.cn/Article/details/gkymjawjs.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.hesvh.cn/Article/details/gdiftausd.sHtML

) t WHERE rn = 1;
来源：http://blog.hesvh.cn/Article/details/gajbdyhet.sHtML

[Q35] 内连接
来源：http://baike.fehbvm.com/Article/details/gziygxxwv.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.zdbjq.cn/Article/details/gdrrchvpn.sHtML

[Q36] 左连接
来源：http://read.share.fehbvm.com/Article/details/gtoeyffds.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.hesvh.cn/Article/details/ghysoicac.sHtML

[Q37] 右连接
来源：http://blog.hesvh.cn/Article/details/gvikupbzr.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.zdbjq.cn/Article/details/gwgaqvhxg.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.zdbjq.cn/Article/details/gawzlihsn.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.hesvh.cn/Article/details/gdlwrrspd.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.zdbjq.cn/Article/details/gdsasyyzw.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.hesvh.cn/Article/details/gmgexdvll.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.zdbjq.cn/Article/details/gveckfilr.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.fehbvm.com/Article/details/glvygjtza.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.hesvh.cn/Article/details/gkmknnawo.sHtML

[Q41] 多表连接
来源：http://www.m.share.fehbvm.com/Article/details/gbqtehyjn.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.fehbvm.com/Article/details/guxnzricg.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.zdbjq.cn/Article/details/gztvzgtaq.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.hesvh.cn/Article/details/grpjihxmu.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.zdbjq.cn/Article/details/gykcvdiir.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.fehbvm.com/Article/details/gdygyaemv.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.fehbvm.com/Article/details/getdiflsf.sHtML

[Q43] 标量子查询
来源：http://read.share.fehbvm.com/Article/details/goalyfyiw.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.zdbjq.cn/Article/details/gwbolkgig.sHtML

[Q44] IN 子查询
来源：http://mobile.hesvh.cn/Article/details/gkoluxkmw.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.fehbvm.com/Article/details/gwygrogll.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.hesvh.cn/Article/details/gxgkybjzx.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.zdbjq.cn/Article/details/gkhvatwij.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.zdbjq.cn/Article/details/gzcinlfzf.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.hesvh.cn/Article/details/gydmatdgx.sHtML

[Q47] 与平均值比较
来源：http://read.share.hesvh.cn/Article/details/glnxirifc.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.zdbjq.cn/Article/details/glhexoowh.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.fehbvm.com/Article/details/ghiootnhm.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.zdbjq.cn/Article/details/gwdpkgolr.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.hesvh.cn/Article/details/gvpeyzeyf.sHtML

[Q49] 更新单行
来源：http://mobile.zdbjq.cn/Article/details/gkagprmnk.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.hesvh.cn/Article/details/gmpvubpfr.sHtML

[Q50] 批量更新
来源：http://www.share.zdbjq.cn/Article/details/grivkhumd.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.zdbjq.cn/Article/details/glqkeslbw.sHtML

[Q51] 用子查询更新
来源：http://m.share.hesvh.cn/Article/details/gyygoduvg.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.hesvh.cn/Article/details/geiytfbmi.sHtML

[Q52] 删除指定行
来源：http://blog.fehbvm.com/Article/details/gidmmhdlq.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.m.share.hesvh.cn/Article/details/ggitsdfqv.sHtML

[Q53] 按条件删除
来源：http://www.m.share.hesvh.cn/Article/details/gwygoiygp.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.zdbjq.cn/Article/details/gmncvagay.sHtML

[Q54] 清空表
来源：http://3g.hesvh.cn/Article/details/grithjqga.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.zdbjq.cn/Article/details/gkzqgggbr.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.fehbvm.com/Article/details/gaolvzejz.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.zdbjq.cn/Article/details/gzwcgmzlp.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.zdbjq.cn/Article/details/gvgrdsdxm.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.fehbvm.com/Article/details/ghhunhxwj.sHtML

[Q57] 行号
来源：http://www.m.share.fehbvm.com/Article/details/gwrpvjbbu.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gpybijyha.sHtML

[Q58] 累计求和
来源：http://read.share.hesvh.cn/Article/details/gzaixwtqm.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gzngxpxwj.sHtML

[Q59] 分组内累计
来源：http://read.share.hesvh.cn/Article/details/gsesuwpom.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gubbeeasn.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.zdbjq.cn/Article/details/gdgsawerx.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.zdbjq.cn/Article/details/gzzespahf.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.hesvh.cn/Article/details/ggwyodajh.sHtML

[Q61] 移动平均
来源：http://www.m.share.fehbvm.com/Article/details/gyvfgqbcu.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gwrvvvnnk.sHtML

[Q62] 分组占比
来源：http://baike.fehbvm.com/Article/details/gviziqgyw.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.zdbjq.cn/Article/details/gjevjmkof.sHtML

[Q63] 开启事务
来源：http://read.share.fehbvm.com/Article/details/gtwapyskp.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.fehbvm.com/Article/details/grptmdtzm.sHtML

[Q64] 提交事务
来源：http://mobile.zdbjq.cn/Article/details/gyhenosly.sHtML

COMMIT;
来源：http://read.share.hesvh.cn/Article/details/ghtxvtukm.sHtML

[Q65] 回滚事务
来源：http://www.blog.zdbjq.cn/Article/details/ghiwlovcq.sHtML

ROLLBACK;
来源：http://read.share.hesvh.cn/Article/details/gydxtjcbc.sHtML

[Q66] 行锁查询
来源：http://m.share.zdbjq.cn/Article/details/ghjyzqfvi.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.zdbjq.cn/Article/details/gbtclbbxn.sHtML

[Q67] 设置隔离级别
来源：http://blog.hesvh.cn/Article/details/guycejofn.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.hesvh.cn/Article/details/gxfeqpjbz.sHtML

[Q68] 保存点
来源：http://blog.fehbvm.com/Article/details/gnkirbvqr.sHtML

SAVEPOINT sp1;
来源：http://www.blog.zdbjq.cn/Article/details/gnqnsbhtl.sHtML

ROLLBACK TO sp1;
来源：http://www.share.zdbjq.cn/Article/details/gmbalewos.sHtML

[Q69] 查看执行计划
来源：http://m.share.hesvh.cn/Article/details/gykwaixis.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.hesvh.cn/Article/details/gvkajpjcf.sHtML

[Q70] 更新统计信息
来源：http://wap.fehbvm.com/Article/details/gxujsuuyh.sHtML

ANALYZE TABLE users;
来源：http://mobile.zdbjq.cn/Article/details/gepqmindh.sHtML

[Q71] 查看建表语句
来源：http://www.blog.zdbjq.cn/Article/details/gkpehhyub.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.zdbjq.cn/Article/details/ggdykixqw.sHtML

[Q72] 查看索引
来源：http://blog.zdbjq.cn/Article/details/gkoztbioq.sHtML

SHOW INDEX FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gkeddrmgm.sHtML

[Q73] 查看表状态
来源：http://www.share.zdbjq.cn/Article/details/gunowduqe.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.hesvh.cn/Article/details/ghbqsywef.sHtML

[Q74] 强制使用索引
来源：http://mobile.hesvh.cn/Article/details/gjgyenqud.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.zdbjq.cn/Article/details/gzcgrexer.sHtML

[Q75] 日期格式化
来源：http://www.share.zdbjq.cn/Article/details/ghxrhsboj.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gvcwxnrdo.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.hesvh.cn/Article/details/gbyuyzary.sHtML

[Q76] 按天统计
来源：http://blog.hesvh.cn/Article/details/gtrdujhyw.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.hesvh.cn/Article/details/gdghjxmue.sHtML

[Q77] 时间加减
来源：http://3g.fehbvm.com/Article/details/ggsrphnnn.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.hesvh.cn/Article/details/giurpakzg.sHtML

[Q78] 当前时间
来源：http://read.share.fehbvm.com/Article/details/ghmlygwnh.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.zdbjq.cn/Article/details/gkucpvmet.sHtML

[Q79] 字符串拼接
来源：http://blog.zdbjq.cn/Article/details/gjpcxyppe.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.zdbjq.cn/Article/details/gecdbaomt.sHtML

[Q80] 字符串截取
来源：http://3g.zdbjq.cn/Article/details/gdqvgeffq.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.hesvh.cn/Article/details/golaxzxql.sHtML

[Q81] 字符串替换
来源：http://read.share.zdbjq.cn/Article/details/gfptcxede.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/guxzvpbbj.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.hesvh.cn/Article/details/gyengodqv.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gzoynrsri.sHtML

[Q83] 大小写转换
来源：http://baike.hesvh.cn/Article/details/gcxolsmmt.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/guqwaneih.sHtML

[Q84] 去除首尾空格
来源：http://www.blog.hesvh.cn/Article/details/gpfioemqi.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gxskfbtsk.sHtML

[Q85] 数值取整
来源：http://www.share.fehbvm.com/Article/details/gkmwjsawp.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.hesvh.cn/Article/details/gemppdlqi.sHtML

[Q86] 读取 JSON 字段
来源：http://read.share.zdbjq.cn/Article/details/ghmxwkarh.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fehbvm.com/Article/details/gtwpvyoda.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.hesvh.cn/Article/details/geztqtkra.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fehbvm.com/Article/details/gcsyvtorm.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.hesvh.cn/Article/details/ghatzmskm.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.hesvh.cn/Article/details/gymafcnrp.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.zdbjq.cn/Article/details/gzzxllzmb.sHtML

[Q89] 判断表是否存在
来源：http://read.share.fehbvm.com/Article/details/gtowhboae.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fehbvm.com/Article/details/gcrajqsls.sHtML

[Q90] 生成序号列
来源：http://read.share.fehbvm.com/Article/details/glqqjafsm.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.fehbvm.com/Article/details/gmechozju.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gpcyyhpiw.sHtML

R. Bash 专题
来源：http://blog.hesvh.cn/Article/details/gehltwhbk.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/glfppkwwq.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.fehbvm.com/Article/details/glllpgrmr.sHtML

#!/usr/bin/env bash
来源：http://baike.fehbvm.com/Article/details/gjldbqsmg.sHtML

set -euo pipefail
来源：http://www.share.fehbvm.com/Article/details/garujvhzm.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fehbvm.com/Article/details/gglmdpaze.sHtML

name="Tom"; echo "$name"
来源：http://www.m.share.hesvh.cn/Article/details/gblbodzir.sHtML

[R03] 只读变量
来源：http://m.share.fehbvm.com/Article/details/gtdyifuzi.sHtML

readonly PI=3.14
来源：http://wap.fehbvm.com/Article/details/gmqigkgml.sHtML

[R04] 位置参数
来源：http://m.share.fehbvm.com/Article/details/grbhvrier.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.fehbvm.com/Article/details/gqwpkuhmr.sHtML

[R05] 参数默认值
来源：http://3g.hesvh.cn/Article/details/grwjxsyrl.sHtML

name="${1:-default}"
来源：http://mobile.zdbjq.cn/Article/details/gozqetbxq.sHtML

[R06] 判断命令是否存在
来源：http://wap.fehbvm.com/Article/details/gixlbukwx.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.zdbjq.cn/Article/details/gtwpkywci.sHtML

[R07] if 判断文件
来源：http://wap.zdbjq.cn/Article/details/gudzcqtiw.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.zdbjq.cn/Article/details/gdseauhsg.sHtML

[R08] 数值比较
来源：http://blog.hesvh.cn/Article/details/grzquazzy.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.fehbvm.com/Article/details/gzwpoqbmy.sHtML

[R09] 字符串比较
来源：http://3g.fehbvm.com/Article/details/gzljcpjgn.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.fehbvm.com/Article/details/gboxhvnbm.sHtML

[R10] 正则匹配
来源：http://3g.zdbjq.cn/Article/details/gqfzdlcfo.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fehbvm.com/Article/details/gtkycgckl.sHtML

[R11] case 多分支
来源：http://m.share.zdbjq.cn/Article/details/gndredafj.sHtML

case "$1" in
来源：http://blog.fehbvm.com/Article/details/gnfmifzea.sHtML

start) echo "启动" ;;
来源：http://www.share.fehbvm.com/Article/details/geecjzmbo.sHtML

stop)  echo "停止" ;;
来源：http://wap.hesvh.cn/Article/details/ggvzkvlwd.sHtML

*)     echo "未知命令" ;;
来源：http://3g.hesvh.cn/Article/details/gmysffcgs.sHtML

esac
来源：http://www.m.share.zdbjq.cn/Article/details/gjwspwwcf.sHtML

[R12] for 遍历文件
来源：http://read.share.hesvh.cn/Article/details/gdskocsoc.sHtML

for f in *.txt; do echo "$f"; done
来源：http://baike.hesvh.cn/Article/details/gegvletdm.sHtML

[R13] for 计数循环
来源：http://www.share.hesvh.cn/Article/details/gihpawnnx.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.hesvh.cn/Article/details/goisqjhjk.sHtML

[R14] C 风格 for
来源：http://3g.hesvh.cn/Article/details/gprjiijry.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.zdbjq.cn/Article/details/gnycxodce.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gcillaize.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fehbvm.com/Article/details/gfkspmrtn.sHtML

[R16] until 等待条件
来源：http://3g.hesvh.cn/Article/details/gfajpekjk.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.hesvh.cn/Article/details/gayksadhl.sHtML

[R17] 数组定义与取值
来源：http://wap.zdbjq.cn/Article/details/gzhdqziij.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.hesvh.cn/Article/details/gcogoredk.sHtML

[R18] 遍历数组
来源：http://www.m.share.fehbvm.com/Article/details/gnzccqhxu.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.hesvh.cn/Article/details/gctfcftck.sHtML

[R19] 数组长度
来源：http://www.m.share.hesvh.cn/Article/details/gtstffsyv.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gdxxgbksm.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.zdbjq.cn/Article/details/gtwnnkmwf.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.fehbvm.com/Article/details/gowjymzqe.sHtML

[R21] 字符串长度
来源：http://wap.hesvh.cn/Article/details/gqvosnhun.sHtML

echo "${#s}"
来源：http://3g.zdbjq.cn/Article/details/gxatkbqyb.sHtML

[R22] 截取子串
来源：http://www.share.hesvh.cn/Article/details/gjowpkfrb.sHtML

echo "${s:0:5}"
来源：http://m.share.hesvh.cn/Article/details/gytgckjfn.sHtML

[R23] 字符串替换
来源：http://m.share.fehbvm.com/Article/details/govwajwhk.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.zdbjq.cn/Article/details/gywihoqpy.sHtML

[R24] 大小写转换
来源：http://3g.zdbjq.cn/Article/details/gqcrtyajk.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fehbvm.com/Article/details/gbkzubgcr.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.zdbjq.cn/Article/details/gzzggvqeb.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.zdbjq.cn/Article/details/gratboloi.sHtML

[R26] 命令替换
来源：http://blog.zdbjq.cn/Article/details/gdvkxohau.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.hesvh.cn/Article/details/ghubxqpia.sHtML

[R27] 算术展开
来源：http://3g.zdbjq.cn/Article/details/ggankbkip.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fehbvm.com/Article/details/gxqdbuxmc.sHtML

[R28] 浮点运算
来源：http://read.share.fehbvm.com/Article/details/gwycdkdtt.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.zdbjq.cn/Article/details/gsfcvoiei.sHtML

[R29] 定义函数
来源：http://www.blog.hesvh.cn/Article/details/gictenmbc.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fehbvm.com/Article/details/gqamsiiap.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gkqzhngkk.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fehbvm.com/Article/details/gackzbwkq.sHtML

[R31] 局部变量
来源：http://www.share.hesvh.cn/Article/details/gwvmrxnkj.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.zdbjq.cn/Article/details/gjxckqdhj.sHtML

[R32] 参数个数校验
来源：http://www.m.share.zdbjq.cn/Article/details/gjdotlvkp.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fehbvm.com/Article/details/gswhzssti.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.zdbjq.cn/Article/details/gombuunky.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fehbvm.com/Article/details/grjffgadf.sHtML

[R34] 退出时清理
来源：http://mobile.zdbjq.cn/Article/details/gstabrwob.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.zdbjq.cn/Article/details/gwquaqlux.sHtML

[R35] 后台执行并等待
来源：http://baike.zdbjq.cn/Article/details/gllbqaytt.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.hesvh.cn/Article/details/grqqukcld.sHtML

[R36] 并发执行多个任务
来源：http://blog.fehbvm.com/Article/details/ghorxxbtz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.hesvh.cn/Article/details/gbrsbhgkw.sHtML

[R37] 把输出赋给变量
来源：http://baike.hesvh.cn/Article/details/glwfhdvqp.sHtML

files=$(ls -1)
来源：http://wap.zdbjq.cn/Article/details/gntnbosxy.sHtML

[R38] 管道串联
来源：http://m.share.hesvh.cn/Article/details/gofrbdycy.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.hesvh.cn/Article/details/gmcafhrgr.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.hesvh.cn/Article/details/gnggrslvy.sHtML

cmd > out.log 2>&1
来源：http://www.blog.hesvh.cn/Article/details/gayxcibkm.sHtML

[R40] 追加写日志
来源：http://blog.hesvh.cn/Article/details/gavpcxgpi.sHtML

echo "log" >> out.log
来源：http://www.share.fehbvm.com/Article/details/giptqbyjn.sHtML

[R41] 丢弃输出
来源：http://www.blog.hesvh.cn/Article/details/gzbzdbgcv.sHtML

cmd >/dev/null 2>&1
来源：http://blog.fehbvm.com/Article/details/gnwohrtea.sHtML

[R42] 输入重定向
来源：http://m.share.fehbvm.com/Article/details/gzbgfntnr.sHtML

wc -l < a.txt
来源：http://baike.hesvh.cn/Article/details/gxzhqzvaf.sHtML

[R43] 按名字查找文件
来源：http://m.share.zdbjq.cn/Article/details/ghrhfhejr.sHtML

find . -name "*.log" -type f
来源：http://3g.hesvh.cn/Article/details/gvsycvhjt.sHtML

[R44] 按修改时间查找
来源：http://blog.fehbvm.com/Article/details/gplahufnx.sHtML

find . -mtime -7 -type f
来源：http://mobile.fehbvm.com/Article/details/gidcmbnyj.sHtML

[R45] 批量删除
来源：http://wap.zdbjq.cn/Article/details/gmxdorgwp.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.hesvh.cn/Article/details/gksrcoxoq.sHtML

[R46] 递归替换文件内容
来源：http://wap.fehbvm.com/Article/details/glzrharqt.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.hesvh.cn/Article/details/ggzsahhbz.sHtML

[R47] sed 单行替换
来源：http://www.blog.fehbvm.com/Article/details/gbkporzaw.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.hesvh.cn/Article/details/gkipnskrw.sHtML

[R48] awk 取指定列
来源：http://blog.zdbjq.cn/Article/details/gqyiqgayn.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.zdbjq.cn/Article/details/ggbgurkqd.sHtML

[R49] awk 带条件
来源：http://www.blog.fehbvm.com/Article/details/gvytdphla.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.zdbjq.cn/Article/details/gfhqlslvo.sHtML

[R50] awk 求和
来源：http://www.blog.hesvh.cn/Article/details/ghxofnplo.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gwjtenfrp.sHtML

[R51] 排序去重取前几
来源：http://blog.fehbvm.com/Article/details/gdxxxxefr.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fehbvm.com/Article/details/gabqwqtwb.sHtML

[R52] 统计行数
来源：http://www.share.zdbjq.cn/Article/details/gufbtwhlo.sHtML

wc -l a.txt
来源：http://m.share.hesvh.cn/Article/details/gjjpehfky.sHtML

[R53] 查看文件头与实时尾
来源：http://m.share.fehbvm.com/Article/details/gvlyueotg.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.fehbvm.com/Article/details/gokrazbff.sHtML

[R54] 比较两个文件
来源：http://blog.zdbjq.cn/Article/details/gpvhlbwad.sHtML

diff a.txt b.txt
来源：http://read.share.hesvh.cn/Article/details/gzxdipeyo.sHtML

[R55] 压缩与解压
来源：http://www.share.hesvh.cn/Article/details/gcupsihrq.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.zdbjq.cn/Article/details/gthaxffma.sHtML

[R56] 远程拷贝
来源：http://www.share.fehbvm.com/Article/details/gwuetfssz.sHtML

scp file user@host:/path/
来源：http://3g.hesvh.cn/Article/details/gabwaktue.sHtML

[R57] 远程执行命令
来源：http://blog.fehbvm.com/Article/details/gtzaxyrbi.sHtML

ssh user@host 'uptime'
来源：http://read.share.zdbjq.cn/Article/details/gnesakpfj.sHtML

[R58] 下载文件
来源：http://blog.zdbjq.cn/Article/details/gelmxvtkk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.zdbjq.cn/Article/details/gsqzpqjai.sHtML

[R59] 发 POST JSON
来源：http://3g.hesvh.cn/Article/details/gwgukgkgw.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.zdbjq.cn/Article/details/gzugmqmyv.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.hesvh.cn/Article/details/gboclqhia.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.zdbjq.cn/Article/details/gnphnxpom.sHtML

[R61] 磁盘占用
来源：http://www.blog.fehbvm.com/Article/details/gtrcdxxed.sHtML

df -h;  du -sh *
来源：http://m.share.zdbjq.cn/Article/details/gjuyvrxpb.sHtML

[R62] 找最占空间的文件
来源：http://m.share.fehbvm.com/Article/details/gwmemzfoj.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.zdbjq.cn/Article/details/gdbjlknpv.sHtML

[R63] 内存与进程
来源：http://www.blog.fehbvm.com/Article/details/gcqiwlbgp.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.hesvh.cn/Article/details/gvvbxizol.sHtML

[R64] 结束进程
来源：http://m.share.fehbvm.com/Article/details/gsulmutjc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.zdbjq.cn/Article/details/gtuzsrrwe.sHtML

[R65] 查看端口占用
来源：http://read.share.hesvh.cn/Article/details/gpqmsjxky.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fehbvm.com/Article/details/gqmvwcrpu.sHtML

[R66] 定时任务
来源：http://mobile.zdbjq.cn/Article/details/gfrsvovwb.sHtML

crontab -e;  crontab -l
来源：http://m.share.zdbjq.cn/Article/details/goqnmggpg.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.zdbjq.cn/Article/details/gtviimabm.sHtML

openssl rand -hex 16
来源：http://mobile.zdbjq.cn/Article/details/gqikdqsav.sHtML

[R68] 计算文件校验值
来源：http://www.share.zdbjq.cn/Article/details/gtsvjizpl.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fehbvm.com/Article/details/gexqatewu.sHtML

[R69] 生成随机密码
来源：http://read.share.hesvh.cn/Article/details/gxxslmjai.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.hesvh.cn/Article/details/gfcxfjvvg.sHtML

[R70] 时间戳与互转
来源：http://read.share.zdbjq.cn/Article/details/grdrfflir.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fehbvm.com/Article/details/ghglshmxt.sHtML

[R71] 日期格式化
来源：http://blog.hesvh.cn/Article/details/gkgrbgwmb.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fehbvm.com/Article/details/gophpxbei.sHtML

[R72] 等待端口就绪
来源：http://3g.hesvh.cn/Article/details/gurvbypzv.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fehbvm.com/Article/details/glsvsrpxc.sHtML

[R73] 分割大日志
来源：http://baike.hesvh.cn/Article/details/gkxzkmgqv.sHtML

split -l 1000 big.log part_
来源：http://www.share.hesvh.cn/Article/details/gtxakutal.sHtML

[R74] 批量重命名
来源：http://www.blog.hesvh.cn/Article/details/gmyedyjgo.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.hesvh.cn/Article/details/gsgsfdnwk.sHtML

[R75] 导出环境变量
来源：http://m.share.hesvh.cn/Article/details/ggsahizwn.sHtML


<!-- 参考信息 -->