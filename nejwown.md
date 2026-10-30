代发 wailian999

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://baike.hesvh.cn/Article/details/gjxsuroxd.sHtML

[Q28] 求和与平均
来源：http://blog.hesvh.cn/Article/details/gqzjutrbh.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/ghkgsvwhe.sHtML

[Q29] 最大最小值
来源：http://3g.hesvh.cn/Article/details/gwnklolxj.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.share.zdbjq.cn/Article/details/geiymtrhy.sHtML

[Q30] 分组统计
来源：http://read.share.hesvh.cn/Article/details/gyxzedjsm.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://3g.hesvh.cn/Article/details/gyasgsysd.sHtML

[Q31] 分组后过滤
来源：http://www.share.hesvh.cn/Article/details/gbxswbqgy.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.zdbjq.cn/Article/details/gmeivgsqb.sHtML

[Q32] 分组拼接字符串
来源：http://www.share.hesvh.cn/Article/details/ghsuwnnrz.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.blog.hesvh.cn/Article/details/ginqcnfzh.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.zdbjq.cn/Article/details/gbfbejhrf.sHtML

[Q33] 多列分组
来源：http://m.share.hesvh.cn/Article/details/gevvhceka.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://read.share.fehbvm.com/Article/details/gthhoakln.sHtML

[Q34] 每组取第一条
来源：http://baike.zdbjq.cn/Article/details/gnkqmpcef.sHtML

SELECT * FROM (
来源：http://www.blog.fehbvm.com/Article/details/gooeleeuv.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.blog.hesvh.cn/Article/details/gcyclhiue.sHtML

) t WHERE rn = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gvqchjucx.sHtML

[Q35] 内连接
来源：http://www.share.fehbvm.com/Article/details/ghjvuyymr.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://mobile.zdbjq.cn/Article/details/gdpnfkspc.sHtML

[Q36] 左连接
来源：http://www.blog.zdbjq.cn/Article/details/gekxkphxn.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://blog.hesvh.cn/Article/details/gboargrcg.sHtML

[Q37] 右连接
来源：http://read.share.hesvh.cn/Article/details/gdgwmudzr.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://mobile.hesvh.cn/Article/details/gdnarjayf.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.zdbjq.cn/Article/details/gbchhqjkd.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://wap.fehbvm.com/Article/details/gnkxqkfvz.sHtML

[Q39] 自连接（查上下级）
来源：http://www.blog.hesvh.cn/Article/details/guzrtcrdo.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://mobile.hesvh.cn/Article/details/gbizobjzb.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.m.share.zdbjq.cn/Article/details/gvmwhvabt.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.share.fehbvm.com/Article/details/gnguonnpw.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.hesvh.cn/Article/details/gbfghxond.sHtML

[Q41] 多表连接
来源：http://www.blog.zdbjq.cn/Article/details/gjbqdlugc.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.share.fehbvm.com/Article/details/gbiaqfchs.sHtML

JOIN users u ON u.id = o.user_id
来源：http://www.share.hesvh.cn/Article/details/gndznnqlw.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://read.share.hesvh.cn/Article/details/gygsjexof.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.hesvh.cn/Article/details/gqkdmrdnd.sHtML

SELECT u.name, o.amount FROM users u
来源：http://baike.fehbvm.com/Article/details/gsspqrnvo.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://m.share.hesvh.cn/Article/details/gywrqdizg.sHtML

[Q43] 标量子查询
来源：http://www.m.share.fehbvm.com/Article/details/gbzlvthur.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://wap.fehbvm.com/Article/details/gghvhurrh.sHtML

[Q44] IN 子查询
来源：http://www.m.share.zdbjq.cn/Article/details/gbhynexkm.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://3g.zdbjq.cn/Article/details/gnwenbfim.sHtML

[Q45] EXISTS 判断存在
来源：http://www.blog.fehbvm.com/Article/details/gpixuemsa.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.blog.hesvh.cn/Article/details/gtmnjohsh.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.hesvh.cn/Article/details/gvdmuzulb.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.zdbjq.cn/Article/details/gkuverjep.sHtML

