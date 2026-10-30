代发 wailian999

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://baike.fanxiaobao.xyz/Article/details/gmjyanrlr.sHtML

[Q26] 计数
来源：http://wap.fanxiaobao.xyz/Article/details/ghlqcyriv.sHtML

SELECT COUNT(*) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gblnyxvgt.sHtML

[Q27] 条件计数
来源：http://read.share.fanxiaobao.xyz/Article/details/ghfdidsoy.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gkhvrszjj.sHtML

[Q28] 求和与平均
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxjxrlyou.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxtfxsype.sHtML

[Q29] 最大最小值
来源：http://wap.fanxiaobao.xyz/Article/details/gwelrmjdo.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/giiqarqix.sHtML

[Q30] 分组统计
来源：http://wap.fanxiaobao.xyz/Article/details/gwrlqqonm.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxmsljrtw.sHtML

[Q31] 分组后过滤
来源：http://baike.fanxiaobao.xyz/Article/details/ghtlcablx.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gkfvovtpp.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gvielluue.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://m.share.fanxiaobao.xyz/Article/details/guqbhrzzi.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.fanxiaobao.xyz/Article/details/gnhpdfjmz.sHtML

[Q33] 多列分组
来源：http://baike.fanxiaobao.xyz/Article/details/gseljqyoz.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.fanxiaobao.xyz/Article/details/gptnepoak.sHtML

[Q34] 每组取第一条
来源：http://blog.fanxiaobao.xyz/Article/details/gntgfsvao.sHtML

SELECT * FROM (
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gprxiplbe.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzcxbrglu.sHtML

) t WHERE rn = 1;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdekyhxoj.sHtML

[Q35] 内连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gkxyzgpal.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsfazzylg.sHtML

[Q36] 左连接
来源：http://blog.fanxiaobao.xyz/Article/details/gvpreatat.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.fanxiaobao.xyz/Article/details/guvbufvgc.sHtML

[Q37] 右连接
来源：http://3g.fanxiaobao.xyz/Article/details/gdoklcixg.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gvqzvnhit.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggfdppztc.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.fanxiaobao.xyz/Article/details/gictlafjw.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.fanxiaobao.xyz/Article/details/gmbhwenay.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.fanxiaobao.xyz/Article/details/gnbyhhirs.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.fanxiaobao.xyz/Article/details/gpmaxktqh.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.fanxiaobao.xyz/Article/details/guieidxxl.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwigfjuei.sHtML

[Q41] 多表连接
来源：http://www.share.fanxiaobao.xyz/Article/details/granvxklt.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbwdavlsp.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjbkbcrxd.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmkqjyqhs.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gshofrkmi.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.fanxiaobao.xyz/Article/details/gkcpmyrss.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.fanxiaobao.xyz/Article/details/gljdkwdmt.sHtML

[Q43] 标量子查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gvgmotkcc.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.fanxiaobao.xyz/Article/details/gajuroqaq.sHtML

[Q44] IN 子查询
来源：http://www.blog.fanxiaobao.xyz/Article/details/gncudevwy.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.fanxiaobao.xyz/Article/details/gztuvsvei.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gqcjhwayx.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.fanxiaobao.xyz/Article/details/gryzdsirk.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.fanxiaobao.xyz/Article/details/gayikayvy.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fanxiaobao.xyz/Article/details/gegpkdxyo.sHtML

[Q47] 与平均值比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gqnpescfl.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.fanxiaobao.xyz/Article/details/gncuidclc.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/gndirxsno.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.fanxiaobao.xyz/Article/details/ggqcsptoe.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwrvgrnoz.sHtML

[Q49] 更新单行
来源：http://blog.fanxiaobao.xyz/Article/details/gmldbjbkn.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gbhmpjyxt.sHtML

[Q50] 批量更新
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gajlomloo.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.fanxiaobao.xyz/Article/details/gczfxbmed.sHtML

[Q51] 用子查询更新
来源：http://baike.fanxiaobao.xyz/Article/details/gyuahpkii.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkwjyhuiq.sHtML

[Q52] 删除指定行
来源：http://wap.fanxiaobao.xyz/Article/details/gpkworhko.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gopqbmukn.sHtML

[Q53] 按条件删除
来源：http://baike.fanxiaobao.xyz/Article/details/gtnazffhp.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://baike.fanxiaobao.xyz/Article/details/gpmqrifel.sHtML

