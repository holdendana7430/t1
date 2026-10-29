代发 wailian999

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://3g.fehbvm.com/Article/details/gykwlugrb.sHtML

[Q24] 去重
来源：http://wap.zdbjq.cn/Article/details/goswacjqc.sHtML

SELECT DISTINCT city FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gtyfdevid.sHtML

[Q25] 只取前 N 条
来源：http://www.m.share.fehbvm.com/Article/details/gtqvdvzgv.sHtML

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://wap.hesvh.cn/Article/details/gcnjnfhln.sHtML

[Q26] 计数
来源：http://read.share.zdbjq.cn/Article/details/gsieghtco.sHtML

SELECT COUNT(*) FROM users;
来源：http://3g.hesvh.cn/Article/details/gpqxhhoqo.sHtML

[Q27] 条件计数
来源：http://baike.hesvh.cn/Article/details/gojbnbala.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gomkzoxfm.sHtML

[Q28] 求和与平均
来源：http://mobile.hesvh.cn/Article/details/ghgoyhoud.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gtuucqnpa.sHtML

[Q29] 最大最小值
来源：http://m.share.fehbvm.com/Article/details/gfgoadjgb.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://3g.hesvh.cn/Article/details/gvdfconmx.sHtML

[Q30] 分组统计
来源：http://wap.fehbvm.com/Article/details/gbmjcuunz.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gkyxcuara.sHtML

[Q31] 分组后过滤
来源：http://www.m.share.fehbvm.com/Article/details/gzrwpfzyw.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.hesvh.cn/Article/details/gefgcxmnr.sHtML

[Q32] 分组拼接字符串
来源：http://baike.fehbvm.com/Article/details/ggkynhzxo.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://3g.fehbvm.com/Article/details/gfsrvqyjr.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://m.share.hesvh.cn/Article/details/gobsxvxpz.sHtML

[Q33] 多列分组
来源：http://www.m.share.fehbvm.com/Article/details/gowladgbe.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://mobile.hesvh.cn/Article/details/gjcpqrpxz.sHtML

[Q34] 每组取第一条
来源：http://www.blog.hesvh.cn/Article/details/giheokvoz.sHtML

SELECT * FROM (
来源：http://www.m.share.hesvh.cn/Article/details/gcbzxymnf.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://baike.hesvh.cn/Article/details/gzfzrvijk.sHtML

) t WHERE rn = 1;
来源：http://mobile.zdbjq.cn/Article/details/glqmkvvrk.sHtML

[Q35] 内连接
来源：http://blog.zdbjq.cn/Article/details/gxhkadekn.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://baike.fehbvm.com/Article/details/goswnoriq.sHtML

[Q36] 左连接
来源：http://www.m.share.fehbvm.com/Article/details/gvuwasmqb.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.blog.zdbjq.cn/Article/details/gumqzcmzf.sHtML

[Q37] 右连接
来源：http://www.blog.hesvh.cn/Article/details/gheemganh.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.fehbvm.com/Article/details/gnkgaslav.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.hesvh.cn/Article/details/gflegjkfc.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.fehbvm.com/Article/details/gqlgyiovf.sHtML

[Q39] 自连接（查上下级）
来源：http://3g.hesvh.cn/Article/details/gcqqbucdo.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://wap.zdbjq.cn/Article/details/gntdiglws.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.hesvh.cn/Article/details/gztsdovyw.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.fehbvm.com/Article/details/gzhlmhmez.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.zdbjq.cn/Article/details/gqpcbjbdi.sHtML

[Q41] 多表连接
来源：http://3g.hesvh.cn/Article/details/gwqmyedfv.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.zdbjq.cn/Article/details/gemmbncig.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.blog.zdbjq.cn/Article/details/gvtibrdis.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.hesvh.cn/Article/details/gdczuqdgr.sHtML

[Q42] 连接条件附加过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gyqmawxjj.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.blog.zdbjq.cn/Article/details/gpgufwmnd.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.hesvh.cn/Article/details/gculwgnyf.sHtML

[Q43] 标量子查询
来源：http://m.share.fehbvm.com/Article/details/gwtzhkhmw.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.hesvh.cn/Article/details/gfhdclorg.sHtML

[Q44] IN 子查询
来源：http://www.share.hesvh.cn/Article/details/gjfqlrgyw.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.fehbvm.com/Article/details/gtunafpfl.sHtML

