代发 wailian999

[Q33] 多列分组
来源：http://www.m.share.hesvh.cn/Article/details/gmshfhhhy.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.hesvh.cn/Article/details/glkkgophm.sHtML

[Q34] 每组取第一条
来源：http://read.share.hesvh.cn/Article/details/gnbvlpqef.sHtML

SELECT * FROM (
来源：http://www.blog.hesvh.cn/Article/details/gyfwhdrpy.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.hesvh.cn/Article/details/gjthjipfj.sHtML

) t WHERE rn = 1;
来源：http://www.share.zdbjq.cn/Article/details/gcrbxgiyz.sHtML

[Q35] 内连接
来源：http://read.share.hesvh.cn/Article/details/gnzaxohko.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://3g.hesvh.cn/Article/details/gyyioldvx.sHtML

[Q36] 左连接
来源：http://wap.hesvh.cn/Article/details/ganybatyz.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.hesvh.cn/Article/details/gmguhjdml.sHtML

[Q37] 右连接
来源：http://read.share.hesvh.cn/Article/details/gawsvatwu.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.m.share.zdbjq.cn/Article/details/gfwxnzlpl.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://wap.fehbvm.com/Article/details/ggbmqspgn.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.zdbjq.cn/Article/details/gsmplzhqz.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.fehbvm.com/Article/details/gztspoxoo.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.hesvh.cn/Article/details/gpilhnxtc.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.blog.fehbvm.com/Article/details/gpwkvhzba.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://blog.zdbjq.cn/Article/details/gmyzibeoc.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.zdbjq.cn/Article/details/gcdbbgmtx.sHtML

[Q41] 多表连接
来源：http://3g.hesvh.cn/Article/details/gonhrksre.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.fehbvm.com/Article/details/gzdyvhhof.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.m.share.fehbvm.com/Article/details/gcbimuhiy.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://3g.hesvh.cn/Article/details/gnwfpront.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.hesvh.cn/Article/details/gwdipiewr.sHtML

SELECT u.name, o.amount FROM users u
来源：http://m.share.hesvh.cn/Article/details/gmvthvldu.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.hesvh.cn/Article/details/gywyccijp.sHtML

[Q43] 标量子查询
来源：http://blog.fehbvm.com/Article/details/gbohgwqhi.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.m.share.fehbvm.com/Article/details/gwpbilrhr.sHtML

[Q44] IN 子查询
来源：http://www.m.share.hesvh.cn/Article/details/gbiryrfoa.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.hesvh.cn/Article/details/grvxptjpi.sHtML

[Q45] EXISTS 判断存在
来源：http://baike.fehbvm.com/Article/details/gbbqijlgh.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.fehbvm.com/Article/details/gfiaqqawv.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.hesvh.cn/Article/details/gzzbdkzhv.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.hesvh.cn/Article/details/gwiuiutbk.sHtML

[Q47] 与平均值比较
来源：http://baike.fehbvm.com/Article/details/ggulpybtr.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.fehbvm.com/Article/details/gocmbjlvp.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.fehbvm.com/Article/details/gpdcsbkeu.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.fehbvm.com/Article/details/gewrxkhst.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.m.share.zdbjq.cn/Article/details/guxvfzzjy.sHtML

[Q49] 更新单行
来源：http://www.m.share.fehbvm.com/Article/details/gmlcebyvg.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.share.hesvh.cn/Article/details/gedvvvcdz.sHtML

[Q50] 批量更新
来源：http://mobile.zdbjq.cn/Article/details/gffoctwah.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.hesvh.cn/Article/details/gzqhnanbx.sHtML

[Q51] 用子查询更新
来源：http://www.share.hesvh.cn/Article/details/gxlcrlqdy.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.m.share.zdbjq.cn/Article/details/gzvivloia.sHtML

[Q52] 删除指定行
来源：http://3g.hesvh.cn/Article/details/gsinzpwcm.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.fehbvm.com/Article/details/gklxaimhk.sHtML

[Q53] 按条件删除
来源：http://m.share.zdbjq.cn/Article/details/giwvismdz.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.hesvh.cn/Article/details/ggjpueztm.sHtML

[Q54] 清空表
来源：http://mobile.fehbvm.com/Article/details/gaozrtfog.sHtML

TRUNCATE TABLE logs;
来源：http://www.blog.fehbvm.com/Article/details/gysrkfnmj.sHtML

