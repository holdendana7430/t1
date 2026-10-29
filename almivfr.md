代发 wailian999

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://read.share.hesvh.cn/Article/details/gkrheufay.sHtML

[Q32] 分组拼接字符串
来源：http://read.share.zdbjq.cn/Article/details/gadoxnuab.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://blog.zdbjq.cn/Article/details/gibqkqlva.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.m.share.hesvh.cn/Article/details/gnvcqgcgk.sHtML

[Q33] 多列分组
来源：http://mobile.fehbvm.com/Article/details/gxvvwxgtj.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.blog.fehbvm.com/Article/details/gzcyjgyvl.sHtML

[Q34] 每组取第一条
来源：http://www.blog.zdbjq.cn/Article/details/geansuedo.sHtML

SELECT * FROM (
来源：http://www.share.hesvh.cn/Article/details/gbhjlgnxx.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.m.share.hesvh.cn/Article/details/gvocrasxh.sHtML

) t WHERE rn = 1;
来源：http://wap.fehbvm.com/Article/details/gknfrynel.sHtML

[Q35] 内连接
来源：http://m.share.hesvh.cn/Article/details/ggwydhkvp.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://m.share.hesvh.cn/Article/details/gcpgqnvnn.sHtML

[Q36] 左连接
来源：http://www.blog.zdbjq.cn/Article/details/gvmwzkmcr.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://3g.fehbvm.com/Article/details/gqqyxjosw.sHtML

[Q37] 右连接
来源：http://baike.zdbjq.cn/Article/details/gqhkqtjtq.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://m.share.zdbjq.cn/Article/details/gefwzareu.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://www.share.hesvh.cn/Article/details/gedgwgfuo.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://baike.hesvh.cn/Article/details/gkmgefbas.sHtML

[Q39] 自连接（查上下级）
来源：http://blog.zdbjq.cn/Article/details/gejufgqmc.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://baike.zdbjq.cn/Article/details/gungyoinh.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://baike.hesvh.cn/Article/details/gqeusrrdr.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://www.blog.hesvh.cn/Article/details/gwikfmyhj.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://wap.fehbvm.com/Article/details/gjogtntbk.sHtML

[Q41] 多表连接
来源：http://read.share.hesvh.cn/Article/details/gdjsggjnv.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.m.share.zdbjq.cn/Article/details/gpfitelja.sHtML

JOIN users u ON u.id = o.user_id
来源：http://m.share.hesvh.cn/Article/details/gvgnvscre.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://wap.zdbjq.cn/Article/details/gvpvotwbx.sHtML

[Q42] 连接条件附加过滤
来源：http://wap.zdbjq.cn/Article/details/gzqtpncdt.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.fehbvm.com/Article/details/gbeykxwaw.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://3g.zdbjq.cn/Article/details/gqadvnbxe.sHtML

[Q43] 标量子查询
来源：http://baike.zdbjq.cn/Article/details/gvyptxyaw.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.share.zdbjq.cn/Article/details/gusddzmdq.sHtML

[Q44] IN 子查询
来源：http://www.blog.hesvh.cn/Article/details/gcsweqdml.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://mobile.fehbvm.com/Article/details/glakzrjww.sHtML

[Q45] EXISTS 判断存在
来源：http://blog.fehbvm.com/Article/details/gjbcwshia.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://wap.zdbjq.cn/Article/details/ggrhkprel.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://www.share.zdbjq.cn/Article/details/glvuqgknx.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://read.share.hesvh.cn/Article/details/gvoxfzqkd.sHtML

[Q47] 与平均值比较
来源：http://wap.zdbjq.cn/Article/details/gzzefozxk.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://baike.hesvh.cn/Article/details/gkotxsrwu.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.fehbvm.com/Article/details/gxtrmwbir.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://3g.zdbjq.cn/Article/details/giyijlcxh.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://3g.hesvh.cn/Article/details/grwdluecv.sHtML

