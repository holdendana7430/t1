代发 wailian999

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/gsidgdurf.sHtML

[Q28] 求和与平均
来源：http://wap.fanxiaobao.xyz/Article/details/gwyiqbrjw.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gjerrzozy.sHtML

[Q29] 最大最小值
来源：http://www.share.fanxiaobao.xyz/Article/details/gpnjbeslh.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzhojhqiy.sHtML

[Q30] 分组统计
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gozhxhbqp.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.fanxiaobao.xyz/Article/details/gfveeopwc.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcncsxdtu.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://baike.fanxiaobao.xyz/Article/details/gaiwgvrcf.sHtML

[Q32] 分组拼接字符串
来源：http://baike.fanxiaobao.xyz/Article/details/gyotgotys.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.fanxiaobao.xyz/Article/details/gncqralyo.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.fanxiaobao.xyz/Article/details/gajhqhmzv.sHtML

[Q33] 多列分组
来源：http://blog.fanxiaobao.xyz/Article/details/gjczhoswu.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.fanxiaobao.xyz/Article/details/gdhnjaugc.sHtML

[Q34] 每组取第一条
来源：http://mobile.fanxiaobao.xyz/Article/details/gjaytaabm.sHtML

SELECT * FROM (
来源：http://mobile.fanxiaobao.xyz/Article/details/gzhkcgpaj.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxupfespj.sHtML

) t WHERE rn = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gnaodkvcl.sHtML

[Q35] 内连接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpjwjssro.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.fanxiaobao.xyz/Article/details/gsxqtkdet.sHtML

[Q36] 左连接
来源：http://blog.fanxiaobao.xyz/Article/details/gsqfdwtxd.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.fanxiaobao.xyz/Article/details/gaijleizo.sHtML

[Q37] 右连接
来源：http://m.share.fanxiaobao.xyz/Article/details/glgbqarbb.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdrhecqvz.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://read.share.fanxiaobao.xyz/Article/details/gvicqckac.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkodknnmn.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.fanxiaobao.xyz/Article/details/gyijfomaa.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.fanxiaobao.xyz/Article/details/gmsqwrtrw.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzwhwjodk.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdbxsrfmi.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.fanxiaobao.xyz/Article/details/geraxjuji.sHtML

[Q41] 多表连接
来源：http://www.share.fanxiaobao.xyz/Article/details/gikjolsvw.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.fanxiaobao.xyz/Article/details/gmdgkzzzp.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.fanxiaobao.xyz/Article/details/glbqeyrar.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.fanxiaobao.xyz/Article/details/gvpykmkzh.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwoirdldv.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.fanxiaobao.xyz/Article/details/gxjnhkmgj.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.fanxiaobao.xyz/Article/details/gobxtvqjl.sHtML

[Q43] 标量子查询
来源：http://blog.fanxiaobao.xyz/Article/details/gulatgdgy.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.fanxiaobao.xyz/Article/details/gryczuyur.sHtML

[Q44] IN 子查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gdhnhsvka.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjubmjhli.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.fanxiaobao.xyz/Article/details/geubkljfb.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fanxiaobao.xyz/Article/details/gsgjlncea.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtaoqresd.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkjfcippt.sHtML

[Q47] 与平均值比较
来源：http://baike.fanxiaobao.xyz/Article/details/gvetdjhha.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjegmpdsl.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gnzultwys.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.fanxiaobao.xyz/Article/details/ghheasdnt.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.fanxiaobao.xyz/Article/details/gjtwwnmiy.sHtML

[Q49] 更新单行
来源：http://3g.fanxiaobao.xyz/Article/details/gmzihrhiz.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gibezwnjl.sHtML

[Q50] 批量更新
来源：http://3g.fanxiaobao.xyz/Article/details/gcuxgnibb.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.fanxiaobao.xyz/Article/details/gfgdikkng.sHtML

[Q51] 用子查询更新
来源：http://blog.fanxiaobao.xyz/Article/details/glgofvzug.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gsyorbziv.sHtML

[Q52] 删除指定行
来源：http://m.share.fanxiaobao.xyz/Article/details/glggwnsgx.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gczkbygwq.sHtML

[Q53] 按条件删除
来源：http://3g.fanxiaobao.xyz/Article/details/giqxdgmqu.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.fanxiaobao.xyz/Article/details/gmeqnluiw.sHtML

