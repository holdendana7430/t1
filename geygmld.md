代发 wailian999

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://m.share.zdbjq.cn/Article/details/glwhtizgr.sHtML

[Q24] 去重
来源：http://www.blog.fehbvm.com/Article/details/gicpgmatq.sHtML

SELECT DISTINCT city FROM users;
来源：http://wap.fehbvm.com/Article/details/grvagvytc.sHtML

[Q25] 只取前 N 条
来源：http://www.blog.hesvh.cn/Article/details/ghwpcbxxt.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://mobile.hesvh.cn/Article/details/gmkxyyood.sHtML

[Q26] 计数
来源：http://m.share.fehbvm.com/Article/details/ghmcfqall.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gnbhtolla.sHtML

[Q27] 条件计数
来源：http://baike.fehbvm.com/Article/details/gijqcwawe.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://m.share.zdbjq.cn/Article/details/ganvtqvja.sHtML

[Q28] 求和与平均
来源：http://baike.zdbjq.cn/Article/details/gcgiqjplk.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gewlqmttn.sHtML

[Q29] 最大最小值
来源：http://www.share.hesvh.cn/Article/details/gpamcjaio.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gukuttscb.sHtML

[Q30] 分组统计
来源：http://read.share.fehbvm.com/Article/details/gfisixort.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.zdbjq.cn/Article/details/gvqlmlgub.sHtML

[Q31] 分组后过滤
来源：http://m.share.zdbjq.cn/Article/details/gxjtvedfu.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://m.share.hesvh.cn/Article/details/guctfuiib.sHtML

[Q32] 分组拼接字符串
来源：http://blog.zdbjq.cn/Article/details/gxvvitvwq.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/grxpvpmag.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.blog.fehbvm.com/Article/details/gafmunyjw.sHtML

[Q33] 多列分组
来源：http://baike.fehbvm.com/Article/details/gfwzcltsm.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.fehbvm.com/Article/details/gcheyepvu.sHtML

[Q34] 每组取第一条
来源：http://baike.fehbvm.com/Article/details/gzkbhrhke.sHtML

