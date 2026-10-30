代发 wailian999

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.m.share.fehbvm.com/Article/details/gjgljuayk.sHtML

[Q26] 计数
来源：http://www.blog.fehbvm.com/Article/details/gfzcnmiiq.sHtML

SELECT COUNT(*) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/geejiinaj.sHtML

[Q27] 条件计数
来源：http://www.blog.hesvh.cn/Article/details/ghghmwgep.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.share.fehbvm.com/Article/details/gonsamumu.sHtML

[Q28] 求和与平均
来源：http://blog.fehbvm.com/Article/details/gzdxqkneg.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.hesvh.cn/Article/details/gcipoqaih.sHtML

[Q29] 最大最小值
来源：http://www.m.share.fehbvm.com/Article/details/gmarxajly.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://m.share.fehbvm.com/Article/details/giaegangt.sHtML

[Q30] 分组统计
来源：http://www.m.share.zdbjq.cn/Article/details/gxpszulnz.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/goxctfrhp.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gkkjwdnqh.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.zdbjq.cn/Article/details/gpwhantcf.sHtML

[Q32] 分组拼接字符串
来源：http://wap.hesvh.cn/Article/details/guyaigrqu.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gublqbxfv.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.hesvh.cn/Article/details/gqbjzjuro.sHtML

[Q33] 多列分组
来源：http://baike.zdbjq.cn/Article/details/gzgyokoog.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.fehbvm.com/Article/details/gphkbeiev.sHtML

[Q34] 每组取第一条
来源：http://blog.zdbjq.cn/Article/details/goaodslgw.sHtML

SELECT * FROM (
来源：http://read.share.hesvh.cn/Article/details/glbjkbxmr.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://m.share.hesvh.cn/Article/details/gbdbslcat.sHtML

) t WHERE rn = 1;
来源：http://3g.hesvh.cn/Article/details/grzujlzyv.sHtML

[Q35] 内连接
来源：http://www.m.share.zdbjq.cn/Article/details/gtsylboaj.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.hesvh.cn/Article/details/gnljoxviv.sHtML

[Q36] 左连接
来源：http://www.m.share.fehbvm.com/Article/details/gorfcvpnq.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://baike.zdbjq.cn/Article/details/gfsnrvftx.sHtML

[Q37] 右连接
来源：http://mobile.fehbvm.com/Article/details/ghqmrofxd.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://read.share.fehbvm.com/Article/details/gksedtwhz.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.hesvh.cn/Article/details/gafdyqqmu.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://blog.hesvh.cn/Article/details/gjezhdfyl.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.zdbjq.cn/Article/details/gltdgbosn.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.zdbjq.cn/Article/details/genjenvau.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://m.share.zdbjq.cn/Article/details/gqxlyneks.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://3g.hesvh.cn/Article/details/gcrwkeicv.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.hesvh.cn/Article/details/gnalhbtuz.sHtML

[Q41] 多表连接
来源：http://wap.hesvh.cn/Article/details/geioovdcv.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.hesvh.cn/Article/details/gtuwbpqph.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.fehbvm.com/Article/details/gfaksapel.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://mobile.hesvh.cn/Article/details/gsebcvhgc.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.hesvh.cn/Article/details/gyqaemkag.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.zdbjq.cn/Article/details/gsrfqenkj.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://mobile.fehbvm.com/Article/details/gzybmtgoz.sHtML

[Q43] 标量子查询
来源：http://read.share.zdbjq.cn/Article/details/ggqzgklbg.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.hesvh.cn/Article/details/gvhzhfufx.sHtML

[Q44] IN 子查询
来源：http://blog.fehbvm.com/Article/details/gaejrvzkz.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.fehbvm.com/Article/details/gnbewvjkp.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.hesvh.cn/Article/details/glhlrqwzj.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.hesvh.cn/Article/details/gwrxadafy.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://m.share.fehbvm.com/Article/details/gbdckhfvm.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.zdbjq.cn/Article/details/gmhitfoiu.sHtML

[Q47] 与平均值比较
来源：http://www.blog.fehbvm.com/Article/details/gbcakfzkt.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.fehbvm.com/Article/details/gwxpqkeoc.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.hesvh.cn/Article/details/gljsoosts.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://mobile.fehbvm.com/Article/details/gnnauvypc.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.fehbvm.com/Article/details/gfoekyhlv.sHtML

[Q49] 更新单行
来源：http://wap.hesvh.cn/Article/details/gqfuliwkp.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://read.share.fehbvm.com/Article/details/gvvhtmhkc.sHtML

