代发 wailian999

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.share.hesvh.cn/Article/details/gemxbusid.sHtML

[Q24] 去重
来源：http://baike.zdbjq.cn/Article/details/grvaecatw.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.hesvh.cn/Article/details/ghdggzevb.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.hesvh.cn/Article/details/gjdkhybat.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.zdbjq.cn/Article/details/ghwoevugf.sHtML

[Q26] 计数
来源：http://baike.zdbjq.cn/Article/details/gilscdsjz.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.hesvh.cn/Article/details/gtbgdetkk.sHtML

[Q27] 条件计数
来源：http://baike.zdbjq.cn/Article/details/gixjrostt.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.hesvh.cn/Article/details/gmsgaxsma.sHtML

[Q28] 求和与平均
来源：http://m.share.hesvh.cn/Article/details/gxutvdwfl.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gvtaqxqvi.sHtML

[Q29] 最大最小值
来源：http://3g.zdbjq.cn/Article/details/gjbrpfbgs.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.fehbvm.com/Article/details/gxitccmfb.sHtML

[Q30] 分组统计
来源：http://m.share.hesvh.cn/Article/details/garoyfylq.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gpwspzjpy.sHtML

[Q31] 分组后过滤
来源：http://m.share.zdbjq.cn/Article/details/ghmssblmt.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.fehbvm.com/Article/details/gvvwwykpv.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.zdbjq.cn/Article/details/gbijjgugw.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/ggalyxaen.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.hesvh.cn/Article/details/gsvqffjnr.sHtML

[Q33] 多列分组
来源：http://www.m.share.hesvh.cn/Article/details/gimiobuyi.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.zdbjq.cn/Article/details/gjrtwvzae.sHtML

[Q34] 每组取第一条
来源：http://3g.zdbjq.cn/Article/details/gssbkgeib.sHtML

SELECT * FROM (
来源：http://m.share.zdbjq.cn/Article/details/giojfvtmx.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.fehbvm.com/Article/details/gjkwincys.sHtML

) t WHERE rn = 1;
来源：http://3g.zdbjq.cn/Article/details/ghssblpyk.sHtML

[Q35] 内连接
来源：http://www.share.fehbvm.com/Article/details/gcrzllwpc.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.zdbjq.cn/Article/details/glzvqogyi.sHtML

[Q36] 左连接
来源：http://baike.fehbvm.com/Article/details/gofoeojif.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.hesvh.cn/Article/details/gpmwhdmjd.sHtML

[Q37] 右连接
来源：http://wap.fehbvm.com/Article/details/gewyjnvgv.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.zdbjq.cn/Article/details/ghrogoedq.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.hesvh.cn/Article/details/gysiajiqo.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.hesvh.cn/Article/details/ggudbixor.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.hesvh.cn/Article/details/gatrqpgkw.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://3g.hesvh.cn/Article/details/gqptzsjid.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.zdbjq.cn/Article/details/gfcfgccul.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.zdbjq.cn/Article/details/getzomcwr.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://baike.zdbjq.cn/Article/details/gvpycxpfy.sHtML

[Q41] 多表连接
来源：http://3g.hesvh.cn/Article/details/gkahhffqi.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.zdbjq.cn/Article/details/gbucufttu.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.fehbvm.com/Article/details/gdpseqdej.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.zdbjq.cn/Article/details/gnhvzsezn.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.hesvh.cn/Article/details/gozyfdops.sHtML

SELECT u.name, o.amount FROM users u
来源：http://mobile.hesvh.cn/Article/details/gxxlcgwey.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.zdbjq.cn/Article/details/gedvwmwni.sHtML

[Q43] 标量子查询
来源：http://m.share.hesvh.cn/Article/details/giztmttwz.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.fehbvm.com/Article/details/gcpernthy.sHtML

[Q44] IN 子查询
来源：http://baike.hesvh.cn/Article/details/gdfiyneha.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.hesvh.cn/Article/details/gfxppvgpu.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.fehbvm.com/Article/details/gfgpnbaqw.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.zdbjq.cn/Article/details/gvkztpuuz.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.zdbjq.cn/Article/details/gcwfjsudn.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.zdbjq.cn/Article/details/grzxnalhp.sHtML