[Q45] EXISTS 判断存在
来源：http://m.share.hesvh.cn/Article/details/gzitgeows.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.zdbjq.cn/Article/details/gnnhxybzj.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.fehbvm.com/Article/details/gonmnndlb.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://baike.fehbvm.com/Article/details/ghyoscpel.sHtML

[Q47] 与平均值比较
来源：http://3g.fehbvm.com/Article/details/gyrtydaic.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://wap.fehbvm.com/Article/details/gchijceax.sHtML

[Q48] CTE 公用表表达式
来源：http://www.m.share.fehbvm.com/Article/details/gugquhrvq.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://read.share.fehbvm.com/Article/details/gskqihnhq.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.zdbjq.cn/Article/details/gdxmivnjj.sHtML

[Q49] 更新单行
来源：http://read.share.fehbvm.com/Article/details/gjrkvsglf.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.fehbvm.com/Article/details/gqzbcfean.sHtML

[Q50] 批量更新
来源：http://www.blog.fehbvm.com/Article/details/gktlkonju.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://baike.fehbvm.com/Article/details/gudyyplad.sHtML

[Q51] 用子查询更新
来源：http://baike.hesvh.cn/Article/details/gmztpzepq.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.fehbvm.com/Article/details/ghldcvafh.sHtML

[Q52] 删除指定行
来源：http://m.share.hesvh.cn/Article/details/gwekoyxvo.sHtML

DELETE FROM users WHERE id = 10;
来源：http://blog.fehbvm.com/Article/details/guzzeqnbo.sHtML

[Q53] 按条件删除
来源：http://www.m.share.fehbvm.com/Article/details/gmuqnzwdn.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.hesvh.cn/Article/details/gvzqdossn.sHtML

[Q54] 清空表
来源：http://mobile.zdbjq.cn/Article/details/gjzawtrve.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fehbvm.com/Article/details/guiehqazw.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.fehbvm.com/Article/details/goosrbkvk.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.hesvh.cn/Article/details/gairwbgcl.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.fehbvm.com/Article/details/gjfhrpamc.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://mobile.fehbvm.com/Article/details/glomzacav.sHtML

[Q57] 行号
来源：http://www.blog.zdbjq.cn/Article/details/ggdczexzp.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://baike.fehbvm.com/Article/details/gorsiznnj.sHtML

[Q58] 累计求和
来源：http://www.blog.zdbjq.cn/Article/details/gtujlmmsl.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gsgghjaep.sHtML

[Q59] 分组内累计
来源：http://www.share.zdbjq.cn/Article/details/ggcckdbcs.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gwdjdbefs.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.zdbjq.cn/Article/details/gwkgoiyut.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.fehbvm.com/Article/details/gunhmebox.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gddpfwcah.sHtML

[Q61] 移动平均
来源：http://baike.hesvh.cn/Article/details/gugzpvdun.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gtvkzpxxj.sHtML

[Q62] 分组占比
来源：http://mobile.hesvh.cn/Article/details/gjokwbchp.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/gnigpoppj.sHtML

[Q63] 开启事务
来源：http://blog.zdbjq.cn/Article/details/gzbofayvb.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://mobile.hesvh.cn/Article/details/gxwhngbpv.sHtML

[Q64] 提交事务
来源：http://www.blog.hesvh.cn/Article/details/gdbunkptd.sHtML

COMMIT;
来源：http://www.blog.fehbvm.com/Article/details/gcfmsnroi.sHtML

[Q65] 回滚事务
来源：http://www.share.hesvh.cn/Article/details/gysyolbin.sHtML

ROLLBACK;
来源：http://mobile.fehbvm.com/Article/details/gmfrpoefi.sHtML

[Q66] 行锁查询
来源：http://read.share.hesvh.cn/Article/details/gorjrwwnr.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.fehbvm.com/Article/details/gdlgrdszw.sHtML

[Q67] 设置隔离级别
来源：http://www.m.share.hesvh.cn/Article/details/gbqsjluqn.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.zdbjq.cn/Article/details/gfjgpbljj.sHtML

[Q68] 保存点
来源：http://3g.zdbjq.cn/Article/details/gcxghkctk.sHtML

SAVEPOINT sp1;
来源：http://www.share.hesvh.cn/Article/details/gnfqfoftp.sHtML

ROLLBACK TO sp1;
来源：http://baike.hesvh.cn/Article/details/gcsvdbcfy.sHtML

