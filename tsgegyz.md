代发 wailian999

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.fehbvm.com/Article/details/giaiauijb.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.fehbvm.com/Article/details/gqfaobhik.sHtML

[Q39] 自连接（查上下级）
来源：http://read.share.zdbjq.cn/Article/details/gdjwajpul.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.hesvh.cn/Article/details/gmuiwyuxz.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.fehbvm.com/Article/details/gkvatdaon.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.fehbvm.com/Article/details/gzyxbfnaw.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.hesvh.cn/Article/details/gnzhpytab.sHtML

[Q41] 多表连接
来源：http://read.share.fehbvm.com/Article/details/gwjuprldi.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://blog.zdbjq.cn/Article/details/gqkjijkyi.sHtML

JOIN users u ON u.id = o.user_id
来源：http://mobile.fehbvm.com/Article/details/godbaabdg.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.fehbvm.com/Article/details/grgiscscw.sHtML

[Q42] 连接条件附加过滤
来源：http://www.share.zdbjq.cn/Article/details/gzoxllzsb.sHtML

SELECT u.name, o.amount FROM users u
来源：http://3g.fehbvm.com/Article/details/gcjcwbpsa.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.hesvh.cn/Article/details/gqzwoittk.sHtML

[Q43] 标量子查询
来源：http://read.share.fehbvm.com/Article/details/ggheumpnq.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://blog.hesvh.cn/Article/details/geuihvrfl.sHtML

[Q44] IN 子查询
来源：http://read.share.hesvh.cn/Article/details/gbntotysa.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.fehbvm.com/Article/details/gaowrtrhb.sHtML

[Q45] EXISTS 判断存在
来源：http://www.share.hesvh.cn/Article/details/gxmkcpahf.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.zdbjq.cn/Article/details/gtpgcqkxk.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.zdbjq.cn/Article/details/gyeyhvjvb.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.zdbjq.cn/Article/details/gqmhhigxv.sHtML

[Q47] 与平均值比较
来源：http://3g.hesvh.cn/Article/details/gstmuqvho.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://read.share.fehbvm.com/Article/details/gvumlmqbb.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.hesvh.cn/Article/details/gvgfgknir.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.zdbjq.cn/Article/details/ggigqiyee.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://wap.hesvh.cn/Article/details/gjkumxlqx.sHtML

[Q49] 更新单行
来源：http://m.share.hesvh.cn/Article/details/geoyjnakl.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gozbeqedu.sHtML

[Q50] 批量更新
来源：http://read.share.zdbjq.cn/Article/details/gywelysqy.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://read.share.hesvh.cn/Article/details/gwuvsppev.sHtML

[Q51] 用子查询更新
来源：http://mobile.fehbvm.com/Article/details/gajiqfddm.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.zdbjq.cn/Article/details/ggnqrdzjk.sHtML

[Q52] 删除指定行
来源：http://blog.fehbvm.com/Article/details/gthqqmwvy.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.fehbvm.com/Article/details/gtnhegwqs.sHtML

[Q53] 按条件删除
来源：http://www.share.fehbvm.com/Article/details/giaonueuv.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.zdbjq.cn/Article/details/gojfbckqg.sHtML

[Q54] 清空表
来源：http://www.share.hesvh.cn/Article/details/gpjebaoau.sHtML

TRUNCATE TABLE logs;
来源：http://blog.hesvh.cn/Article/details/gtlisescu.sHtML

[Q55] 排名（并列占位）
来源：http://www.m.share.fehbvm.com/Article/details/gypzadxio.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.hesvh.cn/Article/details/gfqxaqgrl.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.fehbvm.com/Article/details/ggtmmuzxq.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://baike.hesvh.cn/Article/details/gevmreqdi.sHtML

[Q57] 行号
来源：http://blog.zdbjq.cn/Article/details/gpvephcsl.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://blog.zdbjq.cn/Article/details/gqtcinqzp.sHtML

