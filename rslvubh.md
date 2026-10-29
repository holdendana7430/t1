代发 wailian999

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.share.zdbjq.cn/Article/details/gbiftytbf.sHtML

[Q26] 计数
来源：http://mobile.fehbvm.com/Article/details/gkfstumun.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/giwtnniao.sHtML

[Q27] 条件计数
来源：http://wap.hesvh.cn/Article/details/gezujlfsz.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.hesvh.cn/Article/details/gzskzxepv.sHtML

[Q28] 求和与平均
来源：http://www.m.share.hesvh.cn/Article/details/gvcsroexa.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gbqhxdhrz.sHtML

[Q29] 最大最小值
来源：http://mobile.hesvh.cn/Article/details/goabbppoi.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.hesvh.cn/Article/details/ghizyixvi.sHtML

[Q30] 分组统计
来源：http://baike.fehbvm.com/Article/details/gmeprczif.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.zdbjq.cn/Article/details/gnhzozgin.sHtML

[Q31] 分组后过滤
来源：http://3g.fehbvm.com/Article/details/gqnqqqdip.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.hesvh.cn/Article/details/gmjbciqzb.sHtML

[Q32] 分组拼接字符串
来源：http://baike.fehbvm.com/Article/details/gxvbhocac.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/giciaipok.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.zdbjq.cn/Article/details/gtlrxfqyd.sHtML

[Q33] 多列分组
来源：http://baike.hesvh.cn/Article/details/gqxlbrpsd.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.zdbjq.cn/Article/details/gfievxxxv.sHtML

[Q34] 每组取第一条
来源：http://3g.fehbvm.com/Article/details/gnddiriqm.sHtML

SELECT * FROM (
来源：http://3g.fehbvm.com/Article/details/golqkesxw.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://wap.hesvh.cn/Article/details/gziotnyyh.sHtML

) t WHERE rn = 1;
来源：http://blog.fehbvm.com/Article/details/gxnfiagyz.sHtML

[Q35] 内连接
来源：http://baike.hesvh.cn/Article/details/gfksuspdb.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/gtsxgjbsa.sHtML

[Q36] 左连接
来源：http://www.share.hesvh.cn/Article/details/gxevqzlcw.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.zdbjq.cn/Article/details/gjanvdufp.sHtML

[Q37] 右连接
来源：http://mobile.zdbjq.cn/Article/details/gmgfacboc.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.fehbvm.com/Article/details/gqyrnkkqv.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://blog.hesvh.cn/Article/details/glfzlrwnx.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.fehbvm.com/Article/details/gqdzinhfj.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.fehbvm.com/Article/details/ghlnpnaey.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.fehbvm.com/Article/details/gyidodklg.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.zdbjq.cn/Article/details/gapuaykzh.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.fehbvm.com/Article/details/gtocqanjp.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://blog.fehbvm.com/Article/details/gygfnccld.sHtML

[Q41] 多表连接
来源：http://www.blog.fehbvm.com/Article/details/gckqhjbgq.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://m.share.zdbjq.cn/Article/details/gsqosxabw.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.hesvh.cn/Article/details/grrmrmsdz.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.hesvh.cn/Article/details/gymryxrle.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gvluhubpg.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.zdbjq.cn/Article/details/gfrlbahht.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.zdbjq.cn/Article/details/gimfhiwwt.sHtML

[Q43] 标量子查询
来源：http://3g.zdbjq.cn/Article/details/goswhowlq.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.fehbvm.com/Article/details/gmvdqypzd.sHtML

[Q44] IN 子查询
来源：http://m.share.zdbjq.cn/Article/details/geimwtrjs.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.zdbjq.cn/Article/details/gerfbnycx.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.hesvh.cn/Article/details/ggvlwtwnm.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.zdbjq.cn/Article/details/gigyuvbiv.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.fehbvm.com/Article/details/gdzpjrwfd.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.hesvh.cn/Article/details/gakfaeafe.sHtML

[Q47] 与平均值比较
来源：http://www.share.hesvh.cn/Article/details/ghghrycdm.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.zdbjq.cn/Article/details/gcqhyalwu.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.fehbvm.com/Article/details/gcbfrzsyy.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://m.share.fehbvm.com/Article/details/glszklvay.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.hesvh.cn/Article/details/gqolzzetm.sHtML

[Q49] 更新单行
来源：http://blog.zdbjq.cn/Article/details/gowmwlxif.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.hesvh.cn/Article/details/gttkmcrjz.sHtML

