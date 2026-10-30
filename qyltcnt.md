代发 wailian999

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gojmyritd.sHtML

[Q32] 分组拼接字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gypzuoivz.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.fanxiaobao.xyz/Article/details/gfabkfbfl.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.fanxiaobao.xyz/Article/details/gofhedjdq.sHtML

[Q33] 多列分组
来源：http://wap.fanxiaobao.xyz/Article/details/gzymkizjd.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.fanxiaobao.xyz/Article/details/gizgililj.sHtML

[Q34] 每组取第一条
来源：http://www.blog.fanxiaobao.xyz/Article/details/gldveprmv.sHtML

SELECT * FROM (
来源：http://3g.fanxiaobao.xyz/Article/details/gbjrifmzp.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.fanxiaobao.xyz/Article/details/gzmvnqwax.sHtML

) t WHERE rn = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbyvyydgf.sHtML

[Q35] 内连接
来源：http://m.share.fanxiaobao.xyz/Article/details/gobzwevbe.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fanxiaobao.xyz/Article/details/gtlfgooka.sHtML

[Q36] 左连接
来源：http://www.share.fanxiaobao.xyz/Article/details/goufzudis.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fanxiaobao.xyz/Article/details/gukomsdik.sHtML

[Q37] 右连接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gixiwzssv.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://baike.fanxiaobao.xyz/Article/details/gzvbxihgg.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gydjugygz.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.fanxiaobao.xyz/Article/details/ghmsqpyzm.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.fanxiaobao.xyz/Article/details/gjtmjtldk.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.fanxiaobao.xyz/Article/details/grwkpfiwl.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gpvmrqkvl.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.fanxiaobao.xyz/Article/details/gmyejcrkj.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.fanxiaobao.xyz/Article/details/ghlguyzii.sHtML

[Q41] 多表连接
来源：http://mobile.fanxiaobao.xyz/Article/details/grswxicwl.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfwidkssk.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.fanxiaobao.xyz/Article/details/gltlyoaxf.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.fanxiaobao.xyz/Article/details/gwbbelfzx.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gqxbciyqt.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.fanxiaobao.xyz/Article/details/gdnpieaof.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.fanxiaobao.xyz/Article/details/gufkwlquh.sHtML

[Q43] 标量子查询
来源：http://baike.fanxiaobao.xyz/Article/details/gaqwjffpl.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.fanxiaobao.xyz/Article/details/gpuussder.sHtML

[Q44] IN 子查询
来源：http://baike.fanxiaobao.xyz/Article/details/gimzcjtgv.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.fanxiaobao.xyz/Article/details/gkctfkuhn.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.fanxiaobao.xyz/Article/details/ggvhftubl.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fanxiaobao.xyz/Article/details/grwxwhvpp.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.fanxiaobao.xyz/Article/details/grqppvbqn.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goydylain.sHtML

[Q47] 与平均值比较
来源：http://blog.fanxiaobao.xyz/Article/details/ghgddccyb.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.fanxiaobao.xyz/Article/details/gyyjppfdb.sHtML

[Q48] CTE 公用表表达式
来源：http://mobile.fanxiaobao.xyz/Article/details/gifdvralf.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.fanxiaobao.xyz/Article/details/geounaatd.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.fanxiaobao.xyz/Article/details/gyksunjmi.sHtML

[Q49] 更新单行
来源：http://3g.fanxiaobao.xyz/Article/details/gmuodglfd.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/grfilvhyy.sHtML

[Q50] 批量更新
来源：http://wap.fanxiaobao.xyz/Article/details/gtjnoofzj.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gezejvxxo.sHtML

[Q51] 用子查询更新
来源：http://mobile.fanxiaobao.xyz/Article/details/gfdrfdkzv.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/glythzvud.sHtML

[Q52] 删除指定行
来源：http://www.share.fanxiaobao.xyz/Article/details/grdmywbxm.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/giddbprlw.sHtML

[Q53] 按条件删除
来源：http://3g.fanxiaobao.xyz/Article/details/gvucwjtxu.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.fanxiaobao.xyz/Article/details/glizlexyj.sHtML

[Q54] 清空表
来源：http://wap.fanxiaobao.xyz/Article/details/gvvkxihjc.sHtML

TRUNCATE TABLE logs;
来源：http://blog.fanxiaobao.xyz/Article/details/gtlfzxxrb.sHtML