SELECT * FROM (
来源：http://read.share.hesvh.cn/Article/details/gkcgnguau.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.fehbvm.com/Article/details/gyphxukfn.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gnojzxkcp.sHtML

[Q35] 内连接
来源：http://wap.zdbjq.cn/Article/details/gggdyfiwc.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.zdbjq.cn/Article/details/gpjfzufib.sHtML

[Q36] 左连接
来源：http://read.share.zdbjq.cn/Article/details/glnvoyrvw.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.hesvh.cn/Article/details/ghazsksxa.sHtML

[Q37] 右连接
来源：http://read.share.zdbjq.cn/Article/details/grqxkgtnl.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://wap.hesvh.cn/Article/details/gzejyxcik.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.fehbvm.com/Article/details/gwyvkxkjc.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.fehbvm.com/Article/details/gacikcuxc.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.hesvh.cn/Article/details/gkmpznjin.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://blog.hesvh.cn/Article/details/goxarjsje.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gargjylix.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.m.share.hesvh.cn/Article/details/gninzcbjf.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.zdbjq.cn/Article/details/gqpagfgtf.sHtML

[Q41] 多表连接
来源：http://blog.zdbjq.cn/Article/details/gybkgrxlr.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://wap.fehbvm.com/Article/details/gnvcdasaa.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.hesvh.cn/Article/details/gpqijriwz.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.fehbvm.com/Article/details/gxziwpdto.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.hesvh.cn/Article/details/gxianwies.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.fehbvm.com/Article/details/gcfyutkor.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.fehbvm.com/Article/details/gpqdhzudd.sHtML

[Q43] 标量子查询
来源：http://blog.zdbjq.cn/Article/details/gqddlshdj.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.fehbvm.com/Article/details/gyrctxtsm.sHtML

[Q44] IN 子查询
来源：http://wap.zdbjq.cn/Article/details/gmnkuufmy.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.zdbjq.cn/Article/details/gnwpycitz.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.zdbjq.cn/Article/details/gudabqcni.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.zdbjq.cn/Article/details/gbevhpmse.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.fehbvm.com/Article/details/gfgbwlscb.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.zdbjq.cn/Article/details/gnmrjnphm.sHtML

[Q47] 与平均值比较
来源：http://www.blog.hesvh.cn/Article/details/gfgpkhrtc.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.fehbvm.com/Article/details/guyqacmxj.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.hesvh.cn/Article/details/gjzwhdgpg.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.hesvh.cn/Article/details/gtewlsnzm.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://blog.zdbjq.cn/Article/details/givzefjyz.sHtML

[Q49] 更新单行
来源：http://m.share.zdbjq.cn/Article/details/geoeoiivk.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.hesvh.cn/Article/details/gdkknasak.sHtML

[Q50] 批量更新
来源：http://baike.fehbvm.com/Article/details/geaoozjyz.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.m.share.fehbvm.com/Article/details/gdrewsvnh.sHtML

[Q51] 用子查询更新
来源：http://read.share.fehbvm.com/Article/details/gxynuqtsn.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.fehbvm.com/Article/details/gnqtvkmoq.sHtML

[Q52] 删除指定行
来源：http://mobile.fehbvm.com/Article/details/gcwbzihcu.sHtML

DELETE FROM users WHERE id = 10;
来源：http://m.share.zdbjq.cn/Article/details/guszmppvq.sHtML

[Q53] 按条件删除
来源：http://wap.fehbvm.com/Article/details/giujihfts.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.hesvh.cn/Article/details/gxgwqmvvk.sHtML

[Q54] 清空表
来源：http://3g.hesvh.cn/Article/details/gctwsvfom.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.hesvh.cn/Article/details/gwirdkyzd.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.hesvh.cn/Article/details/gektbusqe.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://3g.fehbvm.com/Article/details/gsnrzxced.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.zdbjq.cn/Article/details/gmfgiebqy.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.hesvh.cn/Article/details/gwiqfllgf.sHtML

[Q57] 行号
来源：http://mobile.zdbjq.cn/Article/details/gkvgdajvb.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.zdbjq.cn/Article/details/gmwvxjhbt.sHtML

[Q58] 累计求和
来源：http://read.share.zdbjq.cn/Article/details/glcvqqobs.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.fehbvm.com/Article/details/ggxqampkh.sHtML

[Q59] 分组内累计
来源：http://3g.zdbjq.cn/Article/details/gorrhxblv.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gwdsbenlw.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.fehbvm.com/Article/details/gcajajigc.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.hesvh.cn/Article/details/gmflupplf.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.hesvh.cn/Article/details/ghmxdjlax.sHtML

[Q61] 移动平均
来源：http://baike.fehbvm.com/Article/details/gelvhcihl.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gzuxgmmnr.sHtML

[Q62] 分组占比
来源：http://wap.fehbvm.com/Article/details/ghbujbswl.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/gawuvuwsb.sHtML

[Q63] 开启事务
来源：http://read.share.zdbjq.cn/Article/details/gwbozhmov.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.fehbvm.com/Article/details/gzjbswbrr.sHtML

[Q64] 提交事务
来源：http://m.share.hesvh.cn/Article/details/gmfnrogcw.sHtML

COMMIT;
来源：http://www.blog.hesvh.cn/Article/details/gfdnfxijr.sHtML

[Q65] 回滚事务
来源：http://www.share.zdbjq.cn/Article/details/gubdcynha.sHtML

ROLLBACK;
来源：http://blog.fehbvm.com/Article/details/gszvlhimd.sHtML

[Q66] 行锁查询
来源：http://www.blog.hesvh.cn/Article/details/ghxjomgbq.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://blog.hesvh.cn/Article/details/gqxuxdlmj.sHtML

[Q67] 设置隔离级别
来源：http://baike.zdbjq.cn/Article/details/gqfqewojc.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.zdbjq.cn/Article/details/gtrfaqicy.sHtML

[Q68] 保存点
来源：http://www.blog.zdbjq.cn/Article/details/gsmqglyrg.sHtML

SAVEPOINT sp1;
来源：http://m.share.zdbjq.cn/Article/details/gxadmylya.sHtML

ROLLBACK TO sp1;
来源：http://www.m.share.zdbjq.cn/Article/details/gvhznfuod.sHtML

[Q69] 查看执行计划
来源：http://baike.fehbvm.com/Article/details/gclqegiyn.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.fehbvm.com/Article/details/gstjhiuwy.sHtML

[Q70] 更新统计信息
来源：http://read.share.zdbjq.cn/Article/details/ghczfeoaq.sHtML

ANALYZE TABLE users;
来源：http://wap.hesvh.cn/Article/details/gcoishdhy.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fehbvm.com/Article/details/gbsjvvxhu.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.hesvh.cn/Article/details/grpfcgrcd.sHtML

[Q72] 查看索引
来源：http://3g.zdbjq.cn/Article/details/gprgedcyz.sHtML

SHOW INDEX FROM users;
来源：http://mobile.hesvh.cn/Article/details/ggiowxunv.sHtML

[Q73] 查看表状态
来源：http://www.blog.zdbjq.cn/Article/details/gavqycglr.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.fehbvm.com/Article/details/gnuatyltj.sHtML

[Q74] 强制使用索引
来源：http://read.share.hesvh.cn/Article/details/gaghhjbfi.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.hesvh.cn/Article/details/gcjehpjdg.sHtML

[Q75] 日期格式化
来源：http://m.share.zdbjq.cn/Article/details/gjjtmhbjc.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.hesvh.cn/Article/details/gskjeidtg.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.hesvh.cn/Article/details/gjsdwvkqb.sHtML

[Q76] 按天统计
来源：http://m.share.fehbvm.com/Article/details/gyfiicgng.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.zdbjq.cn/Article/details/gtmxpvept.sHtML

[Q77] 时间加减
来源：http://www.share.fehbvm.com/Article/details/gkjcmabfx.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fehbvm.com/Article/details/gkazjezpy.sHtML

[Q78] 当前时间
来源：http://baike.fehbvm.com/Article/details/gulatfzxp.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.hesvh.cn/Article/details/gmpvgdtlu.sHtML

[Q79] 字符串拼接
来源：http://baike.zdbjq.cn/Article/details/gbhchgord.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.zdbjq.cn/Article/details/goxewphsj.sHtML

[Q80] 字符串截取
来源：http://3g.hesvh.cn/Article/details/gzjyiamal.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gfrfvnddk.sHtML

[Q81] 字符串替换
来源：http://3g.hesvh.cn/Article/details/gehcvrocw.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://m.share.fehbvm.com/Article/details/giuzzoujs.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.zdbjq.cn/Article/details/gxdbvooic.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/goxaowkvl.sHtML

[Q83] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/gqnlewtvb.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gjtbqcvrm.sHtML

[Q84] 去除首尾空格
来源：http://www.share.fehbvm.com/Article/details/gyhdqhket.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gotmatnzj.sHtML

[Q85] 数值取整
来源：http://www.m.share.zdbjq.cn/Article/details/gvsuoirwr.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.fehbvm.com/Article/details/gnrtvfrpd.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.hesvh.cn/Article/details/gqsmtkbxl.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.hesvh.cn/Article/details/gdsfufoob.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.hesvh.cn/Article/details/gflhghlcf.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.zdbjq.cn/Article/details/gfjztpcbt.sHtML

[Q88] 行转列（条件聚合）
来源：http://read.share.zdbjq.cn/Article/details/gofvolywg.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.fehbvm.com/Article/details/grdaiwkkv.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.zdbjq.cn/Article/details/gxyffwuly.sHtML

[Q89] 判断表是否存在
来源：http://blog.hesvh.cn/Article/details/galsqnqqz.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.fehbvm.com/Article/details/gjewytjpn.sHtML

[Q90] 生成序号列
来源：http://www.m.share.fehbvm.com/Article/details/gaalyntsb.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.fehbvm.com/Article/details/ggtodjtho.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/goruvoycu.sHtML

R. Bash 专题
来源：http://baike.hesvh.cn/Article/details/gssqwdzod.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gdfoccezz.sHtML

[R01] shebang 与严格模式
来源：http://www.share.fehbvm.com/Article/details/gbhfiizye.sHtML

#!/usr/bin/env bash
来源：http://baike.fehbvm.com/Article/details/gmcuhcdpn.sHtML

set -euo pipefail
来源：http://baike.fehbvm.com/Article/details/gihknbakd.sHtML

[R02] 变量赋值与使用
来源：http://m.share.fehbvm.com/Article/details/ggodefgog.sHtML

name="Tom"; echo "$name"
来源：http://blog.zdbjq.cn/Article/details/gxjnbcwtx.sHtML

[R03] 只读变量
来源：http://www.share.hesvh.cn/Article/details/guktsfaer.sHtML

readonly PI=3.14
来源：http://www.m.share.hesvh.cn/Article/details/gptrrvqbz.sHtML

[R04] 位置参数
来源：http://baike.fehbvm.com/Article/details/gmppjyfcq.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.zdbjq.cn/Article/details/gmychbmxv.sHtML

[R05] 参数默认值
来源：http://www.blog.zdbjq.cn/Article/details/gsxjcmrds.sHtML

name="${1:-default}"
来源：http://blog.hesvh.cn/Article/details/gxohorhqy.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.zdbjq.cn/Article/details/ghpndwkii.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fehbvm.com/Article/details/gqzktakpe.sHtML

[R07] if 判断文件
来源：http://www.blog.fehbvm.com/Article/details/gatlpzvks.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.hesvh.cn/Article/details/gaxkpgmpg.sHtML

[R08] 数值比较
来源：http://baike.hesvh.cn/Article/details/gjgyqlcmz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.fehbvm.com/Article/details/gpxpnmhex.sHtML

[R09] 字符串比较
来源：http://3g.hesvh.cn/Article/details/gqqnbiqus.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fehbvm.com/Article/details/gjwmrkqmr.sHtML

[R10] 正则匹配
来源：http://www.share.fehbvm.com/Article/details/gumusiugi.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.hesvh.cn/Article/details/gadqhjwgq.sHtML

[R11] case 多分支
来源：http://mobile.zdbjq.cn/Article/details/gkvfphilb.sHtML

case "$1" in
来源：http://3g.fehbvm.com/Article/details/gbshjwejm.sHtML

start) echo "启动" ;;
来源：http://3g.fehbvm.com/Article/details/ghyrpkboc.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fehbvm.com/Article/details/gpqqkmdfu.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.zdbjq.cn/Article/details/gujyrrnqq.sHtML

