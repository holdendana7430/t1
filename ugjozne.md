代发 wailian999

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.blog.zdbjq.cn/Article/details/gsslvrvlv.sHtML

[Q24] 去重
来源：http://www.share.hesvh.cn/Article/details/gvmgvxwfm.sHtML

SELECT DISTINCT city FROM users;
来源：http://m.share.fehbvm.com/Article/details/glwunbxss.sHtML

[Q25] 只取前 N 条
来源：http://mobile.fehbvm.com/Article/details/gylhbuvgu.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.zdbjq.cn/Article/details/gtlbrufmc.sHtML

[Q26] 计数
来源：http://read.share.fehbvm.com/Article/details/ghxidjtwo.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gvqmnczhq.sHtML

[Q27] 条件计数
来源：http://read.share.zdbjq.cn/Article/details/geofizrjp.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.hesvh.cn/Article/details/grkhudsku.sHtML

[Q28] 求和与平均
来源：http://wap.fehbvm.com/Article/details/grutdbjlp.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gqgdrvdgn.sHtML

[Q29] 最大最小值
来源：http://mobile.hesvh.cn/Article/details/gffsgnbim.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.zdbjq.cn/Article/details/ggxsdcrti.sHtML

[Q30] 分组统计
来源：http://mobile.zdbjq.cn/Article/details/glbinlpem.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/gqtlzhban.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.fehbvm.com/Article/details/gdeqclvbq.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://blog.fehbvm.com/Article/details/gdajxttop.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/gemmkvdag.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gjiosgtwn.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://baike.fehbvm.com/Article/details/gpqxcixkp.sHtML

[Q33] 多列分组
来源：http://mobile.zdbjq.cn/Article/details/gikwhryti.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.fehbvm.com/Article/details/ghxpmmupo.sHtML

[Q34] 每组取第一条
来源：http://blog.fehbvm.com/Article/details/gqpdophci.sHtML

SELECT * FROM (
来源：http://m.share.fehbvm.com/Article/details/gvpqofotm.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://read.share.hesvh.cn/Article/details/ggevzdnnx.sHtML

) t WHERE rn = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gifpikqfn.sHtML

[Q35] 内连接
来源：http://wap.fehbvm.com/Article/details/gosdhinme.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fehbvm.com/Article/details/gwjrzggie.sHtML

[Q36] 左连接
来源：http://www.m.share.fehbvm.com/Article/details/gtjczkdvl.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fehbvm.com/Article/details/gofwbqxsn.sHtML

[Q37] 右连接
来源：http://www.share.fehbvm.com/Article/details/gjefbyxlf.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.fehbvm.com/Article/details/gyvhnebpx.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.hesvh.cn/Article/details/gfcmdsdts.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.zdbjq.cn/Article/details/gsjlfhkrq.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.hesvh.cn/Article/details/gqrsmficw.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.zdbjq.cn/Article/details/gjuegyvgm.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.fehbvm.com/Article/details/ggbpmrece.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.hesvh.cn/Article/details/gkormdsst.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.m.share.zdbjq.cn/Article/details/goccgzxrn.sHtML

[Q41] 多表连接
来源：http://read.share.zdbjq.cn/Article/details/gtfoyqmai.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.hesvh.cn/Article/details/gxuuxnius.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.hesvh.cn/Article/details/gzforcwyg.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.hesvh.cn/Article/details/gzrmyrjmg.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.fehbvm.com/Article/details/gvgzxopbo.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.hesvh.cn/Article/details/glxoamrap.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.zdbjq.cn/Article/details/gtdvtynsz.sHtML

[Q43] 标量子查询
来源：http://www.blog.zdbjq.cn/Article/details/gffzidevg.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.fehbvm.com/Article/details/gywlkftkw.sHtML

[Q44] IN 子查询
来源：http://m.share.hesvh.cn/Article/details/gpaafffql.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.hesvh.cn/Article/details/gmzukpzjq.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.fehbvm.com/Article/details/gnvlhlarc.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.fehbvm.com/Article/details/gqmczhoid.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.fehbvm.com/Article/details/gqdntgcnl.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.hesvh.cn/Article/details/gkbfzvgws.sHtML

