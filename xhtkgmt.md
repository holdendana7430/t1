代发 wailian999

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://wap.hesvh.cn/Article/details/gzgfrlwbg.sHtML

[Q28] 求和与平均
来源：http://www.m.share.fehbvm.com/Article/details/gjmvvkaef.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/glfoomdjj.sHtML

[Q29] 最大最小值
来源：http://wap.hesvh.cn/Article/details/glsrbvqgt.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gwbqkozdu.sHtML

[Q30] 分组统计
来源：http://3g.hesvh.cn/Article/details/glqdqjbqf.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://blog.fehbvm.com/Article/details/gopugvzfq.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gadklpbyf.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.zdbjq.cn/Article/details/gfeuvppms.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gjrdvtpny.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/gmibrkjlx.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://read.share.fehbvm.com/Article/details/giughsnud.sHtML

[Q33] 多列分组
来源：http://baike.hesvh.cn/Article/details/grgwnqzby.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.zdbjq.cn/Article/details/gonptmiwl.sHtML

[Q34] 每组取第一条
来源：http://baike.hesvh.cn/Article/details/gumsabufh.sHtML

SELECT * FROM (
来源：http://www.share.zdbjq.cn/Article/details/gsuchqabf.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.fehbvm.com/Article/details/gxoalnfee.sHtML

) t WHERE rn = 1;
来源：http://www.m.share.hesvh.cn/Article/details/gavwdatui.sHtML

[Q35] 内连接
来源：http://mobile.fehbvm.com/Article/details/gulaxqivi.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.zdbjq.cn/Article/details/gxgteccmu.sHtML

[Q36] 左连接
来源：http://baike.fehbvm.com/Article/details/gbjgbqvmq.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.hesvh.cn/Article/details/gjbstneqr.sHtML

[Q37] 右连接
来源：http://baike.fehbvm.com/Article/details/gegqqotfh.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.hesvh.cn/Article/details/gzasuidow.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.zdbjq.cn/Article/details/ggzklgdas.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.fehbvm.com/Article/details/gnojcjyel.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.hesvh.cn/Article/details/gzcuwxuaf.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.fehbvm.com/Article/details/gzsdodpwb.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.fehbvm.com/Article/details/gwhvypmri.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.hesvh.cn/Article/details/gxsjughxl.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.hesvh.cn/Article/details/gumeubgzr.sHtML

[Q41] 多表连接
来源：http://wap.zdbjq.cn/Article/details/gulcwyzoh.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://baike.zdbjq.cn/Article/details/gekxtoefl.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.hesvh.cn/Article/details/glkyrdoeu.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.hesvh.cn/Article/details/gambexjrc.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.hesvh.cn/Article/details/gczfrytfe.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.fehbvm.com/Article/details/gdbjuwxqy.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.zdbjq.cn/Article/details/gkbkkdipe.sHtML

[Q43] 标量子查询
来源：http://read.share.fehbvm.com/Article/details/gmswkaeim.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.blog.fehbvm.com/Article/details/glbbeqfue.sHtML

[Q44] IN 子查询
来源：http://baike.zdbjq.cn/Article/details/gpcxxegjp.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.fehbvm.com/Article/details/garinyohu.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.zdbjq.cn/Article/details/gtlredzop.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://m.share.fehbvm.com/Article/details/gbdufltaw.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.blog.hesvh.cn/Article/details/ggoollmlc.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fehbvm.com/Article/details/gptyxqpok.sHtML

[Q47] 与平均值比较
来源：http://blog.fehbvm.com/Article/details/gewqqimfb.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.zdbjq.cn/Article/details/gtyilcfpv.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.fehbvm.com/Article/details/glkizapnh.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://wap.fehbvm.com/Article/details/gkddlliwe.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.zdbjq.cn/Article/details/gtmsdnogx.sHtML

[Q49] 更新单行
来源：http://baike.fehbvm.com/Article/details/grvlvvcqz.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.hesvh.cn/Article/details/gtdlhjhtc.sHtML

[Q50] 批量更新
来源：http://www.blog.zdbjq.cn/Article/details/googdiymh.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.fehbvm.com/Article/details/gajacbuap.sHtML

[Q51] 用子查询更新
来源：http://mobile.fehbvm.com/Article/details/gfzmzuvfe.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.hesvh.cn/Article/details/gzembzybt.sHtML