[Q47] 与平均值比较
来源：http://www.m.share.hesvh.cn/Article/details/ginayenhg.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://m.share.fehbvm.com/Article/details/glfanainw.sHtML

[Q48] CTE 公用表表达式
来源：http://www.share.hesvh.cn/Article/details/gmwxwhdmp.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.zdbjq.cn/Article/details/grsvnzsrh.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.zdbjq.cn/Article/details/garpkkpsx.sHtML

[Q49] 更新单行
来源：http://baike.hesvh.cn/Article/details/guwpyuaqt.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://mobile.fehbvm.com/Article/details/gauzgqvnk.sHtML

[Q50] 批量更新
来源：http://wap.fehbvm.com/Article/details/gokvdarok.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.share.hesvh.cn/Article/details/gapodwuqd.sHtML

[Q51] 用子查询更新
来源：http://m.share.zdbjq.cn/Article/details/gqjvbeohu.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://mobile.fehbvm.com/Article/details/gcrzrtsyu.sHtML

[Q52] 删除指定行
来源：http://m.share.fehbvm.com/Article/details/gvhacpffc.sHtML

DELETE FROM users WHERE id = 10;
来源：http://wap.zdbjq.cn/Article/details/gdjumglcq.sHtML

[Q53] 按条件删除
来源：http://3g.fehbvm.com/Article/details/gvvwfgxbs.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://read.share.hesvh.cn/Article/details/gakwlfaxy.sHtML

[Q54] 清空表
来源：http://3g.hesvh.cn/Article/details/girmzozcl.sHtML

TRUNCATE TABLE logs;
来源：http://www.share.zdbjq.cn/Article/details/gerpwwaax.sHtML

[Q55] 排名（并列占位）
来源：http://mobile.fehbvm.com/Article/details/gxotimnfl.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.m.share.hesvh.cn/Article/details/gwsnmtetp.sHtML

[Q56] 密集排名（并列不占位）
来源：http://3g.zdbjq.cn/Article/details/ghmzspxem.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://wap.fehbvm.com/Article/details/gkvqwjzwf.sHtML

[Q57] 行号
来源：http://www.m.share.fehbvm.com/Article/details/gzbgykyyc.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.fehbvm.com/Article/details/gerdxzeow.sHtML

[Q58] 累计求和
来源：http://3g.hesvh.cn/Article/details/gewipcsor.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://read.share.fehbvm.com/Article/details/grjnuvaur.sHtML

[Q59] 分组内累计
来源：http://blog.zdbjq.cn/Article/details/govbwxmii.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.fehbvm.com/Article/details/gghipizqn.sHtML

[Q60] 取上一行 / 下一行
来源：http://blog.fehbvm.com/Article/details/gcpeiwpqu.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.m.share.zdbjq.cn/Article/details/gtcrgbhnq.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.share.hesvh.cn/Article/details/gtrbkjvrm.sHtML

[Q61] 移动平均
来源：http://m.share.hesvh.cn/Article/details/gjnoscilh.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gvglxmxzh.sHtML

[Q62] 分组占比
来源：http://m.share.zdbjq.cn/Article/details/gpwhtwhid.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://wap.fehbvm.com/Article/details/gnzspiiky.sHtML

[Q63] 开启事务
来源：http://www.share.hesvh.cn/Article/details/gwpdxefgy.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.zdbjq.cn/Article/details/geyomtfxt.sHtML

[Q64] 提交事务
来源：http://baike.fehbvm.com/Article/details/gehulfsam.sHtML

COMMIT;
来源：http://baike.fehbvm.com/Article/details/gbqxxqgkh.sHtML

[Q65] 回滚事务
来源：http://read.share.hesvh.cn/Article/details/gqjkzlndz.sHtML

ROLLBACK;
来源：http://3g.zdbjq.cn/Article/details/grgbmwjqz.sHtML

