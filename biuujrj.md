代发 wailian999

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.fanxiaobao.xyz/Article/details/gsvvmspqq.sHtML

[Q26] 计数
来源：http://mobile.fanxiaobao.xyz/Article/details/gqvbbzmmt.sHtML

SELECT COUNT(*) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gyuwtotvv.sHtML

[Q27] 条件计数
来源：http://blog.fanxiaobao.xyz/Article/details/gjqgnzlmj.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gszkxujun.sHtML

[Q28] 求和与平均
来源：http://blog.fanxiaobao.xyz/Article/details/gdykwzdph.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gilpdjrjz.sHtML

[Q29] 最大最小值
来源：http://read.share.fanxiaobao.xyz/Article/details/gehoatbwd.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjzqcbkno.sHtML

[Q30] 分组统计
来源：http://www.blog.fanxiaobao.xyz/Article/details/glhctqzcu.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.fanxiaobao.xyz/Article/details/gzyfgtkca.sHtML

[Q31] 分组后过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gzkjvruhf.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.fanxiaobao.xyz/Article/details/guiwxbeoa.sHtML

[Q32] 分组拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gwhrzqbxd.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.fanxiaobao.xyz/Article/details/grjpfsbac.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.fanxiaobao.xyz/Article/details/gqghsuoiy.sHtML

[Q33] 多列分组
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvgotoirn.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxobkinzq.sHtML

[Q34] 每组取第一条
来源：http://blog.fanxiaobao.xyz/Article/details/gleazzzdr.sHtML

SELECT * FROM (
来源：http://www.blog.fanxiaobao.xyz/Article/details/gryxyrcme.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.fanxiaobao.xyz/Article/details/gxdcbtbqo.sHtML

) t WHERE rn = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gniwspfzl.sHtML

[Q35] 内连接
来源：http://baike.fanxiaobao.xyz/Article/details/gfpdvbnne.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvznwryds.sHtML

[Q36] 左连接
来源：http://baike.fanxiaobao.xyz/Article/details/goxsiulhz.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gqezloqlg.sHtML

[Q37] 右连接
来源：http://baike.fanxiaobao.xyz/Article/details/gguscwcaz.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.fanxiaobao.xyz/Article/details/gtvgfqkqq.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.fanxiaobao.xyz/Article/details/gzblhtwiw.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.fanxiaobao.xyz/Article/details/gqgaqtcfw.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.fanxiaobao.xyz/Article/details/gtsujbsyu.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.fanxiaobao.xyz/Article/details/gpdnjcclg.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.fanxiaobao.xyz/Article/details/gkzmfjoie.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.fanxiaobao.xyz/Article/details/grkcagsrl.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyodzotcw.sHtML

[Q41] 多表连接
来源：http://3g.fanxiaobao.xyz/Article/details/gczkicqfb.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.fanxiaobao.xyz/Article/details/gzoocccgb.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.fanxiaobao.xyz/Article/details/ggocozplb.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.fanxiaobao.xyz/Article/details/gvtnnjmqw.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gucnxfdce.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.fanxiaobao.xyz/Article/details/gfprncfyw.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.fanxiaobao.xyz/Article/details/gwfglfhzl.sHtML

[Q43] 标量子查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gobxfchhb.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.fanxiaobao.xyz/Article/details/gthvdxybt.sHtML

[Q44] IN 子查询
来源：http://wap.fanxiaobao.xyz/Article/details/gltmllowx.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://blog.fanxiaobao.xyz/Article/details/gdwechxgv.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.fanxiaobao.xyz/Article/details/gizdgmxhd.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fanxiaobao.xyz/Article/details/gguesfrdo.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.fanxiaobao.xyz/Article/details/gpjvgsvre.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fanxiaobao.xyz/Article/details/gwqukssqq.sHtML

[Q47] 与平均值比较
来源：http://www.share.fanxiaobao.xyz/Article/details/gfdeyfnbm.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.fanxiaobao.xyz/Article/details/gwszfpnwy.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/goiidzwkw.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.fanxiaobao.xyz/Article/details/goqvtgqkb.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkmtoivgz.sHtML

[Q49] 更新单行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glaswcjoh.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gygnuzqqv.sHtML

[Q50] 批量更新
来源：http://www.share.fanxiaobao.xyz/Article/details/gqasfdrnl.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.fanxiaobao.xyz/Article/details/gvmodtecw.sHtML