[Q54] 清空表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxlgqaogx.sHtML

TRUNCATE TABLE logs;
来源：http://baike.fanxiaobao.xyz/Article/details/gjldbzfvg.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.fanxiaobao.xyz/Article/details/gkakpwwfh.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://blog.fanxiaobao.xyz/Article/details/gveurhgku.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.fanxiaobao.xyz/Article/details/geudecmaf.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbshyvnvw.sHtML

[Q57] 行号
来源：http://m.share.fanxiaobao.xyz/Article/details/glbylzqjj.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gptwmbryo.sHtML

[Q58] 累计求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gypbnxgbe.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggklpqqqq.sHtML

[Q59] 分组内累计
来源：http://mobile.fanxiaobao.xyz/Article/details/gcnucerkn.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gqbazwivz.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.fanxiaobao.xyz/Article/details/gkthcqihe.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbglyfqhh.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwduolcsl.sHtML

[Q61] 移动平均
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gypkxpxkl.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwebqqmbd.sHtML

[Q62] 分组占比
来源：http://read.share.fanxiaobao.xyz/Article/details/gewpipldf.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.fanxiaobao.xyz/Article/details/gusoyqwvh.sHtML

[Q63] 开启事务
来源：http://wap.fanxiaobao.xyz/Article/details/gvryahxwv.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.fanxiaobao.xyz/Article/details/gccuqcqet.sHtML

[Q64] 提交事务
来源：http://www.share.fanxiaobao.xyz/Article/details/gpbsotock.sHtML

COMMIT;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghkfrhvjw.sHtML

[Q65] 回滚事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gfvqmettx.sHtML

ROLLBACK;
来源：http://3g.fanxiaobao.xyz/Article/details/grobipcee.sHtML

[Q66] 行锁查询
来源：http://3g.fanxiaobao.xyz/Article/details/gxzwmwxmc.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.fanxiaobao.xyz/Article/details/gkxoaonzc.sHtML

[Q67] 设置隔离级别
来源：http://m.share.fanxiaobao.xyz/Article/details/gcsnuxlic.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.fanxiaobao.xyz/Article/details/grplmzooo.sHtML

[Q68] 保存点
来源：http://m.share.fanxiaobao.xyz/Article/details/guesqjdju.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxpuwjcmd.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjzlmahgi.sHtML

[Q69] 查看执行计划
来源：http://m.share.fanxiaobao.xyz/Article/details/grddywbuq.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fanxiaobao.xyz/Article/details/gihzsjuqx.sHtML

[Q70] 更新统计信息
来源：http://wap.fanxiaobao.xyz/Article/details/ghyqhdmpy.sHtML

ANALYZE TABLE users;
来源：http://www.share.fanxiaobao.xyz/Article/details/giurzezua.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fanxiaobao.xyz/Article/details/gegasofiq.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fanxiaobao.xyz/Article/details/gsinryoio.sHtML

[Q72] 查看索引
来源：http://blog.fanxiaobao.xyz/Article/details/gzztshske.sHtML

SHOW INDEX FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gbplielzz.sHtML

[Q73] 查看表状态
来源：http://m.share.fanxiaobao.xyz/Article/details/goohngphk.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.fanxiaobao.xyz/Article/details/ggsbkylkv.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsgmbrngr.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbtggljot.sHtML

[Q75] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/ggnejobva.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/ghmdayxjm.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.fanxiaobao.xyz/Article/details/gbyzpwvci.sHtML

[Q76] 按天统计
来源：http://m.share.fanxiaobao.xyz/Article/details/gnvpwcats.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.share.fanxiaobao.xyz/Article/details/gijnivpqz.sHtML

[Q77] 时间加减
来源：http://baike.fanxiaobao.xyz/Article/details/gdjoehxlf.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.fanxiaobao.xyz/Article/details/gzzqgdkbz.sHtML

[Q78] 当前时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyaxvgvls.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geayrpqct.sHtML

[Q79] 字符串拼接
来源：http://wap.fanxiaobao.xyz/Article/details/gvqhgzwia.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.fanxiaobao.xyz/Article/details/gdnayebaq.sHtML

[Q80] 字符串截取
来源：http://3g.fanxiaobao.xyz/Article/details/gftimcrkd.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpzqenmbo.sHtML

