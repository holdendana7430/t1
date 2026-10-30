代发 wailian999

SELECT * FROM users WHERE email IS NULL;
来源：http://www.m.share.hesvh.cn/Article/details/gbnhknzlc.sHtML

[Q22] 排序
来源：http://3g.zdbjq.cn/Article/details/ggsihtmvz.sHtML

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.share.fehbvm.com/Article/details/ggqdpjoxv.sHtML

[Q23] 分页
来源：http://www.share.hesvh.cn/Article/details/gwziqqors.sHtML

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.m.share.zdbjq.cn/Article/details/gbyilykwy.sHtML

[Q24] 去重
来源：http://mobile.fehbvm.com/Article/details/gyiuoohxx.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gbszdfthl.sHtML

[Q25] 只取前 N 条
来源：http://read.share.fehbvm.com/Article/details/gyqrcvvbo.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.hesvh.cn/Article/details/ghhuutsds.sHtML

[Q26] 计数
来源：http://www.m.share.zdbjq.cn/Article/details/gfikgfwtf.sHtML

SELECT COUNT(*) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gkpyfecsc.sHtML

[Q27] 条件计数
来源：http://www.blog.fehbvm.com/Article/details/gaekjsgua.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://blog.hesvh.cn/Article/details/gxnfglfiq.sHtML

[Q28] 求和与平均
来源：http://blog.fehbvm.com/Article/details/gipybfzqm.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/grxzgeeav.sHtML

[Q29] 最大最小值
来源：http://www.m.share.zdbjq.cn/Article/details/gnaytwxsh.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gjmulwwyq.sHtML

[Q30] 分组统计
来源：http://blog.zdbjq.cn/Article/details/gpayhdokn.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.hesvh.cn/Article/details/gtxaznocm.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gmtontjlc.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.fehbvm.com/Article/details/ggecawruk.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gtvmevcoi.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gdjylzpil.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.hesvh.cn/Article/details/gizqjwtjd.sHtML

[Q33] 多列分组
来源：http://baike.fehbvm.com/Article/details/golrqfvdl.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://3g.fehbvm.com/Article/details/grlmdidxs.sHtML

[Q34] 每组取第一条
来源：http://wap.fehbvm.com/Article/details/goagpbytc.sHtML