[Q55] 排名（并列占位）
来源：http://blog.fanxiaobao.xyz/Article/details/ghpvpiewu.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://m.share.fanxiaobao.xyz/Article/details/gltlnhuxp.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.fanxiaobao.xyz/Article/details/guravgkal.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.fanxiaobao.xyz/Article/details/gbrkfdaxt.sHtML

[Q57] 行号
来源：http://www.share.fanxiaobao.xyz/Article/details/gbpledcid.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfdegwiku.sHtML

[Q58] 累计求和
来源：http://baike.fanxiaobao.xyz/Article/details/gobfeorwy.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gaajywdft.sHtML

[Q59] 分组内累计
来源：http://baike.fanxiaobao.xyz/Article/details/gnvqyiako.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gznkwbykh.sHtML

[Q60] 取上一行 / 下一行
来源：http://m.share.fanxiaobao.xyz/Article/details/gasztexhf.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fanxiaobao.xyz/Article/details/gsmunhwfi.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnkaaipey.sHtML

[Q61] 移动平均
来源：http://blog.fanxiaobao.xyz/Article/details/gmmldnimw.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gpvdxcyph.sHtML

[Q62] 分组占比
来源：http://blog.fanxiaobao.xyz/Article/details/gppeqsmkm.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqwphsjmk.sHtML

[Q63] 开启事务
来源：http://blog.fanxiaobao.xyz/Article/details/gropehysi.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.fanxiaobao.xyz/Article/details/gyqxjxpnc.sHtML

[Q64] 提交事务
来源：http://wap.fanxiaobao.xyz/Article/details/gufwujjpa.sHtML

COMMIT;
来源：http://wap.fanxiaobao.xyz/Article/details/gjzdnpwvr.sHtML

[Q65] 回滚事务
来源：http://mobile.fanxiaobao.xyz/Article/details/gclujhkoh.sHtML

ROLLBACK;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gosparkni.sHtML

[Q66] 行锁查询
来源：http://3g.fanxiaobao.xyz/Article/details/gdumihkvz.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.fanxiaobao.xyz/Article/details/girkwrzfg.sHtML

[Q67] 设置隔离级别
来源：http://3g.fanxiaobao.xyz/Article/details/gjxfowjgm.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcieykhvv.sHtML

[Q68] 保存点
来源：http://mobile.fanxiaobao.xyz/Article/details/gwswwxgue.sHtML

SAVEPOINT sp1;
来源：http://baike.fanxiaobao.xyz/Article/details/gikisvryi.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqgvppgdu.sHtML

[Q69] 查看执行计划
来源：http://baike.fanxiaobao.xyz/Article/details/gpjkueorr.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.fanxiaobao.xyz/Article/details/gzokwxeii.sHtML

[Q70] 更新统计信息
来源：http://baike.fanxiaobao.xyz/Article/details/gywpxfsil.sHtML

ANALYZE TABLE users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwzfdfbql.sHtML

[Q71] 查看建表语句
来源：http://m.share.fanxiaobao.xyz/Article/details/gdhyquqin.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.fanxiaobao.xyz/Article/details/gidecodvs.sHtML

[Q72] 查看索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gacrbeper.sHtML

SHOW INDEX FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gytwvnnxb.sHtML

[Q73] 查看表状态
来源：http://blog.fanxiaobao.xyz/Article/details/gstdxghmd.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.fanxiaobao.xyz/Article/details/gtetpouvf.sHtML

[Q74] 强制使用索引
来源：http://read.share.fanxiaobao.xyz/Article/details/gbmbsiuxs.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://wap.fanxiaobao.xyz/Article/details/gcocfxcno.sHtML

[Q75] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gjpnldhdl.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gcakupwhv.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.fanxiaobao.xyz/Article/details/grztynvdj.sHtML

[Q76] 按天统计
来源：http://blog.fanxiaobao.xyz/Article/details/grizcbhgh.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fanxiaobao.xyz/Article/details/ginfnkycx.sHtML

[Q77] 时间加减
来源：http://read.share.fanxiaobao.xyz/Article/details/gnludhojx.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.fanxiaobao.xyz/Article/details/glgdhfqpk.sHtML

[Q78] 当前时间
来源：http://m.share.fanxiaobao.xyz/Article/details/gwgtnkhzd.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.fanxiaobao.xyz/Article/details/gtaqhwyun.sHtML

[Q79] 字符串拼接
来源：http://m.share.fanxiaobao.xyz/Article/details/gmtuopmlb.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gstqiengq.sHtML