[Q49] 更新单行
来源：http://www.share.zdbjq.cn/Article/details/gshfyuitu.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.fehbvm.com/Article/details/ghrkktcfc.sHtML

[Q50] 批量更新
来源：http://wap.zdbjq.cn/Article/details/gjdftbtpz.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://m.share.fehbvm.com/Article/details/gizzmvcnn.sHtML

[Q51] 用子查询更新
来源：http://wap.fehbvm.com/Article/details/ggapspssc.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.hesvh.cn/Article/details/gjgqzkyfj.sHtML

[Q52] 删除指定行
来源：http://blog.fehbvm.com/Article/details/gqqcubepo.sHtML

DELETE FROM users WHERE id = 10;
来源：http://read.share.fehbvm.com/Article/details/grbuhisav.sHtML

[Q53] 按条件删除
来源：http://baike.hesvh.cn/Article/details/gozsmcipe.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.share.zdbjq.cn/Article/details/gvfupzbws.sHtML

[Q54] 清空表
来源：http://blog.zdbjq.cn/Article/details/gttytgdks.sHtML

TRUNCATE TABLE logs;
来源：http://mobile.fehbvm.com/Article/details/gfgslfwlm.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.fehbvm.com/Article/details/gksgitbyu.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://baike.hesvh.cn/Article/details/gmcazrwwe.sHtML

[Q56] 密集排名（并列不占位）
来源：http://m.share.zdbjq.cn/Article/details/gxwpwgcpq.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.hesvh.cn/Article/details/glcbkvwql.sHtML

[Q57] 行号
来源：http://m.share.hesvh.cn/Article/details/gwbvtklek.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.m.share.zdbjq.cn/Article/details/gucosvmlp.sHtML

[Q58] 累计求和
来源：http://3g.hesvh.cn/Article/details/gbttnbhpz.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://blog.hesvh.cn/Article/details/ggeaqstzm.sHtML

[Q59] 分组内累计
来源：http://m.share.zdbjq.cn/Article/details/grjxmqtrj.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.zdbjq.cn/Article/details/gwkgqliwt.sHtML

[Q60] 取上一行 / 下一行
来源：http://baike.fehbvm.com/Article/details/ggrhlswbn.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://wap.hesvh.cn/Article/details/gyxubnpos.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://blog.zdbjq.cn/Article/details/gdabkowad.sHtML

[Q61] 移动平均
来源：http://blog.zdbjq.cn/Article/details/gcsscwenf.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.share.zdbjq.cn/Article/details/gphsshmhf.sHtML

[Q62] 分组占比
来源：http://www.blog.hesvh.cn/Article/details/gavmjoveh.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.fehbvm.com/Article/details/gsgowdghe.sHtML

[Q63] 开启事务
来源：http://www.share.zdbjq.cn/Article/details/gajjhliex.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://baike.zdbjq.cn/Article/details/gctncdqct.sHtML

[Q64] 提交事务
来源：http://3g.fehbvm.com/Article/details/gjljvubnd.sHtML

COMMIT;
来源：http://www.blog.zdbjq.cn/Article/details/gcyfkivvk.sHtML

[Q65] 回滚事务
来源：http://blog.zdbjq.cn/Article/details/glfwdxpku.sHtML

ROLLBACK;
来源：http://mobile.fehbvm.com/Article/details/gjjtaqmqy.sHtML

[Q66] 行锁查询
来源：http://www.share.fehbvm.com/Article/details/gzlbxwmim.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://3g.zdbjq.cn/Article/details/geouwjbai.sHtML

[Q67] 设置隔离级别
来源：http://wap.fehbvm.com/Article/details/gmnfpelzn.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://wap.hesvh.cn/Article/details/glkizvvzl.sHtML

[Q68] 保存点
来源：http://www.m.share.fehbvm.com/Article/details/gktuwkjqb.sHtML

SAVEPOINT sp1;
来源：http://blog.fehbvm.com/Article/details/gzskbvnfv.sHtML

ROLLBACK TO sp1;
来源：http://m.share.fehbvm.com/Article/details/gmpskdydn.sHtML