[Q54] 清空表
来源：http://mobile.fanxiaobao.xyz/Article/details/gsrvosrhs.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.fanxiaobao.xyz/Article/details/gnjeoaflo.sHtML

[Q55] 排名（并列占位）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwobwjkbc.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.fanxiaobao.xyz/Article/details/gxwybklsn.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.share.fanxiaobao.xyz/Article/details/gkgpyzkdj.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqezhyjsp.sHtML

[Q57] 行号
来源：http://blog.fanxiaobao.xyz/Article/details/gsxkdoylk.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/gtvuoxtko.sHtML

[Q58] 累计求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gicmenzim.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://baike.fanxiaobao.xyz/Article/details/gsdqvktnn.sHtML

[Q59] 分组内累计
来源：http://www.blog.fanxiaobao.xyz/Article/details/gajjgfgpl.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.fanxiaobao.xyz/Article/details/gsvrgvwnj.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.fanxiaobao.xyz/Article/details/gwbovhtmx.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.fanxiaobao.xyz/Article/details/gnishwexb.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gruzjxwwk.sHtML

[Q61] 移动平均
来源：http://3g.fanxiaobao.xyz/Article/details/gexbzrsoj.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/gmbwyoext.sHtML

[Q62] 分组占比
来源：http://read.share.fanxiaobao.xyz/Article/details/gwvbjwjqe.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbjfmjsrq.sHtML

[Q63] 开启事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwsccpsdy.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://wap.fanxiaobao.xyz/Article/details/gzcilekdd.sHtML

[Q64] 提交事务
来源：http://read.share.fanxiaobao.xyz/Article/details/gmomfrnrh.sHtML

COMMIT;
来源：http://www.share.fanxiaobao.xyz/Article/details/gyystwbng.sHtML

[Q65] 回滚事务
来源：http://blog.fanxiaobao.xyz/Article/details/gluuvkpcs.sHtML

ROLLBACK;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbsmrjkzx.sHtML

[Q66] 行锁查询
来源：http://www.share.fanxiaobao.xyz/Article/details/gxngvuyli.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggqoqqnvr.sHtML

[Q67] 设置隔离级别
来源：http://www.share.fanxiaobao.xyz/Article/details/guzswkyro.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfrevbqoc.sHtML

[Q68] 保存点
来源：http://m.share.fanxiaobao.xyz/Article/details/gptxuyxyy.sHtML

SAVEPOINT sp1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwravkctl.sHtML

ROLLBACK TO sp1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjnecgzfx.sHtML

[Q69] 查看执行计划
来源：http://blog.fanxiaobao.xyz/Article/details/gnjzkxizo.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.fanxiaobao.xyz/Article/details/gskozfovc.sHtML

[Q70] 更新统计信息
来源：http://baike.fanxiaobao.xyz/Article/details/gzrubebsb.sHtML

ANALYZE TABLE users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gevgkhhsm.sHtML

[Q71] 查看建表语句
来源：http://www.share.fanxiaobao.xyz/Article/details/gepaoualo.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzqxjgpcl.sHtML

[Q72] 查看索引
来源：http://www.share.fanxiaobao.xyz/Article/details/gwlarhdop.sHtML

SHOW INDEX FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gikoagzin.sHtML

[Q73] 查看表状态
来源：http://www.blog.fanxiaobao.xyz/Article/details/gagommvrt.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.fanxiaobao.xyz/Article/details/gikuiliwc.sHtML

[Q74] 强制使用索引
来源：http://3g.fanxiaobao.xyz/Article/details/ghvuizugy.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.fanxiaobao.xyz/Article/details/gcgfzjyhb.sHtML

[Q75] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glylhfgsy.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://m.share.fanxiaobao.xyz/Article/details/gjyowsqlu.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.fanxiaobao.xyz/Article/details/gkkjlcaye.sHtML

[Q76] 按天统计
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcuprweii.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmhokfbby.sHtML

[Q77] 时间加减
来源：http://www.share.fanxiaobao.xyz/Article/details/gychpwgtg.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fanxiaobao.xyz/Article/details/gvcryixlh.sHtML

[Q78] 当前时间
来源：http://wap.fanxiaobao.xyz/Article/details/guuachanf.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.fanxiaobao.xyz/Article/details/gmcnmnukq.sHtML

[Q79] 字符串拼接
来源：http://www.blog.fanxiaobao.xyz/Article/details/gycfgjmhi.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.fanxiaobao.xyz/Article/details/gaortinwf.sHtML

