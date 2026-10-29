代发 wailian999

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://blog.zdbjq.cn/Article/details/gywecqckh.sHtML

[Q26] 计数
来源：http://read.share.fehbvm.com/Article/details/gamprcznu.sHtML

SELECT COUNT(*) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gyuutsoah.sHtML

[Q27] 条件计数
来源：http://www.m.share.fehbvm.com/Article/details/gaupwojbw.sHtML

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://3g.fehbvm.com/Article/details/gxmltpohm.sHtML

[Q28] 求和与平均
来源：http://wap.hesvh.cn/Article/details/gmmyjqkgp.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gowxailoi.sHtML

[Q29] 最大最小值
来源：http://www.m.share.zdbjq.cn/Article/details/gpygiqrao.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gfbfocxst.sHtML

[Q30] 分组统计
来源：http://3g.zdbjq.cn/Article/details/gymwxwunu.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://m.share.fehbvm.com/Article/details/gtwjcqemg.sHtML

[Q31] 分组后过滤
来源：http://3g.fehbvm.com/Article/details/gkxxaewij.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://3g.hesvh.cn/Article/details/gdvkibavt.sHtML

[Q32] 分组拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gfqrehief.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/gfwehpcyh.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://3g.hesvh.cn/Article/details/glauypmed.sHtML

[Q33] 多列分组
来源：http://blog.hesvh.cn/Article/details/gnaznkkkk.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://m.share.hesvh.cn/Article/details/guuxkmtjc.sHtML

[Q34] 每组取第一条
来源：http://www.share.zdbjq.cn/Article/details/gdeffwiln.sHtML

SELECT * FROM (
来源：http://www.m.share.hesvh.cn/Article/details/gydxlrdxl.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://blog.zdbjq.cn/Article/details/gewdlooez.sHtML

) t WHERE rn = 1;
来源：http://www.share.fehbvm.com/Article/details/gpmykqobx.sHtML

[Q35] 内连接
来源：http://3g.zdbjq.cn/Article/details/gogkyjeyw.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://blog.zdbjq.cn/Article/details/gvunjebjf.sHtML

[Q36] 左连接
来源：http://wap.fehbvm.com/Article/details/gkvcltwhq.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.hesvh.cn/Article/details/gswrtnutj.sHtML

[Q37] 右连接
来源：http://wap.hesvh.cn/Article/details/gmuxbcpmf.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.fehbvm.com/Article/details/gdggzlmvg.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.m.share.hesvh.cn/Article/details/gxxowcmwc.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://m.share.zdbjq.cn/Article/details/gwetpphpk.sHtML

[Q39] 自连接（查上下级）
来源：http://www.share.fehbvm.com/Article/details/gxmimnkhw.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://read.share.fehbvm.com/Article/details/gzpucnnlk.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://read.share.zdbjq.cn/Article/details/geglypxwj.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://mobile.hesvh.cn/Article/details/grhpysucc.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.share.hesvh.cn/Article/details/guwnvazsv.sHtML

[Q41] 多表连接
来源：http://blog.fehbvm.com/Article/details/gwcfnaqnl.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.fehbvm.com/Article/details/goywnwgoa.sHtML

JOIN users u ON u.id = o.user_id
来源：http://blog.hesvh.cn/Article/details/gldpsehdu.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://baike.fehbvm.com/Article/details/gwbwbpijr.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.hesvh.cn/Article/details/glcezdmnv.sHtML

SELECT u.name, o.amount FROM users u
来源：http://www.share.zdbjq.cn/Article/details/gbrgzxbuk.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.m.share.hesvh.cn/Article/details/gcgmwuaon.sHtML

[Q43] 标量子查询
来源：http://www.m.share.fehbvm.com/Article/details/gcvnivpim.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://mobile.hesvh.cn/Article/details/gxemfmiqj.sHtML