[Q47] 与平均值比较
来源：http://3g.zdbjq.cn/Article/details/gquwprnwc.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.fehbvm.com/Article/details/giiioklek.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.fehbvm.com/Article/details/gpzppdyjo.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fehbvm.com/Article/details/guqglplyt.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.fehbvm.com/Article/details/gxrossbrf.sHtML

[Q49] 更新单行
来源：http://mobile.fehbvm.com/Article/details/gtyhjgmgh.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.hesvh.cn/Article/details/gagdbbyqc.sHtML

[Q50] 批量更新
来源：http://www.blog.fehbvm.com/Article/details/grshjfdjj.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fehbvm.com/Article/details/ghsrxeonx.sHtML

[Q51] 用子查询更新
来源：http://read.share.zdbjq.cn/Article/details/gbrogxkyn.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.fehbvm.com/Article/details/gfelfwzrp.sHtML

[Q52] 删除指定行
来源：http://www.blog.fehbvm.com/Article/details/gmvxbwwdz.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.hesvh.cn/Article/details/gqiwblion.sHtML

[Q53] 按条件删除
来源：http://mobile.fehbvm.com/Article/details/gbglyzzui.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.hesvh.cn/Article/details/gymrbzayl.sHtML

[Q54] 清空表
来源：http://wap.hesvh.cn/Article/details/gjpyssoec.sHtML

TRUNCATE TABLE logs;
来源：http://3g.hesvh.cn/Article/details/grpgbzwsz.sHtML

[Q55] 排名（并列占位）
来源：http://blog.fehbvm.com/Article/details/goqwhuzym.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.zdbjq.cn/Article/details/gxljmrwlf.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.hesvh.cn/Article/details/gbcnfrvpc.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.zdbjq.cn/Article/details/gcpcxccjv.sHtML

[Q57] 行号
来源：http://blog.zdbjq.cn/Article/details/gqpeagaaa.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.fehbvm.com/Article/details/gpbtnsbws.sHtML

[Q58] 累计求和
来源：http://mobile.fehbvm.com/Article/details/gbptcdzzk.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gnbaxeacx.sHtML

[Q59] 分组内累计
来源：http://www.blog.hesvh.cn/Article/details/gbaywknjc.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gxyqmgthv.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.hesvh.cn/Article/details/gukwhwsag.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.fehbvm.com/Article/details/gabvbzfyk.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.hesvh.cn/Article/details/gizfhdmis.sHtML

[Q61] 移动平均
来源：http://www.m.share.zdbjq.cn/Article/details/gadhwncvb.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gjmlreugo.sHtML

[Q62] 分组占比
来源：http://www.m.share.zdbjq.cn/Article/details/goyxwnnzb.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/ghmfigrka.sHtML

[Q63] 开启事务
来源：http://wap.hesvh.cn/Article/details/glhebseuk.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.zdbjq.cn/Article/details/ghaxinhfq.sHtML

[Q64] 提交事务
来源：http://read.share.fehbvm.com/Article/details/gadlxzfvv.sHtML

COMMIT;
来源：http://www.blog.fehbvm.com/Article/details/gigsbwlsc.sHtML

[Q65] 回滚事务
来源：http://blog.hesvh.cn/Article/details/grfxmzkqw.sHtML

ROLLBACK;
来源：http://wap.fehbvm.com/Article/details/gjomvgcrg.sHtML

[Q66] 行锁查询
来源：http://www.share.zdbjq.cn/Article/details/gwhqophre.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.fehbvm.com/Article/details/geijjocsm.sHtML

[Q67] 设置隔离级别
来源：http://baike.zdbjq.cn/Article/details/gphqjoewc.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.hesvh.cn/Article/details/goyrrbolh.sHtML

[Q68] 保存点
来源：http://www.m.share.zdbjq.cn/Article/details/gntrbjeip.sHtML

SAVEPOINT sp1;
来源：http://read.share.fehbvm.com/Article/details/ghldgsjai.sHtML

ROLLBACK TO sp1;
来源：http://mobile.hesvh.cn/Article/details/gywuxniyh.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.fehbvm.com/Article/details/glpwnpifb.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.share.fehbvm.com/Article/details/gzvetnnfj.sHtML

[Q70] 更新统计信息
来源：http://www.blog.fehbvm.com/Article/details/gbigkwsam.sHtML

