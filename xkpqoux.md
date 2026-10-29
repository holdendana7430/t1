代发 wailian999

[Q36] 左连接
来源：http://3g.zdbjq.cn/Article/details/gegwcbibk.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://mobile.fehbvm.com/Article/details/giiwkvsdq.sHtML

[Q37] 右连接
来源：http://baike.fehbvm.com/Article/details/gdglissfz.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://blog.fehbvm.com/Article/details/ggnmbvtzu.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://3g.hesvh.cn/Article/details/glzvaiiod.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.m.share.zdbjq.cn/Article/details/grfpjfmvt.sHtML

[Q39] 自连接（查上下级）
来源：http://mobile.fehbvm.com/Article/details/gifueezlf.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://m.share.fehbvm.com/Article/details/gsqfmgbjr.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.share.zdbjq.cn/Article/details/gbuidcrwp.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.zdbjq.cn/Article/details/gcdaoayhs.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://mobile.hesvh.cn/Article/details/ggapvyvuf.sHtML

[Q41] 多表连接
来源：http://3g.fehbvm.com/Article/details/gjbgqibpt.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://mobile.zdbjq.cn/Article/details/gwkfjwyrs.sHtML

JOIN users u ON u.id = o.user_id
来源：http://3g.fehbvm.com/Article/details/gqylimvxy.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.blog.fehbvm.com/Article/details/gujysnpup.sHtML

[Q42] 连接条件附加过滤
来源：http://read.share.fehbvm.com/Article/details/gpmezfdus.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.fehbvm.com/Article/details/gxiogufpx.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.blog.fehbvm.com/Article/details/gerwcfjyc.sHtML

[Q43] 标量子查询
来源：http://www.share.zdbjq.cn/Article/details/ggiaytrms.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://m.share.hesvh.cn/Article/details/gjjerdztp.sHtML

[Q44] IN 子查询
来源：http://www.share.zdbjq.cn/Article/details/gylvpaymt.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.hesvh.cn/Article/details/gmjfyqkbx.sHtML

[Q45] EXISTS 判断存在
来源：http://www.m.share.hesvh.cn/Article/details/gknfeohif.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.share.zdbjq.cn/Article/details/guvnstodk.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://baike.fehbvm.com/Article/details/gsccqeigw.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.fehbvm.com/Article/details/gnaptyhzy.sHtML

[Q47] 与平均值比较
来源：http://www.blog.zdbjq.cn/Article/details/gwfqywzjy.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.m.share.hesvh.cn/Article/details/grdgfobwz.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.fehbvm.com/Article/details/geremyczw.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.zdbjq.cn/Article/details/gnmqzgbte.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://www.share.zdbjq.cn/Article/details/godznlaoj.sHtML

[Q49] 更新单行
来源：http://www.share.zdbjq.cn/Article/details/grdyejhjy.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.hesvh.cn/Article/details/gwpgfzsua.sHtML

[Q50] 批量更新
来源：http://read.share.zdbjq.cn/Article/details/gdlmdtzaz.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.fehbvm.com/Article/details/giydfpqln.sHtML

[Q51] 用子查询更新
来源：http://www.blog.hesvh.cn/Article/details/gzcvawthh.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://m.share.zdbjq.cn/Article/details/gvtofbpga.sHtML

[Q52] 删除指定行
来源：http://www.share.hesvh.cn/Article/details/gbysyhejt.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.blog.zdbjq.cn/Article/details/gluhwauux.sHtML

[Q53] 按条件删除
来源：http://mobile.fehbvm.com/Article/details/gitruqelo.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://mobile.zdbjq.cn/Article/details/gsnfbxktv.sHtML

[Q54] 清空表
来源：http://m.share.fehbvm.com/Article/details/gpmhkixxw.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.zdbjq.cn/Article/details/grryqtlqa.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.fehbvm.com/Article/details/gkwclloab.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://read.share.hesvh.cn/Article/details/gflsaotkl.sHtML