SELECT * FROM (
来源：http://blog.hesvh.cn/Article/details/gmurdqjae.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.hesvh.cn/Article/details/gfflugfpm.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/ghfdribvx.sHtML

[Q35] 内连接
来源：http://mobile.fehbvm.com/Article/details/grepjwdzj.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://wap.zdbjq.cn/Article/details/gtsusysgi.sHtML

[Q36] 左连接
来源：http://www.blog.hesvh.cn/Article/details/gmfjrpgwd.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.zdbjq.cn/Article/details/gbivzzdxp.sHtML

[Q37] 右连接
来源：http://www.blog.hesvh.cn/Article/details/ghhcgzipj.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fehbvm.com/Article/details/gslsvvewk.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.hesvh.cn/Article/details/glekbhpjh.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.fehbvm.com/Article/details/ggtrzvavn.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.hesvh.cn/Article/details/gtawrixis.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.zdbjq.cn/Article/details/gpovthikx.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.fehbvm.com/Article/details/gzkzltgqp.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.hesvh.cn/Article/details/gdohutmus.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.hesvh.cn/Article/details/ggzwmssmp.sHtML

[Q41] 多表连接
来源：http://read.share.hesvh.cn/Article/details/gukwekwbb.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.zdbjq.cn/Article/details/gakhxiych.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.zdbjq.cn/Article/details/gxxdgnonx.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.fehbvm.com/Article/details/gklboajfv.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.fehbvm.com/Article/details/gkgkbowea.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.hesvh.cn/Article/details/gbsvrvhsl.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://baike.hesvh.cn/Article/details/geieutyhx.sHtML

[Q43] 标量子查询
来源：http://m.share.fehbvm.com/Article/details/guwkidsks.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://read.share.fehbvm.com/Article/details/gznbxxmxx.sHtML

[Q44] IN 子查询
来源：http://m.share.hesvh.cn/Article/details/ghfikhfhb.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.hesvh.cn/Article/details/gcsiewffz.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.fehbvm.com/Article/details/geinnupwd.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.hesvh.cn/Article/details/gububgvjp.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://3g.hesvh.cn/Article/details/gaouotcrj.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fehbvm.com/Article/details/gwsmatrbt.sHtML

[Q47] 与平均值比较
来源：http://read.share.fehbvm.com/Article/details/gqancmlrc.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.zdbjq.cn/Article/details/glgeqlili.sHtML

[Q48] CTE 公用表表达式
来源：http://read.share.zdbjq.cn/Article/details/gpypaoeaz.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.fehbvm.com/Article/details/gkrbwvctx.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.blog.hesvh.cn/Article/details/gxontioyu.sHtML

[Q49] 更新单行
来源：http://wap.zdbjq.cn/Article/details/gyxjustrf.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.zdbjq.cn/Article/details/gpeugqdwz.sHtML

[Q50] 批量更新
来源：http://read.share.hesvh.cn/Article/details/goztbtlwz.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://3g.fehbvm.com/Article/details/ghetjqztl.sHtML

[Q51] 用子查询更新
来源：http://blog.zdbjq.cn/Article/details/gfmrehygx.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.fehbvm.com/Article/details/gjpamjvyd.sHtML

[Q52] 删除指定行
来源：http://mobile.hesvh.cn/Article/details/ghnsugvmu.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.zdbjq.cn/Article/details/gkmrzwvye.sHtML

[Q53] 按条件删除
来源：http://3g.fehbvm.com/Article/details/gitisvdvg.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.hesvh.cn/Article/details/ghkvvmfot.sHtML

[Q54] 清空表
来源：http://www.share.hesvh.cn/Article/details/gwxmrtaxl.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.zdbjq.cn/Article/details/gwnqmuysw.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.fehbvm.com/Article/details/grosxilas.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.fehbvm.com/Article/details/galboqafx.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.zdbjq.cn/Article/details/gbbumrdpy.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.zdbjq.cn/Article/details/gicgvpcde.sHtML

[Q57] 行号
来源：http://blog.hesvh.cn/Article/details/gnbuilbdw.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.zdbjq.cn/Article/details/gyegerwid.sHtML

[Q58] 累计求和
来源：http://read.share.fehbvm.com/Article/details/gfjiwjcpb.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gjsefcnkd.sHtML

[Q59] 分组内累计
来源：http://mobile.hesvh.cn/Article/details/grfcsqumi.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gkrsfjoao.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.fehbvm.com/Article/details/grfaqlnzz.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.hesvh.cn/Article/details/gshlojpuk.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://baike.hesvh.cn/Article/details/gtndcvurl.sHtML

[Q61] 移动平均
来源：http://blog.hesvh.cn/Article/details/ggigwhtmv.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gcixsumhv.sHtML

[Q62] 分组占比
来源：http://3g.zdbjq.cn/Article/details/gepfaqrrg.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/gpnrrngft.sHtML

[Q63] 开启事务
来源：http://www.m.share.hesvh.cn/Article/details/gfxgxyhbe.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.zdbjq.cn/Article/details/guzvbjgho.sHtML

[Q64] 提交事务
来源：http://read.share.hesvh.cn/Article/details/gcunozrtq.sHtML

COMMIT;
来源：http://blog.hesvh.cn/Article/details/gfqmdlawr.sHtML

[Q65] 回滚事务
来源：http://mobile.zdbjq.cn/Article/details/ggmuikdzi.sHtML

ROLLBACK;
来源：http://baike.hesvh.cn/Article/details/gwhpjduag.sHtML

[Q66] 行锁查询
来源：http://mobile.hesvh.cn/Article/details/gmaczuwmi.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.fehbvm.com/Article/details/gnvxuumpt.sHtML

[Q67] 设置隔离级别
来源：http://wap.hesvh.cn/Article/details/grrbohllz.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.fehbvm.com/Article/details/gimgvcknj.sHtML

[Q68] 保存点
来源：http://read.share.hesvh.cn/Article/details/gvegxrfif.sHtML

SAVEPOINT sp1;
来源：http://www.blog.hesvh.cn/Article/details/gmlhrftgh.sHtML

ROLLBACK TO sp1;
来源：http://3g.zdbjq.cn/Article/details/gdbzxuoto.sHtML

[Q69] 查看执行计划
来源：http://baike.hesvh.cn/Article/details/gjzaholki.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.fehbvm.com/Article/details/giwyaavhs.sHtML

[Q70] 更新统计信息
来源：http://blog.hesvh.cn/Article/details/gklaiwwup.sHtML

ANALYZE TABLE users;
来源：http://www.share.hesvh.cn/Article/details/gmslxesvc.sHtML

[Q71] 查看建表语句
来源：http://mobile.fehbvm.com/Article/details/gkylpocxr.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.zdbjq.cn/Article/details/gnzgsiouy.sHtML

[Q72] 查看索引
来源：http://m.share.fehbvm.com/Article/details/gsvcwjoyj.sHtML

SHOW INDEX FROM users;
来源：http://wap.hesvh.cn/Article/details/gtdhuchwa.sHtML

[Q73] 查看表状态
来源：http://www.share.hesvh.cn/Article/details/gjvqstmmq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.fehbvm.com/Article/details/gbcwddiey.sHtML

[Q74] 强制使用索引
来源：http://3g.fehbvm.com/Article/details/gygdnzpun.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.hesvh.cn/Article/details/goohpbpyf.sHtML

[Q75] 日期格式化
来源：http://3g.fehbvm.com/Article/details/gbqkcwtwl.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gqjkkbevj.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.hesvh.cn/Article/details/gdzskygtm.sHtML

[Q76] 按天统计
来源：http://blog.hesvh.cn/Article/details/gdzuvqega.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.hesvh.cn/Article/details/gahykowdp.sHtML

[Q77] 时间加减
来源：http://3g.fehbvm.com/Article/details/gaztfihdv.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.fehbvm.com/Article/details/galccqbjo.sHtML

[Q78] 当前时间
来源：http://3g.fehbvm.com/Article/details/gwmcgdubg.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.zdbjq.cn/Article/details/gktqafqpv.sHtML

[Q79] 字符串拼接
来源：http://baike.fehbvm.com/Article/details/ghaslfbls.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.hesvh.cn/Article/details/ggucowdhm.sHtML

[Q80] 字符串截取
来源：http://wap.fehbvm.com/Article/details/gttcwyavv.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/grqtvtyji.sHtML

[Q81] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/gvlcbsulh.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.fehbvm.com/Article/details/gdyeihekk.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.hesvh.cn/Article/details/gcfhwcrqw.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/grtmkkpkm.sHtML

[Q83] 大小写转换
来源：http://blog.fehbvm.com/Article/details/gtrrryssy.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/ggtlsrnfu.sHtML

[Q84] 去除首尾空格
来源：http://m.share.fehbvm.com/Article/details/grjiiqslf.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.zdbjq.cn/Article/details/gquwvlwpq.sHtML

[Q85] 数值取整
来源：http://blog.zdbjq.cn/Article/details/gxgtuuqdl.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.fehbvm.com/Article/details/gsnkurudq.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fehbvm.com/Article/details/gcvmcjwfw.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://m.share.zdbjq.cn/Article/details/gzqgzmfxt.sHtML

[Q87] JSON 字段做条件
来源：http://www.share.hesvh.cn/Article/details/gcsbiuxrs.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.zdbjq.cn/Article/details/gdqapuuwp.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fehbvm.com/Article/details/grhgluomg.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.zdbjq.cn/Article/details/gnypakdmz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.fehbvm.com/Article/details/gwowbzygg.sHtML

[Q89] 判断表是否存在
来源：http://www.blog.hesvh.cn/Article/details/grjgvhvul.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fehbvm.com/Article/details/gslcbgwcy.sHtML

[Q90] 生成序号列
来源：http://www.blog.fehbvm.com/Article/details/gseafxhiw.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://mobile.zdbjq.cn/Article/details/gnwhxvyxx.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gwleiczxp.sHtML

R. Bash 专题
来源：http://m.share.hesvh.cn/Article/details/gqjocjaoc.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/geknvdhcc.sHtML

[R01] shebang 与严格模式
来源：http://wap.zdbjq.cn/Article/details/gcwgouwqr.sHtML

#!/usr/bin/env bash
来源：http://3g.zdbjq.cn/Article/details/gamlqjtlf.sHtML

set -euo pipefail
来源：http://blog.hesvh.cn/Article/details/gslmejwnh.sHtML

[R02] 变量赋值与使用
来源：http://mobile.zdbjq.cn/Article/details/gtftqjsps.sHtML

name="Tom"; echo "$name"
来源：http://read.share.zdbjq.cn/Article/details/gxcoiczkz.sHtML

[R03] 只读变量
来源：http://3g.fehbvm.com/Article/details/gcsccfuun.sHtML

readonly PI=3.14
来源：http://www.m.share.fehbvm.com/Article/details/gddutkelq.sHtML

[R04] 位置参数
来源：http://www.m.share.fehbvm.com/Article/details/gdbrlxfoc.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.hesvh.cn/Article/details/gshrnfxlx.sHtML

[R05] 参数默认值
来源：http://mobile.zdbjq.cn/Article/details/gxgmstirr.sHtML

name="${1:-default}"
来源：http://read.share.fehbvm.com/Article/details/gnmvmlzdl.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.hesvh.cn/Article/details/gsinxscaz.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.hesvh.cn/Article/details/gvelutkku.sHtML

[R07] if 判断文件
来源：http://www.blog.zdbjq.cn/Article/details/glqfoldkm.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gxnvqcjxb.sHtML

[R08] 数值比较
来源：http://read.share.zdbjq.cn/Article/details/gippogxgj.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.zdbjq.cn/Article/details/gxbwbcixt.sHtML

[R09] 字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/gvoskxard.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.zdbjq.cn/Article/details/giuxubdaj.sHtML

[R10] 正则匹配
来源：http://www.blog.zdbjq.cn/Article/details/gplwclezv.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.hesvh.cn/Article/details/guvfzyrtd.sHtML

[R11] case 多分支
来源：http://www.blog.hesvh.cn/Article/details/gsdxsdoxe.sHtML

case "$1" in
来源：http://www.share.fehbvm.com/Article/details/ghinqkynd.sHtML

start) echo "启动" ;;
来源：http://www.blog.hesvh.cn/Article/details/gvdjauoyf.sHtML