[Q51] 用子查询更新
来源：http://m.share.fanxiaobao.xyz/Article/details/ggpnbyxlu.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gzfgdgmvu.sHtML

[Q52] 删除指定行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gathzbbxl.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gspachgzc.sHtML

[Q53] 按条件删除
来源：http://blog.fanxiaobao.xyz/Article/details/grcitdhdl.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.fanxiaobao.xyz/Article/details/geytqhbyu.sHtML

[Q54] 清空表
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpithzuvx.sHtML

TRUNCATE TABLE logs;
来源：http://blog.fanxiaobao.xyz/Article/details/ggjrpohag.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.fanxiaobao.xyz/Article/details/gzqjwojkl.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.fanxiaobao.xyz/Article/details/gfqnfmdjp.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.fanxiaobao.xyz/Article/details/grooxupzl.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxxzzjcvh.sHtML

[Q57] 行号
来源：http://baike.fanxiaobao.xyz/Article/details/guoavuaae.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gxacgmabr.sHtML

[Q58] 累计求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzjrthfan.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gxcyydajq.sHtML

[Q59] 分组内累计
来源：http://baike.fanxiaobao.xyz/Article/details/gnjcapjyt.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghutoyhfm.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.fanxiaobao.xyz/Article/details/gygcefldk.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fanxiaobao.xyz/Article/details/gswlyzowb.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gdwbdbsgg.sHtML

[Q61] 移动平均
来源：http://www.share.fanxiaobao.xyz/Article/details/gwdisrxto.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gjlegcpnv.sHtML

[Q62] 分组占比
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcroxegkz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbvzqeqmn.sHtML

[Q63] 开启事务
来源：http://blog.fanxiaobao.xyz/Article/details/gmbtgxqyu.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://read.share.fanxiaobao.xyz/Article/details/gdlcugakz.sHtML

[Q64] 提交事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gjoesjfkw.sHtML

COMMIT;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwefklesk.sHtML

[Q65] 回滚事务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtyixkoqk.sHtML

ROLLBACK;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gadfeviks.sHtML

[Q66] 行锁查询
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gypmhusnp.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.fanxiaobao.xyz/Article/details/gabqukstu.sHtML

[Q67] 设置隔离级别
来源：http://read.share.fanxiaobao.xyz/Article/details/gtajofqli.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.fanxiaobao.xyz/Article/details/gwhoicxvl.sHtML

[Q68] 保存点
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfwcbofhl.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gapsqivyo.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grmmwfugc.sHtML

[Q69] 查看执行计划
来源：http://baike.fanxiaobao.xyz/Article/details/grjfyvrkz.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fanxiaobao.xyz/Article/details/gcgcqwbqp.sHtML

[Q70] 更新统计信息
来源：http://wap.fanxiaobao.xyz/Article/details/gziujdmji.sHtML

ANALYZE TABLE users;
来源：http://m.share.fanxiaobao.xyz/Article/details/glzyiwque.sHtML

[Q71] 查看建表语句
来源：http://3g.fanxiaobao.xyz/Article/details/gnoloqhne.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.fanxiaobao.xyz/Article/details/gszavocbc.sHtML

[Q72] 查看索引
来源：http://blog.fanxiaobao.xyz/Article/details/grhxrcnmu.sHtML

SHOW INDEX FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gbedvnhmq.sHtML

[Q73] 查看表状态
来源：http://baike.fanxiaobao.xyz/Article/details/gazjtghyf.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.fanxiaobao.xyz/Article/details/gjyynfvxe.sHtML

[Q74] 强制使用索引
来源：http://baike.fanxiaobao.xyz/Article/details/gcbkmdqun.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.fanxiaobao.xyz/Article/details/guwpcikjx.sHtML

[Q75] 日期格式化
来源：http://www.share.fanxiaobao.xyz/Article/details/ggqxdzztn.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkzmdwiac.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fanxiaobao.xyz/Article/details/grthkhxno.sHtML

[Q76] 按天统计
来源：http://www.share.fanxiaobao.xyz/Article/details/gwrluupeb.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxwveyadn.sHtML

[Q77] 时间加减
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggzljalek.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.fanxiaobao.xyz/Article/details/gziqazrzy.sHtML

[Q78] 当前时间
来源：http://wap.fanxiaobao.xyz/Article/details/gnrbhnhez.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.fanxiaobao.xyz/Article/details/gxslbcedl.sHtML