[Q80] 字符串截取
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtbbnytmw.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghelytwfj.sHtML

[Q81] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/ggmqnqcst.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gcoofefph.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gdrkhdbtf.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glaeyxhvq.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkokczixe.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gshoyqbpf.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fanxiaobao.xyz/Article/details/gwgylgedt.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggkwwrxqz.sHtML

[Q85] 数值取整
来源：http://baike.fanxiaobao.xyz/Article/details/gbxcrsmry.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdrftasfe.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fanxiaobao.xyz/Article/details/gymjtvxnp.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fanxiaobao.xyz/Article/details/ggeuimxuz.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gogkcuyad.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fanxiaobao.xyz/Article/details/ggqclxakh.sHtML

[Q88] 行转列（条件聚合）
来源：http://baike.fanxiaobao.xyz/Article/details/gkzwdepki.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.share.fanxiaobao.xyz/Article/details/ggvcwzfsh.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gfmzzbvdr.sHtML

[Q89] 判断表是否存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gtaicnlgc.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fanxiaobao.xyz/Article/details/gawpsfrcs.sHtML

[Q90] 生成序号列
来源：http://3g.fanxiaobao.xyz/Article/details/glvyhtmzu.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fanxiaobao.xyz/Article/details/gadizoeev.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdfdwripc.sHtML

R. Bash 专题
来源：http://read.share.fanxiaobao.xyz/Article/details/gdcnkpjwi.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gkfiqdqwh.sHtML

[R01] shebang 与严格模式
来源：http://3g.fanxiaobao.xyz/Article/details/gbbjfuzcw.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtmilmgwo.sHtML

set -euo pipefail
来源：http://www.blog.fanxiaobao.xyz/Article/details/gorpzqtza.sHtML

[R02] 变量赋值与使用
来源：http://3g.fanxiaobao.xyz/Article/details/gbuonkkfg.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fanxiaobao.xyz/Article/details/gxuhmvola.sHtML

[R03] 只读变量
来源：http://blog.fanxiaobao.xyz/Article/details/gxlrlwkcd.sHtML

readonly PI=3.14
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghvyayulq.sHtML

[R04] 位置参数
来源：http://www.share.fanxiaobao.xyz/Article/details/grvnmxqhi.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fanxiaobao.xyz/Article/details/gdkaqgjoj.sHtML

[R05] 参数默认值
来源：http://blog.fanxiaobao.xyz/Article/details/goprevrtr.sHtML

name="${1:-default}"
来源：http://baike.fanxiaobao.xyz/Article/details/ghafzfqhm.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnpmyvqro.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gepyqexba.sHtML

[R07] if 判断文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gtlxopguw.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkhkcdqcq.sHtML

[R08] 数值比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gnvekfxwl.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gcxjuiyib.sHtML

[R09] 字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gsdxmzxry.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gofrnibxm.sHtML

[R10] 正则匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gqctbeyix.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goawhmjzo.sHtML

[R11] case 多分支
来源：http://www.share.fanxiaobao.xyz/Article/details/ghiwfibih.sHtML

case "$1" in
来源：http://3g.fanxiaobao.xyz/Article/details/genvijwjz.sHtML

start) echo "启动" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/ganykyvze.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnsayxsab.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghqdjzjez.sHtML

esac
来源：http://mobile.fanxiaobao.xyz/Article/details/gnwqfctto.sHtML

[R12] for 遍历文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gbxhrvnwa.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gisnhpsve.sHtML

[R13] for 计数循环
来源：http://read.share.fanxiaobao.xyz/Article/details/gkxhodzjp.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/grfgjober.sHtML

[R14] C 风格 for
来源：http://mobile.fanxiaobao.xyz/Article/details/gwgirckdb.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gdgjivtbc.sHtML

[R15] while 逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gwkcdwuxb.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/geislhzel.sHtML

[R16] until 等待条件
来源：http://wap.fanxiaobao.xyz/Article/details/gmqkaroot.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gedbkurth.sHtML

[R17] 数组定义与取值
来源：http://wap.fanxiaobao.xyz/Article/details/ganzwjoyp.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwnbqteyo.sHtML

[R18] 遍历数组
来源：http://m.share.fanxiaobao.xyz/Article/details/govufrhkb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/giinsftnd.sHtML

[R19] 数组长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdnswcmyc.sHtML

echo "${#arr[@]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/grswcxmgk.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fanxiaobao.xyz/Article/details/gjtmvzhdv.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gppaxcnua.sHtML