stop)  echo "停止" ;;
来源：http://m.share.zdbjq.cn/Article/details/guaerbops.sHtML

*)     echo "未知命令" ;;
来源：http://wap.hesvh.cn/Article/details/gixqytywq.sHtML

esac
来源：http://blog.fehbvm.com/Article/details/gqcrlekll.sHtML

[R12] for 遍历文件
来源：http://www.share.fehbvm.com/Article/details/gnvgztrjz.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fehbvm.com/Article/details/gqcwndham.sHtML

[R13] for 计数循环
来源：http://www.blog.hesvh.cn/Article/details/gpteszoae.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.fehbvm.com/Article/details/gsbtgddtd.sHtML

[R14] C 风格 for
来源：http://baike.fehbvm.com/Article/details/gcjcgeuvc.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.zdbjq.cn/Article/details/gacippvdo.sHtML

[R15] while 逐行读文件
来源：http://m.share.hesvh.cn/Article/details/gdfutmpja.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.zdbjq.cn/Article/details/gxkqplhxz.sHtML

[R16] until 等待条件
来源：http://wap.zdbjq.cn/Article/details/gxftidaxq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fehbvm.com/Article/details/gdqpezygl.sHtML

[R17] 数组定义与取值
来源：http://blog.zdbjq.cn/Article/details/gxdnzedmp.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.hesvh.cn/Article/details/gdvldbgmm.sHtML