[Q55] 排名（并列占位）
来源：http://wap.hesvh.cn/Article/details/gfnqeemin.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.hesvh.cn/Article/details/gclqnwgrn.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.zdbjq.cn/Article/details/gpqpovuqm.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.fehbvm.com/Article/details/gxktcoecw.sHtML

[Q57] 行号
来源：http://blog.hesvh.cn/Article/details/gowadwilq.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gdxlunmbt.sHtML

[Q58] 累计求和
来源：http://m.share.zdbjq.cn/Article/details/gegwnftph.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gkpbzeoja.sHtML

[Q59] 分组内累计
来源：http://www.blog.hesvh.cn/Article/details/goxnjuotp.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gczuuefrf.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.share.fehbvm.com/Article/details/gclxcykkk.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.fehbvm.com/Article/details/gzczzgmvk.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gcbxisckt.sHtML

[Q61] 移动平均
来源：http://read.share.zdbjq.cn/Article/details/gcwcogvwo.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/gezhtbnlp.sHtML

[Q62] 分组占比
来源：http://wap.hesvh.cn/Article/details/gcapwxfvq.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gcnsbhtsn.sHtML

[Q63] 开启事务
来源：http://wap.hesvh.cn/Article/details/gzucilmgg.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.fehbvm.com/Article/details/ggspflyih.sHtML

[Q64] 提交事务
来源：http://mobile.hesvh.cn/Article/details/guutikylf.sHtML

COMMIT;
来源：http://m.share.zdbjq.cn/Article/details/gvexiwjwr.sHtML

[Q65] 回滚事务
来源：http://m.share.zdbjq.cn/Article/details/guoraodkn.sHtML

ROLLBACK;
来源：http://m.share.hesvh.cn/Article/details/gvrpekprc.sHtML

[Q66] 行锁查询
来源：http://read.share.hesvh.cn/Article/details/gnrlitdvj.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.hesvh.cn/Article/details/gvwigcbdj.sHtML

[Q67] 设置隔离级别
来源：http://www.share.zdbjq.cn/Article/details/gpzttettr.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.fehbvm.com/Article/details/gzrpbgbhq.sHtML

[Q68] 保存点
来源：http://www.m.share.hesvh.cn/Article/details/gcsunownl.sHtML

SAVEPOINT sp1;
来源：http://blog.hesvh.cn/Article/details/gknknuhlt.sHtML

ROLLBACK TO sp1;
来源：http://read.share.zdbjq.cn/Article/details/gsdenjrdb.sHtML

[Q69] 查看执行计划
来源：http://mobile.fehbvm.com/Article/details/gpdohdvhn.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://3g.zdbjq.cn/Article/details/gsnrgyivt.sHtML

[Q70] 更新统计信息
来源：http://blog.hesvh.cn/Article/details/gaxknlcnw.sHtML

ANALYZE TABLE users;
来源：http://wap.hesvh.cn/Article/details/gnxdbqkie.sHtML

[Q71] 查看建表语句
来源：http://baike.fehbvm.com/Article/details/gohpmvlut.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://baike.zdbjq.cn/Article/details/gtlpcyaib.sHtML

[Q72] 查看索引
来源：http://m.share.hesvh.cn/Article/details/gsilottdc.sHtML

SHOW INDEX FROM users;
来源：http://mobile.hesvh.cn/Article/details/gaeiqvzkg.sHtML

[Q73] 查看表状态
来源：http://www.share.zdbjq.cn/Article/details/gjsloybst.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.hesvh.cn/Article/details/gefqcfwrz.sHtML

[Q74] 强制使用索引
来源：http://mobile.fehbvm.com/Article/details/gvmiyxwtw.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.zdbjq.cn/Article/details/gjbmdlilq.sHtML

[Q75] 日期格式化
来源：http://blog.fehbvm.com/Article/details/gdmrjnbrn.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.fehbvm.com/Article/details/gohbbvtqu.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://wap.hesvh.cn/Article/details/gzmvjaccr.sHtML

[Q76] 按天统计
来源：http://www.share.fehbvm.com/Article/details/gmpyjfwyu.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.hesvh.cn/Article/details/gjedwhhll.sHtML

[Q77] 时间加减
来源：http://3g.fehbvm.com/Article/details/goanwdxbq.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://mobile.hesvh.cn/Article/details/guswfrtvw.sHtML

[Q78] 当前时间
来源：http://3g.zdbjq.cn/Article/details/gknckkxgo.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://3g.zdbjq.cn/Article/details/gxyqqiwwy.sHtML