[Q56] 密集排名（并列不占位）
来源：http://wap.fehbvm.com/Article/details/gfvtruqvi.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.share.zdbjq.cn/Article/details/gggsrfawe.sHtML

[Q57] 行号
来源：http://m.share.fehbvm.com/Article/details/gshghnnui.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.fehbvm.com/Article/details/gvjixwhlz.sHtML

[Q58] 累计求和
来源：http://baike.zdbjq.cn/Article/details/gsiabbksk.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.fehbvm.com/Article/details/gelrntcxk.sHtML

[Q59] 分组内累计
来源：http://www.blog.fehbvm.com/Article/details/gicpuhvtl.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://m.share.hesvh.cn/Article/details/grhbfcijr.sHtML

[Q60] 取上一行 / 下一行
来源：http://www.blog.hesvh.cn/Article/details/ghqzuhbdu.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://mobile.fehbvm.com/Article/details/gwqtdzraq.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.hesvh.cn/Article/details/gmurafyms.sHtML

[Q61] 移动平均
来源：http://read.share.fehbvm.com/Article/details/gdhfmnoqu.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.blog.fehbvm.com/Article/details/gawbmpztd.sHtML

[Q62] 分组占比
来源：http://read.share.fehbvm.com/Article/details/gsaruifii.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.hesvh.cn/Article/details/gjvcepwfa.sHtML

[Q63] 开启事务
来源：http://m.share.zdbjq.cn/Article/details/gvosgandm.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://m.share.zdbjq.cn/Article/details/gksgcvipu.sHtML

[Q64] 提交事务
来源：http://baike.fehbvm.com/Article/details/gghsbxygi.sHtML

COMMIT;
来源：http://baike.zdbjq.cn/Article/details/glrhxtyxp.sHtML

[Q65] 回滚事务
来源：http://www.m.share.fehbvm.com/Article/details/gtiqrjwpw.sHtML

ROLLBACK;
来源：http://baike.zdbjq.cn/Article/details/gesztrkgv.sHtML

[Q66] 行锁查询
来源：http://read.share.hesvh.cn/Article/details/gjoyibvtv.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://baike.fehbvm.com/Article/details/ghlcmsaev.sHtML

[Q67] 设置隔离级别
来源：http://baike.zdbjq.cn/Article/details/guiwygdvi.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.share.hesvh.cn/Article/details/gvivvxiyb.sHtML

[Q68] 保存点
来源：http://mobile.fehbvm.com/Article/details/gzqeqjbls.sHtML

SAVEPOINT sp1;
来源：http://m.share.fehbvm.com/Article/details/gsdlnizvr.sHtML

ROLLBACK TO sp1;
来源：http://m.share.zdbjq.cn/Article/details/guxuivkdu.sHtML

[Q69] 查看执行计划
来源：http://baike.fehbvm.com/Article/details/gitdugkwn.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://m.share.hesvh.cn/Article/details/gphpgtzoe.sHtML

[Q70] 更新统计信息
来源：http://read.share.fehbvm.com/Article/details/givnfrwqn.sHtML

ANALYZE TABLE users;
来源：http://wap.fehbvm.com/Article/details/gdvtfcvox.sHtML

[Q71] 查看建表语句
来源：http://mobile.zdbjq.cn/Article/details/gxvliuepf.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://mobile.fehbvm.com/Article/details/godqdjapj.sHtML

[Q72] 查看索引
来源：http://www.m.share.hesvh.cn/Article/details/gopfzfbih.sHtML

SHOW INDEX FROM users;
来源：http://m.share.fehbvm.com/Article/details/gwfczvoqq.sHtML

[Q73] 查看表状态
来源：http://m.share.hesvh.cn/Article/details/gwqhdkrhu.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.fehbvm.com/Article/details/gokvxoqli.sHtML

[Q74] 强制使用索引
来源：http://m.share.zdbjq.cn/Article/details/gwzjgnmkt.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.m.share.zdbjq.cn/Article/details/gtqoskfwl.sHtML

