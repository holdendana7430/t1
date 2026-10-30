代发 wailian999

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.fanxiaobao.xyz/Article/details/giewldbpc.sHtML

[Q26] 计数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gktewivki.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gksfcjepe.sHtML

[Q27] 条件计数
来源：http://wap.fanxiaobao.xyz/Article/details/gteykuvad.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gumvgersc.sHtML

[Q28] 求和与平均
来源：http://mobile.fanxiaobao.xyz/Article/details/ggpjaockc.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gchlwxxti.sHtML

[Q29] 最大最小值
来源：http://m.share.fanxiaobao.xyz/Article/details/gidwvbbjv.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqztclvpn.sHtML

[Q30] 分组统计
来源：http://mobile.fanxiaobao.xyz/Article/details/gqpnyhbnd.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.fanxiaobao.xyz/Article/details/gqnimkusv.sHtML

[Q31] 分组后过滤
来源：http://baike.fanxiaobao.xyz/Article/details/gpippvbch.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfeioxqeo.sHtML

[Q32] 分组拼接字符串
来源：http://baike.fanxiaobao.xyz/Article/details/grdggteoy.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.fanxiaobao.xyz/Article/details/gtrqpxekc.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.fanxiaobao.xyz/Article/details/gvtomsbwx.sHtML

[Q33] 多列分组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmjrixmev.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://wap.fanxiaobao.xyz/Article/details/gjscynyvi.sHtML

[Q34] 每组取第一条
来源：http://www.share.fanxiaobao.xyz/Article/details/ggujulmvn.sHtML