[Q80] 字符串截取
来源：http://read.share.fanxiaobao.xyz/Article/details/gqizqjnpc.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.fanxiaobao.xyz/Article/details/ghnntzwib.sHtML

[Q81] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gekpbnykx.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.fanxiaobao.xyz/Article/details/gcyslhehw.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fanxiaobao.xyz/Article/details/girkdjkfi.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gbnijdorm.sHtML

[Q83] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gxrysgrsp.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbxqvmvkj.sHtML

[Q84] 去除首尾空格
来源：http://baike.fanxiaobao.xyz/Article/details/ggylyssdv.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gbqirirhb.sHtML

[Q85] 数值取整
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjtkbmmjx.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.fanxiaobao.xyz/Article/details/gbwsxsopv.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcmrskous.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fanxiaobao.xyz/Article/details/gbxwdazni.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gnznmwndj.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.fanxiaobao.xyz/Article/details/gmzisqmxy.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.fanxiaobao.xyz/Article/details/gapcrjkzn.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fanxiaobao.xyz/Article/details/givxsurmr.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fanxiaobao.xyz/Article/details/gfxshqdvg.sHtML

[Q89] 判断表是否存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gvwvuxztr.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fanxiaobao.xyz/Article/details/ggxjmycdy.sHtML

[Q90] 生成序号列
来源：http://blog.fanxiaobao.xyz/Article/details/gxanfpppq.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.fanxiaobao.xyz/Article/details/gnqhighqh.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gnpllhqyq.sHtML

R. Bash 专题
来源：http://baike.fanxiaobao.xyz/Article/details/gaqvlszep.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gajiwvnjt.sHtML

[R01] shebang 与严格模式
来源：http://wap.fanxiaobao.xyz/Article/details/gvqvrudgz.sHtML

#!/usr/bin/env bash
来源：http://read.share.fanxiaobao.xyz/Article/details/gptmzgyet.sHtML

set -euo pipefail
来源：http://baike.fanxiaobao.xyz/Article/details/greqjvdor.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fanxiaobao.xyz/Article/details/goprzrals.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fanxiaobao.xyz/Article/details/gyxomjjha.sHtML

[R03] 只读变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsasdfxqd.sHtML

readonly PI=3.14
来源：http://www.share.fanxiaobao.xyz/Article/details/gdlinmzrh.sHtML

[R04] 位置参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gnzwjjjpt.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fanxiaobao.xyz/Article/details/gddhrnpzf.sHtML

[R05] 参数默认值
来源：http://3g.fanxiaobao.xyz/Article/details/gbusiljdz.sHtML

name="${1:-default}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpmqplkwe.sHtML

[R06] 判断命令是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gbsjrvwbc.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gowkwnpel.sHtML

[R07] if 判断文件
来源：http://www.share.fanxiaobao.xyz/Article/details/ghsdvtzzp.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/ghwrcqvtl.sHtML

[R08] 数值比较
来源：http://read.share.fanxiaobao.xyz/Article/details/grilgkpri.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gygwkgbbm.sHtML

[R09] 字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gquenluqp.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggbqtoqlm.sHtML

[R10] 正则匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gfpsboblh.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/ggtujijmk.sHtML

[R11] case 多分支
来源：http://www.blog.fanxiaobao.xyz/Article/details/grazlcxbr.sHtML

case "$1" in
来源：http://mobile.fanxiaobao.xyz/Article/details/ghtloqtzs.sHtML

start) echo "启动" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/ghtuclxfe.sHtML

stop)  echo "停止" ;;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnxybyslt.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gakgzmhfu.sHtML

esac
来源：http://mobile.fanxiaobao.xyz/Article/details/gxczkatzx.sHtML

[R12] for 遍历文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gguscaytr.sHtML

for f in *.txt; do echo "$f"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/ghlnsxfij.sHtML

[R13] for 计数循环
来源：http://blog.fanxiaobao.xyz/Article/details/gusnmnypm.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gwdrflldi.sHtML

[R14] C 风格 for
来源：http://m.share.fanxiaobao.xyz/Article/details/gxttbayzj.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gvhuzcxtq.sHtML

[R15] while 逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gryrghrle.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gwguemcae.sHtML

[R16] until 等待条件
来源：http://wap.fanxiaobao.xyz/Article/details/gosrxefve.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gspnogwdg.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwyinmmuw.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fanxiaobao.xyz/Article/details/ggshpnwra.sHtML

