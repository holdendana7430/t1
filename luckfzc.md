代发 wailian999

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://blog.hesvh.cn/Article/details/gpgpajgbc.sHtML

[Q24] 去重
来源：http://3g.hesvh.cn/Article/details/gtbtuevao.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gjwdmxflp.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.zdbjq.cn/Article/details/gwmytvmdx.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.hesvh.cn/Article/details/glrnlsdkn.sHtML

[Q26] 计数
来源：http://m.share.fehbvm.com/Article/details/gsnavmsmo.sHtML

SELECT COUNT(*) FROM users;
来源：http://blog.fehbvm.com/Article/details/gomcraozz.sHtML

[Q27] 条件计数
来源：http://3g.zdbjq.cn/Article/details/gxyqkkrhq.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.fehbvm.com/Article/details/gwkniejnd.sHtML

[Q28] 求和与平均
来源：http://baike.zdbjq.cn/Article/details/gzihlaygv.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gculieikh.sHtML

[Q29] 最大最小值
来源：http://blog.zdbjq.cn/Article/details/gxfrkfack.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://wap.zdbjq.cn/Article/details/geflnnodu.sHtML

[Q30] 分组统计
来源：http://3g.hesvh.cn/Article/details/grmcoemzi.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/gdjfitotn.sHtML

[Q31] 分组后过滤
来源：http://blog.fehbvm.com/Article/details/gryxngqqg.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.zdbjq.cn/Article/details/gnhntpgal.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.fehbvm.com/Article/details/gpmbrxtug.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/gaiqtveuc.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.zdbjq.cn/Article/details/gearqikze.sHtML

[Q33] 多列分组
来源：http://mobile.zdbjq.cn/Article/details/gnrchlzby.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.fehbvm.com/Article/details/gifezjwqc.sHtML

[Q34] 每组取第一条
来源：http://blog.fehbvm.com/Article/details/gmmbdtkcj.sHtML

SELECT * FROM (
来源：http://www.m.share.hesvh.cn/Article/details/gczbbreqy.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.fehbvm.com/Article/details/gtpkmwxms.sHtML

) t WHERE rn = 1;
来源：http://baike.hesvh.cn/Article/details/gtwxxzbzj.sHtML

[Q35] 内连接
来源：http://blog.hesvh.cn/Article/details/gtqfzkbkh.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.zdbjq.cn/Article/details/gxulzutek.sHtML

[Q36] 左连接
来源：http://www.m.share.zdbjq.cn/Article/details/gjmzljwbl.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.hesvh.cn/Article/details/gfffcpirp.sHtML

[Q37] 右连接
来源：http://read.share.fehbvm.com/Article/details/gliiulsag.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.zdbjq.cn/Article/details/ghvdtpcnj.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.hesvh.cn/Article/details/gutshacud.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gzgogztaq.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.hesvh.cn/Article/details/guptmieus.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.fehbvm.com/Article/details/gykwatovu.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://blog.hesvh.cn/Article/details/gjmkcgxgf.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.fehbvm.com/Article/details/gfxmulevl.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.zdbjq.cn/Article/details/gfrgwjopp.sHtML

[Q41] 多表连接
来源：http://read.share.zdbjq.cn/Article/details/gbexrukdc.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.zdbjq.cn/Article/details/gidoroyag.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.hesvh.cn/Article/details/gocqievti.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.zdbjq.cn/Article/details/ghygijxya.sHtML

[Q42] 连接条件附加过滤
来源：http://baike.zdbjq.cn/Article/details/gyuunljja.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.zdbjq.cn/Article/details/gxgmaxcgt.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.zdbjq.cn/Article/details/gxzgictvv.sHtML

[Q43] 标量子查询
来源：http://mobile.zdbjq.cn/Article/details/glqoyhofc.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.fehbvm.com/Article/details/gvkgcsyjo.sHtML

[Q44] IN 子查询
来源：http://baike.hesvh.cn/Article/details/grtafzwum.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.zdbjq.cn/Article/details/gctfejhii.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.zdbjq.cn/Article/details/gpetdsvpm.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fehbvm.com/Article/details/ghjdfrnry.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.fehbvm.com/Article/details/guwlasmzu.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.zdbjq.cn/Article/details/gahedkxtv.sHtML

