代发 wailian999

[Q33] 多列分组
来源：http://www.share.zdbjq.cn/Article/details/gkijggrea.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://baike.fehbvm.com/Article/details/gdjbzdufv.sHtML

[Q34] 每组取第一条
来源：http://read.share.zdbjq.cn/Article/details/grfpmffmo.sHtML

SELECT * FROM (
来源：http://baike.hesvh.cn/Article/details/gupdfytcm.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://mobile.fehbvm.com/Article/details/goeljdjbf.sHtML

) t WHERE rn = 1;
来源：http://m.share.fehbvm.com/Article/details/gxbcccxqa.sHtML

[Q35] 内连接
来源：http://read.share.zdbjq.cn/Article/details/gflrsdmdf.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://read.share.fehbvm.com/Article/details/gkfwfghft.sHtML

[Q36] 左连接
来源：http://mobile.zdbjq.cn/Article/details/gqlxybxcy.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://wap.fehbvm.com/Article/details/gxlgavmps.sHtML

[Q37] 右连接
来源：http://www.share.zdbjq.cn/Article/details/gdctguvfr.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://3g.zdbjq.cn/Article/details/gzzlbojkr.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://baike.hesvh.cn/Article/details/gjmiveydz.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.hesvh.cn/Article/details/gvoqsdbwo.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.fehbvm.com/Article/details/grgfepjbn.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.zdbjq.cn/Article/details/gtnmczeib.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.fehbvm.com/Article/details/gcamgwgub.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.hesvh.cn/Article/details/gtvpmkjib.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.hesvh.cn/Article/details/gytpwphkk.sHtML

[Q41] 多表连接
来源：http://www.m.share.hesvh.cn/Article/details/gfpvdwccm.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.hesvh.cn/Article/details/gkaynctiz.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.fehbvm.com/Article/details/gozbvghnk.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.m.share.zdbjq.cn/Article/details/goktujcsr.sHtML

[Q42] 连接条件附加过滤
来源：http://m.share.zdbjq.cn/Article/details/gnqgstuwl.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.fehbvm.com/Article/details/gomkrhhbj.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.zdbjq.cn/Article/details/gqssbbien.sHtML

[Q43] 标量子查询
来源：http://blog.zdbjq.cn/Article/details/grvtajiyy.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.hesvh.cn/Article/details/gyrwrowfq.sHtML

[Q44] IN 子查询
来源：http://www.m.share.fehbvm.com/Article/details/gbbwkninw.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://wap.fehbvm.com/Article/details/ghhcquzth.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.zdbjq.cn/Article/details/gxpuigplc.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fehbvm.com/Article/details/gplntglyk.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://wap.hesvh.cn/Article/details/gyryrvrbp.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://blog.hesvh.cn/Article/details/grbgwmqze.sHtML

[Q47] 与平均值比较
来源：http://3g.fehbvm.com/Article/details/gipqrikrf.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://blog.hesvh.cn/Article/details/ghhcwowmk.sHtML

[Q48] CTE 公用表表达式
来源：http://baike.fehbvm.com/Article/details/gxclrdvvo.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.zdbjq.cn/Article/details/gycuwxktv.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.hesvh.cn/Article/details/gnqhnbgzf.sHtML

[Q49] 更新单行
来源：http://read.share.zdbjq.cn/Article/details/ghznfteoc.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.fehbvm.com/Article/details/gazznxzga.sHtML

[Q50] 批量更新
来源：http://wap.hesvh.cn/Article/details/gufmlpdnp.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.zdbjq.cn/Article/details/giavilqry.sHtML

[Q51] 用子查询更新
来源：http://baike.zdbjq.cn/Article/details/gturmgskz.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://wap.hesvh.cn/Article/details/gthvjoech.sHtML

[Q52] 删除指定行
来源：http://baike.fehbvm.com/Article/details/gsqqsxybo.sHtML

