代发 wailian999

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3xrewtnpz.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3ztbgbtns.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3xreptyju.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3fyobkbsk.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt3tontxtkq.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3mtavreio.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3reubydtf.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3ezpdioji.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3mpqqxcjd.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3nrnvhoxa.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ovtwbwnz.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3ywchifki.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ecrsnsak.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3xhcvslzj.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3dihvuwjg.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3bnndwmne.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fojimbjx.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3nnzutwmw.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3ijqeufzi.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3kbrtgect.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3bazjksfu.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3rydxexit.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3lbnvaers.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3bziyffwo.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3ixjnxmje.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3xwwizjxn.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3pmsiwpru.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3bhgimxzb.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3bktbdftm.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3qjleapup.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3dgiwrkcd.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3wurxiana.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3verfwlhz.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3rnyqcgll.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3jizgqenr.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3zfmjqnci.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3rzdfsqic.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3ygxxttmf.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3kcwrzkqu.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3niwkxxbd.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3imcfcmuu.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3ykwesshn.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3sfqupbjv.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3iqilmxbf.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3ncnokdnf.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3lrzuzund.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3dghckqgb.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3etbhqkbw.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3dmsrgrat.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3ybonpcrf.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3rbhbngtc.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3qskqwtxp.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3fsghygqc.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3bqjqozzg.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3ocnqimvk.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3zooojtmg.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3uvxpeprr.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3dietkulc.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3sckoddvr.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3qywcvokd.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3bkdhzixo.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3wdddqoup.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3krjkhiqh.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3fnhvvsyd.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3tunswros.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3nphibdlj.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3zxvyctxc.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3qezomdeg.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3drswxceg.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3nxyvkmut.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3gbseggqq.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3ksoepapd.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3wdxzqqhw.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3eyrsfatb.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3ukyfbvpy.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3dkqctmzg.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3pxrjbckd.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3cokqjmrz.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3wmqcfrlz.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3pwhxecwa.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kgmmobmx.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3bybmcwan.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3wfbjyugb.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3pmuaitxd.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3locjfrhu.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3dpbvgujb.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3jhzxbife.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3qqvwoeqj.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3pzovyclk.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3zbmltcoo.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3rnruwxpe.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3obownumz.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3gjgybqve.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3zdykbmbp.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3wrgeuhdo.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3mlxsxotp.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3xvosikys.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3tpkxrort.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3sclqmpxe.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3vvohylsj.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3nwzxkfcw.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3hokeqews.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3oednnywg.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3zaakvtup.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3ikxxeiuz.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3vqczbnfo.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3zcoumcaz.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3meiiagtr.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3ocjxigbf.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3kizdqeyc.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3qraegqli.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3qpnclufq.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3khxndler.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3gjoiuvyp.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3dxxqszdo.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3nnbqtbdi.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3ojplrepy.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3qqtrodcv.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3fxzazjpg.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3idrnscgc.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3qksdwghe.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3mnxpiryk.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3ihmldloy.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3bimjypps.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3ntafiika.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3tyorkhxq.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3dwzvfehw.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3ekhqifqg.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3ohuidrka.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3uedsfzqb.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3eqoqxsqt.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ycpsfzbw.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3igisqwoj.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3btksmyep.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3vyehjctm.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qihanpyz.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3wlckvpyc.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3oziblzac.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3szwphrnv.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3bxvabolc.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3fhgwnptq.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3bcsnwffe.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3xqmtojug.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3hovcwmgm.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3veguyljg.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3uvgmrdsw.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jqigdnke.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3yvgutvtg.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3hqpqjraz.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3nefzcygg.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3bobmatat.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mlrhicgc.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3ssowrbui.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3njyeskrr.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3mssgsyfb.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3yywhuqus.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3qvakvxjs.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3atzypxlz.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3oywfmxoc.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3wiegysla.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3jhzttpaj.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3odfwcjsi.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3dranefqn.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3kdvzotlq.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3vsioycng.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3mpuugkuh.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3bzhuhsxc.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3chxspkeq.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3vzfwbqxf.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3igajwmni.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3pkfvuxyq.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3snkedekh.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ysmfhfku.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3tsolbwwb.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3eyyuvdya.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3fsvchhxh.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3ncwqdqlb.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3ifjppbuo.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3ncypfnje.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3aaghwfco.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3zksxslfm.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3lgigwhhy.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3hbtrjqoz.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3eghpphdm.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3rdqrudiz.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3azyguogb.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3pnemtebd.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3jspcxwrt.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ftccaerr.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3mijhalyw.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3srlduehv.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3sjvtsiqm.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3yiyiufjl.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3ipcxywgz.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3enlxdunf.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3ipmjctin.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3ujdjrbqp.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3xdgrwmip.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3nuevgodb.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3ilseicwk.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3kcuetjie.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3nrpcizwd.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3acdnzbwi.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3yeqjkswx.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3ynwtkybq.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3apmunawt.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3hcdehoox.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3ezlfoppg.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3gywojgmf.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3achtdrqx.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3igmmwivp.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3iwycawjj.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3clpnubjp.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3hnpqujue.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3cgyzwnkb.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3ajoffxft.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3umwnryja.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3kqnlqjov.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3huxwnqcl.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3ralpyvdi.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xzucpdfg.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3xwzatwlq.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3uzqvajta.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3zyjkhqis.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3fknazept.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3qfyyplnk.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3evzrgwcn.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3ztorlgcx.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3xmhvclvb.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3xnurumph.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3exodvvgv.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3uvzhfyaw.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3rkzuxzmt.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3ijlryhtz.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3gbryydqr.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3iavwqpxm.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3sgmcramm.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3hughtbni.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3kncxqdfq.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3ximzzmtj.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3pscnurfs.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3hopphpfu.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3lbxkxski.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3ypjbfpuo.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3loysffck.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3lmpfibys.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3wmbippgz.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3fljntebw.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3tejppwuy.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3jaffvpmi.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3ljzqkjxt.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3auvdcswv.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vytfywne.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3kqgcpcfw.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3swyybddo.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3mqeerzli.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3orjgscwx.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3eaimmirb.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3fechtbid.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3fruwgxay.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3ozbktxug.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3nfaxfafq.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3snnwwpjj.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3nrihmfpw.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3ghajktox.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3llobdowl.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wgfabyac.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3xchwhbvj.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3cbkubqyq.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3ztfbgofc.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3cblldorc.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3nzxngxnn.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3kvgxhicc.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3osjjjdzz.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3foiyhhba.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3hmfajaqk.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3ndiyzomv.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3rbyiffse.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3mcypmact.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3jswznoiu.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3xyvdqews.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3esuhugxi.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3xkbqbaxg.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3ljfipwzz.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3njqbluzz.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3fzreiqqy.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3kulejujv.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3zgbvzymo.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3upxltkfx.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3jrdbjrni.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3dmmhxwgn.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3hnotpzpb.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3ceqcchtj.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3smyoljpz.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ftdxuehu.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3agispeqi.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3yxpcdsmt.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3rdazpigw.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3rodnelfj.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3yktzcugd.html


<!-- 参考信息 -->