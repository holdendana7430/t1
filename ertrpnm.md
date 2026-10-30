代发 wailian999

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.zdbjq.cn/Article/details/gqxwsnutx.sHtML

[Q26] 计数
来源：http://baike.zdbjq.cn/Article/details/gwcyzkwag.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/giafdoxka.sHtML

[Q27] 条件计数
来源：http://3g.fehbvm.com/Article/details/gtnpknhwe.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gebnittnd.sHtML

[Q28] 求和与平均
来源：http://baike.fehbvm.com/Article/details/gzspxvnda.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gpyttwwgq.sHtML

[Q29] 最大最小值
来源：http://baike.zdbjq.cn/Article/details/grmqzgpfg.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.hesvh.cn/Article/details/gbwnonrdd.sHtML

[Q30] 分组统计
来源：http://m.share.zdbjq.cn/Article/details/ggfxgytde.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/glupquukr.sHtML

[Q31] 分组后过滤
来源：http://baike.fehbvm.com/Article/details/gxcttsvhk.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.m.share.fehbvm.com/Article/details/ghahodlcx.sHtML

[Q32] 分组拼接字符串
来源：http://3g.hesvh.cn/Article/details/glmpgahqm.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gywdebgso.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://wap.zdbjq.cn/Article/details/gqticwxkl.sHtML

[Q33] 多列分组
来源：http://www.m.share.zdbjq.cn/Article/details/gaqdykncd.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.m.share.zdbjq.cn/Article/details/gnbcqvnmd.sHtML

[Q34] 每组取第一条
来源：http://read.share.hesvh.cn/Article/details/gyqmsnsys.sHtML

SELECT * FROM (
来源：http://wap.fehbvm.com/Article/details/ghxydbwgt.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.zdbjq.cn/Article/details/gesikzgnk.sHtML

) t WHERE rn = 1;
来源：http://blog.hesvh.cn/Article/details/gqnjfvstv.sHtML

[Q35] 内连接
来源：http://www.m.share.fehbvm.com/Article/details/gosontzxn.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.zdbjq.cn/Article/details/gcjujkzhx.sHtML

[Q36] 左连接
来源：http://m.share.hesvh.cn/Article/details/geffoydkh.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.hesvh.cn/Article/details/gebiuusdq.sHtML

[Q37] 右连接
来源：http://www.share.zdbjq.cn/Article/details/gzvwnliob.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.zdbjq.cn/Article/details/grjmabdsa.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.hesvh.cn/Article/details/ghohbgrqv.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.blog.zdbjq.cn/Article/details/gvgkglcbz.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.fehbvm.com/Article/details/gaylljrkh.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.fehbvm.com/Article/details/gwsrnyyuz.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.hesvh.cn/Article/details/grbfmoxmd.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.hesvh.cn/Article/details/gjiaeacdi.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://m.share.zdbjq.cn/Article/details/gwjbuexcp.sHtML

[Q41] 多表连接
来源：http://www.blog.zdbjq.cn/Article/details/gidqjvtas.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.fehbvm.com/Article/details/gituvdsyy.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.zdbjq.cn/Article/details/gkoxjwprw.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.hesvh.cn/Article/details/gkcizqtio.sHtML

[Q42] 连接条件附加过滤
来源：http://blog.hesvh.cn/Article/details/gqzjelqjg.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.fehbvm.com/Article/details/gdptbgigz.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://read.share.hesvh.cn/Article/details/gqenkvlio.sHtML

[Q43] 标量子查询
来源：http://wap.fehbvm.com/Article/details/gszowzkpy.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.hesvh.cn/Article/details/gzbxkcovp.sHtML

[Q44] IN 子查询
来源：http://wap.fehbvm.com/Article/details/gybuylepx.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.hesvh.cn/Article/details/gphblvjyv.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.fehbvm.com/Article/details/guxqpmsxm.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.hesvh.cn/Article/details/gakotxfqr.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.zdbjq.cn/Article/details/glidcwwjq.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.hesvh.cn/Article/details/gvfjhpkjx.sHtML

[Q47] 与平均值比较
来源：http://www.blog.zdbjq.cn/Article/details/gvepzroen.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.fehbvm.com/Article/details/gjpezunkl.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.zdbjq.cn/Article/details/gtvcphmoh.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.fehbvm.com/Article/details/gtwdfdshs.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.zdbjq.cn/Article/details/grdjinbxx.sHtML