[Q52] 删除指定行
来源：http://mobile.hesvh.cn/Article/details/gvkzrdwyc.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.zdbjq.cn/Article/details/gnsfbnoud.sHtML

[Q53] 按条件删除
来源：http://www.m.share.zdbjq.cn/Article/details/ggrjgkmwf.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://3g.hesvh.cn/Article/details/ghgcmfaxq.sHtML

[Q54] 清空表
来源：http://3g.hesvh.cn/Article/details/gbbumeqda.sHtML

TRUNCATE TABLE logs;
来源：http://3g.hesvh.cn/Article/details/gcqovgdkx.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.hesvh.cn/Article/details/gphduuwue.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.fehbvm.com/Article/details/gksptggmt.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.zdbjq.cn/Article/details/gnasxdctu.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.hesvh.cn/Article/details/gllebbosk.sHtML

[Q57] 行号
来源：http://www.share.fehbvm.com/Article/details/gpirbltrz.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.hesvh.cn/Article/details/gujhumuyb.sHtML

[Q58] 累计求和
来源：http://www.blog.hesvh.cn/Article/details/guqlwfmmd.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.zdbjq.cn/Article/details/grfxfqjvz.sHtML

[Q59] 分组内累计
来源：http://mobile.zdbjq.cn/Article/details/gkknpnhgh.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.zdbjq.cn/Article/details/gymevgzpq.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.hesvh.cn/Article/details/gqwukqupd.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://blog.hesvh.cn/Article/details/glhgwtgiw.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gwdgjhvqa.sHtML

[Q61] 移动平均
来源：http://blog.hesvh.cn/Article/details/grlfrtwyc.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gdltjiftw.sHtML

[Q62] 分组占比
来源：http://www.m.share.zdbjq.cn/Article/details/gizsbcenz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.blog.zdbjq.cn/Article/details/gcchbaxvp.sHtML

[Q63] 开启事务
来源：http://www.blog.fehbvm.com/Article/details/grnvtemhw.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.zdbjq.cn/Article/details/gecjvneyt.sHtML

[Q64] 提交事务
来源：http://www.blog.fehbvm.com/Article/details/gkulhegma.sHtML

COMMIT;
来源：http://wap.hesvh.cn/Article/details/gpxttxxbx.sHtML

[Q65] 回滚事务
来源：http://mobile.fehbvm.com/Article/details/grklciybm.sHtML

ROLLBACK;
来源：http://m.share.zdbjq.cn/Article/details/ggslxqnrb.sHtML

[Q66] 行锁查询
来源：http://www.m.share.hesvh.cn/Article/details/gamgrkdel.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.hesvh.cn/Article/details/ghkcuezwe.sHtML

[Q67] 设置隔离级别
来源：http://blog.hesvh.cn/Article/details/gzlzkhaov.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://mobile.hesvh.cn/Article/details/gkyvjeqge.sHtML

[Q68] 保存点
来源：http://www.share.fehbvm.com/Article/details/ggdlmorlx.sHtML

SAVEPOINT sp1;
来源：http://www.share.hesvh.cn/Article/details/gyplpetyx.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fehbvm.com/Article/details/glsvbudoh.sHtML

[Q69] 查看执行计划
来源：http://baike.zdbjq.cn/Article/details/gelwpnmbd.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.zdbjq.cn/Article/details/ggurfrtra.sHtML

[Q70] 更新统计信息
来源：http://wap.zdbjq.cn/Article/details/gjgjrkqde.sHtML

ANALYZE TABLE users;
来源：http://blog.hesvh.cn/Article/details/gwhztgjss.sHtML

[Q71] 查看建表语句
来源：http://baike.zdbjq.cn/Article/details/ggeydqbfn.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.zdbjq.cn/Article/details/gaduffgjm.sHtML

[Q72] 查看索引
来源：http://www.share.hesvh.cn/Article/details/gzmwtjoyb.sHtML

SHOW INDEX FROM users;
来源：http://wap.zdbjq.cn/Article/details/gtpzhwwpc.sHtML

[Q73] 查看表状态
来源：http://www.m.share.hesvh.cn/Article/details/grvugktka.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.fehbvm.com/Article/details/gwdkgxmuq.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.fehbvm.com/Article/details/gaulghdnm.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.zdbjq.cn/Article/details/gydsqtjbh.sHtML