[Q44] IN 子查询
来源：http://baike.hesvh.cn/Article/details/ghthyyern.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://read.share.hesvh.cn/Article/details/gehzowhww.sHtML

[Q45] EXISTS 判断存在
来源：http://mobile.fehbvm.com/Article/details/gjfojelah.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://3g.hesvh.cn/Article/details/gqcyuqrwa.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://blog.hesvh.cn/Article/details/gibfgfnlm.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.fehbvm.com/Article/details/gnmzkfbph.sHtML

[Q47] 与平均值比较
来源：http://www.share.hesvh.cn/Article/details/giehoglgl.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.zdbjq.cn/Article/details/ggvjrndfc.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.hesvh.cn/Article/details/gybllbwus.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.blog.hesvh.cn/Article/details/giqbbsirg.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://mobile.hesvh.cn/Article/details/gisgugnnc.sHtML

[Q49] 更新单行
来源：http://www.share.zdbjq.cn/Article/details/gtydjtnqk.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://m.share.hesvh.cn/Article/details/goixjkajq.sHtML

[Q50] 批量更新
来源：http://mobile.hesvh.cn/Article/details/gubesiqwl.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.hesvh.cn/Article/details/goitcpwxz.sHtML

[Q51] 用子查询更新
来源：http://blog.fehbvm.com/Article/details/gizystrrl.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.blog.fehbvm.com/Article/details/glhmfdwbc.sHtML

[Q52] 删除指定行
来源：http://www.share.hesvh.cn/Article/details/gyiqmmkwm.sHtML

DELETE FROM users WHERE id = 10;
来源：http://mobile.fehbvm.com/Article/details/gegharxss.sHtML

[Q53] 按条件删除
来源：http://read.share.fehbvm.com/Article/details/govivqxqz.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://m.share.fehbvm.com/Article/details/grgxjlzpr.sHtML

[Q54] 清空表
来源：http://blog.fehbvm.com/Article/details/gzaaiglkx.sHtML

TRUNCATE TABLE logs;
来源：http://3g.hesvh.cn/Article/details/gxstmfnhl.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.zdbjq.cn/Article/details/gqtdrnwrl.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.hesvh.cn/Article/details/ghriqjggk.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.zdbjq.cn/Article/details/gjljpnubq.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://blog.hesvh.cn/Article/details/ggnremtvc.sHtML

[Q57] 行号
来源：http://www.blog.hesvh.cn/Article/details/gbqahwsdq.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://read.share.hesvh.cn/Article/details/ghgovbybu.sHtML

[Q58] 累计求和
来源：http://mobile.hesvh.cn/Article/details/gjnlnohrd.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.zdbjq.cn/Article/details/griowpqaq.sHtML

[Q59] 分组内累计
来源：http://www.m.share.fehbvm.com/Article/details/godrdzsfw.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gymvotswp.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.zdbjq.cn/Article/details/gszizgcyf.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://baike.zdbjq.cn/Article/details/geglgafpo.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://read.share.zdbjq.cn/Article/details/gnosctkjj.sHtML

[Q61] 移动平均
来源：http://mobile.fehbvm.com/Article/details/gvgybcrmf.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://mobile.fehbvm.com/Article/details/gmlgwzbfd.sHtML

[Q62] 分组占比
来源：http://wap.fehbvm.com/Article/details/gwxfqulpw.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/gjbrwcacl.sHtML

[Q63] 开启事务
来源：http://www.share.hesvh.cn/Article/details/gkutgxyjt.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.fehbvm.com/Article/details/gtbcexkoz.sHtML

[Q64] 提交事务
来源：http://3g.zdbjq.cn/Article/details/gbcpwlruu.sHtML

COMMIT;
来源：http://www.blog.fehbvm.com/Article/details/ghjlkfkbk.sHtML

[Q65] 回滚事务
来源：http://baike.hesvh.cn/Article/details/guouepnqz.sHtML

ROLLBACK;
来源：http://www.blog.hesvh.cn/Article/details/gchhwihyp.sHtML

