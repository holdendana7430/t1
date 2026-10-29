代发 wailian999

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.blog.fehbvm.com/Article/details/gazgmhkfs.sHtML

[Q26] 计数
来源：http://blog.zdbjq.cn/Article/details/ghcybggbi.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.hesvh.cn/Article/details/gnsxovqwk.sHtML

[Q27] 条件计数
来源：http://3g.zdbjq.cn/Article/details/getxeiuko.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://read.share.fehbvm.com/Article/details/glarqjerw.sHtML

[Q28] 求和与平均
来源：http://read.share.zdbjq.cn/Article/details/gmpdhvvkb.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/ghfcwfdth.sHtML

[Q29] 最大最小值
来源：http://www.m.share.zdbjq.cn/Article/details/gzjmwnrgu.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gqdrzdntm.sHtML

[Q30] 分组统计
来源：http://www.share.zdbjq.cn/Article/details/gopshffkx.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gcakpilho.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.zdbjq.cn/Article/details/ggjwrphbu.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.hesvh.cn/Article/details/gjuowibgu.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.hesvh.cn/Article/details/gzflbkcnr.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/gkeybdfrs.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.fehbvm.com/Article/details/gkwtqiuzv.sHtML

[Q33] 多列分组
来源：http://www.share.hesvh.cn/Article/details/gmzvfvjht.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.zdbjq.cn/Article/details/gbalzofbd.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.zdbjq.cn/Article/details/gsaffvydj.sHtML

SELECT * FROM (
来源：http://3g.zdbjq.cn/Article/details/gapztmacl.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.zdbjq.cn/Article/details/gitauwyqa.sHtML

) t WHERE rn = 1;
来源：http://www.blog.hesvh.cn/Article/details/ghwwvrrzs.sHtML

[Q35] 内连接
来源：http://read.share.zdbjq.cn/Article/details/gcbwsmdfy.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.hesvh.cn/Article/details/gkcioxxfq.sHtML

[Q36] 左连接
来源：http://mobile.fehbvm.com/Article/details/gxgeghdcu.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.zdbjq.cn/Article/details/ggrmdxzyv.sHtML

[Q37] 右连接
来源：http://3g.zdbjq.cn/Article/details/gvcabeebs.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.zdbjq.cn/Article/details/gnzudbtjt.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://m.share.zdbjq.cn/Article/details/ghkefypoc.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.hesvh.cn/Article/details/gbmcducjq.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.hesvh.cn/Article/details/gigbkpslj.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.zdbjq.cn/Article/details/gfotrrxhn.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.fehbvm.com/Article/details/gvugmssne.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.zdbjq.cn/Article/details/gciayhide.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.zdbjq.cn/Article/details/gwagkcoup.sHtML

[Q41] 多表连接
来源：http://www.m.share.zdbjq.cn/Article/details/geiyitpml.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.fehbvm.com/Article/details/gmnmnurow.sHtML

JOIN users u ON u.id = o.user_id
来源：http://read.share.fehbvm.com/Article/details/gaydhxgno.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://m.share.hesvh.cn/Article/details/gesauzsvs.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.hesvh.cn/Article/details/gcsvbxibo.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.hesvh.cn/Article/details/gvcvtdkvv.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.fehbvm.com/Article/details/guzebefsg.sHtML

[Q43] 标量子查询
来源：http://mobile.fehbvm.com/Article/details/gzbbdnliq.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.zdbjq.cn/Article/details/gzeuqgayg.sHtML

[Q44] IN 子查询
来源：http://www.blog.zdbjq.cn/Article/details/guuccrryw.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.hesvh.cn/Article/details/gljyjxces.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.hesvh.cn/Article/details/gqmbqwxfi.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fehbvm.com/Article/details/gfqinagbi.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.fehbvm.com/Article/details/gvgdiezdm.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.hesvh.cn/Article/details/gzsrmnfxx.sHtML

[Q47] 与平均值比较
来源：http://blog.zdbjq.cn/Article/details/gkjozlwrf.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.hesvh.cn/Article/details/gvgbwaqmo.sHtML

[Q48] CTE 公用表表达式
来源：http://3g.zdbjq.cn/Article/details/gsjtorllj.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.hesvh.cn/Article/details/grnhipfdr.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.zdbjq.cn/Article/details/gxeefgruw.sHtML