[Q75] 日期格式化
来源：http://mobile.zdbjq.cn/Article/details/gwubquzjt.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gvmvckqta.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.fehbvm.com/Article/details/ghbwtajgu.sHtML

[Q76] 按天统计
来源：http://baike.zdbjq.cn/Article/details/gbabohtil.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.fehbvm.com/Article/details/gjskpmmzo.sHtML

[Q77] 时间加减
来源：http://read.share.hesvh.cn/Article/details/glyhlimxf.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.zdbjq.cn/Article/details/gbodvycph.sHtML

[Q78] 当前时间
来源：http://blog.hesvh.cn/Article/details/gxpvcaudm.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.fehbvm.com/Article/details/gqpjarlac.sHtML

[Q79] 字符串拼接
来源：http://3g.fehbvm.com/Article/details/gwvdltfjw.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.zdbjq.cn/Article/details/gixpmxufj.sHtML

[Q80] 字符串截取
来源：http://m.share.hesvh.cn/Article/details/gvgmmohof.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.fehbvm.com/Article/details/ghqwgtgbj.sHtML

[Q81] 字符串替换
来源：http://read.share.fehbvm.com/Article/details/gowfooykf.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gthppncew.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.zdbjq.cn/Article/details/gdqxmtojr.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://3g.zdbjq.cn/Article/details/gxuizxrmo.sHtML

[Q83] 大小写转换
来源：http://wap.zdbjq.cn/Article/details/gifootasa.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/goyvgmnmf.sHtML

[Q84] 去除首尾空格
来源：http://blog.fehbvm.com/Article/details/gcadmvwos.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gskwtddig.sHtML

[Q85] 数值取整
来源：http://www.m.share.hesvh.cn/Article/details/ghnqioqai.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.zdbjq.cn/Article/details/gfqkgidyz.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.zdbjq.cn/Article/details/gqzfenpxd.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.zdbjq.cn/Article/details/gsftfwwax.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fehbvm.com/Article/details/gogzqpfif.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.zdbjq.cn/Article/details/gkfvjubnl.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.hesvh.cn/Article/details/gvkfjyqjb.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.fehbvm.com/Article/details/ggdtrazxx.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gxmwwcsmr.sHtML

[Q89] 判断表是否存在
来源：http://wap.zdbjq.cn/Article/details/gaqvxgvoq.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.share.hesvh.cn/Article/details/gxxtuwwoa.sHtML

[Q90] 生成序号列
来源：http://blog.zdbjq.cn/Article/details/ggfrkztxt.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.fehbvm.com/Article/details/gfxxkakof.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gewugltva.sHtML

R. Bash 专题
来源：http://www.share.zdbjq.cn/Article/details/gltpyzvjr.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gkxyqlbfs.sHtML

[R01] shebang 与严格模式
来源：http://mobile.fehbvm.com/Article/details/gbecdmmjq.sHtML

#!/usr/bin/env bash
来源：http://m.share.hesvh.cn/Article/details/gyuylujik.sHtML

set -euo pipefail
来源：http://blog.zdbjq.cn/Article/details/gjdaqgfvt.sHtML

[R02] 变量赋值与使用
来源：http://wap.fehbvm.com/Article/details/gburzlhne.sHtML

name="Tom"; echo "$name"
来源：http://wap.zdbjq.cn/Article/details/gmogqwtjy.sHtML

[R03] 只读变量
来源：http://www.share.hesvh.cn/Article/details/gnelpfqdq.sHtML

readonly PI=3.14
来源：http://www.blog.fehbvm.com/Article/details/ggejaphkn.sHtML

[R04] 位置参数
来源：http://www.m.share.zdbjq.cn/Article/details/gdlcavrcf.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.hesvh.cn/Article/details/gowflnpig.sHtML

[R05] 参数默认值
来源：http://read.share.zdbjq.cn/Article/details/gpgxqlgjk.sHtML

name="${1:-default}"
来源：http://baike.hesvh.cn/Article/details/gdgqmaigv.sHtML

[R06] 判断命令是否存在
来源：http://m.share.hesvh.cn/Article/details/gluiaphuw.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.hesvh.cn/Article/details/gcywoxtrs.sHtML

[R07] if 判断文件
来源：http://www.share.fehbvm.com/Article/details/gogfetyhr.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.hesvh.cn/Article/details/gphsmscep.sHtML

