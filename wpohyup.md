代发 wailian999

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gluelawnw.sHtML

[Q30] 分组统计
来源：http://blog.zdbjq.cn/Article/details/ggoavlqkd.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/gxdgyfjfc.sHtML

[Q31] 分组后过滤
来源：http://www.share.zdbjq.cn/Article/details/ghadjqlpw.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.share.hesvh.cn/Article/details/gwwvqhofq.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/geveqnity.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gbrccvgmd.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.share.zdbjq.cn/Article/details/gjerjcnqo.sHtML

[Q33] 多列分组
来源：http://blog.zdbjq.cn/Article/details/grzbkkgpj.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.hesvh.cn/Article/details/gedonaqkn.sHtML

[Q34] 每组取第一条
来源：http://m.share.zdbjq.cn/Article/details/gnuazlduq.sHtML

SELECT * FROM (
来源：http://3g.fehbvm.com/Article/details/gnslaijwt.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.zdbjq.cn/Article/details/gvveywrtf.sHtML

) t WHERE rn = 1;
来源：http://read.share.zdbjq.cn/Article/details/gijlabrqd.sHtML

[Q35] 内连接
来源：http://read.share.fehbvm.com/Article/details/gfksowfhv.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fehbvm.com/Article/details/gsnggozmk.sHtML

[Q36] 左连接
来源：http://mobile.hesvh.cn/Article/details/ggguykhug.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://m.share.fehbvm.com/Article/details/gfrawinkq.sHtML

[Q37] 右连接
来源：http://3g.hesvh.cn/Article/details/gxjnxasce.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.fehbvm.com/Article/details/gtgwxzcuv.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.blog.fehbvm.com/Article/details/grhzepljr.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.share.hesvh.cn/Article/details/gjgpwjdsf.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.hesvh.cn/Article/details/gatpowvwa.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.hesvh.cn/Article/details/gehzbngxz.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://wap.zdbjq.cn/Article/details/giafccbjz.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://read.share.fehbvm.com/Article/details/gnmcmyuoy.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://read.share.fehbvm.com/Article/details/gactacjys.sHtML

[Q41] 多表连接
来源：http://mobile.zdbjq.cn/Article/details/gjfjsgcpl.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://3g.hesvh.cn/Article/details/gvcvrctxz.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.hesvh.cn/Article/details/grhihmrqw.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.fehbvm.com/Article/details/gqigvpwnk.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.hesvh.cn/Article/details/gggytiyoq.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.zdbjq.cn/Article/details/gwltnftpq.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.share.hesvh.cn/Article/details/gfxjguggm.sHtML

[Q43] 标量子查询
来源：http://www.blog.zdbjq.cn/Article/details/grrpjeksb.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.fehbvm.com/Article/details/ggkeqpeti.sHtML

[Q44] IN 子查询
来源：http://m.share.zdbjq.cn/Article/details/gggwwmfgs.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.hesvh.cn/Article/details/gfepqahvz.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.fehbvm.com/Article/details/grewjontx.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.m.share.hesvh.cn/Article/details/gugaocamy.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.zdbjq.cn/Article/details/glygdaatl.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.hesvh.cn/Article/details/gvpamagkh.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.fehbvm.com/Article/details/ghgptdhlr.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.zdbjq.cn/Article/details/gwduotvwr.sHtML

[Q48] CTE 公用表表达式
来源：http://m.share.hesvh.cn/Article/details/gvsgwnpij.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.hesvh.cn/Article/details/gkkqwyqrr.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.hesvh.cn/Article/details/gkmloxhos.sHtML

[Q49] 更新单行
来源：http://www.blog.zdbjq.cn/Article/details/gaduuynbj.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.blog.hesvh.cn/Article/details/gvkkqiswz.sHtML

[Q50] 批量更新
来源：http://mobile.hesvh.cn/Article/details/gjyggxpob.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.blog.zdbjq.cn/Article/details/geqqlperj.sHtML

[Q51] 用子查询更新
来源：http://m.share.fehbvm.com/Article/details/gdjiyxmlp.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://3g.fehbvm.com/Article/details/gqyalisgw.sHtML

[Q52] 删除指定行
来源：http://m.share.fehbvm.com/Article/details/gbyhcgzmr.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.zdbjq.cn/Article/details/grlriagmo.sHtML

[Q53] 按条件删除
来源：http://www.blog.hesvh.cn/Article/details/glfmxtjzm.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.zdbjq.cn/Article/details/gqgxrltfu.sHtML