[Q49] 更新单行
来源：http://wap.hesvh.cn/Article/details/gviqzyttd.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://wap.zdbjq.cn/Article/details/goyyzlytg.sHtML

[Q50] 批量更新
来源：http://m.share.zdbjq.cn/Article/details/gbhlekkvk.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.hesvh.cn/Article/details/gbyikagjy.sHtML

[Q51] 用子查询更新
来源：http://www.blog.zdbjq.cn/Article/details/gcqxsuyng.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.zdbjq.cn/Article/details/gpqkyjotu.sHtML

[Q52] 删除指定行
来源：http://wap.zdbjq.cn/Article/details/gmzdsttyu.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.zdbjq.cn/Article/details/glqfzxbrf.sHtML

[Q53] 按条件删除
来源：http://wap.zdbjq.cn/Article/details/gpirhrtln.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.fehbvm.com/Article/details/gjbkrzvcg.sHtML

[Q54] 清空表
来源：http://wap.zdbjq.cn/Article/details/gxlrteyxx.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fehbvm.com/Article/details/gigkkhzuq.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.fehbvm.com/Article/details/getejcrnl.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.hesvh.cn/Article/details/gpzhsfsnn.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.fehbvm.com/Article/details/gfsdtgcdo.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.fehbvm.com/Article/details/gcmscpomx.sHtML

[Q57] 行号
来源：http://read.share.zdbjq.cn/Article/details/gdoozrlxz.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.hesvh.cn/Article/details/gqdkeiwkn.sHtML

[Q58] 累计求和
来源：http://m.share.hesvh.cn/Article/details/gfilqmzyh.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.fehbvm.com/Article/details/grfczxttm.sHtML

[Q59] 分组内累计
来源：http://m.share.hesvh.cn/Article/details/gyahtabdo.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gflsgckxp.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.hesvh.cn/Article/details/grcqimnjn.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.fehbvm.com/Article/details/ggnzgdqzj.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.fehbvm.com/Article/details/gvxpuwjpr.sHtML

[Q61] 移动平均
来源：http://baike.fehbvm.com/Article/details/ganhxzdqo.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://blog.hesvh.cn/Article/details/gwucwzrnq.sHtML

[Q62] 分组占比
来源：http://www.share.zdbjq.cn/Article/details/gzybevvoa.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gbzbmfqry.sHtML

[Q63] 开启事务
来源：http://www.share.zdbjq.cn/Article/details/gejsyhbve.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.fehbvm.com/Article/details/gsdzryiqg.sHtML

[Q64] 提交事务
来源：http://mobile.hesvh.cn/Article/details/grlpannnj.sHtML

COMMIT;
来源：http://www.share.fehbvm.com/Article/details/gbujyrntp.sHtML

[Q65] 回滚事务
来源：http://www.blog.zdbjq.cn/Article/details/gnokbyuyk.sHtML

ROLLBACK;
来源：http://read.share.fehbvm.com/Article/details/gfdujtwku.sHtML

[Q66] 行锁查询
来源：http://baike.zdbjq.cn/Article/details/gaktgyuan.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.fehbvm.com/Article/details/gcpdanznz.sHtML

[Q67] 设置隔离级别
来源：http://baike.fehbvm.com/Article/details/gsqymqczy.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.zdbjq.cn/Article/details/gawupdjro.sHtML

[Q68] 保存点
来源：http://wap.hesvh.cn/Article/details/glylaorok.sHtML

SAVEPOINT sp1;
来源：http://blog.fehbvm.com/Article/details/glqiyvvdv.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fehbvm.com/Article/details/gnhfolhuo.sHtML

[Q69] 查看执行计划
来源：http://wap.hesvh.cn/Article/details/gseighlfz.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.zdbjq.cn/Article/details/gjbqitaic.sHtML

[Q70] 更新统计信息
来源：http://baike.zdbjq.cn/Article/details/gxpixzqve.sHtML

ANALYZE TABLE users;
来源：http://3g.hesvh.cn/Article/details/gcwzmjyvy.sHtML

[Q71] 查看建表语句
来源：http://3g.hesvh.cn/Article/details/gacbaidka.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fehbvm.com/Article/details/gykcapyna.sHtML

[Q72] 查看索引
来源：http://www.blog.hesvh.cn/Article/details/ggrneylsk.sHtML