[R08] 数值比较
来源：http://www.m.share.zdbjq.cn/Article/details/giviqajmn.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fehbvm.com/Article/details/ggkhyhbyi.sHtML

[R09] 字符串比较
来源：http://baike.hesvh.cn/Article/details/gabirbnua.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.zdbjq.cn/Article/details/gteqlnhgx.sHtML

[R10] 正则匹配
来源：http://read.share.hesvh.cn/Article/details/gwpldmshg.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.hesvh.cn/Article/details/gqwtewesu.sHtML

[R11] case 多分支
来源：http://blog.hesvh.cn/Article/details/gcwjqfbcj.sHtML

case "$1" in
来源：http://wap.zdbjq.cn/Article/details/gojitiztz.sHtML

start) echo "启动" ;;
来源：http://3g.fehbvm.com/Article/details/gmsnsgpud.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.hesvh.cn/Article/details/gnzwqxuag.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fehbvm.com/Article/details/gxpigvopw.sHtML

esac
来源：http://3g.zdbjq.cn/Article/details/ggedhgmrv.sHtML

[R12] for 遍历文件
来源：http://3g.zdbjq.cn/Article/details/gfygcvikc.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fehbvm.com/Article/details/gqqqsrhnb.sHtML

[R13] for 计数循环
来源：http://3g.fehbvm.com/Article/details/gkeohkzab.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.zdbjq.cn/Article/details/gybisudyz.sHtML

[R14] C 风格 for
来源：http://3g.hesvh.cn/Article/details/gzwncbahb.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/gvgwzmfkq.sHtML

[R15] while 逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gwuqninaz.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.zdbjq.cn/Article/details/gsxbzcpqm.sHtML

[R16] until 等待条件
来源：http://baike.zdbjq.cn/Article/details/gvhffckmx.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/gkcxbwpjf.sHtML

[R17] 数组定义与取值
来源：http://blog.hesvh.cn/Article/details/gjjznczqn.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.zdbjq.cn/Article/details/gdjvorapp.sHtML

[R18] 遍历数组
来源：http://www.m.share.hesvh.cn/Article/details/gtufjehpe.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://3g.hesvh.cn/Article/details/gzywioizc.sHtML

[R19] 数组长度
来源：http://www.blog.zdbjq.cn/Article/details/gxltnfxrx.sHtML

echo "${#arr[@]}"
来源：http://baike.hesvh.cn/Article/details/gaufgfwpt.sHtML

[R20] 关联数组（字典）
来源：http://baike.hesvh.cn/Article/details/gypqwvdll.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.zdbjq.cn/Article/details/ggkwwwgcp.sHtML

[R21] 字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/gpccgwoqh.sHtML

echo "${#s}"
来源：http://baike.zdbjq.cn/Article/details/gbcgbuwbj.sHtML

[R22] 截取子串
来源：http://www.blog.fehbvm.com/Article/details/gzyypyywj.sHtML

echo "${s:0:5}"
来源：http://www.m.share.fehbvm.com/Article/details/gvohtmbiz.sHtML

[R23] 字符串替换
来源：http://3g.hesvh.cn/Article/details/gwqaraxzh.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.hesvh.cn/Article/details/gaswpjlud.sHtML

[R24] 大小写转换
来源：http://wap.zdbjq.cn/Article/details/gwdjmnifl.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.hesvh.cn/Article/details/grsfwvmti.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.hesvh.cn/Article/details/gfnvwzsut.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.zdbjq.cn/Article/details/gstbkoynw.sHtML

[R26] 命令替换
来源：http://www.blog.hesvh.cn/Article/details/gbkrudjhe.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.zdbjq.cn/Article/details/gycalfwdn.sHtML

[R27] 算术展开
来源：http://www.m.share.fehbvm.com/Article/details/gchkzegtc.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.hesvh.cn/Article/details/gcwqdogca.sHtML

[R28] 浮点运算
来源：http://www.m.share.zdbjq.cn/Article/details/ghdzavstv.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.zdbjq.cn/Article/details/ghrtvleqm.sHtML

[R29] 定义函数
来源：http://mobile.fehbvm.com/Article/details/gaxfcjrqv.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.hesvh.cn/Article/details/gjjbplypz.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gubwlcftj.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.zdbjq.cn/Article/details/gfsqkltdg.sHtML