[R18] 遍历数组
来源：http://baike.hesvh.cn/Article/details/guuqglcuq.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.zdbjq.cn/Article/details/gvfdhgixx.sHtML

[R19] 数组长度
来源：http://baike.zdbjq.cn/Article/details/gmxarbtih.sHtML

echo "${#arr[@]}"
来源：http://3g.hesvh.cn/Article/details/gxavspqsj.sHtML

[R20] 关联数组（字典）
来源：http://read.share.fehbvm.com/Article/details/gwqntcxoy.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fehbvm.com/Article/details/gqltlgggu.sHtML

[R21] 字符串长度
来源：http://www.share.fehbvm.com/Article/details/gqnpjsrij.sHtML

echo "${#s}"
来源：http://read.share.zdbjq.cn/Article/details/gkgkjlznm.sHtML

[R22] 截取子串
来源：http://read.share.fehbvm.com/Article/details/gwlenfvbo.sHtML

echo "${s:0:5}"
来源：http://baike.zdbjq.cn/Article/details/gnotykrth.sHtML

[R23] 字符串替换
来源：http://blog.fehbvm.com/Article/details/gdydtmhtp.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fehbvm.com/Article/details/gcpvujxwv.sHtML

[R24] 大小写转换
来源：http://wap.zdbjq.cn/Article/details/gcsqfknaf.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.fehbvm.com/Article/details/gremlzgua.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.zdbjq.cn/Article/details/gizypqmnz.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fehbvm.com/Article/details/gfoebjwlr.sHtML