[Q50] 批量更新
来源：http://3g.fehbvm.com/Article/details/grvqdhvfm.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.fehbvm.com/Article/details/gkamnndze.sHtML

[Q51] 用子查询更新
来源：http://wap.fehbvm.com/Article/details/gcwhtxisu.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.fehbvm.com/Article/details/gdqxmqiss.sHtML

[Q52] 删除指定行
来源：http://blog.zdbjq.cn/Article/details/ghsqunjbi.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.hesvh.cn/Article/details/gwodwnqub.sHtML

[Q53] 按条件删除
来源：http://3g.fehbvm.com/Article/details/ggpvsbwub.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.blog.fehbvm.com/Article/details/golzuieat.sHtML

[Q54] 清空表
来源：http://wap.fehbvm.com/Article/details/gromkyxhh.sHtML

TRUNCATE TABLE logs;
来源：http://baike.fehbvm.com/Article/details/grsozhvjp.sHtML

[Q55] 排名（并列占位）
来源：http://baike.fehbvm.com/Article/details/gsthkxipj.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.hesvh.cn/Article/details/gqgcszqcn.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.hesvh.cn/Article/details/gzxnlgqbs.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://read.share.fehbvm.com/Article/details/giyxmfhcq.sHtML

[Q57] 行号
来源：http://read.share.hesvh.cn/Article/details/ghbqwdhdf.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gcsiictqa.sHtML

[Q58] 累计求和
来源：http://mobile.zdbjq.cn/Article/details/guhzbccjk.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gyxmwxner.sHtML

[Q59] 分组内累计
来源：http://m.share.hesvh.cn/Article/details/gmrhuswlt.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gvdyteloj.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.hesvh.cn/Article/details/gllubofeh.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.hesvh.cn/Article/details/gdihedsut.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.zdbjq.cn/Article/details/giuetusyp.sHtML

[Q61] 移动平均
来源：http://read.share.fehbvm.com/Article/details/gnqmwhbnm.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gmuwxdeds.sHtML

[Q62] 分组占比
来源：http://read.share.zdbjq.cn/Article/details/gytrvutgz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gioacetlo.sHtML

[Q63] 开启事务
来源：http://m.share.fehbvm.com/Article/details/gvktfxaah.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.zdbjq.cn/Article/details/ghvufrtyr.sHtML

[Q64] 提交事务
来源：http://m.share.zdbjq.cn/Article/details/gvtvtlksn.sHtML

COMMIT;
来源：http://read.share.fehbvm.com/Article/details/gvijhfjdt.sHtML

[Q65] 回滚事务
来源：http://www.share.fehbvm.com/Article/details/gicvyzajw.sHtML

ROLLBACK;
来源：http://www.m.share.hesvh.cn/Article/details/ghhectnyt.sHtML

[Q66] 行锁查询
来源：http://www.m.share.fehbvm.com/Article/details/gltjrxkba.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.zdbjq.cn/Article/details/geuvnsudf.sHtML

[Q67] 设置隔离级别
来源：http://m.share.hesvh.cn/Article/details/gcgghlvvl.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.hesvh.cn/Article/details/giihjjswv.sHtML

[Q68] 保存点
来源：http://3g.hesvh.cn/Article/details/gbahjscia.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fehbvm.com/Article/details/gqocbrywy.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.zdbjq.cn/Article/details/gdnfrusus.sHtML

[Q69] 查看执行计划
来源：http://read.share.fehbvm.com/Article/details/gkxuzwuzr.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.zdbjq.cn/Article/details/gjvuvkrih.sHtML

[Q70] 更新统计信息
来源：http://mobile.zdbjq.cn/Article/details/gophrywhr.sHtML

ANALYZE TABLE users;
来源：http://wap.fehbvm.com/Article/details/gypayyoex.sHtML

[Q71] 查看建表语句
来源：http://blog.fehbvm.com/Article/details/gwazvzuou.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.zdbjq.cn/Article/details/glcdjmioc.sHtML

[Q72] 查看索引
来源：http://www.share.zdbjq.cn/Article/details/ggownclby.sHtML

SHOW INDEX FROM users;
来源：http://www.share.hesvh.cn/Article/details/gkftrtcuf.sHtML

[Q73] 查看表状态
来源：http://mobile.zdbjq.cn/Article/details/gmjukkvnt.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.fehbvm.com/Article/details/gtxssbaar.sHtML