SELECT * FROM (
来源：http://www.share.fanxiaobao.xyz/Article/details/gshzogugl.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.fanxiaobao.xyz/Article/details/getmponbt.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxtcdxfdj.sHtML

[Q35] 内连接
来源：http://blog.fanxiaobao.xyz/Article/details/gpqwiwtlt.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaznjujog.sHtML

[Q36] 左连接
来源：http://blog.fanxiaobao.xyz/Article/details/gkzgtrxjq.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpwmebwam.sHtML

[Q37] 右连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gulfibvll.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fanxiaobao.xyz/Article/details/guonnydrd.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.fanxiaobao.xyz/Article/details/gsadntrdt.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.fanxiaobao.xyz/Article/details/gpxdxrfyy.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.fanxiaobao.xyz/Article/details/gvtqsnaks.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnpvenbzk.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gygragtbi.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxyggxcee.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.fanxiaobao.xyz/Article/details/gudqtlcfn.sHtML

[Q41] 多表连接
来源：http://mobile.fanxiaobao.xyz/Article/details/gwdegqjeu.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjzjzmctd.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.fanxiaobao.xyz/Article/details/gsrpqphzh.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.fanxiaobao.xyz/Article/details/gagjzrfwq.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/givfgguqm.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzwgcujif.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.fanxiaobao.xyz/Article/details/gjjfosjiq.sHtML

[Q43] 标量子查询
来源：http://read.share.fanxiaobao.xyz/Article/details/glgrhjius.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.fanxiaobao.xyz/Article/details/gokbucucg.sHtML

[Q44] IN 子查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwotczsak.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.share.fanxiaobao.xyz/Article/details/gvnslqjhz.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.fanxiaobao.xyz/Article/details/gofcnrayh.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fanxiaobao.xyz/Article/details/gbqlhpqya.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcslvztjf.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fanxiaobao.xyz/Article/details/geqqhunkj.sHtML

[Q47] 与平均值比较
来源：http://wap.fanxiaobao.xyz/Article/details/gcxivirhj.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.fanxiaobao.xyz/Article/details/gkvdnchkh.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghthnpzsc.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.fanxiaobao.xyz/Article/details/gfxjguprp.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://baike.fanxiaobao.xyz/Article/details/gsvgxguvq.sHtML

[Q49] 更新单行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpjoejzft.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmdkoyozs.sHtML

[Q50] 批量更新
来源：http://wap.fanxiaobao.xyz/Article/details/grgruoyhm.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.fanxiaobao.xyz/Article/details/gqnnxpvzs.sHtML

[Q51] 用子查询更新
来源：http://www.blog.fanxiaobao.xyz/Article/details/grgrfeeeh.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gcwqbqwoa.sHtML

[Q52] 删除指定行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpeexwtsk.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gzkywwmcm.sHtML

[Q53] 按条件删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyvlgqzyy.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.fanxiaobao.xyz/Article/details/gzjgnbtch.sHtML

[Q54] 清空表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkulottvs.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fanxiaobao.xyz/Article/details/gixkzhszu.sHtML

[Q55] 排名（并列占位）
来源：http://baike.fanxiaobao.xyz/Article/details/gqexqwueo.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqlmwtpvs.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxkbqajfz.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.fanxiaobao.xyz/Article/details/gijtgzdba.sHtML

[Q57] 行号
来源：http://blog.fanxiaobao.xyz/Article/details/gbcyqidqi.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/glivngyie.sHtML

[Q58] 累计求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gvldrjivl.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/ggcpnbgbi.sHtML

[Q59] 分组内累计
来源：http://www.share.fanxiaobao.xyz/Article/details/gmwbuhclx.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwhigwayd.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.fanxiaobao.xyz/Article/details/goitdqopt.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.fanxiaobao.xyz/Article/details/gtoxdeswm.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbxuopyqv.sHtML

[Q61] 移动平均
来源：http://www.blog.fanxiaobao.xyz/Article/details/guoevhwte.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/grnessymt.sHtML

[Q62] 分组占比
来源：http://m.share.fanxiaobao.xyz/Article/details/gyzwspicz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.fanxiaobao.xyz/Article/details/gsmvfeiko.sHtML

[Q63] 开启事务
来源：http://3g.fanxiaobao.xyz/Article/details/gbedbjjej.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.fanxiaobao.xyz/Article/details/gkubfppwe.sHtML

[Q64] 提交事务
来源：http://baike.fanxiaobao.xyz/Article/details/gjcubbwdo.sHtML

COMMIT;
来源：http://read.share.fanxiaobao.xyz/Article/details/guxmovsqw.sHtML

[Q65] 回滚事务
来源：http://3g.fanxiaobao.xyz/Article/details/gxqnburzr.sHtML

ROLLBACK;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmrxqwkvn.sHtML

[Q66] 行锁查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gljprqvcr.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.fanxiaobao.xyz/Article/details/gsenpldbn.sHtML

[Q67] 设置隔离级别
来源：http://blog.fanxiaobao.xyz/Article/details/gxtfadani.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://blog.fanxiaobao.xyz/Article/details/gggudokld.sHtML

[Q68] 保存点
来源：http://m.share.fanxiaobao.xyz/Article/details/gxaapqoin.sHtML

SAVEPOINT sp1;
来源：http://mobile.fanxiaobao.xyz/Article/details/grvocvcff.sHtML

ROLLBACK TO sp1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gctdrlbjg.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtbtmvfce.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.fanxiaobao.xyz/Article/details/gepakcnnl.sHtML

[Q70] 更新统计信息
来源：http://blog.fanxiaobao.xyz/Article/details/gozkzbqwh.sHtML

ANALYZE TABLE users;
来源：http://baike.fanxiaobao.xyz/Article/details/gjjmtyddg.sHtML

[Q71] 查看建表语句
来源：http://baike.fanxiaobao.xyz/Article/details/glpxvwfgm.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.fanxiaobao.xyz/Article/details/gfmjujryd.sHtML

[Q72] 查看索引
来源：http://mobile.fanxiaobao.xyz/Article/details/ggtjizysc.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/guwqnsxgv.sHtML

[Q73] 查看表状态
来源：http://mobile.fanxiaobao.xyz/Article/details/gucsdlkmh.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.fanxiaobao.xyz/Article/details/gyooslypc.sHtML

[Q74] 强制使用索引
来源：http://3g.fanxiaobao.xyz/Article/details/gwtzyiuje.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.fanxiaobao.xyz/Article/details/gvsvdlcme.sHtML

[Q75] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gpejlcdpt.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/ghrdyaecx.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.fanxiaobao.xyz/Article/details/gtqwgnzcl.sHtML

[Q76] 按天统计
来源：http://m.share.fanxiaobao.xyz/Article/details/gebkhmsfm.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxpwrqetx.sHtML

[Q77] 时间加减
来源：http://wap.fanxiaobao.xyz/Article/details/gxaiqmlrj.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fanxiaobao.xyz/Article/details/gsdlvpfqj.sHtML

[Q78] 当前时间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcmuebuuy.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.fanxiaobao.xyz/Article/details/gmigpmkkd.sHtML

[Q79] 字符串拼接
来源：http://baike.fanxiaobao.xyz/Article/details/gnaxjvplv.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcbfdmieo.sHtML

[Q80] 字符串截取
来源：http://blog.fanxiaobao.xyz/Article/details/gqxvlsosd.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gfexrzsoa.sHtML

[Q81] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gyeicxune.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmucrbala.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.fanxiaobao.xyz/Article/details/gvbcolqym.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnwdpqxka.sHtML

[Q83] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gkoqgtfyp.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gjbpaaoii.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fanxiaobao.xyz/Article/details/gymtcuedj.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gbbkqgcad.sHtML

[Q85] 数值取整
来源：http://www.blog.fanxiaobao.xyz/Article/details/gakcdpfll.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.fanxiaobao.xyz/Article/details/gytssknuu.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fanxiaobao.xyz/Article/details/ganbkzymk.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fanxiaobao.xyz/Article/details/gqnqkftwl.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fanxiaobao.xyz/Article/details/gkqstkmxx.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjqudslfu.sHtML

[Q88] 行转列（条件聚合）
来源：http://m.share.fanxiaobao.xyz/Article/details/gjgpditkx.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fanxiaobao.xyz/Article/details/gwxovjyby.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/giahsgqjh.sHtML

[Q89] 判断表是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/glkjoilor.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.fanxiaobao.xyz/Article/details/gzejlhswx.sHtML

[Q90] 生成序号列
来源：http://m.share.fanxiaobao.xyz/Article/details/gentednkc.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fanxiaobao.xyz/Article/details/gmppmnnbq.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/grgviolxd.sHtML

R. Bash 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/grqqvxkpz.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gvlukhdmw.sHtML

[R01] shebang 与严格模式
来源：http://baike.fanxiaobao.xyz/Article/details/gxcisrzud.sHtML

#!/usr/bin/env bash
来源：http://read.share.fanxiaobao.xyz/Article/details/gpcrkelsh.sHtML

set -euo pipefail
来源：http://m.share.fanxiaobao.xyz/Article/details/gfdhsxpuf.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fanxiaobao.xyz/Article/details/guyibenpi.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fanxiaobao.xyz/Article/details/gdazeotjp.sHtML

[R03] 只读变量
来源：http://3g.fanxiaobao.xyz/Article/details/gvlqgmopk.sHtML

readonly PI=3.14
来源：http://blog.fanxiaobao.xyz/Article/details/gvicehpof.sHtML

[R04] 位置参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gpiotcjvc.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.fanxiaobao.xyz/Article/details/gkvarndgb.sHtML

[R05] 参数默认值
来源：http://m.share.fanxiaobao.xyz/Article/details/gwtcndqaz.sHtML

name="${1:-default}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gtfytlife.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gyqskymtj.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/godtmuhjg.sHtML

[R07] if 判断文件
来源：http://mobile.fanxiaobao.xyz/Article/details/glczirqbh.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gpxhwddra.sHtML

[R08] 数值比较
来源：http://baike.fanxiaobao.xyz/Article/details/gzbokllde.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gvpikawfq.sHtML

[R09] 字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gvfadhaew.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gowdlglgn.sHtML

[R10] 正则匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvbiqyfii.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/ggptpzgza.sHtML

[R11] case 多分支
来源：http://www.blog.fanxiaobao.xyz/Article/details/gabcliign.sHtML

case "$1" in
来源：http://m.share.fanxiaobao.xyz/Article/details/gwhfgzrmj.sHtML

start) echo "启动" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbqtuwokc.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxxfhfwgn.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gvlfwdrnp.sHtML