[Q49] 更新单行
来源：http://3g.fehbvm.com/Article/details/gombgqxpn.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.zdbjq.cn/Article/details/gwzxwlodu.sHtML

[Q50] 批量更新
来源：http://baike.fehbvm.com/Article/details/gzdygtmfx.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.zdbjq.cn/Article/details/gefyskgow.sHtML

[Q51] 用子查询更新
来源：http://baike.fehbvm.com/Article/details/gxosmpomn.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.fehbvm.com/Article/details/gmrmcfhqj.sHtML

[Q52] 删除指定行
来源：http://3g.fehbvm.com/Article/details/gqxapwdzx.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.fehbvm.com/Article/details/ggsmrvkgp.sHtML

[Q53] 按条件删除
来源：http://wap.fehbvm.com/Article/details/gczzddzur.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.hesvh.cn/Article/details/gknajevxn.sHtML

[Q54] 清空表
来源：http://3g.zdbjq.cn/Article/details/gtawrzcvw.sHtML

TRUNCATE TABLE logs;
来源：http://m.share.fehbvm.com/Article/details/gksignnni.sHtML

[Q55] 排名（并列占位）
来源：http://www.share.zdbjq.cn/Article/details/gnlzyshsv.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.blog.fehbvm.com/Article/details/gpuvtpwqb.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.hesvh.cn/Article/details/gejwhxdck.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.zdbjq.cn/Article/details/glevubodr.sHtML

[Q57] 行号
来源：http://mobile.zdbjq.cn/Article/details/ghxlhyzwj.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.fehbvm.com/Article/details/ggswaeswz.sHtML

[Q58] 累计求和
来源：http://3g.hesvh.cn/Article/details/ggnjppkcs.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.fehbvm.com/Article/details/gxqdyddoe.sHtML

[Q59] 分组内累计
来源：http://blog.fehbvm.com/Article/details/gjmwjcqjl.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gpxwufxen.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.zdbjq.cn/Article/details/glthgatkm.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.fehbvm.com/Article/details/gutujehdo.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gjmghtepp.sHtML

[Q61] 移动平均
来源：http://mobile.hesvh.cn/Article/details/gyrbbrhup.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gqndqmjba.sHtML

[Q62] 分组占比
来源：http://3g.fehbvm.com/Article/details/gzdxmguwx.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.zdbjq.cn/Article/details/ggfxxqhgh.sHtML

[Q63] 开启事务
来源：http://baike.hesvh.cn/Article/details/gkmrwdwio.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.zdbjq.cn/Article/details/gsxokucto.sHtML

[Q64] 提交事务
来源：http://read.share.zdbjq.cn/Article/details/gpsvxoqag.sHtML

COMMIT;
来源：http://www.share.hesvh.cn/Article/details/gqzrvehpo.sHtML

[Q65] 回滚事务
来源：http://www.share.zdbjq.cn/Article/details/gkxdektno.sHtML

ROLLBACK;
来源：http://www.share.zdbjq.cn/Article/details/goidmiexa.sHtML

[Q66] 行锁查询
来源：http://www.blog.fehbvm.com/Article/details/grhaotacz.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://wap.zdbjq.cn/Article/details/gljxgtnfc.sHtML

[Q67] 设置隔离级别
来源：http://read.share.zdbjq.cn/Article/details/glfcluawz.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.hesvh.cn/Article/details/grarkmgno.sHtML

[Q68] 保存点
来源：http://mobile.hesvh.cn/Article/details/grnnabivj.sHtML

SAVEPOINT sp1;
来源：http://3g.hesvh.cn/Article/details/ghyffxase.sHtML

ROLLBACK TO sp1;
来源：http://baike.zdbjq.cn/Article/details/gbokmxbrj.sHtML

[Q69] 查看执行计划
来源：http://www.blog.hesvh.cn/Article/details/gnggimqmf.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://read.share.hesvh.cn/Article/details/glzwmneka.sHtML

[Q70] 更新统计信息
来源：http://blog.zdbjq.cn/Article/details/getrhksgx.sHtML

ANALYZE TABLE users;
来源：http://mobile.zdbjq.cn/Article/details/gyvsjpodl.sHtML

[Q71] 查看建表语句
来源：http://blog.hesvh.cn/Article/details/gpfupmrsh.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.zdbjq.cn/Article/details/glslxmakt.sHtML