[Q75] 日期格式化
来源：http://www.blog.zdbjq.cn/Article/details/gthjkkjzr.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/ghopurthm.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.blog.hesvh.cn/Article/details/gnphfmbnn.sHtML

[Q76] 按天统计
来源：http://mobile.zdbjq.cn/Article/details/gdxoogcmf.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fehbvm.com/Article/details/gxvqtcfph.sHtML

[Q77] 时间加减
来源：http://blog.zdbjq.cn/Article/details/gdrgxtciu.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://baike.fehbvm.com/Article/details/gzaojpheu.sHtML

[Q78] 当前时间
来源：http://blog.zdbjq.cn/Article/details/gonmexhzj.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.zdbjq.cn/Article/details/gqycdlehu.sHtML

[Q79] 字符串拼接
来源：http://www.m.share.fehbvm.com/Article/details/giuibjfhu.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.hesvh.cn/Article/details/gspcixytd.sHtML

[Q80] 字符串截取
来源：http://blog.hesvh.cn/Article/details/gswxakysr.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://wap.zdbjq.cn/Article/details/gtsmzqffw.sHtML

[Q81] 字符串替换
来源：http://www.share.zdbjq.cn/Article/details/glwaybsjw.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.zdbjq.cn/Article/details/gbwdeyywk.sHtML

[Q82] 字符长度与字节长度
来源：http://blog.fehbvm.com/Article/details/gmbmvbcdg.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/gjcdikspn.sHtML

[Q83] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/gtzszzhan.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.fehbvm.com/Article/details/gexiqnyqg.sHtML

[Q84] 去除首尾空格
来源：http://3g.fehbvm.com/Article/details/gufecufth.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.zdbjq.cn/Article/details/grybefntk.sHtML

[Q85] 数值取整
来源：http://wap.fehbvm.com/Article/details/gllndalqf.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.hesvh.cn/Article/details/ghztnybnd.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.hesvh.cn/Article/details/gcgyqwkcw.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.hesvh.cn/Article/details/gekkwzazq.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.zdbjq.cn/Article/details/goetzgzpr.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://blog.zdbjq.cn/Article/details/gzisjflxi.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.blog.hesvh.cn/Article/details/glkrqszqb.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.m.share.hesvh.cn/Article/details/gmfxyqghz.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://wap.zdbjq.cn/Article/details/gmyfchbqy.sHtML

[Q89] 判断表是否存在
来源：http://baike.fehbvm.com/Article/details/gcvwxoodk.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.zdbjq.cn/Article/details/gbypqgrsv.sHtML

[Q90] 生成序号列
来源：http://3g.zdbjq.cn/Article/details/gkdiliafx.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://3g.fehbvm.com/Article/details/gtahybrla.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gytxgcxtj.sHtML

R. Bash 专题
来源：http://www.blog.fehbvm.com/Article/details/gbsdbibdi.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gzlbwfwep.sHtML

[R01] shebang 与严格模式
来源：http://read.share.hesvh.cn/Article/details/gmgwvmzqx.sHtML

#!/usr/bin/env bash
来源：http://3g.fehbvm.com/Article/details/glquumico.sHtML

set -euo pipefail
来源：http://wap.zdbjq.cn/Article/details/gxbggodoz.sHtML

[R02] 变量赋值与使用
来源：http://3g.zdbjq.cn/Article/details/gtfqrktfa.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fehbvm.com/Article/details/gslbzhzui.sHtML

[R03] 只读变量
来源：http://m.share.fehbvm.com/Article/details/gecqvxzum.sHtML

readonly PI=3.14
来源：http://blog.hesvh.cn/Article/details/gipyeuncz.sHtML

[R04] 位置参数
来源：http://www.blog.fehbvm.com/Article/details/gpriteiqj.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.hesvh.cn/Article/details/gzxdvpmai.sHtML

[R05] 参数默认值
来源：http://m.share.hesvh.cn/Article/details/geqwrtpzu.sHtML

