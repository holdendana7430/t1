代发 wailian999

[Q36] 左连接
来源：http://baike.hesvh.cn/Article/details/gtjqkheeu.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.share.fehbvm.com/Article/details/glujzjrsg.sHtML

[Q37] 右连接
来源：http://baike.hesvh.cn/Article/details/gqckyfnpv.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.zdbjq.cn/Article/details/gyuyymfut.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.hesvh.cn/Article/details/gcjrtrtch.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.hesvh.cn/Article/details/gyuirzecg.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.zdbjq.cn/Article/details/gruaxhrqy.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.blog.hesvh.cn/Article/details/gkmrmdouu.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.zdbjq.cn/Article/details/gtdvxeaxt.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://wap.fehbvm.com/Article/details/gvcrljthk.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.fehbvm.com/Article/details/gbrhyldil.sHtML

[Q41] 多表连接
来源：http://www.m.share.fehbvm.com/Article/details/gawbbiugb.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.blog.fehbvm.com/Article/details/gnchzkqvz.sHtML

JOIN users u ON u.id = o.user_id
来源：http://wap.zdbjq.cn/Article/details/gdgkzczkq.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://blog.hesvh.cn/Article/details/gdydwoulj.sHtML

[Q42] 连接条件附加过滤
来源：http://mobile.hesvh.cn/Article/details/gybdushmm.sHtML

SELECT u.name, o.amount FROM users u
来源：http://wap.zdbjq.cn/Article/details/glscvbibr.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://blog.hesvh.cn/Article/details/gcojvgvqf.sHtML

[Q43] 标量子查询
来源：http://read.share.hesvh.cn/Article/details/gnjhyzicp.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://baike.zdbjq.cn/Article/details/gvmwwjerx.sHtML

[Q44] IN 子查询
来源：http://wap.zdbjq.cn/Article/details/grjjbilvb.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://baike.fehbvm.com/Article/details/gxrmbtdsr.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.hesvh.cn/Article/details/gnzhmuqbb.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.hesvh.cn/Article/details/gvdxzbpqu.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.zdbjq.cn/Article/details/gvguhtyhe.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.fehbvm.com/Article/details/ghglgcwpl.sHtML

[Q47] 与平均值比较
来源：http://mobile.fehbvm.com/Article/details/gondnbbls.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.blog.fehbvm.com/Article/details/gcilewalm.sHtML

[Q48] CTE 公用表表达式
来源：http://www.blog.fehbvm.com/Article/details/glpdjhkhq.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.zdbjq.cn/Article/details/gmbfaiwfr.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.hesvh.cn/Article/details/gsnrhqsib.sHtML

[Q49] 更新单行
来源：http://3g.zdbjq.cn/Article/details/gxocswcpc.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.zdbjq.cn/Article/details/gmwtdgkwd.sHtML

[Q50] 批量更新
来源：http://mobile.zdbjq.cn/Article/details/gekecugiz.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.fehbvm.com/Article/details/gyysgpbdm.sHtML

[Q51] 用子查询更新
来源：http://blog.hesvh.cn/Article/details/gwenzecft.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.hesvh.cn/Article/details/gpwupqpce.sHtML

[Q52] 删除指定行
来源：http://www.blog.hesvh.cn/Article/details/getdxyzfr.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.zdbjq.cn/Article/details/gbzbdlslc.sHtML

[Q53] 按条件删除
来源：http://www.share.hesvh.cn/Article/details/gobblunvx.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.m.share.hesvh.cn/Article/details/gfwrishwl.sHtML

[Q54] 清空表
来源：http://www.share.zdbjq.cn/Article/details/gjvoclnkr.sHtML

TRUNCATE TABLE logs;
来源：http://baike.hesvh.cn/Article/details/gfsznuyqp.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.hesvh.cn/Article/details/geqphzfbw.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.fehbvm.com/Article/details/gbexofxyu.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.fehbvm.com/Article/details/gqeleseap.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://m.share.fehbvm.com/Article/details/gxutzltma.sHtML