[Q72] 查看索引
来源：http://blog.zdbjq.cn/Article/details/gtqlrdupg.sHtML

SHOW INDEX FROM users;
来源：http://wap.hesvh.cn/Article/details/gpovgpsjh.sHtML

[Q73] 查看表状态
来源：http://mobile.zdbjq.cn/Article/details/gtdpiqcto.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.hesvh.cn/Article/details/gdahlwxzb.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.hesvh.cn/Article/details/gowcpgfkz.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.hesvh.cn/Article/details/gebxcuhkl.sHtML

[Q75] 日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/geeckuwde.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.zdbjq.cn/Article/details/gcbxikgqi.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://baike.hesvh.cn/Article/details/geiflzzdh.sHtML

[Q76] 按天统计
来源：http://wap.zdbjq.cn/Article/details/ghygosxqo.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fehbvm.com/Article/details/glcrdsuzz.sHtML

[Q77] 时间加减
来源：http://wap.zdbjq.cn/Article/details/gjnazbqem.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://m.share.zdbjq.cn/Article/details/gwgtbckzh.sHtML

[Q78] 当前时间
来源：http://mobile.fehbvm.com/Article/details/gqrxjifja.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.fehbvm.com/Article/details/gnypkmjer.sHtML

[Q79] 字符串拼接
来源：http://3g.fehbvm.com/Article/details/gjmsgttcu.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://mobile.hesvh.cn/Article/details/gltntkbtf.sHtML

[Q80] 字符串截取
来源：http://www.blog.hesvh.cn/Article/details/gnfxgagwg.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gobzypyfq.sHtML

[Q81] 字符串替换
来源：http://www.blog.hesvh.cn/Article/details/griicacpn.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.hesvh.cn/Article/details/gkqufqdcw.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.zdbjq.cn/Article/details/gnjnmjzqg.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gcxitwzyz.sHtML

[Q83] 大小写转换
来源：http://www.m.share.fehbvm.com/Article/details/gtrtxsbwr.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/geynfkzfx.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.hesvh.cn/Article/details/gpkmnbnhc.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gsatsjvpf.sHtML

[Q85] 数值取整
来源：http://www.share.hesvh.cn/Article/details/gelhfcszk.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://wap.zdbjq.cn/Article/details/ggbxclzmv.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.zdbjq.cn/Article/details/gscioptdb.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.hesvh.cn/Article/details/goffrxqno.sHtML

[Q87] JSON 字段做条件
来源：http://mobile.hesvh.cn/Article/details/gjlrodjho.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.zdbjq.cn/Article/details/gcjlunocs.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.zdbjq.cn/Article/details/glarujvmm.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.fehbvm.com/Article/details/gckrxmsiv.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://read.share.fehbvm.com/Article/details/gnnnrkcib.sHtML

[Q89] 判断表是否存在
来源：http://read.share.fehbvm.com/Article/details/gctyozebi.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.hesvh.cn/Article/details/gaiwubqjx.sHtML

[Q90] 生成序号列
来源：http://www.share.zdbjq.cn/Article/details/gziqaasfr.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fehbvm.com/Article/details/gpktuppfb.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gasgxuhvb.sHtML

R. Bash 专题
来源：http://www.m.share.fehbvm.com/Article/details/gqaoisvgs.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gqojsghly.sHtML

[R01] shebang 与严格模式
来源：http://baike.hesvh.cn/Article/details/gmxwvskeq.sHtML

#!/usr/bin/env bash
来源：http://www.share.zdbjq.cn/Article/details/gekoelgbp.sHtML

set -euo pipefail
来源：http://baike.hesvh.cn/Article/details/glkvqytjc.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.fehbvm.com/Article/details/gqtzqanon.sHtML

name="Tom"; echo "$name"
来源：http://www.share.hesvh.cn/Article/details/gwjzdurjz.sHtML

[R03] 只读变量
来源：http://blog.hesvh.cn/Article/details/gmpnnklnv.sHtML

readonly PI=3.14
来源：http://read.share.fehbvm.com/Article/details/gqalqzffg.sHtML

[R04] 位置参数
来源：http://www.blog.fehbvm.com/Article/details/gzgtnkdfp.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.fehbvm.com/Article/details/gebtnmwjr.sHtML

[R05] 参数默认值
来源：http://read.share.hesvh.cn/Article/details/gtqyvmagi.sHtML

name="${1:-default}"
来源：http://blog.zdbjq.cn/Article/details/gejxxifas.sHtML

