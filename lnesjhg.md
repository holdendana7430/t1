代发 wailian999

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.m.share.hesvh.cn/Article/details/gwjwtbqjv.sHtML

[Q28] 求和与平均
来源：http://mobile.hesvh.cn/Article/details/gthbudxlz.sHtML

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://baike.fehbvm.com/Article/details/growndkhp.sHtML

[Q29] 最大最小值
来源：http://www.share.zdbjq.cn/Article/details/gdedkhpzx.sHtML

SELECT MAX(age), MIN(age) FROM users;
来源：http://blog.fehbvm.com/Article/details/gjgcodqra.sHtML

[Q30] 分组统计
来源：http://read.share.zdbjq.cn/Article/details/gctfmxpqf.sHtML

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://mobile.zdbjq.cn/Article/details/grwinhlgr.sHtML

[Q31] 分组后过滤
来源：http://read.share.zdbjq.cn/Article/details/gnkdbqmtg.sHtML

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.blog.fehbvm.com/Article/details/gqclndfji.sHtML

[Q32] 分组拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gwwpurmcc.sHtML

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://baike.fehbvm.com/Article/details/geapgxzbe.sHtML

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://blog.hesvh.cn/Article/details/gbyqcavho.sHtML

[Q33] 多列分组
来源：http://wap.fehbvm.com/Article/details/gojqdtjxd.sHtML

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.share.fehbvm.com/Article/details/gavukrfsv.sHtML

[Q34] 每组取第一条
来源：http://read.share.zdbjq.cn/Article/details/gqhwxspyp.sHtML

SELECT * FROM (
来源：http://wap.hesvh.cn/Article/details/gzpkuzgzm.sHtML

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.share.hesvh.cn/Article/details/gjpjjpqbq.sHtML

) t WHERE rn = 1;
来源：http://www.share.fehbvm.com/Article/details/gvmjrvspn.sHtML

[Q35] 内连接
来源：http://www.blog.fehbvm.com/Article/details/gpbgohpys.sHtML

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.share.hesvh.cn/Article/details/gymbnxdtz.sHtML

[Q36] 左连接
来源：http://3g.fehbvm.com/Article/details/gdifhvhlh.sHtML

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://read.share.hesvh.cn/Article/details/godboptoi.sHtML

[Q37] 右连接
来源：http://www.m.share.hesvh.cn/Article/details/gmnpmsxrr.sHtML

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.share.hesvh.cn/Article/details/gmhuvfzar.sHtML

[Q38] 全外连接（PostgreSQL）
来源：http://mobile.fehbvm.com/Article/details/givyvbqlc.sHtML

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://mobile.zdbjq.cn/Article/details/giggrssho.sHtML

[Q39] 自连接（查上下级）
来源：http://m.share.hesvh.cn/Article/details/gkkzdcyuc.sHtML

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.m.share.fehbvm.com/Article/details/gyipdzkay.sHtML

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://3g.zdbjq.cn/Article/details/gtydmexcf.sHtML

[Q40] 交叉连接（笛卡尔积）
来源：http://baike.fehbvm.com/Article/details/giitwjiqa.sHtML

SELECT * FROM colors CROSS JOIN sizes;
来源：http://3g.fehbvm.com/Article/details/ghrmvemfg.sHtML

[Q41] 多表连接
来源：http://read.share.fehbvm.com/Article/details/gkfzrvmfl.sHtML

SELECT o.id, u.name, p.title FROM orders o
来源：http://read.share.hesvh.cn/Article/details/gwdurtlbv.sHtML

JOIN users u ON u.id = o.user_id
来源：http://baike.fehbvm.com/Article/details/gxkqedvwg.sHtML

JOIN products p ON p.id = o.product_id;
来源：http://www.share.fehbvm.com/Article/details/gwfxosruj.sHtML

[Q42] 连接条件附加过滤
来源：http://www.blog.fehbvm.com/Article/details/gkzdplxft.sHtML

SELECT u.name, o.amount FROM users u
来源：http://read.share.zdbjq.cn/Article/details/gejhvxhuj.sHtML

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://wap.fehbvm.com/Article/details/ghzlhvjvt.sHtML