[Q54] 清空表
来源：http://m.share.hesvh.cn/Article/details/gmatyrjhj.sHtML

TRUNCATE TABLE logs;
来源：http://www.m.share.fehbvm.com/Article/details/gikzrprij.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.fehbvm.com/Article/details/gkmqacfar.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.fehbvm.com/Article/details/gpwgsjvsi.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.zdbjq.cn/Article/details/gpnamhqbm.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.fehbvm.com/Article/details/gvbthzbqt.sHtML

[Q57] 行号
来源：http://m.share.zdbjq.cn/Article/details/gsutrtwlt.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.zdbjq.cn/Article/details/gidnteaob.sHtML

[Q58] 累计求和
来源：http://3g.fehbvm.com/Article/details/goyinaytt.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.share.fehbvm.com/Article/details/giwlwjfqk.sHtML

[Q59] 分组内累计
来源：http://www.blog.hesvh.cn/Article/details/gjvzxlxit.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.zdbjq.cn/Article/details/gpsvgzcuq.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.hesvh.cn/Article/details/gkeaogykh.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.fehbvm.com/Article/details/gzfkiaowy.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gzozvsjql.sHtML

[Q61] 移动平均
来源：http://read.share.fehbvm.com/Article/details/gfaaqjspi.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/ghfmuhngu.sHtML

[Q62] 分组占比
来源：http://read.share.hesvh.cn/Article/details/ggigmxnvj.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.hesvh.cn/Article/details/gxycpqhsv.sHtML

[Q63] 开启事务
来源：http://www.m.share.hesvh.cn/Article/details/gnmitzyly.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.zdbjq.cn/Article/details/gjrbcgeho.sHtML

[Q64] 提交事务
来源：http://blog.zdbjq.cn/Article/details/ggwcjmnbb.sHtML

COMMIT;
来源：http://www.m.share.hesvh.cn/Article/details/gxswhpxly.sHtML

[Q65] 回滚事务
来源：http://blog.hesvh.cn/Article/details/gfmfmsdpf.sHtML

ROLLBACK;
来源：http://read.share.fehbvm.com/Article/details/gcpwfzznr.sHtML

[Q66] 行锁查询
来源：http://www.m.share.hesvh.cn/Article/details/gulwqbtvl.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.zdbjq.cn/Article/details/glcverjxe.sHtML

[Q67] 设置隔离级别
来源：http://www.share.hesvh.cn/Article/details/gtwwzjhvf.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.fehbvm.com/Article/details/gcvqznylr.sHtML

[Q68] 保存点
来源：http://read.share.fehbvm.com/Article/details/gxkpdlrai.sHtML

SAVEPOINT sp1;
来源：http://3g.zdbjq.cn/Article/details/gufskynkq.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.zdbjq.cn/Article/details/givdhnare.sHtML

[Q69] 查看执行计划
来源：http://mobile.zdbjq.cn/Article/details/guydkcwwu.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.zdbjq.cn/Article/details/gmcashpcn.sHtML

[Q70] 更新统计信息
来源：http://www.blog.zdbjq.cn/Article/details/gqxjgmhgb.sHtML

ANALYZE TABLE users;
来源：http://blog.fehbvm.com/Article/details/gxfhbknpo.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.hesvh.cn/Article/details/gdrqyseju.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.blog.fehbvm.com/Article/details/gfciyvazu.sHtML

[Q72] 查看索引
来源：http://3g.hesvh.cn/Article/details/ghrqqkljf.sHtML

SHOW INDEX FROM users;
来源：http://read.share.hesvh.cn/Article/details/gujmypewf.sHtML

[Q73] 查看表状态
来源：http://3g.fehbvm.com/Article/details/gjkcgxedc.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.fehbvm.com/Article/details/grfabicbz.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.hesvh.cn/Article/details/gbxpsmjlf.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://blog.fehbvm.com/Article/details/gjouanebq.sHtML

[Q75] 日期格式化
来源：http://www.share.hesvh.cn/Article/details/gfsiywrbi.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gooltvujk.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://mobile.fehbvm.com/Article/details/galaofxlo.sHtML

[Q76] 按天统计
来源：http://3g.fehbvm.com/Article/details/gtvmqufrg.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://mobile.hesvh.cn/Article/details/gbtvsrevf.sHtML

[Q77] 时间加减
来源：http://blog.hesvh.cn/Article/details/gygwgtrtb.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.zdbjq.cn/Article/details/gbqnwqrux.sHtML