[Q66] 行锁查询
来源：http://read.share.hesvh.cn/Article/details/gojusmjfv.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.hesvh.cn/Article/details/ggjzbeqzz.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.fehbvm.com/Article/details/gvucertlh.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://read.share.fehbvm.com/Article/details/gpdttqwkm.sHtML

[Q68] 保存点
来源：http://www.m.share.fehbvm.com/Article/details/gunbdjaxp.sHtML

SAVEPOINT sp1;
来源：http://www.blog.hesvh.cn/Article/details/gbflqvwbr.sHtML

ROLLBACK TO sp1;
来源：http://m.share.hesvh.cn/Article/details/gutwgraee.sHtML

[Q69] 查看执行计划
来源：http://baike.zdbjq.cn/Article/details/gdzgsifrx.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.fehbvm.com/Article/details/glynhnfkc.sHtML

[Q70] 更新统计信息
来源：http://wap.hesvh.cn/Article/details/gpgytplpu.sHtML

ANALYZE TABLE users;
来源：http://baike.zdbjq.cn/Article/details/gclsfjsci.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.zdbjq.cn/Article/details/glzojfned.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.zdbjq.cn/Article/details/gsqfcfbtn.sHtML

[Q72] 查看索引
来源：http://www.blog.zdbjq.cn/Article/details/gubjnqgcb.sHtML

SHOW INDEX FROM users;
来源：http://baike.hesvh.cn/Article/details/gdodrfgvh.sHtML

[Q73] 查看表状态
来源：http://www.share.zdbjq.cn/Article/details/gmnkoyyby.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://3g.zdbjq.cn/Article/details/gcncuznwk.sHtML

[Q74] 强制使用索引
来源：http://www.share.fehbvm.com/Article/details/gmihpgiyf.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.hesvh.cn/Article/details/guocwveqq.sHtML

[Q75] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/gsdnpmikh.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.blog.zdbjq.cn/Article/details/ghezyqxrc.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.fehbvm.com/Article/details/gmqcemfki.sHtML

[Q76] 按天统计
来源：http://blog.hesvh.cn/Article/details/gfyycncnt.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://wap.fehbvm.com/Article/details/gisfaewrb.sHtML

[Q77] 时间加减
来源：http://read.share.zdbjq.cn/Article/details/gnnovclqo.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://blog.fehbvm.com/Article/details/gcmmcxedx.sHtML

[Q78] 当前时间
来源：http://m.share.zdbjq.cn/Article/details/gxaxrwndn.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.zdbjq.cn/Article/details/glkaxbhmp.sHtML

[Q79] 字符串拼接
来源：http://baike.zdbjq.cn/Article/details/gsojifabm.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://baike.fehbvm.com/Article/details/gqlhuevia.sHtML

[Q80] 字符串截取
来源：http://www.m.share.fehbvm.com/Article/details/gvyjbxdru.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gunegwaxj.sHtML

[Q81] 字符串替换
来源：http://blog.fehbvm.com/Article/details/gvfzpkwla.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://baike.zdbjq.cn/Article/details/gvfwqrqrk.sHtML

[Q82] 字符长度与字节长度
来源：http://wap.zdbjq.cn/Article/details/ggbsffjrt.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://read.share.fehbvm.com/Article/details/gdgovsaii.sHtML

[Q83] 大小写转换
来源：http://read.share.zdbjq.cn/Article/details/glpsebmdd.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/guvuwyezi.sHtML

[Q84] 去除首尾空格
来源：http://blog.hesvh.cn/Article/details/gomktabat.sHtML