[Q43] 标量子查询
来源：http://m.share.fehbvm.com/Article/details/gqhpopbbb.sHtML

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://3g.fehbvm.com/Article/details/gdutuoimn.sHtML

[Q44] IN 子查询
来源：http://mobile.hesvh.cn/Article/details/gsezkdnrv.sHtML

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.m.share.zdbjq.cn/Article/details/gqjaumnte.sHtML

[Q45] EXISTS 判断存在
来源：http://read.share.zdbjq.cn/Article/details/grblpmtly.sHtML

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.zdbjq.cn/Article/details/gqwwfrrit.sHtML

[Q46] NOT EXISTS 判断不存在
来源：http://read.share.zdbjq.cn/Article/details/gmzbvdfqt.sHtML

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://mobile.zdbjq.cn/Article/details/gufolkbqa.sHtML

[Q47] 与平均值比较
来源：http://m.share.hesvh.cn/Article/details/gaqzkzhlf.sHtML

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.share.zdbjq.cn/Article/details/gjgvrtzjq.sHtML

[Q48] CTE 公用表表达式
来源：http://blog.hesvh.cn/Article/details/gajnqhurz.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.m.share.fehbvm.com/Article/details/griicggyy.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://read.share.zdbjq.cn/Article/details/gtiolvkye.sHtML

[Q49] 更新单行
来源：http://blog.hesvh.cn/Article/details/grlmkpceo.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://3g.fehbvm.com/Article/details/gktcrzscy.sHtML

[Q50] 批量更新
来源：http://www.m.share.fehbvm.com/Article/details/gykwwqlze.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://wap.hesvh.cn/Article/details/gqpyzcidi.sHtML

[Q51] 用子查询更新
来源：http://blog.fehbvm.com/Article/details/gkbmmlthp.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.share.zdbjq.cn/Article/details/grewvfqdb.sHtML

[Q52] 删除指定行
来源：http://wap.zdbjq.cn/Article/details/gjeousrmp.sHtML

DELETE FROM users WHERE id = 10;
来源：http://www.share.hesvh.cn/Article/details/gzbweuaga.sHtML

[Q53] 按条件删除
来源：http://baike.fehbvm.com/Article/details/gutlrrdmw.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.zdbjq.cn/Article/details/gsnhtasxz.sHtML

[Q54] 清空表
来源：http://www.share.hesvh.cn/Article/details/gaxhellva.sHtML

TRUNCATE TABLE logs;
来源：http://baike.fehbvm.com/Article/details/gftqnpqyj.sHtML

[Q55] 排名（并列占位）
来源：http://read.share.zdbjq.cn/Article/details/gkjtqprqk.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.share.hesvh.cn/Article/details/gffzabsie.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.m.share.hesvh.cn/Article/details/geupciglf.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://3g.hesvh.cn/Article/details/gsbvctbtj.sHtML

[Q57] 行号
来源：http://mobile.zdbjq.cn/Article/details/gpifhqmlp.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://3g.zdbjq.cn/Article/details/gqokgatic.sHtML

[Q58] 累计求和
来源：http://mobile.hesvh.cn/Article/details/grsnlulzh.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.fehbvm.com/Article/details/gayrqqoir.sHtML

[Q59] 分组内累计
来源：http://www.share.fehbvm.com/Article/details/gdmxgfwkk.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://3g.fehbvm.com/Article/details/gximcbaoy.sHtML

[Q60] 取上一行 / 下一行
来源：http://mobile.hesvh.cn/Article/details/gjdqdrvxo.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.blog.hesvh.cn/Article/details/gaupulimz.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://wap.fehbvm.com/Article/details/godpmkjsx.sHtML

[Q61] 移动平均
来源：http://wap.hesvh.cn/Article/details/gepquoiup.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://m.share.fehbvm.com/Article/details/giqrlsecv.sHtML

[Q62] 分组占比
来源：http://mobile.zdbjq.cn/Article/details/gbcybfkoz.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://read.share.fehbvm.com/Article/details/gejtzkpxq.sHtML

[Q63] 开启事务
来源：http://read.share.fehbvm.com/Article/details/gijgergls.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://blog.hesvh.cn/Article/details/gylhifilj.sHtML

[Q64] 提交事务
来源：http://wap.fehbvm.com/Article/details/gizikmucr.sHtML