[Q81] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxweeiaxh.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbyxhxfnk.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.fanxiaobao.xyz/Article/details/gmmwlsqfq.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gisoarwep.sHtML

[Q83] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/glhqdciat.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/gexfxshuu.sHtML

[Q84] 去除首尾空格
来源：http://baike.fanxiaobao.xyz/Article/details/gkeppflme.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gazwaqqkv.sHtML

[Q85] 数值取整
来源：http://www.blog.fanxiaobao.xyz/Article/details/govptalfj.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.fanxiaobao.xyz/Article/details/gukkuzsmm.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmbrqrews.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fanxiaobao.xyz/Article/details/glmvcppup.sHtML

[Q87] JSON 字段做条件
来源：http://3g.fanxiaobao.xyz/Article/details/gigolgftn.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwkhmawnv.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.fanxiaobao.xyz/Article/details/gxlhpuxnz.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://m.share.fanxiaobao.xyz/Article/details/ggatlxhmn.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzblwzcbc.sHtML

[Q89] 判断表是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gnfwpdvih.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmnwidkwq.sHtML

[Q90] 生成序号列
来源：http://blog.fanxiaobao.xyz/Article/details/gbkkxhosf.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fanxiaobao.xyz/Article/details/gynvdkprk.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/guwrdivbc.sHtML

R. Bash 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/gvktuhgps.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gltzmsvkr.sHtML

[R01] shebang 与严格模式
来源：http://blog.fanxiaobao.xyz/Article/details/ghgbsaxet.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggyaeprdu.sHtML

set -euo pipefail
来源：http://www.share.fanxiaobao.xyz/Article/details/gbcebflqh.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fanxiaobao.xyz/Article/details/gjcnwmgop.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fanxiaobao.xyz/Article/details/gurmhcovp.sHtML

[R03] 只读变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gbmpohozk.sHtML

readonly PI=3.14
来源：http://www.share.fanxiaobao.xyz/Article/details/gefyjxlcd.sHtML

[R04] 位置参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gkoviqvyl.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fanxiaobao.xyz/Article/details/geqrnnayq.sHtML

[R05] 参数默认值
来源：http://m.share.fanxiaobao.xyz/Article/details/gpgsdcdiv.sHtML

name="${1:-default}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpzglyeio.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxuknfmpq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfgraiskt.sHtML

[R07] if 判断文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gzwejxokf.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/ggnornhai.sHtML

[R08] 数值比较
来源：http://baike.fanxiaobao.xyz/Article/details/gobunddkd.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.fanxiaobao.xyz/Article/details/gklesijmx.sHtML

[R09] 字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqisvvcbu.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gkjcfmoxi.sHtML

[R10] 正则匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gupkcyenp.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/givpzklcb.sHtML

[R11] case 多分支
来源：http://3g.fanxiaobao.xyz/Article/details/ggcvxsrln.sHtML

case "$1" in
来源：http://blog.fanxiaobao.xyz/Article/details/gfziynatv.sHtML

start) echo "启动" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gqdhjjlsk.sHtML

stop)  echo "停止" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/gxxzixfkm.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpbozxkwq.sHtML

esac
来源：http://baike.fanxiaobao.xyz/Article/details/gtmfdtbwt.sHtML

[R12] for 遍历文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gvirdijqs.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gfarlwpmv.sHtML

[R13] for 计数循环
来源：http://3g.fanxiaobao.xyz/Article/details/gvlqthyny.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gpuufvioq.sHtML

[R14] C 风格 for
来源：http://3g.fanxiaobao.xyz/Article/details/guocdjvnm.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gguwgnlte.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gojxkpnxs.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gakwvzqem.sHtML

[R16] until 等待条件
来源：http://mobile.fanxiaobao.xyz/Article/details/govbgqljm.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.fanxiaobao.xyz/Article/details/gpkladnzw.sHtML

[R17] 数组定义与取值
来源：http://wap.fanxiaobao.xyz/Article/details/ghqmdnede.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gshycojaa.sHtML

[R18] 遍历数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqsiqglla.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gglwtriap.sHtML

[R19] 数组长度
来源：http://baike.fanxiaobao.xyz/Article/details/gcqunbcit.sHtML