[R31] 局部变量
来源：http://wap.hesvh.cn/Article/details/gdrjpsfce.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkpghzaum.sHtML

[R32] 参数个数校验
来源：http://baike.zdbjq.cn/Article/details/gdmtzxvjc.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.hesvh.cn/Article/details/grfcjdvfw.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.zdbjq.cn/Article/details/gyoyhjnqt.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.hesvh.cn/Article/details/gmimvnrxh.sHtML

[R34] 退出时清理
来源：http://baike.hesvh.cn/Article/details/gfjrxpmoi.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.zdbjq.cn/Article/details/gtmupmlwm.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.zdbjq.cn/Article/details/godyclazz.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fehbvm.com/Article/details/grnnfbayy.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fehbvm.com/Article/details/gtikdsubz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.zdbjq.cn/Article/details/gvnwisqok.sHtML

[R37] 把输出赋给变量
来源：http://3g.zdbjq.cn/Article/details/glzclmyfz.sHtML

files=$(ls -1)
来源：http://3g.zdbjq.cn/Article/details/gjvuxvyqi.sHtML

[R38] 管道串联
来源：http://baike.hesvh.cn/Article/details/geizyaltn.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.hesvh.cn/Article/details/gadmvzcuh.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.hesvh.cn/Article/details/gqynjtvoc.sHtML

cmd > out.log 2>&1
来源：http://blog.hesvh.cn/Article/details/gucvlniuq.sHtML

[R40] 追加写日志
来源：http://mobile.hesvh.cn/Article/details/gpxwamaig.sHtML

echo "log" >> out.log
来源：http://blog.fehbvm.com/Article/details/gzvtuqkgi.sHtML

[R41] 丢弃输出
来源：http://baike.zdbjq.cn/Article/details/gnvhzvkmi.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.zdbjq.cn/Article/details/ghvundegj.sHtML

[R42] 输入重定向
来源：http://baike.fehbvm.com/Article/details/geabzgatq.sHtML

wc -l < a.txt
来源：http://baike.fehbvm.com/Article/details/gkzflaqli.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.zdbjq.cn/Article/details/ghuudvfza.sHtML

find . -name "*.log" -type f
来源：http://baike.fehbvm.com/Article/details/gqofpgccc.sHtML

[R44] 按修改时间查找
来源：http://read.share.fehbvm.com/Article/details/gxrnaqbki.sHtML

find . -mtime -7 -type f
来源：http://read.share.hesvh.cn/Article/details/gadufqdsu.sHtML

[R45] 批量删除
来源：http://wap.zdbjq.cn/Article/details/gdndtvlhl.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.hesvh.cn/Article/details/ghrpuksmt.sHtML

[R46] 递归替换文件内容
来源：http://m.share.zdbjq.cn/Article/details/gtmynhxky.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.zdbjq.cn/Article/details/gywhnmjqk.sHtML

[R47] sed 单行替换
来源：http://www.blog.fehbvm.com/Article/details/gsabmrczy.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fehbvm.com/Article/details/gqnptdyaz.sHtML

[R48] awk 取指定列
来源：http://mobile.hesvh.cn/Article/details/ghfxcuupn.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.zdbjq.cn/Article/details/gqkpuuprm.sHtML

[R49] awk 带条件
来源：http://baike.zdbjq.cn/Article/details/gxjhawmlw.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.zdbjq.cn/Article/details/gssqjytzr.sHtML

[R50] awk 求和
来源：http://read.share.hesvh.cn/Article/details/gaeehqixw.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gizucjadr.sHtML

[R51] 排序去重取前几
来源：http://3g.zdbjq.cn/Article/details/gtumtvkca.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.hesvh.cn/Article/details/gaapwxxvc.sHtML

[R52] 统计行数
来源：http://3g.zdbjq.cn/Article/details/gjtnymvuf.sHtML

wc -l a.txt
来源：http://www.share.fehbvm.com/Article/details/gqfatqwro.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fehbvm.com/Article/details/gzpdfzrbf.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.hesvh.cn/Article/details/ghsdordov.sHtML

[R54] 比较两个文件
来源：http://blog.zdbjq.cn/Article/details/gcxoanmwg.sHtML

diff a.txt b.txt
来源：http://blog.hesvh.cn/Article/details/gnyrvwtjm.sHtML