COMMIT;
来源：http://3g.fehbvm.com/Article/details/gmllftpxh.sHtML

[Q65] 回滚事务
来源：http://3g.fehbvm.com/Article/details/gaujxrcez.sHtML

ROLLBACK;
来源：http://m.share.zdbjq.cn/Article/details/gezwuqegy.sHtML

[Q66] 行锁查询
来源：http://www.share.hesvh.cn/Article/details/gbhqjhqqy.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://m.share.hesvh.cn/Article/details/grpmsrgnq.sHtML

[Q67] 设置隔离级别
来源：http://m.share.hesvh.cn/Article/details/gkspjwjcn.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://baike.fehbvm.com/Article/details/gcuuryegn.sHtML

[Q68] 保存点
来源：http://m.share.hesvh.cn/Article/details/ggpvcdzoy.sHtML

SAVEPOINT sp1;
来源：http://mobile.hesvh.cn/Article/details/gunslrccd.sHtML

ROLLBACK TO sp1;
来源：http://3g.zdbjq.cn/Article/details/glpgguogm.sHtML

[Q69] 查看执行计划
来源：http://blog.fehbvm.com/Article/details/guvqvfkpr.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://blog.zdbjq.cn/Article/details/gxlsdeenh.sHtML

[Q70] 更新统计信息
来源：http://read.share.hesvh.cn/Article/details/gylqqgfyx.sHtML

ANALYZE TABLE users;
来源：http://read.share.hesvh.cn/Article/details/ghhcjaryf.sHtML

[Q71] 查看建表语句
来源：http://www.m.share.zdbjq.cn/Article/details/gdojjxril.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.m.share.zdbjq.cn/Article/details/ghsipduoy.sHtML

[Q72] 查看索引
来源：http://blog.hesvh.cn/Article/details/gfdmtyiuk.sHtML

SHOW INDEX FROM users;
来源：http://www.share.hesvh.cn/Article/details/gbanflmmb.sHtML

[Q73] 查看表状态
来源：http://baike.fehbvm.com/Article/details/gsjdtcuro.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://mobile.hesvh.cn/Article/details/glyjvzviv.sHtML

[Q74] 强制使用索引
来源：http://mobile.hesvh.cn/Article/details/ghkbldjes.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.share.hesvh.cn/Article/details/guhcdfmsw.sHtML

[Q75] 日期格式化
来源：http://mobile.fehbvm.com/Article/details/gyvyjhnio.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://3g.hesvh.cn/Article/details/gkvsjzffm.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://m.share.hesvh.cn/Article/details/ggvetljjt.sHtML

[Q76] 按天统计
来源：http://wap.zdbjq.cn/Article/details/gsmvedihg.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://baike.fehbvm.com/Article/details/gjzaldose.sHtML

[Q77] 时间加减
来源：http://blog.hesvh.cn/Article/details/gxupexhkg.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.blog.zdbjq.cn/Article/details/ghqdyzrfs.sHtML

[Q78] 当前时间
来源：http://blog.zdbjq.cn/Article/details/gysbkumfs.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.blog.zdbjq.cn/Article/details/gpvkykxjh.sHtML

[Q79] 字符串拼接
来源：http://wap.fehbvm.com/Article/details/gbdtgqiiu.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://wap.zdbjq.cn/Article/details/gwnzmzsuo.sHtML

[Q80] 字符串截取
来源：http://blog.hesvh.cn/Article/details/geucxffcp.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.zdbjq.cn/Article/details/gfetbpjeo.sHtML

[Q81] 字符串替换
来源：http://baike.hesvh.cn/Article/details/guzerjmke.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.blog.hesvh.cn/Article/details/gzqyfhaxr.sHtML

[Q82] 字符长度与字节长度
来源：http://www.share.fehbvm.com/Article/details/ggxkwrcvw.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.m.share.fehbvm.com/Article/details/gfafgwcqm.sHtML

[Q83] 大小写转换
来源：http://www.blog.zdbjq.cn/Article/details/gamkifous.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.blog.hesvh.cn/Article/details/guzerquxm.sHtML

[Q84] 去除首尾空格
来源：http://www.m.share.zdbjq.cn/Article/details/gcupgsfji.sHtML

