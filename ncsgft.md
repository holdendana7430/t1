代发 wailian999

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2tikecond.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2jletrnah.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kwwyijtq.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2uevqmfcv.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2sgcuhoja.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2cylmacsc.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mdupzpkg.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2zcgcfzxb.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cvdimwwg.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2sgsyfsex.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2dhwwiulk.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2ikywnpgn.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nebgfohb.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2alnsgrif.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2jujshehv.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2wrjyacur.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2jvkqadiz.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2uajhobrw.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2djpscglu.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2dpwudwaz.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2bsukksol.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2namlewwl.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2sfnvfzdk.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2yanhsgus.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2kbwjaryj.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2inoybtuv.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2qcoyazsn.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2pxeqklqw.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2ksjrpkvk.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2fxicfwhj.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2zouebafc.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2jvvjdfja.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2giihgexr.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2zsodanon.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2ajdrkbym.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2gzeucjim.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2enivlrdu.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2dstusxbg.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2qpggbyqe.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2yhmgbusc.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2fcxersba.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2orlwbdjv.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2fivmcjhi.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2uyujfhhu.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2qihiwpnj.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2knppfosa.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2dnhgfjmx.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2qanqrcmu.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2ofwthvrz.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2htylrxev.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2iwtrsecl.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2bnbroqmb.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2ovbhnxps.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2skgdzsgd.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2wmebtzcg.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2kweafxsi.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2pygzczkr.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2ctyrexce.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2glvklukn.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2gwasyjkl.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2gwwqgiyr.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2pjtrbpcf.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2uagnzhod.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2sqjjxxsr.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2qrbvovva.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2icjtypmc.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2anxokgjt.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2kzsxgmvy.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2ywzfkyqk.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2kltzjxkx.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2ncqbousb.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2igvljtht.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2oudfvdoq.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2vmzvgzgv.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2qimworgl.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2kxtdxtxg.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gfoldcmv.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2diljdeyo.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2qcfkmeiu.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2tcwhohkc.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2hyyvgrdv.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2ltclwbay.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2jliujcho.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2qbwfmmkq.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2xvuznvnj.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2xdlcsicn.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2qakhmpfn.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2sczaohkh.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2zvqdpssw.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2rqvelcss.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2pzpcinmw.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2ixrbgwlr.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2rgptgdsd.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2bkqhyyfr.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2nxxtriex.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2boquojhq.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2lgiuoipq.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2vkewfpka.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2vjhiocrd.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2rxuhpcpj.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2sgiuxzzh.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2myeaniat.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2asztsore.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2bemsqshr.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2zofwfmsj.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2tfseabee.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2vwxcwqeh.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2cyirvass.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ehcawuye.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2yxhquzqs.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2kxbobbca.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2wuvlaehv.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2fjfpzsfs.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2klxgmqfz.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2bntqkazg.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2ubnjfxjf.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2ypbwlnbb.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2vuzjkuah.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2vnvihupe.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2garflecq.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2oxovbyhf.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2odcugehg.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2tokygnug.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2rpbgquux.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2gvxzrhhb.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2vlhycbyh.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2sqqdejuq.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wwdoeevo.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2geodemrb.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gpmstgly.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2eeylmmhg.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pmseilof.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2zxxcjhko.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2egvtwkti.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2ueavxefa.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2sdfvcest.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2olvbasxv.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2quqmeauc.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2xxvnxxdo.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2byifiles.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2iudfijkc.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2knvozuir.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2emlzagfz.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ttxhgmtm.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2nddmexnl.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2ikaukrkh.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2scambqwi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2khiievlg.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2nenewiat.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cfceiobu.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2jezbbmvi.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2kgckcfwx.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2hnspjvba.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2rwybqwlt.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2lreznozx.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2lhddhtjc.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2yfwpwtlz.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2mbiettft.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2yrswniwy.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2hohfnfnt.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2frctwxab.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2tbyjxioi.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2stnssztz.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2vroliufc.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2kezwquiy.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2tbowsdce.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2pfyganix.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2mvktjaae.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2jiwrbsxt.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2sdeckhfz.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2ukcojnno.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2zxzsoipy.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2xxfszggd.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2gtjjektk.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2wtwsplyc.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2lwdzyvxw.html

esac
来源：http://www.52xcode.cn/Article/details/gt2mldfwdnw.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2hlqsgmcl.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2weruwmog.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2tyrqcyaf.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2gfvvrmjg.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2dxeygoqf.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ubxxjnfi.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ksahnwmd.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2nztobyxj.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2ghnsjwny.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2zyxzkqhz.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2jyzcljyo.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2grsmenmu.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2hlhpqayi.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2aamlgfgs.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2jzwoiage.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2vsmfodml.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2iqntfyxr.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2jvpixgtb.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2skuoyqzw.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2tgundccl.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2cnltnowl.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2npdlczdx.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2lloolram.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2wlwxyodk.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2zpzlddwm.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2dtqqtmgs.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2ffiwhmqw.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2yjklsywb.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2dizjwbbb.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2ihiuopum.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2myydnnkg.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2yhwzqgir.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2loehioch.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2scryjxeo.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2hjofkutq.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2fpyiuwqo.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2lcsvnpfa.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2cbjsplgw.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2byewzqhs.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2byopivau.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2oueehqgf.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2exqddore.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2cobtlmbd.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2unbubgbx.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2dsjfmnpm.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2eeugtzhu.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2grufbros.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2zwriuupk.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2mfhfwpfx.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2aqzrlexe.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2esyxwuia.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2ffoihkxd.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2qvymveky.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2xpaaculd.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2syvhyzsr.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2xmopcakm.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2pqpjsudv.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2ltmutbev.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2ixalrdqi.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2jtlnwsxw.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2dlxkhfjn.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2usywwbul.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2emmxnukv.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2esebmzyo.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2hgkukumg.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2nyajusfc.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2qfasjkit.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2gemlaolr.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2xgrrivlj.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2xhjsxhrf.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2rppkrsvr.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ncjbmksd.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2cattcali.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gckyzpkm.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2qtgjakxq.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2syaetthf.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2fkxjpoae.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2bubyldbi.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2zbgrycpz.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2zqbztyih.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2chmvlrjh.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fsycucjv.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2cvyfuygs.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2vjwpxyks.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2izpulsat.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2zacisura.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2kxgkthko.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2yfbmqvpj.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2lhlkrurk.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2nygjjmdj.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2hwnvwspa.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2gcyhdcru.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2mkxewdsm.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2rfmmnujr.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2uoxqmoon.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2jasvvqiu.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2kmdhneqd.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2fdkxubry.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2gdqlbtbf.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2ezsjwmgx.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2yjoxbomu.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2ofsdddvo.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2bwyohott.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2wwfghpqs.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2zsbqqtzf.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2kdugeeup.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2ziujknff.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2tvssvddp.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2qmercmhu.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2fjbfitpq.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2iykihkbb.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2cywdfyuo.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2yhinkzlo.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2gokirtro.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2lqtunfyn.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2jdoaugbs.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2ggtsjpsd.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2pudisuku.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2gbhxkzkb.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2iitqzmcq.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2dshyrfiv.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2qbsdzzol.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2svmkzovm.html


<!-- 参考信息 -->