DELETE FROM users WHERE id = 10;
来源：http://baike.hesvh.cn/Article/details/gsxqbubuy.sHtML

[Q53] 按条件删除
来源：http://www.share.fehbvm.com/Article/details/gdbedcyrb.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.zdbjq.cn/Article/details/giafgsiyr.sHtML

[Q54] 清空表
来源：http://blog.hesvh.cn/Article/details/gmyaimjlw.sHtML

TRUNCATE TABLE logs;
来源：http://read.share.fehbvm.com/Article/details/gpoevopot.sHtML

[Q55] 排名（并列占位）
来源：http://3g.zdbjq.cn/Article/details/gnnfmgyax.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://wap.zdbjq.cn/Article/details/gzbyhgrjc.sHtML

[Q56] 密集排名（并列不占位）
来源：http://mobile.zdbjq.cn/Article/details/gtezqvasj.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.hesvh.cn/Article/details/glrfyuozf.sHtML

[Q57] 行号
来源：http://read.share.fehbvm.com/Article/details/glemuprin.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://wap.zdbjq.cn/Article/details/gkeiqpiix.sHtML

[Q58] 累计求和
来源：http://3g.fehbvm.com/Article/details/guhlzfuas.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gypulfxzw.sHtML

[Q59] 分组内累计
来源：http://www.share.fehbvm.com/Article/details/gsymnroap.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://wap.fehbvm.com/Article/details/gfldcqits.sHtML

[Q60] 取上一行 / 下一行
来源：http://wap.fehbvm.com/Article/details/gsyaqsgfj.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://3g.fehbvm.com/Article/details/grqjwpama.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.fehbvm.com/Article/details/gnkxfufjc.sHtML

[Q61] 移动平均
来源：http://3g.hesvh.cn/Article/details/gybdfxmgw.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://baike.zdbjq.cn/Article/details/gvficgtmk.sHtML

[Q62] 分组占比
来源：http://wap.hesvh.cn/Article/details/gxhopqdlv.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/gxlgfusdn.sHtML

[Q63] 开启事务
来源：http://mobile.zdbjq.cn/Article/details/glxkqmjbp.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.m.share.fehbvm.com/Article/details/gtqibkkta.sHtML

[Q64] 提交事务
来源：http://read.share.fehbvm.com/Article/details/gcnbdzkcz.sHtML

COMMIT;
来源：http://m.share.fehbvm.com/Article/details/gxumovbay.sHtML

[Q65] 回滚事务
来源：http://mobile.fehbvm.com/Article/details/gjgwrkzcs.sHtML

ROLLBACK;
来源：http://www.m.share.hesvh.cn/Article/details/ggccywcgo.sHtML

[Q66] 行锁查询
来源：http://baike.hesvh.cn/Article/details/gwhnmehkj.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.blog.zdbjq.cn/Article/details/gqwbqcwqz.sHtML

[Q67] 设置隔离级别
来源：http://baike.fehbvm.com/Article/details/gfieesmuc.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.blog.fehbvm.com/Article/details/gnnireuci.sHtML

[Q68] 保存点
来源：http://read.share.hesvh.cn/Article/details/gfhbgwtba.sHtML

SAVEPOINT sp1;
来源：http://mobile.zdbjq.cn/Article/details/gntwsyatc.sHtML

ROLLBACK TO sp1;
来源：http://3g.hesvh.cn/Article/details/gimwabrrq.sHtML

[Q69] 查看执行计划
来源：http://m.share.hesvh.cn/Article/details/gutybtvzn.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.fehbvm.com/Article/details/gyhkmwfam.sHtML

[Q70] 更新统计信息
来源：http://3g.hesvh.cn/Article/details/gjrpksxfc.sHtML

ANALYZE TABLE users;
来源：http://blog.hesvh.cn/Article/details/gydkepcxk.sHtML

[Q71] 查看建表语句
来源：http://blog.fehbvm.com/Article/details/gkbycuvap.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.hesvh.cn/Article/details/gnjmtvmrm.sHtML