SELECT TRIM(name) FROM users;
来源：http://m.share.fehbvm.com/Article/details/gosezvent.sHtML

[Q85] 数值取整
来源：http://baike.hesvh.cn/Article/details/gbywdxrjg.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://3g.hesvh.cn/Article/details/gujpcpabn.sHtML

[Q86] 读取 JSON 字段
来源：http://wap.hesvh.cn/Article/details/gizgijena.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://blog.hesvh.cn/Article/details/gyewmteww.sHtML

[Q87] JSON 字段做条件
来源：http://wap.fehbvm.com/Article/details/gfnfbbuml.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.share.hesvh.cn/Article/details/gxcutklpf.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.zdbjq.cn/Article/details/gmqkgsviz.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://wap.hesvh.cn/Article/details/gkubgxuho.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://mobile.fehbvm.com/Article/details/gbmqthoyk.sHtML

[Q89] 判断表是否存在
来源：http://m.share.zdbjq.cn/Article/details/gklglpvda.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.m.share.hesvh.cn/Article/details/geaviboan.sHtML

[Q90] 生成序号列
来源：http://www.blog.zdbjq.cn/Article/details/grzjuphod.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.share.fehbvm.com/Article/details/gjfbbrlwn.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gvvxasstm.sHtML

R. Bash 专题
来源：http://3g.zdbjq.cn/Article/details/gyawrlzgh.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gwkjijdbb.sHtML

[R01] shebang 与严格模式
来源：http://mobile.zdbjq.cn/Article/details/gfblnbsaj.sHtML

#!/usr/bin/env bash
来源：http://blog.hesvh.cn/Article/details/gnquccehi.sHtML

set -euo pipefail
来源：http://m.share.hesvh.cn/Article/details/gsohppvea.sHtML

[R02] 变量赋值与使用
来源：http://wap.hesvh.cn/Article/details/gdntyifii.sHtML

name="Tom"; echo "$name"
来源：http://wap.fehbvm.com/Article/details/gogwkylnt.sHtML

[R03] 只读变量
来源：http://www.share.hesvh.cn/Article/details/gjjxhiuuv.sHtML

readonly PI=3.14
来源：http://www.m.share.hesvh.cn/Article/details/gwwejwmvn.sHtML

[R04] 位置参数
来源：http://mobile.zdbjq.cn/Article/details/gcmtvcjju.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://blog.hesvh.cn/Article/details/gxjscaofe.sHtML

[R05] 参数默认值
来源：http://baike.fehbvm.com/Article/details/gugoritxr.sHtML

name="${1:-default}"
来源：http://www.blog.hesvh.cn/Article/details/gdrrzkwwv.sHtML

[R06] 判断命令是否存在
来源：http://www.blog.hesvh.cn/Article/details/gljwfldyb.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.share.fehbvm.com/Article/details/giqufntzl.sHtML

[R07] if 判断文件
来源：http://read.share.fehbvm.com/Article/details/giuwpzqqc.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fehbvm.com/Article/details/giehwbrfz.sHtML

[R08] 数值比较
来源：http://baike.hesvh.cn/Article/details/gjzxhispr.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://mobile.hesvh.cn/Article/details/gkszugppk.sHtML

[R09] 字符串比较
来源：http://3g.zdbjq.cn/Article/details/ghbcamkgg.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.zdbjq.cn/Article/details/gmwcurbck.sHtML

[R10] 正则匹配
来源：http://read.share.fehbvm.com/Article/details/gisxlbslr.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fehbvm.com/Article/details/gxehfodoj.sHtML

[R11] case 多分支
来源：http://www.blog.hesvh.cn/Article/details/gvgyegbdu.sHtML

case "$1" in
来源：http://3g.fehbvm.com/Article/details/gdxpjmjtb.sHtML

start) echo "启动" ;;
来源：http://read.share.hesvh.cn/Article/details/gfoeuhapa.sHtML

stop)  echo "停止" ;;
来源：http://3g.zdbjq.cn/Article/details/gkbrjbdwm.sHtML

*)     echo "未知命令" ;;
来源：http://blog.zdbjq.cn/Article/details/gurbkwfrk.sHtML