[Q79] 字符串拼接
来源：http://baike.fehbvm.com/Article/details/gdtfpeczl.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.blog.zdbjq.cn/Article/details/gzihiivan.sHtML

[Q80] 字符串截取
来源：http://www.m.share.fehbvm.com/Article/details/gifmnzlfh.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gqjilobpw.sHtML

[Q81] 字符串替换
来源：http://wap.fehbvm.com/Article/details/gxjcdxvjh.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.fehbvm.com/Article/details/gehsugxsb.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.fehbvm.com/Article/details/gtukzdjxl.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gujscjnct.sHtML

[Q83] 大小写转换
来源：http://mobile.fehbvm.com/Article/details/gvszkxdhl.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gjhllyfwk.sHtML

[Q84] 去除首尾空格
来源：http://mobile.fehbvm.com/Article/details/gptjoeyki.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/geatzkawm.sHtML

[Q85] 数值取整
来源：http://mobile.zdbjq.cn/Article/details/gdjexvtat.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.hesvh.cn/Article/details/gsykuphzx.sHtML

[Q86] 读取 JSON 字段
来源：http://blog.hesvh.cn/Article/details/grgxcnuxb.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://baike.hesvh.cn/Article/details/gwwgirzfm.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.zdbjq.cn/Article/details/gsisvivdm.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://wap.zdbjq.cn/Article/details/giknugtqw.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.hesvh.cn/Article/details/gogfqiloo.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.hesvh.cn/Article/details/goehobozh.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gvzqjafei.sHtML

[Q89] 判断表是否存在
来源：http://wap.hesvh.cn/Article/details/gxbszfkbk.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://m.share.fehbvm.com/Article/details/gybzdeexv.sHtML

[Q90] 生成序号列
来源：http://read.share.fehbvm.com/Article/details/gvwcplrvk.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.zdbjq.cn/Article/details/gtkteculd.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gvjeiejek.sHtML

R. Bash 专题
来源：http://read.share.hesvh.cn/Article/details/gvrjxuqmt.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gwiqayhax.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.zdbjq.cn/Article/details/gtawjfirb.sHtML

#!/usr/bin/env bash
来源：http://read.share.hesvh.cn/Article/details/gpfdokhzx.sHtML

set -euo pipefail
来源：http://m.share.hesvh.cn/Article/details/ggxwehejx.sHtML

[R02] 变量赋值与使用
来源：http://www.m.share.zdbjq.cn/Article/details/gqufcbgwy.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.zdbjq.cn/Article/details/gahfkqogc.sHtML

[R03] 只读变量
来源：http://3g.fehbvm.com/Article/details/gjtkjhbsu.sHtML

readonly PI=3.14
来源：http://wap.hesvh.cn/Article/details/gazouigsi.sHtML

[R04] 位置参数
来源：http://www.m.share.hesvh.cn/Article/details/gnxgypqmr.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://baike.hesvh.cn/Article/details/gewapsjhq.sHtML

[R05] 参数默认值
来源：http://www.blog.hesvh.cn/Article/details/goejcudnf.sHtML

name="${1:-default}"
来源：http://www.share.fehbvm.com/Article/details/gqarjipox.sHtML

[R06] 判断命令是否存在
来源：http://www.share.zdbjq.cn/Article/details/gniermgiy.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.hesvh.cn/Article/details/gsslcvmrw.sHtML

[R07] if 判断文件
来源：http://wap.zdbjq.cn/Article/details/gylamdcsl.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.zdbjq.cn/Article/details/gbnonyemz.sHtML

[R08] 数值比较
来源：http://wap.fehbvm.com/Article/details/gerxczxut.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.zdbjq.cn/Article/details/gsugtufve.sHtML

[R09] 字符串比较
来源：http://3g.zdbjq.cn/Article/details/gssysvzkm.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.share.hesvh.cn/Article/details/ghpeisrnp.sHtML

[R10] 正则匹配
来源：http://www.m.share.fehbvm.com/Article/details/gicxjkdjq.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.zdbjq.cn/Article/details/gjtrdwyru.sHtML

[R11] case 多分支
来源：http://m.share.zdbjq.cn/Article/details/gpqrkqgcq.sHtML

case "$1" in
来源：http://baike.fehbvm.com/Article/details/gxrbtlvmi.sHtML