[Q47] 与平均值比较
来源：http://m.share.zdbjq.cn/Article/details/gnlsjyikm.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.fehbvm.com/Article/details/gaybnnder.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.fehbvm.com/Article/details/gqrswwayt.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.share.hesvh.cn/Article/details/gqppaptso.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.zdbjq.cn/Article/details/ghluxfisj.sHtML

[Q49] 更新单行
来源：http://www.share.fehbvm.com/Article/details/gowgwuatb.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.zdbjq.cn/Article/details/gnegovzik.sHtML

[Q50] 批量更新
来源：http://www.m.share.fehbvm.com/Article/details/goezicurv.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.fehbvm.com/Article/details/ghxaenxgu.sHtML

[Q51] 用子查询更新
来源：http://read.share.hesvh.cn/Article/details/gtkjrabpo.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.hesvh.cn/Article/details/giladourt.sHtML

[Q52] 删除指定行
来源：http://www.blog.hesvh.cn/Article/details/gellkufph.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.zdbjq.cn/Article/details/gzxtuwian.sHtML

[Q53] 按条件删除
来源：http://read.share.zdbjq.cn/Article/details/gtjltgagk.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://blog.fehbvm.com/Article/details/gggdcedkv.sHtML

[Q54] 清空表
来源：http://read.share.hesvh.cn/Article/details/grrfsntpf.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.fehbvm.com/Article/details/gpzkiijbh.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.fehbvm.com/Article/details/gsfscuqvv.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.fehbvm.com/Article/details/gbyfdyqed.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.fehbvm.com/Article/details/gkxaqyitk.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.zdbjq.cn/Article/details/gowdmvevy.sHtML

[Q57] 行号
来源：http://www.share.fehbvm.com/Article/details/gqiflxitj.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.zdbjq.cn/Article/details/gsgbgtoxk.sHtML

[Q58] 累计求和
来源：http://m.share.zdbjq.cn/Article/details/glmhjruqg.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.hesvh.cn/Article/details/grtitrfxl.sHtML

[Q59] 分组内累计
来源：http://www.m.share.fehbvm.com/Article/details/gxlnudpis.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.hesvh.cn/Article/details/gpkvulwbc.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.hesvh.cn/Article/details/gdqfmgymu.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://m.share.fehbvm.com/Article/details/gdbxgjquw.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gtrhlybkk.sHtML

[Q61] 移动平均
来源：http://www.blog.fehbvm.com/Article/details/gtajlkbfq.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gamdtmrfm.sHtML

[Q62] 分组占比
来源：http://baike.zdbjq.cn/Article/details/gwhwcvapc.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/gnaogahgz.sHtML

[Q63] 开启事务
来源：http://www.share.hesvh.cn/Article/details/gjqhhitya.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.zdbjq.cn/Article/details/gbraosdez.sHtML

[Q64] 提交事务
来源：http://3g.zdbjq.cn/Article/details/gcsewlgwn.sHtML

COMMIT;
来源：http://www.share.hesvh.cn/Article/details/gnqnifavd.sHtML

[Q65] 回滚事务
来源：http://3g.hesvh.cn/Article/details/gvgyxtfhi.sHtML

ROLLBACK;
来源：http://wap.fehbvm.com/Article/details/gnmpzseub.sHtML

[Q66] 行锁查询
来源：http://www.m.share.zdbjq.cn/Article/details/gjrdrlogn.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.hesvh.cn/Article/details/gshagvube.sHtML

[Q67] 设置隔离级别
来源：http://blog.fehbvm.com/Article/details/gagwmzhqf.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://m.share.hesvh.cn/Article/details/gralkahev.sHtML

[Q68] 保存点
来源：http://mobile.zdbjq.cn/Article/details/gopliatlb.sHtML

SAVEPOINT sp1;
来源：http://mobile.fehbvm.com/Article/details/glqzbmtin.sHtML

ROLLBACK TO sp1;
来源：http://read.share.zdbjq.cn/Article/details/gfwxnznfz.sHtML

[Q69] 查看执行计划
来源：http://www.m.share.fehbvm.com/Article/details/gukbkunbc.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.zdbjq.cn/Article/details/gasnwwiro.sHtML

[Q70] 更新统计信息
来源：http://mobile.zdbjq.cn/Article/details/gdbancwkf.sHtML

ANALYZE TABLE users;
来源：http://blog.hesvh.cn/Article/details/ggjigrdju.sHtML