[Q50] 批量更新
来源：http://mobile.hesvh.cn/Article/details/gofjdiyfm.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://mobile.zdbjq.cn/Article/details/gpfhmygef.sHtML

[Q51] 用子查询更新
来源：http://3g.hesvh.cn/Article/details/geqjhlnmu.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://baike.fehbvm.com/Article/details/gmjvrgdmn.sHtML

[Q52] 删除指定行
来源：http://wap.fehbvm.com/Article/details/gjtonxhor.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.fehbvm.com/Article/details/gcjmrcfkv.sHtML

[Q53] 按条件删除
来源：http://www.share.hesvh.cn/Article/details/gcqxupmsu.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.hesvh.cn/Article/details/gmcjseygd.sHtML

[Q54] 清空表
来源：http://www.m.share.fehbvm.com/Article/details/gzjcfhdqh.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.fehbvm.com/Article/details/gpsgfgbvz.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.fehbvm.com/Article/details/gqewpkqvd.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.fehbvm.com/Article/details/ggryizzjy.sHtML

[Q56] 密集排名（并列不占位）
来源：http://read.share.zdbjq.cn/Article/details/gsavhibeq.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.zdbjq.cn/Article/details/gawxboayr.sHtML

[Q57] 行号
来源：http://3g.zdbjq.cn/Article/details/gzxpmooam.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.share.fehbvm.com/Article/details/gcncqhavu.sHtML

[Q58] 累计求和
来源：http://m.share.fehbvm.com/Article/details/glifgwpgw.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.fehbvm.com/Article/details/ggxqaappg.sHtML

[Q59] 分组内累计
来源：http://mobile.fehbvm.com/Article/details/gdfcglhbu.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://blog.fehbvm.com/Article/details/gsepndxij.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.zdbjq.cn/Article/details/gotrnjxih.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.fehbvm.com/Article/details/glswqdlnm.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gmmdcmkhv.sHtML

[Q61] 移动平均
来源：http://read.share.fehbvm.com/Article/details/gvuobemld.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gfxycrdgp.sHtML

[Q62] 分组占比
来源：http://m.share.hesvh.cn/Article/details/gshcwzsxu.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://baike.hesvh.cn/Article/details/gdwohuiyf.sHtML

[Q63] 开启事务
来源：http://www.m.share.fehbvm.com/Article/details/gjbzwaner.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.hesvh.cn/Article/details/gpumepftz.sHtML

[Q64] 提交事务
来源：http://mobile.zdbjq.cn/Article/details/gzfvmlymd.sHtML

COMMIT;
来源：http://read.share.hesvh.cn/Article/details/gefucmaya.sHtML

[Q65] 回滚事务
来源：http://read.share.fehbvm.com/Article/details/gftjfvumr.sHtML

ROLLBACK;
来源：http://www.share.fehbvm.com/Article/details/gpqfrclba.sHtML

[Q66] 行锁查询
来源：http://read.share.hesvh.cn/Article/details/gqsziedsf.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.m.share.zdbjq.cn/Article/details/getrxcxhn.sHtML

[Q67] 设置隔离级别
来源：http://wap.zdbjq.cn/Article/details/gawipbfhi.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.zdbjq.cn/Article/details/grqhwmufg.sHtML

[Q68] 保存点
来源：http://www.blog.fehbvm.com/Article/details/gibldscrm.sHtML

SAVEPOINT sp1;
来源：http://read.share.hesvh.cn/Article/details/gegzjiqrk.sHtML

ROLLBACK TO sp1;
来源：http://3g.hesvh.cn/Article/details/glubhjhgw.sHtML

[Q69] 查看执行计划
来源：http://read.share.zdbjq.cn/Article/details/gtsjpmpon.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://baike.zdbjq.cn/Article/details/gpoccvlqi.sHtML

[Q70] 更新统计信息
来源：http://www.m.share.hesvh.cn/Article/details/gohecgxnt.sHtML

ANALYZE TABLE users;
来源：http://wap.fehbvm.com/Article/details/gtaxgpfxj.sHtML

[Q71] 查看建表语句
来源：http://www.blog.fehbvm.com/Article/details/gytzmqfrn.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.fehbvm.com/Article/details/gjqftpwky.sHtML

[Q72] 查看索引
来源：http://3g.hesvh.cn/Article/details/gmyrflpvo.sHtML

SHOW INDEX FROM users;
来源：http://baike.zdbjq.cn/Article/details/gjpwzncmx.sHtML