start) echo "启动" ;;
来源：http://m.share.fehbvm.com/Article/details/gjbcpoigm.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fehbvm.com/Article/details/gubflkxhw.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fehbvm.com/Article/details/gcpzwphrc.sHtML

esac
来源：http://read.share.zdbjq.cn/Article/details/ghzrfluih.sHtML

[R12] for 遍历文件
来源：http://3g.zdbjq.cn/Article/details/gkhdfyyrg.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.hesvh.cn/Article/details/gsmazoell.sHtML

[R13] for 计数循环
来源：http://blog.zdbjq.cn/Article/details/gkdbhnfxj.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.fehbvm.com/Article/details/gbbztcgmd.sHtML

[R14] C 风格 for
来源：http://www.blog.zdbjq.cn/Article/details/gblpzgqqm.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://mobile.fehbvm.com/Article/details/gmkujvxsg.sHtML

[R15] while 逐行读文件
来源：http://wap.zdbjq.cn/Article/details/gcbuudxnj.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.hesvh.cn/Article/details/glznioquh.sHtML

[R16] until 等待条件
来源：http://blog.zdbjq.cn/Article/details/gvbsmgcdp.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.fehbvm.com/Article/details/gudhkifgd.sHtML

[R17] 数组定义与取值
来源：http://read.share.hesvh.cn/Article/details/glnhmczkx.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fehbvm.com/Article/details/gfsoztnkl.sHtML

[R18] 遍历数组
来源：http://blog.fehbvm.com/Article/details/gmvxprmsz.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.zdbjq.cn/Article/details/gqofezcoa.sHtML

[R19] 数组长度
来源：http://m.share.hesvh.cn/Article/details/gpdouxhzp.sHtML

echo "${#arr[@]}"
来源：http://wap.zdbjq.cn/Article/details/geelhkhtz.sHtML

[R20] 关联数组（字典）
来源：http://baike.hesvh.cn/Article/details/gflcweamc.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.hesvh.cn/Article/details/gfmnzktke.sHtML

[R21] 字符串长度
来源：http://mobile.hesvh.cn/Article/details/gouskoqfk.sHtML

echo "${#s}"
来源：http://read.share.fehbvm.com/Article/details/grtemvncs.sHtML

[R22] 截取子串
来源：http://wap.zdbjq.cn/Article/details/gjeeooyfv.sHtML

echo "${s:0:5}"
来源：http://3g.fehbvm.com/Article/details/guvkdidzu.sHtML

[R23] 字符串替换
来源：http://mobile.zdbjq.cn/Article/details/grzeypuel.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.zdbjq.cn/Article/details/gpoqhsuix.sHtML

[R24] 大小写转换
来源：http://www.share.hesvh.cn/Article/details/guyhweeap.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fehbvm.com/Article/details/gkecimzij.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.zdbjq.cn/Article/details/gxpktesqb.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://baike.hesvh.cn/Article/details/grzaspcpx.sHtML

[R26] 命令替换
来源：http://wap.hesvh.cn/Article/details/gozlqelpx.sHtML

now=$(date +%F); echo "$now"
来源：http://www.blog.hesvh.cn/Article/details/gvmwlmqnu.sHtML

[R27] 算术展开
来源：http://m.share.hesvh.cn/Article/details/ggeiionhf.sHtML

echo $((1 + 2 * 3))
来源：http://blog.hesvh.cn/Article/details/gbxbkislh.sHtML

[R28] 浮点运算
来源：http://blog.zdbjq.cn/Article/details/gpvqceipp.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fehbvm.com/Article/details/gstdesdvd.sHtML

[R29] 定义函数
来源：http://baike.hesvh.cn/Article/details/gbsnkeaey.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.zdbjq.cn/Article/details/gbbnveplh.sHtML

[R30] 函数返回状态码
来源：http://www.blog.zdbjq.cn/Article/details/gripruaen.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.zdbjq.cn/Article/details/gtaxumorh.sHtML

[R31] 局部变量
来源：http://baike.zdbjq.cn/Article/details/ghourtpdm.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.zdbjq.cn/Article/details/ggknwzpfh.sHtML

[R32] 参数个数校验
来源：http://www.blog.hesvh.cn/Article/details/gzoqfcbum.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.zdbjq.cn/Article/details/glnlmsktf.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fehbvm.com/Article/details/gtfeyeyoq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fehbvm.com/Article/details/gxkwnhncs.sHtML

