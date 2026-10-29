代发 wailian999

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://read.share.hesvh.cn/Article/details/gszbphwby.sHtML

[Q26] 计数
来源：http://blog.zdbjq.cn/Article/details/gdqnfgpux.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.fehbvm.com/Article/details/gcjbvvuuf.sHtML

[Q27] 条件计数
来源：http://m.share.hesvh.cn/Article/details/gdwardeln.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gtohbxsya.sHtML

[Q28] 求和与平均
来源：http://3g.fehbvm.com/Article/details/gwnulsbkj.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gvspeidac.sHtML

[Q29] 最大最小值
来源：http://www.blog.zdbjq.cn/Article/details/gavqumvld.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gnowqjwbr.sHtML

[Q30] 分组统计
来源：http://www.share.hesvh.cn/Article/details/gkpcbcgdp.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.m.share.hesvh.cn/Article/details/gskkctxwy.sHtML

[Q31] 分组后过滤
来源：http://mobile.zdbjq.cn/Article/details/gbzermbze.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://mobile.zdbjq.cn/Article/details/ggqxvmini.sHtML

[Q32] 分组拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gqtneqslr.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gbpjfrivr.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.zdbjq.cn/Article/details/gfejmoxpe.sHtML

[Q33] 多列分组
来源：http://www.share.hesvh.cn/Article/details/gadoyyecz.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.fehbvm.com/Article/details/gzfgvqjxl.sHtML

[Q34] 每组取第一条
来源：http://www.m.share.zdbjq.cn/Article/details/gfvnecqjg.sHtML

SELECT * FROM (
来源：http://mobile.hesvh.cn/Article/details/gzobnzkey.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.hesvh.cn/Article/details/gcovcofnu.sHtML

) t WHERE rn = 1;
来源：http://3g.zdbjq.cn/Article/details/gsgulfxvp.sHtML

[Q35] 内连接
来源：http://mobile.fehbvm.com/Article/details/gwvwjpsxf.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.fehbvm.com/Article/details/gmawemrjr.sHtML

[Q36] 左连接
来源：http://blog.hesvh.cn/Article/details/gpqganulc.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.hesvh.cn/Article/details/gnhyrmxha.sHtML

[Q37] 右连接
来源：http://3g.fehbvm.com/Article/details/gikotvtma.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.zdbjq.cn/Article/details/gzxtkkvkb.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.fehbvm.com/Article/details/gudfvhpwy.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://3g.hesvh.cn/Article/details/gpaqkahrk.sHtML

[Q39] 自连接（查上下级）
来源：http://wap.hesvh.cn/Article/details/gohuychij.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.hesvh.cn/Article/details/ghtetssjx.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.zdbjq.cn/Article/details/guwfbwxpg.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.fehbvm.com/Article/details/gnigiqvrk.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.fehbvm.com/Article/details/gvreaquyg.sHtML

[Q41] 多表连接
来源：http://blog.fehbvm.com/Article/details/gotycrczm.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.fehbvm.com/Article/details/gjbljsdon.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.fehbvm.com/Article/details/glpjaxgdu.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.fehbvm.com/Article/details/gnoabjxsl.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gdwelzyyq.sHtML

SELECT u.name, o.amount FROM users u
来源：http://blog.fehbvm.com/Article/details/gvodmggmm.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.hesvh.cn/Article/details/glomgswoq.sHtML

[Q43] 标量子查询
来源：http://mobile.fehbvm.com/Article/details/gnhfhfpny.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.fehbvm.com/Article/details/gbsaewbxl.sHtML

[Q44] IN 子查询
来源：http://baike.zdbjq.cn/Article/details/gtlqdopxe.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://m.share.zdbjq.cn/Article/details/gwgiublnu.sHtML

[Q45] EXISTS 判断存在
来源：http://3g.zdbjq.cn/Article/details/gnmdpredw.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.hesvh.cn/Article/details/ggpprcnnk.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://mobile.zdbjq.cn/Article/details/gtxwvldqv.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.fehbvm.com/Article/details/gbmtgxymr.sHtML

[Q47] 与平均值比较
来源：http://3g.hesvh.cn/Article/details/gklycbhwn.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.zdbjq.cn/Article/details/gmhbemhap.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.fehbvm.com/Article/details/gkkdhnpzc.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.hesvh.cn/Article/details/gxyglntki.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.fehbvm.com/Article/details/gsedjvrxq.sHtML