esac
来源：http://m.share.fanxiaobao.xyz/Article/details/gmzpntryo.sHtML

[R12] for 遍历文件
来源：http://www.share.fanxiaobao.xyz/Article/details/ggcicdwve.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.fanxiaobao.xyz/Article/details/glmeoenvr.sHtML

[R13] for 计数循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdbxoxkqd.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gizjfsdnh.sHtML

[R14] C 风格 for
来源：http://wap.fanxiaobao.xyz/Article/details/gnkkqjheb.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gedghckub.sHtML

[R15] while 逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gkmwpfnln.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/giywenked.sHtML

[R16] until 等待条件
来源：http://wap.fanxiaobao.xyz/Article/details/gyzduqgdg.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/grwhvlquw.sHtML

[R17] 数组定义与取值
来源：http://baike.fanxiaobao.xyz/Article/details/gmttfiuqd.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fanxiaobao.xyz/Article/details/ggnvuqwjd.sHtML

[R18] 遍历数组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grqzmpnqw.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gudeiiwxm.sHtML

[R19] 数组长度
来源：http://wap.fanxiaobao.xyz/Article/details/gdfnhkmka.sHtML

echo "${#arr[@]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gqwdypctq.sHtML

[R20] 关联数组（字典）
来源：http://wap.fanxiaobao.xyz/Article/details/gfmtuxowe.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdtgdlexh.sHtML