ANALYZE TABLE users;
来源：http://blog.zdbjq.cn/Article/details/gepkfljdl.sHtML

[Q71] 查看建表语句
来源：http://m.share.fehbvm.com/Article/details/gntxabqvp.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.fehbvm.com/Article/details/gmwnswejc.sHtML

[Q72] 查看索引
来源：http://baike.zdbjq.cn/Article/details/gkzjnbiko.sHtML

SHOW INDEX FROM users;
来源：http://www.share.fehbvm.com/Article/details/gmvgdfkdg.sHtML

[Q73] 查看表状态
来源：http://3g.hesvh.cn/Article/details/gynsjcqqq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.hesvh.cn/Article/details/gpdxfvvcs.sHtML

[Q74] 强制使用索引
来源：http://m.share.zdbjq.cn/Article/details/gsreysggg.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.hesvh.cn/Article/details/gkojdafya.sHtML

[Q75] 日期格式化
来源：http://mobile.zdbjq.cn/Article/details/gwhhiebkx.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gwnvprgur.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.zdbjq.cn/Article/details/gnbosfzjw.sHtML

[Q76] 按天统计
来源：http://read.share.hesvh.cn/Article/details/gtnemhrzz.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.fehbvm.com/Article/details/gwoitbymd.sHtML

[Q77] 时间加减
来源：http://www.share.zdbjq.cn/Article/details/gquxoojat.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.hesvh.cn/Article/details/gdmmamzbx.sHtML

[Q78] 当前时间
来源：http://blog.hesvh.cn/Article/details/glwvvuozq.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.zdbjq.cn/Article/details/gzlkfdtzk.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.zdbjq.cn/Article/details/gppkgwije.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.hesvh.cn/Article/details/guhvwgndz.sHtML

[Q80] 字符串截取
来源：http://read.share.fehbvm.com/Article/details/gnaydlozr.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gwnsbsbpc.sHtML

[Q81] 字符串替换
来源：http://www.blog.fehbvm.com/Article/details/gsikrcngv.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gffdeypgp.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.fehbvm.com/Article/details/gpbkofxum.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/goezqkohr.sHtML

[Q83] 大小写转换
来源：http://read.share.hesvh.cn/Article/details/gajkdkugh.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/guhcaucih.sHtML

[Q84] 去除首尾空格
来源：http://3g.zdbjq.cn/Article/details/geyewwahj.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/geqeeokpj.sHtML

[Q85] 数值取整
来源：http://www.m.share.fehbvm.com/Article/details/gpczllmfd.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.hesvh.cn/Article/details/gexweaiie.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.zdbjq.cn/Article/details/gfexfuxrc.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fehbvm.com/Article/details/gtiuekmut.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.zdbjq.cn/Article/details/gluaawbbi.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.zdbjq.cn/Article/details/grvtcmqul.sHtML

[Q88] 行转列（条件聚合）
来源：http://wap.zdbjq.cn/Article/details/gstpmpkga.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.hesvh.cn/Article/details/gghzbuxfd.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fehbvm.com/Article/details/ghoupjwqy.sHtML

[Q89] 判断表是否存在
来源：http://wap.zdbjq.cn/Article/details/gwhbqathw.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.hesvh.cn/Article/details/gnsohfeop.sHtML

[Q90] 生成序号列
来源：http://mobile.zdbjq.cn/Article/details/ggmpesbts.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fehbvm.com/Article/details/ggjbpnyml.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/ggaydotsy.sHtML

R. Bash 专题
来源：http://www.blog.hesvh.cn/Article/details/gazzqofts.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gxgfrbecy.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.hesvh.cn/Article/details/gycpfiftr.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.zdbjq.cn/Article/details/gnrybsqfv.sHtML

set -euo pipefail
来源：http://3g.hesvh.cn/Article/details/ggidipxxi.sHtML

[R02] 变量赋值与使用
来源：http://www.share.zdbjq.cn/Article/details/gpcyetkfn.sHtML

name="Tom"; echo "$name"
来源：http://read.share.hesvh.cn/Article/details/giimwfnfz.sHtML

[R03] 只读变量
来源：http://baike.hesvh.cn/Article/details/grjdibwtd.sHtML

readonly PI=3.14
来源：http://wap.hesvh.cn/Article/details/gtskuglil.sHtML