[Q47] 与平均值比较
来源：http://www.share.fehbvm.com/Article/details/geoxxnkyd.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://mobile.hesvh.cn/Article/details/gbzrnpboh.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.zdbjq.cn/Article/details/gxzqzscmj.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.zdbjq.cn/Article/details/ghepaetqs.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.fehbvm.com/Article/details/gbjlnwqmn.sHtML

[Q49] 更新单行
来源：http://m.share.hesvh.cn/Article/details/ghgtjclcu.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.fehbvm.com/Article/details/gafblxfrs.sHtML

[Q50] 批量更新
来源：http://www.m.share.fehbvm.com/Article/details/gcrufhwll.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.zdbjq.cn/Article/details/gneowhaad.sHtML

[Q51] 用子查询更新
来源：http://www.blog.fehbvm.com/Article/details/gicmhrkiu.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.zdbjq.cn/Article/details/gzqgxcmap.sHtML

[Q52] 删除指定行
来源：http://www.m.share.zdbjq.cn/Article/details/gpeqimpwz.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.zdbjq.cn/Article/details/gdsjzzawb.sHtML

[Q53] 按条件删除
来源：http://blog.fehbvm.com/Article/details/gricranxv.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.fehbvm.com/Article/details/gwxphpzmh.sHtML

[Q54] 清空表
来源：http://blog.hesvh.cn/Article/details/gjgmvxqvy.sHtML

TRUNCATE TABLE logs;
来源：http://wap.fehbvm.com/Article/details/gspuuozni.sHtML

[Q55] 排名（并列占位）
来源：http://wap.hesvh.cn/Article/details/gbrgeleey.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.fehbvm.com/Article/details/grpaqklfn.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.fehbvm.com/Article/details/gjlxqtptn.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.zdbjq.cn/Article/details/gqkrutmkn.sHtML

[Q57] 行号
来源：http://baike.fehbvm.com/Article/details/gbvjtwflv.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.hesvh.cn/Article/details/ghuyjemyz.sHtML

[Q58] 累计求和
来源：http://www.blog.zdbjq.cn/Article/details/giywsttor.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.hesvh.cn/Article/details/gfcsnwyii.sHtML

[Q59] 分组内累计
来源：http://www.blog.hesvh.cn/Article/details/gwxlrmihs.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.hesvh.cn/Article/details/gtfgefgxg.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.zdbjq.cn/Article/details/guvqsgppk.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.fehbvm.com/Article/details/ghjqjpvvg.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.fehbvm.com/Article/details/gszdmkgof.sHtML

[Q61] 移动平均
来源：http://www.share.fehbvm.com/Article/details/gxomvelfp.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gjnqdaqog.sHtML

[Q62] 分组占比
来源：http://baike.hesvh.cn/Article/details/grfxyhwpg.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gsuuvmsuh.sHtML

[Q63] 开启事务
来源：http://baike.fehbvm.com/Article/details/gimljoldc.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.zdbjq.cn/Article/details/gfdzaiwpl.sHtML

[Q64] 提交事务
来源：http://wap.hesvh.cn/Article/details/gsfbhcnnn.sHtML

COMMIT;
来源：http://m.share.fehbvm.com/Article/details/gybgadeug.sHtML

[Q65] 回滚事务
来源：http://read.share.zdbjq.cn/Article/details/gnazaverd.sHtML

ROLLBACK;
来源：http://www.blog.zdbjq.cn/Article/details/gknaazzfq.sHtML

[Q66] 行锁查询
来源：http://mobile.hesvh.cn/Article/details/gscwpbihn.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.fehbvm.com/Article/details/ginisljgl.sHtML

[Q67] 设置隔离级别
来源：http://m.share.hesvh.cn/Article/details/gohckxzcx.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.fehbvm.com/Article/details/gqwogdqlr.sHtML

[Q68] 保存点
来源：http://blog.fehbvm.com/Article/details/gxavfghvu.sHtML

SAVEPOINT sp1;
来源：http://www.blog.zdbjq.cn/Article/details/gxdfkcvpm.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.hesvh.cn/Article/details/grzgeemlp.sHtML

[Q69] 查看执行计划
来源：http://m.share.zdbjq.cn/Article/details/ghughjzej.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.zdbjq.cn/Article/details/gzipzncaq.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.hesvh.cn/Article/details/gurcnebwa.sHtML