[Q78] 当前时间
来源：http://www.blog.zdbjq.cn/Article/details/gfiucaoef.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://m.share.zdbjq.cn/Article/details/gkzamxsgx.sHtML

[Q79] 字符串拼接
来源：http://mobile.fehbvm.com/Article/details/gzzfnxcgo.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.fehbvm.com/Article/details/gjsrbqrtz.sHtML

[Q80] 字符串截取
来源：http://wap.zdbjq.cn/Article/details/gwqsrkmwk.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gnbyrhbgm.sHtML

[Q81] 字符串替换
来源：http://www.share.hesvh.cn/Article/details/gpbxqwmrs.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://mobile.fehbvm.com/Article/details/gbwpxhpep.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.fehbvm.com/Article/details/gpcelhhan.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gpghtxitc.sHtML

[Q83] 大小写转换
来源：http://blog.hesvh.cn/Article/details/gsuypwfwh.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/geqkgjfud.sHtML

[Q84] 去除首尾空格
来源：http://blog.zdbjq.cn/Article/details/gremysebo.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gvjkkykuo.sHtML

[Q85] 数值取整
来源：http://www.m.share.fehbvm.com/Article/details/ghnocuwmh.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.zdbjq.cn/Article/details/gmhwnfrui.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.hesvh.cn/Article/details/gixyxulbh.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.hesvh.cn/Article/details/gychbkqqw.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.zdbjq.cn/Article/details/gufhpkloh.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.zdbjq.cn/Article/details/gjfkegorc.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.zdbjq.cn/Article/details/gyfdtckeh.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.zdbjq.cn/Article/details/gpfzdnzem.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gbvzwagzs.sHtML

[Q89] 判断表是否存在
来源：http://baike.fehbvm.com/Article/details/gdxwqfkdo.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.zdbjq.cn/Article/details/gqwcvoaso.sHtML

[Q90] 生成序号列
来源：http://read.share.fehbvm.com/Article/details/gibqewynu.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.zdbjq.cn/Article/details/ggvafhtkm.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/geblsiavw.sHtML

R. Bash 专题
来源：http://mobile.fehbvm.com/Article/details/gvwwerugy.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gucvvrplb.sHtML

[R01] shebang 与严格模式
来源：http://www.blog.fehbvm.com/Article/details/gzpuoqjjp.sHtML

#!/usr/bin/env bash
来源：http://wap.hesvh.cn/Article/details/gzjpdmonk.sHtML

set -euo pipefail
来源：http://m.share.hesvh.cn/Article/details/gmkqxzcwh.sHtML

[R02] 变量赋值与使用
来源：http://mobile.hesvh.cn/Article/details/gpdomnqkm.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.hesvh.cn/Article/details/gofydbzcf.sHtML

[R03] 只读变量
来源：http://www.share.zdbjq.cn/Article/details/gvzmsecbz.sHtML

readonly PI=3.14
来源：http://blog.zdbjq.cn/Article/details/gncnnatby.sHtML

[R04] 位置参数
来源：http://www.blog.zdbjq.cn/Article/details/gpskywxmy.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.share.hesvh.cn/Article/details/grfcfgpif.sHtML

[R05] 参数默认值
来源：http://www.share.zdbjq.cn/Article/details/gilpoaifh.sHtML

name="${1:-default}"
来源：http://wap.zdbjq.cn/Article/details/gjzsvitwz.sHtML

[R06] 判断命令是否存在
来源：http://www.share.hesvh.cn/Article/details/gyzpagiji.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.zdbjq.cn/Article/details/geohxyubu.sHtML

[R07] if 判断文件
来源：http://www.m.share.zdbjq.cn/Article/details/gzfvrzgde.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.hesvh.cn/Article/details/getwdorxt.sHtML

[R08] 数值比较
来源：http://www.blog.zdbjq.cn/Article/details/gcaadwuvm.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fehbvm.com/Article/details/gjfbmlhfo.sHtML

[R09] 字符串比较
来源：http://www.share.hesvh.cn/Article/details/ghckndnnv.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.hesvh.cn/Article/details/gefbwatzr.sHtML

[R10] 正则匹配
来源：http://3g.hesvh.cn/Article/details/gxptalcpe.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fehbvm.com/Article/details/gwhtqzkvl.sHtML

[R11] case 多分支
来源：http://www.m.share.zdbjq.cn/Article/details/gbiloqcxf.sHtML