echo "${#arr[@]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gbkwbjcmi.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grgjdrdyk.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gzhyoxsob.sHtML

[R21] 字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/garmbirec.sHtML

echo "${#s}"
来源：http://wap.fanxiaobao.xyz/Article/details/gkpavrcfp.sHtML

[R22] 截取子串
来源：http://wap.fanxiaobao.xyz/Article/details/gyluqtfta.sHtML

echo "${s:0:5}"
来源：http://wap.fanxiaobao.xyz/Article/details/gutwhujmi.sHtML

[R23] 字符串替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gzhflwiou.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fanxiaobao.xyz/Article/details/gdprqfxds.sHtML

[R24] 大小写转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gmeqdxtsy.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fanxiaobao.xyz/Article/details/gldcggyxt.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fanxiaobao.xyz/Article/details/gkvkhlujo.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fanxiaobao.xyz/Article/details/gvrcwwtcv.sHtML

[R26] 命令替换
来源：http://mobile.fanxiaobao.xyz/Article/details/ghdckkwho.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghocagfdv.sHtML

[R27] 算术展开
来源：http://read.share.fanxiaobao.xyz/Article/details/gsiqjhrwq.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fanxiaobao.xyz/Article/details/gajqphabj.sHtML

[R28] 浮点运算
来源：http://baike.fanxiaobao.xyz/Article/details/gdfcxslhg.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fanxiaobao.xyz/Article/details/giyukvumu.sHtML

[R29] 定义函数
来源：http://3g.fanxiaobao.xyz/Article/details/gdmguxqqh.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gchgpcikf.sHtML

[R30] 函数返回状态码
来源：http://baike.fanxiaobao.xyz/Article/details/ggzecnanp.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.fanxiaobao.xyz/Article/details/gudxrhvou.sHtML

[R31] 局部变量
来源：http://baike.fanxiaobao.xyz/Article/details/ginpuxkpd.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/guuueqxhe.sHtML

[R32] 参数个数校验
来源：http://m.share.fanxiaobao.xyz/Article/details/gwxkoeuxq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gllgdduzo.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fanxiaobao.xyz/Article/details/glukaqzdn.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fanxiaobao.xyz/Article/details/gjstuvovn.sHtML

[R34] 退出时清理
来源：http://read.share.fanxiaobao.xyz/Article/details/gxupsobxo.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fanxiaobao.xyz/Article/details/guuvynieu.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fanxiaobao.xyz/Article/details/gktnyhwze.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gytijzljp.sHtML

[R36] 并发执行多个任务
来源：http://m.share.fanxiaobao.xyz/Article/details/gvwhhyvmm.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fanxiaobao.xyz/Article/details/gvdtmphvg.sHtML

[R37] 把输出赋给变量
来源：http://3g.fanxiaobao.xyz/Article/details/gqgcsaywf.sHtML

files=$(ls -1)
来源：http://3g.fanxiaobao.xyz/Article/details/gwmtzewnp.sHtML

[R38] 管道串联
来源：http://mobile.fanxiaobao.xyz/Article/details/ggievfuzl.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gfggbzytd.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/gllyekgkw.sHtML

cmd > out.log 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gyjdjhunj.sHtML

[R40] 追加写日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfamlvrxw.sHtML

echo "log" >> out.log
来源：http://www.share.fanxiaobao.xyz/Article/details/glnugaejc.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmrlqfueo.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/ghqsmhsjd.sHtML

[R42] 输入重定向
来源：http://blog.fanxiaobao.xyz/Article/details/ggjwrwvnz.sHtML

wc -l < a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gaugvtpbr.sHtML

[R43] 按名字查找文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gitdcgwwk.sHtML

find . -name "*.log" -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/glbblfuga.sHtML

[R44] 按修改时间查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gslayexyo.sHtML

find . -mtime -7 -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/gwsgvntch.sHtML

[R45] 批量删除
来源：http://wap.fanxiaobao.xyz/Article/details/guxcivytl.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fanxiaobao.xyz/Article/details/gfcmptyha.sHtML

[R46] 递归替换文件内容
来源：http://3g.fanxiaobao.xyz/Article/details/gqwwftews.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fanxiaobao.xyz/Article/details/gautnvovv.sHtML

[R47] sed 单行替换
来源：http://baike.fanxiaobao.xyz/Article/details/gcujfxdmb.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gedpsdnui.sHtML