[R26] 命令替换
来源：http://baike.zdbjq.cn/Article/details/gkludwuey.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.zdbjq.cn/Article/details/gtkwvqhqs.sHtML

[R27] 算术展开
来源：http://www.m.share.hesvh.cn/Article/details/gejphoozi.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fehbvm.com/Article/details/gpnsstfyk.sHtML

[R28] 浮点运算
来源：http://www.share.hesvh.cn/Article/details/gbddatjas.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fehbvm.com/Article/details/grgeayeel.sHtML

[R29] 定义函数
来源：http://read.share.zdbjq.cn/Article/details/gemwntqtw.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.hesvh.cn/Article/details/garrfwstt.sHtML

[R30] 函数返回状态码
来源：http://mobile.zdbjq.cn/Article/details/gdctnhzby.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fehbvm.com/Article/details/goowhrgon.sHtML

[R31] 局部变量
来源：http://baike.fehbvm.com/Article/details/gvmehgzmt.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.zdbjq.cn/Article/details/gcvsrplkj.sHtML

[R32] 参数个数校验
来源：http://mobile.hesvh.cn/Article/details/golubtzdq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.hesvh.cn/Article/details/ghordygxe.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.fehbvm.com/Article/details/gfoesflnr.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.hesvh.cn/Article/details/gjpmyjghy.sHtML

[R34] 退出时清理
来源：http://www.blog.zdbjq.cn/Article/details/gylyuxpmb.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gokorkbsr.sHtML

[R35] 后台执行并等待
来源：http://blog.fehbvm.com/Article/details/gckoyanqj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.zdbjq.cn/Article/details/gbbszfwtn.sHtML

[R36] 并发执行多个任务
来源：http://3g.zdbjq.cn/Article/details/gibeixfcp.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.hesvh.cn/Article/details/gnqutehxw.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fehbvm.com/Article/details/gxnbotwca.sHtML

files=$(ls -1)
来源：http://baike.hesvh.cn/Article/details/gkxphevog.sHtML

[R38] 管道串联
来源：http://blog.zdbjq.cn/Article/details/gtdwsntja.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fehbvm.com/Article/details/gdcvdprll.sHtML

[R39] 重定向标准输出与错误
来源：http://www.blog.zdbjq.cn/Article/details/gafhchcye.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.zdbjq.cn/Article/details/gefbehwvt.sHtML

[R40] 追加写日志
来源：http://m.share.fehbvm.com/Article/details/gyiurjiiu.sHtML

echo "log" >> out.log
来源：http://wap.fehbvm.com/Article/details/glgymqqnb.sHtML

[R41] 丢弃输出
来源：http://3g.zdbjq.cn/Article/details/gdgbijusy.sHtML

cmd >/dev/null 2>&1
来源：http://blog.hesvh.cn/Article/details/gxenrlwhv.sHtML

[R42] 输入重定向
来源：http://www.share.zdbjq.cn/Article/details/gzqjdhwgw.sHtML

wc -l < a.txt
来源：http://www.blog.hesvh.cn/Article/details/gmcctenyo.sHtML

[R43] 按名字查找文件
来源：http://www.share.hesvh.cn/Article/details/gafiiuecl.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.zdbjq.cn/Article/details/gziyvexyh.sHtML

[R44] 按修改时间查找
来源：http://read.share.fehbvm.com/Article/details/gfmjjohdt.sHtML

find . -mtime -7 -type f
来源：http://wap.fehbvm.com/Article/details/ggucffeql.sHtML

[R45] 批量删除
来源：http://www.m.share.fehbvm.com/Article/details/gqiojmlre.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.hesvh.cn/Article/details/gkaqzanev.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fehbvm.com/Article/details/gurhjtsqo.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.hesvh.cn/Article/details/gjenrwmnk.sHtML

[R47] sed 单行替换
来源：http://www.blog.hesvh.cn/Article/details/gvltbqdlc.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.fehbvm.com/Article/details/guurtjunl.sHtML