case "$1" in
来源：http://read.share.hesvh.cn/Article/details/gocwwltoz.sHtML

start) echo "启动" ;;
来源：http://www.m.share.zdbjq.cn/Article/details/gggtpinem.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.hesvh.cn/Article/details/gpylzynif.sHtML

*)     echo "未知命令" ;;
来源：http://baike.fehbvm.com/Article/details/gmeowiswl.sHtML

esac
来源：http://www.share.zdbjq.cn/Article/details/gytdylhid.sHtML

[R12] for 遍历文件
来源：http://www.blog.hesvh.cn/Article/details/glqbplspu.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fehbvm.com/Article/details/gkltqnhgi.sHtML

[R13] for 计数循环
来源：http://www.blog.zdbjq.cn/Article/details/ggqcrrpue.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.hesvh.cn/Article/details/gkulsabsk.sHtML

[R14] C 风格 for
来源：http://3g.hesvh.cn/Article/details/gcdezuxpq.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/glwydafij.sHtML

[R15] while 逐行读文件
来源：http://baike.fehbvm.com/Article/details/gwwqmjitg.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.hesvh.cn/Article/details/gzszgjfii.sHtML

[R16] until 等待条件
来源：http://wap.fehbvm.com/Article/details/ggwuqyzzq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/gcfmttgwl.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fehbvm.com/Article/details/grhowihex.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.share.fehbvm.com/Article/details/glodmmuet.sHtML

[R18] 遍历数组
来源：http://www.share.hesvh.cn/Article/details/gqjmkjhbi.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fehbvm.com/Article/details/gskwjsave.sHtML

[R19] 数组长度
来源：http://3g.fehbvm.com/Article/details/gkpgghtwq.sHtML

echo "${#arr[@]}"
来源：http://m.share.hesvh.cn/Article/details/gcmmxgzaw.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.hesvh.cn/Article/details/gnzogxlin.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fehbvm.com/Article/details/gidklyfrw.sHtML

[R21] 字符串长度
来源：http://m.share.fehbvm.com/Article/details/gvakqczix.sHtML

echo "${#s}"
来源：http://mobile.hesvh.cn/Article/details/gwbmzkkck.sHtML

[R22] 截取子串
来源：http://www.m.share.zdbjq.cn/Article/details/gqytmwqgq.sHtML

echo "${s:0:5}"
来源：http://www.blog.zdbjq.cn/Article/details/gzuryrhus.sHtML

[R23] 字符串替换
来源：http://m.share.hesvh.cn/Article/details/gkrktfsbp.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.fehbvm.com/Article/details/gzhfswozh.sHtML

[R24] 大小写转换
来源：http://3g.zdbjq.cn/Article/details/gzmcdzhor.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://baike.fehbvm.com/Article/details/gzqgitdyg.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.m.share.zdbjq.cn/Article/details/goyxdkjrp.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fehbvm.com/Article/details/gxphdqzpk.sHtML

[R26] 命令替换
来源：http://blog.fehbvm.com/Article/details/gzqtukqml.sHtML

now=$(date +%F); echo "$now"
来源：http://baike.hesvh.cn/Article/details/goxjpjano.sHtML

[R27] 算术展开
来源：http://mobile.fehbvm.com/Article/details/grdifndxx.sHtML

echo $((1 + 2 * 3))
来源：http://www.share.zdbjq.cn/Article/details/gpyotkvum.sHtML

[R28] 浮点运算
来源：http://blog.zdbjq.cn/Article/details/ggpasoosj.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.blog.fehbvm.com/Article/details/gjwoilhce.sHtML

[R29] 定义函数
来源：http://blog.zdbjq.cn/Article/details/gtpgfhwrq.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.m.share.hesvh.cn/Article/details/gsepnplih.sHtML

[R30] 函数返回状态码
来源：http://blog.zdbjq.cn/Article/details/gtzmwcmdi.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://baike.hesvh.cn/Article/details/gnxppygzj.sHtML

[R31] 局部变量
来源：http://www.blog.fehbvm.com/Article/details/gxvfuqvhd.sHtML

f() { local x=1; echo "$x"; }
来源：http://read.share.zdbjq.cn/Article/details/grlbixtrd.sHtML

[R32] 参数个数校验
来源：http://m.share.fehbvm.com/Article/details/gskhqpkwy.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fehbvm.com/Article/details/guddvulvo.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.hesvh.cn/Article/details/gpvffpjeb.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.blog.hesvh.cn/Article/details/gxczcpije.sHtML