[Q57] 行号
来源：http://www.share.hesvh.cn/Article/details/ggdkkmwxj.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gelooyxik.sHtML

[Q58] 累计求和
来源：http://mobile.hesvh.cn/Article/details/gqlhdgbzi.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gyadulclw.sHtML

[Q59] 分组内累计
来源：http://mobile.zdbjq.cn/Article/details/gpriibsrb.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://read.share.hesvh.cn/Article/details/gxobycksq.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.m.share.hesvh.cn/Article/details/gskmovlby.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.share.hesvh.cn/Article/details/gvjhfvnsy.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.fehbvm.com/Article/details/gtacaforl.sHtML

[Q61] 移动平均
来源：http://baike.zdbjq.cn/Article/details/gsnwqgbnh.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.hesvh.cn/Article/details/gogybboem.sHtML

[Q62] 分组占比
来源：http://baike.hesvh.cn/Article/details/gvkifuszn.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.zdbjq.cn/Article/details/gobvqtwsq.sHtML

[Q63] 开启事务
来源：http://3g.fehbvm.com/Article/details/gsolmfulw.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.blog.hesvh.cn/Article/details/ghxdffpkj.sHtML

[Q64] 提交事务
来源：http://www.share.fehbvm.com/Article/details/gllitijpc.sHtML

COMMIT;
来源：http://read.share.fehbvm.com/Article/details/gtocfqagx.sHtML

[Q65] 回滚事务
来源：http://blog.fehbvm.com/Article/details/gpqsmrmpb.sHtML

ROLLBACK;
来源：http://www.blog.fehbvm.com/Article/details/gnaqyrpjx.sHtML

[Q66] 行锁查询
来源：http://www.share.zdbjq.cn/Article/details/gpfhytygi.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://mobile.hesvh.cn/Article/details/gnnzfdyvg.sHtML

[Q67] 设置隔离级别
来源：http://3g.fehbvm.com/Article/details/gargnoagr.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.fehbvm.com/Article/details/gpobdseky.sHtML

[Q68] 保存点
来源：http://www.blog.fehbvm.com/Article/details/guxdbkizz.sHtML

SAVEPOINT sp1;
来源：http://www.blog.zdbjq.cn/Article/details/gstyumzoj.sHtML

ROLLBACK TO sp1;
来源：http://www.blog.fehbvm.com/Article/details/gbvqukanm.sHtML

[Q69] 查看执行计划
来源：http://www.blog.hesvh.cn/Article/details/gnihwzbeu.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.m.share.fehbvm.com/Article/details/gxvippvac.sHtML

[Q70] 更新统计信息
来源：http://baike.zdbjq.cn/Article/details/glrfgvcgf.sHtML

ANALYZE TABLE users;
来源：http://m.share.zdbjq.cn/Article/details/gfaaiwurv.sHtML

[Q71] 查看建表语句
来源：http://wap.zdbjq.cn/Article/details/gyguxghql.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://m.share.fehbvm.com/Article/details/gbylruteg.sHtML

[Q72] 查看索引
来源：http://m.share.zdbjq.cn/Article/details/gqhekhmgp.sHtML

SHOW INDEX FROM users;
来源：http://blog.hesvh.cn/Article/details/grkkvzbty.sHtML

[Q73] 查看表状态
来源：http://baike.hesvh.cn/Article/details/gkywshegh.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.zdbjq.cn/Article/details/gyahyzhgl.sHtML

[Q74] 强制使用索引
来源：http://baike.hesvh.cn/Article/details/gabfhbzwr.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.hesvh.cn/Article/details/gkylmrnqb.sHtML

[Q75] 日期格式化
来源：http://baike.hesvh.cn/Article/details/ghhblqgau.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://wap.zdbjq.cn/Article/details/gqakmliiv.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.zdbjq.cn/Article/details/gohzsercc.sHtML