[Q69] 查看执行计划
来源：http://m.share.hesvh.cn/Article/details/gvrbamdsw.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fehbvm.com/Article/details/gachsivfj.sHtML

[Q70] 更新统计信息
来源：http://blog.zdbjq.cn/Article/details/gecdhlawl.sHtML

ANALYZE TABLE users;
来源：http://read.share.zdbjq.cn/Article/details/ggfgktggx.sHtML

[Q71] 查看建表语句
来源：http://mobile.zdbjq.cn/Article/details/gphgerfix.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://3g.hesvh.cn/Article/details/gzodnbiov.sHtML

[Q72] 查看索引
来源：http://www.share.zdbjq.cn/Article/details/gvpnmvqux.sHtML

SHOW INDEX FROM users;
来源：http://www.share.zdbjq.cn/Article/details/gdnbblgrm.sHtML

[Q73] 查看表状态
来源：http://blog.fehbvm.com/Article/details/giawhpizv.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://www.m.share.zdbjq.cn/Article/details/gqchdmstu.sHtML

[Q74] 强制使用索引
来源：http://www.m.share.hesvh.cn/Article/details/gjlzosrac.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://3g.zdbjq.cn/Article/details/ggmececaf.sHtML

[Q75] 日期格式化
来源：http://blog.fehbvm.com/Article/details/gnroshkhs.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.m.share.hesvh.cn/Article/details/gvhcemrhp.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.hesvh.cn/Article/details/gouhvxysu.sHtML

[Q76] 按天统计
来源：http://m.share.hesvh.cn/Article/details/geomulmui.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://m.share.hesvh.cn/Article/details/gcweurxrj.sHtML

[Q77] 时间加减
来源：http://mobile.hesvh.cn/Article/details/gnqmikfld.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.hesvh.cn/Article/details/grzcoqnbd.sHtML

[Q78] 当前时间
来源：http://baike.hesvh.cn/Article/details/gqiicombt.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://baike.fehbvm.com/Article/details/gceiuvzfb.sHtML

[Q79] 字符串拼接
来源：http://wap.fehbvm.com/Article/details/gbglumcot.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.share.zdbjq.cn/Article/details/ggfuocjxd.sHtML

[Q80] 字符串截取
来源：http://wap.zdbjq.cn/Article/details/gjrvzvveu.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://blog.hesvh.cn/Article/details/gtgwpklnl.sHtML

[Q81] 字符串替换
来源：http://baike.fehbvm.com/Article/details/gfhirbjdv.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.zdbjq.cn/Article/details/gueyxnvlp.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fehbvm.com/Article/details/gzevkklwn.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.share.hesvh.cn/Article/details/gsapqntzi.sHtML

[Q83] 大小写转换
来源：http://m.share.hesvh.cn/Article/details/gfexhnoyk.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://3g.hesvh.cn/Article/details/gqrrbyibn.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.zdbjq.cn/Article/details/gavwgthci.sHtML

SELECT TRIM(name) FROM users;
来源：http://mobile.hesvh.cn/Article/details/gdaklnykf.sHtML

[Q85] 数值取整
来源：http://mobile.fehbvm.com/Article/details/gqtmiomva.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://blog.hesvh.cn/Article/details/gmgrbhqyz.sHtML

[Q86] 读取 JSON 字段
来源：http://www.blog.hesvh.cn/Article/details/gqpcidlun.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://read.share.hesvh.cn/Article/details/gquccrrkt.sHtML

[Q87] JSON 字段做条件
来源：http://blog.hesvh.cn/Article/details/gsavlbyke.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.blog.hesvh.cn/Article/details/gwofgiqoa.sHtML

[Q88] 行转列（条件聚合）
来源：http://mobile.hesvh.cn/Article/details/gpaxrsoaf.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://read.share.hesvh.cn/Article/details/gutxyjoip.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://blog.fehbvm.com/Article/details/gdiaofkjp.sHtML