[Q69] 查看执行计划
来源：http://mobile.fehbvm.com/Article/details/gssbqbxbm.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.hesvh.cn/Article/details/gfohmfnoj.sHtML

[Q70] 更新统计信息
来源：http://3g.hesvh.cn/Article/details/gzxvblcpl.sHtML

ANALYZE TABLE users;
来源：http://blog.fehbvm.com/Article/details/gvyfoljeq.sHtML

[Q71] 查看建表语句
来源：http://read.share.fehbvm.com/Article/details/grlowpeai.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://wap.hesvh.cn/Article/details/grhphafct.sHtML

[Q72] 查看索引
来源：http://baike.fehbvm.com/Article/details/gjacbaihz.sHtML

SHOW INDEX FROM users;
来源：http://blog.fehbvm.com/Article/details/gtgttdgro.sHtML

[Q73] 查看表状态
来源：http://blog.zdbjq.cn/Article/details/gfiumoaof.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.blog.zdbjq.cn/Article/details/gqevspkqd.sHtML

[Q74] 强制使用索引
来源：http://m.share.fehbvm.com/Article/details/gwqzfnamt.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.hesvh.cn/Article/details/gmivltayb.sHtML

[Q75] 日期格式化
来源：http://wap.hesvh.cn/Article/details/geoedkmtp.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gifyjkhtn.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.zdbjq.cn/Article/details/gqnzxoikx.sHtML

[Q76] 按天统计
来源：http://baike.zdbjq.cn/Article/details/gewytctqq.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.fehbvm.com/Article/details/gygthhxfr.sHtML

[Q77] 时间加减
来源：http://read.share.zdbjq.cn/Article/details/gybsyqvxk.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.share.fehbvm.com/Article/details/gbckubpaa.sHtML

[Q78] 当前时间
来源：http://baike.zdbjq.cn/Article/details/gchcgzwkc.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.hesvh.cn/Article/details/gdwjguebl.sHtML

[Q79] 字符串拼接
来源：http://blog.fehbvm.com/Article/details/grfdcmfvp.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.zdbjq.cn/Article/details/gkyndlvab.sHtML

[Q80] 字符串截取
来源：http://baike.zdbjq.cn/Article/details/grmnvkxaq.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gcmqtgomx.sHtML

[Q81] 字符串替换
来源：http://www.share.hesvh.cn/Article/details/grabpdupv.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gjqfejcig.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.fehbvm.com/Article/details/gwnysqyyk.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/getthxcab.sHtML

[Q83] 大小写转换
来源：http://m.share.hesvh.cn/Article/details/gcgcbqrzv.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gbqfpafho.sHtML

[Q84] 去除首尾空格
来源：http://read.share.fehbvm.com/Article/details/gzujvmvvh.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.hesvh.cn/Article/details/gdtrmafpc.sHtML

[Q85] 数值取整
来源：http://3g.hesvh.cn/Article/details/gcyoficzl.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.blog.fehbvm.com/Article/details/ghficsvyr.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.fehbvm.com/Article/details/ggveedmba.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.zdbjq.cn/Article/details/gpcntevhq.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fehbvm.com/Article/details/gpivnwcvv.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fehbvm.com/Article/details/gsoxyxtva.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fehbvm.com/Article/details/gvqoeuvdl.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.hesvh.cn/Article/details/gdafzjhqi.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.hesvh.cn/Article/details/gxiidmpdz.sHtML

[Q89] 判断表是否存在
来源：http://www.share.zdbjq.cn/Article/details/gbgyyhyjt.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://mobile.zdbjq.cn/Article/details/gnxwelwuh.sHtML

[Q90] 生成序号列
来源：http://wap.zdbjq.cn/Article/details/gbjsqpfcp.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://wap.zdbjq.cn/Article/details/ggtppmsrp.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/golivjlag.sHtML

R. Bash 专题
来源：http://mobile.zdbjq.cn/Article/details/gsfbyaqdp.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gzffzsmym.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.hesvh.cn/Article/details/goksxyiiq.sHtML

#!/usr/bin/env bash
来源：http://www.blog.fehbvm.com/Article/details/gmxjjhorm.sHtML

set -euo pipefail
来源：http://mobile.fehbvm.com/Article/details/gtdcbtcno.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.zdbjq.cn/Article/details/gkbpidikt.sHtML

name="Tom"; echo "$name"
来源：http://blog.fehbvm.com/Article/details/gciwldanr.sHtML