[Q58] 累计求和
来源：http://blog.fehbvm.com/Article/details/gqqoatykl.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://m.share.fehbvm.com/Article/details/gwbbbbduo.sHtML

[Q59] 分组内累计
来源：http://www.blog.zdbjq.cn/Article/details/gigoaundr.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gekprrqta.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.hesvh.cn/Article/details/gejtvylxi.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.zdbjq.cn/Article/details/gnucwvjzn.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://m.share.hesvh.cn/Article/details/gvnycvctj.sHtML

[Q61] 移动平均
来源：http://read.share.fehbvm.com/Article/details/gtldzstrd.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/glnuvsgms.sHtML

[Q62] 分组占比
来源：http://www.m.share.hesvh.cn/Article/details/gqhrinktp.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.fehbvm.com/Article/details/gaueqfxjg.sHtML

[Q63] 开启事务
来源：http://www.blog.fehbvm.com/Article/details/gvhvktrev.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.hesvh.cn/Article/details/gckumqmcq.sHtML

[Q64] 提交事务
来源：http://baike.zdbjq.cn/Article/details/gqxhzqdqa.sHtML

COMMIT;
来源：http://mobile.fehbvm.com/Article/details/gqrvgizgo.sHtML

[Q65] 回滚事务
来源：http://www.share.hesvh.cn/Article/details/gobzhbucn.sHtML

ROLLBACK;
来源：http://www.m.share.fehbvm.com/Article/details/ggemvxajo.sHtML

[Q66] 行锁查询
来源：http://mobile.hesvh.cn/Article/details/gkfuhlftl.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.fehbvm.com/Article/details/gjvfkpqgf.sHtML

[Q67] 设置隔离级别
来源：http://m.share.zdbjq.cn/Article/details/gwnzaprem.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.hesvh.cn/Article/details/gibtylrqo.sHtML

[Q68] 保存点
来源：http://m.share.zdbjq.cn/Article/details/gdjhqnpit.sHtML

SAVEPOINT sp1;
来源：http://read.share.fehbvm.com/Article/details/guojjjrqe.sHtML

ROLLBACK TO sp1;
来源：http://wap.fehbvm.com/Article/details/ggfzvulqf.sHtML

[Q69] 查看执行计划
来源：http://www.blog.zdbjq.cn/Article/details/gxftpyjur.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://mobile.fehbvm.com/Article/details/ggaxqnams.sHtML

[Q70] 更新统计信息
来源：http://m.share.zdbjq.cn/Article/details/gnjtolalq.sHtML

ANALYZE TABLE users;
来源：http://mobile.fehbvm.com/Article/details/gvvrjdnmr.sHtML

[Q71] 查看建表语句
来源：http://blog.hesvh.cn/Article/details/gqizrhess.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.zdbjq.cn/Article/details/gxkjrhzmm.sHtML

[Q72] 查看索引
来源：http://www.share.hesvh.cn/Article/details/gxqnduzcb.sHtML

SHOW INDEX FROM users;
来源：http://3g.hesvh.cn/Article/details/gcpjimvid.sHtML

[Q73] 查看表状态
来源：http://m.share.hesvh.cn/Article/details/gyyzvyamw.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.hesvh.cn/Article/details/gicuhzrxd.sHtML

[Q74] 强制使用索引
来源：http://read.share.hesvh.cn/Article/details/govnjjqcn.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.zdbjq.cn/Article/details/ggcpqsnco.sHtML

[Q75] 日期格式化
来源：http://m.share.hesvh.cn/Article/details/gbzcrhyzl.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.fehbvm.com/Article/details/gzkkcyxep.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.zdbjq.cn/Article/details/gbqkokhov.sHtML

[Q76] 按天统计
来源：http://wap.fehbvm.com/Article/details/gvqigymqj.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.m.share.zdbjq.cn/Article/details/gmswvqzvz.sHtML