[Q74] 强制使用索引
来源：http://blog.hesvh.cn/Article/details/gwbtfaqtz.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.hesvh.cn/Article/details/gikansbuz.sHtML

[Q75] 日期格式化
来源：http://baike.hesvh.cn/Article/details/glglxqzsw.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gvfixosfm.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fehbvm.com/Article/details/glvxldtda.sHtML

[Q76] 按天统计
来源：http://www.blog.hesvh.cn/Article/details/gqymiwigb.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.hesvh.cn/Article/details/gntohyslx.sHtML

[Q77] 时间加减
来源：http://mobile.hesvh.cn/Article/details/gauqdcmqb.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.zdbjq.cn/Article/details/gkmqmmbxp.sHtML

[Q78] 当前时间
来源：http://m.share.fehbvm.com/Article/details/gmsbhmspb.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.share.hesvh.cn/Article/details/gbwgbcidf.sHtML

[Q79] 字符串拼接
来源：http://www.share.fehbvm.com/Article/details/gcroarxya.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.hesvh.cn/Article/details/gonwkeqnx.sHtML

[Q80] 字符串截取
来源：http://www.blog.fehbvm.com/Article/details/gewkhrsqb.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.fehbvm.com/Article/details/grkjcczec.sHtML

[Q81] 字符串替换
来源：http://wap.zdbjq.cn/Article/details/gwfctjjcf.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.hesvh.cn/Article/details/gukpaqnps.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.zdbjq.cn/Article/details/guzoulzag.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gjeiegdue.sHtML

[Q83] 大小写转换
来源：http://read.share.hesvh.cn/Article/details/gzrawrrnm.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gppghaudf.sHtML

[Q84] 去除首尾空格
来源：http://baike.fehbvm.com/Article/details/gqdskwqvy.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gmqnsebyr.sHtML

[Q85] 数值取整
来源：http://mobile.fehbvm.com/Article/details/gbbzywhwh.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.fehbvm.com/Article/details/glyaclrbi.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.zdbjq.cn/Article/details/gtthdqhxy.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.hesvh.cn/Article/details/gdwkawmbe.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fehbvm.com/Article/details/gxgcbptwe.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fehbvm.com/Article/details/gbrpgsbzx.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.hesvh.cn/Article/details/gbnjupvxq.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fehbvm.com/Article/details/gvdtygrdt.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gvknhlwrr.sHtML

[Q89] 判断表是否存在
来源：http://blog.zdbjq.cn/Article/details/gejwdehfd.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fehbvm.com/Article/details/gdzpnsmgx.sHtML

[Q90] 生成序号列
来源：http://wap.zdbjq.cn/Article/details/gnwtdhxlk.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fehbvm.com/Article/details/gouaoidon.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gohofjtbi.sHtML

R. Bash 专题
来源：http://www.blog.hesvh.cn/Article/details/ggwanmvam.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gdxaqolnw.sHtML

[R01] shebang 与严格模式
来源：http://3g.zdbjq.cn/Article/details/gmiclejvc.sHtML

#!/usr/bin/env bash
来源：http://mobile.hesvh.cn/Article/details/gowqocgsv.sHtML

set -euo pipefail
来源：http://www.m.share.hesvh.cn/Article/details/gjfdktuge.sHtML

[R02] 变量赋值与使用
来源：http://baike.hesvh.cn/Article/details/gdvpsjtqu.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.zdbjq.cn/Article/details/gcmxmnech.sHtML

[R03] 只读变量
来源：http://mobile.hesvh.cn/Article/details/gqtleuxbk.sHtML

readonly PI=3.14
来源：http://mobile.hesvh.cn/Article/details/gtvuvtkrc.sHtML

[R04] 位置参数
来源：http://www.blog.zdbjq.cn/Article/details/gqhyncumg.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.zdbjq.cn/Article/details/gvsqkjpbi.sHtML

[R05] 参数默认值
来源：http://blog.hesvh.cn/Article/details/gmgbkffeo.sHtML

name="${1:-default}"
来源：http://www.blog.zdbjq.cn/Article/details/gkxqlxenl.sHtML

[R06] 判断命令是否存在
来源：http://www.share.fehbvm.com/Article/details/gvqhqbtku.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.hesvh.cn/Article/details/goucxpeja.sHtML

