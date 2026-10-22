代发 wailian999

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2zlblpten.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2qgykzaam.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ngjhuxsp.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2aljfkyrw.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2zjmxxqdn.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2zygolfmi.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dmzwbdfg.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2wzmwvyul.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ngjkaoqx.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2gdlfrvhd.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2rnmnlwxn.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2xkshogpy.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dejpskwx.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2ltzkbqeu.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2qxpimqdg.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2dnjyyfcd.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2dghibpye.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fimwykyv.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2sfizvrgm.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2vslujbql.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2ubzaevaw.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2edmxytde.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2nghgqjcp.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2whhepraj.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2bcaxfoms.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2ptsfmzzr.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2yegefsom.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2ibnaaqrn.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2odlgvckk.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2yghshqqr.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2izgoqxqn.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2zzlpcrhx.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2tqiyzmow.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2futepulc.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2zjdwqair.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2eetcntkx.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2jncwqbbh.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2zccjljpg.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2kyxvcnla.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2epmglbiy.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2azvxymoe.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2euxwluzp.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2pwpprmat.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2vxybbepj.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2lpukcbsi.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2rbzwdqyz.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2vbghxgcq.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2zriagpcg.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2oxdzzlsb.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2svaknuiu.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2iidsrdvz.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2exrjnked.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2wvuzvfgc.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2cjyrowaz.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2tforkdja.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2zmgggkcj.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2aizzxzxa.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2kjrrpphu.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2zqtnvlzf.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2bmhcuivk.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2cgbfgyiy.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2vqhgtrwu.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2zinnrany.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2ydiulaeo.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2baaqqnfm.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2xzipbtpg.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2dffhdali.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2tuzkfcgt.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2jzgixlin.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2qazyburf.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2qqpjttwf.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2nkgygoae.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2utujngns.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2fboujelr.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2aucudxqm.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2crxzgllf.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hebispvp.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2xerkukuh.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2drzreebz.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2tpqtdscc.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2mhfbftrn.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2qjnjfxgs.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2jgeffzvc.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2mqnhsgyp.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2xxszzece.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2qzkbznqb.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2whuqeked.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2xviluqzb.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2xmpvneea.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2hceanocx.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2ofmxnnxq.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2rpffybnw.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2jqsrklbc.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2xvatgmbi.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2vtpssxgm.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2bfduqjap.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2kznrygbc.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2vtabhjsy.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2sqemcrik.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2gqktnvqv.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2jrehtumn.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2mdnfauun.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2maenllsb.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2hcawiyuw.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2jcjnrgge.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2pilxvlyn.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2zgrkipfl.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2hztqhuhh.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2auausiya.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2bhqngysf.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2ekcbnodx.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2gclycdhz.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2dyyudnhi.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ovedgoml.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ieoazidl.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2isqzfreg.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2obmsnztj.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2glripaat.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2jlydzmml.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2jehedgae.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2zdqugynv.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2alerfvuu.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2tdhknyew.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2mufudvzp.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2bckdrxho.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2roreebni.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2xxdmobqe.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qthzckae.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2luwmgkiz.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zkkthzpy.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2wwtrumyz.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2flnfmjes.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2qllqjgve.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cftprhtn.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2vaxvviio.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2pruqfhqn.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2vqpftjqw.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2vrbvetmv.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2kfrpttpb.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2fzfzccaj.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2fuzlssyh.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2bwnqlwvd.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2czfkajwm.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2wrmuazgc.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2yfcasqkf.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2jzalspyq.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2wzzljtao.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ldfrylsk.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2lfxydjwf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oqqaggjl.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2ojvvlrva.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2vlskkklt.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2syraqozw.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2kwncylcu.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2bllxrmmh.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2yvdqpfxv.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2ghkiultd.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2ghsoapuf.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2pzpxbrom.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2uuwigyxw.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2khurkqvz.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2khzzbbbi.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2nsbgoxgs.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2tdsxxzju.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2jevqrdzm.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2sfbpdepm.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2ateblpqj.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2ibnzueax.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2sdlmtzux.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2dgycsiww.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2djybvyqh.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2lojpaovp.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2lastweom.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2depuqiqi.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2jdgwhvxk.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2odoeevlf.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2vzxjvxgl.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2kgvjdljs.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2tyiekvir.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2eikdimip.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2olkhcsbl.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2idoillva.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2cxiiaale.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2hswbdsih.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mlkeiwlo.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2ejlbqhsk.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2pjwlnecr.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2laxeavbi.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2ctiecwlx.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2kytzrsuh.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2grdjvpxi.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2zdzmnyok.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2ngojsiet.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2ewdpkuar.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2uyjyuvrp.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2fwyudfnx.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2runbzusj.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2plreqbie.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2yrlyinbs.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2qiqtomxq.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2azhffaor.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2szayywvk.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2fierbljq.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2kheswtms.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2vtguwpqy.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2gzxdeqss.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2vgbqezbb.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2zmwuzevk.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2abebnctu.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2apgnntzc.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2wfklwbmu.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2vswryiwy.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2nxrhftxe.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2bikaopyf.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2raulcdec.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2ddohrokf.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2flhgbiur.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2vfhuzgiu.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2sngouepe.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2sfuqewfx.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2uwhoodvw.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2kxzikthv.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2ruszppjj.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2yoprldaj.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2hzbecuru.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2udcywdtl.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2suueyxwk.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2mmbmasqs.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2dmsissxu.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2pqjadigq.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2vohcxqvg.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2ozvzcbam.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2dmzmbzqt.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2hgqsuhie.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2xxsahhjn.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2oextjqub.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2zcfgpwoe.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2jnuaugyt.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2bsnppzef.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2phyzkwoz.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2smtdltve.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2oczqlyun.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2cfjpwwow.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2qqechpoy.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2paoezexa.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2xxfajpoo.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2cgejsvne.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2oefkiqjq.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2tzdpoeqn.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2anynxvim.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2beiqspuk.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2hquasgbe.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2doqjjayj.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2tbddwvnx.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2tfnciybo.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2tcyuukuo.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2crhsuwty.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2gniljsbo.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2smvuzrnl.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2ggilqrpp.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2xziltleb.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2mziqjfld.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2huieomuj.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2vgubdkbc.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2bsbaqhvr.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2vahmablk.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2cccictqw.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2yrxewkmx.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2txdqjfnq.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2rkgyasjq.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2fpbvmhzk.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2xfwjwkpy.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2srceyfda.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2vmbudmmn.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2thlpobxf.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2lnaqxfzt.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2mcmcjyfh.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2qonhbcqi.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2sqkxohob.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2nlkzafmc.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2iuqjjagh.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2asbnwwac.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2lglkuxjx.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2jbbobgnk.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2lodlseit.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2ojkkqofn.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2ulpzqxdw.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2olwqmttt.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2peotemnb.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2rztitcwf.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xnubvxdp.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2tphdyihg.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2atfterez.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2tccgpcus.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2gtglbawq.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2nexllpfz.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2sikjxlax.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2zmavpdoy.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2sgwjbedp.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2tenizkmu.html


<!-- 参考信息 -->