esac
来源：http://m.share.zdbjq.cn/Article/details/gmoqsrwvn.sHtML

[R12] for 遍历文件
来源：http://mobile.fehbvm.com/Article/details/gedppjqgv.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.m.share.hesvh.cn/Article/details/gvmzjxyjs.sHtML

[R13] for 计数循环
来源：http://m.share.hesvh.cn/Article/details/getdkbhkp.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://baike.zdbjq.cn/Article/details/gthozdhye.sHtML

[R14] C 风格 for
来源：http://mobile.zdbjq.cn/Article/details/gffyvegnl.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.zdbjq.cn/Article/details/ghyajxdol.sHtML

[R15] while 逐行读文件
来源：http://baike.hesvh.cn/Article/details/gmimyttqa.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://wap.zdbjq.cn/Article/details/gwlbhcghd.sHtML

[R16] until 等待条件
来源：http://www.m.share.fehbvm.com/Article/details/gxulukknr.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://3g.hesvh.cn/Article/details/gwotesmbt.sHtML

[R17] 数组定义与取值
来源：http://www.blog.zdbjq.cn/Article/details/gauhzjibn.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://mobile.hesvh.cn/Article/details/gpbytkcyv.sHtML

[R18] 遍历数组
来源：http://blog.zdbjq.cn/Article/details/gnmjsswsb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.share.fehbvm.com/Article/details/gwjzxctvw.sHtML

[R19] 数组长度
来源：http://read.share.zdbjq.cn/Article/details/ghimrmisz.sHtML

echo "${#arr[@]}"
来源：http://3g.fehbvm.com/Article/details/gcumssizw.sHtML

[R20] 关联数组（字典）
来源：http://3g.zdbjq.cn/Article/details/gtzlfskdg.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.zdbjq.cn/Article/details/gbipqgyjl.sHtML

[R21] 字符串长度
来源：http://m.share.fehbvm.com/Article/details/gbxkkueae.sHtML

echo "${#s}"
来源：http://wap.hesvh.cn/Article/details/gxdjjdwbr.sHtML

[R22] 截取子串
来源：http://www.blog.hesvh.cn/Article/details/gnqqjplso.sHtML

echo "${s:0:5}"
来源：http://baike.fehbvm.com/Article/details/glvytyrhw.sHtML

[R23] 字符串替换
来源：http://wap.fehbvm.com/Article/details/gdshyeejy.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fehbvm.com/Article/details/gbnsttupg.sHtML

[R24] 大小写转换
来源：http://www.share.fehbvm.com/Article/details/gwmwrouew.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://m.share.zdbjq.cn/Article/details/giyuogedh.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.share.hesvh.cn/Article/details/gvxtxhjrp.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.m.share.zdbjq.cn/Article/details/gxoikasgp.sHtML

[R26] 命令替换
来源：http://blog.hesvh.cn/Article/details/goqqqckqq.sHtML

now=$(date +%F); echo "$now"
来源：http://3g.hesvh.cn/Article/details/gvsilkrfz.sHtML

[R27] 算术展开
来源：http://mobile.zdbjq.cn/Article/details/grgyhoshs.sHtML

echo $((1 + 2 * 3))
来源：http://blog.hesvh.cn/Article/details/gdjwdqoor.sHtML

[R28] 浮点运算
来源：http://baike.zdbjq.cn/Article/details/glmqsotnv.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fehbvm.com/Article/details/gzpfyajlo.sHtML

[R29] 定义函数
来源：http://m.share.fehbvm.com/Article/details/gpigmzdxu.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fehbvm.com/Article/details/gzxtchzbp.sHtML

[R30] 函数返回状态码
来源：http://blog.hesvh.cn/Article/details/gvqujazsq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.fehbvm.com/Article/details/gmfqztrfs.sHtML

[R31] 局部变量
来源：http://www.m.share.fehbvm.com/Article/details/gkkctodnf.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.zdbjq.cn/Article/details/gogvlpgwe.sHtML

[R32] 参数个数校验
来源：http://www.m.share.zdbjq.cn/Article/details/gqainytha.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.zdbjq.cn/Article/details/giszdabkh.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.zdbjq.cn/Article/details/gvrhdxhyx.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fehbvm.com/Article/details/gqwjjhnnt.sHtML