[R03] 只读变量
来源：http://3g.hesvh.cn/Article/details/gelnchlgz.sHtML

readonly PI=3.14
来源：http://www.blog.hesvh.cn/Article/details/gjkufgdem.sHtML

[R04] 位置参数
来源：http://www.blog.hesvh.cn/Article/details/gdikfbupb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.fehbvm.com/Article/details/gcjfxttlr.sHtML

[R05] 参数默认值
来源：http://blog.fehbvm.com/Article/details/gfqnqwxna.sHtML

name="${1:-default}"
来源：http://m.share.hesvh.cn/Article/details/ghekyvuyw.sHtML

[R06] 判断命令是否存在
来源：http://m.share.fehbvm.com/Article/details/gjwauezkd.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.hesvh.cn/Article/details/glivqgvqf.sHtML

[R07] if 判断文件
来源：http://wap.fehbvm.com/Article/details/gbvgpevec.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fehbvm.com/Article/details/gvvlnrdzb.sHtML

[R08] 数值比较
来源：http://www.m.share.fehbvm.com/Article/details/gzxhizygz.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://blog.zdbjq.cn/Article/details/goyqjduml.sHtML

[R09] 字符串比较
来源：http://www.share.fehbvm.com/Article/details/gbxagacdb.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.fehbvm.com/Article/details/goihkagbd.sHtML

[R10] 正则匹配
来源：http://read.share.zdbjq.cn/Article/details/ghpawmlfi.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fehbvm.com/Article/details/goyecxkor.sHtML

[R11] case 多分支
来源：http://www.m.share.zdbjq.cn/Article/details/ghlletrnu.sHtML

case "$1" in
来源：http://mobile.hesvh.cn/Article/details/gfjxabgqd.sHtML

start) echo "启动" ;;
来源：http://wap.zdbjq.cn/Article/details/gzzihvafl.sHtML

stop)  echo "停止" ;;
来源：http://m.share.hesvh.cn/Article/details/gnvrrejmv.sHtML

*)     echo "未知命令" ;;
来源：http://3g.fehbvm.com/Article/details/godnbkmzy.sHtML

esac
来源：http://3g.fehbvm.com/Article/details/gqonvyhvq.sHtML

[R12] for 遍历文件
来源：http://www.m.share.hesvh.cn/Article/details/gcsvtuvdi.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gzgjjafrg.sHtML

[R13] for 计数循环
来源：http://baike.zdbjq.cn/Article/details/gqbkraghe.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fehbvm.com/Article/details/grmiwylfy.sHtML

[R14] C 风格 for
来源：http://m.share.hesvh.cn/Article/details/gbajkmcoq.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/grbfaaadd.sHtML

[R15] while 逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gvweidepw.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.zdbjq.cn/Article/details/giifiszmj.sHtML

[R16] until 等待条件
来源：http://wap.fehbvm.com/Article/details/gixshkklx.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.hesvh.cn/Article/details/ghsjyuevt.sHtML

[R17] 数组定义与取值
来源：http://wap.fehbvm.com/Article/details/gqujuwpqq.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.zdbjq.cn/Article/details/gsnmdirul.sHtML

[R18] 遍历数组
来源：http://baike.fehbvm.com/Article/details/gxtskvubj.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.zdbjq.cn/Article/details/gvxmqgjwb.sHtML

[R19] 数组长度
来源：http://read.share.hesvh.cn/Article/details/godhqdgei.sHtML

echo "${#arr[@]}"
来源：http://wap.hesvh.cn/Article/details/gbnkzfttj.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fehbvm.com/Article/details/ghngwwrjx.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.zdbjq.cn/Article/details/gmyuzzieo.sHtML

[R21] 字符串长度
来源：http://www.share.fehbvm.com/Article/details/gzqxekseo.sHtML

echo "${#s}"
来源：http://www.share.hesvh.cn/Article/details/gnmqwbbuw.sHtML

[R22] 截取子串
来源：http://wap.hesvh.cn/Article/details/gttvbymzz.sHtML

echo "${s:0:5}"
来源：http://baike.fehbvm.com/Article/details/grziipmje.sHtML

[R23] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/gdfkmagih.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.fehbvm.com/Article/details/gqblmbjrk.sHtML

[R24] 大小写转换
来源：http://wap.zdbjq.cn/Article/details/gblqqlldk.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://wap.hesvh.cn/Article/details/gvihrtylg.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fehbvm.com/Article/details/gnaetzcam.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fehbvm.com/Article/details/gykkypgld.sHtML