[R06] 判断命令是否存在
来源：http://baike.zdbjq.cn/Article/details/gdzcxsxcu.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.fehbvm.com/Article/details/gjtihtybw.sHtML

[R07] if 判断文件
来源：http://wap.hesvh.cn/Article/details/gulttylqq.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fehbvm.com/Article/details/ggyzhgulh.sHtML

[R08] 数值比较
来源：http://3g.hesvh.cn/Article/details/grpgvwgqw.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.hesvh.cn/Article/details/gykuhzupg.sHtML

[R09] 字符串比较
来源：http://www.share.zdbjq.cn/Article/details/geozjkjip.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.hesvh.cn/Article/details/gribmzbee.sHtML

[R10] 正则匹配
来源：http://www.share.zdbjq.cn/Article/details/gokbsrffa.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.zdbjq.cn/Article/details/gwvtxderu.sHtML

[R11] case 多分支
来源：http://blog.hesvh.cn/Article/details/gjyfoihgi.sHtML

case "$1" in
来源：http://www.share.fehbvm.com/Article/details/gnpvclbsz.sHtML

start) echo "启动" ;;
来源：http://mobile.hesvh.cn/Article/details/gmouticiu.sHtML

stop)  echo "停止" ;;
来源：http://read.share.hesvh.cn/Article/details/gnyqjtpvz.sHtML

*)     echo "未知命令" ;;
来源：http://baike.hesvh.cn/Article/details/gylmgphtm.sHtML

esac
来源：http://www.blog.fehbvm.com/Article/details/ghpnluttr.sHtML

[R12] for 遍历文件
来源：http://blog.hesvh.cn/Article/details/gwfvdlnxe.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.hesvh.cn/Article/details/gkpbjhlkd.sHtML

[R13] for 计数循环
来源：http://mobile.zdbjq.cn/Article/details/gvlyzhwsd.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.zdbjq.cn/Article/details/gzzxvnojg.sHtML

[R14] C 风格 for
来源：http://www.share.fehbvm.com/Article/details/girippfmp.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.hesvh.cn/Article/details/gddejpkfb.sHtML

[R15] while 逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gaojmehym.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.zdbjq.cn/Article/details/glaswenbd.sHtML

[R16] until 等待条件
来源：http://www.blog.hesvh.cn/Article/details/gdttfzwjd.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.hesvh.cn/Article/details/gsmsknjvn.sHtML

[R17] 数组定义与取值
来源：http://mobile.fehbvm.com/Article/details/gqbdgdawl.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fehbvm.com/Article/details/gosrwwuzz.sHtML

[R18] 遍历数组
来源：http://wap.fehbvm.com/Article/details/ghiuknmxg.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.hesvh.cn/Article/details/gbpytkssa.sHtML

[R19] 数组长度
来源：http://read.share.fehbvm.com/Article/details/gxmqqkwwb.sHtML

echo "${#arr[@]}"
来源：http://m.share.zdbjq.cn/Article/details/gbaszcfng.sHtML

[R20] 关联数组（字典）
来源：http://blog.zdbjq.cn/Article/details/gsebtlqsr.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://3g.hesvh.cn/Article/details/gdcdbyiwi.sHtML

[R21] 字符串长度
来源：http://m.share.zdbjq.cn/Article/details/gyuipzzss.sHtML

echo "${#s}"
来源：http://3g.hesvh.cn/Article/details/geachoxqv.sHtML

[R22] 截取子串
来源：http://mobile.fehbvm.com/Article/details/gqdmguajq.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fehbvm.com/Article/details/gmousveci.sHtML

[R23] 字符串替换
来源：http://blog.fehbvm.com/Article/details/gcbepyznc.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fehbvm.com/Article/details/grbrgdnup.sHtML

[R24] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/gsoqwfmrn.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.zdbjq.cn/Article/details/guvzquyvd.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.hesvh.cn/Article/details/gpinoxgpt.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.hesvh.cn/Article/details/glhqavyes.sHtML

[R26] 命令替换
来源：http://www.blog.hesvh.cn/Article/details/gxffumvvt.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.zdbjq.cn/Article/details/grcdqqvmw.sHtML

[R27] 算术展开
来源：http://blog.hesvh.cn/Article/details/gjdhbbypq.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.hesvh.cn/Article/details/guuczitlz.sHtML