name="${1:-default}"
来源：http://www.share.zdbjq.cn/Article/details/gxxqupyrc.sHtML

[R06] 判断命令是否存在
来源：http://mobile.fehbvm.com/Article/details/grlxeczgo.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.zdbjq.cn/Article/details/gjloqreio.sHtML

[R07] if 判断文件
来源：http://www.share.zdbjq.cn/Article/details/govbkvsxs.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fehbvm.com/Article/details/gtgxrtgku.sHtML

[R08] 数值比较
来源：http://3g.fehbvm.com/Article/details/gbbvniqsm.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.hesvh.cn/Article/details/gebzzhhli.sHtML

[R09] 字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/gsihlpypt.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://baike.fehbvm.com/Article/details/giuioikeg.sHtML

[R10] 正则匹配
来源：http://www.m.share.zdbjq.cn/Article/details/gqleaheuc.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.zdbjq.cn/Article/details/guuhdgpbz.sHtML

[R11] case 多分支
来源：http://blog.hesvh.cn/Article/details/gkcskhepk.sHtML

case "$1" in
来源：http://3g.fehbvm.com/Article/details/genznkwsu.sHtML

start) echo "启动" ;;
来源：http://mobile.fehbvm.com/Article/details/gqbxqhkfb.sHtML

stop)  echo "停止" ;;
来源：http://baike.hesvh.cn/Article/details/gmvsauugc.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fehbvm.com/Article/details/guppmcuqc.sHtML

esac
来源：http://www.share.zdbjq.cn/Article/details/genyxsgrz.sHtML

[R12] for 遍历文件
来源：http://mobile.fehbvm.com/Article/details/gfxzjsjvn.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.zdbjq.cn/Article/details/gykfumidy.sHtML

[R13] for 计数循环
来源：http://blog.hesvh.cn/Article/details/gtoejyxrs.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.zdbjq.cn/Article/details/gskxrcsyf.sHtML

[R14] C 风格 for
来源：http://www.m.share.fehbvm.com/Article/details/gmlspxlrg.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.hesvh.cn/Article/details/gijhpgtde.sHtML

[R15] while 逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/guzfosgls.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.hesvh.cn/Article/details/gvgvbrpnn.sHtML

[R16] until 等待条件
来源：http://baike.fehbvm.com/Article/details/gwxkzldmx.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.share.zdbjq.cn/Article/details/gpwctqykm.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.hesvh.cn/Article/details/gdpvcdggj.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gerjrrrlf.sHtML

[R18] 遍历数组
来源：http://www.blog.zdbjq.cn/Article/details/gwtqwfebk.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fehbvm.com/Article/details/gehmzohyh.sHtML

[R19] 数组长度
来源：http://baike.fehbvm.com/Article/details/gyqydkehy.sHtML

echo "${#arr[@]}"
来源：http://3g.zdbjq.cn/Article/details/gxlbkzugn.sHtML

[R20] 关联数组（字典）
来源：http://www.blog.hesvh.cn/Article/details/gnkmhdqyl.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://blog.fehbvm.com/Article/details/guykvfpkv.sHtML

[R21] 字符串长度
来源：http://www.blog.fehbvm.com/Article/details/gdxvxitgd.sHtML

echo "${#s}"
来源：http://read.share.fehbvm.com/Article/details/gkivqimed.sHtML

[R22] 截取子串
来源：http://www.share.fehbvm.com/Article/details/gkxpndqsr.sHtML

echo "${s:0:5}"
来源：http://3g.fehbvm.com/Article/details/ggdzxgscq.sHtML

[R23] 字符串替换
来源：http://www.blog.zdbjq.cn/Article/details/gldhxafny.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.m.share.zdbjq.cn/Article/details/gpmrlkedj.sHtML

[R24] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/gvvvoupdj.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fehbvm.com/Article/details/gdlazxsnh.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.zdbjq.cn/Article/details/gpbcpepxy.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.zdbjq.cn/Article/details/gxqvwwugw.sHtML