[Q76] 按天统计
来源：http://blog.zdbjq.cn/Article/details/gkjucsxol.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.zdbjq.cn/Article/details/gtymbtuay.sHtML

[Q77] 时间加减
来源：http://blog.hesvh.cn/Article/details/grkchmohk.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.fehbvm.com/Article/details/gsvvyvtfb.sHtML

[Q78] 当前时间
来源：http://wap.zdbjq.cn/Article/details/gykclivog.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.zdbjq.cn/Article/details/grhmrbjvl.sHtML

[Q79] 字符串拼接
来源：http://m.share.hesvh.cn/Article/details/gygahrerp.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://3g.zdbjq.cn/Article/details/gicitmlbp.sHtML

[Q80] 字符串截取
来源：http://3g.hesvh.cn/Article/details/gfqlrjzei.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gtafsrtxf.sHtML

[Q81] 字符串替换
来源：http://www.blog.hesvh.cn/Article/details/goneyidee.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gojkfajsv.sHtML

[Q82] 字符长度与字节长度
来源：http://www.m.share.fehbvm.com/Article/details/gabyqqqkg.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/gpmaacyvq.sHtML

[Q83] 大小写转换
来源：http://mobile.fehbvm.com/Article/details/gybwnfljn.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gpkbbeasc.sHtML

[Q84] 去除首尾空格
来源：http://mobile.fehbvm.com/Article/details/gganulwnf.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fehbvm.com/Article/details/gaetevhhi.sHtML

[Q85] 数值取整
来源：http://www.share.zdbjq.cn/Article/details/gifwwrjzx.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://baike.hesvh.cn/Article/details/goiyuorxk.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.zdbjq.cn/Article/details/gjjbzorjd.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.share.hesvh.cn/Article/details/gyrgmcymi.sHtML

[Q87] JSON 字段做条件
来源：http://blog.fehbvm.com/Article/details/grubicnpa.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.hesvh.cn/Article/details/guagojzve.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.share.fehbvm.com/Article/details/ghvvajvtu.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://mobile.hesvh.cn/Article/details/gzyradatd.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.hesvh.cn/Article/details/ggtmcizxm.sHtML

[Q89] 判断表是否存在
来源：http://3g.zdbjq.cn/Article/details/gagblojpe.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://baike.zdbjq.cn/Article/details/gsmiovlab.sHtML

[Q90] 生成序号列
来源：http://baike.fehbvm.com/Article/details/gdxnpmwxu.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://m.share.fehbvm.com/Article/details/gbqkbtoiw.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gopjcmfqg.sHtML

R. Bash 专题
来源：http://www.share.hesvh.cn/Article/details/gwrdyuxgq.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gdcboqxyn.sHtML

[R01] shebang 与严格模式
来源：http://baike.zdbjq.cn/Article/details/gkswlupxw.sHtML

#!/usr/bin/env bash
来源：http://m.share.zdbjq.cn/Article/details/guhupiqkw.sHtML

set -euo pipefail
来源：http://3g.zdbjq.cn/Article/details/gnsyogpti.sHtML

[R02] 变量赋值与使用
来源：http://read.share.hesvh.cn/Article/details/gxzfyhsgt.sHtML

name="Tom"; echo "$name"
来源：http://wap.fehbvm.com/Article/details/grfbpdund.sHtML

[R03] 只读变量
来源：http://blog.fehbvm.com/Article/details/gjgeuwabe.sHtML

readonly PI=3.14
来源：http://3g.zdbjq.cn/Article/details/glirycyjf.sHtML

[R04] 位置参数
来源：http://read.share.fehbvm.com/Article/details/gkhcarkyd.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fehbvm.com/Article/details/gkihmzcxo.sHtML

[R05] 参数默认值
来源：http://www.share.fehbvm.com/Article/details/gsmgygthd.sHtML