[Q89] 判断表是否存在
来源：http://3g.hesvh.cn/Article/details/gmgojctdr.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://3g.fehbvm.com/Article/details/gzyxixjpw.sHtML

[Q90] 生成序号列
来源：http://wap.fehbvm.com/Article/details/grartyztn.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.blog.fehbvm.com/Article/details/gmksydazl.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gvtxpyhns.sHtML

R. Bash 专题
来源：http://m.share.hesvh.cn/Article/details/glnwipxwo.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gntzspmzn.sHtML

[R01] shebang 与严格模式
来源：http://3g.hesvh.cn/Article/details/golavkghq.sHtML

#!/usr/bin/env bash
来源：http://www.m.share.zdbjq.cn/Article/details/gfnvaagyg.sHtML

set -euo pipefail
来源：http://wap.hesvh.cn/Article/details/gdxvzmiko.sHtML

[R02] 变量赋值与使用
来源：http://www.blog.hesvh.cn/Article/details/gqvcidbhz.sHtML

name="Tom"; echo "$name"
来源：http://blog.hesvh.cn/Article/details/gnpfwaegm.sHtML

[R03] 只读变量
来源：http://m.share.fehbvm.com/Article/details/gmexrzgkg.sHtML

readonly PI=3.14
来源：http://www.m.share.hesvh.cn/Article/details/gzwjbdmrq.sHtML

[R04] 位置参数
来源：http://blog.hesvh.cn/Article/details/gponayhfr.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://3g.zdbjq.cn/Article/details/geykzlabu.sHtML

[R05] 参数默认值
来源：http://baike.hesvh.cn/Article/details/gnbwavzyj.sHtML

name="${1:-default}"
来源：http://www.blog.hesvh.cn/Article/details/gojvpwljw.sHtML

[R06] 判断命令是否存在
来源：http://3g.zdbjq.cn/Article/details/gylcwsmcp.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.blog.hesvh.cn/Article/details/gdsyudyty.sHtML

[R07] if 判断文件
来源：http://baike.hesvh.cn/Article/details/gvhxaovyc.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.share.fehbvm.com/Article/details/gzmqxnkmw.sHtML

[R08] 数值比较
来源：http://www.m.share.zdbjq.cn/Article/details/gmygszbra.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.zdbjq.cn/Article/details/gbhceyizw.sHtML

[R09] 字符串比较
来源：http://wap.zdbjq.cn/Article/details/goynhjixs.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://m.share.hesvh.cn/Article/details/gdgeoejgs.sHtML

[R10] 正则匹配
来源：http://read.share.zdbjq.cn/Article/details/gzmyugdad.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.hesvh.cn/Article/details/ggazbaxak.sHtML

[R11] case 多分支
来源：http://wap.zdbjq.cn/Article/details/gkwqctvfk.sHtML

case "$1" in
来源：http://www.m.share.fehbvm.com/Article/details/gncimyiey.sHtML

start) echo "启动" ;;
来源：http://wap.fehbvm.com/Article/details/gtktfzcui.sHtML

stop)  echo "停止" ;;
来源：http://3g.fehbvm.com/Article/details/guckojnbx.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.hesvh.cn/Article/details/gmvgnxqnh.sHtML

esac
来源：http://baike.hesvh.cn/Article/details/gkwpymeac.sHtML

[R12] for 遍历文件
来源：http://www.blog.zdbjq.cn/Article/details/gdaxarlvx.sHtML

for f in *.txt; do echo "$f"; done
来源：http://m.share.hesvh.cn/Article/details/gkuqncxwp.sHtML

[R13] for 计数循环
来源：http://blog.hesvh.cn/Article/details/gstuxfjjx.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.zdbjq.cn/Article/details/gvqdllikd.sHtML

[R14] C 风格 for
来源：http://blog.zdbjq.cn/Article/details/guqhrgoxy.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.share.fehbvm.com/Article/details/gdtahwlxb.sHtML

[R15] while 逐行读文件
来源：http://3g.fehbvm.com/Article/details/grfjglnku.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.zdbjq.cn/Article/details/gtnrinssk.sHtML