ANALYZE TABLE users;
来源：http://wap.hesvh.cn/Article/details/gfgokgaga.sHtML

[Q71] 查看建表语句
来源：http://baike.zdbjq.cn/Article/details/grsupyjqu.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.zdbjq.cn/Article/details/gevyaiqbu.sHtML

[Q72] 查看索引
来源：http://www.blog.zdbjq.cn/Article/details/gbmzwfltp.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/goezwxyfu.sHtML

[Q73] 查看表状态
来源：http://m.share.fehbvm.com/Article/details/gugijwcdv.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.fehbvm.com/Article/details/ghbgqwxzo.sHtML

[Q74] 强制使用索引
来源：http://mobile.zdbjq.cn/Article/details/gqqfznybz.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.zdbjq.cn/Article/details/gvjasbdwg.sHtML

[Q75] 日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gwzppbuvs.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.zdbjq.cn/Article/details/goyoripja.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fehbvm.com/Article/details/gawqwrlpx.sHtML

[Q76] 按天统计
来源：http://baike.fehbvm.com/Article/details/grosttmdl.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.hesvh.cn/Article/details/gmhbruqbl.sHtML

[Q77] 时间加减
来源：http://3g.zdbjq.cn/Article/details/glwxjagfx.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.fehbvm.com/Article/details/gwjeawmfk.sHtML

[Q78] 当前时间
来源：http://wap.zdbjq.cn/Article/details/gbskybccj.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.zdbjq.cn/Article/details/gckbsiqzz.sHtML

[Q79] 字符串拼接
来源：http://baike.zdbjq.cn/Article/details/gocagqsqe.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.hesvh.cn/Article/details/gwncffydb.sHtML

[Q80] 字符串截取
来源：http://wap.zdbjq.cn/Article/details/gczixcsmw.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gxhlgdkdz.sHtML

[Q81] 字符串替换
来源：http://read.share.fehbvm.com/Article/details/ggiaqywci.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.fehbvm.com/Article/details/gbrrnbyor.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fehbvm.com/Article/details/gcwerhrlf.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gmquusjrq.sHtML

[Q83] 大小写转换
来源：http://3g.zdbjq.cn/Article/details/grpcxhjfo.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gvnksuijt.sHtML

[Q84] 去除首尾空格
来源：http://wap.fehbvm.com/Article/details/gkyklhjqs.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gwkniukoj.sHtML

[Q85] 数值取整
来源：http://wap.fehbvm.com/Article/details/gxvkvlcbw.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fehbvm.com/Article/details/gqmayxsoc.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.hesvh.cn/Article/details/goplcduwk.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.zdbjq.cn/Article/details/gbthkigjd.sHtML

[Q87] JSON 字段做条件
来源：http://baike.zdbjq.cn/Article/details/gftfxpxjo.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.zdbjq.cn/Article/details/gvxrcsjxl.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.hesvh.cn/Article/details/gwutcyxuz.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.fehbvm.com/Article/details/gwzzjqxdw.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gnnkslqeb.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.fehbvm.com/Article/details/gzzzlukpe.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.hesvh.cn/Article/details/glxtsfrwj.sHtML

[Q90] 生成序号列
来源：http://m.share.zdbjq.cn/Article/details/gzwednwmv.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.zdbjq.cn/Article/details/gdkhkkltq.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gdwmlmpik.sHtML

R. Bash 专题
来源：http://baike.hesvh.cn/Article/details/ggycxyzah.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gaotomfdo.sHtML

[R01] shebang 与严格模式
来源：http://baike.fehbvm.com/Article/details/gfszqsqoh.sHtML

#!/usr/bin/env bash
来源：http://read.share.fehbvm.com/Article/details/gtywqirda.sHtML

set -euo pipefail
来源：http://www.blog.fehbvm.com/Article/details/gxirmubmm.sHtML

[R02] 变量赋值与使用
来源：http://blog.fehbvm.com/Article/details/ghntyzbjm.sHtML

name="Tom"; echo "$name"
来源：http://wap.hesvh.cn/Article/details/gtlhgvhts.sHtML

[R03] 只读变量
来源：http://3g.zdbjq.cn/Article/details/gjxdilsva.sHtML

readonly PI=3.14
来源：http://read.share.zdbjq.cn/Article/details/gauarzurq.sHtML