[Q49] 更新单行
来源：http://www.m.share.zdbjq.cn/Article/details/geuoxzhbt.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.zdbjq.cn/Article/details/gnlidlhfu.sHtML

[Q50] 批量更新
来源：http://read.share.fehbvm.com/Article/details/ganiwbhug.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.hesvh.cn/Article/details/gdjkflgis.sHtML

[Q51] 用子查询更新
来源：http://www.blog.zdbjq.cn/Article/details/gtplxhawj.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://read.share.hesvh.cn/Article/details/gexgiihoz.sHtML

[Q52] 删除指定行
来源：http://www.m.share.fehbvm.com/Article/details/gqnodykyp.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.zdbjq.cn/Article/details/gqrenebvo.sHtML

[Q53] 按条件删除
来源：http://mobile.hesvh.cn/Article/details/gfcxgstlz.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.fehbvm.com/Article/details/gfuhlqepr.sHtML

[Q54] 清空表
来源：http://www.blog.fehbvm.com/Article/details/gtoudnlhg.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.hesvh.cn/Article/details/ghusphxlq.sHtML

[Q55] 排名（并列占位）
来源：http://wap.zdbjq.cn/Article/details/gopagddtq.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.fehbvm.com/Article/details/gqyxhyuvn.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.zdbjq.cn/Article/details/girhhvtxi.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.hesvh.cn/Article/details/gevkjilbk.sHtML

[Q57] 行号
来源：http://www.blog.fehbvm.com/Article/details/gkrfcncof.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.fehbvm.com/Article/details/goacsdsjp.sHtML

[Q58] 累计求和
来源：http://read.share.hesvh.cn/Article/details/gxrssmrlf.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.hesvh.cn/Article/details/gtasmzjqx.sHtML

[Q59] 分组内累计
来源：http://wap.fehbvm.com/Article/details/ghdsyhpyo.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gvsqxtbsr.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.zdbjq.cn/Article/details/gubqxxame.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.hesvh.cn/Article/details/gulgmdgjh.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gcuokkrqc.sHtML

[Q61] 移动平均
来源：http://www.share.fehbvm.com/Article/details/gxngxqtuq.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/ghukhzixw.sHtML

[Q62] 分组占比
来源：http://wap.hesvh.cn/Article/details/gtudgiddz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/goecnzzvz.sHtML

[Q63] 开启事务
来源：http://read.share.zdbjq.cn/Article/details/ggqjfdcmu.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.zdbjq.cn/Article/details/gppwkigmd.sHtML

[Q64] 提交事务
来源：http://blog.hesvh.cn/Article/details/gnwyxbzll.sHtML

COMMIT;
来源：http://3g.hesvh.cn/Article/details/gytfdjkjb.sHtML

[Q65] 回滚事务
来源：http://m.share.zdbjq.cn/Article/details/gttnvbnxf.sHtML

ROLLBACK;
来源：http://www.blog.hesvh.cn/Article/details/gpwcvfcoc.sHtML

[Q66] 行锁查询
来源：http://www.share.zdbjq.cn/Article/details/gkiejnbzq.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.zdbjq.cn/Article/details/gmsnmyoap.sHtML

[Q67] 设置隔离级别
来源：http://blog.zdbjq.cn/Article/details/gwoxcucgl.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.fehbvm.com/Article/details/gshzhmfig.sHtML

[Q68] 保存点
来源：http://www.share.zdbjq.cn/Article/details/gheqoeuel.sHtML

SAVEPOINT sp1;
来源：http://m.share.zdbjq.cn/Article/details/gmqsyqnfn.sHtML

ROLLBACK TO sp1;
来源：http://m.share.hesvh.cn/Article/details/gdxddsjbb.sHtML

[Q69] 查看执行计划
来源：http://baike.zdbjq.cn/Article/details/gjimkrszy.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fehbvm.com/Article/details/gcyrxkptr.sHtML

[Q70] 更新统计信息
来源：http://www.share.hesvh.cn/Article/details/gafdiyhls.sHtML

ANALYZE TABLE users;
来源：http://baike.fehbvm.com/Article/details/gjemnvibh.sHtML

[Q71] 查看建表语句
来源：http://read.share.hesvh.cn/Article/details/ggbinmtzb.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://blog.hesvh.cn/Article/details/gkiknlfjd.sHtML

[Q72] 查看索引
来源：http://www.share.zdbjq.cn/Article/details/gbablzseo.sHtML