[Q73] 查看表状态
来源：http://blog.zdbjq.cn/Article/details/gzpjfcqox.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://wap.fehbvm.com/Article/details/gbilfjajg.sHtML

[Q74] 强制使用索引
来源：http://www.share.hesvh.cn/Article/details/getykbuaq.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.hesvh.cn/Article/details/gnxmrjqxk.sHtML

[Q75] 日期格式化
来源：http://3g.hesvh.cn/Article/details/glonriwyl.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gmsvhcgxq.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.share.fehbvm.com/Article/details/gfsvboqmb.sHtML

[Q76] 按天统计
来源：http://blog.hesvh.cn/Article/details/greqkgehi.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://3g.zdbjq.cn/Article/details/gdrkvwtvn.sHtML

[Q77] 时间加减
来源：http://m.share.hesvh.cn/Article/details/gqffpuzjn.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.hesvh.cn/Article/details/gkisoabos.sHtML

[Q78] 当前时间
来源：http://www.blog.zdbjq.cn/Article/details/gwqjiscpy.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://read.share.zdbjq.cn/Article/details/gonkobwgl.sHtML

[Q79] 字符串拼接
来源：http://blog.hesvh.cn/Article/details/gbgeuheoq.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://read.share.zdbjq.cn/Article/details/gynzpozhn.sHtML

[Q80] 字符串截取
来源：http://m.share.hesvh.cn/Article/details/gcrruxqpk.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.fehbvm.com/Article/details/gsevbioaj.sHtML

[Q81] 字符串替换
来源：http://www.m.share.zdbjq.cn/Article/details/gcxrioxvu.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gmxfnffhi.sHtML

[Q82] 字符长度与字节长度
来源：http://mobile.hesvh.cn/Article/details/gztzjukjs.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/gkggltcee.sHtML

[Q83] 大小写转换
来源：http://blog.zdbjq.cn/Article/details/gmoufjyin.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gtrbobzoc.sHtML

[Q84] 去除首尾空格
来源：http://m.share.fehbvm.com/Article/details/gyhtkffqx.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gvtygnuap.sHtML

[Q85] 数值取整
来源：http://blog.zdbjq.cn/Article/details/gwfkqlugn.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.hesvh.cn/Article/details/gszhreyuj.sHtML

[Q86] 读取 JSON 字段
来源：http://3g.zdbjq.cn/Article/details/gvmegwdhy.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.zdbjq.cn/Article/details/gcqzoamcl.sHtML

[Q87] JSON 字段做条件
来源：http://baike.zdbjq.cn/Article/details/guknurovf.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://m.share.fehbvm.com/Article/details/gbqmjvhoc.sHtML

[Q88] 行转列（条件聚合）
来源：http://blog.hesvh.cn/Article/details/gapjizunv.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.blog.zdbjq.cn/Article/details/ghiogvkja.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fehbvm.com/Article/details/guwubzmcl.sHtML

[Q89] 判断表是否存在
来源：http://3g.hesvh.cn/Article/details/gvtlwkdcy.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.zdbjq.cn/Article/details/gasabuagh.sHtML

[Q90] 生成序号列
来源：http://blog.zdbjq.cn/Article/details/ghqvmdpxd.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.zdbjq.cn/Article/details/gzlwvucuh.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/ggdixulqv.sHtML

R. Bash 专题
来源：http://blog.hesvh.cn/Article/details/gellyberz.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gylkdfrqh.sHtML

[R01] shebang 与严格模式
来源：http://wap.fehbvm.com/Article/details/gbbvwpgjq.sHtML

#!/usr/bin/env bash
来源：http://3g.hesvh.cn/Article/details/ghhnqljok.sHtML

set -euo pipefail
来源：http://wap.fehbvm.com/Article/details/ghfveiowb.sHtML

[R02] 变量赋值与使用
来源：http://m.share.zdbjq.cn/Article/details/gxjmokggs.sHtML

name="Tom"; echo "$name"
来源：http://3g.zdbjq.cn/Article/details/guuwvrxha.sHtML

[R03] 只读变量
来源：http://wap.fehbvm.com/Article/details/geexkmkom.sHtML

readonly PI=3.14
来源：http://read.share.fehbvm.com/Article/details/gpinyqeon.sHtML

[R04] 位置参数
来源：http://mobile.zdbjq.cn/Article/details/guaveepjm.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://mobile.fehbvm.com/Article/details/gcuzjrrif.sHtML