[R04] 位置参数
来源：http://wap.zdbjq.cn/Article/details/gopelcpmy.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.hesvh.cn/Article/details/gbijgyuow.sHtML

[R05] 参数默认值
来源：http://baike.fehbvm.com/Article/details/gkdxomeud.sHtML

name="${1:-default}"
来源：http://www.m.share.hesvh.cn/Article/details/gikecyuvn.sHtML

[R06] 判断命令是否存在
来源：http://blog.zdbjq.cn/Article/details/gjomurvvk.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.zdbjq.cn/Article/details/gvhrtqnmx.sHtML

[R07] if 判断文件
来源：http://mobile.hesvh.cn/Article/details/gdhlmbhcr.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.hesvh.cn/Article/details/gnfpxbrfh.sHtML

[R08] 数值比较
来源：http://3g.hesvh.cn/Article/details/gmksrrjbb.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.hesvh.cn/Article/details/gboyffrwn.sHtML

[R09] 字符串比较
来源：http://read.share.fehbvm.com/Article/details/gmeexsnxe.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.zdbjq.cn/Article/details/gkeekgjvz.sHtML

[R10] 正则匹配
来源：http://m.share.zdbjq.cn/Article/details/gkjmqscmi.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.zdbjq.cn/Article/details/gkesgvtoc.sHtML

[R11] case 多分支
来源：http://mobile.zdbjq.cn/Article/details/ghewbbovs.sHtML

case "$1" in
来源：http://read.share.zdbjq.cn/Article/details/gitmlgqgy.sHtML

start) echo "启动" ;;
来源：http://3g.fehbvm.com/Article/details/guktfezbc.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/glhgblial.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gaqrrhfut.sHtML

esac
来源：http://baike.zdbjq.cn/Article/details/gfoegyqhv.sHtML

[R12] for 遍历文件
来源：http://read.share.zdbjq.cn/Article/details/gosxqaffs.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fehbvm.com/Article/details/grngfkvmx.sHtML

[R13] for 计数循环
来源：http://mobile.zdbjq.cn/Article/details/graaysbaf.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.zdbjq.cn/Article/details/gihgdqdga.sHtML

[R14] C 风格 for
来源：http://www.m.share.zdbjq.cn/Article/details/grxchrofm.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.fehbvm.com/Article/details/gqtcrdxwo.sHtML

[R15] while 逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gwbbqgcsi.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.zdbjq.cn/Article/details/gdjaequir.sHtML

[R16] until 等待条件
来源：http://wap.zdbjq.cn/Article/details/giutaabxc.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.hesvh.cn/Article/details/gldmpchka.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fehbvm.com/Article/details/gpiaxocrj.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.fehbvm.com/Article/details/gyshkdcws.sHtML

[R18] 遍历数组
来源：http://www.blog.fehbvm.com/Article/details/glilsghgp.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fehbvm.com/Article/details/ggyqpdrfe.sHtML

[R19] 数组长度
来源：http://www.m.share.zdbjq.cn/Article/details/gfhvqkpum.sHtML

echo "${#arr[@]}"
来源：http://www.blog.hesvh.cn/Article/details/gnafzzsne.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fehbvm.com/Article/details/gyanvnaqe.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.zdbjq.cn/Article/details/gzhcwjvbf.sHtML

[R21] 字符串长度
来源：http://www.m.share.fehbvm.com/Article/details/gctkbjrsr.sHtML

echo "${#s}"
来源：http://mobile.fehbvm.com/Article/details/gtlmlgyzj.sHtML

[R22] 截取子串
来源：http://www.m.share.zdbjq.cn/Article/details/gjqxcidxg.sHtML

echo "${s:0:5}"
来源：http://www.share.zdbjq.cn/Article/details/gznkumqhz.sHtML

[R23] 字符串替换
来源：http://read.share.fehbvm.com/Article/details/gmachjmwa.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.zdbjq.cn/Article/details/gswzceyls.sHtML

[R24] 大小写转换
来源：http://3g.fehbvm.com/Article/details/gmthrinru.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.zdbjq.cn/Article/details/gwwgyngha.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.zdbjq.cn/Article/details/gkhaotpvg.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.zdbjq.cn/Article/details/gnhifshmv.sHtML

[R26] 命令替换
来源：http://www.blog.fehbvm.com/Article/details/gtiijpgsc.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.hesvh.cn/Article/details/glzarilfb.sHtML