[R21] 字符串长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gqcjvxwws.sHtML

echo "${#s}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gvmursqvh.sHtML

[R22] 截取子串
来源：http://3g.fanxiaobao.xyz/Article/details/grgdyydrd.sHtML

echo "${s:0:5}"
来源：http://wap.fanxiaobao.xyz/Article/details/gwokneoof.sHtML

[R23] 字符串替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gyxkfpnrj.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fanxiaobao.xyz/Article/details/ggomajnyt.sHtML

[R24] 大小写转换
来源：http://m.share.fanxiaobao.xyz/Article/details/glnqktjbf.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gcpyziuuu.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fanxiaobao.xyz/Article/details/gljtmeekv.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gnqlprrfd.sHtML

[R26] 命令替换
来源：http://3g.fanxiaobao.xyz/Article/details/gmouhyeen.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fanxiaobao.xyz/Article/details/gijxozzsg.sHtML

[R27] 算术展开
来源：http://mobile.fanxiaobao.xyz/Article/details/gcstjnqvg.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fanxiaobao.xyz/Article/details/gwifvgaou.sHtML

[R28] 浮点运算
来源：http://mobile.fanxiaobao.xyz/Article/details/gnbccwnyu.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fanxiaobao.xyz/Article/details/gqspisyys.sHtML

[R29] 定义函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gnkfhwdjd.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gbugwuwvz.sHtML

[R30] 函数返回状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gbafijaaj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fanxiaobao.xyz/Article/details/ghmxphjpy.sHtML

[R31] 局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gidwjcknm.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gzyxdhgpq.sHtML

[R32] 参数个数校验
来源：http://www.share.fanxiaobao.xyz/Article/details/ggrwcfxmi.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gecnnctsh.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxohffwno.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fanxiaobao.xyz/Article/details/gathjrfaj.sHtML

[R34] 退出时清理
来源：http://www.share.fanxiaobao.xyz/Article/details/gauodybhv.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/grnjkccnu.sHtML

[R35] 后台执行并等待
来源：http://blog.fanxiaobao.xyz/Article/details/gasatwxsb.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fanxiaobao.xyz/Article/details/gujikemig.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gccwcaafm.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fanxiaobao.xyz/Article/details/gtqyxrbty.sHtML

[R37] 把输出赋给变量
来源：http://baike.fanxiaobao.xyz/Article/details/gknwedkzs.sHtML

files=$(ls -1)
来源：http://blog.fanxiaobao.xyz/Article/details/gnxgklfob.sHtML

[R38] 管道串联
来源：http://mobile.fanxiaobao.xyz/Article/details/gewyjlnai.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fanxiaobao.xyz/Article/details/gorryxrkv.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fanxiaobao.xyz/Article/details/gyafchfxa.sHtML

cmd > out.log 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gepqejsnt.sHtML

[R40] 追加写日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxzkzqqvs.sHtML

echo "log" >> out.log
来源：http://blog.fanxiaobao.xyz/Article/details/gmuuwwwzr.sHtML

[R41] 丢弃输出
来源：http://3g.fanxiaobao.xyz/Article/details/ghxonuzgf.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gdqiqzsoh.sHtML

[R42] 输入重定向
来源：http://wap.fanxiaobao.xyz/Article/details/gevqmwkrk.sHtML

wc -l < a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/glfhtwzfm.sHtML

[R43] 按名字查找文件
来源：http://blog.fanxiaobao.xyz/Article/details/geveehnzn.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggopsfunt.sHtML

[R44] 按修改时间查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gjjcdtavx.sHtML

find . -mtime -7 -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gliggqiyw.sHtML

[R45] 批量删除
来源：http://blog.fanxiaobao.xyz/Article/details/gnlwjobss.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fanxiaobao.xyz/Article/details/gjmyplesx.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fanxiaobao.xyz/Article/details/grghnqbeg.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fanxiaobao.xyz/Article/details/gevoziyys.sHtML