name="${1:-default}"
来源：http://mobile.zdbjq.cn/Article/details/gbldjqdss.sHtML

[R06] 判断命令是否存在
来源：http://m.share.hesvh.cn/Article/details/gasocdoqw.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.hesvh.cn/Article/details/gohomfyps.sHtML

[R07] if 判断文件
来源：http://blog.fehbvm.com/Article/details/gtblxlvji.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://mobile.fehbvm.com/Article/details/geksptiaq.sHtML

[R08] 数值比较
来源：http://blog.hesvh.cn/Article/details/gfqiikiqi.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.hesvh.cn/Article/details/glgdhrdac.sHtML

[R09] 字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/gnvswrlly.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://read.share.fehbvm.com/Article/details/gwvoonzfr.sHtML

[R10] 正则匹配
来源：http://baike.hesvh.cn/Article/details/ggmpxhwjk.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://m.share.zdbjq.cn/Article/details/giyvjviul.sHtML

[R11] case 多分支
来源：http://www.share.fehbvm.com/Article/details/gbabbqpgx.sHtML

case "$1" in
来源：http://m.share.hesvh.cn/Article/details/gqupogvzq.sHtML

start) echo "启动" ;;
来源：http://m.share.zdbjq.cn/Article/details/gbdklkzhc.sHtML

stop)  echo "停止" ;;
来源：http://3g.fehbvm.com/Article/details/gsijynjhd.sHtML

*)     echo "未知命令" ;;
来源：http://www.share.hesvh.cn/Article/details/glltkzbxc.sHtML

esac
来源：http://mobile.hesvh.cn/Article/details/ghvcigfbc.sHtML

[R12] for 遍历文件
来源：http://www.m.share.zdbjq.cn/Article/details/gdkrqjbdl.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.zdbjq.cn/Article/details/gctqprlsh.sHtML

[R13] for 计数循环
来源：http://m.share.zdbjq.cn/Article/details/ghuznagvt.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://wap.zdbjq.cn/Article/details/gpcenptat.sHtML

[R14] C 风格 for
来源：http://m.share.hesvh.cn/Article/details/gaodpcwja.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.blog.fehbvm.com/Article/details/gqismczui.sHtML

[R15] while 逐行读文件
来源：http://wap.hesvh.cn/Article/details/gpnujhjfi.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://baike.hesvh.cn/Article/details/ggghpapat.sHtML

[R16] until 等待条件
来源：http://baike.zdbjq.cn/Article/details/gmicungup.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://wap.zdbjq.cn/Article/details/ggewxynji.sHtML

[R17] 数组定义与取值
来源：http://www.blog.fehbvm.com/Article/details/glygvdavf.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.zdbjq.cn/Article/details/gpjmbhiet.sHtML

[R18] 遍历数组
来源：http://wap.fehbvm.com/Article/details/goglctulp.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fehbvm.com/Article/details/gnfabsnem.sHtML

[R19] 数组长度
来源：http://read.share.fehbvm.com/Article/details/gizxmoubl.sHtML

echo "${#arr[@]}"
来源：http://mobile.zdbjq.cn/Article/details/gpypfxuli.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fehbvm.com/Article/details/gmgmgfxyo.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.fehbvm.com/Article/details/gbeoyuelc.sHtML

[R21] 字符串长度
来源：http://www.share.fehbvm.com/Article/details/gfeozkfoh.sHtML

echo "${#s}"
来源：http://m.share.fehbvm.com/Article/details/gzihzpghq.sHtML

[R22] 截取子串
来源：http://www.m.share.zdbjq.cn/Article/details/gigunjpre.sHtML

echo "${s:0:5}"
来源：http://www.share.zdbjq.cn/Article/details/gjhwscqyy.sHtML

[R23] 字符串替换
来源：http://m.share.hesvh.cn/Article/details/gkgtfoded.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fehbvm.com/Article/details/gywwxchco.sHtML