[Q66] 行锁查询
来源：http://mobile.hesvh.cn/Article/details/gbvmudnjw.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://read.share.hesvh.cn/Article/details/gqywajmav.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.hesvh.cn/Article/details/gugnaoron.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.hesvh.cn/Article/details/gimtqtaim.sHtML

[Q68] 保存点
来源：http://read.share.fehbvm.com/Article/details/gazwxfxmp.sHtML

SAVEPOINT sp1;
来源：http://www.blog.fehbvm.com/Article/details/garkuuiea.sHtML

ROLLBACK TO sp1;
来源：http://www.share.zdbjq.cn/Article/details/gkkopieks.sHtML

[Q69] 查看执行计划
来源：http://blog.hesvh.cn/Article/details/gcwvnhdzh.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.blog.hesvh.cn/Article/details/gchahpyum.sHtML

[Q70] 更新统计信息
来源：http://www.blog.hesvh.cn/Article/details/guktioxax.sHtML

ANALYZE TABLE users;
来源：http://3g.fehbvm.com/Article/details/gawjtezon.sHtML

[Q71] 查看建表语句
来源：http://www.blog.hesvh.cn/Article/details/gosutpcit.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fehbvm.com/Article/details/ghzxbpilx.sHtML

[Q72] 查看索引
来源：http://wap.fehbvm.com/Article/details/gjmuldhje.sHtML

SHOW INDEX FROM users;
来源：http://mobile.fehbvm.com/Article/details/ggrnhlexf.sHtML

[Q73] 查看表状态
来源：http://www.m.share.fehbvm.com/Article/details/gzreirtmt.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://read.share.fehbvm.com/Article/details/gpbdoxmwg.sHtML

[Q74] 强制使用索引
来源：http://www.blog.hesvh.cn/Article/details/gqafiutly.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://read.share.hesvh.cn/Article/details/gjtjqslcg.sHtML

[Q75] 日期格式化
来源：http://mobile.zdbjq.cn/Article/details/gbfapjmmj.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://blog.zdbjq.cn/Article/details/grwppnufc.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://3g.hesvh.cn/Article/details/gwvdudrdx.sHtML

[Q76] 按天统计
来源：http://www.blog.fehbvm.com/Article/details/gjuvlorvj.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://read.share.fehbvm.com/Article/details/gdirypatr.sHtML

[Q77] 时间加减
来源：http://wap.hesvh.cn/Article/details/gqyocdtbk.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.m.share.hesvh.cn/Article/details/gjvswheff.sHtML

[Q78] 当前时间
来源：http://read.share.fehbvm.com/Article/details/gyzckvryr.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://mobile.zdbjq.cn/Article/details/goyiyyptf.sHtML

[Q79] 字符串拼接
来源：http://mobile.fehbvm.com/Article/details/gxbeesivg.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.m.share.fehbvm.com/Article/details/gmlwhdmds.sHtML

[Q80] 字符串截取
来源：http://wap.zdbjq.cn/Article/details/ggbgjnuik.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://baike.fehbvm.com/Article/details/gqndvhmlb.sHtML

[Q81] 字符串替换
来源：http://3g.zdbjq.cn/Article/details/gfdimnfie.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://wap.zdbjq.cn/Article/details/genpzqcen.sHtML

[Q82] 字符长度与字节长度
来源：http://3g.fehbvm.com/Article/details/gezvyeoeg.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://blog.hesvh.cn/Article/details/gutvnwihc.sHtML

[Q83] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/gpzjhjsvf.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://mobile.zdbjq.cn/Article/details/gvrgwdxom.sHtML

[Q84] 去除首尾空格
来源：http://mobile.hesvh.cn/Article/details/gpkoibivw.sHtML

SELECT TRIM(name) FROM users;
来源：http://baike.fehbvm.com/Article/details/glkaudukm.sHtML

[Q85] 数值取整
来源：http://wap.hesvh.cn/Article/details/gnxfbkvdp.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.fehbvm.com/Article/details/gmlqtqokh.sHtML