[R07] if 判断文件
来源：http://www.share.zdbjq.cn/Article/details/glrxtpmde.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://m.share.hesvh.cn/Article/details/gupuqixsh.sHtML

[R08] 数值比较
来源：http://wap.hesvh.cn/Article/details/giooknezi.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.zdbjq.cn/Article/details/gfhxwbquo.sHtML

[R09] 字符串比较
来源：http://www.share.zdbjq.cn/Article/details/gmtffimyr.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.hesvh.cn/Article/details/gljgjlqcv.sHtML

[R10] 正则匹配
来源：http://www.blog.fehbvm.com/Article/details/gsbvtdqdi.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.hesvh.cn/Article/details/ggbqzdljj.sHtML

[R11] case 多分支
来源：http://blog.hesvh.cn/Article/details/ggwyjylof.sHtML

case "$1" in
来源：http://www.blog.fehbvm.com/Article/details/goikmrtud.sHtML

start) echo "启动" ;;
来源：http://blog.hesvh.cn/Article/details/gjhnwjcai.sHtML

stop)  echo "停止" ;;
来源：http://3g.fehbvm.com/Article/details/gsezimfvw.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.zdbjq.cn/Article/details/gxohlurpd.sHtML

esac
来源：http://mobile.zdbjq.cn/Article/details/ggbvybogh.sHtML

[R12] for 遍历文件
来源：http://blog.zdbjq.cn/Article/details/ggtjusizc.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fehbvm.com/Article/details/ghkekfptv.sHtML

[R13] for 计数循环
来源：http://3g.zdbjq.cn/Article/details/gmctqdagn.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.hesvh.cn/Article/details/giflwchrf.sHtML

[R14] C 风格 for
来源：http://baike.zdbjq.cn/Article/details/gjocecxbt.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fehbvm.com/Article/details/gynrrcrpl.sHtML

[R15] while 逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gkfvkmkzw.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fehbvm.com/Article/details/gvkodseip.sHtML

[R16] until 等待条件
来源：http://wap.hesvh.cn/Article/details/glusxjvxd.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.zdbjq.cn/Article/details/gcnabkeln.sHtML

[R17] 数组定义与取值
来源：http://m.share.zdbjq.cn/Article/details/geidxgpak.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.hesvh.cn/Article/details/gotvldetw.sHtML

[R18] 遍历数组
来源：http://read.share.zdbjq.cn/Article/details/gmijzaihm.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.hesvh.cn/Article/details/gphkafjni.sHtML

[R19] 数组长度
来源：http://m.share.zdbjq.cn/Article/details/glehbibhh.sHtML

echo "${#arr[@]}"
来源：http://www.share.hesvh.cn/Article/details/gbliauspy.sHtML

[R20] 关联数组（字典）
来源：http://3g.zdbjq.cn/Article/details/gudxwzmtw.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.hesvh.cn/Article/details/gmbntszhd.sHtML

[R21] 字符串长度
来源：http://mobile.zdbjq.cn/Article/details/gfjkvradc.sHtML

echo "${#s}"
来源：http://3g.zdbjq.cn/Article/details/gttdhhgoh.sHtML

[R22] 截取子串
来源：http://blog.zdbjq.cn/Article/details/gpupxckps.sHtML

echo "${s:0:5}"
来源：http://read.share.hesvh.cn/Article/details/gdcuzrmqn.sHtML

[R23] 字符串替换
来源：http://m.share.zdbjq.cn/Article/details/gkojjsmzj.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.zdbjq.cn/Article/details/gahktmcal.sHtML

[R24] 大小写转换
来源：http://wap.hesvh.cn/Article/details/gesrbnxyd.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fehbvm.com/Article/details/gykvzlwzb.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.zdbjq.cn/Article/details/gexatuxiw.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fehbvm.com/Article/details/gyitbkoiu.sHtML

[R26] 命令替换
来源：http://mobile.zdbjq.cn/Article/details/gfmveutyt.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.zdbjq.cn/Article/details/gtstxxxxp.sHtML

[R27] 算术展开
来源：http://read.share.fehbvm.com/Article/details/gexpwavxe.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fehbvm.com/Article/details/grfijksyp.sHtML

[R28] 浮点运算
来源：http://www.share.hesvh.cn/Article/details/gzacppidg.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.zdbjq.cn/Article/details/gsiyundst.sHtML

[R29] 定义函数
来源：http://www.blog.zdbjq.cn/Article/details/gzshhtqac.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.hesvh.cn/Article/details/gobzlwlqs.sHtML