[Q79] 字符串拼接
来源：http://wap.fanxiaobao.xyz/Article/details/gcebcjwvr.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.fanxiaobao.xyz/Article/details/grrjjjumj.sHtML

[Q80] 字符串截取
来源：http://www.blog.fanxiaobao.xyz/Article/details/goulfmnmw.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gyktotzan.sHtML

[Q81] 字符串替换
来源：http://3g.fanxiaobao.xyz/Article/details/gbsqcqiua.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gztxcrrqh.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpwymqvoz.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gycxogiji.sHtML

[Q83] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/godlkcbob.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gmsvcncxt.sHtML

[Q84] 去除首尾空格
来源：http://m.share.fanxiaobao.xyz/Article/details/gexcircxf.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gahznehgz.sHtML

[Q85] 数值取整
来源：http://m.share.fanxiaobao.xyz/Article/details/gudbkukxe.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://mobile.fanxiaobao.xyz/Article/details/gczaljrvs.sHtML

[Q86] 读取 JSON 字段
来源：http://www.share.fanxiaobao.xyz/Article/details/gdusrubxr.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.fanxiaobao.xyz/Article/details/gzsqngwou.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gdubhkufk.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fanxiaobao.xyz/Article/details/gidwsfwnd.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.fanxiaobao.xyz/Article/details/gpwiqhols.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fanxiaobao.xyz/Article/details/glyzbsabl.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzdfpwmea.sHtML

[Q89] 判断表是否存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gwfrxfxtc.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fanxiaobao.xyz/Article/details/gjngrgyrc.sHtML

[Q90] 生成序号列
来源：http://3g.fanxiaobao.xyz/Article/details/gxuzqymgy.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.fanxiaobao.xyz/Article/details/gslqgmtdz.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gjanxeagm.sHtML

R. Bash 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfpfviqbl.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/glsfwxjhb.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fanxiaobao.xyz/Article/details/gnviexedt.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goktlktkr.sHtML

set -euo pipefail
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggtoidfxl.sHtML

[R02] 变量赋值与使用
来源：http://3g.fanxiaobao.xyz/Article/details/gxrjvsrck.sHtML

name="Tom"; echo "$name"
来源：http://3g.fanxiaobao.xyz/Article/details/gmerognuf.sHtML

[R03] 只读变量
来源：http://baike.fanxiaobao.xyz/Article/details/gjibxmbff.sHtML

readonly PI=3.14
来源：http://blog.fanxiaobao.xyz/Article/details/gbvvzlfuz.sHtML

[R04] 位置参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gjbdfuhsh.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gliardcey.sHtML

[R05] 参数默认值
来源：http://3g.fanxiaobao.xyz/Article/details/gotejapdr.sHtML

name="${1:-default}"
来源：http://wap.fanxiaobao.xyz/Article/details/gdqicfmlk.sHtML

[R06] 判断命令是否存在
来源：http://3g.fanxiaobao.xyz/Article/details/gwnieuhwo.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/geyvytdlm.sHtML

[R07] if 判断文件
来源：http://m.share.fanxiaobao.xyz/Article/details/ghsxfcrqu.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/ggtrboexy.sHtML

[R08] 数值比较
来源：http://wap.fanxiaobao.xyz/Article/details/gjsfbcgjm.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gyaygjchq.sHtML

[R09] 字符串比较
来源：http://m.share.fanxiaobao.xyz/Article/details/gjknbstin.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkvpawjfb.sHtML

[R10] 正则匹配
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glpnoqulv.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gspkethvl.sHtML

[R11] case 多分支
来源：http://www.blog.fanxiaobao.xyz/Article/details/graawbcoh.sHtML

case "$1" in
来源：http://wap.fanxiaobao.xyz/Article/details/gyvecwuxs.sHtML

start) echo "启动" ;;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnwdlzqsq.sHtML

stop)  echo "停止" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gwegukqok.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkkkultnt.sHtML

esac
来源：http://read.share.fanxiaobao.xyz/Article/details/goqewhhwv.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggxvczigu.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gshuuqfjl.sHtML

[R13] for 计数循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gyzuhyzki.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gateemoih.sHtML

[R14] C 风格 for
来源：http://m.share.fanxiaobao.xyz/Article/details/gmlbojgzr.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwymdrrid.sHtML

[R15] while 逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gmmjqygvb.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggdtreytd.sHtML

[R16] until 等待条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqmsrjqzk.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gowetpplb.sHtML