SHOW INDEX FROM users;
来源：http://wap.fehbvm.com/Article/details/gcthnthqa.sHtML

[Q73] 查看表状态
来源：http://blog.zdbjq.cn/Article/details/gtxydugvt.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.fehbvm.com/Article/details/gxivehmnk.sHtML

[Q74] 强制使用索引
来源：http://www.share.fehbvm.com/Article/details/gofctxmjp.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://m.share.zdbjq.cn/Article/details/grumiayto.sHtML

[Q75] 日期格式化
来源：http://read.share.hesvh.cn/Article/details/gawpcxqwt.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gstuiaawm.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.zdbjq.cn/Article/details/gftlcbato.sHtML

[Q76] 按天统计
来源：http://www.share.zdbjq.cn/Article/details/gskvottwf.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.zdbjq.cn/Article/details/gwvphzwna.sHtML

[Q77] 时间加减
来源：http://baike.hesvh.cn/Article/details/grwawpwkl.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.hesvh.cn/Article/details/gsezyenil.sHtML

[Q78] 当前时间
来源：http://www.share.zdbjq.cn/Article/details/gocntgiyi.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.fehbvm.com/Article/details/gfspoeviw.sHtML

[Q79] 字符串拼接
来源：http://read.share.fehbvm.com/Article/details/gjyrtgikn.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.hesvh.cn/Article/details/gnngkbflc.sHtML

[Q80] 字符串截取
来源：http://www.share.zdbjq.cn/Article/details/gnkwugjuy.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gaoyghksn.sHtML

[Q81] 字符串替换
来源：http://m.share.hesvh.cn/Article/details/gmafrcdzt.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gqhqivifk.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.hesvh.cn/Article/details/gyqhlpvfn.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gzrwwemou.sHtML

[Q83] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/gucsfhyba.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gjofnhlvq.sHtML

[Q84] 去除首尾空格
来源：http://read.share.hesvh.cn/Article/details/gfjrrwzye.sHtML

SELECT TRIM(name) FROM users;
来源：http://3g.fehbvm.com/Article/details/grdgnxthn.sHtML

[Q85] 数值取整
来源：http://mobile.hesvh.cn/Article/details/gazdwssde.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.zdbjq.cn/Article/details/gyabwrbfd.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.zdbjq.cn/Article/details/gvmjaqatm.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.hesvh.cn/Article/details/ghjiukiez.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.zdbjq.cn/Article/details/gdqijxujl.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.fehbvm.com/Article/details/gbrbdelnw.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.hesvh.cn/Article/details/gmsaknche.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.zdbjq.cn/Article/details/gegwfpnkr.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.zdbjq.cn/Article/details/gyqckoecd.sHtML

[Q89] 判断表是否存在
来源：http://mobile.zdbjq.cn/Article/details/gjmwlhpwu.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.hesvh.cn/Article/details/gqetcmyok.sHtML

[Q90] 生成序号列
来源：http://read.share.hesvh.cn/Article/details/gqdkwdbgu.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.hesvh.cn/Article/details/gqmmvufvn.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/grposqxed.sHtML

R. Bash 专题
来源：http://3g.hesvh.cn/Article/details/goitbrcwj.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gymoxnhky.sHtML

[R01] shebang 与严格模式
来源：http://wap.hesvh.cn/Article/details/gsqfnjdjl.sHtML

#!/usr/bin/env bash
来源：http://blog.fehbvm.com/Article/details/gfvlrxzpu.sHtML

set -euo pipefail
来源：http://blog.fehbvm.com/Article/details/gozydtzyv.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.hesvh.cn/Article/details/gseemgzrw.sHtML

name="Tom"; echo "$name"
来源：http://wap.fehbvm.com/Article/details/gyluyqorh.sHtML

[R03] 只读变量
来源：http://www.m.share.hesvh.cn/Article/details/gnzloidvy.sHtML

readonly PI=3.14
来源：http://wap.hesvh.cn/Article/details/gunkgervb.sHtML

[R04] 位置参数
来源：http://m.share.zdbjq.cn/Article/details/gncujwxxu.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.zdbjq.cn/Article/details/gzqjyaswu.sHtML

[R05] 参数默认值
来源：http://www.blog.hesvh.cn/Article/details/gadwgkdty.sHtML