[Q86] 读取 JSON 字段
来源：http://baike.hesvh.cn/Article/details/gkppigkvr.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.m.share.hesvh.cn/Article/details/gjkaauywc.sHtML

[Q87] JSON 字段做条件
来源：http://read.share.hesvh.cn/Article/details/guetiocjf.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://baike.fehbvm.com/Article/details/gdrghwmma.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.fehbvm.com/Article/details/gfozbsoym.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://baike.fehbvm.com/Article/details/glqpykvtm.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://baike.fehbvm.com/Article/details/gztzvjbuq.sHtML

[Q89] 判断表是否存在
来源：http://www.m.share.hesvh.cn/Article/details/giscitwrh.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fehbvm.com/Article/details/gwmtrbyts.sHtML

[Q90] 生成序号列
来源：http://mobile.hesvh.cn/Article/details/gxqczeond.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://blog.fehbvm.com/Article/details/gotpzuiwd.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gnxtgiflt.sHtML

R. Bash 专题
来源：http://blog.hesvh.cn/Article/details/gttgqcqju.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gkkpvyvvp.sHtML

[R01] shebang 与严格模式
来源：http://baike.hesvh.cn/Article/details/gzelnzmfi.sHtML

#!/usr/bin/env bash
来源：http://m.share.hesvh.cn/Article/details/gaqaprrzi.sHtML

set -euo pipefail
来源：http://blog.hesvh.cn/Article/details/gkgvrltrv.sHtML

[R02] 变量赋值与使用
来源：http://m.share.fehbvm.com/Article/details/guusnjclw.sHtML

name="Tom"; echo "$name"
来源：http://mobile.fehbvm.com/Article/details/gmrdjwamj.sHtML

[R03] 只读变量
来源：http://mobile.hesvh.cn/Article/details/gwwxfbfsu.sHtML

readonly PI=3.14
来源：http://blog.zdbjq.cn/Article/details/gntfgmnbp.sHtML

[R04] 位置参数
来源：http://3g.fehbvm.com/Article/details/gedvahvxk.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://read.share.hesvh.cn/Article/details/gjpfmqwxq.sHtML

[R05] 参数默认值
来源：http://www.blog.fehbvm.com/Article/details/gwwnoonff.sHtML

name="${1:-default}"
来源：http://mobile.hesvh.cn/Article/details/gbyoqxfcu.sHtML

[R06] 判断命令是否存在
来源：http://www.m.share.zdbjq.cn/Article/details/gonhdfarm.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.fehbvm.com/Article/details/gdjtqlyhh.sHtML

[R07] if 判断文件
来源：http://read.share.zdbjq.cn/Article/details/gzzdxbatx.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.hesvh.cn/Article/details/govzydjlq.sHtML

[R08] 数值比较
来源：http://www.m.share.hesvh.cn/Article/details/giikiacjy.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.m.share.fehbvm.com/Article/details/gkzqruswq.sHtML

[R09] 字符串比较
来源：http://baike.hesvh.cn/Article/details/gcazwedjr.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.zdbjq.cn/Article/details/gevynqoqr.sHtML

[R10] 正则匹配
来源：http://3g.hesvh.cn/Article/details/gewabvzdh.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://read.share.hesvh.cn/Article/details/gmltlyxax.sHtML

[R11] case 多分支
来源：http://blog.zdbjq.cn/Article/details/gfuyrfplw.sHtML

case "$1" in
来源：http://www.blog.hesvh.cn/Article/details/gbcjqlani.sHtML

start) echo "启动" ;;
来源：http://m.share.fehbvm.com/Article/details/gbvlhiahe.sHtML

stop)  echo "停止" ;;
来源：http://www.share.zdbjq.cn/Article/details/gmctchzfd.sHtML

*)     echo "未知命令" ;;
来源：http://m.share.fehbvm.com/Article/details/geydibejd.sHtML

esac
来源：http://m.share.fehbvm.com/Article/details/guttajmsr.sHtML

[R12] for 遍历文件
来源：http://wap.hesvh.cn/Article/details/gzrkohyoz.sHtML