[Q77] 时间加减
来源：http://www.blog.zdbjq.cn/Article/details/gyyuqzfng.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.hesvh.cn/Article/details/gvhjxyfcm.sHtML

[Q78] 当前时间
来源：http://www.blog.hesvh.cn/Article/details/gqmtetfcz.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.hesvh.cn/Article/details/gixpsdajc.sHtML

[Q79] 字符串拼接
来源：http://www.share.fehbvm.com/Article/details/ghzchqksn.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.hesvh.cn/Article/details/gobuwlduj.sHtML

[Q80] 字符串截取
来源：http://blog.hesvh.cn/Article/details/gmfsumwtd.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://3g.fehbvm.com/Article/details/gmdicbpaz.sHtML

[Q81] 字符串替换
来源：http://baike.zdbjq.cn/Article/details/gmiasswwj.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.fehbvm.com/Article/details/gogdmpzku.sHtML

[Q82] 字符长度与字节长度
来源：http://www.blog.zdbjq.cn/Article/details/gulszlzwn.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://wap.fehbvm.com/Article/details/gkrlbhhwd.sHtML

[Q83] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/gowwguswf.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gxjzqvyeu.sHtML

[Q84] 去除首尾空格
来源：http://wap.hesvh.cn/Article/details/gcrpyyptk.sHtML

SELECT TRIM(name) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gerugqumf.sHtML

[Q85] 数值取整
来源：http://www.blog.zdbjq.cn/Article/details/gbtmwugyl.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://m.share.zdbjq.cn/Article/details/gjoypsqed.sHtML

[Q86] 读取 JSON 字段
来源：http://www.m.share.hesvh.cn/Article/details/gvsqooeye.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.fehbvm.com/Article/details/guvkvvexp.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fehbvm.com/Article/details/gkrllapfz.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://3g.fehbvm.com/Article/details/gwewltziz.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.hesvh.cn/Article/details/gtnmjwkev.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.hesvh.cn/Article/details/gxixsjtfv.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.zdbjq.cn/Article/details/gxblqdfyy.sHtML

[Q89] 判断表是否存在
来源：http://www.share.hesvh.cn/Article/details/gmdmqkwms.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.zdbjq.cn/Article/details/gghrzzlmc.sHtML

[Q90] 生成序号列
来源：http://wap.fehbvm.com/Article/details/gynsupecj.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.hesvh.cn/Article/details/gicjhsmua.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gaqmgnrmm.sHtML

R. Bash 专题
来源：http://3g.fehbvm.com/Article/details/gzulgywxe.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ghsjwhihp.sHtML

[R01] shebang 与严格模式
来源：http://3g.fehbvm.com/Article/details/giqsmvcbp.sHtML

#!/usr/bin/env bash
来源：http://baike.fehbvm.com/Article/details/gfydzhxea.sHtML

set -euo pipefail
来源：http://www.m.share.zdbjq.cn/Article/details/ggwgxdout.sHtML

[R02] 变量赋值与使用
来源：http://mobile.hesvh.cn/Article/details/gahaypxka.sHtML

name="Tom"; echo "$name"
来源：http://blog.fehbvm.com/Article/details/gipavhkgh.sHtML

[R03] 只读变量
来源：http://m.share.fehbvm.com/Article/details/gjdfxmefe.sHtML

readonly PI=3.14
来源：http://wap.fehbvm.com/Article/details/gdenakwsr.sHtML

[R04] 位置参数
来源：http://www.blog.zdbjq.cn/Article/details/gjlqupsit.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.zdbjq.cn/Article/details/gyldnlfab.sHtML

[R05] 参数默认值
来源：http://wap.zdbjq.cn/Article/details/gnmkozsib.sHtML

name="${1:-default}"
来源：http://baike.zdbjq.cn/Article/details/gexmtdmeg.sHtML

[R06] 判断命令是否存在
来源：http://wap.zdbjq.cn/Article/details/gfiizumjo.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.zdbjq.cn/Article/details/gifddzbkc.sHtML