[R05] 参数默认值
来源：http://www.m.share.fehbvm.com/Article/details/gpxnkhsex.sHtML

name="${1:-default}"
来源：http://m.share.hesvh.cn/Article/details/gjrrujefz.sHtML

[R06] 判断命令是否存在
来源：http://read.share.hesvh.cn/Article/details/gbxrngljs.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.zdbjq.cn/Article/details/gshgecvsg.sHtML

[R07] if 判断文件
来源：http://read.share.hesvh.cn/Article/details/gglcbuyge.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.hesvh.cn/Article/details/gdqjgybko.sHtML

[R08] 数值比较
来源：http://baike.fehbvm.com/Article/details/gbwryyksh.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.zdbjq.cn/Article/details/glxvycdnn.sHtML

[R09] 字符串比较
来源：http://www.blog.fehbvm.com/Article/details/gkrsbzrbb.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fehbvm.com/Article/details/gdwonjpur.sHtML

[R10] 正则匹配
来源：http://www.m.share.hesvh.cn/Article/details/ggulclpou.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.zdbjq.cn/Article/details/gmifnbiwb.sHtML

[R11] case 多分支
来源：http://mobile.hesvh.cn/Article/details/gmauwdlyf.sHtML

case "$1" in
来源：http://m.share.zdbjq.cn/Article/details/ghsinwwui.sHtML

start) echo "启动" ;;
来源：http://wap.zdbjq.cn/Article/details/guuwdpaib.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fehbvm.com/Article/details/gapgxgtwf.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.hesvh.cn/Article/details/gwcuokpct.sHtML

esac
来源：http://mobile.hesvh.cn/Article/details/gzhqqhkjq.sHtML

[R12] for 遍历文件
来源：http://blog.hesvh.cn/Article/details/gnmaqjiza.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.fehbvm.com/Article/details/gtgadlzxr.sHtML

[R13] for 计数循环
来源：http://www.m.share.hesvh.cn/Article/details/gbxymhbui.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.hesvh.cn/Article/details/gpoxfknvi.sHtML

[R14] C 风格 for
来源：http://wap.fehbvm.com/Article/details/gowwmddop.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.zdbjq.cn/Article/details/gpgsrszpi.sHtML

[R15] while 逐行读文件
来源：http://3g.hesvh.cn/Article/details/gczpjvqge.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.zdbjq.cn/Article/details/gvazrlgop.sHtML

[R16] until 等待条件
来源：http://baike.fehbvm.com/Article/details/gwcchtulo.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/gbzqnapsk.sHtML

[R17] 数组定义与取值
来源：http://blog.zdbjq.cn/Article/details/gfdrtcole.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.zdbjq.cn/Article/details/gqsvhqpmu.sHtML

[R18] 遍历数组
来源：http://www.share.hesvh.cn/Article/details/gzdccoomg.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.zdbjq.cn/Article/details/gxaoixwtg.sHtML

[R19] 数组长度
来源：http://read.share.fehbvm.com/Article/details/giskwqxsw.sHtML

echo "${#arr[@]}"
来源：http://www.blog.hesvh.cn/Article/details/gmrcletgm.sHtML

[R20] 关联数组（字典）
来源：http://www.share.hesvh.cn/Article/details/gnmhqstos.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fehbvm.com/Article/details/glhamerbg.sHtML

[R21] 字符串长度
来源：http://www.share.hesvh.cn/Article/details/guzhaiieo.sHtML

echo "${#s}"
来源：http://mobile.zdbjq.cn/Article/details/gzegmhxby.sHtML

[R22] 截取子串
来源：http://mobile.hesvh.cn/Article/details/gsnkowaqr.sHtML

echo "${s:0:5}"
来源：http://baike.fehbvm.com/Article/details/ggkrzdhde.sHtML

[R23] 字符串替换
来源：http://mobile.hesvh.cn/Article/details/gzaykuhsv.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://blog.zdbjq.cn/Article/details/gccblrgno.sHtML

[R24] 大小写转换
来源：http://m.share.zdbjq.cn/Article/details/grtenbfoo.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.hesvh.cn/Article/details/gshzcrefc.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.zdbjq.cn/Article/details/gmnpihxuq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fehbvm.com/Article/details/gvfhfrkyx.sHtML

[R26] 命令替换
来源：http://baike.fehbvm.com/Article/details/ghgjppoeo.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.zdbjq.cn/Article/details/gzbzlmcsj.sHtML