esac
来源：http://www.m.share.zdbjq.cn/Article/details/ghdszhdby.sHtML

[R12] for 遍历文件
来源：http://www.share.zdbjq.cn/Article/details/gllbkoldv.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gbkbsaodv.sHtML

[R13] for 计数循环
来源：http://www.blog.hesvh.cn/Article/details/gohhomrej.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://m.share.hesvh.cn/Article/details/gzmspmckq.sHtML

[R14] C 风格 for
来源：http://blog.fehbvm.com/Article/details/gfbojjnmq.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.m.share.hesvh.cn/Article/details/gilgijqjd.sHtML

[R15] while 逐行读文件
来源：http://3g.fehbvm.com/Article/details/gowagoqbh.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.hesvh.cn/Article/details/gwiqdvtil.sHtML

[R16] until 等待条件
来源：http://3g.zdbjq.cn/Article/details/gcunxixtn.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.zdbjq.cn/Article/details/gntqrkbjz.sHtML

[R17] 数组定义与取值
来源：http://baike.fehbvm.com/Article/details/gznteanwg.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.hesvh.cn/Article/details/goxmovwfo.sHtML

[R18] 遍历数组
来源：http://m.share.fehbvm.com/Article/details/gkwshqydm.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fehbvm.com/Article/details/gkydeugia.sHtML