[Q71] 查看建表语句
来源：http://read.share.zdbjq.cn/Article/details/gsuxhinzn.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.hesvh.cn/Article/details/gzgqlukux.sHtML

[Q72] 查看索引
来源：http://wap.hesvh.cn/Article/details/gmimqatid.sHtML

SHOW INDEX FROM users;
来源：http://baike.fehbvm.com/Article/details/gmwpuyiht.sHtML

[Q73] 查看表状态
来源：http://wap.hesvh.cn/Article/details/glipyxnkp.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.hesvh.cn/Article/details/gcgiryjnk.sHtML

[Q74] 强制使用索引
来源：http://www.blog.hesvh.cn/Article/details/gnvojfzqo.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://mobile.hesvh.cn/Article/details/gcomshxin.sHtML

[Q75] 日期格式化
来源：http://mobile.hesvh.cn/Article/details/gscssivld.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gktddimba.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.m.share.fehbvm.com/Article/details/gjzajumkv.sHtML

[Q76] 按天统计
来源：http://m.share.hesvh.cn/Article/details/gczbwwurw.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.fehbvm.com/Article/details/gtqglptor.sHtML

[Q77] 时间加减
来源：http://blog.zdbjq.cn/Article/details/gbmaxavtk.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.zdbjq.cn/Article/details/gbcrdlwpe.sHtML

[Q78] 当前时间
来源：http://wap.zdbjq.cn/Article/details/ghsewubay.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.fehbvm.com/Article/details/glgpectqc.sHtML

[Q79] 字符串拼接
来源：http://m.share.hesvh.cn/Article/details/gvjfmhkeu.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.hesvh.cn/Article/details/gekcikfse.sHtML

[Q80] 字符串截取
来源：http://www.share.fehbvm.com/Article/details/gckzfallc.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gwdxnsjut.sHtML

[Q81] 字符串替换
来源：http://mobile.zdbjq.cn/Article/details/gempxrymp.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://3g.zdbjq.cn/Article/details/guqbjwnxc.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fehbvm.com/Article/details/gktkwvjht.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gxvrwitca.sHtML

[Q83] 大小写转换
来源：http://blog.hesvh.cn/Article/details/ghtmutktl.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/ghwpzwicj.sHtML

[Q84] 去除首尾空格
来源：http://m.share.fehbvm.com/Article/details/gsldbmqcl.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gnjknryfd.sHtML

[Q85] 数值取整
来源：http://blog.hesvh.cn/Article/details/glmryyxdw.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.hesvh.cn/Article/details/gpsrzuhkr.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.hesvh.cn/Article/details/gnolxycpb.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.fehbvm.com/Article/details/gghontgdn.sHtML

[Q87] JSON 字段做条件
来源：http://www.blog.zdbjq.cn/Article/details/gptexlcvh.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.fehbvm.com/Article/details/golnueoco.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.hesvh.cn/Article/details/genshpydh.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.hesvh.cn/Article/details/gvfheriyw.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gyolhxdzq.sHtML

[Q89] 判断表是否存在
来源：http://wap.hesvh.cn/Article/details/gsohwqyhz.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.zdbjq.cn/Article/details/gwzpqczrp.sHtML

[Q90] 生成序号列
来源：http://www.share.hesvh.cn/Article/details/gdyydceoz.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://read.share.hesvh.cn/Article/details/gjqfskhwa.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/glovotnvx.sHtML

R. Bash 专题
来源：http://baike.zdbjq.cn/Article/details/gxrxzhadq.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gzrhxcekp.sHtML

[R01] shebang 与严格模式
来源：http://m.share.hesvh.cn/Article/details/gltmscfgp.sHtML

#!/usr/bin/env bash
来源：http://read.share.fehbvm.com/Article/details/guijmfbnu.sHtML

set -euo pipefail
来源：http://mobile.fehbvm.com/Article/details/guhyrtuxy.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fehbvm.com/Article/details/gdmgxvjkg.sHtML

name="Tom"; echo "$name"
来源：http://read.share.fehbvm.com/Article/details/gullimoii.sHtML

[R03] 只读变量
来源：http://www.m.share.fehbvm.com/Article/details/grudnggiz.sHtML

readonly PI=3.14
来源：http://3g.zdbjq.cn/Article/details/grhlkumih.sHtML

[R04] 位置参数
来源：http://www.m.share.hesvh.cn/Article/details/gamnvvqwo.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.hesvh.cn/Article/details/gaetqvbvd.sHtML