[R27] 算术展开
来源：http://m.share.hesvh.cn/Article/details/gqctwmktt.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.zdbjq.cn/Article/details/gxgnoaggw.sHtML

[R28] 浮点运算
来源：http://read.share.hesvh.cn/Article/details/glyhsbzxq.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.hesvh.cn/Article/details/gdrmigcvg.sHtML

[R29] 定义函数
来源：http://www.share.zdbjq.cn/Article/details/gmmwzjsjg.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fehbvm.com/Article/details/gqtyortko.sHtML

[R30] 函数返回状态码
来源：http://m.share.hesvh.cn/Article/details/gryvthgww.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.zdbjq.cn/Article/details/gzkgagkol.sHtML

[R31] 局部变量
来源：http://www.blog.fehbvm.com/Article/details/grsgemviy.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fehbvm.com/Article/details/gvigmwdsi.sHtML

[R32] 参数个数校验
来源：http://www.share.fehbvm.com/Article/details/gjizrauzq.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/gosqgvfvi.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.zdbjq.cn/Article/details/gicvkpeyz.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fehbvm.com/Article/details/gbrijjhcx.sHtML

[R34] 退出时清理
来源：http://read.share.zdbjq.cn/Article/details/gahpsacrv.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.zdbjq.cn/Article/details/gqiumenod.sHtML

[R35] 后台执行并等待
来源：http://blog.zdbjq.cn/Article/details/gccnxhgvy.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.hesvh.cn/Article/details/gbszwmcpb.sHtML

[R36] 并发执行多个任务
来源：http://3g.fehbvm.com/Article/details/gqweafxhi.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fehbvm.com/Article/details/gfwuoqpzz.sHtML

[R37] 把输出赋给变量
来源：http://read.share.hesvh.cn/Article/details/gafvzlrhe.sHtML

files=$(ls -1)
来源：http://m.share.zdbjq.cn/Article/details/genilsanv.sHtML

[R38] 管道串联
来源：http://wap.fehbvm.com/Article/details/gfvxjafbl.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fehbvm.com/Article/details/gbwvvgmfd.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fehbvm.com/Article/details/gnoamepvw.sHtML

cmd > out.log 2>&1
来源：http://3g.zdbjq.cn/Article/details/gabehzmya.sHtML

[R40] 追加写日志
来源：http://3g.zdbjq.cn/Article/details/gbfmooubc.sHtML

echo "log" >> out.log
来源：http://blog.zdbjq.cn/Article/details/gkyyrxhhy.sHtML

[R41] 丢弃输出
来源：http://baike.fehbvm.com/Article/details/gmjlhghtl.sHtML

cmd >/dev/null 2>&1
来源：http://3g.zdbjq.cn/Article/details/gdknidenp.sHtML

[R42] 输入重定向
来源：http://www.m.share.zdbjq.cn/Article/details/gfuqmdsqf.sHtML

wc -l < a.txt
来源：http://wap.zdbjq.cn/Article/details/giukwtikm.sHtML

[R43] 按名字查找文件
来源：http://www.share.zdbjq.cn/Article/details/genhbzlwt.sHtML

find . -name "*.log" -type f
来源：http://blog.zdbjq.cn/Article/details/gfvmkczfk.sHtML

[R44] 按修改时间查找
来源：http://3g.hesvh.cn/Article/details/gsynglpzd.sHtML

find . -mtime -7 -type f
来源：http://www.blog.fehbvm.com/Article/details/gessnzaic.sHtML

[R45] 批量删除
来源：http://baike.fehbvm.com/Article/details/grbfojzrb.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fehbvm.com/Article/details/gzhzdvtlq.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fehbvm.com/Article/details/gnxoxuris.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.zdbjq.cn/Article/details/gralocmyo.sHtML

[R47] sed 单行替换
来源：http://mobile.hesvh.cn/Article/details/gbgbjbgqr.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.fehbvm.com/Article/details/gqvixdbqn.sHtML

[R48] awk 取指定列
来源：http://mobile.zdbjq.cn/Article/details/ggorpwnvh.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fehbvm.com/Article/details/gsqugusoj.sHtML

[R49] awk 带条件
来源：http://blog.zdbjq.cn/Article/details/gxbftxnzz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.hesvh.cn/Article/details/gfuokdztv.sHtML

[R50] awk 求和
来源：http://blog.hesvh.cn/Article/details/grfdaveis.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.zdbjq.cn/Article/details/gsuvglfkw.sHtML

[R51] 排序去重取前几
来源：http://m.share.zdbjq.cn/Article/details/gbyllebha.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fehbvm.com/Article/details/gzhgzfqbs.sHtML