[R34] 退出时清理
来源：http://3g.fehbvm.com/Article/details/gigpuvvfg.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.zdbjq.cn/Article/details/gdkfovxry.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.fehbvm.com/Article/details/gwqktqwav.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.m.share.zdbjq.cn/Article/details/guarjtpms.sHtML

[R36] 并发执行多个任务
来源：http://blog.hesvh.cn/Article/details/gahgtmxjz.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.zdbjq.cn/Article/details/gugnxfwue.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fehbvm.com/Article/details/gcbaxerpv.sHtML

files=$(ls -1)
来源：http://www.m.share.hesvh.cn/Article/details/glemqqtsg.sHtML

[R38] 管道串联
来源：http://3g.fehbvm.com/Article/details/gfivelctq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.zdbjq.cn/Article/details/ggraqwpsx.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.zdbjq.cn/Article/details/gapisttfj.sHtML

cmd > out.log 2>&1
来源：http://blog.fehbvm.com/Article/details/gnehdnegx.sHtML

[R40] 追加写日志
来源：http://www.blog.fehbvm.com/Article/details/gkisbfkhq.sHtML

echo "log" >> out.log
来源：http://m.share.hesvh.cn/Article/details/gmnmnlybs.sHtML

[R41] 丢弃输出
来源：http://www.blog.hesvh.cn/Article/details/gdvwrrahh.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.zdbjq.cn/Article/details/gcmawmrkp.sHtML

[R42] 输入重定向
来源：http://m.share.fehbvm.com/Article/details/gcixpkdvs.sHtML

wc -l < a.txt
来源：http://blog.fehbvm.com/Article/details/gwzpcnstq.sHtML

[R43] 按名字查找文件
来源：http://mobile.hesvh.cn/Article/details/gaimvaibs.sHtML

find . -name "*.log" -type f
来源：http://read.share.zdbjq.cn/Article/details/gmuknfcat.sHtML

[R44] 按修改时间查找
来源：http://wap.zdbjq.cn/Article/details/gdcwaopen.sHtML

find . -mtime -7 -type f
来源：http://read.share.hesvh.cn/Article/details/gbakmbfcv.sHtML

[R45] 批量删除
来源：http://read.share.hesvh.cn/Article/details/gcinamfuq.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.hesvh.cn/Article/details/gajzwrgkk.sHtML

[R46] 递归替换文件内容
来源：http://blog.zdbjq.cn/Article/details/grabkjwnd.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fehbvm.com/Article/details/gcsiwncll.sHtML

[R47] sed 单行替换
来源：http://read.share.hesvh.cn/Article/details/ggbdonpdw.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fehbvm.com/Article/details/gfqgedejm.sHtML

[R48] awk 取指定列
来源：http://www.m.share.hesvh.cn/Article/details/gyqcwliny.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.hesvh.cn/Article/details/gtxrcikbi.sHtML

[R49] awk 带条件
来源：http://mobile.zdbjq.cn/Article/details/gizxliamk.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.fehbvm.com/Article/details/gibccaehq.sHtML

[R50] awk 求和
来源：http://read.share.hesvh.cn/Article/details/gzhxasvxm.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://m.share.fehbvm.com/Article/details/grgcbsqdz.sHtML

[R51] 排序去重取前几
来源：http://wap.fehbvm.com/Article/details/gruvvpngh.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://blog.zdbjq.cn/Article/details/gcneagsej.sHtML

[R52] 统计行数
来源：http://www.m.share.zdbjq.cn/Article/details/galqgeffs.sHtML

wc -l a.txt
来源：http://baike.hesvh.cn/Article/details/gozxuidpe.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fehbvm.com/Article/details/grhdtqkns.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.hesvh.cn/Article/details/gzlnbvtqe.sHtML

[R54] 比较两个文件
来源：http://baike.fehbvm.com/Article/details/gabegfxyq.sHtML

diff a.txt b.txt
来源：http://mobile.hesvh.cn/Article/details/gpulcrrno.sHtML

[R55] 压缩与解压
来源：http://mobile.fehbvm.com/Article/details/gixdzwoim.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fehbvm.com/Article/details/gtgegukjr.sHtML

[R56] 远程拷贝
来源：http://www.blog.zdbjq.cn/Article/details/gmfqrfzkf.sHtML

scp file user@host:/path/
来源：http://www.share.hesvh.cn/Article/details/ggtgsmogi.sHtML

[R57] 远程执行命令
来源：http://read.share.fehbvm.com/Article/details/gxrqvntkt.sHtML