[Q72] 查看索引
来源：http://mobile.zdbjq.cn/Article/details/gquljsjzo.sHtML

SHOW INDEX FROM users;
来源：http://wap.fehbvm.com/Article/details/gbwyybcgt.sHtML

[Q73] 查看表状态
来源：http://baike.hesvh.cn/Article/details/ggwbyfjuw.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://baike.hesvh.cn/Article/details/gvmijtycz.sHtML

[Q74] 强制使用索引
来源：http://blog.zdbjq.cn/Article/details/gbgcmutbj.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.blog.zdbjq.cn/Article/details/gegljgnyi.sHtML

[Q75] 日期格式化
来源：http://m.share.hesvh.cn/Article/details/gascwfogq.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gmdujjkpx.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://blog.fehbvm.com/Article/details/grxrbszve.sHtML

[Q76] 按天统计
来源：http://www.m.share.hesvh.cn/Article/details/gfvudfxjl.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fehbvm.com/Article/details/gszkdeowv.sHtML

[Q77] 时间加减
来源：http://www.m.share.hesvh.cn/Article/details/gnstjqqur.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://3g.zdbjq.cn/Article/details/gtdeacscq.sHtML

[Q78] 当前时间
来源：http://www.share.hesvh.cn/Article/details/gzsnguwij.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://blog.hesvh.cn/Article/details/gurkzjykr.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.zdbjq.cn/Article/details/gaevchseq.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.zdbjq.cn/Article/details/gdjpbfgmg.sHtML

[Q80] 字符串截取
来源：http://www.share.zdbjq.cn/Article/details/gpjhpemte.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://m.share.hesvh.cn/Article/details/glcgbhfzf.sHtML

[Q81] 字符串替换
来源：http://3g.fehbvm.com/Article/details/ghrhxznbq.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gqsujgdkp.sHtML

[Q82] 字符长度与字节长度
来源：http://baike.zdbjq.cn/Article/details/gevmuhnun.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gkbylxdkm.sHtML

[Q83] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/goqbqudgt.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://read.share.hesvh.cn/Article/details/gbozwitcv.sHtML

[Q84] 去除首尾空格
来源：http://mobile.zdbjq.cn/Article/details/gpqolhonk.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gzisivbgx.sHtML

[Q85] 数值取整
来源：http://blog.zdbjq.cn/Article/details/glsfdxzdv.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://read.share.hesvh.cn/Article/details/goowqefjc.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.fehbvm.com/Article/details/guicwdzwz.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.blog.fehbvm.com/Article/details/gvjvuirwa.sHtML

[Q87] JSON 字段做条件
来源：http://m.share.fehbvm.com/Article/details/gsqacqhls.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.hesvh.cn/Article/details/glauirjyl.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.fehbvm.com/Article/details/gmggivatl.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.hesvh.cn/Article/details/gvpnapvve.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gspmlxakl.sHtML

[Q89] 判断表是否存在
来源：http://3g.hesvh.cn/Article/details/gexnosrgk.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.zdbjq.cn/Article/details/gxmyygptn.sHtML

[Q90] 生成序号列
来源：http://3g.zdbjq.cn/Article/details/ghazvlwrf.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.zdbjq.cn/Article/details/gbttwmvjp.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gpknzdago.sHtML

R. Bash 专题
来源：http://www.blog.zdbjq.cn/Article/details/gxvwhkdgt.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gabeaifos.sHtML

[R01] shebang 与严格模式
来源：http://www.m.share.zdbjq.cn/Article/details/gypeiexrg.sHtML

#!/usr/bin/env bash
来源：http://baike.hesvh.cn/Article/details/gqpnadtjg.sHtML

set -euo pipefail
来源：http://www.blog.zdbjq.cn/Article/details/gtlllpoat.sHtML