[R30] 函数返回状态码
来源：http://wap.hesvh.cn/Article/details/gswfxuvjr.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.hesvh.cn/Article/details/goifhfcix.sHtML

[R31] 局部变量
来源：http://www.blog.zdbjq.cn/Article/details/gpkcmxeua.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.hesvh.cn/Article/details/gnwpqnnht.sHtML

[R32] 参数个数校验
来源：http://baike.hesvh.cn/Article/details/geaglgiwu.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.zdbjq.cn/Article/details/gsljvlben.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.hesvh.cn/Article/details/ggqzobgny.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://read.share.hesvh.cn/Article/details/gzwkmkxek.sHtML

[R34] 退出时清理
来源：http://mobile.hesvh.cn/Article/details/gqoppydfe.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.zdbjq.cn/Article/details/gahwsopfe.sHtML

[R35] 后台执行并等待
来源：http://www.blog.zdbjq.cn/Article/details/gtlaqebvp.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fehbvm.com/Article/details/gicvjcblf.sHtML

[R36] 并发执行多个任务
来源：http://3g.fehbvm.com/Article/details/gtuwjsccj.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.hesvh.cn/Article/details/gaejyyfpy.sHtML

[R37] 把输出赋给变量
来源：http://wap.fehbvm.com/Article/details/gzvbemrhm.sHtML

files=$(ls -1)
来源：http://3g.hesvh.cn/Article/details/gjlqdqmdu.sHtML

[R38] 管道串联
来源：http://mobile.fehbvm.com/Article/details/gxmjnwtbf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fehbvm.com/Article/details/gexzhavgo.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.zdbjq.cn/Article/details/gyzmbxoeb.sHtML

cmd > out.log 2>&1
来源：http://3g.zdbjq.cn/Article/details/grkmvsjrf.sHtML

[R40] 追加写日志
来源：http://blog.hesvh.cn/Article/details/gcaovtsyi.sHtML

echo "log" >> out.log
来源：http://mobile.zdbjq.cn/Article/details/gsefxbjdu.sHtML

[R41] 丢弃输出
来源：http://blog.fehbvm.com/Article/details/gcwjkpvkj.sHtML

cmd >/dev/null 2>&1
来源：http://blog.zdbjq.cn/Article/details/giihuzhwh.sHtML

[R42] 输入重定向
来源：http://www.blog.hesvh.cn/Article/details/gletkyekd.sHtML

wc -l < a.txt
来源：http://www.share.fehbvm.com/Article/details/gudldqfwy.sHtML

[R43] 按名字查找文件
来源：http://m.share.fehbvm.com/Article/details/gzbdpvnuk.sHtML

find . -name "*.log" -type f
来源：http://mobile.fehbvm.com/Article/details/gyyozvdri.sHtML

[R44] 按修改时间查找
来源：http://m.share.fehbvm.com/Article/details/gdwfnmtiq.sHtML

find . -mtime -7 -type f
来源：http://mobile.fehbvm.com/Article/details/geuxvrymd.sHtML

[R45] 批量删除
来源：http://m.share.fehbvm.com/Article/details/gtdkmdxob.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.zdbjq.cn/Article/details/gzqgdnusq.sHtML

[R46] 递归替换文件内容
来源：http://www.share.zdbjq.cn/Article/details/gyysqnpxf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fehbvm.com/Article/details/gbmgdxyvl.sHtML

[R47] sed 单行替换
来源：http://www.blog.zdbjq.cn/Article/details/gqvghkvxs.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.hesvh.cn/Article/details/gvbuxuobi.sHtML

[R48] awk 取指定列
来源：http://www.blog.hesvh.cn/Article/details/gwjcgpqrb.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fehbvm.com/Article/details/gqfdvsfyv.sHtML

[R49] awk 带条件
来源：http://m.share.zdbjq.cn/Article/details/gwqzuluqt.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.zdbjq.cn/Article/details/gvgozjutc.sHtML

[R50] awk 求和
来源：http://read.share.fehbvm.com/Article/details/gqeygzhny.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.hesvh.cn/Article/details/glevntuiz.sHtML

[R51] 排序去重取前几
来源：http://baike.fehbvm.com/Article/details/ghtjvpnpe.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.zdbjq.cn/Article/details/gsbbfzuog.sHtML