[R07] if 判断文件
来源：http://blog.hesvh.cn/Article/details/gyzpwmbhj.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.hesvh.cn/Article/details/ghqaxlghi.sHtML

[R08] 数值比较
来源：http://mobile.hesvh.cn/Article/details/gubauoujs.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.fehbvm.com/Article/details/gdoprazbq.sHtML

[R09] 字符串比较
来源：http://www.blog.hesvh.cn/Article/details/gdjxwxhxy.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gqmokggxu.sHtML

[R10] 正则匹配
来源：http://3g.fehbvm.com/Article/details/gupyzrssp.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.hesvh.cn/Article/details/gedeygxdq.sHtML

[R11] case 多分支
来源：http://www.share.zdbjq.cn/Article/details/ggibnsqfu.sHtML

case "$1" in
来源：http://blog.zdbjq.cn/Article/details/gdyuyugul.sHtML

start) echo "启动" ;;
来源：http://baike.fehbvm.com/Article/details/ggcpbnszk.sHtML

stop)  echo "停止" ;;
来源：http://mobile.zdbjq.cn/Article/details/gbeqgmohy.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.hesvh.cn/Article/details/ghusovblp.sHtML

esac
来源：http://wap.hesvh.cn/Article/details/gbnesvcpi.sHtML

[R12] for 遍历文件
来源：http://mobile.hesvh.cn/Article/details/gsncfazzq.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.zdbjq.cn/Article/details/gleqcgxfv.sHtML

[R13] for 计数循环
来源：http://www.m.share.hesvh.cn/Article/details/gawlaauae.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fehbvm.com/Article/details/gaabdnutq.sHtML

[R14] C 风格 for
来源：http://baike.fehbvm.com/Article/details/gwiqzonwt.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fehbvm.com/Article/details/gcwimumry.sHtML

[R15] while 逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gzsazkkyk.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.hesvh.cn/Article/details/gryjmkzmc.sHtML

[R16] until 等待条件
来源：http://3g.zdbjq.cn/Article/details/gssqndxpn.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.zdbjq.cn/Article/details/gqbhctcfk.sHtML

[R17] 数组定义与取值
来源：http://www.share.hesvh.cn/Article/details/glazfgfmg.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.hesvh.cn/Article/details/gsvzpwseo.sHtML

[R18] 遍历数组
来源：http://baike.hesvh.cn/Article/details/gtzedvuue.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.hesvh.cn/Article/details/gdowxlcjz.sHtML

[R19] 数组长度
来源：http://www.m.share.fehbvm.com/Article/details/gpfpjmbcp.sHtML

echo "${#arr[@]}"
来源：http://mobile.zdbjq.cn/Article/details/gqwsqiykd.sHtML

[R20] 关联数组（字典）
来源：http://mobile.hesvh.cn/Article/details/gewutcosr.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://read.share.zdbjq.cn/Article/details/grtowcafi.sHtML

[R21] 字符串长度
来源：http://wap.hesvh.cn/Article/details/ggzfgcgyr.sHtML

echo "${#s}"
来源：http://www.m.share.hesvh.cn/Article/details/gmnuidjii.sHtML

[R22] 截取子串
来源：http://www.m.share.fehbvm.com/Article/details/gglwxxwjw.sHtML

echo "${s:0:5}"
来源：http://wap.hesvh.cn/Article/details/gkxfeocbz.sHtML

[R23] 字符串替换
来源：http://baike.hesvh.cn/Article/details/gwlwlyqtj.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://wap.zdbjq.cn/Article/details/grcgdnhih.sHtML

[R24] 大小写转换
来源：http://blog.hesvh.cn/Article/details/ggyyobfdj.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.hesvh.cn/Article/details/gmxxilqpp.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.hesvh.cn/Article/details/gxuqdksge.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.hesvh.cn/Article/details/gqgznkqpg.sHtML