[R48] awk 取指定列
来源：http://mobile.hesvh.cn/Article/details/gkvkisfqy.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.hesvh.cn/Article/details/ggbebpbdp.sHtML

[R49] awk 带条件
来源：http://www.blog.fehbvm.com/Article/details/gghtomess.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fehbvm.com/Article/details/gppeakxgb.sHtML

[R50] awk 求和
来源：http://www.share.zdbjq.cn/Article/details/grqydjrdw.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gwfceycxe.sHtML

[R51] 排序去重取前几
来源：http://baike.hesvh.cn/Article/details/gdbjzqvlu.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.zdbjq.cn/Article/details/gjarsgymv.sHtML

[R52] 统计行数
来源：http://baike.fehbvm.com/Article/details/gttakcdyx.sHtML

wc -l a.txt
来源：http://read.share.hesvh.cn/Article/details/gtlbmdqow.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fehbvm.com/Article/details/gycjwyppr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.hesvh.cn/Article/details/gvxsthjqz.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fehbvm.com/Article/details/geslfrqud.sHtML

diff a.txt b.txt
来源：http://wap.fehbvm.com/Article/details/gootmvikn.sHtML

[R55] 压缩与解压
来源：http://www.share.fehbvm.com/Article/details/ggbiotkvw.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.zdbjq.cn/Article/details/ggdgankfe.sHtML

[R56] 远程拷贝
来源：http://mobile.hesvh.cn/Article/details/gnqterzlr.sHtML

scp file user@host:/path/
来源：http://www.blog.hesvh.cn/Article/details/geurdvymo.sHtML

[R57] 远程执行命令
来源：http://www.m.share.zdbjq.cn/Article/details/gpiybivfc.sHtML

ssh user@host 'uptime'
来源：http://wap.hesvh.cn/Article/details/ggnwcvtnk.sHtML

[R58] 下载文件
来源：http://www.blog.zdbjq.cn/Article/details/gtfcdiequ.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.hesvh.cn/Article/details/gekkneran.sHtML

[R59] 发 POST JSON
来源：http://m.share.hesvh.cn/Article/details/giaxxhiau.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://mobile.fehbvm.com/Article/details/giejtdnmm.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fehbvm.com/Article/details/ghangdgjx.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.hesvh.cn/Article/details/gzlogcsot.sHtML

[R61] 磁盘占用
来源：http://baike.zdbjq.cn/Article/details/gtewdlkqq.sHtML

df -h;  du -sh *
来源：http://www.share.fehbvm.com/Article/details/glrzvjdhm.sHtML

[R62] 找最占空间的文件
来源：http://wap.hesvh.cn/Article/details/gcokgtode.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.zdbjq.cn/Article/details/gjvwlalgt.sHtML

[R63] 内存与进程
来源：http://3g.zdbjq.cn/Article/details/garxxhhff.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.zdbjq.cn/Article/details/gcutyttno.sHtML

[R64] 结束进程
来源：http://wap.hesvh.cn/Article/details/gzmzwcpij.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.zdbjq.cn/Article/details/gzaxiyqpf.sHtML

[R65] 查看端口占用
来源：http://blog.hesvh.cn/Article/details/gqngvxkxh.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.zdbjq.cn/Article/details/gldpbqeta.sHtML

[R66] 定时任务
来源：http://www.share.fehbvm.com/Article/details/glzihfvuz.sHtML

crontab -e;  crontab -l
来源：http://read.share.zdbjq.cn/Article/details/gdonfadqw.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.zdbjq.cn/Article/details/grqufccwz.sHtML

openssl rand -hex 16
来源：http://m.share.fehbvm.com/Article/details/gttqappwb.sHtML

[R68] 计算文件校验值
来源：http://www.share.zdbjq.cn/Article/details/gsmmsvgdw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.zdbjq.cn/Article/details/gohpruroz.sHtML

[R69] 生成随机密码
来源：http://mobile.zdbjq.cn/Article/details/gbmgjyeeg.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.hesvh.cn/Article/details/gptxkzwaw.sHtML

[R70] 时间戳与互转
来源：http://m.share.hesvh.cn/Article/details/gyoswkchg.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fehbvm.com/Article/details/gbqenjwjb.sHtML

[R71] 日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/gsuzolxbh.sHtML


<!-- 参考信息 -->