ssh user@host 'uptime'
来源：http://3g.hesvh.cn/Article/details/gmsjjzjpo.sHtML

[R58] 下载文件
来源：http://mobile.fehbvm.com/Article/details/gtjofgssb.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.fehbvm.com/Article/details/gijrnmiky.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fehbvm.com/Article/details/gcpiiumue.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.zdbjq.cn/Article/details/gciuuxbyd.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.zdbjq.cn/Article/details/ggxkedqhm.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.zdbjq.cn/Article/details/gdporkqzm.sHtML

[R61] 磁盘占用
来源：http://www.blog.zdbjq.cn/Article/details/gztcrdwwe.sHtML

df -h;  du -sh *
来源：http://baike.fehbvm.com/Article/details/gqetvkwfw.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fehbvm.com/Article/details/gstxpuznb.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.hesvh.cn/Article/details/gpatwqawl.sHtML

[R63] 内存与进程
来源：http://read.share.fehbvm.com/Article/details/gersmvppu.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.hesvh.cn/Article/details/gkokombbx.sHtML

[R64] 结束进程
来源：http://m.share.hesvh.cn/Article/details/goxkuyxan.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.zdbjq.cn/Article/details/greuybikh.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fehbvm.com/Article/details/gqvfvwcns.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.hesvh.cn/Article/details/gasezwcee.sHtML

[R66] 定时任务
来源：http://3g.fehbvm.com/Article/details/gjlownsdt.sHtML

crontab -e;  crontab -l
来源：http://mobile.fehbvm.com/Article/details/gziusdpzb.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fehbvm.com/Article/details/giytphawy.sHtML

openssl rand -hex 16
来源：http://m.share.zdbjq.cn/Article/details/ggjzsnauf.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fehbvm.com/Article/details/gbwucowxs.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.zdbjq.cn/Article/details/gnefhcgdx.sHtML

[R69] 生成随机密码
来源：http://m.share.fehbvm.com/Article/details/gomymcqut.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.hesvh.cn/Article/details/gpfhzvlgy.sHtML

[R70] 时间戳与互转
来源：http://baike.hesvh.cn/Article/details/gousochgk.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.zdbjq.cn/Article/details/grwinmmui.sHtML

[R71] 日期格式化
来源：http://3g.fehbvm.com/Article/details/gwthtbfcr.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.zdbjq.cn/Article/details/gdnzvxhlu.sHtML

[R72] 等待端口就绪
来源：http://mobile.zdbjq.cn/Article/details/gzdnruvng.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.zdbjq.cn/Article/details/gnjxrnfme.sHtML

[R73] 分割大日志
来源：http://wap.zdbjq.cn/Article/details/gtaevtcro.sHtML

split -l 1000 big.log part_
来源：http://blog.hesvh.cn/Article/details/gswcbdfzq.sHtML

[R74] 批量重命名
来源：http://m.share.zdbjq.cn/Article/details/gklfwqejv.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.hesvh.cn/Article/details/gfgczvjbp.sHtML

[R75] 导出环境变量
来源：http://mobile.fehbvm.com/Article/details/gmuhhrvfm.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.hesvh.cn/Article/details/gvwbgmbhx.sHtML

[R76] 使用临时文件
来源：http://wap.fehbvm.com/Article/details/gzowozyws.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.hesvh.cn/Article/details/gpykqulrj.sHtML

[R77] 读取用户输入
来源：http://blog.zdbjq.cn/Article/details/goyicfgtk.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fehbvm.com/Article/details/gxdnygjkc.sHtML

[R78] 交互式菜单
来源：http://3g.hesvh.cn/Article/details/gaedkpthb.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fehbvm.com/Article/details/gdssnaqkm.sHtML

[R79] 解析命令行选项
来源：http://m.share.hesvh.cn/Article/details/gowxxjkda.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.hesvh.cn/Article/details/gmtemiywn.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.zdbjq.cn/Article/details/gwsyvbsbb.sHtML

time ./run.sh
来源：http://3g.fehbvm.com/Article/details/gvvjpvodt.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/glqlwblcl.sHtML

S. C / C++ 专题
来源：http://baike.fehbvm.com/Article/details/gjouklmbe.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gphzwicco.sHtML

[S01] C：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gmukrgywa.sHtML

#include <stdio.h>
来源：http://m.share.fehbvm.com/Article/details/gvevypjks.sHtML


<!-- 参考信息 -->