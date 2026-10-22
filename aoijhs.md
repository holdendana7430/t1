代发 wailian999

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2tjdtsnro.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2suzicklo.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2inhlzvzs.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2abeoudbp.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2nvwudjzw.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2qmmctoaj.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2hngvhuuy.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2gafjlsiq.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2dxolxxax.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2ptfhtlzj.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ybtgwcsb.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2dylyivqc.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2cmbocfms.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2lzfzgpub.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cydrwqbs.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2hocuewkz.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qjirfqit.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2dmifnzur.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2hsruocwg.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2dwzxnsey.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ipngmznw.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2xtfraprc.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2dufhobie.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2exkfitkn.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2kypwcytx.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2pluqexlv.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2vkmsujsx.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2ziwpskik.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2hydyurhd.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2stzqakds.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2uavkzwro.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2okpktvfv.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2ylrmwlxz.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2eidzmhyx.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2jbocuzrf.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2gouxyrrr.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2dirgtwsl.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2tvmngqhh.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2bhlchiru.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2fnsufsgl.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2tpgsnmsl.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2nscwnfym.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2zyanmwke.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2uhvaomln.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ovvwfyqz.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2nkwfdxty.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2egkrqtpy.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2kkksyqwj.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2cupapxuj.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2ubasqghe.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2vzjihyaz.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2jcyrnwnu.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2llvogiau.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2lawfgkky.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2jfjrpiew.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2zaaoxqho.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2fofjtnfn.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2wzwvnbon.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2vdncjopo.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2olldawny.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2fkykzooi.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2xxmxlmch.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2urznmkjt.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2vygtrhsk.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2frmpjerl.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2ytxnhhvi.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2wbwnsewk.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2efgyikzo.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2muhhhfjn.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2pwanqsmi.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2avcekibe.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2daimrskf.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2zaxyobxs.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2vclimvhy.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ncidizej.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2yadofcwr.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2zakvajhz.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2hruyxqal.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2eqpujquc.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2havhoszy.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2ltakghnw.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2nteodvls.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2deqhnlxn.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2fxlwwgpc.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bsuxoupx.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2uzhpyrze.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ndmnyhcd.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2mlotqdxx.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2goqgojee.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2fddymgjz.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2nbxxtgij.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2qymryxjm.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2grbitgcy.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2xbpokbmi.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2bwrzupzg.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2cceipqse.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2uvozbtil.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2uorwsmyr.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2csymvacd.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2fltxiuqy.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2ogrmgfvz.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2rmivlhhb.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2vijuunyj.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2noedfkiv.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2brnupbdu.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2ppdytgnn.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2kxnqnmgk.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2qppyojgy.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2dszvqnth.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2kjzlhyzr.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2plrdyuzp.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2tkthgftp.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2ytqysabg.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2japlegwm.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2xkttztgu.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2thbivfis.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ouepnggt.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2nvswbxra.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2aivqaxxx.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2iuxchmev.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2zsogbmke.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2lhsykqlg.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2aabpllia.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2pojwdxne.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2rrbgdrqk.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2zyivfiic.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2ebeiqbrj.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2ehtlreew.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2wrixwcbv.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2aeuuiiew.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2ijivppqm.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2ehugvsrt.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2idtbwmko.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cjdptcra.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2yoljzvdc.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dkwetafg.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2szakqxqd.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jbyjgymi.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2wmkorzzv.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dpuuatpc.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2jloqqrrv.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2uigqzxok.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2bgvxyeqm.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2yfkxccut.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2mvbvazkz.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2ffwrdbax.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2bgrwxsmj.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2linoqmzv.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2gqjdgrih.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2llvackkm.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kxopojmr.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2sgjytaxy.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2ujtosxer.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2irldbmcd.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2liqmhahu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2albkjyqz.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2djbjghut.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ygquyfhy.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2whcumlod.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2ekrkofvo.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2oqyfjldw.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2jwlgaitz.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2gsrzuhsk.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2wcxhxhnu.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2cecpmevi.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2zmnprruh.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2twisopfb.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2xjjzsrlj.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2ybyswgqy.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2yinaplzh.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2oqtsqsoz.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2ognhmagf.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2mtkzaxzb.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2deorhqlp.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2rprrlkiw.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2ealeicww.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2btqlvynm.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2kdeghbks.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2vppfwyau.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2xwrumbbx.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2xrsfmwsp.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2bzytismj.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2ylpmxfit.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2eldvsynb.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2lponfgzt.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2jopfttfs.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2obzcduvj.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2gaepydth.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2enckvxwz.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2vblandwy.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2nonkgkuk.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2qwahgxlt.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mwqhzoyv.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2yapsmbwd.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2nsoayngb.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2tpsqoxpd.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2vmxgqoes.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2ryprsdcz.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2uhdowakv.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2vczcjdgt.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2uvgzpoth.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2nafiqnmp.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2enzapznw.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2fardhfok.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2clsedtsn.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2ezufgcdn.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2pmlwregt.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2ptvkxgcy.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2nuykapki.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2ybjzwupl.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2bafnvuea.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2xujhbint.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2auvjfgxj.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2xuzepmlz.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2dwjujxxd.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2atjdycyj.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2jumkcedr.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2uvfplyfy.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2lkonzhux.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2gjvtarlz.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2vhqprhsb.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ehrjpsby.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2xkhpivud.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2nnezanmt.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2smteqsrr.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2kjzrjvku.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2kljoiztj.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2dabvqbkj.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2ohrjcpbr.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2olngjztw.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2rgnggiiy.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2ddnlyubn.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2mywwivnv.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2tjzatcrq.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2ffqyevum.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2wtopxdej.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2edceimiz.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2zxydnsep.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2raslkiry.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2eynpealq.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2vqumlwim.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2djmqesya.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2yjsxyatx.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2wtsfbvlu.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2xuigdevf.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2wzsirlna.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2hfmgukam.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2llcbobgh.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2fwkbmkqs.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2nunvfepo.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2lnqpomzm.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2nufjywgf.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2svekrcww.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2ufjyfdcp.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2cieotxee.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2goxwokti.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2gbfpddvm.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2mgxdldpy.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2oipaeddf.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2oizhfmqo.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2ldbhnaxa.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2mafqndiw.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zfamshjk.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2rwwufzwe.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2hkvifznx.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2rokrxmzw.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2bsengyio.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2dzswpcbc.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2tplbdojk.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2lxtdgpta.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2duesfxzd.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2daddohcc.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2hfstgkoy.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2ibxxojqb.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2zfqfqidf.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2uezfccak.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2hpsowufz.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2xvkxemzl.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2npmxloyo.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ynycqtrr.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2lmqkwqnc.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2dgrqjnrk.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2grqhxxon.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2oppbuysh.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2rqljlinx.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2jdpbzeoy.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2gnfjmktp.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2rsrtpolk.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2ynylvdgw.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2akowbqas.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2ulyxyoze.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2lopkiznm.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2bhlfmmby.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2idnwsoyf.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2iozeemvp.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2oovsvsry.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2fvzzdpzh.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2wndzzhzd.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2tokewaew.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2hmqfkpkr.html


<!-- 参考信息 -->