[R21] 字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbguomlyt.sHtML

echo "${#s}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gmubhzxit.sHtML

[R22] 截取子串
来源：http://baike.fanxiaobao.xyz/Article/details/gmwgnafzi.sHtML

echo "${s:0:5}"
来源：http://m.share.fanxiaobao.xyz/Article/details/grejrvrpu.sHtML

[R23] 字符串替换
来源：http://wap.fanxiaobao.xyz/Article/details/gdtkzbakq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggrwwtwoz.sHtML

[R24] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gmuqkratu.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gexmmteoj.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.fanxiaobao.xyz/Article/details/ghamcposm.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fanxiaobao.xyz/Article/details/glqjwprmy.sHtML

[R26] 命令替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsnzmrucc.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.fanxiaobao.xyz/Article/details/gpejgqtbu.sHtML

[R27] 算术展开
来源：http://3g.fanxiaobao.xyz/Article/details/gmruzppfd.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fanxiaobao.xyz/Article/details/gqgnhkund.sHtML

[R28] 浮点运算
来源：http://baike.fanxiaobao.xyz/Article/details/gppjqyinu.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fanxiaobao.xyz/Article/details/gfbgwgjsw.sHtML

[R29] 定义函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gpbzixbsk.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gstdmnwrk.sHtML

[R30] 函数返回状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/ghmoyshzx.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyanqfkqw.sHtML

[R31] 局部变量
来源：http://read.share.fanxiaobao.xyz/Article/details/geuimwsrm.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gobzpzrpk.sHtML

[R32] 参数个数校验
来源：http://blog.fanxiaobao.xyz/Article/details/gfrurpgnl.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gwjptituv.sHtML

[R33] 捕获错误并提示行号
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfkbofwws.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.fanxiaobao.xyz/Article/details/gsmilptkd.sHtML

[R34] 退出时清理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyvxmzjry.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gahakqcqy.sHtML

[R35] 后台执行并等待
来源：http://blog.fanxiaobao.xyz/Article/details/ghbgdxlit.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fanxiaobao.xyz/Article/details/glxvaczcq.sHtML

[R36] 并发执行多个任务
来源：http://3g.fanxiaobao.xyz/Article/details/gnpjcclhm.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.fanxiaobao.xyz/Article/details/gckunqlea.sHtML

[R37] 把输出赋给变量
来源：http://wap.fanxiaobao.xyz/Article/details/gpuxycktc.sHtML

files=$(ls -1)
来源：http://baike.fanxiaobao.xyz/Article/details/gvfbqvkpq.sHtML

[R38] 管道串联
来源：http://m.share.fanxiaobao.xyz/Article/details/guicpxmkf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.fanxiaobao.xyz/Article/details/gsnealmyh.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fanxiaobao.xyz/Article/details/geadwboss.sHtML

cmd > out.log 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/gijonenhv.sHtML

[R40] 追加写日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqshmasxt.sHtML

echo "log" >> out.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gjapcihvs.sHtML

[R41] 丢弃输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gpntfzlds.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/glotkufbm.sHtML

[R42] 输入重定向
来源：http://read.share.fanxiaobao.xyz/Article/details/gcvyuvmew.sHtML

wc -l < a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gjekqhpqy.sHtML

[R43] 按名字查找文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gcmmwhanu.sHtML

find . -name "*.log" -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gofjsactt.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqpvltehg.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gutidkngt.sHtML

[R45] 批量删除
来源：http://m.share.fanxiaobao.xyz/Article/details/gkqtzvnre.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fanxiaobao.xyz/Article/details/gmsmoubbr.sHtML

[R46] 递归替换文件内容
来源：http://m.share.fanxiaobao.xyz/Article/details/gkiupsvnv.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fanxiaobao.xyz/Article/details/ggxxhqowi.sHtML

[R47] sed 单行替换
来源：http://m.share.fanxiaobao.xyz/Article/details/geosxnbsg.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gnykykvdx.sHtML

[R48] awk 取指定列
来源：http://baike.fanxiaobao.xyz/Article/details/gxrfccvus.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gfigbbxwh.sHtML

[R49] awk 带条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gpvieeyhc.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fanxiaobao.xyz/Article/details/glgdcrpwr.sHtML

[R50] awk 求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtgpfuoub.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gncrcdtoj.sHtML

[R51] 排序去重取前几
来源：http://baike.fanxiaobao.xyz/Article/details/gydydgwma.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.fanxiaobao.xyz/Article/details/garcrfvbf.sHtML