[R17] 数组定义与取值
来源：http://mobile.fanxiaobao.xyz/Article/details/gdklpcxbn.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gjelqkdhu.sHtML

[R18] 遍历数组
来源：http://blog.fanxiaobao.xyz/Article/details/gluwvyomw.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gkfjfysaw.sHtML

[R19] 数组长度
来源：http://wap.fanxiaobao.xyz/Article/details/gmfkgwqwj.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gidgvrghs.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fanxiaobao.xyz/Article/details/gkxovtirc.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fanxiaobao.xyz/Article/details/gdzrdvzmm.sHtML

[R21] 字符串长度
来源：http://wap.fanxiaobao.xyz/Article/details/ghqzaxdmj.sHtML

echo "${#s}"
来源：http://wap.fanxiaobao.xyz/Article/details/gcwyrpoqx.sHtML

[R22] 截取子串
来源：http://3g.fanxiaobao.xyz/Article/details/gaaxfohat.sHtML

echo "${s:0:5}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/giqegxtzv.sHtML

[R23] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjwoosodz.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fanxiaobao.xyz/Article/details/gsmjvhptl.sHtML

[R24] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/glhojljzh.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.fanxiaobao.xyz/Article/details/ggzghmfbq.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fanxiaobao.xyz/Article/details/gxxznptkd.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fanxiaobao.xyz/Article/details/ggighnjne.sHtML

[R26] 命令替换
来源：http://read.share.fanxiaobao.xyz/Article/details/ghldtgjku.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fanxiaobao.xyz/Article/details/ggnqobvbn.sHtML

[R27] 算术展开
来源：http://wap.fanxiaobao.xyz/Article/details/gawsvjjjq.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.fanxiaobao.xyz/Article/details/gsviukbon.sHtML

[R28] 浮点运算
来源：http://read.share.fanxiaobao.xyz/Article/details/gmadhcozy.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fanxiaobao.xyz/Article/details/gtlmuhrby.sHtML

[R29] 定义函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gdkvhvily.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fanxiaobao.xyz/Article/details/geuhlxhjx.sHtML

[R30] 函数返回状态码
来源：http://read.share.fanxiaobao.xyz/Article/details/gjencaeyp.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fanxiaobao.xyz/Article/details/gbniydphp.sHtML

[R31] 局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/gfvwanxcs.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdggczekd.sHtML

[R32] 参数个数校验
来源：http://wap.fanxiaobao.xyz/Article/details/golzrrmxr.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggcadkftw.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fanxiaobao.xyz/Article/details/gefuwaooa.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fanxiaobao.xyz/Article/details/gqbiocfag.sHtML

[R34] 退出时清理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geiauaegv.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/ghtcqncmp.sHtML

[R35] 后台执行并等待
来源：http://wap.fanxiaobao.xyz/Article/details/gpgdpvxlh.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.fanxiaobao.xyz/Article/details/gjirafncg.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvpmwkjcw.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fanxiaobao.xyz/Article/details/gevltfrpw.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gdtjzbbhk.sHtML

files=$(ls -1)
来源：http://wap.fanxiaobao.xyz/Article/details/gifritkuy.sHtML

[R38] 管道串联
来源：http://www.m.share.fanxiaobao.xyz/Article/details/golbugdct.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fanxiaobao.xyz/Article/details/gsstocees.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwehsxwua.sHtML

cmd > out.log 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gfddvwoyz.sHtML

[R40] 追加写日志
来源：http://3g.fanxiaobao.xyz/Article/details/gyfuhobzw.sHtML

echo "log" >> out.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gcemngzrp.sHtML

[R41] 丢弃输出
来源：http://3g.fanxiaobao.xyz/Article/details/gahtgtreb.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fanxiaobao.xyz/Article/details/gmppnykwv.sHtML

[R42] 输入重定向
来源：http://3g.fanxiaobao.xyz/Article/details/gpoxxjpcm.sHtML

wc -l < a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gkqncxhug.sHtML

[R43] 按名字查找文件
来源：http://wap.fanxiaobao.xyz/Article/details/graihyumn.sHtML

find . -name "*.log" -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gygyjhbxr.sHtML

[R44] 按修改时间查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gtsdfigyx.sHtML

find . -mtime -7 -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gsopjrlyj.sHtML

[R45] 批量删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghizxejdr.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpryqwlxq.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaagqjrwm.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggcmbatma.sHtML