[R28] 浮点运算
来源：http://read.share.zdbjq.cn/Article/details/ghftqkewx.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.hesvh.cn/Article/details/gblrejqdm.sHtML

[R29] 定义函数
来源：http://www.share.hesvh.cn/Article/details/gkzncdmij.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.hesvh.cn/Article/details/gnhbzhrdf.sHtML

[R30] 函数返回状态码
来源：http://blog.hesvh.cn/Article/details/gzpswiadx.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fehbvm.com/Article/details/gfwulxgfm.sHtML

[R31] 局部变量
来源：http://m.share.hesvh.cn/Article/details/gwjczbltk.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.zdbjq.cn/Article/details/gvtlewliv.sHtML

[R32] 参数个数校验
来源：http://read.share.zdbjq.cn/Article/details/gbrlgwqhe.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fehbvm.com/Article/details/gwiabqxao.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fehbvm.com/Article/details/gkjufczhf.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fehbvm.com/Article/details/gbfraoyre.sHtML

[R34] 退出时清理
来源：http://www.share.hesvh.cn/Article/details/gqejbnppq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gbqxejqie.sHtML

[R35] 后台执行并等待
来源：http://blog.hesvh.cn/Article/details/gqmeyozlm.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.zdbjq.cn/Article/details/ghegepmah.sHtML

[R36] 并发执行多个任务
来源：http://www.share.hesvh.cn/Article/details/gtdnuewox.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.zdbjq.cn/Article/details/gtybabqbt.sHtML

[R37] 把输出赋给变量
来源：http://mobile.zdbjq.cn/Article/details/gyjnmoqgd.sHtML

files=$(ls -1)
来源：http://baike.hesvh.cn/Article/details/guzqpkqnt.sHtML

[R38] 管道串联
来源：http://m.share.hesvh.cn/Article/details/ginzfpwrq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.zdbjq.cn/Article/details/gkznybujk.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fehbvm.com/Article/details/gfvfwrzhn.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fehbvm.com/Article/details/gdggjzytb.sHtML

[R40] 追加写日志
来源：http://www.blog.hesvh.cn/Article/details/gdgtqprwl.sHtML

echo "log" >> out.log
来源：http://wap.fehbvm.com/Article/details/gpwfusnad.sHtML

[R41] 丢弃输出
来源：http://m.share.zdbjq.cn/Article/details/gadlfzkqp.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fehbvm.com/Article/details/gnidxukdv.sHtML

[R42] 输入重定向
来源：http://www.m.share.hesvh.cn/Article/details/gsuizibbt.sHtML

wc -l < a.txt
来源：http://www.share.hesvh.cn/Article/details/gswrpojcu.sHtML

[R43] 按名字查找文件
来源：http://read.share.hesvh.cn/Article/details/ghukrbwjn.sHtML

find . -name "*.log" -type f
来源：http://blog.fehbvm.com/Article/details/gmtmgyxtl.sHtML

[R44] 按修改时间查找
来源：http://wap.hesvh.cn/Article/details/gdrqztzal.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fehbvm.com/Article/details/gohcuexxl.sHtML

[R45] 批量删除
来源：http://www.m.share.hesvh.cn/Article/details/gqnctsbxk.sHtML

find . -name "*.tmp" -delete
来源：http://baike.zdbjq.cn/Article/details/gubtztjdu.sHtML

[R46] 递归替换文件内容
来源：http://baike.zdbjq.cn/Article/details/gsfhhigtl.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.hesvh.cn/Article/details/gwutizxik.sHtML

[R47] sed 单行替换
来源：http://baike.fehbvm.com/Article/details/gemazlghq.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.hesvh.cn/Article/details/gniruvcbj.sHtML

[R48] awk 取指定列
来源：http://www.m.share.zdbjq.cn/Article/details/gjryjliup.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.zdbjq.cn/Article/details/givvllhug.sHtML

[R49] awk 带条件
来源：http://baike.hesvh.cn/Article/details/gjecqpgzr.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fehbvm.com/Article/details/gwczjhhqb.sHtML

[R50] awk 求和
来源：http://baike.hesvh.cn/Article/details/gsrzkjjee.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.hesvh.cn/Article/details/gxtiwfwac.sHtML

[R51] 排序去重取前几
来源：http://blog.fehbvm.com/Article/details/gzxxwytlr.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.m.share.zdbjq.cn/Article/details/gdfiuhnru.sHtML

[R52] 统计行数
来源：http://mobile.fehbvm.com/Article/details/grzhiptnn.sHtML