[R04] 位置参数
来源：http://m.share.zdbjq.cn/Article/details/gsaoyvhll.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.hesvh.cn/Article/details/grmpwfzfj.sHtML

[R05] 参数默认值
来源：http://blog.zdbjq.cn/Article/details/gjtfmbnnb.sHtML

name="${1:-default}"
来源：http://m.share.zdbjq.cn/Article/details/gfdwpzled.sHtML

[R06] 判断命令是否存在
来源：http://blog.zdbjq.cn/Article/details/gqxjkqbum.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/gdiplbgpw.sHtML

[R07] if 判断文件
来源：http://blog.hesvh.cn/Article/details/gnjpgdamz.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.hesvh.cn/Article/details/gwmebqglv.sHtML

[R08] 数值比较
来源：http://mobile.hesvh.cn/Article/details/ghmvxglem.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gqtxeiwuc.sHtML

[R09] 字符串比较
来源：http://m.share.fehbvm.com/Article/details/gwagevfnv.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.hesvh.cn/Article/details/grtpyjpth.sHtML

[R10] 正则匹配
来源：http://wap.zdbjq.cn/Article/details/gbuiqomdj.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.hesvh.cn/Article/details/gfpdnvrux.sHtML

[R11] case 多分支
来源：http://baike.zdbjq.cn/Article/details/gmguzkiht.sHtML

case "$1" in
来源：http://blog.hesvh.cn/Article/details/gfqqsfbts.sHtML

start) echo "启动" ;;
来源：http://wap.zdbjq.cn/Article/details/gatmuaftu.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fehbvm.com/Article/details/gwkzyirig.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.hesvh.cn/Article/details/ggwekjolt.sHtML

esac
来源：http://read.share.hesvh.cn/Article/details/gjgnbrbru.sHtML

[R12] for 遍历文件
来源：http://www.m.share.hesvh.cn/Article/details/gpvufhofw.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fehbvm.com/Article/details/gkrqrqvzn.sHtML

[R13] for 计数循环
来源：http://baike.hesvh.cn/Article/details/gydrjsyjw.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.zdbjq.cn/Article/details/givxbldjk.sHtML

[R14] C 风格 for
来源：http://blog.zdbjq.cn/Article/details/gcpobszki.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.zdbjq.cn/Article/details/glcovtncn.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/glaaqfkqi.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.hesvh.cn/Article/details/gokzophfa.sHtML

[R16] until 等待条件
来源：http://blog.fehbvm.com/Article/details/gfwqyrtwc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fehbvm.com/Article/details/gudifbyft.sHtML

[R17] 数组定义与取值
来源：http://blog.zdbjq.cn/Article/details/gsrdgixmx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fehbvm.com/Article/details/ggilyoalt.sHtML

[R18] 遍历数组
来源：http://m.share.hesvh.cn/Article/details/gsgvnmsxf.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.fehbvm.com/Article/details/gljkevxpd.sHtML

[R19] 数组长度
来源：http://www.m.share.hesvh.cn/Article/details/gczphsapt.sHtML

echo "${#arr[@]}"
来源：http://3g.hesvh.cn/Article/details/gvtadqlvq.sHtML

[R20] 关联数组（字典）
来源：http://m.share.hesvh.cn/Article/details/gbqvmvnym.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.share.fehbvm.com/Article/details/gfernsnnn.sHtML

[R21] 字符串长度
来源：http://www.share.hesvh.cn/Article/details/gtnfjuvgr.sHtML

echo "${#s}"
来源：http://blog.hesvh.cn/Article/details/gtxzmwzan.sHtML

[R22] 截取子串
来源：http://read.share.fehbvm.com/Article/details/gyakksisy.sHtML

echo "${s:0:5}"
来源：http://read.share.fehbvm.com/Article/details/ghrkntffa.sHtML

[R23] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/gmvibdkmb.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.hesvh.cn/Article/details/glihauzth.sHtML

[R24] 大小写转换
来源：http://wap.fehbvm.com/Article/details/gaobocftq.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fehbvm.com/Article/details/ggtqnmlki.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.zdbjq.cn/Article/details/gvnaxchku.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.zdbjq.cn/Article/details/gdlvftmel.sHtML

[R26] 命令替换
来源：http://wap.zdbjq.cn/Article/details/glkbxsedk.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.fehbvm.com/Article/details/gpasuiofu.sHtML