[R52] 统计行数
来源：http://baike.fehbvm.com/Article/details/gxmdpghoh.sHtML

wc -l a.txt
来源：http://blog.hesvh.cn/Article/details/gkffaaqlb.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.hesvh.cn/Article/details/gvuamjglu.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.zdbjq.cn/Article/details/gxnydjgey.sHtML

[R54] 比较两个文件
来源：http://wap.fehbvm.com/Article/details/ggqcayvwr.sHtML

diff a.txt b.txt
来源：http://www.share.fehbvm.com/Article/details/gnjvetzgx.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fehbvm.com/Article/details/gklwjckjt.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.hesvh.cn/Article/details/gizkzmzgz.sHtML

[R56] 远程拷贝
来源：http://www.m.share.hesvh.cn/Article/details/glcccvldu.sHtML

scp file user@host:/path/
来源：http://www.m.share.zdbjq.cn/Article/details/ghcqystqp.sHtML

[R57] 远程执行命令
来源：http://www.m.share.zdbjq.cn/Article/details/gmtynbatz.sHtML

ssh user@host 'uptime'
来源：http://mobile.hesvh.cn/Article/details/gbexgnaxu.sHtML

[R58] 下载文件
来源：http://3g.zdbjq.cn/Article/details/givkgdjag.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.hesvh.cn/Article/details/gowzidvdd.sHtML

[R59] 发 POST JSON
来源：http://read.share.fehbvm.com/Article/details/guzapqmcb.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.zdbjq.cn/Article/details/ghaprmblt.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.hesvh.cn/Article/details/gdrrpwnus.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fehbvm.com/Article/details/gjqhwljtc.sHtML

[R61] 磁盘占用
来源：http://wap.fehbvm.com/Article/details/gktmridqz.sHtML

df -h;  du -sh *
来源：http://www.m.share.hesvh.cn/Article/details/gtzvxdolp.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.zdbjq.cn/Article/details/gsmjjpyep.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.zdbjq.cn/Article/details/gacvpbkgj.sHtML

[R63] 内存与进程
来源：http://blog.zdbjq.cn/Article/details/gqzwhpcyc.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.hesvh.cn/Article/details/gmrivwdxl.sHtML

[R64] 结束进程
来源：http://wap.hesvh.cn/Article/details/gpaurmjao.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.fehbvm.com/Article/details/glausebdq.sHtML

[R65] 查看端口占用
来源：http://wap.zdbjq.cn/Article/details/gkjxfvypv.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.zdbjq.cn/Article/details/gyinumgka.sHtML

[R66] 定时任务
来源：http://www.blog.fehbvm.com/Article/details/gcynjosuq.sHtML

crontab -e;  crontab -l
来源：http://baike.fehbvm.com/Article/details/gdrvrsxxm.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.hesvh.cn/Article/details/gstubrqst.sHtML

openssl rand -hex 16
来源：http://blog.fehbvm.com/Article/details/grefgnyjx.sHtML

[R68] 计算文件校验值
来源：http://mobile.zdbjq.cn/Article/details/gsralcdgl.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.hesvh.cn/Article/details/glygyqbtj.sHtML

[R69] 生成随机密码
来源：http://mobile.hesvh.cn/Article/details/gghltepgo.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fehbvm.com/Article/details/gyclktlzd.sHtML

[R70] 时间戳与互转
来源：http://m.share.fehbvm.com/Article/details/glwuiftre.sHtML

date +%s;  date -d @1700000000
来源：http://baike.hesvh.cn/Article/details/geqvivfaa.sHtML

[R71] 日期格式化
来源：http://www.m.share.zdbjq.cn/Article/details/gzfyxukws.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.zdbjq.cn/Article/details/gptywsfik.sHtML

[R72] 等待端口就绪
来源：http://www.share.fehbvm.com/Article/details/gyzrfwevo.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/gmxpwqxvj.sHtML

[R73] 分割大日志
来源：http://baike.zdbjq.cn/Article/details/grhmtlryn.sHtML

split -l 1000 big.log part_
来源：http://www.blog.hesvh.cn/Article/details/gnwgnotjo.sHtML

[R74] 批量重命名
来源：http://mobile.hesvh.cn/Article/details/gqieylzwi.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.hesvh.cn/Article/details/gkwvpdigi.sHtML

[R75] 导出环境变量
来源：http://blog.hesvh.cn/Article/details/gcoyhwybw.sHtML


<!-- 参考信息 -->