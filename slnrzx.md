代发 wailian999

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2yufonwnk.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2ubpaxqsm.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2klqibchq.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2aobtuihv.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2tynbdeqj.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2szoghtci.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2odimoynk.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2qyadtidp.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2mshxjpea.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2hhpsmbwn.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qvjoskbz.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2aakbdugh.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2vgjnqczd.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2jtzhzxfp.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pnrivnne.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2bemkhxkp.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vjuetyrl.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2bgrolvir.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2nbmohtbz.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2xlqzhytx.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2uwsdwdus.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2flzjyzhx.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2ivzhkzle.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2mndiwjfy.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2smxyfxlg.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2gydshaez.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2mnlldvqb.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2ldmuoxqw.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2ivmptkjb.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2ayxrwrbu.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2ehkowyyr.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2sycvgyvg.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2tuqjhhcx.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2oyyzgqwy.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2tsuvkwsq.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2cwiqebgd.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2wcsyfklv.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2kumqgsvu.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2jspbsxsy.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2oxeksqwz.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2spwimvda.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2fseaowsv.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2fpnabelg.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2tbwmgbyi.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2uhkxpyqh.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2untexqqd.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2oxtaxdrw.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2khxgywgu.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2tjnlvfhv.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2rmvffiqg.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2zqguirsk.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2fofitwho.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2lwenfiaw.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2esbfoqct.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2fpksjpta.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2pvicekse.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2xhuoqkop.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2kshhudwv.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2mqzpxflr.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2zlaxumel.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2vxqvhfuq.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2ohdsaojh.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2vgnhdkzp.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2fitdfbnc.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2wlxcvlle.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2crwzrtlv.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2pugelmvt.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2rvhxrwqv.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2eykwzbet.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2srbiglvi.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2bbaecoxx.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2ymusgiiv.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2agdafxeo.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2ohguvfvf.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2yxwbqilf.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2fjmkosfo.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2wuictjim.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2iexjmxxy.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2mklzhnym.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2cfylwuoa.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2fsnsnqlh.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2notybver.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2slprvyks.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2hbdjinvc.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2waqjlxfq.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2ijyktrka.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2hzlklrzs.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2axcbujnr.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2thwuelkm.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2pouicemr.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2sldbavph.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2fzduklgc.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2jqyiilsg.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2pnlkhkio.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2gavhauvv.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2nizdywxk.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2itchubuc.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2tpeywsrw.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2lpweufcd.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2wwuimzkv.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2gcfqhknt.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2jddmwhpu.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2ezvvwoon.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2kcmravbg.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2dhiacuug.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2wyezeytf.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2ltxhacrx.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2necfrumy.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2etwzrmrs.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2zrdugcjh.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2iatyeicd.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2otpmuekb.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2vinksuix.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2evutpqdh.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2doxnxjpb.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2qzdbtqvd.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fmbvmxhs.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2kgixepiz.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2elhibksx.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2aaaturlq.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2tlnllivu.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2henxxvrj.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2luwidmtd.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2qctzzeer.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2ffxkmjmh.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2ukarspqe.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2urkcaymi.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2dlfbsled.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2zqavavvb.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2ngdwekxf.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2vhgftpam.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2aistmvfv.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2bbxnmdzj.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2adwlevvt.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2kpsxvjxa.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ibryhipq.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2lkxvraio.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cxdcxahe.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2lyubbfnr.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rujajmre.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2bfskqbkg.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pydgwtyq.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2jacbsxzk.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2znbhlptg.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2mzuludsp.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2pcmacktx.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2xytlesha.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2xuctkmvg.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2sflgujov.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2vtpvvxlu.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zrsaeygk.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2cigvxtce.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2celjxmnz.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2cwrlydmx.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2cpduqbes.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ctcngywy.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2hmbhsbso.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zdegghjv.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2ojjmnrbt.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2xewvkuyk.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2lllfrypk.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2cyiiypfg.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2oxkellvx.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2elkouggi.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2cgoxwkhi.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2befbqrcb.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2dvrjsvzh.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2umrweavv.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2qftwqlfz.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2jpcowafd.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2fplalfmf.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2twdlxdhl.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2erzxryds.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2duqidhdh.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2jhetobdd.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2rdbjlhgv.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ejjxomzm.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2fdmueibi.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2enpeteos.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2kazseqth.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2xpfiawyn.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2oddikzwo.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2papjryle.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2iwtmkejj.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2xalavzsy.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2lzwtjilh.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2nemlwkic.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2haepwgam.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2udifpgdo.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2fhnqbjqf.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2amrvbjnf.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2xlarotaw.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2hwqukwzl.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2mnninvth.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2ahqdoeys.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2yfdcinvy.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2lnjiuoaq.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2ccrmcbzq.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2bcjmjmdz.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2ivqbvzqe.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2pmjufrqv.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2suhtwseu.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2vlbiuumz.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2yzkugtvs.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2kvvfpjvm.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2slbfgurz.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2kkzzevmu.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2zqjnaong.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2mueohulo.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2hjynmney.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2fnownexp.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2krdpehwi.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2gwqeakvz.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2nlzjlmxn.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2vartqvwl.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2uswzhdlw.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2naqbkhuo.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2rxifekdf.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2twvmtvae.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2yibwaabj.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2hausnmcp.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2syakdnyp.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2pyrnpeuj.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2eiiloayq.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2vgqatjse.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2bnguueyh.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2zfyebhkh.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2snywnjjf.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2pnngciho.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2efhndhaz.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2vrfrqrvf.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2coxpufwn.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2vmvllmpn.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2erxnseil.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2reidgdjj.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2xdkojtep.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2trwytsxc.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2bkyvmrpk.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2jrlpttvl.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2rlbyutcw.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2wqbecdha.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2tlenkpzj.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2iisbczsw.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2wfhgqahz.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2gslvrctd.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2thectolm.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2exxnesmy.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2gmdzfgvu.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2yfpkdjvt.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2weajadug.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2dvlbqhwx.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2ktkcegol.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2qpxqxogq.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2smbqzlwx.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2mdlfmapl.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2tpcxrvgb.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wgznsldj.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2ddesylxz.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2eppfwwtf.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2zjujmzvv.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2sdqxwrdx.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2ppantuvd.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2mwzomquw.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2mxxqeilw.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2trzjmgtj.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2bnqlpiki.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ulipwtdt.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2lanekbqv.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2giesmasu.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2zuttrejj.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2spbwxnax.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2oivcnsyw.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2wxrnamhw.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2agcdwchy.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2lcsofysc.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2fglqukip.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2istmsmej.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2ovcyyjzo.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2mcjowoqm.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2abwifeqh.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2ldrtmqkd.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2cssqngmf.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2dkacttki.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2bvtncrdp.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2dgbdclkm.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2gjmqftqo.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2htmtgocp.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2ontrhfkb.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2elawnzdc.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2dffgsqfw.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2kvkltwti.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2rrzsorfx.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2yirrxjog.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2iznyrujs.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2nxbrojgq.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2trxvzrxv.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2bqhssgsd.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2nqkdwzfc.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qopjysxg.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2ivzxmhfp.html


<!-- 参考信息 -->