[R26] 命令替换
来源：http://www.blog.fehbvm.com/Article/details/gntmikcxd.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.zdbjq.cn/Article/details/gsicdfbnz.sHtML

[R27] 算术展开
来源：http://read.share.zdbjq.cn/Article/details/gkpovzblx.sHtML

echo $((1 + 2 * 3))
来源：http://www.m.share.hesvh.cn/Article/details/gynojugji.sHtML

[R28] 浮点运算
来源：http://blog.fehbvm.com/Article/details/gaqjsthev.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.fehbvm.com/Article/details/gcpmruwmg.sHtML

[R29] 定义函数
来源：http://read.share.fehbvm.com/Article/details/gzppeztmd.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.hesvh.cn/Article/details/gbrocoqmo.sHtML

[R30] 函数返回状态码
来源：http://m.share.zdbjq.cn/Article/details/gvwprxytb.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.zdbjq.cn/Article/details/gyejrxrqn.sHtML

[R31] 局部变量
来源：http://baike.zdbjq.cn/Article/details/gfgpxvagc.sHtML

f() { local x=1; echo "$x"; }
来源：http://mobile.hesvh.cn/Article/details/geonoxcsl.sHtML

[R32] 参数个数校验
来源：http://baike.zdbjq.cn/Article/details/goepxaytt.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.hesvh.cn/Article/details/gnnlajhwn.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.zdbjq.cn/Article/details/gjnquguow.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fehbvm.com/Article/details/gijxrqjib.sHtML

[R34] 退出时清理
来源：http://mobile.zdbjq.cn/Article/details/gdnbwpgkk.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.zdbjq.cn/Article/details/ghccfxyxz.sHtML

[R35] 后台执行并等待
来源：http://www.share.hesvh.cn/Article/details/gdgbidtvl.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fehbvm.com/Article/details/gchhqoskk.sHtML

[R36] 并发执行多个任务
来源：http://baike.zdbjq.cn/Article/details/gtxpuknfq.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://mobile.fehbvm.com/Article/details/gqfkeglvp.sHtML

[R37] 把输出赋给变量
来源：http://3g.hesvh.cn/Article/details/gmxsiwcvz.sHtML

files=$(ls -1)
来源：http://wap.hesvh.cn/Article/details/gbsbiaass.sHtML

[R38] 管道串联
来源：http://www.blog.hesvh.cn/Article/details/gjxlgwvzi.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.fehbvm.com/Article/details/gkmhllqao.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.hesvh.cn/Article/details/guqakyoca.sHtML

cmd > out.log 2>&1
来源：http://m.share.hesvh.cn/Article/details/ghrnaatun.sHtML

[R40] 追加写日志
来源：http://read.share.zdbjq.cn/Article/details/gjxgkmjik.sHtML

echo "log" >> out.log
来源：http://wap.zdbjq.cn/Article/details/gfeqryyfk.sHtML

[R41] 丢弃输出
来源：http://www.m.share.zdbjq.cn/Article/details/gsqwubnwp.sHtML

cmd >/dev/null 2>&1
来源：http://blog.zdbjq.cn/Article/details/gouftljri.sHtML

[R42] 输入重定向
来源：http://www.share.fehbvm.com/Article/details/gbllmqtye.sHtML

wc -l < a.txt
来源：http://baike.fehbvm.com/Article/details/glrekndeo.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.zdbjq.cn/Article/details/gxtviopiu.sHtML

find . -name "*.log" -type f
来源：http://baike.zdbjq.cn/Article/details/gkbnppjnz.sHtML

[R44] 按修改时间查找
来源：http://wap.zdbjq.cn/Article/details/guwfcfdqs.sHtML

find . -mtime -7 -type f
来源：http://www.share.zdbjq.cn/Article/details/gxcccjavy.sHtML