SELECT TRIM(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/gpfxywxcu.sHtML

[Q85] 数值取整
来源：http://wap.fehbvm.com/Article/details/gfvghrwuc.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.m.share.zdbjq.cn/Article/details/gxgyalhxz.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.hesvh.cn/Article/details/gqjjwhuts.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://wap.hesvh.cn/Article/details/gycuzalnl.sHtML

[Q87] JSON 字段做条件
来源：http://www.m.share.fehbvm.com/Article/details/gmpplzcay.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.zdbjq.cn/Article/details/gcwarflgx.sHtML

[Q88] 行转列（条件聚合）
来源：http://3g.hesvh.cn/Article/details/gosjbkrbq.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://3g.zdbjq.cn/Article/details/grlfnvwwx.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.zdbjq.cn/Article/details/gthaolfhr.sHtML

[Q89] 判断表是否存在
来源：http://blog.fehbvm.com/Article/details/gpkulfdrh.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://wap.hesvh.cn/Article/details/gjpmgdbrq.sHtML

[Q90] 生成序号列
来源：http://read.share.hesvh.cn/Article/details/gijsajbup.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://baike.zdbjq.cn/Article/details/goprzlmci.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gntiqtjaf.sHtML

R. Bash 专题
来源：http://blog.zdbjq.cn/Article/details/gprhwsfjj.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gdpvkyhlt.sHtML

[R01] shebang 与严格模式
来源：http://3g.fehbvm.com/Article/details/guzakbvjl.sHtML

#!/usr/bin/env bash
来源：http://mobile.hesvh.cn/Article/details/gnjpljyqe.sHtML

set -euo pipefail
来源：http://read.share.hesvh.cn/Article/details/gfwahvywn.sHtML

[R02] 变量赋值与使用
来源：http://baike.fehbvm.com/Article/details/giqdlhgur.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fehbvm.com/Article/details/glbeodzch.sHtML

[R03] 只读变量
来源：http://baike.zdbjq.cn/Article/details/gnxrjokya.sHtML

readonly PI=3.14
来源：http://www.m.share.fehbvm.com/Article/details/gonxmmlhh.sHtML

[R04] 位置参数
来源：http://mobile.hesvh.cn/Article/details/guefkosqr.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.zdbjq.cn/Article/details/gbyzoynrp.sHtML

[R05] 参数默认值
来源：http://3g.zdbjq.cn/Article/details/gllguhbyk.sHtML

name="${1:-default}"
来源：http://read.share.zdbjq.cn/Article/details/gayqjmzcd.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.hesvh.cn/Article/details/galvuyvtm.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.m.share.fehbvm.com/Article/details/gwgnsbjth.sHtML

[R07] if 判断文件
来源：http://www.blog.zdbjq.cn/Article/details/grmixcvqg.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fehbvm.com/Article/details/gksdvceen.sHtML

[R08] 数值比较
来源：http://www.blog.fehbvm.com/Article/details/gmvgnijlq.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://3g.fehbvm.com/Article/details/gulbyabkx.sHtML

[R09] 字符串比较
来源：http://mobile.zdbjq.cn/Article/details/gjjdeyzhg.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gbyhdxwyk.sHtML

[R10] 正则匹配
来源：http://blog.zdbjq.cn/Article/details/ghgvsvoli.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.share.fehbvm.com/Article/details/gykjjcerz.sHtML

[R11] case 多分支
来源：http://read.share.fehbvm.com/Article/details/gwgtpwwth.sHtML

case "$1" in
来源：http://m.share.fehbvm.com/Article/details/gdvzrgiwt.sHtML

start) echo "启动" ;;
来源：http://read.share.zdbjq.cn/Article/details/gqbaznpgd.sHtML

stop)  echo "停止" ;;
来源：http://mobile.hesvh.cn/Article/details/gtewpvbde.sHtML

*)     echo "未知命令" ;;
来源：http://blog.fehbvm.com/Article/details/ghqjelstf.sHtML

esac
来源：http://3g.zdbjq.cn/Article/details/gehlygykr.sHtML

[R12] for 遍历文件
来源：http://www.m.share.hesvh.cn/Article/details/gyojjlynz.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.hesvh.cn/Article/details/gnxykgtsb.sHtML