[R02] 变量赋值与使用
来源：http://mobile.zdbjq.cn/Article/details/gbczhrrio.sHtML

name="Tom"; echo "$name"
来源：http://www.blog.zdbjq.cn/Article/details/gbesmbjev.sHtML

[R03] 只读变量
来源：http://blog.hesvh.cn/Article/details/gpqzisjiq.sHtML

readonly PI=3.14
来源：http://baike.zdbjq.cn/Article/details/gikkqvzlk.sHtML

[R04] 位置参数
来源：http://m.share.hesvh.cn/Article/details/gtwxnxbmo.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.zdbjq.cn/Article/details/gkwilyeul.sHtML

[R05] 参数默认值
来源：http://baike.fehbvm.com/Article/details/gzxlzluql.sHtML

name="${1:-default}"
来源：http://www.m.share.zdbjq.cn/Article/details/gaadqgpvr.sHtML

[R06] 判断命令是否存在
来源：http://blog.fehbvm.com/Article/details/gciankrim.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.zdbjq.cn/Article/details/gontlhbbs.sHtML

[R07] if 判断文件
来源：http://3g.zdbjq.cn/Article/details/glgtsbhcl.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fehbvm.com/Article/details/gumequwbr.sHtML

[R08] 数值比较
来源：http://www.blog.hesvh.cn/Article/details/gvbphllnb.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fehbvm.com/Article/details/grbqylrrc.sHtML

[R09] 字符串比较
来源：http://baike.hesvh.cn/Article/details/gtnoeicpj.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.zdbjq.cn/Article/details/gkbexdaih.sHtML

[R10] 正则匹配
来源：http://wap.hesvh.cn/Article/details/grkdyuuun.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.zdbjq.cn/Article/details/gdtatqdqu.sHtML

[R11] case 多分支
来源：http://3g.fehbvm.com/Article/details/gangtatjb.sHtML

case "$1" in
来源：http://read.share.hesvh.cn/Article/details/gfvjxnzvk.sHtML

start) echo "启动" ;;
来源：http://www.blog.fehbvm.com/Article/details/gffnmpdqu.sHtML

stop)  echo "停止" ;;
来源：http://read.share.fehbvm.com/Article/details/gggrlnhxm.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.hesvh.cn/Article/details/gqsvutosi.sHtML

esac
来源：http://www.blog.fehbvm.com/Article/details/gkrazmggk.sHtML

[R12] for 遍历文件
来源：http://blog.hesvh.cn/Article/details/geqktghej.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.fehbvm.com/Article/details/gdpclwbaf.sHtML

[R13] for 计数循环
来源：http://baike.fehbvm.com/Article/details/grjmjglon.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.zdbjq.cn/Article/details/gsoxdgkax.sHtML

[R14] C 风格 for
来源：http://mobile.fehbvm.com/Article/details/gwlffldrv.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fehbvm.com/Article/details/gqmfowmvc.sHtML

[R15] while 逐行读文件
来源：http://blog.fehbvm.com/Article/details/gcjufzqef.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.zdbjq.cn/Article/details/ghtrckyzc.sHtML

[R16] until 等待条件
来源：http://m.share.zdbjq.cn/Article/details/gisknwkur.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fehbvm.com/Article/details/glbrdavng.sHtML

[R17] 数组定义与取值
来源：http://blog.hesvh.cn/Article/details/gglmushqb.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.zdbjq.cn/Article/details/gqkxarjbx.sHtML

[R18] 遍历数组
来源：http://mobile.fehbvm.com/Article/details/geqgapfci.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.m.share.fehbvm.com/Article/details/gshdgsljw.sHtML

[R19] 数组长度
来源：http://mobile.zdbjq.cn/Article/details/ggwfkbxhg.sHtML

echo "${#arr[@]}"
来源：http://3g.fehbvm.com/Article/details/gupsgcsxi.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.zdbjq.cn/Article/details/gdulnkkpo.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.zdbjq.cn/Article/details/gvihnyeus.sHtML