[R26] 命令替换
来源：http://wap.fehbvm.com/Article/details/gjcpgfmcf.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fehbvm.com/Article/details/gbwnnrlhn.sHtML

[R27] 算术展开
来源：http://wap.zdbjq.cn/Article/details/gqtenbppb.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fehbvm.com/Article/details/glkjsdaoy.sHtML

[R28] 浮点运算
来源：http://mobile.hesvh.cn/Article/details/gbagmhcxa.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.m.share.fehbvm.com/Article/details/gzboxckje.sHtML

[R29] 定义函数
来源：http://wap.fehbvm.com/Article/details/gpzbikvif.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.fehbvm.com/Article/details/gxarojuqz.sHtML

[R30] 函数返回状态码
来源：http://3g.fehbvm.com/Article/details/gqtkhjexy.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.zdbjq.cn/Article/details/gkdjyqtbs.sHtML

[R31] 局部变量
来源：http://mobile.fehbvm.com/Article/details/grezqzhhu.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqcjbxezb.sHtML

[R32] 参数个数校验
来源：http://m.share.zdbjq.cn/Article/details/geteitvzf.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.zdbjq.cn/Article/details/gzuehrizy.sHtML

[R33] 捕获错误并提示行号
来源：http://www.blog.hesvh.cn/Article/details/gqsiuukbm.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fehbvm.com/Article/details/ggesafpzo.sHtML

[R34] 退出时清理
来源：http://wap.hesvh.cn/Article/details/grapwzvsq.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://blog.hesvh.cn/Article/details/gfkshlzmp.sHtML

[R35] 后台执行并等待
来源：http://baike.fehbvm.com/Article/details/gmrakufca.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.fehbvm.com/Article/details/gkmyiwaqc.sHtML

[R36] 并发执行多个任务
来源：http://baike.hesvh.cn/Article/details/giptfxxen.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.zdbjq.cn/Article/details/gqizoowas.sHtML

[R37] 把输出赋给变量
来源：http://wap.zdbjq.cn/Article/details/gwliuaahs.sHtML

files=$(ls -1)
来源：http://www.share.fehbvm.com/Article/details/gvzzmpwtd.sHtML

[R38] 管道串联
来源：http://blog.hesvh.cn/Article/details/gqwjianry.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fehbvm.com/Article/details/grxoaiugs.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.hesvh.cn/Article/details/gyzhxcnzw.sHtML

cmd > out.log 2>&1
来源：http://3g.hesvh.cn/Article/details/gektlixxm.sHtML

[R40] 追加写日志
来源：http://www.m.share.hesvh.cn/Article/details/gblpmuuce.sHtML

echo "log" >> out.log
来源：http://wap.hesvh.cn/Article/details/gaqlbadzd.sHtML

[R41] 丢弃输出
来源：http://www.share.hesvh.cn/Article/details/gelelxyaw.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/gtgawvhwe.sHtML

[R42] 输入重定向
来源：http://mobile.zdbjq.cn/Article/details/gdbjwtukz.sHtML

wc -l < a.txt
来源：http://wap.zdbjq.cn/Article/details/gerysyqwh.sHtML

[R43] 按名字查找文件
来源：http://www.share.zdbjq.cn/Article/details/guonnifvo.sHtML

find . -name "*.log" -type f
来源：http://baike.hesvh.cn/Article/details/gnigmjjeu.sHtML

[R44] 按修改时间查找
来源：http://wap.zdbjq.cn/Article/details/gwfjyqkcj.sHtML

find . -mtime -7 -type f
来源：http://baike.zdbjq.cn/Article/details/geflasydj.sHtML

[R45] 批量删除
来源：http://www.blog.fehbvm.com/Article/details/gyzxhlzbh.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fehbvm.com/Article/details/gpfgmwnbb.sHtML

[R46] 递归替换文件内容
来源：http://blog.hesvh.cn/Article/details/glkeblqzu.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.hesvh.cn/Article/details/ghzjrcrhv.sHtML