for f in *.txt; do echo "$f"; done
来源：http://wap.zdbjq.cn/Article/details/gcwyquvef.sHtML

[R13] for 计数循环
来源：http://www.blog.zdbjq.cn/Article/details/giasacfpm.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gzzjygzbh.sHtML

[R14] C 风格 for
来源：http://blog.zdbjq.cn/Article/details/ghxnqoiex.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fehbvm.com/Article/details/gnjkjzlsi.sHtML

[R15] while 逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gqypvjkbm.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://m.share.zdbjq.cn/Article/details/gnajftfuv.sHtML

[R16] until 等待条件
来源：http://3g.hesvh.cn/Article/details/gnkfruvnd.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/garromouw.sHtML

[R17] 数组定义与取值
来源：http://wap.hesvh.cn/Article/details/gggjwinol.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.hesvh.cn/Article/details/gilxdtnny.sHtML

[R18] 遍历数组
来源：http://wap.hesvh.cn/Article/details/gtdnsudhv.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://mobile.hesvh.cn/Article/details/gujgvyokf.sHtML

[R19] 数组长度
来源：http://www.m.share.fehbvm.com/Article/details/glwlomgqv.sHtML

echo "${#arr[@]}"
来源：http://www.blog.zdbjq.cn/Article/details/gnsnscyve.sHtML

[R20] 关联数组（字典）
来源：http://mobile.hesvh.cn/Article/details/gjwevgqdl.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.fehbvm.com/Article/details/gibuvvgol.sHtML

[R21] 字符串长度
来源：http://wap.hesvh.cn/Article/details/gthkjdehz.sHtML

echo "${#s}"
来源：http://www.share.fehbvm.com/Article/details/guootmqln.sHtML

[R22] 截取子串
来源：http://www.blog.hesvh.cn/Article/details/gfmylxemt.sHtML

echo "${s:0:5}"
来源：http://www.share.zdbjq.cn/Article/details/gemxobczh.sHtML

[R23] 字符串替换
来源：http://3g.fehbvm.com/Article/details/giqvpctql.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.hesvh.cn/Article/details/ggzsqnbpw.sHtML

[R24] 大小写转换
来源：http://www.blog.hesvh.cn/Article/details/gxogyfarq.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.hesvh.cn/Article/details/gkladerpv.sHtML

[R25] 去后缀 / 去前缀
来源：http://mobile.hesvh.cn/Article/details/ghgwotcmq.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fehbvm.com/Article/details/gmddndfzr.sHtML

[R26] 命令替换
来源：http://mobile.zdbjq.cn/Article/details/gfmqzgljz.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.hesvh.cn/Article/details/gkagybjxb.sHtML

[R27] 算术展开
来源：http://blog.fehbvm.com/Article/details/geacnavvh.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.hesvh.cn/Article/details/gdpgeonnr.sHtML

[R28] 浮点运算
来源：http://baike.hesvh.cn/Article/details/gcscyhfyf.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.hesvh.cn/Article/details/gmuyeqhpz.sHtML

[R29] 定义函数
来源：http://www.m.share.fehbvm.com/Article/details/gsxpilojp.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://blog.hesvh.cn/Article/details/gidkmutgo.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gmzjtqyxw.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.zdbjq.cn/Article/details/gkkhcuskb.sHtML

[R31] 局部变量
来源：http://m.share.zdbjq.cn/Article/details/gdoglbntn.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fehbvm.com/Article/details/gjqpgfqpd.sHtML

[R32] 参数个数校验
来源：http://read.share.fehbvm.com/Article/details/gpukdzzio.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fehbvm.com/Article/details/gbuxjlkpn.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.hesvh.cn/Article/details/gipocfopy.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.share.hesvh.cn/Article/details/gbhbqxeno.sHtML

[R34] 退出时清理
来源：http://read.share.fehbvm.com/Article/details/gaallxcxo.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.zdbjq.cn/Article/details/gqjunnfcb.sHtML