[R27] 算术展开
来源：http://www.share.fehbvm.com/Article/details/gladmpmxh.sHtML

echo $((1 + 2 * 3))
来源：http://blog.zdbjq.cn/Article/details/gcdsliymz.sHtML

[R28] 浮点运算
来源：http://3g.hesvh.cn/Article/details/ghexfecqy.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.zdbjq.cn/Article/details/gygecgkdi.sHtML

[R29] 定义函数
来源：http://baike.fehbvm.com/Article/details/gcnblsydr.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.hesvh.cn/Article/details/gaddbvkmi.sHtML

[R30] 函数返回状态码
来源：http://blog.fehbvm.com/Article/details/gytgljflx.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.zdbjq.cn/Article/details/gzxvnwzhf.sHtML

[R31] 局部变量
来源：http://wap.hesvh.cn/Article/details/glrzoyppm.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.zdbjq.cn/Article/details/gyozquiys.sHtML

[R32] 参数个数校验
来源：http://www.blog.hesvh.cn/Article/details/gpegerhld.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/gfdvqxxty.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.hesvh.cn/Article/details/gyqomdwal.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.zdbjq.cn/Article/details/gqcixyekb.sHtML

[R34] 退出时清理
来源：http://blog.zdbjq.cn/Article/details/gevhjnbyc.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.hesvh.cn/Article/details/gazrszfmn.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fehbvm.com/Article/details/glknigpea.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.hesvh.cn/Article/details/gblhgwwao.sHtML

[R36] 并发执行多个任务
来源：http://www.share.zdbjq.cn/Article/details/gepzrlpnf.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.zdbjq.cn/Article/details/gxwrlqaen.sHtML

[R37] 把输出赋给变量
来源：http://wap.zdbjq.cn/Article/details/gxauaaeeu.sHtML

files=$(ls -1)
来源：http://blog.fehbvm.com/Article/details/gdedojqkv.sHtML

[R38] 管道串联
来源：http://www.share.fehbvm.com/Article/details/guwmmaoyv.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.hesvh.cn/Article/details/gruxgjvlv.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.zdbjq.cn/Article/details/gzwfhnkdd.sHtML

cmd > out.log 2>&1
来源：http://www.blog.hesvh.cn/Article/details/gcujoduyz.sHtML

[R40] 追加写日志
来源：http://www.share.zdbjq.cn/Article/details/gafjkplow.sHtML

echo "log" >> out.log
来源：http://www.m.share.hesvh.cn/Article/details/gnzsmlvjg.sHtML

[R41] 丢弃输出
来源：http://read.share.hesvh.cn/Article/details/gvduwatfw.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.zdbjq.cn/Article/details/gwpetnmuf.sHtML

[R42] 输入重定向
来源：http://www.m.share.hesvh.cn/Article/details/gjinprrlx.sHtML

wc -l < a.txt
来源：http://wap.zdbjq.cn/Article/details/gmomjlwnx.sHtML

[R43] 按名字查找文件
来源：http://m.share.zdbjq.cn/Article/details/gmbltbrsa.sHtML

find . -name "*.log" -type f
来源：http://m.share.hesvh.cn/Article/details/gkkcaejwy.sHtML

[R44] 按修改时间查找
来源：http://read.share.zdbjq.cn/Article/details/galprgvpd.sHtML

find . -mtime -7 -type f
来源：http://m.share.hesvh.cn/Article/details/grfltwdep.sHtML

[R45] 批量删除
来源：http://3g.hesvh.cn/Article/details/gzodonoyh.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.zdbjq.cn/Article/details/ggokjasng.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.hesvh.cn/Article/details/gubeqjjhg.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.zdbjq.cn/Article/details/grlelqtzq.sHtML

[R47] sed 单行替换
来源：http://m.share.hesvh.cn/Article/details/giwissyhp.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.fehbvm.com/Article/details/ggunnsopv.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fehbvm.com/Article/details/gxewzjrnx.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fehbvm.com/Article/details/gwgqbudxq.sHtML

[R49] awk 带条件
来源：http://baike.fehbvm.com/Article/details/gmqkbvcyk.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.hesvh.cn/Article/details/gqvzobxsl.sHtML