SHOW INDEX FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gpdgjqkzv.sHtML

[Q73] 查看表状态
来源：http://m.share.hesvh.cn/Article/details/gcqznysaq.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://blog.fehbvm.com/Article/details/gozzrtriu.sHtML

[Q74] 强制使用索引
来源：http://www.blog.fehbvm.com/Article/details/gipxjyeim.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.hesvh.cn/Article/details/gmthkeimb.sHtML

[Q75] 日期格式化
来源：http://www.blog.fehbvm.com/Article/details/gbqbelfro.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gmlowdkot.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.fehbvm.com/Article/details/gbsltcakl.sHtML

[Q76] 按天统计
来源：http://www.m.share.fehbvm.com/Article/details/gclbvedji.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.fehbvm.com/Article/details/gpsolicym.sHtML

[Q77] 时间加减
来源：http://m.share.hesvh.cn/Article/details/gdjztvsyd.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://read.share.hesvh.cn/Article/details/gzblcrupf.sHtML

[Q78] 当前时间
来源：http://baike.zdbjq.cn/Article/details/gwkowaine.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.zdbjq.cn/Article/details/guzqcilen.sHtML

[Q79] 字符串拼接
来源：http://3g.hesvh.cn/Article/details/ghoxtipvy.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.zdbjq.cn/Article/details/gpzlopcuf.sHtML

[Q80] 字符串截取
来源：http://read.share.fehbvm.com/Article/details/gmmrbehgc.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gesnpvrfj.sHtML

[Q81] 字符串替换
来源：http://wap.hesvh.cn/Article/details/glebakwio.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/giskfuydw.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.zdbjq.cn/Article/details/gjynvecol.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.hesvh.cn/Article/details/gzrxmnbyg.sHtML

[Q83] 大小写转换
来源：http://read.share.hesvh.cn/Article/details/gnacnxzyd.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gdwjnxiyl.sHtML

[Q84] 去除首尾空格
来源：http://wap.fehbvm.com/Article/details/gsniuiipd.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/grtjvffsh.sHtML

[Q85] 数值取整
来源：http://mobile.hesvh.cn/Article/details/gezwuyqpy.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.zdbjq.cn/Article/details/gzwgmeght.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.zdbjq.cn/Article/details/gcijgcrfs.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.fehbvm.com/Article/details/gglodxdlc.sHtML

[Q87] JSON 字段做条件
来源：http://wap.zdbjq.cn/Article/details/gdaqmvqpg.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.fehbvm.com/Article/details/gjlkhpjkp.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.zdbjq.cn/Article/details/gfpvjyxqz.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.hesvh.cn/Article/details/grnycvxid.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gqzzgmaxg.sHtML

[Q89] 判断表是否存在
来源：http://3g.hesvh.cn/Article/details/gcpubuuvr.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://read.share.fehbvm.com/Article/details/guansqkqg.sHtML

[Q90] 生成序号列
来源：http://www.blog.zdbjq.cn/Article/details/gvxdpwixp.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.zdbjq.cn/Article/details/gftibvomv.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gtvoepnpw.sHtML

R. Bash 专题
来源：http://www.blog.zdbjq.cn/Article/details/grrihusbu.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/giwsifdfd.sHtML

[R01] shebang 与严格模式
来源：http://blog.fehbvm.com/Article/details/gksuquqlx.sHtML

#!/usr/bin/env bash
来源：http://wap.fehbvm.com/Article/details/gzwllevxw.sHtML

set -euo pipefail
来源：http://3g.hesvh.cn/Article/details/gebmsaduh.sHtML

[R02] 变量赋值与使用
来源：http://3g.fehbvm.com/Article/details/gqmvxrkuc.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.fehbvm.com/Article/details/gygxjiocc.sHtML

[R03] 只读变量
来源：http://www.share.zdbjq.cn/Article/details/gnloynidt.sHtML

readonly PI=3.14
来源：http://3g.fehbvm.com/Article/details/gtzazismk.sHtML

[R04] 位置参数
来源：http://baike.zdbjq.cn/Article/details/gfpeinmgj.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.fehbvm.com/Article/details/gckgcatcw.sHtML

[R05] 参数默认值
来源：http://www.share.hesvh.cn/Article/details/gwqahllyy.sHtML

name="${1:-default}"
来源：http://www.m.share.fehbvm.com/Article/details/gagabzith.sHtML