[R35] 后台执行并等待
来源：http://www.m.share.hesvh.cn/Article/details/gccegxrbt.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fehbvm.com/Article/details/gbbuwuhzm.sHtML

[R36] 并发执行多个任务
来源：http://blog.zdbjq.cn/Article/details/gcquzrrej.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.zdbjq.cn/Article/details/ghcfmbluz.sHtML

[R37] 把输出赋给变量
来源：http://baike.zdbjq.cn/Article/details/gzzlwbzob.sHtML

files=$(ls -1)
来源：http://m.share.hesvh.cn/Article/details/gbuxsmqbd.sHtML

[R38] 管道串联
来源：http://m.share.zdbjq.cn/Article/details/gvrxqxyhw.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fehbvm.com/Article/details/gqocpcxbd.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.zdbjq.cn/Article/details/gcbjgbjkh.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.zdbjq.cn/Article/details/gbzyqdoci.sHtML

[R40] 追加写日志
来源：http://www.m.share.fehbvm.com/Article/details/grhpabowb.sHtML

echo "log" >> out.log
来源：http://blog.fehbvm.com/Article/details/gkjrgdngu.sHtML

[R41] 丢弃输出
来源：http://www.m.share.fehbvm.com/Article/details/gdgiwwmrd.sHtML

cmd >/dev/null 2>&1
来源：http://baike.fehbvm.com/Article/details/gadxsrzlw.sHtML

[R42] 输入重定向
来源：http://www.m.share.zdbjq.cn/Article/details/gecovxsdz.sHtML

wc -l < a.txt
来源：http://mobile.zdbjq.cn/Article/details/glodjserd.sHtML

[R43] 按名字查找文件
来源：http://m.share.hesvh.cn/Article/details/gjaqczyrl.sHtML

find . -name "*.log" -type f
来源：http://blog.fehbvm.com/Article/details/gcuufkslm.sHtML

[R44] 按修改时间查找
来源：http://blog.hesvh.cn/Article/details/gccprthro.sHtML

find . -mtime -7 -type f
来源：http://wap.zdbjq.cn/Article/details/gwakwdefb.sHtML

[R45] 批量删除
来源：http://3g.fehbvm.com/Article/details/gkhxukkba.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.hesvh.cn/Article/details/gkfpkprqi.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.zdbjq.cn/Article/details/grexaqhtf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.hesvh.cn/Article/details/ggezwknft.sHtML

[R47] sed 单行替换
来源：http://www.share.hesvh.cn/Article/details/giaofblms.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.hesvh.cn/Article/details/glquysnld.sHtML

[R48] awk 取指定列
来源：http://m.share.hesvh.cn/Article/details/gbikqualz.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.hesvh.cn/Article/details/gysoiaoed.sHtML

[R49] awk 带条件
来源：http://mobile.hesvh.cn/Article/details/gpuvcjabv.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.hesvh.cn/Article/details/gwhhfieek.sHtML

[R50] awk 求和
来源：http://blog.hesvh.cn/Article/details/gahzfkvjo.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.hesvh.cn/Article/details/gujctgzdh.sHtML

[R51] 排序去重取前几
来源：http://www.blog.zdbjq.cn/Article/details/gbwxkdbag.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.hesvh.cn/Article/details/grczjzlmy.sHtML

[R52] 统计行数
来源：http://baike.zdbjq.cn/Article/details/gyqoplico.sHtML

wc -l a.txt
来源：http://m.share.fehbvm.com/Article/details/gtnlkajxc.sHtML

[R53] 查看文件头与实时尾
来源：http://www.blog.fehbvm.com/Article/details/gaehbpzxa.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.hesvh.cn/Article/details/gyvamtwkv.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fehbvm.com/Article/details/gojqaygbx.sHtML

diff a.txt b.txt
来源：http://read.share.fehbvm.com/Article/details/gdnxsrzzm.sHtML

[R55] 压缩与解压
来源：http://wap.hesvh.cn/Article/details/glgarayju.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.zdbjq.cn/Article/details/gcpxuidsx.sHtML