name="${1:-default}"
来源：http://baike.fehbvm.com/Article/details/gwvbqrdbd.sHtML

[R06] 判断命令是否存在
来源：http://www.share.hesvh.cn/Article/details/ggledkrtr.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://read.share.zdbjq.cn/Article/details/grrklkfhu.sHtML

[R07] if 判断文件
来源：http://www.m.share.fehbvm.com/Article/details/gsuayzqip.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.hesvh.cn/Article/details/gwnwuxpph.sHtML

[R08] 数值比较
来源：http://www.m.share.hesvh.cn/Article/details/grfsewmin.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://baike.fehbvm.com/Article/details/ggcihfyqk.sHtML

[R09] 字符串比较
来源：http://read.share.zdbjq.cn/Article/details/gnszuirww.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.hesvh.cn/Article/details/gzapldcxj.sHtML

[R10] 正则匹配
来源：http://wap.fehbvm.com/Article/details/gbwybjojv.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.zdbjq.cn/Article/details/gtzxghnxy.sHtML

[R11] case 多分支
来源：http://mobile.fehbvm.com/Article/details/gsjfzqcnc.sHtML

case "$1" in
来源：http://mobile.fehbvm.com/Article/details/gtjulgvie.sHtML

start) echo "启动" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gqpxbqeuu.sHtML

stop)  echo "停止" ;;
来源：http://3g.zdbjq.cn/Article/details/gptsnxkau.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gnmoljtlj.sHtML

esac
来源：http://www.share.zdbjq.cn/Article/details/gbipgjbep.sHtML

[R12] for 遍历文件
来源：http://www.blog.zdbjq.cn/Article/details/golsvtlfi.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.zdbjq.cn/Article/details/gbnvkgpss.sHtML

[R13] for 计数循环
来源：http://www.m.share.fehbvm.com/Article/details/ggjfqqfxa.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.hesvh.cn/Article/details/gfhhyqlnj.sHtML

[R14] C 风格 for
来源：http://www.blog.fehbvm.com/Article/details/gvnaomtgz.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fehbvm.com/Article/details/ghfyjnxut.sHtML

[R15] while 逐行读文件
来源：http://baike.fehbvm.com/Article/details/gprbsljud.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fehbvm.com/Article/details/gmrcgwppb.sHtML

[R16] until 等待条件
来源：http://baike.hesvh.cn/Article/details/gwgtdunjx.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/gjjrnrslk.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.zdbjq.cn/Article/details/gahzdvnvh.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.zdbjq.cn/Article/details/gqllvtvdh.sHtML

[R18] 遍历数组
来源：http://m.share.hesvh.cn/Article/details/giryenmhu.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fehbvm.com/Article/details/gnctvlyot.sHtML

[R19] 数组长度
来源：http://3g.hesvh.cn/Article/details/gnolaxlfg.sHtML

echo "${#arr[@]}"
来源：http://baike.zdbjq.cn/Article/details/gpinidbmk.sHtML

[R20] 关联数组（字典）
来源：http://mobile.zdbjq.cn/Article/details/gdivwvsdy.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fehbvm.com/Article/details/gjtpvqaeh.sHtML

[R21] 字符串长度
来源：http://blog.hesvh.cn/Article/details/gvsxgfbae.sHtML

echo "${#s}"
来源：http://wap.hesvh.cn/Article/details/gqfuouocl.sHtML

[R22] 截取子串
来源：http://mobile.hesvh.cn/Article/details/gkyxfxlkm.sHtML

echo "${s:0:5}"
来源：http://m.share.hesvh.cn/Article/details/gupvypfia.sHtML

[R23] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/gzminpxsc.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.hesvh.cn/Article/details/giipljwsz.sHtML

[R24] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/glrjvytor.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.hesvh.cn/Article/details/gdgopbstv.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fehbvm.com/Article/details/gbpoofgfs.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.zdbjq.cn/Article/details/gkbonnnrk.sHtML

[R26] 命令替换
来源：http://read.share.zdbjq.cn/Article/details/gevocvzcn.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.hesvh.cn/Article/details/gzumtzdyp.sHtML

[R27] 算术展开
来源：http://3g.hesvh.cn/Article/details/gifqcogza.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.hesvh.cn/Article/details/gwyzjvjlv.sHtML