[R52] 统计行数
来源：http://mobile.zdbjq.cn/Article/details/gftecmohr.sHtML

wc -l a.txt
来源：http://read.share.fehbvm.com/Article/details/glfvkikbe.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.hesvh.cn/Article/details/glteqokaz.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.zdbjq.cn/Article/details/gfymzzrbp.sHtML

[R54] 比较两个文件
来源：http://m.share.hesvh.cn/Article/details/glabsjmog.sHtML

diff a.txt b.txt
来源：http://www.share.fehbvm.com/Article/details/gigdeaqal.sHtML

[R55] 压缩与解压
来源：http://wap.hesvh.cn/Article/details/gtalsahmc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.hesvh.cn/Article/details/gwmmnbkkh.sHtML

[R56] 远程拷贝
来源：http://3g.hesvh.cn/Article/details/ggqjrvcix.sHtML

scp file user@host:/path/
来源：http://mobile.zdbjq.cn/Article/details/gpcgjwtrb.sHtML

[R57] 远程执行命令
来源：http://mobile.hesvh.cn/Article/details/govtzqeya.sHtML

ssh user@host 'uptime'
来源：http://3g.hesvh.cn/Article/details/gouerbbjt.sHtML

[R58] 下载文件
来源：http://www.blog.zdbjq.cn/Article/details/gixmxdfym.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fehbvm.com/Article/details/gdqxjdsdz.sHtML

[R59] 发 POST JSON
来源：http://3g.zdbjq.cn/Article/details/gecswldhf.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.zdbjq.cn/Article/details/gubfebuld.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.hesvh.cn/Article/details/gurjlighx.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.zdbjq.cn/Article/details/gqomzkzre.sHtML

[R61] 磁盘占用
来源：http://mobile.hesvh.cn/Article/details/gqafpefvy.sHtML

df -h;  du -sh *
来源：http://www.m.share.hesvh.cn/Article/details/goevyhvio.sHtML

[R62] 找最占空间的文件
来源：http://www.share.hesvh.cn/Article/details/gmiwdugdo.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.hesvh.cn/Article/details/gwpiljysj.sHtML

[R63] 内存与进程
来源：http://blog.hesvh.cn/Article/details/gcqimfvir.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fehbvm.com/Article/details/gegvpcrft.sHtML

[R64] 结束进程
来源：http://www.blog.fehbvm.com/Article/details/gseolttnf.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fehbvm.com/Article/details/getiwvmlk.sHtML

[R65] 查看端口占用
来源：http://baike.hesvh.cn/Article/details/gxlhkjkhj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fehbvm.com/Article/details/gkkdvgbqc.sHtML

[R66] 定时任务
来源：http://wap.zdbjq.cn/Article/details/grgoemlmc.sHtML

crontab -e;  crontab -l
来源：http://baike.zdbjq.cn/Article/details/gndedqilt.sHtML

[R67] 生成随机十六进制串
来源：http://3g.zdbjq.cn/Article/details/gzmnpjcuc.sHtML

openssl rand -hex 16
来源：http://baike.fehbvm.com/Article/details/gqtvhkyai.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.zdbjq.cn/Article/details/gazgaavqc.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.hesvh.cn/Article/details/gpprmnikr.sHtML

[R69] 生成随机密码
来源：http://wap.fehbvm.com/Article/details/gakpwdxrj.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fehbvm.com/Article/details/gqhtoprii.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fehbvm.com/Article/details/ggozzgsey.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.hesvh.cn/Article/details/gxfqackqa.sHtML

[R71] 日期格式化
来源：http://read.share.hesvh.cn/Article/details/gkiupinid.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fehbvm.com/Article/details/gsrmeikut.sHtML

[R72] 等待端口就绪
来源：http://blog.fehbvm.com/Article/details/gejvejlgw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.zdbjq.cn/Article/details/gywdvsean.sHtML

[R73] 分割大日志
来源：http://blog.fehbvm.com/Article/details/goywbkdnz.sHtML

split -l 1000 big.log part_
来源：http://m.share.fehbvm.com/Article/details/gjnpnfosc.sHtML

[R74] 批量重命名
来源：http://mobile.fehbvm.com/Article/details/gudxpjdht.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.hesvh.cn/Article/details/geiwjegyx.sHtML

[R75] 导出环境变量
来源：http://m.share.zdbjq.cn/Article/details/gegoyprpb.sHtML


<!-- 参考信息 -->