[R16] until 等待条件
来源：http://blog.zdbjq.cn/Article/details/goorpikvb.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.hesvh.cn/Article/details/gchoejmdo.sHtML

[R17] 数组定义与取值
来源：http://mobile.fehbvm.com/Article/details/guykqckov.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.zdbjq.cn/Article/details/gpeexyakw.sHtML

[R18] 遍历数组
来源：http://wap.zdbjq.cn/Article/details/gajphdzqt.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.zdbjq.cn/Article/details/ghjddpwxl.sHtML

[R19] 数组长度
来源：http://www.blog.hesvh.cn/Article/details/gfbdacxwf.sHtML

echo "${#arr[@]}"
来源：http://www.blog.zdbjq.cn/Article/details/ggxjrlxmb.sHtML

[R20] 关联数组（字典）
来源：http://blog.hesvh.cn/Article/details/gudlyzquq.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.zdbjq.cn/Article/details/grtsmzezx.sHtML

[R21] 字符串长度
来源：http://baike.fehbvm.com/Article/details/gixnmbcfl.sHtML

echo "${#s}"
来源：http://read.share.hesvh.cn/Article/details/gdbxxxhta.sHtML

[R22] 截取子串
来源：http://3g.fehbvm.com/Article/details/grrwmavxi.sHtML

echo "${s:0:5}"
来源：http://www.share.hesvh.cn/Article/details/gbumwjiof.sHtML

[R23] 字符串替换
来源：http://www.blog.fehbvm.com/Article/details/glihubhws.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://3g.fehbvm.com/Article/details/giwctcmav.sHtML

[R24] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/gssiqsofw.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.blog.fehbvm.com/Article/details/gifgxxtqa.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.zdbjq.cn/Article/details/gwebmqrsl.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.hesvh.cn/Article/details/gkdydindr.sHtML

[R26] 命令替换
来源：http://www.blog.fehbvm.com/Article/details/gxjyjfzwr.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.zdbjq.cn/Article/details/gybwdsbzy.sHtML

[R27] 算术展开
来源：http://m.share.hesvh.cn/Article/details/gttwvqfml.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fehbvm.com/Article/details/gcvtvkdru.sHtML

[R28] 浮点运算
来源：http://wap.zdbjq.cn/Article/details/gmgxhpqnp.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fehbvm.com/Article/details/gglcpqgyy.sHtML

[R29] 定义函数
来源：http://blog.zdbjq.cn/Article/details/gbjbabgsm.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.hesvh.cn/Article/details/gicrfrzmw.sHtML

[R30] 函数返回状态码
来源：http://read.share.zdbjq.cn/Article/details/gehskhsxm.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.zdbjq.cn/Article/details/gdqzmnnct.sHtML

[R31] 局部变量
来源：http://mobile.zdbjq.cn/Article/details/grfufybqf.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fehbvm.com/Article/details/ggwkovefn.sHtML

[R32] 参数个数校验
来源：http://www.blog.fehbvm.com/Article/details/gdewzsqpd.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://wap.hesvh.cn/Article/details/gikgqxvur.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.hesvh.cn/Article/details/guwngqmjd.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fehbvm.com/Article/details/gbmlzcmpa.sHtML

[R34] 退出时清理
来源：http://3g.hesvh.cn/Article/details/gwgkedcxg.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.share.zdbjq.cn/Article/details/gvifcrxfd.sHtML

[R35] 后台执行并等待
来源：http://www.blog.hesvh.cn/Article/details/gpqnhvlol.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://read.share.fehbvm.com/Article/details/gskanwkzf.sHtML

[R36] 并发执行多个任务
来源：http://wap.hesvh.cn/Article/details/gfpjaylcw.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.blog.zdbjq.cn/Article/details/gywmjatxm.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fehbvm.com/Article/details/gdelwoxsg.sHtML

files=$(ls -1)
来源：http://wap.zdbjq.cn/Article/details/gbhqteprk.sHtML