[R34] 退出时清理
来源：http://blog.zdbjq.cn/Article/details/gvxvbuvjm.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/gmanunuax.sHtML

[R35] 后台执行并等待
来源：http://baike.hesvh.cn/Article/details/givrawxrc.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.hesvh.cn/Article/details/gkxmgaidu.sHtML

[R36] 并发执行多个任务
来源：http://wap.fehbvm.com/Article/details/gtcrrrdko.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://m.share.zdbjq.cn/Article/details/gyrqpxwsi.sHtML

[R37] 把输出赋给变量
来源：http://www.share.zdbjq.cn/Article/details/gefdmftlb.sHtML

files=$(ls -1)
来源：http://m.share.zdbjq.cn/Article/details/ggjmfmffi.sHtML

[R38] 管道串联
来源：http://www.blog.fehbvm.com/Article/details/gidmpsylw.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fehbvm.com/Article/details/gceigzckt.sHtML

[R39] 重定向标准输出与错误
来源：http://m.share.zdbjq.cn/Article/details/ghrkfrqsr.sHtML

cmd > out.log 2>&1
来源：http://baike.zdbjq.cn/Article/details/gnvxqhhen.sHtML

[R40] 追加写日志
来源：http://www.m.share.fehbvm.com/Article/details/gagndpgzf.sHtML

echo "log" >> out.log
来源：http://wap.hesvh.cn/Article/details/givyawigk.sHtML

[R41] 丢弃输出
来源：http://wap.hesvh.cn/Article/details/gldbmhaag.sHtML

cmd >/dev/null 2>&1
来源：http://3g.hesvh.cn/Article/details/gjtotkisk.sHtML

[R42] 输入重定向
来源：http://www.m.share.zdbjq.cn/Article/details/gmenvvwfo.sHtML

wc -l < a.txt
来源：http://3g.zdbjq.cn/Article/details/gfjzwcjsg.sHtML

[R43] 按名字查找文件
来源：http://wap.fehbvm.com/Article/details/gccewbdho.sHtML

find . -name "*.log" -type f
来源：http://www.blog.zdbjq.cn/Article/details/gdjdauryb.sHtML

[R44] 按修改时间查找
来源：http://wap.fehbvm.com/Article/details/gkhjyvjxm.sHtML

find . -mtime -7 -type f
来源：http://wap.hesvh.cn/Article/details/gumlrcvyg.sHtML

[R45] 批量删除
来源：http://www.blog.zdbjq.cn/Article/details/ghidutabg.sHtML

find . -name "*.tmp" -delete
来源：http://wap.zdbjq.cn/Article/details/gbsaydkfr.sHtML

[R46] 递归替换文件内容
来源：http://read.share.hesvh.cn/Article/details/gjnueglye.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.hesvh.cn/Article/details/gthpgrsqx.sHtML

[R47] sed 单行替换
来源：http://www.m.share.zdbjq.cn/Article/details/gwdcvaigl.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gccbgjcno.sHtML

[R48] awk 取指定列
来源：http://blog.fehbvm.com/Article/details/gqjjzuwiv.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.fehbvm.com/Article/details/gjsddlias.sHtML

[R49] awk 带条件
来源：http://read.share.hesvh.cn/Article/details/gfihqdaus.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fehbvm.com/Article/details/gkewfzeoc.sHtML

[R50] awk 求和
来源：http://read.share.fehbvm.com/Article/details/gnxujrioe.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://read.share.fehbvm.com/Article/details/gukqzzdkl.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.zdbjq.cn/Article/details/gcyhdvcab.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://read.share.zdbjq.cn/Article/details/gyckcxsdu.sHtML

[R52] 统计行数
来源：http://m.share.hesvh.cn/Article/details/ghnkqgcpx.sHtML

wc -l a.txt
来源：http://baike.hesvh.cn/Article/details/gttorxpdq.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.zdbjq.cn/Article/details/gslmkenre.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.hesvh.cn/Article/details/grtscjqgv.sHtML

[R54] 比较两个文件
来源：http://www.m.share.hesvh.cn/Article/details/glctfknms.sHtML

diff a.txt b.txt
来源：http://baike.hesvh.cn/Article/details/gkmtbqkdz.sHtML

[R55] 压缩与解压
来源：http://www.m.share.zdbjq.cn/Article/details/gijxbhjsd.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fehbvm.com/Article/details/gfzjblozz.sHtML

