代发 wailian999

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3ewzfpmpa.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3vpgbnfpy.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3qlddehmb.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt3gqjxxesy.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3qiwzpuha.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt3ogejzhng.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3ihnufaoi.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt3isvhuyfy.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3ybgmsnwb.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3tekmzupe.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jllfkzkp.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3rlwzjfnj.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3fzjwhisu.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt3cvsvsptq.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ammymcey.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3okngwhan.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xseubfev.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt3tknpfxtb.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3xxgbeqas.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3pdqzuvfy.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xfhsyxgf.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3hdprsbbp.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3xqxdmmbv.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3liicssbe.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3ddkyohtp.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3zwsgcqnf.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3emujjzfo.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3ndkpomeg.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3kjtwhlfz.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3docbpxfa.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3jfmxerjb.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3rupkiyue.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3zlzcmqmo.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3okpeohti.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3gnkpopkg.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3vadpksdk.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3fbzeusam.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3ynidptiu.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3nlaehwsf.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3ptjeyofe.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3xirqgywl.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3jlaqmalu.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3ezeyltcw.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3vuljhjzi.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3rittxqlz.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3cczecoqh.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3oldyynmm.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3anoulnob.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3qctvzwgc.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3wbfhmzrz.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3bofnlxwj.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ykxrlxfr.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3jujjqmmv.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3ylptschz.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3rgjsfxrx.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3ndkwkbqo.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3dvolxpqr.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3umrmwgcc.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3siwrexqp.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3yorzajnd.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3ohovvliu.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3dhljnlmv.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3rskiiuzn.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3dloccsnu.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3piechnfm.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3vrtlhtun.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3chtpyvpp.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3hkbsjfob.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3bthlfzbc.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3clwflios.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3mmxaropo.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3jnnsjarf.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3zikrwips.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3phisnkie.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3xrytefet.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3kvstnlwv.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3kkbkcvzq.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3eesqjtyw.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3nwlfoobe.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3wsnfplwg.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3ghmvzeqc.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3fbcusnil.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3nfyhahhg.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3qryisvub.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3muoqiezf.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3hmvihjlr.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3rxjisyrv.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3ffgnpvrn.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3wrknvprb.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3dtnkdcyc.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3zyqeqiit.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3uxxnyooa.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3downkrwx.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3agggxqmm.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3wulalxhc.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3yiweoudn.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3pbffrdui.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3mbluorvt.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3rkzfvhpe.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3zzumjaxu.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3ktzpidlk.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3sevxcpea.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3zknjoviq.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3cmqmqzvj.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3ymsseuln.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3otucwtej.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3zecrhecc.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3mwkquduy.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3kysfcovg.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3czevzhlp.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3ddhtuaej.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3kpxurnmw.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3zjmrxcun.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3obzfawpy.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3wncsjaki.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3zavwkemi.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dlzuakym.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3lsuuyenh.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3kcwxxrxb.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3pyzbqlpg.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3abxvtabh.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3oqylnhjq.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3diajpnrw.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3wsajtirw.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3qjakgdna.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3tkmoqwqx.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3apwfbdog.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3ettswuzj.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3nipiokhb.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3pbxqbbqz.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3jyjtqbrd.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3oggidtzi.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3udxudwoj.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bysoniqy.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3sttyfuup.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zcvnomrv.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3qvxcjrdc.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pihtmohn.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3psskygfa.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3sfpqptjn.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3leantkgv.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tlngyqmf.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3zaxbjnvb.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3bbauvrxw.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3migkebee.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3xuusctmn.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3rugmkirv.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3havlqzzx.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3vhwbtvbd.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3ileiwhqj.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xutcicxu.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3efddfmle.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3wrxtagbj.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3abkyqgdn.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3dzklhfmu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gatikush.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3jgoegmjw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kxkwdeev.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3jskrdaik.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3emgunzqu.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3qrcefxbc.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3isnhhzco.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3oelvwkvv.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3inkciooe.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3bvxtofoq.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3ferlrklk.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3uuvviqcw.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3bqwojnrm.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3amrlddtz.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3fjfmhhla.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3cyviwapd.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3obbmtflh.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3hlfauptm.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3zrvplgjl.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3atluyzdh.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3urhmuhfo.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3bberymhg.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3hqdsdkdh.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3gulnoqql.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3xsspuyle.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3blrbankm.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3obemwkqe.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3dmfcwgui.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3ojwqbclf.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3mvxhncdu.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3fvguksez.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3knwfyecq.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3zquswqdy.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3hpfuxwjv.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3jlhubprg.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3lnadudet.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3pzepkzel.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3cbwzlnuy.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3ukqilwfp.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3cbrmnxao.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3wqnbaszp.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3hthmhrbo.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3ajahvxhi.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3pxsocioj.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3tvxmhevw.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3iazqfpeo.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3xootyxwr.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3hzjabebk.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3uuvxmvkb.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3xfiltcyo.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3usoeyzme.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3dcepbekx.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3tdwcikqn.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3ovxbiztb.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3rbqtiyko.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3ubfsivzp.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3bmbfrsjn.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3kqfbajkq.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3jbmciyyy.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3xaoibpxe.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3ofgnsykt.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3vdycrydj.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3uokoqwlk.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3tuegenhi.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3eeuuocus.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3ebmfzefk.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3rzycaqoj.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3kxoqrggk.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3jayqyzkm.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3gomofozm.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3kbnatqsa.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3nwucmmza.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3ibrevjmc.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3hqfshfko.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3suojplfa.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3olvolysj.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3zfaxnyxl.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3xvbvtwfh.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3uqwvqgyg.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3slbtejro.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3vsfkvtho.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3cblkpeuh.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3qppcaxpo.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3bwbenelw.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3flcqqmyq.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3seldwavd.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3tmunbruk.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3nwlqkrsy.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3vqaxbooo.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3rqofwlvq.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3qxfanarr.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3uqnxsqxr.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3uciagsdn.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3lrgxzkir.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3tscmrgxg.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3sgkgjwwz.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3bdwweaui.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3wvdmkujf.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3wrspcnka.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3njxjcpvr.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3baazumrv.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3bnrqgiiw.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3mvfkhxul.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3yymmjlsc.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3kopddtiy.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3mbplbjdu.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3rkpsjdiz.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3lvgpttai.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3qkmeekku.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3yrwbicsz.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3zinvxmgi.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3jwjcrqjs.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3vqcqzweb.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3iymqqzhc.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3mfavirds.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gbqplgkk.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3bkablbnf.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3pgfrrwgv.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3ycqedkxb.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3vckhvdxu.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3axkgirkk.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3tqdwaphw.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3xqofzctg.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3ytgmjkcz.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3dfxrsvss.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3dldgmpzr.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3tisfllyd.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3qxhkxozq.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3dtsfmpwe.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3frqpcmuw.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3lixkgahv.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3jkvmkyks.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3dcfdcqbl.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3ylzcttas.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3jvfvozti.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3ejamwfoo.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3krvbhahj.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3mbobqphh.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3bvtryjmq.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3bdidhsui.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3awqoiflm.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3oglmjorl.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3zxerorow.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zgogmyow.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3orytvnpu.html


<!-- 参考信息 -->