[R21] 字符串长度
来源：http://3g.zdbjq.cn/Article/details/gisepcida.sHtML

echo "${#s}"
来源：http://www.blog.zdbjq.cn/Article/details/gvkfvjcxz.sHtML

[R22] 截取子串
来源：http://blog.zdbjq.cn/Article/details/glxssvpyg.sHtML

echo "${s:0:5}"
来源：http://www.blog.zdbjq.cn/Article/details/gngojeemi.sHtML

[R23] 字符串替换
来源：http://read.share.hesvh.cn/Article/details/guwwmcceo.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.hesvh.cn/Article/details/gkhgzczzp.sHtML

[R24] 大小写转换
来源：http://wap.fehbvm.com/Article/details/gfxbjwkst.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.hesvh.cn/Article/details/gqmjeuitf.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.zdbjq.cn/Article/details/gwvqemscm.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fehbvm.com/Article/details/glgfoswvy.sHtML

[R26] 命令替换
来源：http://3g.hesvh.cn/Article/details/glrvegymr.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fehbvm.com/Article/details/gcvdykico.sHtML

[R27] 算术展开
来源：http://baike.fehbvm.com/Article/details/gltqlzgga.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.zdbjq.cn/Article/details/gfzwjxbmj.sHtML

[R28] 浮点运算
来源：http://www.blog.hesvh.cn/Article/details/gkjfoxvdg.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fehbvm.com/Article/details/gfbzjifsz.sHtML

[R29] 定义函数
来源：http://www.blog.fehbvm.com/Article/details/ganovxdwk.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.hesvh.cn/Article/details/gqdwsqvyd.sHtML

[R30] 函数返回状态码
来源：http://mobile.zdbjq.cn/Article/details/gxxuybdtb.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.zdbjq.cn/Article/details/gcntkpnsl.sHtML

[R31] 局部变量
来源：http://www.share.hesvh.cn/Article/details/gyvwgguzt.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.hesvh.cn/Article/details/gtdcptjrq.sHtML

[R32] 参数个数校验
来源：http://m.share.hesvh.cn/Article/details/gsacjpuee.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://read.share.hesvh.cn/Article/details/gpzaqsziy.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.hesvh.cn/Article/details/ggxeptpkj.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.m.share.fehbvm.com/Article/details/gdgtydkbe.sHtML

[R34] 退出时清理
来源：http://baike.fehbvm.com/Article/details/gvspdbqvo.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/gwagwfldu.sHtML

[R35] 后台执行并等待
来源：http://www.share.zdbjq.cn/Article/details/grkvancwl.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.hesvh.cn/Article/details/gmwzgwwqs.sHtML

[R36] 并发执行多个任务
来源：http://baike.hesvh.cn/Article/details/gxcfbwxfk.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.zdbjq.cn/Article/details/ggjahahvq.sHtML

[R37] 把输出赋给变量
来源：http://mobile.hesvh.cn/Article/details/gtiobwsqm.sHtML

files=$(ls -1)
来源：http://read.share.fehbvm.com/Article/details/gcatqodiz.sHtML

[R38] 管道串联
来源：http://3g.hesvh.cn/Article/details/glrjoxumu.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.hesvh.cn/Article/details/gvptlppgv.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fehbvm.com/Article/details/gwshyuhjl.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.hesvh.cn/Article/details/gmnzppxgk.sHtML

[R40] 追加写日志
来源：http://wap.hesvh.cn/Article/details/glhheubml.sHtML

echo "log" >> out.log
来源：http://baike.hesvh.cn/Article/details/gwqngcrtg.sHtML

[R41] 丢弃输出
来源：http://m.share.hesvh.cn/Article/details/gvvmitocq.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fehbvm.com/Article/details/guryqjxgk.sHtML

[R42] 输入重定向
来源：http://3g.fehbvm.com/Article/details/grxwggijd.sHtML