[R38] 管道串联
来源：http://www.blog.fehbvm.com/Article/details/gsadouvpt.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.zdbjq.cn/Article/details/gsfmcqawb.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.fehbvm.com/Article/details/gcabbflvy.sHtML

cmd > out.log 2>&1
来源：http://blog.fehbvm.com/Article/details/gtzojmkcj.sHtML

[R40] 追加写日志
来源：http://www.share.fehbvm.com/Article/details/gawasbhyd.sHtML

echo "log" >> out.log
来源：http://mobile.zdbjq.cn/Article/details/gcsrxlozu.sHtML

[R41] 丢弃输出
来源：http://blog.fehbvm.com/Article/details/gosawzfnl.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.fehbvm.com/Article/details/gfqetpedz.sHtML

[R42] 输入重定向
来源：http://m.share.fehbvm.com/Article/details/gwehvxahc.sHtML

wc -l < a.txt
来源：http://blog.fehbvm.com/Article/details/gvwwyxgjf.sHtML

[R43] 按名字查找文件
来源：http://blog.hesvh.cn/Article/details/gxhybuspm.sHtML

find . -name "*.log" -type f
来源：http://www.blog.hesvh.cn/Article/details/gfjfvkscc.sHtML

[R44] 按修改时间查找
来源：http://mobile.fehbvm.com/Article/details/grcietwlr.sHtML

find . -mtime -7 -type f
来源：http://wap.hesvh.cn/Article/details/gdslwhcit.sHtML

[R45] 批量删除
来源：http://baike.zdbjq.cn/Article/details/gcujhwvqf.sHtML

find . -name "*.tmp" -delete
来源：http://www.share.fehbvm.com/Article/details/gmhiirlpr.sHtML

[R46] 递归替换文件内容
来源：http://mobile.fehbvm.com/Article/details/gsdpayjnb.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://read.share.fehbvm.com/Article/details/gtpkgvsab.sHtML

[R47] sed 单行替换
来源：http://3g.fehbvm.com/Article/details/gqgrqfyke.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fehbvm.com/Article/details/gosuitcku.sHtML

[R48] awk 取指定列
来源：http://wap.zdbjq.cn/Article/details/gznstzqxl.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gvaarccec.sHtML

[R49] awk 带条件
来源：http://www.share.fehbvm.com/Article/details/gkjjqanjh.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fehbvm.com/Article/details/ggfkyjfve.sHtML

[R50] awk 求和
来源：http://read.share.fehbvm.com/Article/details/gpkmaigac.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gipeywudm.sHtML

[R51] 排序去重取前几
来源：http://www.share.fehbvm.com/Article/details/gmefelshv.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.zdbjq.cn/Article/details/ghsdqrdvl.sHtML

[R52] 统计行数
来源：http://3g.zdbjq.cn/Article/details/galkgcxmr.sHtML

wc -l a.txt
来源：http://www.m.share.fehbvm.com/Article/details/ghpbxqorp.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.hesvh.cn/Article/details/griixkwsb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.hesvh.cn/Article/details/gyqqmswpq.sHtML

[R54] 比较两个文件
来源：http://www.m.share.hesvh.cn/Article/details/gndcscjbp.sHtML

diff a.txt b.txt
来源：http://www.blog.fehbvm.com/Article/details/ganxavvwn.sHtML

[R55] 压缩与解压
来源：http://m.share.hesvh.cn/Article/details/giaddvtas.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fehbvm.com/Article/details/gzcgclhhr.sHtML

[R56] 远程拷贝
来源：http://www.blog.zdbjq.cn/Article/details/ghcormyls.sHtML

scp file user@host:/path/
来源：http://read.share.zdbjq.cn/Article/details/grhvxrlfg.sHtML

[R57] 远程执行命令
来源：http://wap.zdbjq.cn/Article/details/gjlwkejaw.sHtML

ssh user@host 'uptime'
来源：http://blog.fehbvm.com/Article/details/gdpgyhboy.sHtML