[R18] 遍历数组
来源：http://wap.fanxiaobao.xyz/Article/details/guufxmuic.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gmkkqcdyn.sHtML

[R19] 数组长度
来源：http://wap.fanxiaobao.xyz/Article/details/gnfiwdueg.sHtML

echo "${#arr[@]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gwniwgkqt.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpovgshyf.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzbovbypa.sHtML

[R21] 字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gvpxpdekc.sHtML

echo "${#s}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gkydeqxhf.sHtML

[R22] 截取子串
来源：http://mobile.fanxiaobao.xyz/Article/details/gszopuwko.sHtML

echo "${s:0:5}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gqvhaayhj.sHtML

[R23] 字符串替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gifteeoxi.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfiuyjthx.sHtML

[R24] 大小写转换
来源：http://wap.fanxiaobao.xyz/Article/details/gcsmkuzzz.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gmkqpblpv.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fanxiaobao.xyz/Article/details/gvzqrxjpa.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gjamrmhil.sHtML

[R26] 命令替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gfjccfeor.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fanxiaobao.xyz/Article/details/ggnjtbzic.sHtML

[R27] 算术展开
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gphgukgqi.sHtML

echo $((1 + 2 * 3))
来源：http://blog.fanxiaobao.xyz/Article/details/ghwzjzezu.sHtML

[R28] 浮点运算
来源：http://www.share.fanxiaobao.xyz/Article/details/geousfdrv.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fanxiaobao.xyz/Article/details/glepritrz.sHtML

[R29] 定义函数
来源：http://3g.fanxiaobao.xyz/Article/details/grfvcxxqr.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fanxiaobao.xyz/Article/details/glwhhbhzy.sHtML

[R30] 函数返回状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gkamfwxws.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.fanxiaobao.xyz/Article/details/gvatejyva.sHtML

[R31] 局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gpwrddthx.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdhigsvpv.sHtML

[R32] 参数个数校验
来源：http://read.share.fanxiaobao.xyz/Article/details/gnaurdvyt.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjxpsdxgu.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fanxiaobao.xyz/Article/details/gigbnmczq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.fanxiaobao.xyz/Article/details/grbeewmhk.sHtML

[R34] 退出时清理
来源：http://m.share.fanxiaobao.xyz/Article/details/gglgkyiau.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gwtdxxmpg.sHtML

[R35] 后台执行并等待
来源：http://3g.fanxiaobao.xyz/Article/details/gvcadskyp.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fanxiaobao.xyz/Article/details/gabwhrsqe.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfsxvcuij.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fanxiaobao.xyz/Article/details/gcjagagjc.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsohcupqz.sHtML

files=$(ls -1)
来源：http://baike.fanxiaobao.xyz/Article/details/gqwmxweik.sHtML

[R38] 管道串联
来源：http://read.share.fanxiaobao.xyz/Article/details/giwqckefw.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gfspuwpne.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fanxiaobao.xyz/Article/details/gdhhxobfr.sHtML

cmd > out.log 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gjdvjsear.sHtML

[R40] 追加写日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gfdzzhyjl.sHtML

echo "log" >> out.log
来源：http://m.share.fanxiaobao.xyz/Article/details/ggpioxgjq.sHtML

[R41] 丢弃输出
来源：http://wap.fanxiaobao.xyz/Article/details/gwzlpsztf.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzpayoafa.sHtML

[R42] 输入重定向
来源：http://mobile.fanxiaobao.xyz/Article/details/gfmtqfygb.sHtML

wc -l < a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gckyxbsei.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggnqdbkmv.sHtML

find . -name "*.log" -type f
来源：http://mobile.fanxiaobao.xyz/Article/details/grmypfdjw.sHtML

[R44] 按修改时间查找
来源：http://baike.fanxiaobao.xyz/Article/details/gjiwmhhpm.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvnisfxld.sHtML

[R45] 批量删除
来源：http://baike.fanxiaobao.xyz/Article/details/gmnuyqarf.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glyxhluny.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fanxiaobao.xyz/Article/details/glpunsvxf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fanxiaobao.xyz/Article/details/gcpkdbaca.sHtML

[R47] sed 单行替换
来源：http://3g.fanxiaobao.xyz/Article/details/gticypgga.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gvmoxzdzx.sHtML

[R48] awk 取指定列
来源：http://3g.fanxiaobao.xyz/Article/details/gwztlgnob.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gqhpijjzl.sHtML