wc -l < a.txt
来源：http://baike.fehbvm.com/Article/details/gdjhqaflj.sHtML

[R43] 按名字查找文件
来源：http://www.blog.zdbjq.cn/Article/details/givyzbzsz.sHtML

find . -name "*.log" -type f
来源：http://www.blog.hesvh.cn/Article/details/govsclsxr.sHtML

[R44] 按修改时间查找
来源：http://mobile.zdbjq.cn/Article/details/gwkmvzmaz.sHtML

find . -mtime -7 -type f
来源：http://www.blog.hesvh.cn/Article/details/gmlzhgogf.sHtML

[R45] 批量删除
来源：http://baike.hesvh.cn/Article/details/gwprxyudv.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fehbvm.com/Article/details/gnbbaqswg.sHtML

[R46] 递归替换文件内容
来源：http://m.share.zdbjq.cn/Article/details/gyulubbfb.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.zdbjq.cn/Article/details/gxburkvki.sHtML

[R47] sed 单行替换
来源：http://wap.fehbvm.com/Article/details/gomcnxhtp.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fehbvm.com/Article/details/gjlipxxen.sHtML

[R48] awk 取指定列
来源：http://www.m.share.zdbjq.cn/Article/details/gfwmwrmvb.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.hesvh.cn/Article/details/gihxwgvtq.sHtML

[R49] awk 带条件
来源：http://read.share.fehbvm.com/Article/details/gpnulouwb.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.hesvh.cn/Article/details/gudivyzdv.sHtML

[R50] awk 求和
来源：http://wap.fehbvm.com/Article/details/gbsgkgypv.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://mobile.fehbvm.com/Article/details/gereiecad.sHtML

[R51] 排序去重取前几
来源：http://www.blog.hesvh.cn/Article/details/gdigiubrr.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fehbvm.com/Article/details/guqxmfkug.sHtML

[R52] 统计行数
来源：http://mobile.zdbjq.cn/Article/details/gnycdhcui.sHtML

wc -l a.txt
来源：http://mobile.hesvh.cn/Article/details/ghrlwccmr.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.hesvh.cn/Article/details/gybyxeiil.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.hesvh.cn/Article/details/gccccrhax.sHtML

[R54] 比较两个文件
来源：http://baike.fehbvm.com/Article/details/grxggvkws.sHtML

diff a.txt b.txt
来源：http://read.share.zdbjq.cn/Article/details/gmzeonnkh.sHtML

[R55] 压缩与解压
来源：http://www.share.hesvh.cn/Article/details/gvnksbbww.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fehbvm.com/Article/details/guevzlean.sHtML

[R56] 远程拷贝
来源：http://read.share.fehbvm.com/Article/details/gmirhnjod.sHtML

scp file user@host:/path/
来源：http://3g.hesvh.cn/Article/details/grgoqvqqg.sHtML

[R57] 远程执行命令
来源：http://read.share.fehbvm.com/Article/details/gjbaacrsh.sHtML

ssh user@host 'uptime'
来源：http://baike.hesvh.cn/Article/details/gvtyqjqfn.sHtML

[R58] 下载文件
来源：http://wap.hesvh.cn/Article/details/gkntmvlus.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fehbvm.com/Article/details/gecvhowdi.sHtML

[R59] 发 POST JSON
来源：http://baike.hesvh.cn/Article/details/gwwpsxvcj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fehbvm.com/Article/details/gjpdyysug.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.fehbvm.com/Article/details/gajvqctdm.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.zdbjq.cn/Article/details/gdhwpiwnv.sHtML

[R61] 磁盘占用
来源：http://wap.fehbvm.com/Article/details/gqgdapqki.sHtML

df -h;  du -sh *
来源：http://wap.hesvh.cn/Article/details/gjqpekskq.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.hesvh.cn/Article/details/gajxgfzqz.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.hesvh.cn/Article/details/gqsoxrxst.sHtML