[R48] awk 取指定列
来源：http://wap.fanxiaobao.xyz/Article/details/gtxzupzra.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gyiukfzfu.sHtML

[R49] awk 带条件
来源：http://wap.fanxiaobao.xyz/Article/details/gzrnudgvb.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpqfhmmns.sHtML

[R50] awk 求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpfzkjili.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goksjunsj.sHtML

[R51] 排序去重取前几
来源：http://www.share.fanxiaobao.xyz/Article/details/gytcaopwd.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fanxiaobao.xyz/Article/details/ggkuetmfl.sHtML

[R52] 统计行数
来源：http://read.share.fanxiaobao.xyz/Article/details/gupowwuej.sHtML

wc -l a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gzpvvcopy.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fanxiaobao.xyz/Article/details/gjcflmeoz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fanxiaobao.xyz/Article/details/gdvlcqhvw.sHtML

[R54] 比较两个文件
来源：http://read.share.fanxiaobao.xyz/Article/details/giishffep.sHtML

diff a.txt b.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gbjsxgllu.sHtML

[R55] 压缩与解压
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsvwjzuki.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fanxiaobao.xyz/Article/details/gxfjhliud.sHtML

[R56] 远程拷贝
来源：http://www.blog.fanxiaobao.xyz/Article/details/gznybpueg.sHtML

scp file user@host:/path/
来源：http://baike.fanxiaobao.xyz/Article/details/gfthlrodh.sHtML

[R57] 远程执行命令
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnntpbzzr.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsbdpnxif.sHtML

[R58] 下载文件
来源：http://m.share.fanxiaobao.xyz/Article/details/ghvgdbxsv.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.fanxiaobao.xyz/Article/details/glypbfgxx.sHtML

[R59] 发 POST JSON
来源：http://blog.fanxiaobao.xyz/Article/details/gblrfuwbw.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvpeoiish.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gslmteddc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fanxiaobao.xyz/Article/details/glguwifmw.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guxluwjbo.sHtML

df -h;  du -sh *
来源：http://mobile.fanxiaobao.xyz/Article/details/ggcbmjjyc.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gppffiwyf.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyedujjgr.sHtML

[R63] 内存与进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gqfigtrex.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fanxiaobao.xyz/Article/details/gjabbsycj.sHtML

[R64] 结束进程
来源：http://m.share.fanxiaobao.xyz/Article/details/grvgqduzw.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fanxiaobao.xyz/Article/details/gawjjxwpa.sHtML

[R65] 查看端口占用
来源：http://wap.fanxiaobao.xyz/Article/details/groprfgsz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxhwkqrao.sHtML

[R66] 定时任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmgwqzaha.sHtML

crontab -e;  crontab -l
来源：http://read.share.fanxiaobao.xyz/Article/details/ghekzgzpj.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtflagwmo.sHtML

openssl rand -hex 16
来源：http://www.share.fanxiaobao.xyz/Article/details/gymxxxrgh.sHtML

[R68] 计算文件校验值
来源：http://read.share.fanxiaobao.xyz/Article/details/gjueroyar.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gbfbarjqg.sHtML

[R69] 生成随机密码
来源：http://wap.fanxiaobao.xyz/Article/details/giqczzlvk.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fanxiaobao.xyz/Article/details/giauwfyhz.sHtML

[R70] 时间戳与互转
来源：http://www.share.fanxiaobao.xyz/Article/details/gqgoxotpj.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdsgwdqdf.sHtML

[R71] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grzdnueoq.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fanxiaobao.xyz/Article/details/goirrzggk.sHtML

[R72] 等待端口就绪
来源：http://baike.fanxiaobao.xyz/Article/details/gyawxkpgo.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfltnirqz.sHtML

[R73] 分割大日志
来源：http://blog.fanxiaobao.xyz/Article/details/gqyqhjzxv.sHtML

split -l 1000 big.log part_
来源：http://baike.fanxiaobao.xyz/Article/details/gikiozevj.sHtML

[R74] 批量重命名
来源：http://read.share.fanxiaobao.xyz/Article/details/gculzbdym.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fanxiaobao.xyz/Article/details/goafapjzm.sHtML

[R75] 导出环境变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gwfvwiosr.sHtML


<!-- 参考信息 -->