[R45] 批量删除
来源：http://mobile.hesvh.cn/Article/details/gcjnpzdvv.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.zdbjq.cn/Article/details/gkbczuulh.sHtML

[R46] 递归替换文件内容
来源：http://mobile.hesvh.cn/Article/details/gungbsvhh.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fehbvm.com/Article/details/gshvnenjy.sHtML

[R47] sed 单行替换
来源：http://baike.zdbjq.cn/Article/details/gphomeyav.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fehbvm.com/Article/details/gmjeuubpf.sHtML

[R48] awk 取指定列
来源：http://www.blog.zdbjq.cn/Article/details/gcqssaxaz.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.hesvh.cn/Article/details/geakuzgpd.sHtML

[R49] awk 带条件
来源：http://read.share.hesvh.cn/Article/details/gcvoywqvh.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.hesvh.cn/Article/details/gkkqwuscq.sHtML

[R50] awk 求和
来源：http://www.share.hesvh.cn/Article/details/gwcswpaoq.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fehbvm.com/Article/details/gaclyowql.sHtML

[R51] 排序去重取前几
来源：http://m.share.hesvh.cn/Article/details/gyepglzqu.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fehbvm.com/Article/details/gdmbrhxob.sHtML

[R52] 统计行数
来源：http://m.share.hesvh.cn/Article/details/gfvdedsjd.sHtML

wc -l a.txt
来源：http://blog.fehbvm.com/Article/details/griydqswy.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fehbvm.com/Article/details/gkykwveab.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fehbvm.com/Article/details/gpszsyvwu.sHtML

[R54] 比较两个文件
来源：http://read.share.zdbjq.cn/Article/details/gyjbethej.sHtML

diff a.txt b.txt
来源：http://www.blog.fehbvm.com/Article/details/gcjqvgxew.sHtML

[R55] 压缩与解压
来源：http://mobile.zdbjq.cn/Article/details/gdlpaemgx.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.hesvh.cn/Article/details/gvnipldqf.sHtML

[R56] 远程拷贝
来源：http://www.share.zdbjq.cn/Article/details/gegclvgqf.sHtML

scp file user@host:/path/
来源：http://read.share.zdbjq.cn/Article/details/goeqqijli.sHtML

[R57] 远程执行命令
来源：http://www.m.share.hesvh.cn/Article/details/gzfokhziy.sHtML

ssh user@host 'uptime'
来源：http://m.share.zdbjq.cn/Article/details/gticbvmkq.sHtML

[R58] 下载文件
来源：http://blog.hesvh.cn/Article/details/ghawfeyzf.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fehbvm.com/Article/details/gevuabalh.sHtML

[R59] 发 POST JSON
来源：http://m.share.hesvh.cn/Article/details/ggzkndxcr.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.hesvh.cn/Article/details/gdeidcwzm.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.zdbjq.cn/Article/details/gpnenhhqj.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.zdbjq.cn/Article/details/gplktnjtt.sHtML

[R61] 磁盘占用
来源：http://www.m.share.hesvh.cn/Article/details/gfaczbbwz.sHtML

df -h;  du -sh *
来源：http://blog.hesvh.cn/Article/details/gumqvwgzb.sHtML

[R62] 找最占空间的文件
来源：http://wap.fehbvm.com/Article/details/gfvuhcltz.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.zdbjq.cn/Article/details/ggxiclhxr.sHtML

[R63] 内存与进程
来源：http://mobile.fehbvm.com/Article/details/gcgqbmhlk.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.zdbjq.cn/Article/details/gvojwyogc.sHtML

[R64] 结束进程
来源：http://wap.fehbvm.com/Article/details/gdccedjpi.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fehbvm.com/Article/details/gupujjbtp.sHtML

[R65] 查看端口占用
来源：http://www.share.zdbjq.cn/Article/details/ghktorkqy.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.hesvh.cn/Article/details/gqpqqxuep.sHtML

[R66] 定时任务
来源：http://wap.fehbvm.com/Article/details/gkwccavsq.sHtML