[R28] 浮点运算
来源：http://3g.hesvh.cn/Article/details/golrwbksy.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.zdbjq.cn/Article/details/gtdjpiuwy.sHtML

[R29] 定义函数
来源：http://www.blog.fehbvm.com/Article/details/gugmcbwch.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.hesvh.cn/Article/details/gylfxatei.sHtML

[R30] 函数返回状态码
来源：http://www.share.hesvh.cn/Article/details/grslrwgpp.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.zdbjq.cn/Article/details/gkczkxxso.sHtML

[R31] 局部变量
来源：http://blog.hesvh.cn/Article/details/gdsoevvqr.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.zdbjq.cn/Article/details/gvdnwrxae.sHtML

[R32] 参数个数校验
来源：http://read.share.fehbvm.com/Article/details/gjvmodqtk.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/gvdatahvf.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.zdbjq.cn/Article/details/gjjynxikn.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fehbvm.com/Article/details/ggjgpksgn.sHtML

[R34] 退出时清理
来源：http://blog.hesvh.cn/Article/details/gdscvnunh.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.hesvh.cn/Article/details/gmbmglfbi.sHtML

[R35] 后台执行并等待
来源：http://www.blog.zdbjq.cn/Article/details/gphdqkits.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.fehbvm.com/Article/details/gjznradgn.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fehbvm.com/Article/details/gjvnnexcc.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fehbvm.com/Article/details/gbenemwev.sHtML

[R37] 把输出赋给变量
来源：http://baike.zdbjq.cn/Article/details/gpedzvcts.sHtML

files=$(ls -1)
来源：http://blog.hesvh.cn/Article/details/gatnnwxsa.sHtML

[R38] 管道串联
来源：http://wap.hesvh.cn/Article/details/gyxbqtwrd.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.zdbjq.cn/Article/details/gqcnerulh.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.hesvh.cn/Article/details/giwjkbaee.sHtML

cmd > out.log 2>&1
来源：http://mobile.fehbvm.com/Article/details/gckmisqsb.sHtML

[R40] 追加写日志
来源：http://www.share.fehbvm.com/Article/details/gclczqhtj.sHtML

echo "log" >> out.log
来源：http://wap.zdbjq.cn/Article/details/grhtcrkvr.sHtML

[R41] 丢弃输出
来源：http://www.share.fehbvm.com/Article/details/gssslrehv.sHtML

cmd >/dev/null 2>&1
来源：http://wap.zdbjq.cn/Article/details/gcyovpbxk.sHtML

[R42] 输入重定向
来源：http://baike.hesvh.cn/Article/details/gfjnsabfr.sHtML

wc -l < a.txt
来源：http://mobile.hesvh.cn/Article/details/gksuuknur.sHtML

[R43] 按名字查找文件
来源：http://www.blog.hesvh.cn/Article/details/gdgkheqyp.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.hesvh.cn/Article/details/gwszvtsso.sHtML

[R44] 按修改时间查找
来源：http://wap.hesvh.cn/Article/details/gynppzgev.sHtML

find . -mtime -7 -type f
来源：http://www.blog.zdbjq.cn/Article/details/gcmlcksuz.sHtML

[R45] 批量删除
来源：http://baike.hesvh.cn/Article/details/giclasqyd.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fehbvm.com/Article/details/gaietoult.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fehbvm.com/Article/details/glzkijcqg.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.zdbjq.cn/Article/details/gdkunwqqj.sHtML

[R47] sed 单行替换
来源：http://blog.fehbvm.com/Article/details/gthjesknv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.hesvh.cn/Article/details/guqpulxth.sHtML

[R48] awk 取指定列
来源：http://mobile.fehbvm.com/Article/details/ghfzkfmoj.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.zdbjq.cn/Article/details/ghkuzxnlc.sHtML

[R49] awk 带条件
来源：http://read.share.hesvh.cn/Article/details/guzapymgx.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fehbvm.com/Article/details/gzcwvcliv.sHtML

[R50] awk 求和
来源：http://wap.fehbvm.com/Article/details/gpvfbjgje.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gkverxxky.sHtML

[R51] 排序去重取前几
来源：http://baike.zdbjq.cn/Article/details/gcejjgpht.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.zdbjq.cn/Article/details/gctejuksq.sHtML

[R52] 统计行数
来源：http://blog.fehbvm.com/Article/details/gbrchzbnw.sHtML