[R19] 数组长度
来源：http://3g.hesvh.cn/Article/details/gkqjdysib.sHtML

echo "${#arr[@]}"
来源：http://blog.hesvh.cn/Article/details/gashbihjq.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fehbvm.com/Article/details/ghimxgkii.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fehbvm.com/Article/details/ggqfnlsmj.sHtML

[R21] 字符串长度
来源：http://mobile.zdbjq.cn/Article/details/ghqxyvgss.sHtML

echo "${#s}"
来源：http://m.share.fehbvm.com/Article/details/gevejltwu.sHtML

[R22] 截取子串
来源：http://www.m.share.zdbjq.cn/Article/details/garzgjfoo.sHtML

echo "${s:0:5}"
来源：http://m.share.fehbvm.com/Article/details/gkvknkyif.sHtML

[R23] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/gtdaxymne.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.zdbjq.cn/Article/details/ghzhgbdzh.sHtML

[R24] 大小写转换
来源：http://www.share.hesvh.cn/Article/details/gfhpsjldw.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fehbvm.com/Article/details/gldpzjcwy.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.fehbvm.com/Article/details/gyylgooic.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.hesvh.cn/Article/details/gtpskuejo.sHtML

[R26] 命令替换
来源：http://3g.zdbjq.cn/Article/details/gtlkmtzla.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fehbvm.com/Article/details/gwufygnsf.sHtML

[R27] 算术展开
来源：http://www.share.hesvh.cn/Article/details/gvtgkileu.sHtML