[R13] for 计数循环
来源：http://blog.fehbvm.com/Article/details/guxtgvnun.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fehbvm.com/Article/details/geuufnpqf.sHtML

[R14] C 风格 for
来源：http://read.share.hesvh.cn/Article/details/gfbgvvyms.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.hesvh.cn/Article/details/gzavdjird.sHtML

[R15] while 逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gmzntarvb.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.fehbvm.com/Article/details/gwcdmgtaf.sHtML

[R16] until 等待条件
来源：http://www.blog.fehbvm.com/Article/details/gpjhvahke.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.fehbvm.com/Article/details/gmijgmoxb.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.hesvh.cn/Article/details/gnwcgwiwa.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.zdbjq.cn/Article/details/gmgrzsspu.sHtML

[R18] 遍历数组
来源：http://www.blog.fehbvm.com/Article/details/gpacomktf.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://baike.zdbjq.cn/Article/details/gzfuzwidg.sHtML

[R19] 数组长度
来源：http://wap.fehbvm.com/Article/details/gkzbgcwik.sHtML

echo "${#arr[@]}"
来源：http://read.share.hesvh.cn/Article/details/gvlrgfnrn.sHtML

[R20] 关联数组（字典）
来源：http://www.share.zdbjq.cn/Article/details/gkmdbsffu.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fehbvm.com/Article/details/gynfnqohl.sHtML

[R21] 字符串长度
来源：http://www.m.share.fehbvm.com/Article/details/gxsagdbeb.sHtML

echo "${#s}"
来源：http://3g.hesvh.cn/Article/details/gutkatfem.sHtML

[R22] 截取子串
来源：http://baike.hesvh.cn/Article/details/guoedeczt.sHtML

echo "${s:0:5}"
来源：http://www.m.share.hesvh.cn/Article/details/gyoixqrqr.sHtML

[R23] 字符串替换
来源：http://m.share.zdbjq.cn/Article/details/gpodiehlf.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.zdbjq.cn/Article/details/gjlchieht.sHtML

[R24] 大小写转换
来源：http://m.share.fehbvm.com/Article/details/gfwquimhu.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fehbvm.com/Article/details/gkliqlnkn.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.zdbjq.cn/Article/details/ghnothtto.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.zdbjq.cn/Article/details/gmzyaclij.sHtML

[R26] 命令替换
来源：http://m.share.zdbjq.cn/Article/details/gavirbvpd.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.hesvh.cn/Article/details/gucssskhu.sHtML

[R27] 算术展开
来源：http://www.blog.zdbjq.cn/Article/details/ghupmfeyy.sHtML

echo $((1 + 2 * 3))
来源：http://wap.hesvh.cn/Article/details/gckrvbhdv.sHtML

[R28] 浮点运算
来源：http://wap.hesvh.cn/Article/details/ggzdhmnhs.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.fehbvm.com/Article/details/gryffvyve.sHtML

[R29] 定义函数
来源：http://3g.fehbvm.com/Article/details/geseeqglt.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://mobile.zdbjq.cn/Article/details/gpcrisuwc.sHtML

[R30] 函数返回状态码
来源：http://wap.hesvh.cn/Article/details/gzkmwhkpz.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://wap.hesvh.cn/Article/details/gnexngboh.sHtML

[R31] 局部变量
来源：http://mobile.zdbjq.cn/Article/details/gajlpoawk.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.zdbjq.cn/Article/details/gxhiymiah.sHtML

[R32] 参数个数校验
来源：http://baike.hesvh.cn/Article/details/gveotuuuv.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://blog.fehbvm.com/Article/details/gqdykknkr.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fehbvm.com/Article/details/gusiyndxs.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.zdbjq.cn/Article/details/garchguox.sHtML

[R34] 退出时清理
来源：http://m.share.hesvh.cn/Article/details/goehukzpj.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/gufaexhaz.sHtML