wc -l a.txt
来源：http://m.share.hesvh.cn/Article/details/gpzaikvlu.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.zdbjq.cn/Article/details/glzgemsfa.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.hesvh.cn/Article/details/gdpuskdof.sHtML

[R54] 比较两个文件
来源：http://www.share.fehbvm.com/Article/details/gocqmetvj.sHtML

diff a.txt b.txt
来源：http://m.share.fehbvm.com/Article/details/gbifrmlfy.sHtML

[R55] 压缩与解压
来源：http://m.share.fehbvm.com/Article/details/goxczdjtc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.hesvh.cn/Article/details/gxmmaybnm.sHtML

[R56] 远程拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/gvbzxlydl.sHtML

scp file user@host:/path/
来源：http://www.m.share.fehbvm.com/Article/details/grpqupthk.sHtML

[R57] 远程执行命令
来源：http://www.m.share.hesvh.cn/Article/details/gsbdzjhxq.sHtML

ssh user@host 'uptime'
来源：http://blog.hesvh.cn/Article/details/gcavuhphh.sHtML

[R58] 下载文件
来源：http://m.share.zdbjq.cn/Article/details/gvnkuvsic.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.zdbjq.cn/Article/details/gfkaiagrn.sHtML

[R59] 发 POST JSON
来源：http://3g.fehbvm.com/Article/details/gesxxaskh.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.hesvh.cn/Article/details/gtdjconts.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fehbvm.com/Article/details/gzwngnapj.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.zdbjq.cn/Article/details/gxkujpgfo.sHtML

[R61] 磁盘占用
来源：http://baike.hesvh.cn/Article/details/gywpqcxjk.sHtML

df -h;  du -sh *
来源：http://www.share.fehbvm.com/Article/details/gxryvwdkn.sHtML

[R62] 找最占空间的文件
来源：http://baike.fehbvm.com/Article/details/gyujgpnmd.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fehbvm.com/Article/details/ggbwajvmx.sHtML

[R63] 内存与进程
来源：http://www.share.hesvh.cn/Article/details/gcpdaqxvj.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.hesvh.cn/Article/details/gxctvcwlc.sHtML

[R64] 结束进程
来源：http://read.share.hesvh.cn/Article/details/gszlhnlvl.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.hesvh.cn/Article/details/gsndceqcc.sHtML

[R65] 查看端口占用
来源：http://baike.zdbjq.cn/Article/details/gcwzxccho.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fehbvm.com/Article/details/gujrsyhoz.sHtML

[R66] 定时任务
来源：http://www.blog.hesvh.cn/Article/details/gcyqbjqqt.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fehbvm.com/Article/details/gmnuoifcq.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.hesvh.cn/Article/details/gjdzxyshn.sHtML

openssl rand -hex 16
来源：http://mobile.zdbjq.cn/Article/details/gdgatvmfd.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.hesvh.cn/Article/details/gworarkji.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.hesvh.cn/Article/details/gekhqpudr.sHtML

[R69] 生成随机密码
来源：http://read.share.fehbvm.com/Article/details/gstgsxpaq.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.zdbjq.cn/Article/details/gqimfiwix.sHtML

[R70] 时间戳与互转
来源：http://baike.zdbjq.cn/Article/details/gtiwyecxx.sHtML

date +%s;  date -d @1700000000
来源：http://wap.zdbjq.cn/Article/details/gwmzytqfi.sHtML

[R71] 日期格式化
来源：http://m.share.hesvh.cn/Article/details/gunzqjchs.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fehbvm.com/Article/details/gflqdlwxf.sHtML

[R72] 等待端口就绪
来源：http://blog.hesvh.cn/Article/details/ghbluctqs.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.hesvh.cn/Article/details/gxpvoqjth.sHtML

[R73] 分割大日志
来源：http://www.m.share.hesvh.cn/Article/details/gveujkztv.sHtML

split -l 1000 big.log part_
来源：http://m.share.hesvh.cn/Article/details/gydvfmzfz.sHtML

[R74] 批量重命名
来源：http://www.m.share.fehbvm.com/Article/details/gmxemgunn.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.zdbjq.cn/Article/details/gmcxxjhop.sHtML

[R75] 导出环境变量
来源：http://baike.zdbjq.cn/Article/details/gdqlijdev.sHtML


<!-- 参考信息 -->