echo $((1 + 2 * 3))
来源：http://baike.zdbjq.cn/Article/details/gfmpdncbz.sHtML

[R28] 浮点运算
来源：http://mobile.hesvh.cn/Article/details/ghowtwusm.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.zdbjq.cn/Article/details/gtvqlpqhi.sHtML

[R29] 定义函数
来源：http://mobile.fehbvm.com/Article/details/gzyzqtbix.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.zdbjq.cn/Article/details/guzjvshvu.sHtML

[R30] 函数返回状态码
来源：http://wap.hesvh.cn/Article/details/gofztdeie.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.zdbjq.cn/Article/details/ggqmsxbkn.sHtML

[R31] 局部变量
来源：http://m.share.zdbjq.cn/Article/details/gbxzghyve.sHtML

f() { local x=1; echo "$x"; }
来源：http://baike.zdbjq.cn/Article/details/ggjqzdfkc.sHtML

[R32] 参数个数校验
来源：http://blog.zdbjq.cn/Article/details/gkdovqdok.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fehbvm.com/Article/details/gvecyzbrd.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.zdbjq.cn/Article/details/gokdckffn.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.hesvh.cn/Article/details/guxlyrapc.sHtML

[R34] 退出时清理
来源：http://www.share.fehbvm.com/Article/details/gsnqeosme.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fehbvm.com/Article/details/gpaaqhmnn.sHtML

[R35] 后台执行并等待
来源：http://wap.fehbvm.com/Article/details/gimfujbcy.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.zdbjq.cn/Article/details/gywiyxdqw.sHtML

[R36] 并发执行多个任务
来源：http://3g.fehbvm.com/Article/details/gcwzmztgt.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.zdbjq.cn/Article/details/gfpntfeut.sHtML

[R37] 把输出赋给变量
来源：http://m.share.zdbjq.cn/Article/details/gvbxpwvdj.sHtML

files=$(ls -1)
来源：http://mobile.hesvh.cn/Article/details/gaexkiein.sHtML

[R38] 管道串联
来源：http://blog.zdbjq.cn/Article/details/gwmtznvpv.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.hesvh.cn/Article/details/goleavlqn.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.zdbjq.cn/Article/details/gvgeqzfhl.sHtML

cmd > out.log 2>&1
来源：http://www.blog.zdbjq.cn/Article/details/gnunugvwk.sHtML

[R40] 追加写日志
来源：http://www.m.share.hesvh.cn/Article/details/guvnotatk.sHtML

echo "log" >> out.log
来源：http://www.share.fehbvm.com/Article/details/gvytaipvu.sHtML

[R41] 丢弃输出
来源：http://3g.hesvh.cn/Article/details/grxglzlkb.sHtML

cmd >/dev/null 2>&1
来源：http://blog.zdbjq.cn/Article/details/gkmdaklxm.sHtML

[R42] 输入重定向
来源：http://www.blog.hesvh.cn/Article/details/giuibtdbv.sHtML

wc -l < a.txt
来源：http://m.share.fehbvm.com/Article/details/gbpmfieqo.sHtML

[R43] 按名字查找文件
来源：http://mobile.fehbvm.com/Article/details/gxopdccdv.sHtML

find . -name "*.log" -type f
来源：http://mobile.zdbjq.cn/Article/details/gkyvfvuzr.sHtML

[R44] 按修改时间查找
来源：http://wap.fehbvm.com/Article/details/gcjiyymso.sHtML

find . -mtime -7 -type f
来源：http://m.share.zdbjq.cn/Article/details/gslatzhpd.sHtML

[R45] 批量删除
来源：http://www.blog.fehbvm.com/Article/details/gxvtftprj.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.zdbjq.cn/Article/details/gcxnboujj.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.zdbjq.cn/Article/details/gachwqnoj.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.zdbjq.cn/Article/details/gkbwcjjlt.sHtML

[R47] sed 单行替换
来源：http://blog.hesvh.cn/Article/details/gmsfqmhjk.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gzvpavaur.sHtML

[R48] awk 取指定列
来源：http://wap.hesvh.cn/Article/details/glqbqvjdr.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gggphccbt.sHtML

[R49] awk 带条件
来源：http://wap.fehbvm.com/Article/details/ghjggkykk.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fehbvm.com/Article/details/gmsrgtmbh.sHtML

[R50] awk 求和
来源：http://m.share.fehbvm.com/Article/details/gxojvslpf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fehbvm.com/Article/details/gspinaepk.sHtML