[R35] 后台执行并等待
来源：http://wap.fehbvm.com/Article/details/ghnwpnozw.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://baike.hesvh.cn/Article/details/ggxibcgwk.sHtML

[R36] 并发执行多个任务
来源：http://baike.fehbvm.com/Article/details/gvfztinco.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fehbvm.com/Article/details/glxddufiw.sHtML

[R37] 把输出赋给变量
来源：http://www.m.share.fehbvm.com/Article/details/gasgwtxhs.sHtML

files=$(ls -1)
来源：http://wap.fehbvm.com/Article/details/gfmxqlmif.sHtML

[R38] 管道串联
来源：http://mobile.fehbvm.com/Article/details/ghfiuzdkx.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fehbvm.com/Article/details/geoegiqhu.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.hesvh.cn/Article/details/gmbcewski.sHtML

cmd > out.log 2>&1
来源：http://baike.hesvh.cn/Article/details/gxkuwnvaq.sHtML

[R40] 追加写日志
来源：http://blog.fehbvm.com/Article/details/givmzxycg.sHtML

echo "log" >> out.log
来源：http://www.share.zdbjq.cn/Article/details/gyvcubskg.sHtML

[R41] 丢弃输出
来源：http://3g.zdbjq.cn/Article/details/gnodnuzcs.sHtML

cmd >/dev/null 2>&1
来源：http://read.share.fehbvm.com/Article/details/gizvcmwpm.sHtML

[R42] 输入重定向
来源：http://m.share.zdbjq.cn/Article/details/gwrqdxeil.sHtML

wc -l < a.txt
来源：http://www.share.hesvh.cn/Article/details/gligdbhuc.sHtML

[R43] 按名字查找文件
来源：http://read.share.hesvh.cn/Article/details/gzpyvquxz.sHtML

find . -name "*.log" -type f
来源：http://blog.fehbvm.com/Article/details/gwkcwduvd.sHtML

[R44] 按修改时间查找
来源：http://wap.fehbvm.com/Article/details/gzsqrmjgz.sHtML

find . -mtime -7 -type f
来源：http://mobile.hesvh.cn/Article/details/ghbgddayj.sHtML

[R45] 批量删除
来源：http://m.share.fehbvm.com/Article/details/galcnrrun.sHtML

find . -name "*.tmp" -delete
来源：http://3g.fehbvm.com/Article/details/gapxhypqv.sHtML

[R46] 递归替换文件内容
来源：http://www.share.hesvh.cn/Article/details/gjlfubjpz.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fehbvm.com/Article/details/grkdhkgvm.sHtML

[R47] sed 单行替换
来源：http://mobile.zdbjq.cn/Article/details/gmlijwmzp.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://m.share.hesvh.cn/Article/details/gvlvzmpuh.sHtML

[R48] awk 取指定列
来源：http://baike.zdbjq.cn/Article/details/gtdknmdhf.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.hesvh.cn/Article/details/gbsqfbpgb.sHtML

[R49] awk 带条件
来源：http://www.blog.zdbjq.cn/Article/details/gejshlnfp.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.zdbjq.cn/Article/details/gavtqqjdg.sHtML

[R50] awk 求和
来源：http://blog.fehbvm.com/Article/details/gugzkosye.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.hesvh.cn/Article/details/glinjsekq.sHtML

[R51] 排序去重取前几
来源：http://m.share.zdbjq.cn/Article/details/gmydixsfs.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.hesvh.cn/Article/details/gqemgyatp.sHtML

[R52] 统计行数
来源：http://wap.hesvh.cn/Article/details/gnuydbrxz.sHtML

wc -l a.txt
来源：http://read.share.zdbjq.cn/Article/details/gzjvtnryy.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.hesvh.cn/Article/details/gnwghgajr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.hesvh.cn/Article/details/gpiyxuztd.sHtML

[R54] 比较两个文件
来源：http://www.blog.fehbvm.com/Article/details/gzwahwegm.sHtML