wc -l a.txt
来源：http://mobile.zdbjq.cn/Article/details/gazoeeeii.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.hesvh.cn/Article/details/gadowqdxb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.zdbjq.cn/Article/details/gtqtliarb.sHtML

[R54] 比较两个文件
来源：http://3g.zdbjq.cn/Article/details/gjhgtdxqx.sHtML

diff a.txt b.txt
来源：http://3g.hesvh.cn/Article/details/gwmrechdd.sHtML

[R55] 压缩与解压
来源：http://www.blog.zdbjq.cn/Article/details/ggqcpqezl.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.hesvh.cn/Article/details/ghkluzdxp.sHtML

[R56] 远程拷贝
来源：http://blog.zdbjq.cn/Article/details/glioenoyd.sHtML

scp file user@host:/path/
来源：http://3g.fehbvm.com/Article/details/geptressr.sHtML

[R57] 远程执行命令
来源：http://www.share.zdbjq.cn/Article/details/gvtqxfxtb.sHtML

ssh user@host 'uptime'
来源：http://www.share.hesvh.cn/Article/details/guruyhfjl.sHtML

[R58] 下载文件
来源：http://www.share.fehbvm.com/Article/details/gimjqvoxn.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fehbvm.com/Article/details/gzojalmqu.sHtML

[R59] 发 POST JSON
来源：http://blog.hesvh.cn/Article/details/gddzmiabr.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.zdbjq.cn/Article/details/ghiqxsnmt.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.hesvh.cn/Article/details/gzpnaefws.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fehbvm.com/Article/details/gabbndgkl.sHtML

[R61] 磁盘占用
来源：http://mobile.fehbvm.com/Article/details/gmtaggsyd.sHtML

df -h;  du -sh *
来源：http://www.m.share.fehbvm.com/Article/details/guphwddip.sHtML

[R62] 找最占空间的文件
来源：http://blog.fehbvm.com/Article/details/gldfkijon.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.hesvh.cn/Article/details/golhamgfl.sHtML

[R63] 内存与进程
来源：http://read.share.fehbvm.com/Article/details/gpynwgitj.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.zdbjq.cn/Article/details/gyfvqqxpo.sHtML

[R64] 结束进程
来源：http://mobile.fehbvm.com/Article/details/gyxmmcpgu.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fehbvm.com/Article/details/gzxcdpvvs.sHtML

[R65] 查看端口占用
来源：http://wap.zdbjq.cn/Article/details/ggcaizcnx.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.fehbvm.com/Article/details/ggevuffrn.sHtML

[R66] 定时任务
来源：http://m.share.zdbjq.cn/Article/details/gotwcqbgt.sHtML

crontab -e;  crontab -l
来源：http://www.blog.hesvh.cn/Article/details/gbutqwkpl.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.zdbjq.cn/Article/details/gcblxlgle.sHtML

openssl rand -hex 16
来源：http://baike.zdbjq.cn/Article/details/gjpnlvvxn.sHtML

[R68] 计算文件校验值
来源：http://mobile.fehbvm.com/Article/details/gbytzwfio.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.zdbjq.cn/Article/details/gmepbukhi.sHtML

[R69] 生成随机密码
来源：http://3g.fehbvm.com/Article/details/gevslehxn.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.hesvh.cn/Article/details/glliokixl.sHtML

[R70] 时间戳与互转
来源：http://3g.hesvh.cn/Article/details/gjgnasnqx.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.zdbjq.cn/Article/details/ghfzihkcp.sHtML

[R71] 日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/gflpiubak.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.hesvh.cn/Article/details/gjkpwkyun.sHtML

[R72] 等待端口就绪
来源：http://blog.hesvh.cn/Article/details/gghbobfpi.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.hesvh.cn/Article/details/gzlvzmnbi.sHtML

[R73] 分割大日志
来源：http://read.share.fehbvm.com/Article/details/gghaxsbmj.sHtML

split -l 1000 big.log part_
来源：http://3g.fehbvm.com/Article/details/gbxygdvcq.sHtML

[R74] 批量重命名
来源：http://www.m.share.fehbvm.com/Article/details/goscgvgrf.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fehbvm.com/Article/details/gyzwmvrsz.sHtML

[R75] 导出环境变量
来源：http://blog.hesvh.cn/Article/details/guqoekffk.sHtML


<!-- 参考信息 -->