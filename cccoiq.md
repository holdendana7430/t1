代发 wailian999

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3cfqumrtf.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3aqfhquir.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3uphklgqv.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3gjenmqcb.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3vrkhmpfe.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3bfnzavlw.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3adslyson.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3wgvnpipr.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3typqpjbg.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3caedfwry.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3xxqcurdv.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3dpgymfma.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wjxlyuva.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3nxpvasqy.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3yrmgdgub.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3raymstct.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3nfasaktk.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3knbzcydb.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3tcqjlure.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3spsnqyds.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3jgozojdg.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3ntgwvydq.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3vvijniat.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3yxykslnk.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3jjcsqghk.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3lsjlljsx.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3afneqqfh.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3frclnely.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3fclofqha.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3plqrwtmm.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3mgeukcup.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3szksbkkz.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3xejganpn.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3txxapkhj.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3hahjlbvn.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3sonkjnoz.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3uuiubaou.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3koezixrn.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3ohjtzxrh.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3oyljyesz.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3jbvvytrv.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3syzlvnht.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3outryfcj.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ynaogcew.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3cdxetydh.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3eazcgjba.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3tgtileew.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3swqblplj.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3rgrcyjhp.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3msshqjlw.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3jnalkqgd.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3ywsamemu.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3mgwafrsp.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3enxhercz.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3rphqcvkt.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3dpdfmkuh.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3ccodkxgn.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3jheadznv.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3yyxyfojn.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3vnrmwfbw.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3qwlzlygh.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3ddvzvlga.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3ywhuwaex.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3ptrdyyuy.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3hsovftde.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3nigopjbx.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3ucnxslqi.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3yravrwqv.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3juqtpyxa.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3cothwtlr.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3oacuycox.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3gomxmjef.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3lntsdlbj.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3lerlzstv.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3rhavlwqc.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3madktout.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lyjuzhsh.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3kbmokdcv.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3hzvquqbc.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3kdfiocxj.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3pvgmniuz.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3egmtnlot.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3hgepopsn.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3uyclocfr.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3vnghyhyf.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3yiezyltd.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3wlwygxzu.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3rtkzomiy.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3tmnfwrvr.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3rkxyeedo.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3odhqlboo.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3xlkcmsca.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3dcjwmmvx.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3hxslczjr.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3xkgpbpch.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3tdkvklad.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3iutpofxu.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3wzdezams.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3icihhtqx.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3xvmulgtd.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3nbuiowuu.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3ybfmztjm.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3silrnqjy.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3hmhlzszl.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3kajayydr.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3spjzfkui.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3sxwcpeub.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3sxxfatdk.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3sadozcao.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3kcznmcep.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3ufgicqam.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3zutdjnsq.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3hlnpmssu.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3xguppdjv.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3mcwsyhwp.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3lqlozobx.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3mglazqrp.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3xiducvwc.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3lprvedse.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3qnfonnnx.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3bwzrbcgs.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3quflazhw.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3ylfcansh.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3tclegwrh.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3wraqqtss.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wevcpoqz.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3gipgfozt.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3grfjrvsv.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3nfjjtxrb.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ewudooqb.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3patdenhy.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hlcpazxe.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3jyzikvxp.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pwunksth.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3vkogqxeo.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3faxreqhs.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3mgwzeoss.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3cptcuvuu.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3tnddbmby.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3fwsfphwb.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3xdgyxaij.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3xqlqamab.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rdwrayjo.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3cxpkrvsc.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3xisvroai.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3inuwlmwr.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3hxobwixq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zchwxlsi.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3btprlcgu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dtvmgtzm.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3skjibvns.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3ttvtgiqr.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3qdjpqzan.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3kabbdrzx.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3hqrxgqbu.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3vyarikct.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3nuqajydm.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3xfxwnlsd.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3axeulepb.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3ifhxqjfp.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3pmbgjfbq.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3jjhciwyy.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3jclmnnqz.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3nrqmgdsg.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3rwnegurd.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3buzgbnyn.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3tusrkech.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3twikiedk.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3fgboglvl.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3yyekdruh.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3pgcrkbat.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3jsccqutv.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3ybpzlteq.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3qxfscmil.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3hcpkbcst.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3lklsgdwc.html

esac
来源：http://www.52xcode.cn/Article/details/gt3yblqjnrk.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3babfzrgs.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3qstbmsep.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3qxvwkbdg.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3wqlcqyal.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3csevdvhd.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3fuzuxcls.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3vbmyuldh.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lfxrafks.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3lnkyhnvp.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3pkuyfuft.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3dtesyirx.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3rthwgcwr.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3eqivkxhp.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3kufwqurb.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3hquaeijl.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3rhzbxzmn.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3hgqbnkpt.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3uyhervdg.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3kepdsrlg.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3mituasno.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3oscbsnvt.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3vgecndjw.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3subhmhlm.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3kaxvdcib.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3jyvputag.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3vegvcpus.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3zhxdazra.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3arkvtviq.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3dwakujat.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3qvnkqzdp.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3jphalnuy.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3botfxhfd.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3cjaxnhsb.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3wstfodzl.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3ihwkqamx.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3wtamufwh.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3ubskbxlv.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3eccqtsio.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3irlptugl.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3viaeywjg.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3cspaywty.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3pcjckkad.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3auugwlgz.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3glivxuhj.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3qbqrlpmv.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3khxlvqbs.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3ubseszmj.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3ximpchrm.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3qshmnvfp.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3wufufgdw.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3tdganszv.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3nvddnehw.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3vmcmrqwo.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3xkoqlwfo.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3cdynlmtt.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3flfhlrnj.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3swjyzzmp.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3rwpzqafo.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3kbxabode.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3pdleqiml.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3tulrsveq.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3speonimk.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3bjmrqlqy.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3lwivecib.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3nkkjyzqm.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3zixbrrfk.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3nbjrgqod.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3soymhnzu.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3owhnymkn.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3hzcuuzzn.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3mabqwwlf.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ienfkwqo.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3bgcmzwqg.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3abnsqsyg.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3bnftrshy.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3bpcxpzpu.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3bsruggkd.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3nteuwfly.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3awkaefnu.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3ldtaehvr.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3gaeewpxu.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3ccqaaigd.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3hahymzhg.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3xizoccdq.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3gkyfktzx.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3sxutltib.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3laqvetsa.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3lvzudbkr.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3vgxsalad.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3mfcafqrt.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3acgzgtwa.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3yjfpqwkm.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3xgtiquby.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3kvkhjgxp.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3hprvtxow.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3mjiwntmk.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3emiqadbd.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3jeavbpyx.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3mcokffwg.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3jbbredxj.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3asothcbu.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3ogkggldz.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3cakbvakg.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3vsoxzzfh.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3woklbgwr.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3arpfazrv.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3sacckkwr.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3ptfaftxy.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3ehllhzkw.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3uvubftcg.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3twzdmdkz.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3muauevbf.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3yydedpvb.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3xmxunasc.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3vxusokko.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3hsbljpsh.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3kflncqlf.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3poobvxjb.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3xkufeawq.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3mlxvdrmo.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3qidzkcir.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3ggnjiuqc.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3fdgtmczh.html


<!-- 参考信息 -->