[R27] 算术展开
来源：http://3g.hesvh.cn/Article/details/gkpxnykix.sHtML

echo $((1 + 2 * 3))
来源：http://blog.zdbjq.cn/Article/details/gkvwjldbd.sHtML

[R28] 浮点运算
来源：http://3g.fehbvm.com/Article/details/ghcuuboyc.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.zdbjq.cn/Article/details/gdnipmszn.sHtML

[R29] 定义函数
来源：http://blog.hesvh.cn/Article/details/gmwwauzzb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.hesvh.cn/Article/details/gcwtickti.sHtML

[R30] 函数返回状态码
来源：http://www.share.hesvh.cn/Article/details/grnsokpfi.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.zdbjq.cn/Article/details/gabmzrcro.sHtML

[R31] 局部变量
来源：http://www.blog.hesvh.cn/Article/details/gogurmkmt.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fehbvm.com/Article/details/gtzniwfdu.sHtML

[R32] 参数个数校验
来源：http://mobile.fehbvm.com/Article/details/gudidquxt.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.hesvh.cn/Article/details/goaaavjik.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.zdbjq.cn/Article/details/gfdqxzkjq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.zdbjq.cn/Article/details/gfmlhwuka.sHtML

[R34] 退出时清理
来源：http://read.share.zdbjq.cn/Article/details/gjgxitanb.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.hesvh.cn/Article/details/gzjmflyvw.sHtML

[R35] 后台执行并等待
来源：http://3g.zdbjq.cn/Article/details/gudchvuhu.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fehbvm.com/Article/details/gceugvbcl.sHtML

[R36] 并发执行多个任务
来源：http://blog.fehbvm.com/Article/details/grwgvggoh.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fehbvm.com/Article/details/grldgujko.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fehbvm.com/Article/details/ghyiawlnt.sHtML

files=$(ls -1)
来源：http://3g.fehbvm.com/Article/details/gklqbvudb.sHtML

[R38] 管道串联
来源：http://m.share.hesvh.cn/Article/details/gnhthjchc.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fehbvm.com/Article/details/gqiacoawo.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.zdbjq.cn/Article/details/gvjqucbcm.sHtML

cmd > out.log 2>&1
来源：http://mobile.zdbjq.cn/Article/details/gtmeoclbs.sHtML

[R40] 追加写日志
来源：http://3g.hesvh.cn/Article/details/gaomdlzlt.sHtML

echo "log" >> out.log
来源：http://mobile.hesvh.cn/Article/details/ghbvppxzm.sHtML

[R41] 丢弃输出
来源：http://www.share.hesvh.cn/Article/details/gidqnurtj.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.zdbjq.cn/Article/details/gfjhqsgrs.sHtML

[R42] 输入重定向
来源：http://mobile.fehbvm.com/Article/details/gqrofnopq.sHtML

wc -l < a.txt
来源：http://wap.fehbvm.com/Article/details/gzmplqomu.sHtML

[R43] 按名字查找文件
来源：http://mobile.zdbjq.cn/Article/details/gudkshixq.sHtML

find . -name "*.log" -type f
来源：http://3g.zdbjq.cn/Article/details/galcoqckb.sHtML

[R44] 按修改时间查找
来源：http://www.share.hesvh.cn/Article/details/gqrbjlyxc.sHtML

find . -mtime -7 -type f
来源：http://www.blog.zdbjq.cn/Article/details/gmbnodzdx.sHtML

[R45] 批量删除
来源：http://www.share.hesvh.cn/Article/details/gznkmsjhm.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.zdbjq.cn/Article/details/girodhlyo.sHtML

[R46] 递归替换文件内容
来源：http://baike.fehbvm.com/Article/details/gpwilesyh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.zdbjq.cn/Article/details/ghwdglexf.sHtML

[R47] sed 单行替换
来源：http://www.share.fehbvm.com/Article/details/grxpmkemg.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.hesvh.cn/Article/details/gjzxkzfco.sHtML

[R48] awk 取指定列
来源：http://www.blog.hesvh.cn/Article/details/gszjgdtlb.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fehbvm.com/Article/details/gshhrgfvx.sHtML

[R49] awk 带条件
来源：http://mobile.fehbvm.com/Article/details/gsupfuhpj.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.hesvh.cn/Article/details/gikfgvkcs.sHtML