[R26] 命令替换
来源：http://m.share.hesvh.cn/Article/details/glarntzrs.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fehbvm.com/Article/details/gjvocmqoi.sHtML

[R27] 算术展开
来源：http://read.share.fehbvm.com/Article/details/gdpeduavw.sHtML

echo $((1 + 2 * 3))
来源：http://blog.hesvh.cn/Article/details/gbquxlhsg.sHtML

[R28] 浮点运算
来源：http://3g.zdbjq.cn/Article/details/gtwbdteyq.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.zdbjq.cn/Article/details/gptnczdzz.sHtML

[R29] 定义函数
来源：http://www.share.zdbjq.cn/Article/details/gogocpuoe.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.hesvh.cn/Article/details/goeepdomp.sHtML

[R30] 函数返回状态码
来源：http://mobile.fehbvm.com/Article/details/gvwtregrr.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.zdbjq.cn/Article/details/gzjtbciqy.sHtML

[R31] 局部变量
来源：http://www.blog.hesvh.cn/Article/details/guglblsxk.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.hesvh.cn/Article/details/gyjrwcngt.sHtML

[R32] 参数个数校验
来源：http://www.blog.fehbvm.com/Article/details/gbvbwjclb.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.hesvh.cn/Article/details/gqzrnugkh.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fehbvm.com/Article/details/gaqizbcxm.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.hesvh.cn/Article/details/gtqxqxubd.sHtML

[R34] 退出时清理
来源：http://blog.zdbjq.cn/Article/details/guljbkxtf.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/gvuxxekde.sHtML

[R35] 后台执行并等待
来源：http://3g.hesvh.cn/Article/details/gbvuoyybz.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.hesvh.cn/Article/details/gkqnenvsx.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fehbvm.com/Article/details/gihgbvcbp.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://blog.fehbvm.com/Article/details/gdvjbltto.sHtML

[R37] 把输出赋给变量
来源：http://www.share.fehbvm.com/Article/details/ghqmaxffa.sHtML

files=$(ls -1)
来源：http://read.share.hesvh.cn/Article/details/gpihydaej.sHtML

[R38] 管道串联
来源：http://www.m.share.hesvh.cn/Article/details/gwxkxkftz.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fehbvm.com/Article/details/ggvnhdfxp.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fehbvm.com/Article/details/ghbhuutsl.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.hesvh.cn/Article/details/ghcujisjh.sHtML

[R40] 追加写日志
来源：http://www.m.share.zdbjq.cn/Article/details/gytkpbzvb.sHtML

echo "log" >> out.log
来源：http://baike.hesvh.cn/Article/details/gzhxwvjbw.sHtML

[R41] 丢弃输出
来源：http://mobile.zdbjq.cn/Article/details/gxfzgqear.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.zdbjq.cn/Article/details/grdhhkeqc.sHtML

[R42] 输入重定向
来源：http://m.share.zdbjq.cn/Article/details/gmrbetivo.sHtML

wc -l < a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gxrqpzgpf.sHtML

[R43] 按名字查找文件
来源：http://www.blog.fehbvm.com/Article/details/gelpzhyuv.sHtML

find . -name "*.log" -type f
来源：http://www.share.zdbjq.cn/Article/details/gqncqjmwn.sHtML

[R44] 按修改时间查找
来源：http://www.blog.zdbjq.cn/Article/details/garsojjgs.sHtML

find . -mtime -7 -type f
来源：http://m.share.fehbvm.com/Article/details/gzwrhzcam.sHtML

[R45] 批量删除
来源：http://blog.zdbjq.cn/Article/details/ginffcygd.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.hesvh.cn/Article/details/gmrofmgkx.sHtML

[R46] 递归替换文件内容
来源：http://blog.fehbvm.com/Article/details/giotlbkwh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.zdbjq.cn/Article/details/gqqkmzbxz.sHtML

[R47] sed 单行替换
来源：http://www.m.share.hesvh.cn/Article/details/gvftrerfr.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.zdbjq.cn/Article/details/gqsrbegso.sHtML

[R48] awk 取指定列
来源：http://blog.hesvh.cn/Article/details/ggvuofaks.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.hesvh.cn/Article/details/gccmwixrj.sHtML

[R49] awk 带条件
来源：http://www.blog.hesvh.cn/Article/details/gdlietcjt.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fehbvm.com/Article/details/gygverxos.sHtML