[R47] sed 单行替换
来源：http://wap.fanxiaobao.xyz/Article/details/ghaqpnpbc.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gqdayiodi.sHtML

[R48] awk 取指定列
来源：http://read.share.fanxiaobao.xyz/Article/details/gzrevlxbe.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gysgrlerd.sHtML

[R49] awk 带条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gmqsgqnzl.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fanxiaobao.xyz/Article/details/gcnfgjcnb.sHtML

[R50] awk 求和
来源：http://m.share.fanxiaobao.xyz/Article/details/giwdwoawt.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gvycustxp.sHtML

[R51] 排序去重取前几
来源：http://read.share.fanxiaobao.xyz/Article/details/gxvrpedet.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fanxiaobao.xyz/Article/details/gjyjgmows.sHtML

[R52] 统计行数
来源：http://mobile.fanxiaobao.xyz/Article/details/gyxawymgf.sHtML

wc -l a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gwzreverq.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fanxiaobao.xyz/Article/details/gmmnnacvg.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gsoowngtb.sHtML

[R54] 比较两个文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gahljalwj.sHtML

diff a.txt b.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gyttxinym.sHtML

[R55] 压缩与解压
来源：http://mobile.fanxiaobao.xyz/Article/details/gzaxcdoyy.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.fanxiaobao.xyz/Article/details/glxaysvvd.sHtML

[R56] 远程拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gmmbxnsrc.sHtML

scp file user@host:/path/
来源：http://wap.fanxiaobao.xyz/Article/details/gzuwtknfz.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glyygruey.sHtML

ssh user@host 'uptime'
来源：http://www.share.fanxiaobao.xyz/Article/details/gtmkaryaj.sHtML

[R58] 下载文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gffrejuvb.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fanxiaobao.xyz/Article/details/gujjwheas.sHtML

[R59] 发 POST JSON
来源：http://blog.fanxiaobao.xyz/Article/details/gcodlbgdn.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fanxiaobao.xyz/Article/details/gtuklgukq.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gxmbzubqa.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/gibdilfji.sHtML

[R61] 磁盘占用
来源：http://blog.fanxiaobao.xyz/Article/details/guoomtwki.sHtML

df -h;  du -sh *
来源：http://3g.fanxiaobao.xyz/Article/details/gwlftzblx.sHtML

[R62] 找最占空间的文件
来源：http://baike.fanxiaobao.xyz/Article/details/gtvtaqbgi.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fanxiaobao.xyz/Article/details/gekssvatx.sHtML

[R63] 内存与进程
来源：http://3g.fanxiaobao.xyz/Article/details/gdidukank.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fanxiaobao.xyz/Article/details/guyxzlfvs.sHtML

[R64] 结束进程
来源：http://read.share.fanxiaobao.xyz/Article/details/gfauobyfx.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geijzdkgk.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gezfqxszo.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fanxiaobao.xyz/Article/details/gvjudlvyz.sHtML

[R66] 定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/gcilwweot.sHtML

crontab -e;  crontab -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gjmnzncmi.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmavmkhpv.sHtML

openssl rand -hex 16
来源：http://blog.fanxiaobao.xyz/Article/details/gwrlmoubg.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gopsgeqvj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gnvotwzud.sHtML

[R69] 生成随机密码
来源：http://wap.fanxiaobao.xyz/Article/details/gwfagyhht.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fanxiaobao.xyz/Article/details/gzysigttx.sHtML

[R70] 时间戳与互转
来源：http://www.share.fanxiaobao.xyz/Article/details/grcbnvdxh.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fanxiaobao.xyz/Article/details/gfxeqwdks.sHtML

[R71] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gyxiwjedu.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghwlsoexv.sHtML

[R72] 等待端口就绪
来源：http://www.share.fanxiaobao.xyz/Article/details/grhkmgyps.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gefqiduel.sHtML

[R73] 分割大日志
来源：http://www.share.fanxiaobao.xyz/Article/details/gglxghmmx.sHtML

split -l 1000 big.log part_
来源：http://baike.fanxiaobao.xyz/Article/details/gbbzhtxde.sHtML

[R74] 批量重命名
来源：http://3g.fanxiaobao.xyz/Article/details/gwildcrjr.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fanxiaobao.xyz/Article/details/ggesrrbqw.sHtML

[R75] 导出环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/grvflnmub.sHtML


<!-- 参考信息 -->