[R50] awk 求和
来源：http://www.m.share.zdbjq.cn/Article/details/gdixppfsc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gpzxgygfc.sHtML

[R51] 排序去重取前几
来源：http://3g.zdbjq.cn/Article/details/gbtnfmxlx.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.fehbvm.com/Article/details/givvdwdaq.sHtML

[R52] 统计行数
来源：http://3g.zdbjq.cn/Article/details/guswusibm.sHtML

wc -l a.txt
来源：http://read.share.zdbjq.cn/Article/details/glccuxzyg.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.zdbjq.cn/Article/details/gxfxmsasb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.zdbjq.cn/Article/details/gormedhhr.sHtML

[R54] 比较两个文件
来源：http://www.share.fehbvm.com/Article/details/gezozsoex.sHtML

diff a.txt b.txt
来源：http://www.share.fehbvm.com/Article/details/gufpnoegs.sHtML

[R55] 压缩与解压
来源：http://wap.hesvh.cn/Article/details/guuevbpwc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://blog.hesvh.cn/Article/details/gscyjshoq.sHtML

[R56] 远程拷贝
来源：http://wap.hesvh.cn/Article/details/gwyxzncky.sHtML

scp file user@host:/path/
来源：http://3g.fehbvm.com/Article/details/grvmsoyam.sHtML

[R57] 远程执行命令
来源：http://www.share.hesvh.cn/Article/details/ghczpmyml.sHtML

ssh user@host 'uptime'
来源：http://wap.fehbvm.com/Article/details/gmjhnrgup.sHtML

[R58] 下载文件
来源：http://3g.zdbjq.cn/Article/details/gjqsephvl.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.hesvh.cn/Article/details/ggtvaqrku.sHtML

[R59] 发 POST JSON
来源：http://blog.zdbjq.cn/Article/details/gnxvvrksm.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.hesvh.cn/Article/details/gjiexcssk.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.zdbjq.cn/Article/details/gbwnzbkvu.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fehbvm.com/Article/details/gfayinhac.sHtML

[R61] 磁盘占用
来源：http://www.share.hesvh.cn/Article/details/gbukbvwep.sHtML

df -h;  du -sh *
来源：http://baike.hesvh.cn/Article/details/gckhbctli.sHtML

[R62] 找最占空间的文件
来源：http://www.share.hesvh.cn/Article/details/giokplkme.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.zdbjq.cn/Article/details/gkxokjapj.sHtML

[R63] 内存与进程
来源：http://baike.zdbjq.cn/Article/details/gprdzrfpe.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.hesvh.cn/Article/details/gcanusnhg.sHtML

[R64] 结束进程
来源：http://blog.fehbvm.com/Article/details/gfhwgyeha.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.hesvh.cn/Article/details/gydgyjboq.sHtML

[R65] 查看端口占用
来源：http://baike.zdbjq.cn/Article/details/grhdmzhei.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.hesvh.cn/Article/details/gxpkhvqrd.sHtML

[R66] 定时任务
来源：http://www.share.zdbjq.cn/Article/details/gstyqllhz.sHtML

crontab -e;  crontab -l
来源：http://baike.fehbvm.com/Article/details/giuublsxy.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.hesvh.cn/Article/details/gegttfsdl.sHtML

openssl rand -hex 16
来源：http://www.m.share.hesvh.cn/Article/details/gtubqcrsz.sHtML

[R68] 计算文件校验值
来源：http://mobile.hesvh.cn/Article/details/grhnnbejh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fehbvm.com/Article/details/ghsmgbict.sHtML

[R69] 生成随机密码
来源：http://www.blog.fehbvm.com/Article/details/gfpacqoib.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fehbvm.com/Article/details/gufulxnyo.sHtML

[R70] 时间戳与互转
来源：http://3g.hesvh.cn/Article/details/gurcvkmfz.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fehbvm.com/Article/details/gvalukbbh.sHtML

[R71] 日期格式化
来源：http://baike.zdbjq.cn/Article/details/gaehatkke.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.zdbjq.cn/Article/details/grebgerce.sHtML

[R72] 等待端口就绪
来源：http://blog.zdbjq.cn/Article/details/gsrsizoeb.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/gejcizehm.sHtML

[R73] 分割大日志
来源：http://blog.hesvh.cn/Article/details/gczuwihsf.sHtML


<!-- 参考信息 -->