[R34] 退出时清理
来源：http://www.share.hesvh.cn/Article/details/gvpzksnro.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fehbvm.com/Article/details/gbiqwfhko.sHtML

[R35] 后台执行并等待
来源：http://3g.fehbvm.com/Article/details/gzyrexwfw.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.blog.zdbjq.cn/Article/details/gahwofmci.sHtML

[R36] 并发执行多个任务
来源：http://blog.hesvh.cn/Article/details/gpdwmfisg.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fehbvm.com/Article/details/gofbhdnmb.sHtML

[R37] 把输出赋给变量
来源：http://blog.hesvh.cn/Article/details/gwngrfkjw.sHtML

files=$(ls -1)
来源：http://read.share.zdbjq.cn/Article/details/goostrypw.sHtML

[R38] 管道串联
来源：http://mobile.hesvh.cn/Article/details/ghxizhttg.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.zdbjq.cn/Article/details/geqhvmgkr.sHtML

[R39] 重定向标准输出与错误
来源：http://mobile.zdbjq.cn/Article/details/gmtdqiuzo.sHtML

cmd > out.log 2>&1
来源：http://m.share.zdbjq.cn/Article/details/gtazqgwpy.sHtML

[R40] 追加写日志
来源：http://www.m.share.fehbvm.com/Article/details/goqqpvsnc.sHtML

echo "log" >> out.log
来源：http://www.blog.fehbvm.com/Article/details/gkqmwqdoy.sHtML

[R41] 丢弃输出
来源：http://read.share.fehbvm.com/Article/details/gykmrybfp.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.zdbjq.cn/Article/details/gcbintytx.sHtML

[R42] 输入重定向
来源：http://3g.hesvh.cn/Article/details/ghgeoklxj.sHtML

wc -l < a.txt
来源：http://3g.zdbjq.cn/Article/details/ghciuplrg.sHtML

[R43] 按名字查找文件
来源：http://www.blog.zdbjq.cn/Article/details/gsvpwmbth.sHtML

find . -name "*.log" -type f
来源：http://baike.hesvh.cn/Article/details/ghssletpt.sHtML

[R44] 按修改时间查找
来源：http://mobile.fehbvm.com/Article/details/gvxdsgabc.sHtML

find . -mtime -7 -type f
来源：http://mobile.fehbvm.com/Article/details/ghdtwisue.sHtML

[R45] 批量删除
来源：http://baike.fehbvm.com/Article/details/gspznhzyq.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.hesvh.cn/Article/details/gotrtwmqp.sHtML

[R46] 递归替换文件内容
来源：http://www.share.hesvh.cn/Article/details/gyaimdszl.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.zdbjq.cn/Article/details/gimldqldp.sHtML

[R47] sed 单行替换
来源：http://m.share.zdbjq.cn/Article/details/gytvcyeis.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.fehbvm.com/Article/details/gpnbcntev.sHtML

[R48] awk 取指定列
来源：http://wap.fehbvm.com/Article/details/gwofdfiru.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fehbvm.com/Article/details/gqxzmurlw.sHtML

[R49] awk 带条件
来源：http://blog.zdbjq.cn/Article/details/gjlovtrea.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.hesvh.cn/Article/details/gigjblwsd.sHtML

[R50] awk 求和
来源：http://www.m.share.hesvh.cn/Article/details/gvqgbtczc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.zdbjq.cn/Article/details/gvmcuhgve.sHtML

[R51] 排序去重取前几
来源：http://read.share.zdbjq.cn/Article/details/gwthuvbkk.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fehbvm.com/Article/details/gpfucdaoj.sHtML

[R52] 统计行数
来源：http://www.m.share.zdbjq.cn/Article/details/gvprhoafk.sHtML

wc -l a.txt
来源：http://3g.fehbvm.com/Article/details/gpnyhidut.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.zdbjq.cn/Article/details/gjpktsywq.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fehbvm.com/Article/details/ghsmcumph.sHtML

[R54] 比较两个文件
来源：http://wap.hesvh.cn/Article/details/gcnoogvkd.sHtML

diff a.txt b.txt
来源：http://wap.fehbvm.com/Article/details/ganrpvwjo.sHtML