[R55] 压缩与解压
来源：http://baike.zdbjq.cn/Article/details/gytulqdpv.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.hesvh.cn/Article/details/ginsngoiu.sHtML

[R56] 远程拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gbbxqrjiz.sHtML

scp file user@host:/path/
来源：http://blog.hesvh.cn/Article/details/gqkipkgiz.sHtML

[R57] 远程执行命令
来源：http://mobile.zdbjq.cn/Article/details/gunwpngwo.sHtML

ssh user@host 'uptime'
来源：http://read.share.hesvh.cn/Article/details/geodszxst.sHtML

[R58] 下载文件
来源：http://read.share.fehbvm.com/Article/details/gvwcafkiq.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.zdbjq.cn/Article/details/gpawmllca.sHtML

[R59] 发 POST JSON
来源：http://blog.zdbjq.cn/Article/details/gblvxiseq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fehbvm.com/Article/details/gfxwkjynl.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.zdbjq.cn/Article/details/gotmyfxgz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fehbvm.com/Article/details/getuuuzcq.sHtML

[R61] 磁盘占用
来源：http://baike.zdbjq.cn/Article/details/gjjcjygje.sHtML

df -h;  du -sh *
来源：http://wap.hesvh.cn/Article/details/gugcccmhp.sHtML

[R62] 找最占空间的文件
来源：http://wap.hesvh.cn/Article/details/gijosyrhg.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.zdbjq.cn/Article/details/gnddjapjm.sHtML

[R63] 内存与进程
来源：http://baike.hesvh.cn/Article/details/gwkzlbyxd.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fehbvm.com/Article/details/gvizxkcrz.sHtML

[R64] 结束进程
来源：http://m.share.zdbjq.cn/Article/details/gnkrjbaci.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fehbvm.com/Article/details/gmblgzhlp.sHtML

[R65] 查看端口占用
来源：http://www.blog.zdbjq.cn/Article/details/gsmtploms.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fehbvm.com/Article/details/gqkkvnqbl.sHtML

[R66] 定时任务
来源：http://www.blog.zdbjq.cn/Article/details/gondevixn.sHtML

crontab -e;  crontab -l
来源：http://mobile.hesvh.cn/Article/details/gbhtcckrk.sHtML

[R67] 生成随机十六进制串
来源：http://baike.zdbjq.cn/Article/details/ghabjkxkx.sHtML

openssl rand -hex 16
来源：http://blog.fehbvm.com/Article/details/gpubcclfb.sHtML

[R68] 计算文件校验值
来源：http://m.share.hesvh.cn/Article/details/ggagsaxxs.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.hesvh.cn/Article/details/gollkzvjz.sHtML

[R69] 生成随机密码
来源：http://wap.fehbvm.com/Article/details/gvclwfrwd.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.hesvh.cn/Article/details/gnsfsqcgu.sHtML

[R70] 时间戳与互转
来源：http://wap.hesvh.cn/Article/details/gpqnxdery.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.hesvh.cn/Article/details/grtadxxbn.sHtML

[R71] 日期格式化
来源：http://baike.fehbvm.com/Article/details/gkxzhljfx.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.zdbjq.cn/Article/details/gvhnwbwlb.sHtML

[R72] 等待端口就绪
来源：http://www.share.fehbvm.com/Article/details/gprqjofka.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fehbvm.com/Article/details/gfrlbnodz.sHtML

[R73] 分割大日志
来源：http://blog.fehbvm.com/Article/details/guxrrxnfp.sHtML

split -l 1000 big.log part_
来源：http://www.blog.zdbjq.cn/Article/details/giwdbctwx.sHtML

[R74] 批量重命名
来源：http://wap.zdbjq.cn/Article/details/gdlmzoocv.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.zdbjq.cn/Article/details/gvljyfwny.sHtML

[R75] 导出环境变量
来源：http://www.share.fehbvm.com/Article/details/ghvkbuzwz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.hesvh.cn/Article/details/gzkxmyogc.sHtML

[R76] 使用临时文件
来源：http://www.share.fehbvm.com/Article/details/glsmnbjux.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fehbvm.com/Article/details/gdvkuhpfp.sHtML

[R77] 读取用户输入
来源：http://wap.fehbvm.com/Article/details/gyqndbmcd.sHtML


<!-- 参考信息 -->