[R58] 下载文件
来源：http://wap.zdbjq.cn/Article/details/gmvqiamst.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fehbvm.com/Article/details/gggjszwnt.sHtML

[R59] 发 POST JSON
来源：http://www.share.fehbvm.com/Article/details/gmetvjguy.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.hesvh.cn/Article/details/gtydhjzwo.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.hesvh.cn/Article/details/gorinfqud.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.zdbjq.cn/Article/details/gxfyanjyo.sHtML

[R61] 磁盘占用
来源：http://mobile.hesvh.cn/Article/details/gohssginf.sHtML

df -h;  du -sh *
来源：http://mobile.hesvh.cn/Article/details/gfkqcfowu.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.hesvh.cn/Article/details/gtqlfhzxp.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.hesvh.cn/Article/details/gidxkjxap.sHtML

[R63] 内存与进程
来源：http://read.share.hesvh.cn/Article/details/gnbzbwlpw.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fehbvm.com/Article/details/gzrxaiyby.sHtML

[R64] 结束进程
来源：http://baike.fehbvm.com/Article/details/gfphqawom.sHtML

kill -9 $(pgrep -f app.py)
来源：http://baike.fehbvm.com/Article/details/gzjpjtmnv.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fehbvm.com/Article/details/gvxaattjt.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fehbvm.com/Article/details/gzblueuqd.sHtML

[R66] 定时任务
来源：http://3g.fehbvm.com/Article/details/gkwkygubn.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.zdbjq.cn/Article/details/gessusefg.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.zdbjq.cn/Article/details/gwqbiotpc.sHtML

openssl rand -hex 16
来源：http://www.m.share.fehbvm.com/Article/details/gmxxbqveg.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.zdbjq.cn/Article/details/grtfsilqm.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.hesvh.cn/Article/details/gasrbavnf.sHtML

[R69] 生成随机密码
来源：http://www.share.fehbvm.com/Article/details/gjqkjbtyd.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.hesvh.cn/Article/details/gapehfxcb.sHtML

[R70] 时间戳与互转
来源：http://m.share.zdbjq.cn/Article/details/ghibjthys.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fehbvm.com/Article/details/gyerxpbrt.sHtML

[R71] 日期格式化
来源：http://m.share.hesvh.cn/Article/details/gickwghgq.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.zdbjq.cn/Article/details/ghermntsh.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fehbvm.com/Article/details/gltmokfur.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/gvpgqoccu.sHtML

[R73] 分割大日志
来源：http://m.share.fehbvm.com/Article/details/gbrevknyc.sHtML

split -l 1000 big.log part_
来源：http://www.share.fehbvm.com/Article/details/gfuptxftp.sHtML

[R74] 批量重命名
来源：http://read.share.hesvh.cn/Article/details/gvqtffezd.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fehbvm.com/Article/details/gnogawlyr.sHtML

[R75] 导出环境变量
来源：http://wap.hesvh.cn/Article/details/gndcyfglf.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fehbvm.com/Article/details/grpdwgzve.sHtML

[R76] 使用临时文件
来源：http://baike.hesvh.cn/Article/details/gttqfqgan.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/gsmqmkscj.sHtML

[R77] 读取用户输入
来源：http://m.share.fehbvm.com/Article/details/gwtbdxjmr.sHtML

read -rp "请输入: " ans
来源：http://www.share.fehbvm.com/Article/details/gzhawwkzn.sHtML

[R78] 交互式菜单
来源：http://www.share.hesvh.cn/Article/details/gwhifwjsf.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.hesvh.cn/Article/details/gnlccrbdu.sHtML

[R79] 解析命令行选项
来源：http://3g.fehbvm.com/Article/details/gcfxqgccy.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fehbvm.com/Article/details/gmbjhlbxf.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.zdbjq.cn/Article/details/gknoblnjc.sHtML

time ./run.sh
来源：http://blog.fehbvm.com/Article/details/gxjfjgflf.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gklsqsfzm.sHtML


<!-- 参考信息 -->