[R05] 参数默认值
来源：http://blog.fehbvm.com/Article/details/gtrtytpay.sHtML

name="${1:-default}"
来源：http://mobile.zdbjq.cn/Article/details/gxefgjhbi.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.hesvh.cn/Article/details/grzxhbfgv.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.fehbvm.com/Article/details/gcbbyvisi.sHtML

[R07] if 判断文件
来源：http://www.share.fehbvm.com/Article/details/gtggkeqek.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.zdbjq.cn/Article/details/gcomblwwv.sHtML

[R08] 数值比较
来源：http://m.share.hesvh.cn/Article/details/gkzdyxcuk.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.hesvh.cn/Article/details/gfottzqeg.sHtML

[R09] 字符串比较
来源：http://wap.hesvh.cn/Article/details/gpdjyhglt.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.zdbjq.cn/Article/details/goqglbrzd.sHtML

[R10] 正则匹配
来源：http://www.share.fehbvm.com/Article/details/gvojzoukm.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://3g.zdbjq.cn/Article/details/ggpbsqmwh.sHtML

[R11] case 多分支
来源：http://read.share.fehbvm.com/Article/details/glaonoqnk.sHtML

case "$1" in
来源：http://baike.fehbvm.com/Article/details/gxpohtzdi.sHtML

start) echo "启动" ;;
来源：http://mobile.zdbjq.cn/Article/details/gwmfpfsow.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gjoecngbm.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fehbvm.com/Article/details/gvnhmjjwb.sHtML

esac
来源：http://m.share.hesvh.cn/Article/details/grkcbkagk.sHtML

[R12] for 遍历文件
来源：http://m.share.fehbvm.com/Article/details/gedqoptbc.sHtML

for f in *.txt; do echo "$f"; done
来源：http://mobile.hesvh.cn/Article/details/glsdwhhvg.sHtML

[R13] for 计数循环
来源：http://3g.zdbjq.cn/Article/details/glechgvel.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.hesvh.cn/Article/details/gitdeawgw.sHtML

[R14] C 风格 for
来源：http://blog.zdbjq.cn/Article/details/ggbswwpzx.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.hesvh.cn/Article/details/ghkepczdp.sHtML

[R15] while 逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gwejhuldb.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fehbvm.com/Article/details/gahrmnzch.sHtML

[R16] until 等待条件
来源：http://mobile.fehbvm.com/Article/details/gfglhgfgf.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.hesvh.cn/Article/details/gctlcqlum.sHtML

[R17] 数组定义与取值
来源：http://blog.zdbjq.cn/Article/details/grctleejn.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fehbvm.com/Article/details/gsbmwpjul.sHtML

[R18] 遍历数组
来源：http://wap.hesvh.cn/Article/details/gndwajthi.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.hesvh.cn/Article/details/gqosniunn.sHtML

[R19] 数组长度
来源：http://mobile.zdbjq.cn/Article/details/gffgceizf.sHtML

echo "${#arr[@]}"
来源：http://www.share.fehbvm.com/Article/details/glgvenvaq.sHtML

[R20] 关联数组（字典）
来源：http://wap.hesvh.cn/Article/details/gzzrbpydw.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.zdbjq.cn/Article/details/gtmipasmb.sHtML

[R21] 字符串长度
来源：http://www.share.fehbvm.com/Article/details/gbskfpnlg.sHtML

echo "${#s}"
来源：http://wap.zdbjq.cn/Article/details/gsrbxhusv.sHtML

[R22] 截取子串
来源：http://www.m.share.zdbjq.cn/Article/details/glmqohztt.sHtML

echo "${s:0:5}"
来源：http://m.share.fehbvm.com/Article/details/gtlhyexiy.sHtML

[R23] 字符串替换
来源：http://mobile.fehbvm.com/Article/details/goegfyktd.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.hesvh.cn/Article/details/gzefiqjyw.sHtML

[R24] 大小写转换
来源：http://3g.fehbvm.com/Article/details/gvatjnudu.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.zdbjq.cn/Article/details/gthkvsqhs.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.hesvh.cn/Article/details/getouobsk.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fehbvm.com/Article/details/gbkpmorxx.sHtML

[R26] 命令替换
来源：http://baike.zdbjq.cn/Article/details/gwynrpmfl.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.hesvh.cn/Article/details/gwiybktuq.sHtML