[R49] awk 带条件
来源：http://wap.fanxiaobao.xyz/Article/details/ghpoysduz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fanxiaobao.xyz/Article/details/gipgaputn.sHtML

[R50] awk 求和
来源：http://baike.fanxiaobao.xyz/Article/details/gjwgdalfy.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gutiifhkj.sHtML

[R51] 排序去重取前几
来源：http://wap.fanxiaobao.xyz/Article/details/gnjlkgnyc.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fanxiaobao.xyz/Article/details/gvppfwmqq.sHtML

[R52] 统计行数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gytljucbr.sHtML

wc -l a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gorxfkuvq.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fanxiaobao.xyz/Article/details/gzqlypner.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fanxiaobao.xyz/Article/details/geykmkkro.sHtML

[R54] 比较两个文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gpxqeicju.sHtML

diff a.txt b.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdgkuwnne.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyilpdhzo.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsylbcghk.sHtML

[R56] 远程拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gbyzkfanf.sHtML

scp file user@host:/path/
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbwlidlif.sHtML

[R57] 远程执行命令
来源：http://3g.fanxiaobao.xyz/Article/details/gfxnoibxc.sHtML

ssh user@host 'uptime'
来源：http://blog.fanxiaobao.xyz/Article/details/gzlhavsba.sHtML

[R58] 下载文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghkrvpyzk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fanxiaobao.xyz/Article/details/gfstwamel.sHtML

[R59] 发 POST JSON
来源：http://blog.fanxiaobao.xyz/Article/details/gfimcpdbz.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fanxiaobao.xyz/Article/details/glvaauccl.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/guhtdedia.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fanxiaobao.xyz/Article/details/gqduuyhkm.sHtML

[R61] 磁盘占用
来源：http://m.share.fanxiaobao.xyz/Article/details/gpzbzejin.sHtML

df -h;  du -sh *
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjiptvzkj.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fanxiaobao.xyz/Article/details/ghzebzgci.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fanxiaobao.xyz/Article/details/gwyokiwjc.sHtML

[R63] 内存与进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gtfioiwjp.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fanxiaobao.xyz/Article/details/gfuzojyei.sHtML

[R64] 结束进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gufhywxdj.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fanxiaobao.xyz/Article/details/gotcoijtk.sHtML

[R65] 查看端口占用
来源：http://baike.fanxiaobao.xyz/Article/details/giedlirlj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fanxiaobao.xyz/Article/details/gkblznpsx.sHtML

[R66] 定时任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gjwanivyk.sHtML

crontab -e;  crontab -l
来源：http://www.share.fanxiaobao.xyz/Article/details/gfrezwxum.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fanxiaobao.xyz/Article/details/gxkyduyqz.sHtML

openssl rand -hex 16
来源：http://3g.fanxiaobao.xyz/Article/details/gawcekhrs.sHtML

[R68] 计算文件校验值
来源：http://wap.fanxiaobao.xyz/Article/details/golrfwfjx.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/giyxuezqa.sHtML

[R69] 生成随机密码
来源：http://www.share.fanxiaobao.xyz/Article/details/gcsutnnrc.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fanxiaobao.xyz/Article/details/gftosrkzm.sHtML

[R70] 时间戳与互转
来源：http://www.share.fanxiaobao.xyz/Article/details/gljfxmyen.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkowxhevm.sHtML

[R71] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gjnnmyqhc.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fanxiaobao.xyz/Article/details/ghbpdrjdj.sHtML

[R72] 等待端口就绪
来源：http://m.share.fanxiaobao.xyz/Article/details/gyrcfzyfu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/grjbtybuf.sHtML

[R73] 分割大日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvijpsgoa.sHtML

split -l 1000 big.log part_
来源：http://www.share.fanxiaobao.xyz/Article/details/gtfvkxgdl.sHtML

[R74] 批量重命名
来源：http://wap.fanxiaobao.xyz/Article/details/gmwnbwprn.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gmrahzphz.sHtML

[R75] 导出环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/gcrufwymu.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fanxiaobao.xyz/Article/details/gxjdisgck.sHtML

[R76] 使用临时文件
来源：http://blog.fanxiaobao.xyz/Article/details/gjqrhirbx.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gazzbykvo.sHtML

[R77] 读取用户输入
来源：http://wap.fanxiaobao.xyz/Article/details/gfuajvwif.sHtML


<!-- 参考信息 -->