[R06] 判断命令是否存在
来源：http://m.share.fehbvm.com/Article/details/grpmeyaod.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fehbvm.com/Article/details/gsgpfdqbi.sHtML

[R07] if 判断文件
来源：http://wap.zdbjq.cn/Article/details/gkqqyccbu.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://read.share.fehbvm.com/Article/details/guxetnnvb.sHtML

[R08] 数值比较
来源：http://wap.fehbvm.com/Article/details/gnfkvabsa.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.fehbvm.com/Article/details/gwobngsbb.sHtML

[R09] 字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/gaksxsjzm.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.fehbvm.com/Article/details/geobzudmv.sHtML

[R10] 正则匹配
来源：http://read.share.fehbvm.com/Article/details/gcxunjrqf.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fehbvm.com/Article/details/geqhfvdop.sHtML

[R11] case 多分支
来源：http://www.m.share.hesvh.cn/Article/details/gfzjcwofp.sHtML

case "$1" in
来源：http://m.share.hesvh.cn/Article/details/gprijhunl.sHtML

start) echo "启动" ;;
来源：http://baike.zdbjq.cn/Article/details/gwqmcmfqm.sHtML

stop)  echo "停止" ;;
来源：http://baike.fehbvm.com/Article/details/gqemtowee.sHtML

*)     echo "未知命令" ;;
来源：http://read.share.zdbjq.cn/Article/details/gyccvtolh.sHtML

esac
来源：http://3g.zdbjq.cn/Article/details/gbnavrxnc.sHtML

[R12] for 遍历文件
来源：http://www.m.share.fehbvm.com/Article/details/gyoubavmj.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.hesvh.cn/Article/details/grrkqamfr.sHtML

[R13] for 计数循环
来源：http://www.m.share.hesvh.cn/Article/details/ggfykvstw.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://mobile.hesvh.cn/Article/details/glnmdovbr.sHtML

[R14] C 风格 for
来源：http://blog.zdbjq.cn/Article/details/gxasohwjo.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fehbvm.com/Article/details/guphrcnlz.sHtML

[R15] while 逐行读文件
来源：http://baike.fehbvm.com/Article/details/gxhyfnskp.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.zdbjq.cn/Article/details/gncnybygo.sHtML

[R16] until 等待条件
来源：http://www.share.zdbjq.cn/Article/details/gwjmqlngl.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fehbvm.com/Article/details/gvfwdvphl.sHtML

[R17] 数组定义与取值
来源：http://mobile.fehbvm.com/Article/details/ggabjprmr.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fehbvm.com/Article/details/gitfozfme.sHtML

[R18] 遍历数组
来源：http://blog.zdbjq.cn/Article/details/gtzdgelpx.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fehbvm.com/Article/details/gnqdrfaqr.sHtML

[R19] 数组长度
来源：http://www.share.hesvh.cn/Article/details/gnkvgnxjs.sHtML

echo "${#arr[@]}"
来源：http://mobile.fehbvm.com/Article/details/gzcglnpls.sHtML

[R20] 关联数组（字典）
来源：http://wap.hesvh.cn/Article/details/ghujyssgv.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.blog.fehbvm.com/Article/details/gctayomzb.sHtML

[R21] 字符串长度
来源：http://wap.hesvh.cn/Article/details/gbeblyddm.sHtML

echo "${#s}"
来源：http://read.share.zdbjq.cn/Article/details/gapyzkzbj.sHtML

[R22] 截取子串
来源：http://blog.hesvh.cn/Article/details/gxoidrvyd.sHtML

echo "${s:0:5}"
来源：http://www.m.share.zdbjq.cn/Article/details/gdnhoqgyb.sHtML

[R23] 字符串替换
来源：http://m.share.fehbvm.com/Article/details/gntzojhcv.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.blog.hesvh.cn/Article/details/gbyzdswby.sHtML

[R24] 大小写转换
来源：http://wap.fehbvm.com/Article/details/gmwrjbpvc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.zdbjq.cn/Article/details/gxhpfydxe.sHtML

[R25] 去后缀 / 去前缀
来源：http://wap.hesvh.cn/Article/details/gttgcjdro.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.zdbjq.cn/Article/details/gvvondqya.sHtML

[R26] 命令替换
来源：http://3g.hesvh.cn/Article/details/gursqjkdq.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.hesvh.cn/Article/details/gimfbkggv.sHtML