[R27] 算术展开
来源：http://blog.fehbvm.com/Article/details/gzdvwtixk.sHtML

echo $((1 + 2 * 3))
来源：http://baike.fehbvm.com/Article/details/gneufhemo.sHtML

[R28] 浮点运算
来源：http://m.share.fehbvm.com/Article/details/gojezisms.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fehbvm.com/Article/details/gpwqtxrlt.sHtML

[R29] 定义函数
来源：http://mobile.hesvh.cn/Article/details/gaippirtp.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.hesvh.cn/Article/details/gnpjaxqfl.sHtML

[R30] 函数返回状态码
来源：http://m.share.fehbvm.com/Article/details/ghdkecuii.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.zdbjq.cn/Article/details/gznhbizsv.sHtML

[R31] 局部变量
来源：http://wap.fehbvm.com/Article/details/gkcgtmubj.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fehbvm.com/Article/details/gietmoxrx.sHtML

[R32] 参数个数校验
来源：http://blog.fehbvm.com/Article/details/glllyrkvx.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.hesvh.cn/Article/details/gklcfwqqz.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fehbvm.com/Article/details/guyvgiskk.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.hesvh.cn/Article/details/gvovmbfao.sHtML

[R34] 退出时清理
来源：http://www.share.zdbjq.cn/Article/details/gfgiibcmj.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gqqodtbgu.sHtML

[R35] 后台执行并等待
来源：http://www.share.fehbvm.com/Article/details/giknfyzqz.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.zdbjq.cn/Article/details/gimogogyr.sHtML

[R36] 并发执行多个任务
来源：http://m.share.hesvh.cn/Article/details/gofecegwv.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fehbvm.com/Article/details/gijvvuwef.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fehbvm.com/Article/details/gmqifjjzn.sHtML

files=$(ls -1)
来源：http://m.share.hesvh.cn/Article/details/gkmjtotta.sHtML

[R38] 管道串联
来源：http://mobile.zdbjq.cn/Article/details/gpqujxyce.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fehbvm.com/Article/details/ggvimxrhw.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.zdbjq.cn/Article/details/gsoznmver.sHtML

cmd > out.log 2>&1
来源：http://3g.fehbvm.com/Article/details/grhpiptcc.sHtML

[R40] 追加写日志
来源：http://read.share.zdbjq.cn/Article/details/gceyovbyy.sHtML

echo "log" >> out.log
来源：http://www.blog.hesvh.cn/Article/details/gjlnwhspj.sHtML

[R41] 丢弃输出
来源：http://3g.zdbjq.cn/Article/details/gaoemoqoy.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.hesvh.cn/Article/details/gearfsrwh.sHtML

[R42] 输入重定向
来源：http://baike.zdbjq.cn/Article/details/grewzuxpe.sHtML

wc -l < a.txt
来源：http://baike.hesvh.cn/Article/details/giofumvpy.sHtML

[R43] 按名字查找文件
来源：http://m.share.hesvh.cn/Article/details/gakunrdvn.sHtML

find . -name "*.log" -type f
来源：http://mobile.zdbjq.cn/Article/details/gltcwyham.sHtML

[R44] 按修改时间查找
来源：http://m.share.zdbjq.cn/Article/details/gkdceqxxe.sHtML

find . -mtime -7 -type f
来源：http://www.share.fehbvm.com/Article/details/gvnmewzlm.sHtML

[R45] 批量删除
来源：http://m.share.hesvh.cn/Article/details/gzftkmhww.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.zdbjq.cn/Article/details/gscdrlapv.sHtML

[R46] 递归替换文件内容
来源：http://wap.hesvh.cn/Article/details/ggrolxdvk.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.hesvh.cn/Article/details/gtacejzxu.sHtML

[R47] sed 单行替换
来源：http://www.share.zdbjq.cn/Article/details/gthxjitxd.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.hesvh.cn/Article/details/gklbxlawo.sHtML

[R48] awk 取指定列
来源：http://baike.hesvh.cn/Article/details/gghbermeu.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.hesvh.cn/Article/details/gfsscifnn.sHtML

[R49] awk 带条件
来源：http://mobile.zdbjq.cn/Article/details/gvksphnkq.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.hesvh.cn/Article/details/gvnimozrk.sHtML

