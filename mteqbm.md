代发 wailian999

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2xuchgjaw.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2nhzhubms.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2cjagztsl.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2lacqyyyo.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2iwqqoqvw.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2yqaiodty.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2emgvzelk.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2ftftlluz.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2onmisywc.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2vkrhbzem.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2jvknzwil.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2gdwjbfxp.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2qygcusad.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2nzgbuarq.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2acpmwfhw.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2etkzmqis.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2oqpxqifs.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2fktkbxex.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rnjwfkfl.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2mxtzxgmb.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vcdxscja.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2rjegwohc.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2gczircqr.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2oxeehzfa.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2eypzaezl.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2ltksnzno.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2zyslnctu.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2yzcbokja.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2rzbzsqsb.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2vxgnbddt.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2kbcanrje.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2hqjpdbsk.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2whreluns.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2bdmkjvfe.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2whjdnnkr.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2cuhalwjp.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2lqtrzozl.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2fgjptebm.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2lakhcjks.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2mhvqstdn.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2eqozlpfu.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2pdvalsce.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2tjgoypik.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2hpofaied.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2rbafjvwq.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2cfoaycmp.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2vaxhrrib.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2jbdovyeu.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ognwbsef.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2likkqkvi.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2duhyoagq.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2puggwcbo.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2kplpjbei.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2ueuaklmn.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2shjukfxk.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2vzsvrwfh.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2buxmbjbj.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2hopzcwlm.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2phprczfn.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2wbqmrkrp.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2szxccmka.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2yfyktuvl.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2kfumgtvx.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2vzwkzdwc.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2rbglpiky.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2owjcyafx.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2ypdcqpnh.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2mbbdyivp.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2rlrxieur.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2bojwiaeo.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2wtvaksay.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2nijnixok.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2fhumewbo.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2yjwelcpu.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2myvcslxs.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2uxmyvohf.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2tcrlhkxj.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2kmumasom.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2polihxqv.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2buawbrky.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2ostalfzw.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2ddmmaixs.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2rhipcmjm.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2udwhocnw.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2eeckrljr.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2bruxleef.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2syxkudwm.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2yzgcwkyk.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bbhqktsp.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2qovfibbv.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2auyqmldf.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2mdacdkbz.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2zmoyxxjn.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2hrknnwwx.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2nufcnhnr.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2zdcurggf.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2xoxjhzsu.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2acilmtzm.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2kutprpar.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2ixcyuwsw.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2dfdexsmp.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2mzsolajr.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2wrzpkqrp.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2idxqposn.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2ytbubqiz.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2ewbxqiux.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2wmpxdgma.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2espaivmf.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2kewdzbce.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2suuhhweo.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2vxgoejzv.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2gsklsnpi.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2cnwsxvwy.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2mufrodal.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2gnghdngo.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2tjqtqbbs.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2osucjawz.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2ukccblhb.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2rcomcxqo.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2dvxhhauh.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2biasfmob.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2hwnszgaw.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2plmpgmhl.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2mgxzgigm.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2typgrvgf.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2hpbqmqjx.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2xumjgnem.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2hynrnbyl.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2kgdwlkxz.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2vcfpofuy.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2vmkostse.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2gpcijgua.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2cljixruh.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2owregpsq.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2dagkffxk.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2agkuwnxp.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2qfnnwkzs.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zerrvszo.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2tlokcdba.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wqgcgeaj.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2vxqcjkiy.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pjwtmrbx.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2ysmblkxf.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2blpzswyt.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2qazmchir.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xvuagnmf.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2bzjgazud.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2gmkwopsz.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2zemoyrww.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2mgxawyla.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2sgkajnfl.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2nqekiazh.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2fonbxfqj.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2vexmrzxr.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2chjvagkl.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2xikwaowa.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2blmvcrra.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2xsfffvnz.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2bgqgstgv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eaddiozv.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2ypifefzt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2htpchtxq.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2vtdukbfz.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2jhorjalp.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2qdcbldkb.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2xlmamygh.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2fpsfjzmk.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2uyuljpdd.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2gsoxclte.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2qjmtromn.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2jpdsbink.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2dgubfwbx.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2itdqafza.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2cbkftstg.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2cpxggvwx.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2ctqxrtxi.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2tkcosicq.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2atmntkpf.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2udgukovi.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2udjmxhta.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2glmeatxa.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2aapzwlel.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2iflpcbcy.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2kvdwxepa.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2prwvzoct.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2tfghfenw.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2jcverqhn.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2yxpvaizj.html

esac
来源：http://www.52xcode.cn/Article/details/gt2thxhpjyx.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2uxfjrjtv.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2faiyotru.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2rafeehxa.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2dsagkvcr.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2lseqtllj.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2jkkbhbet.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2xwemmxoy.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2cvqjiwiz.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2drtdvciq.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2qgasgwfs.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2iejmkxim.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2yvqzqjjd.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2ijtavkrj.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2nebphbww.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2wgeycfay.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2ifrmfvqm.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2lznouola.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2klwyrhwf.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2yjhddoji.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2iqhvwsqu.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2rqlsjhjp.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2dytmnddm.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2ehbnrapk.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2daitwifd.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2slpuifyu.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2jhlvshym.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2zgbfdhfi.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2jvlyezpy.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2sucwjnvv.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2ksspansx.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2eaobfxha.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2blwvazrf.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2ugrcjonc.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2xhhgxkgw.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2pntuwcak.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2qlvakqks.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2howhabzp.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2iidowbak.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2gpodxrko.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lpjyikil.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2jzilddny.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2kvbrsqnb.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2xqyajyxz.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2cmlrdcck.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2calntwkd.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2rxjrkrmd.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2rxjlrxro.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2rwylpjdn.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2gubstowf.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2whmqnhvc.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2gchplqph.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2ybigehra.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2canqbduf.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2cadfdkev.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2scxhzxph.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2gwgbxyas.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2twmirusr.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2rqyzxsku.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2aawzillc.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2rgoeyrzu.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2tvzbcvzx.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zeyvztdh.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2xxcryktf.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2ohknmvjx.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2raoxnbol.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2fsbsdquz.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2qsteokcd.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2rhmvuefc.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2bdumcnee.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2oblyyhnt.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2istmkmvq.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2wfyigbvb.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2dodjjuzi.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2wzalvaxb.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2qowzjiii.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2ccrhghfe.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2twodqprw.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mshzvnlc.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2qvjcsvhd.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2rtkuwity.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2yfndiuld.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zehixkjg.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2yotwafpz.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2gtjswegn.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2instypgr.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hevxuvye.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2ivlgdumi.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2zoxxxauh.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2pqmwjjgu.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2wegbwysl.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2ibcyarcs.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2sfolpnwc.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2vefaozhj.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2eftpfewj.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2dgcsehny.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2ifshgcjj.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2qgudspfp.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2kbfrymlt.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2ourbuvyi.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2vdrkeyed.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2mjcoifjk.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2wnznfaew.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2obgnssip.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2virzpznm.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2enlhwoyz.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2oquwxmct.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2xparzmbm.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2wvnyvgog.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2chnlhfaq.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2ehnepzjw.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2rnulmsip.html


<!-- 参考信息 -->