diff a.txt b.txt
来源：http://www.share.fehbvm.com/Article/details/gjdvzcvzx.sHtML

[R55] 压缩与解压
来源：http://www.blog.hesvh.cn/Article/details/ggmuagukh.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.hesvh.cn/Article/details/gugglqpzk.sHtML

[R56] 远程拷贝
来源：http://m.share.zdbjq.cn/Article/details/glyikwrjb.sHtML

scp file user@host:/path/
来源：http://mobile.hesvh.cn/Article/details/gialytpod.sHtML

[R57] 远程执行命令
来源：http://3g.hesvh.cn/Article/details/gdiugxfgn.sHtML

ssh user@host 'uptime'
来源：http://mobile.hesvh.cn/Article/details/geuppslfa.sHtML

[R58] 下载文件
来源：http://mobile.hesvh.cn/Article/details/gkhulbpcu.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.hesvh.cn/Article/details/gxfbpvume.sHtML

[R59] 发 POST JSON
来源：http://3g.hesvh.cn/Article/details/gtgspinuv.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fehbvm.com/Article/details/gdpcqmpri.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.hesvh.cn/Article/details/gwdgqhctp.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.zdbjq.cn/Article/details/gcjrnlijx.sHtML

[R61] 磁盘占用
来源：http://3g.hesvh.cn/Article/details/ghrdtjqos.sHtML

df -h;  du -sh *
来源：http://mobile.hesvh.cn/Article/details/ggjblhrxh.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.zdbjq.cn/Article/details/gqwyyirko.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.hesvh.cn/Article/details/ghcdolnpb.sHtML

[R63] 内存与进程
来源：http://www.share.zdbjq.cn/Article/details/gdlkzebdr.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.fehbvm.com/Article/details/gzxkutfmh.sHtML

[R64] 结束进程
来源：http://www.blog.fehbvm.com/Article/details/ghjtbiryc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fehbvm.com/Article/details/gohodrjpo.sHtML

[R65] 查看端口占用
来源：http://www.share.fehbvm.com/Article/details/guntqozcv.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fehbvm.com/Article/details/gaidyyuqw.sHtML

[R66] 定时任务
来源：http://baike.zdbjq.cn/Article/details/gboyfuoey.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.zdbjq.cn/Article/details/gyjmqtyfr.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fehbvm.com/Article/details/gifqrejpy.sHtML

openssl rand -hex 16
来源：http://mobile.fehbvm.com/Article/details/gekcdzcmu.sHtML

[R68] 计算文件校验值
来源：http://m.share.fehbvm.com/Article/details/gjceoorao.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.hesvh.cn/Article/details/gihahxxeg.sHtML

[R69] 生成随机密码
来源：http://m.share.zdbjq.cn/Article/details/gdgsamvpe.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.hesvh.cn/Article/details/gttzactjw.sHtML

[R70] 时间戳与互转
来源：http://baike.hesvh.cn/Article/details/gptdygrdy.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.zdbjq.cn/Article/details/ggmwbpudk.sHtML

[R71] 日期格式化
来源：http://wap.zdbjq.cn/Article/details/gzvtriobc.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.hesvh.cn/Article/details/gfapcisvd.sHtML

[R72] 等待端口就绪
来源：http://mobile.hesvh.cn/Article/details/gzbylharc.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.zdbjq.cn/Article/details/gzrudkgzb.sHtML

[R73] 分割大日志
来源：http://read.share.fehbvm.com/Article/details/gwvqqtwcj.sHtML

split -l 1000 big.log part_
来源：http://www.share.hesvh.cn/Article/details/guqmrnayv.sHtML

[R74] 批量重命名
来源：http://mobile.hesvh.cn/Article/details/gnkzintbr.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fehbvm.com/Article/details/glenalwii.sHtML

[R75] 导出环境变量
来源：http://3g.fehbvm.com/Article/details/gbuqlqjlk.sHtML


<!-- 参考信息 -->