[R47] sed 单行替换
来源：http://3g.fanxiaobao.xyz/Article/details/gpzlxajze.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsjidmxiw.sHtML

[R48] awk 取指定列
来源：http://wap.fanxiaobao.xyz/Article/details/gtvexdsgu.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gbtvdbriz.sHtML

[R49] awk 带条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gsektseia.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fanxiaobao.xyz/Article/details/gyrofzmww.sHtML

[R50] awk 求和
来源：http://blog.fanxiaobao.xyz/Article/details/gltthpodd.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gmxtyklhl.sHtML

[R51] 排序去重取前几
来源：http://read.share.fanxiaobao.xyz/Article/details/geslggsmg.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fanxiaobao.xyz/Article/details/ggyyzqtvy.sHtML

[R52] 统计行数
来源：http://www.share.fanxiaobao.xyz/Article/details/gpwzabphr.sHtML

wc -l a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gkbfpcrwy.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsfmkqzxn.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwpqydmek.sHtML

[R54] 比较两个文件
来源：http://wap.fanxiaobao.xyz/Article/details/gemeuqlko.sHtML

diff a.txt b.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grtxfxcts.sHtML

[R55] 压缩与解压
来源：http://blog.fanxiaobao.xyz/Article/details/gitlaxvuw.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fanxiaobao.xyz/Article/details/gkuhczhza.sHtML

[R56] 远程拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/glftfbyeb.sHtML

scp file user@host:/path/
来源：http://m.share.fanxiaobao.xyz/Article/details/garxdrpfp.sHtML

[R57] 远程执行命令
来源：http://wap.fanxiaobao.xyz/Article/details/guuhbdjwv.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gublpfjek.sHtML

[R58] 下载文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gplfijpky.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fanxiaobao.xyz/Article/details/gkrfolsis.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/gumcbmzlj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fanxiaobao.xyz/Article/details/gjqlpxrby.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gvlgksdin.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fanxiaobao.xyz/Article/details/ghscdghok.sHtML

[R61] 磁盘占用
来源：http://3g.fanxiaobao.xyz/Article/details/gomgcyzwx.sHtML

df -h;  du -sh *
来源：http://read.share.fanxiaobao.xyz/Article/details/gilcelwuo.sHtML

[R62] 找最占空间的文件
来源：http://3g.fanxiaobao.xyz/Article/details/glzqhrlit.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fanxiaobao.xyz/Article/details/gleoijkmd.sHtML

[R63] 内存与进程
来源：http://3g.fanxiaobao.xyz/Article/details/gdkjsqwyo.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fanxiaobao.xyz/Article/details/guppqmsrs.sHtML

[R64] 结束进程
来源：http://wap.fanxiaobao.xyz/Article/details/gleijcexy.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fanxiaobao.xyz/Article/details/gpcurshci.sHtML

[R65] 查看端口占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gdbjjnctz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fanxiaobao.xyz/Article/details/gyxtifmqz.sHtML

[R66] 定时任务
来源：http://mobile.fanxiaobao.xyz/Article/details/gkiebuqzw.sHtML

crontab -e;  crontab -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gpiuiilzt.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fanxiaobao.xyz/Article/details/gcpyojtjx.sHtML

openssl rand -hex 16
来源：http://3g.fanxiaobao.xyz/Article/details/gsblqrhhj.sHtML

[R68] 计算文件校验值
来源：http://read.share.fanxiaobao.xyz/Article/details/gvecycgss.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gmypcklvd.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdnuybrug.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fanxiaobao.xyz/Article/details/gheyvuwpu.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grvnokotr.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqeatzmzi.sHtML

[R71] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gjbnytlts.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fanxiaobao.xyz/Article/details/guxadwogm.sHtML

[R72] 等待端口就绪
来源：http://baike.fanxiaobao.xyz/Article/details/gcpotvnvf.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geqngqpkg.sHtML

[R73] 分割大日志
来源：http://3g.fanxiaobao.xyz/Article/details/gyfffmyej.sHtML

split -l 1000 big.log part_
来源：http://3g.fanxiaobao.xyz/Article/details/gxeczbgyl.sHtML

[R74] 批量重命名
来源：http://mobile.fanxiaobao.xyz/Article/details/ghzvvkgmc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gidmdnpdx.sHtML

[R75] 导出环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/gckmsxmev.sHtML


<!-- 参考信息 -->