[R51] 排序去重取前几
来源：http://3g.zdbjq.cn/Article/details/gintsuhby.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.fehbvm.com/Article/details/gpejviocn.sHtML

[R52] 统计行数
来源：http://m.share.zdbjq.cn/Article/details/gsfshctvy.sHtML

wc -l a.txt
来源：http://www.share.hesvh.cn/Article/details/gfropyzpj.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.zdbjq.cn/Article/details/gaafkhqvu.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.hesvh.cn/Article/details/gbbcuvzvl.sHtML

[R54] 比较两个文件
来源：http://mobile.fehbvm.com/Article/details/gfpqweovj.sHtML

diff a.txt b.txt
来源：http://blog.fehbvm.com/Article/details/gkqqewsrm.sHtML

[R55] 压缩与解压
来源：http://www.share.fehbvm.com/Article/details/glzsdicwl.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.hesvh.cn/Article/details/gmklucehw.sHtML

[R56] 远程拷贝
来源：http://www.share.hesvh.cn/Article/details/gzcigzsqf.sHtML

scp file user@host:/path/
来源：http://3g.hesvh.cn/Article/details/grbskolml.sHtML

[R57] 远程执行命令
来源：http://blog.hesvh.cn/Article/details/gerhlvsrx.sHtML

ssh user@host 'uptime'
来源：http://baike.fehbvm.com/Article/details/gxkgebulv.sHtML

[R58] 下载文件
来源：http://www.m.share.fehbvm.com/Article/details/gyipjrniv.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.zdbjq.cn/Article/details/gdawelnlk.sHtML

[R59] 发 POST JSON
来源：http://mobile.zdbjq.cn/Article/details/gwlcjfnlj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fehbvm.com/Article/details/ghjfupslx.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.zdbjq.cn/Article/details/gtjfafqhn.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fehbvm.com/Article/details/gohstgmpt.sHtML

[R61] 磁盘占用
来源：http://www.share.fehbvm.com/Article/details/gkjxolvnm.sHtML

df -h;  du -sh *
来源：http://m.share.zdbjq.cn/Article/details/grogzrcpa.sHtML

[R62] 找最占空间的文件
来源：http://blog.hesvh.cn/Article/details/gqohjovau.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.hesvh.cn/Article/details/gkbqpqxus.sHtML

[R63] 内存与进程
来源：http://www.share.zdbjq.cn/Article/details/gxdgqnvzo.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.hesvh.cn/Article/details/gxurkmksp.sHtML

[R64] 结束进程
来源：http://blog.zdbjq.cn/Article/details/godrxtxmb.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.zdbjq.cn/Article/details/gapxbntpn.sHtML

[R65] 查看端口占用
来源：http://blog.fehbvm.com/Article/details/guorqiqzn.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.zdbjq.cn/Article/details/gqsndvvac.sHtML

[R66] 定时任务
来源：http://read.share.hesvh.cn/Article/details/gxizywodn.sHtML

crontab -e;  crontab -l
来源：http://baike.hesvh.cn/Article/details/gezbgvlhp.sHtML

[R67] 生成随机十六进制串
来源：http://blog.hesvh.cn/Article/details/gnetrzfki.sHtML

openssl rand -hex 16
来源：http://www.share.zdbjq.cn/Article/details/gieywujbk.sHtML

[R68] 计算文件校验值
来源：http://baike.zdbjq.cn/Article/details/gfeyopbzy.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.hesvh.cn/Article/details/gwbsuekix.sHtML

[R69] 生成随机密码
来源：http://www.m.share.zdbjq.cn/Article/details/gkstpfuxw.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.zdbjq.cn/Article/details/gnpfubzem.sHtML

[R70] 时间戳与互转
来源：http://www.share.zdbjq.cn/Article/details/ggqrtbksu.sHtML

date +%s;  date -d @1700000000
来源：http://3g.zdbjq.cn/Article/details/giaubrsde.sHtML

[R71] 日期格式化
来源：http://3g.hesvh.cn/Article/details/gjhbysume.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fehbvm.com/Article/details/ggkkvfkec.sHtML

[R72] 等待端口就绪
来源：http://wap.hesvh.cn/Article/details/gdlylsboj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.zdbjq.cn/Article/details/gxrgjcyeb.sHtML

[R73] 分割大日志
来源：http://wap.hesvh.cn/Article/details/gsvwoacds.sHtML


<!-- 参考信息 -->