[R24] 大小写转换
来源：http://www.share.zdbjq.cn/Article/details/ghmejhvyo.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fehbvm.com/Article/details/gqhjtvrzb.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.zdbjq.cn/Article/details/gnkqcntav.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.hesvh.cn/Article/details/gcktljwrz.sHtML

[R26] 命令替换
来源：http://mobile.hesvh.cn/Article/details/gxjhgkpax.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.fehbvm.com/Article/details/grphbahpz.sHtML

[R27] 算术展开
来源：http://3g.fehbvm.com/Article/details/gqmkhgxqg.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fehbvm.com/Article/details/gamcrpzgt.sHtML

[R28] 浮点运算
来源：http://www.blog.hesvh.cn/Article/details/ghwxezzmi.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.hesvh.cn/Article/details/gxsjzbnap.sHtML

[R29] 定义函数
来源：http://blog.fehbvm.com/Article/details/ghjqsfdbl.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fehbvm.com/Article/details/gbrjjmgci.sHtML

[R30] 函数返回状态码
来源：http://baike.hesvh.cn/Article/details/gqqrbtnny.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.hesvh.cn/Article/details/gykcsdvsh.sHtML

[R31] 局部变量
来源：http://www.blog.zdbjq.cn/Article/details/gkrvkfbqp.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.hesvh.cn/Article/details/gypdxshyv.sHtML

[R32] 参数个数校验
来源：http://blog.hesvh.cn/Article/details/gwjnkemsr.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.hesvh.cn/Article/details/gjkxtukrl.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fehbvm.com/Article/details/gtjdyzutg.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.zdbjq.cn/Article/details/gbfpgljyk.sHtML

[R34] 退出时清理
来源：http://www.m.share.zdbjq.cn/Article/details/gvyoxikki.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.hesvh.cn/Article/details/ghwaiqvss.sHtML

[R35] 后台执行并等待
来源：http://baike.fehbvm.com/Article/details/gbhfuhoqg.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fehbvm.com/Article/details/gihzbvkxj.sHtML

[R36] 并发执行多个任务
来源：http://blog.zdbjq.cn/Article/details/gdlrogngt.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.zdbjq.cn/Article/details/gjbxkggyz.sHtML

[R37] 把输出赋给变量
来源：http://www.share.hesvh.cn/Article/details/gbgaabypp.sHtML

files=$(ls -1)
来源：http://m.share.hesvh.cn/Article/details/gkhdyhncm.sHtML

[R38] 管道串联
来源：http://baike.zdbjq.cn/Article/details/goljdmifk.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.zdbjq.cn/Article/details/gkynskgxs.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.zdbjq.cn/Article/details/gmbkxtuxi.sHtML

cmd > out.log 2>&1
来源：http://read.share.fehbvm.com/Article/details/gviobzmqk.sHtML

[R40] 追加写日志
来源：http://blog.fehbvm.com/Article/details/gugwnncji.sHtML

echo "log" >> out.log
来源：http://read.share.hesvh.cn/Article/details/gmrikfexe.sHtML

[R41] 丢弃输出
来源：http://mobile.hesvh.cn/Article/details/gybfeigjr.sHtML

cmd >/dev/null 2>&1
来源：http://www.blog.fehbvm.com/Article/details/grgphmgvt.sHtML

[R42] 输入重定向
来源：http://m.share.fehbvm.com/Article/details/gsfejodlk.sHtML

wc -l < a.txt
来源：http://m.share.hesvh.cn/Article/details/gpbxwhias.sHtML

[R43] 按名字查找文件
来源：http://www.blog.zdbjq.cn/Article/details/gjrjtvbzq.sHtML

find . -name "*.log" -type f
来源：http://read.share.zdbjq.cn/Article/details/gvuiozjes.sHtML

[R44] 按修改时间查找
来源：http://baike.hesvh.cn/Article/details/glnvbfpbl.sHtML