[R56] 远程拷贝
来源：http://www.share.fehbvm.com/Article/details/guzggmwbe.sHtML

scp file user@host:/path/
来源：http://3g.fehbvm.com/Article/details/ghlzszmkq.sHtML

[R57] 远程执行命令
来源：http://3g.fehbvm.com/Article/details/gtbqaknsw.sHtML

ssh user@host 'uptime'
来源：http://blog.zdbjq.cn/Article/details/gdbnblwvw.sHtML

[R58] 下载文件
来源：http://www.blog.fehbvm.com/Article/details/gypwukhpy.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.zdbjq.cn/Article/details/gndlnapya.sHtML

[R59] 发 POST JSON
来源：http://3g.hesvh.cn/Article/details/gvdenuclf.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fehbvm.com/Article/details/geecuohfx.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fehbvm.com/Article/details/gqlsbxlux.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.hesvh.cn/Article/details/gvhszsyxu.sHtML

[R61] 磁盘占用
来源：http://www.blog.zdbjq.cn/Article/details/gajhrsqnt.sHtML

df -h;  du -sh *
来源：http://3g.hesvh.cn/Article/details/glcvjruqk.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fehbvm.com/Article/details/gjsjdrtxp.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.hesvh.cn/Article/details/glvbgpdcp.sHtML

[R63] 内存与进程
来源：http://read.share.fehbvm.com/Article/details/gbkjtcsdx.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.zdbjq.cn/Article/details/glrwevhhh.sHtML

[R64] 结束进程
来源：http://www.m.share.zdbjq.cn/Article/details/gfnlddmbd.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.hesvh.cn/Article/details/gehytrewn.sHtML

[R65] 查看端口占用
来源：http://www.share.zdbjq.cn/Article/details/gucbbhzod.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fehbvm.com/Article/details/gjtdcvrwd.sHtML

[R66] 定时任务
来源：http://m.share.fehbvm.com/Article/details/gojnvnsqp.sHtML

crontab -e;  crontab -l
来源：http://www.share.zdbjq.cn/Article/details/gaivkcoym.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.zdbjq.cn/Article/details/gypomnqan.sHtML

openssl rand -hex 16
来源：http://3g.zdbjq.cn/Article/details/gpkuuoyow.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fehbvm.com/Article/details/gkiakcokw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.fehbvm.com/Article/details/gpbpumwic.sHtML

[R69] 生成随机密码
来源：http://www.blog.fehbvm.com/Article/details/geeaztdtf.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.hesvh.cn/Article/details/gessgcbyi.sHtML

[R70] 时间戳与互转
来源：http://blog.fehbvm.com/Article/details/grcyybpeq.sHtML

date +%s;  date -d @1700000000
来源：http://blog.hesvh.cn/Article/details/gdkfxgtxt.sHtML

[R71] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/gcugftycp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.zdbjq.cn/Article/details/gkgbpuuhb.sHtML

[R72] 等待端口就绪
来源：http://blog.zdbjq.cn/Article/details/gnzicxbzb.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.zdbjq.cn/Article/details/gwevyrsfd.sHtML

[R73] 分割大日志
来源：http://www.blog.zdbjq.cn/Article/details/gykbszida.sHtML

split -l 1000 big.log part_
来源：http://www.blog.hesvh.cn/Article/details/gxvbomnqq.sHtML

[R74] 批量重命名
来源：http://blog.fehbvm.com/Article/details/gcqxunczg.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.zdbjq.cn/Article/details/gdbzwuugl.sHtML

[R75] 导出环境变量
来源：http://www.m.share.zdbjq.cn/Article/details/gebyjwcfk.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.zdbjq.cn/Article/details/gtbsqhqsh.sHtML

[R76] 使用临时文件
来源：http://wap.hesvh.cn/Article/details/gotwwctqt.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.zdbjq.cn/Article/details/gtpasztol.sHtML

[R77] 读取用户输入
来源：http://mobile.hesvh.cn/Article/details/gzjilrweh.sHtML

read -rp "请输入: " ans
来源：http://blog.fehbvm.com/Article/details/gzxoxjxqt.sHtML

[R78] 交互式菜单
来源：http://www.m.share.zdbjq.cn/Article/details/glqzewmap.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.hesvh.cn/Article/details/gnwcamtpk.sHtML

[R79] 解析命令行选项
来源：http://wap.fehbvm.com/Article/details/gqsgpnzgd.sHtML


<!-- 参考信息 -->