[R52] 统计行数
来源：http://3g.fanxiaobao.xyz/Article/details/gmsfjmrkj.sHtML

wc -l a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gprivookr.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzfnmafkf.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fanxiaobao.xyz/Article/details/ghawmrgou.sHtML

[R54] 比较两个文件
来源：http://wap.fanxiaobao.xyz/Article/details/gjkiwljbu.sHtML

diff a.txt b.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gygiwhond.sHtML

[R55] 压缩与解压
来源：http://blog.fanxiaobao.xyz/Article/details/gvjmrmymf.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fanxiaobao.xyz/Article/details/gqttodfcq.sHtML

[R56] 远程拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyibsqvtt.sHtML

scp file user@host:/path/
来源：http://baike.fanxiaobao.xyz/Article/details/gmjzhgsch.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grcbymelb.sHtML

ssh user@host 'uptime'
来源：http://blog.fanxiaobao.xyz/Article/details/gcppjnhff.sHtML

[R58] 下载文件
来源：http://3g.fanxiaobao.xyz/Article/details/gzyiajkzm.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fanxiaobao.xyz/Article/details/gzsdyhrct.sHtML

[R59] 发 POST JSON
来源：http://3g.fanxiaobao.xyz/Article/details/gayfdyufu.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gzkmhfalg.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gynhwkvuj.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.fanxiaobao.xyz/Article/details/gxmubmupw.sHtML

[R61] 磁盘占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gdmqhyvux.sHtML

df -h;  du -sh *
来源：http://wap.fanxiaobao.xyz/Article/details/gjtloeypc.sHtML

[R62] 找最占空间的文件
来源：http://3g.fanxiaobao.xyz/Article/details/gnzkrrfic.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fanxiaobao.xyz/Article/details/gxgmgqksx.sHtML

[R63] 内存与进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gztlnrowy.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fanxiaobao.xyz/Article/details/gvgxtejna.sHtML

[R64] 结束进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gtjaeabdz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnwexmhtq.sHtML

[R65] 查看端口占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gkmbhpqhb.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fanxiaobao.xyz/Article/details/gzpvnvelf.sHtML

[R66] 定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/gipdpaydi.sHtML

crontab -e;  crontab -l
来源：http://wap.fanxiaobao.xyz/Article/details/gdscmwjkm.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fanxiaobao.xyz/Article/details/gfxwujghf.sHtML

openssl rand -hex 16
来源：http://baike.fanxiaobao.xyz/Article/details/gsaynlyok.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghdudklkl.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glcikgtwn.sHtML

[R69] 生成随机密码
来源：http://blog.fanxiaobao.xyz/Article/details/gndbcgrsu.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fanxiaobao.xyz/Article/details/grqadejll.sHtML

[R70] 时间戳与互转
来源：http://mobile.fanxiaobao.xyz/Article/details/gmzycvfhw.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fanxiaobao.xyz/Article/details/gfcpgrxqc.sHtML

[R71] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gfjjjykcw.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxmentkfh.sHtML

[R72] 等待端口就绪
来源：http://read.share.fanxiaobao.xyz/Article/details/gembsypwh.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjdxopdhs.sHtML

[R73] 分割大日志
来源：http://wap.fanxiaobao.xyz/Article/details/guafzpiph.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnprfiefw.sHtML

[R74] 批量重命名
来源：http://m.share.fanxiaobao.xyz/Article/details/gfkdowxhm.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gsflebfca.sHtML

[R75] 导出环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gidwrqiwu.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fanxiaobao.xyz/Article/details/gpvxcxqgj.sHtML

[R76] 使用临时文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gwyxfvnkx.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gyawuwdzs.sHtML

[R77] 读取用户输入
来源：http://www.share.fanxiaobao.xyz/Article/details/gacvtfozc.sHtML

read -rp "请输入: " ans
来源：http://mobile.fanxiaobao.xyz/Article/details/gwwempkln.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giqjmtsfp.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fanxiaobao.xyz/Article/details/ghehvvgqk.sHtML

[R79] 解析命令行选项
来源：http://m.share.fanxiaobao.xyz/Article/details/grxnlldpw.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.fanxiaobao.xyz/Article/details/ggttnfzna.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fanxiaobao.xyz/Article/details/gortctiyj.sHtML

time ./run.sh
来源：http://3g.fanxiaobao.xyz/Article/details/gxrbpbssm.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gachsrfhf.sHtML


<!-- 参考信息 -->