find . -mtime -7 -type f
来源：http://www.share.fehbvm.com/Article/details/gocizwdpp.sHtML

[R45] 批量删除
来源：http://read.share.hesvh.cn/Article/details/gelbtowrl.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.hesvh.cn/Article/details/gqrctdkad.sHtML

[R46] 递归替换文件内容
来源：http://mobile.hesvh.cn/Article/details/gtiltlyyj.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fehbvm.com/Article/details/gokvoauwt.sHtML

[R47] sed 单行替换
来源：http://blog.hesvh.cn/Article/details/gnmutfwqg.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.hesvh.cn/Article/details/ghpybsxqi.sHtML

[R48] awk 取指定列
来源：http://baike.hesvh.cn/Article/details/gjnqbsumt.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.zdbjq.cn/Article/details/gmcsxznkf.sHtML

[R49] awk 带条件
来源：http://www.m.share.fehbvm.com/Article/details/gdubrqbwm.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.zdbjq.cn/Article/details/gilwsodra.sHtML

[R50] awk 求和
来源：http://m.share.fehbvm.com/Article/details/gjryjnamz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.zdbjq.cn/Article/details/ggrkuysab.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.hesvh.cn/Article/details/gswioatwc.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.zdbjq.cn/Article/details/gkrvrnfya.sHtML

[R52] 统计行数
来源：http://read.share.fehbvm.com/Article/details/gdnzlmtms.sHtML

wc -l a.txt
来源：http://www.share.hesvh.cn/Article/details/gjghtakwd.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fehbvm.com/Article/details/gytlyzcgg.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fehbvm.com/Article/details/gffrqwyyb.sHtML

[R54] 比较两个文件
来源：http://baike.hesvh.cn/Article/details/guwhhuomm.sHtML

diff a.txt b.txt
来源：http://baike.hesvh.cn/Article/details/gexkbvrxw.sHtML

[R55] 压缩与解压
来源：http://3g.zdbjq.cn/Article/details/gnnafbevo.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fehbvm.com/Article/details/gwcehfzoy.sHtML

[R56] 远程拷贝
来源：http://www.m.share.hesvh.cn/Article/details/gihcsqcrp.sHtML

scp file user@host:/path/
来源：http://www.share.fehbvm.com/Article/details/giiqtksnm.sHtML

[R57] 远程执行命令
来源：http://www.m.share.hesvh.cn/Article/details/gkzroubua.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.hesvh.cn/Article/details/gjudixkvx.sHtML

[R58] 下载文件
来源：http://baike.fehbvm.com/Article/details/gpxzblish.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fehbvm.com/Article/details/gmvzqajoy.sHtML

[R59] 发 POST JSON
来源：http://mobile.fehbvm.com/Article/details/gjhqpjokb.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.zdbjq.cn/Article/details/ghciqubjx.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.hesvh.cn/Article/details/gdcddvzgo.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.hesvh.cn/Article/details/gopcmnwlc.sHtML

[R61] 磁盘占用
来源：http://m.share.zdbjq.cn/Article/details/gewnwmqol.sHtML

df -h;  du -sh *
来源：http://baike.hesvh.cn/Article/details/gchnvanip.sHtML

[R62] 找最占空间的文件
来源：http://www.share.zdbjq.cn/Article/details/gkpncsapm.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.fehbvm.com/Article/details/ghnlmwupp.sHtML

[R63] 内存与进程
来源：http://wap.fehbvm.com/Article/details/gpeolyttu.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.zdbjq.cn/Article/details/gzpzwcksr.sHtML

[R64] 结束进程
来源：http://read.share.fehbvm.com/Article/details/gdvcjudms.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.hesvh.cn/Article/details/grfvivyva.sHtML

[R65] 查看端口占用
来源：http://www.m.share.hesvh.cn/Article/details/gmhhtlzjp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fehbvm.com/Article/details/gxuhzappc.sHtML