[R55] 压缩与解压
来源：http://www.m.share.zdbjq.cn/Article/details/gcduznymf.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.hesvh.cn/Article/details/gcqvmdlva.sHtML

[R56] 远程拷贝
来源：http://3g.hesvh.cn/Article/details/gtcrizfzr.sHtML

scp file user@host:/path/
来源：http://www.share.zdbjq.cn/Article/details/gfoywxeyp.sHtML

[R57] 远程执行命令
来源：http://blog.fehbvm.com/Article/details/gpsjhzpew.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.zdbjq.cn/Article/details/gxgupukqt.sHtML

[R58] 下载文件
来源：http://wap.hesvh.cn/Article/details/gmeogouxp.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fehbvm.com/Article/details/gtsubtbig.sHtML

[R59] 发 POST JSON
来源：http://mobile.zdbjq.cn/Article/details/gjsnzcfem.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.hesvh.cn/Article/details/gqxvttimo.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.zdbjq.cn/Article/details/gjdcvtysx.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fehbvm.com/Article/details/gifylujke.sHtML

[R61] 磁盘占用
来源：http://read.share.fehbvm.com/Article/details/gwknnhuaq.sHtML

df -h;  du -sh *
来源：http://mobile.fehbvm.com/Article/details/glwknprbo.sHtML

[R62] 找最占空间的文件
来源：http://read.share.hesvh.cn/Article/details/gfsfltlhz.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.zdbjq.cn/Article/details/gtevusmbl.sHtML

[R63] 内存与进程
来源：http://www.share.hesvh.cn/Article/details/gszbdwrfj.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.zdbjq.cn/Article/details/gflfbspki.sHtML

[R64] 结束进程
来源：http://baike.hesvh.cn/Article/details/gijjfgwol.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.zdbjq.cn/Article/details/gvyaizyzr.sHtML

[R65] 查看端口占用
来源：http://baike.fehbvm.com/Article/details/gjakehmuj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.hesvh.cn/Article/details/gletdreua.sHtML

[R66] 定时任务
来源：http://www.blog.hesvh.cn/Article/details/grtrsbonw.sHtML

crontab -e;  crontab -l
来源：http://wap.hesvh.cn/Article/details/gbdaktjbi.sHtML

[R67] 生成随机十六进制串
来源：http://baike.hesvh.cn/Article/details/gicivxzmh.sHtML

openssl rand -hex 16
来源：http://www.share.fehbvm.com/Article/details/gruzbtfnk.sHtML

[R68] 计算文件校验值
来源：http://blog.fehbvm.com/Article/details/gyaeqcwau.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gtvgxfhuf.sHtML

[R69] 生成随机密码
来源：http://m.share.zdbjq.cn/Article/details/gojfrocrz.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fehbvm.com/Article/details/gbpwcotxr.sHtML

[R70] 时间戳与互转
来源：http://www.blog.zdbjq.cn/Article/details/gdldoqhud.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.hesvh.cn/Article/details/gntawpkkf.sHtML

[R71] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/gtqanycty.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fehbvm.com/Article/details/gtvcvopin.sHtML

[R72] 等待端口就绪
来源：http://www.share.hesvh.cn/Article/details/gvzacqjxz.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.hesvh.cn/Article/details/gbfwusavu.sHtML

[R73] 分割大日志
来源：http://wap.fehbvm.com/Article/details/gzyjdwsmt.sHtML

split -l 1000 big.log part_
来源：http://m.share.fehbvm.com/Article/details/gmpyolqzx.sHtML

[R74] 批量重命名
来源：http://m.share.hesvh.cn/Article/details/ghimhcaoz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.zdbjq.cn/Article/details/gohilovxm.sHtML

[R75] 导出环境变量
来源：http://www.m.share.hesvh.cn/Article/details/gfowxvedn.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.hesvh.cn/Article/details/gtucxrnzr.sHtML

[R76] 使用临时文件
来源：http://m.share.fehbvm.com/Article/details/gqrugjybf.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fehbvm.com/Article/details/gjamntrbx.sHtML

[R77] 读取用户输入
来源：http://baike.fehbvm.com/Article/details/gpjscssxr.sHtML


<!-- 参考信息 -->