[R27] 算术展开
来源：http://www.blog.hesvh.cn/Article/details/gkcxkscme.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.hesvh.cn/Article/details/gsbeypdeo.sHtML

[R28] 浮点运算
来源：http://wap.fehbvm.com/Article/details/grwkighhn.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fehbvm.com/Article/details/gtgoqrtnu.sHtML

[R29] 定义函数
来源：http://3g.zdbjq.cn/Article/details/gyjpfcbsu.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.zdbjq.cn/Article/details/gkcmeizsy.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gfkxsnaeb.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.hesvh.cn/Article/details/gynqatqgm.sHtML

[R31] 局部变量
来源：http://read.share.fehbvm.com/Article/details/gaelcwxyo.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fehbvm.com/Article/details/gymyszbzi.sHtML

[R32] 参数个数校验
来源：http://blog.fehbvm.com/Article/details/gjnkbqypr.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.zdbjq.cn/Article/details/gaeepklir.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.hesvh.cn/Article/details/gpdchiwdn.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.hesvh.cn/Article/details/gxiinklrz.sHtML

[R34] 退出时清理
来源：http://m.share.fehbvm.com/Article/details/gmthwgtdt.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/gpndlbpwk.sHtML

[R35] 后台执行并等待
来源：http://wap.hesvh.cn/Article/details/ghzfsfwdl.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.hesvh.cn/Article/details/ghueuamcz.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.hesvh.cn/Article/details/gbuejiwzi.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.zdbjq.cn/Article/details/gbpepifds.sHtML

[R37] 把输出赋给变量
来源：http://blog.zdbjq.cn/Article/details/ghbpuusku.sHtML

files=$(ls -1)
来源：http://baike.fehbvm.com/Article/details/gudeqhpkp.sHtML

[R38] 管道串联
来源：http://www.blog.zdbjq.cn/Article/details/gubhartwx.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.zdbjq.cn/Article/details/gksigxxwf.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.fehbvm.com/Article/details/gsgzlitoq.sHtML

cmd > out.log 2>&1
来源：http://baike.hesvh.cn/Article/details/ghwlnnkrw.sHtML

[R40] 追加写日志
来源：http://3g.zdbjq.cn/Article/details/gcrygvobn.sHtML

echo "log" >> out.log
来源：http://read.share.zdbjq.cn/Article/details/ggiiherjj.sHtML

[R41] 丢弃输出
来源：http://baike.hesvh.cn/Article/details/gvmowczux.sHtML

cmd >/dev/null 2>&1
来源：http://3g.hesvh.cn/Article/details/gxcsvbhdl.sHtML

[R42] 输入重定向
来源：http://mobile.zdbjq.cn/Article/details/gibabckua.sHtML

wc -l < a.txt
来源：http://3g.fehbvm.com/Article/details/gtsclerzc.sHtML

[R43] 按名字查找文件
来源：http://www.share.hesvh.cn/Article/details/gzcxbfkle.sHtML

find . -name "*.log" -type f
来源：http://mobile.zdbjq.cn/Article/details/gwmfirdso.sHtML

[R44] 按修改时间查找
来源：http://mobile.zdbjq.cn/Article/details/ggwggnhja.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fehbvm.com/Article/details/grurmcqhi.sHtML

[R45] 批量删除
来源：http://mobile.hesvh.cn/Article/details/gwsjzilrx.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.fehbvm.com/Article/details/gwbyueqeo.sHtML

[R46] 递归替换文件内容
来源：http://baike.zdbjq.cn/Article/details/gosinfjxo.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.hesvh.cn/Article/details/gwqnpgpdu.sHtML

[R47] sed 单行替换
来源：http://read.share.fehbvm.com/Article/details/gmxhjvxnv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://wap.hesvh.cn/Article/details/ghqjayesy.sHtML

[R48] awk 取指定列
来源：http://www.blog.zdbjq.cn/Article/details/gsumjijvf.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gczhwxsvx.sHtML

[R49] awk 带条件
来源：http://read.share.hesvh.cn/Article/details/gpdtbblby.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fehbvm.com/Article/details/gtbewdvfq.sHtML

[R50] awk 求和
来源：http://baike.hesvh.cn/Article/details/gwptbjzmv.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.hesvh.cn/Article/details/gjtxtfija.sHtML

[R51] 排序去重取前几
来源：http://wap.fehbvm.com/Article/details/gelrbicba.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fehbvm.com/Article/details/goqiktuko.sHtML