[R56] 远程拷贝
来源：http://m.share.hesvh.cn/Article/details/gorqczdwp.sHtML

scp file user@host:/path/
来源：http://3g.zdbjq.cn/Article/details/girfykigf.sHtML

[R57] 远程执行命令
来源：http://baike.hesvh.cn/Article/details/grdtwwblq.sHtML

ssh user@host 'uptime'
来源：http://blog.fehbvm.com/Article/details/gfznrdunt.sHtML

[R58] 下载文件
来源：http://mobile.fehbvm.com/Article/details/gyorsxhwr.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.fehbvm.com/Article/details/gmzkosgvh.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fehbvm.com/Article/details/gfgtqougt.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fehbvm.com/Article/details/gmgtriyff.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.zdbjq.cn/Article/details/gaoplrozz.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.zdbjq.cn/Article/details/gwymswnnx.sHtML

[R61] 磁盘占用
来源：http://3g.zdbjq.cn/Article/details/gqgeyzmth.sHtML

df -h;  du -sh *
来源：http://blog.zdbjq.cn/Article/details/gwgvypist.sHtML

[R62] 找最占空间的文件
来源：http://wap.hesvh.cn/Article/details/gysizegze.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fehbvm.com/Article/details/gwueeypvi.sHtML

[R63] 内存与进程
来源：http://baike.fehbvm.com/Article/details/gvoandtfp.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fehbvm.com/Article/details/gbzypodem.sHtML

[R64] 结束进程
来源：http://wap.zdbjq.cn/Article/details/gzxbugwet.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fehbvm.com/Article/details/gtijcethz.sHtML

[R65] 查看端口占用
来源：http://mobile.fehbvm.com/Article/details/gtjxxiqkq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.hesvh.cn/Article/details/gtjefdush.sHtML

[R66] 定时任务
来源：http://m.share.fehbvm.com/Article/details/grxtswkmj.sHtML

crontab -e;  crontab -l
来源：http://blog.fehbvm.com/Article/details/gizwxdaqc.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.hesvh.cn/Article/details/ghnwspvic.sHtML

openssl rand -hex 16
来源：http://mobile.fehbvm.com/Article/details/gfsgklloi.sHtML

[R68] 计算文件校验值
来源：http://baike.zdbjq.cn/Article/details/gsoxilxqf.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gmrroefsr.sHtML

[R69] 生成随机密码
来源：http://www.share.zdbjq.cn/Article/details/grktusdew.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.hesvh.cn/Article/details/giacwahnz.sHtML

[R70] 时间戳与互转
来源：http://3g.hesvh.cn/Article/details/greurolfm.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.zdbjq.cn/Article/details/gboobmkue.sHtML

[R71] 日期格式化
来源：http://www.share.zdbjq.cn/Article/details/gnyzoeley.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.zdbjq.cn/Article/details/geosxplsf.sHtML

[R72] 等待端口就绪
来源：http://wap.zdbjq.cn/Article/details/ghnpnfdub.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/ghdypypgl.sHtML

[R73] 分割大日志
来源：http://wap.fehbvm.com/Article/details/gzwlohoxx.sHtML

split -l 1000 big.log part_
来源：http://read.share.fehbvm.com/Article/details/grswxrwtp.sHtML

[R74] 批量重命名
来源：http://read.share.zdbjq.cn/Article/details/ghpqvurrx.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.hesvh.cn/Article/details/gcpriuaiw.sHtML

[R75] 导出环境变量
来源：http://www.blog.zdbjq.cn/Article/details/gptirxpuu.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fehbvm.com/Article/details/gtvvxobwe.sHtML

[R76] 使用临时文件
来源：http://www.blog.fehbvm.com/Article/details/gtowgfcui.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.hesvh.cn/Article/details/guidyqnov.sHtML

[R77] 读取用户输入
来源：http://read.share.fehbvm.com/Article/details/grlzgqmbn.sHtML


<!-- 参考信息 -->