[R47] sed 单行替换
来源：http://blog.zdbjq.cn/Article/details/gtmjljwnc.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.zdbjq.cn/Article/details/glfqqqtzc.sHtML

[R48] awk 取指定列
来源：http://www.m.share.fehbvm.com/Article/details/gjladpaod.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.hesvh.cn/Article/details/gcpsvtkfn.sHtML

[R49] awk 带条件
来源：http://read.share.zdbjq.cn/Article/details/grahbdcgf.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.zdbjq.cn/Article/details/glfmraqbz.sHtML

[R50] awk 求和
来源：http://www.blog.zdbjq.cn/Article/details/gruhzlnnh.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.hesvh.cn/Article/details/ggjtaplzf.sHtML

[R51] 排序去重取前几
来源：http://www.blog.hesvh.cn/Article/details/gjpztjgky.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.zdbjq.cn/Article/details/gkcfyeohi.sHtML

[R52] 统计行数
来源：http://baike.hesvh.cn/Article/details/ghuhbciqo.sHtML

wc -l a.txt
来源：http://mobile.fehbvm.com/Article/details/gsoidmycc.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fehbvm.com/Article/details/gfbwmccjp.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fehbvm.com/Article/details/gpxcwndek.sHtML

[R54] 比较两个文件
来源：http://baike.zdbjq.cn/Article/details/giwqoizqu.sHtML

diff a.txt b.txt
来源：http://www.m.share.hesvh.cn/Article/details/gmlikxweb.sHtML

[R55] 压缩与解压
来源：http://m.share.fehbvm.com/Article/details/gkdgknlzs.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.zdbjq.cn/Article/details/gneistvua.sHtML

[R56] 远程拷贝
来源：http://3g.zdbjq.cn/Article/details/ghjuhgxpl.sHtML

scp file user@host:/path/
来源：http://www.blog.fehbvm.com/Article/details/gxyggevqi.sHtML

[R57] 远程执行命令
来源：http://baike.hesvh.cn/Article/details/guyrljfhc.sHtML

ssh user@host 'uptime'
来源：http://mobile.fehbvm.com/Article/details/ghyaizzie.sHtML

[R58] 下载文件
来源：http://m.share.hesvh.cn/Article/details/ggmwyrbhj.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.zdbjq.cn/Article/details/giqlrssvi.sHtML

[R59] 发 POST JSON
来源：http://www.share.zdbjq.cn/Article/details/gbenjdwcn.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fehbvm.com/Article/details/gzukocctq.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.zdbjq.cn/Article/details/gurzvbugg.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.zdbjq.cn/Article/details/gnzgcjdik.sHtML

[R61] 磁盘占用
来源：http://wap.fehbvm.com/Article/details/gyfmmfjtx.sHtML

df -h;  du -sh *
来源：http://baike.hesvh.cn/Article/details/gjasuxdzk.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fehbvm.com/Article/details/gqkahnimf.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.zdbjq.cn/Article/details/gmxewmzkr.sHtML

[R63] 内存与进程
来源：http://www.m.share.fehbvm.com/Article/details/guyrqyjvf.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fehbvm.com/Article/details/gxluybkon.sHtML

[R64] 结束进程
来源：http://www.m.share.zdbjq.cn/Article/details/gmyxmfzoj.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.hesvh.cn/Article/details/gdvsozxhc.sHtML

[R65] 查看端口占用
来源：http://wap.fehbvm.com/Article/details/gbkeaecwb.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.zdbjq.cn/Article/details/gufvuocje.sHtML

[R66] 定时任务
来源：http://wap.hesvh.cn/Article/details/gwrhhfhgy.sHtML

crontab -e;  crontab -l
来源：http://blog.fehbvm.com/Article/details/ggavmhjap.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fehbvm.com/Article/details/ganjdzshq.sHtML

openssl rand -hex 16
来源：http://read.share.hesvh.cn/Article/details/gbrhoxnvv.sHtML