[R50] awk 求和
来源：http://www.m.share.hesvh.cn/Article/details/gvttqyqwx.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.hesvh.cn/Article/details/grjhvdlzn.sHtML

[R51] 排序去重取前几
来源：http://3g.zdbjq.cn/Article/details/gujsizgmc.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.hesvh.cn/Article/details/gzvmzkxav.sHtML

[R52] 统计行数
来源：http://wap.zdbjq.cn/Article/details/gdoegajuo.sHtML

wc -l a.txt
来源：http://wap.zdbjq.cn/Article/details/gfndiecry.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.hesvh.cn/Article/details/gpubouzub.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.zdbjq.cn/Article/details/gnhhybrlw.sHtML

[R54] 比较两个文件
来源：http://wap.zdbjq.cn/Article/details/gbmtykbgk.sHtML

diff a.txt b.txt
来源：http://3g.zdbjq.cn/Article/details/gtwqkoqzt.sHtML

[R55] 压缩与解压
来源：http://read.share.hesvh.cn/Article/details/gbvtnoozu.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.share.fehbvm.com/Article/details/gvyctzyhb.sHtML

[R56] 远程拷贝
来源：http://www.blog.zdbjq.cn/Article/details/guizyyhxs.sHtML

scp file user@host:/path/
来源：http://blog.hesvh.cn/Article/details/guzfpqhiu.sHtML

[R57] 远程执行命令
来源：http://wap.zdbjq.cn/Article/details/gllckxtfi.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fehbvm.com/Article/details/gmufgrqdr.sHtML

[R58] 下载文件
来源：http://3g.zdbjq.cn/Article/details/gfebibckv.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fehbvm.com/Article/details/gminuonow.sHtML

[R59] 发 POST JSON
来源：http://blog.zdbjq.cn/Article/details/gbybfjwct.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fehbvm.com/Article/details/gdfgagxbj.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fehbvm.com/Article/details/gxgvtbohp.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fehbvm.com/Article/details/gbiixxrmb.sHtML

[R61] 磁盘占用
来源：http://baike.hesvh.cn/Article/details/guetejzkr.sHtML

df -h;  du -sh *
来源：http://wap.zdbjq.cn/Article/details/gvgrtnvwd.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.zdbjq.cn/Article/details/gmpwzpsmw.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.hesvh.cn/Article/details/ggpwzjfqj.sHtML

[R63] 内存与进程
来源：http://3g.hesvh.cn/Article/details/gdtaxtszc.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.hesvh.cn/Article/details/garfnvnxa.sHtML

[R64] 结束进程
来源：http://www.blog.zdbjq.cn/Article/details/gkuamlszb.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fehbvm.com/Article/details/gcnvsyjpy.sHtML

[R65] 查看端口占用
来源：http://www.share.zdbjq.cn/Article/details/giufqimmi.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.hesvh.cn/Article/details/gbcmuckce.sHtML

[R66] 定时任务
来源：http://m.share.hesvh.cn/Article/details/guckbbosz.sHtML

crontab -e;  crontab -l
来源：http://www.blog.hesvh.cn/Article/details/gvhjlznco.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fehbvm.com/Article/details/gynauezzu.sHtML

openssl rand -hex 16
来源：http://3g.zdbjq.cn/Article/details/gvppjavjf.sHtML

[R68] 计算文件校验值
来源：http://blog.zdbjq.cn/Article/details/ggxweecss.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gcjibakjj.sHtML

[R69] 生成随机密码
来源：http://baike.hesvh.cn/Article/details/grojkuoxx.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.hesvh.cn/Article/details/gemktgxzx.sHtML

[R70] 时间戳与互转
来源：http://m.share.fehbvm.com/Article/details/gesnfiwjw.sHtML

date +%s;  date -d @1700000000
来源：http://blog.fehbvm.com/Article/details/gjuwlfwsx.sHtML

[R71] 日期格式化
来源：http://mobile.zdbjq.cn/Article/details/grgbiosil.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fehbvm.com/Article/details/gtildxqqt.sHtML

[R72] 等待端口就绪
来源：http://3g.fehbvm.com/Article/details/gnobthkgo.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.zdbjq.cn/Article/details/ggounwdio.sHtML

[R73] 分割大日志
来源：http://www.share.hesvh.cn/Article/details/gcdjfjiwc.sHtML


<!-- 参考信息 -->