[R50] awk 求和
来源：http://3g.zdbjq.cn/Article/details/grepmuoin.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fehbvm.com/Article/details/gueyhtwrd.sHtML

[R51] 排序去重取前几
来源：http://read.share.zdbjq.cn/Article/details/gflhhpsla.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.hesvh.cn/Article/details/gnvstrlwh.sHtML

[R52] 统计行数
来源：http://read.share.fehbvm.com/Article/details/gqbqzkgnx.sHtML

wc -l a.txt
来源：http://m.share.hesvh.cn/Article/details/girwuiyak.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.zdbjq.cn/Article/details/gvlaytnlf.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fehbvm.com/Article/details/gxittyofe.sHtML

[R54] 比较两个文件
来源：http://www.share.zdbjq.cn/Article/details/ghjkmoxjd.sHtML

diff a.txt b.txt
来源：http://www.m.share.fehbvm.com/Article/details/gdzvyiqcy.sHtML

[R55] 压缩与解压
来源：http://www.m.share.hesvh.cn/Article/details/gtpjnoahe.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fehbvm.com/Article/details/gltdirhuu.sHtML

[R56] 远程拷贝
来源：http://3g.zdbjq.cn/Article/details/gpwdxrfur.sHtML

scp file user@host:/path/
来源：http://www.blog.fehbvm.com/Article/details/gbovmlsqd.sHtML

[R57] 远程执行命令
来源：http://baike.fehbvm.com/Article/details/glsvouysx.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fehbvm.com/Article/details/gsiexxxgl.sHtML

[R58] 下载文件
来源：http://wap.fehbvm.com/Article/details/gcfpwukep.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fehbvm.com/Article/details/gtnvtgdtb.sHtML

[R59] 发 POST JSON
来源：http://blog.zdbjq.cn/Article/details/gbzrvazrc.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.zdbjq.cn/Article/details/gacriafvj.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.hesvh.cn/Article/details/gkqgjkurn.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.hesvh.cn/Article/details/gliiqyjuq.sHtML

[R61] 磁盘占用
来源：http://read.share.hesvh.cn/Article/details/ghddbyyot.sHtML

df -h;  du -sh *
来源：http://wap.hesvh.cn/Article/details/gjdigdpcu.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.zdbjq.cn/Article/details/gyzivdfbn.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.hesvh.cn/Article/details/gtilfhxzx.sHtML

[R63] 内存与进程
来源：http://blog.zdbjq.cn/Article/details/gwtswrwzl.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.hesvh.cn/Article/details/giotahskx.sHtML

[R64] 结束进程
来源：http://3g.zdbjq.cn/Article/details/gzlgqjhxb.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.zdbjq.cn/Article/details/gcehkathk.sHtML

[R65] 查看端口占用
来源：http://read.share.fehbvm.com/Article/details/gbwjqlojg.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.hesvh.cn/Article/details/gkbdboiyh.sHtML

[R66] 定时任务
来源：http://blog.zdbjq.cn/Article/details/gadzjvzdb.sHtML

crontab -e;  crontab -l
来源：http://mobile.zdbjq.cn/Article/details/garezgbcr.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.hesvh.cn/Article/details/gxipwhvpk.sHtML

openssl rand -hex 16
来源：http://www.m.share.fehbvm.com/Article/details/gqccipgmi.sHtML

[R68] 计算文件校验值
来源：http://mobile.hesvh.cn/Article/details/gsfhhhkpg.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fehbvm.com/Article/details/gafoxmxzh.sHtML

[R69] 生成随机密码
来源：http://3g.hesvh.cn/Article/details/gfckkoayx.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.hesvh.cn/Article/details/goxyizrbw.sHtML

[R70] 时间戳与互转
来源：http://blog.fehbvm.com/Article/details/gujttqchz.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.zdbjq.cn/Article/details/gdtlssotg.sHtML

[R71] 日期格式化
来源：http://read.share.zdbjq.cn/Article/details/gdfjtcjhd.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fehbvm.com/Article/details/grplxcnvk.sHtML

[R72] 等待端口就绪
来源：http://mobile.hesvh.cn/Article/details/gqddvcvpc.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/ghmnurwym.sHtML

[R73] 分割大日志
来源：http://www.m.share.zdbjq.cn/Article/details/gfblykghx.sHtML


<!-- 参考信息 -->