crontab -e;  crontab -l
来源：http://www.share.hesvh.cn/Article/details/gtltppuus.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fehbvm.com/Article/details/guqelwbqs.sHtML

openssl rand -hex 16
来源：http://m.share.hesvh.cn/Article/details/ggzwiqcbo.sHtML

[R68] 计算文件校验值
来源：http://www.share.zdbjq.cn/Article/details/ghiuuvgvq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.hesvh.cn/Article/details/gtvrfkqhr.sHtML

[R69] 生成随机密码
来源：http://mobile.zdbjq.cn/Article/details/gtqghsnvi.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fehbvm.com/Article/details/ghsclxjcy.sHtML

[R70] 时间戳与互转
来源：http://read.share.zdbjq.cn/Article/details/gijzvazkb.sHtML

date +%s;  date -d @1700000000
来源：http://3g.hesvh.cn/Article/details/gjgjajiri.sHtML

[R71] 日期格式化
来源：http://3g.hesvh.cn/Article/details/gzqkklctn.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.zdbjq.cn/Article/details/gvjeapnre.sHtML

[R72] 等待端口就绪
来源：http://m.share.zdbjq.cn/Article/details/goxkbdxfo.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.hesvh.cn/Article/details/gpjgxiwei.sHtML

[R73] 分割大日志
来源：http://3g.zdbjq.cn/Article/details/ghkontitp.sHtML

split -l 1000 big.log part_
来源：http://3g.fehbvm.com/Article/details/gqubvkbfn.sHtML

[R74] 批量重命名
来源：http://m.share.hesvh.cn/Article/details/geanclifc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.hesvh.cn/Article/details/gbluyvslz.sHtML

[R75] 导出环境变量
来源：http://baike.zdbjq.cn/Article/details/giasdwxis.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fehbvm.com/Article/details/gnubmicyb.sHtML

[R76] 使用临时文件
来源：http://baike.hesvh.cn/Article/details/guxywfaek.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/gnhwzterq.sHtML

[R77] 读取用户输入
来源：http://m.share.fehbvm.com/Article/details/gckuqfjsx.sHtML

read -rp "请输入: " ans
来源：http://mobile.fehbvm.com/Article/details/gjarumleh.sHtML

[R78] 交互式菜单
来源：http://3g.zdbjq.cn/Article/details/gkovattxt.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.hesvh.cn/Article/details/gejunmyxs.sHtML

[R79] 解析命令行选项
来源：http://baike.zdbjq.cn/Article/details/grvhnhrde.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.hesvh.cn/Article/details/grjggphnh.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.zdbjq.cn/Article/details/givguumpg.sHtML

time ./run.sh
来源：http://www.m.share.zdbjq.cn/Article/details/gboixutom.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gprpnznvx.sHtML

S. C / C++ 专题
来源：http://wap.hesvh.cn/Article/details/gkofudatc.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ggnnrzshp.sHtML

[S01] C：Hello World
来源：http://mobile.fehbvm.com/Article/details/giycjyzzc.sHtML

#include <stdio.h>
来源：http://m.share.fehbvm.com/Article/details/gsnaqbdkd.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.hesvh.cn/Article/details/gnkahrrfk.sHtML

[S02] C：变量与格式化输出
来源：http://baike.fehbvm.com/Article/details/gursgjqzl.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.zdbjq.cn/Article/details/guztyorzb.sHtML

[S03] C：读入整数
来源：http://mobile.hesvh.cn/Article/details/gtzhfslji.sHtML

int x; scanf("%d", &x);
来源：http://wap.fehbvm.com/Article/details/gscoctsss.sHtML

[S04] C：字符串复制
来源：http://baike.hesvh.cn/Article/details/gmozkvnhj.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fehbvm.com/Article/details/ggtuthetx.sHtML

[S05] C：字符串长度
来源：http://mobile.zdbjq.cn/Article/details/ghtwvaosp.sHtML


<!-- 参考信息 -->