[R66] 定时任务
来源：http://wap.hesvh.cn/Article/details/gbalcyqtv.sHtML

crontab -e;  crontab -l
来源：http://m.share.fehbvm.com/Article/details/gzqswmtni.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.zdbjq.cn/Article/details/gafficwbr.sHtML

openssl rand -hex 16
来源：http://www.blog.zdbjq.cn/Article/details/glarbalom.sHtML

[R68] 计算文件校验值
来源：http://m.share.fehbvm.com/Article/details/gyncfoqvz.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.hesvh.cn/Article/details/gfmwmfkda.sHtML

[R69] 生成随机密码
来源：http://www.share.zdbjq.cn/Article/details/gqevvigty.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fehbvm.com/Article/details/giybpjcbc.sHtML

[R70] 时间戳与互转
来源：http://wap.hesvh.cn/Article/details/gqsllqdhz.sHtML

date +%s;  date -d @1700000000
来源：http://3g.hesvh.cn/Article/details/gtvttconz.sHtML

[R71] 日期格式化
来源：http://www.blog.hesvh.cn/Article/details/gniscaszu.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.hesvh.cn/Article/details/gpypnrczt.sHtML

[R72] 等待端口就绪
来源：http://3g.zdbjq.cn/Article/details/gewrzgprr.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fehbvm.com/Article/details/gmusemtqz.sHtML

[R73] 分割大日志
来源：http://wap.hesvh.cn/Article/details/grzgkpxwc.sHtML

split -l 1000 big.log part_
来源：http://blog.zdbjq.cn/Article/details/gxtbwypvt.sHtML

[R74] 批量重命名
来源：http://3g.fehbvm.com/Article/details/goemrvmcq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.hesvh.cn/Article/details/ghjjwlpxo.sHtML

[R75] 导出环境变量
来源：http://m.share.fehbvm.com/Article/details/gxkwynbpn.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fehbvm.com/Article/details/ghmmtrnxw.sHtML

[R76] 使用临时文件
来源：http://www.m.share.hesvh.cn/Article/details/gzydcaeaa.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.zdbjq.cn/Article/details/gywxhirok.sHtML

[R77] 读取用户输入
来源：http://read.share.fehbvm.com/Article/details/gunfzeqzt.sHtML

read -rp "请输入: " ans
来源：http://baike.zdbjq.cn/Article/details/gffcdzcgb.sHtML

[R78] 交互式菜单
来源：http://blog.fehbvm.com/Article/details/glzgbwqed.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fehbvm.com/Article/details/gjwpdezug.sHtML

[R79] 解析命令行选项
来源：http://www.blog.zdbjq.cn/Article/details/gtnggfqvu.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.hesvh.cn/Article/details/gnuxbykys.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.zdbjq.cn/Article/details/gxbmtpigd.sHtML

time ./run.sh
来源：http://mobile.zdbjq.cn/Article/details/gsputwzbk.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gcmbkaewr.sHtML

S. C / C++ 专题
来源：http://blog.zdbjq.cn/Article/details/gpzaqnnpq.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gvehrutky.sHtML

[S01] C：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gypoykaxq.sHtML

#include <stdio.h>
来源：http://mobile.hesvh.cn/Article/details/gypxrlxgm.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fehbvm.com/Article/details/gpmoyroib.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fehbvm.com/Article/details/gpqgrgbso.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.hesvh.cn/Article/details/gztbygkoz.sHtML

[S03] C：读入整数
来源：http://read.share.fehbvm.com/Article/details/gufcrkjvn.sHtML

int x; scanf("%d", &x);
来源：http://read.share.hesvh.cn/Article/details/ggmodxvok.sHtML

[S04] C：字符串复制
来源：http://m.share.zdbjq.cn/Article/details/gihphhxjs.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.zdbjq.cn/Article/details/gcdgvgwdy.sHtML

[S05] C：字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/gvqrbddpn.sHtML


<!-- 参考信息 -->