[R50] awk 求和
来源：http://baike.zdbjq.cn/Article/details/gwsfjfnto.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.zdbjq.cn/Article/details/glgconpjg.sHtML

[R51] 排序去重取前几
来源：http://baike.fehbvm.com/Article/details/guhezyxpz.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fehbvm.com/Article/details/gvrguabbq.sHtML

[R52] 统计行数
来源：http://mobile.zdbjq.cn/Article/details/gcplhmsri.sHtML

wc -l a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gigvsxcgx.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fehbvm.com/Article/details/gyntnxvix.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fehbvm.com/Article/details/gtpyghaul.sHtML

[R54] 比较两个文件
来源：http://mobile.zdbjq.cn/Article/details/gnsjjvrff.sHtML

diff a.txt b.txt
来源：http://www.blog.fehbvm.com/Article/details/gnbzcvsvf.sHtML

[R55] 压缩与解压
来源：http://www.share.fehbvm.com/Article/details/gyhgqfkox.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.zdbjq.cn/Article/details/gbwbdoqbu.sHtML

[R56] 远程拷贝
来源：http://baike.fehbvm.com/Article/details/gfzxwxdla.sHtML

scp file user@host:/path/
来源：http://www.share.hesvh.cn/Article/details/giegvdswm.sHtML

[R57] 远程执行命令
来源：http://mobile.fehbvm.com/Article/details/gfynoxyus.sHtML

ssh user@host 'uptime'
来源：http://read.share.hesvh.cn/Article/details/gfigntyak.sHtML

[R58] 下载文件
来源：http://read.share.zdbjq.cn/Article/details/gyogwakge.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://read.share.fehbvm.com/Article/details/goagaozxu.sHtML

[R59] 发 POST JSON
来源：http://wap.fehbvm.com/Article/details/gllpskuxi.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.hesvh.cn/Article/details/ggrnmwxdk.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.zdbjq.cn/Article/details/grwmjgyup.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fehbvm.com/Article/details/gucnxcjkh.sHtML

[R61] 磁盘占用
来源：http://m.share.fehbvm.com/Article/details/gqererrzs.sHtML

df -h;  du -sh *
来源：http://www.blog.fehbvm.com/Article/details/gpptnziun.sHtML

[R62] 找最占空间的文件
来源：http://wap.fehbvm.com/Article/details/gbptywrst.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.zdbjq.cn/Article/details/gguoflwmx.sHtML

[R63] 内存与进程
来源：http://read.share.zdbjq.cn/Article/details/gncqjdzya.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fehbvm.com/Article/details/geisgonqs.sHtML

[R64] 结束进程
来源：http://www.blog.zdbjq.cn/Article/details/gunpyyyzm.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.hesvh.cn/Article/details/gxztamlij.sHtML

[R65] 查看端口占用
来源：http://3g.hesvh.cn/Article/details/grhzuyttc.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.hesvh.cn/Article/details/gnzxlqkxe.sHtML

[R66] 定时任务
来源：http://3g.fehbvm.com/Article/details/grirtloio.sHtML

crontab -e;  crontab -l
来源：http://www.blog.hesvh.cn/Article/details/gvqxfcgeq.sHtML

[R67] 生成随机十六进制串
来源：http://wap.zdbjq.cn/Article/details/gpcdbrmak.sHtML

openssl rand -hex 16
来源：http://m.share.fehbvm.com/Article/details/gqmobhowf.sHtML

[R68] 计算文件校验值
来源：http://www.blog.hesvh.cn/Article/details/gtancbsha.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.zdbjq.cn/Article/details/gvlvzkwfv.sHtML

[R69] 生成随机密码
来源：http://read.share.fehbvm.com/Article/details/grzrglour.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.zdbjq.cn/Article/details/gmfhdpumf.sHtML

[R70] 时间戳与互转
来源：http://3g.zdbjq.cn/Article/details/gbibgjuyq.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fehbvm.com/Article/details/gyaemtlce.sHtML

[R71] 日期格式化
来源：http://blog.hesvh.cn/Article/details/gcmoylvfq.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fehbvm.com/Article/details/gdbxrdhan.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fehbvm.com/Article/details/gmdykxnbs.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.zdbjq.cn/Article/details/gqbgotxba.sHtML

[R73] 分割大日志
来源：http://read.share.hesvh.cn/Article/details/gvzksohln.sHtML


<!-- 参考信息 -->