[R68] 计算文件校验值
来源：http://www.blog.hesvh.cn/Article/details/gzeemigoy.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.fehbvm.com/Article/details/gxnshkala.sHtML

[R69] 生成随机密码
来源：http://m.share.hesvh.cn/Article/details/gqxbquxee.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fehbvm.com/Article/details/gtzsewefs.sHtML

[R70] 时间戳与互转
来源：http://m.share.zdbjq.cn/Article/details/gdxhqvfoc.sHtML

date +%s;  date -d @1700000000
来源：http://baike.zdbjq.cn/Article/details/giznptoog.sHtML

[R71] 日期格式化
来源：http://wap.zdbjq.cn/Article/details/gqbwptjbp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.zdbjq.cn/Article/details/gxcwqobit.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fehbvm.com/Article/details/gyabylmsk.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.hesvh.cn/Article/details/gppmqidlg.sHtML

[R73] 分割大日志
来源：http://mobile.zdbjq.cn/Article/details/gvewsuaix.sHtML

split -l 1000 big.log part_
来源：http://baike.zdbjq.cn/Article/details/gkjrjpgye.sHtML

[R74] 批量重命名
来源：http://m.share.fehbvm.com/Article/details/gtfafmojl.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.hesvh.cn/Article/details/gvmqlazkr.sHtML

[R75] 导出环境变量
来源：http://3g.zdbjq.cn/Article/details/gsfhpzdaf.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.fehbvm.com/Article/details/goxpctmmp.sHtML

[R76] 使用临时文件
来源：http://wap.zdbjq.cn/Article/details/gzsrshdll.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gvpnjcfyd.sHtML

[R77] 读取用户输入
来源：http://www.share.zdbjq.cn/Article/details/glphknycq.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.zdbjq.cn/Article/details/gvhtqrfim.sHtML

[R78] 交互式菜单
来源：http://mobile.hesvh.cn/Article/details/ggksegaja.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.hesvh.cn/Article/details/gjncjkspa.sHtML

[R79] 解析命令行选项
来源：http://wap.zdbjq.cn/Article/details/gkcedqxee.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.hesvh.cn/Article/details/grcjeaxtr.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.fehbvm.com/Article/details/giirwvqsj.sHtML

time ./run.sh
来源：http://www.blog.fehbvm.com/Article/details/guhoiusod.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/gxvuarnuy.sHtML

S. C / C++ 专题
来源：http://mobile.zdbjq.cn/Article/details/guvpwqfbl.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gglvkkvcc.sHtML

[S01] C：Hello World
来源：http://wap.fehbvm.com/Article/details/gfkqmrgka.sHtML

#include <stdio.h>
来源：http://mobile.fehbvm.com/Article/details/goqfsnjrz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fehbvm.com/Article/details/gierhubwz.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fehbvm.com/Article/details/ggstoqamj.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.hesvh.cn/Article/details/gklxpnfbh.sHtML

[S03] C：读入整数
来源：http://3g.hesvh.cn/Article/details/grupljdzi.sHtML

int x; scanf("%d", &x);
来源：http://www.share.fehbvm.com/Article/details/gnrbnneke.sHtML

[S04] C：字符串复制
来源：http://3g.hesvh.cn/Article/details/ggrvxwufs.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.hesvh.cn/Article/details/gdjkmchyr.sHtML

[S05] C：字符串长度
来源：http://www.share.zdbjq.cn/Article/details/gibsyhrbz.sHtML

strlen(s)
来源：http://blog.hesvh.cn/Article/details/gbbricdrl.sHtML

[S06] C：字符串比较
来源：http://wap.zdbjq.cn/Article/details/gxucdyvzh.sHtML

strcmp(a, b) == 0
来源：http://blog.zdbjq.cn/Article/details/gjatmkxvz.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fehbvm.com/Article/details/gzvxmzsiu.sHtML


<!-- 参考信息 -->