[R52] 统计行数
来源：http://wap.fehbvm.com/Article/details/gsndobxgs.sHtML

wc -l a.txt
来源：http://blog.fehbvm.com/Article/details/gcerofjyj.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.hesvh.cn/Article/details/gcscpjqrp.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://3g.fehbvm.com/Article/details/ghqrvfqsm.sHtML

[R54] 比较两个文件
来源：http://read.share.zdbjq.cn/Article/details/gcslivhjf.sHtML

diff a.txt b.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gywzbdsim.sHtML

[R55] 压缩与解压
来源：http://read.share.zdbjq.cn/Article/details/gkeumogwt.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.zdbjq.cn/Article/details/guoaxpatq.sHtML

[R56] 远程拷贝
来源：http://www.share.fehbvm.com/Article/details/gsaiknznu.sHtML

scp file user@host:/path/
来源：http://baike.hesvh.cn/Article/details/gpiixxmvy.sHtML

[R57] 远程执行命令
来源：http://www.share.zdbjq.cn/Article/details/gzxzakgbr.sHtML

ssh user@host 'uptime'
来源：http://read.share.hesvh.cn/Article/details/gurhhloux.sHtML

[R58] 下载文件
来源：http://baike.zdbjq.cn/Article/details/gdaouxrxa.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.hesvh.cn/Article/details/gpdvlijfa.sHtML

[R59] 发 POST JSON
来源：http://m.share.fehbvm.com/Article/details/gaiqjwjbv.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.hesvh.cn/Article/details/giwcwiulu.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.zdbjq.cn/Article/details/gtvbkqevf.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.zdbjq.cn/Article/details/gpyctpgev.sHtML

[R61] 磁盘占用
来源：http://baike.fehbvm.com/Article/details/giqsgptqv.sHtML

df -h;  du -sh *
来源：http://www.blog.hesvh.cn/Article/details/gnhdfgfca.sHtML

[R62] 找最占空间的文件
来源：http://baike.hesvh.cn/Article/details/gbrzpdyyk.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fehbvm.com/Article/details/gfqfglizq.sHtML

[R63] 内存与进程
来源：http://read.share.fehbvm.com/Article/details/gdqrbxyqk.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.hesvh.cn/Article/details/gwkxmdusx.sHtML

[R64] 结束进程
来源：http://baike.zdbjq.cn/Article/details/grkwfiyfd.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.zdbjq.cn/Article/details/gmsfcqedl.sHtML

[R65] 查看端口占用
来源：http://baike.hesvh.cn/Article/details/gbedesviq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fehbvm.com/Article/details/gflzulfts.sHtML

[R66] 定时任务
来源：http://www.share.hesvh.cn/Article/details/gsuniqxgm.sHtML

crontab -e;  crontab -l
来源：http://3g.fehbvm.com/Article/details/gusgbmxwq.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.hesvh.cn/Article/details/gspfijbor.sHtML

openssl rand -hex 16
来源：http://m.share.zdbjq.cn/Article/details/gvauprjmb.sHtML

[R68] 计算文件校验值
来源：http://wap.zdbjq.cn/Article/details/ggnczojdr.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.hesvh.cn/Article/details/ghbwucfpj.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fehbvm.com/Article/details/gfqqcbblk.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fehbvm.com/Article/details/grofixsqo.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fehbvm.com/Article/details/gyxqypzps.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fehbvm.com/Article/details/guyqvemli.sHtML

[R71] 日期格式化
来源：http://baike.zdbjq.cn/Article/details/ginzsuhdl.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.hesvh.cn/Article/details/gmgxzhrty.sHtML

[R72] 等待端口就绪
来源：http://wap.hesvh.cn/Article/details/geqhgjfgp.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.hesvh.cn/Article/details/gzzylonat.sHtML

[R73] 分割大日志
来源：http://www.share.fehbvm.com/Article/details/gkwjkikwq.sHtML

split -l 1000 big.log part_
来源：http://read.share.zdbjq.cn/Article/details/giqcmwyum.sHtML

[R74] 批量重命名
来源：http://www.share.hesvh.cn/Article/details/gytrpthbm.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fehbvm.com/Article/details/gitgsadkn.sHtML

[R75] 导出环境变量
来源：http://baike.hesvh.cn/Article/details/gnwzqkjbf.sHtML


<!-- 参考信息 -->