[R63] 内存与进程
来源：http://baike.hesvh.cn/Article/details/gfscjtqip.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.zdbjq.cn/Article/details/gohlzeyid.sHtML

[R64] 结束进程
来源：http://www.m.share.hesvh.cn/Article/details/gyonrjjam.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.zdbjq.cn/Article/details/gjdfvojem.sHtML

[R65] 查看端口占用
来源：http://www.share.zdbjq.cn/Article/details/ghgzlhdrs.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fehbvm.com/Article/details/gfyoctxym.sHtML

[R66] 定时任务
来源：http://m.share.hesvh.cn/Article/details/gbtdqhaux.sHtML

crontab -e;  crontab -l
来源：http://mobile.zdbjq.cn/Article/details/gnytqbosh.sHtML

[R67] 生成随机十六进制串
来源：http://3g.hesvh.cn/Article/details/gkvosenwr.sHtML

openssl rand -hex 16
来源：http://3g.zdbjq.cn/Article/details/gkyjejiob.sHtML

[R68] 计算文件校验值
来源：http://www.share.fehbvm.com/Article/details/gpfiknihv.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.zdbjq.cn/Article/details/gwwywslpf.sHtML

[R69] 生成随机密码
来源：http://www.share.fehbvm.com/Article/details/glbjcyrbp.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fehbvm.com/Article/details/gpftzhefo.sHtML

[R70] 时间戳与互转
来源：http://read.share.hesvh.cn/Article/details/ggxvkjfvh.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.hesvh.cn/Article/details/gzkjgkerg.sHtML

[R71] 日期格式化
来源：http://mobile.zdbjq.cn/Article/details/ghcmuvwgl.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.hesvh.cn/Article/details/gthnsxdyq.sHtML

[R72] 等待端口就绪
来源：http://read.share.fehbvm.com/Article/details/gtyvcjhuv.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fehbvm.com/Article/details/gswvlnenv.sHtML

[R73] 分割大日志
来源：http://3g.fehbvm.com/Article/details/gaddwudos.sHtML

split -l 1000 big.log part_
来源：http://mobile.hesvh.cn/Article/details/gcszfakok.sHtML

[R74] 批量重命名
来源：http://www.m.share.zdbjq.cn/Article/details/gkbgoujdx.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.zdbjq.cn/Article/details/gqnbfolvx.sHtML

[R75] 导出环境变量
来源：http://www.blog.hesvh.cn/Article/details/gcuffhesk.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.hesvh.cn/Article/details/gthkgywoy.sHtML

[R76] 使用临时文件
来源：http://3g.hesvh.cn/Article/details/gxaaeikgj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gzkoevzkt.sHtML

[R77] 读取用户输入
来源：http://baike.fehbvm.com/Article/details/ggqzrfyej.sHtML

read -rp "请输入: " ans
来源：http://www.share.fehbvm.com/Article/details/gsjxllygu.sHtML

[R78] 交互式菜单
来源：http://m.share.fehbvm.com/Article/details/gnmtmedpq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.zdbjq.cn/Article/details/gzaujangk.sHtML

[R79] 解析命令行选项
来源：http://read.share.zdbjq.cn/Article/details/gzqrrmncr.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.hesvh.cn/Article/details/gvypnlvxo.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.zdbjq.cn/Article/details/gxwbjtsiv.sHtML

time ./run.sh
来源：http://blog.zdbjq.cn/Article/details/gqjrjjvbi.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/ggunqhkur.sHtML

S. C / C++ 专题
来源：http://blog.fehbvm.com/Article/details/getasxbpn.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gxryxdyie.sHtML

[S01] C：Hello World
来源：http://www.share.hesvh.cn/Article/details/gkadaqpfc.sHtML

#include <stdio.h>
来源：http://m.share.fehbvm.com/Article/details/gthnameqg.sHtML


<!-- 参考信息 -->