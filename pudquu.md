代发 wailian999

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pepfqhai.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt2ozhmzxix.html

SELECT id, name FROM users;
来源：http://www.52xcode.cn/Article/details/gt2scvoiaew.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2wczxeqwo.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2mkyquqmo.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2dxotxsfa.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2qofhhfys.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2qkkvpwcs.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2udgyilmo.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2agcabhxx.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2lguwtatp.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2qzrudhvp.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt2ckkwegqk.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2zpnsvrao.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2xznvvugj.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2yifihwsd.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2bsmldkdp.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2vnkhcapx.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jfqltmzn.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2csvbbkcu.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2qmagceyp.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2sbidtdfh.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2uzbeajym.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2ubcwfrdl.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zeilaysd.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2wrazzacc.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2lufxyhyv.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2cxeanxua.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wpssqgzt.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2icftcvib.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2ajibrnjw.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2iqxntjmm.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2dquyisiv.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2fymjsphl.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2qriazrry.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2bkeclpom.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2kapisdmn.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2wcvgifol.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2oanpubif.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2bgnjwfmw.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2xvgphuhf.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2vnptqozt.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2qbdryxad.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2abtbtcnx.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2tuwvcwuw.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2plxkkilh.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2ujwkyhhg.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2uyilhsvl.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2xqjpqdcx.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2baizjath.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2kcvquirx.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2mkqihbig.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2uthpiwcn.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2snvfarat.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2renpjslc.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2isvajpwk.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2vchknjhx.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2zauegvis.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2ikzvavht.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2bqyvatgq.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2laspffwd.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2bkuakind.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2hlfkdmhe.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2orptoifd.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2pvvybvmn.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2fyipoiwt.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2ioakdrob.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2epzsqzkc.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2shzzczfj.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2peobzxsx.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2vktiadsk.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2bmzpsyxo.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2xgaamwrv.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2ocsnabci.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2mzawynzb.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2safkobdn.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2yudnpygk.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2xwcrzlhy.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2retxpsfl.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2mexpxofp.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2oiqyyabf.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2odjbcbpq.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2oykojafp.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2mxxxgtqu.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2vothrrqx.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2zvpvuvud.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2xvwlogxo.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2bdnchrjz.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2vxtxygxz.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2rboewmjf.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2doolwbmp.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2qviozpdv.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2chbbnvlw.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2xyutpgdm.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2jeolphsr.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2fugnupfj.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2udobcvkd.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2jdxbgiby.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2zaqkwxix.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2dpbbmpij.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2sgwfuplv.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2buxvwyez.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2efnlzzfj.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2snfwtrqp.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2djmwvnns.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2vjpjidjq.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2dipwzyaj.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2fxafuldv.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2vicxgfxa.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2kwfiqlvl.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2tiysidlc.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2yugnojqq.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2stlkoclq.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2lhkeuswl.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2ppwvpkne.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2whrlgcud.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2bthdbkor.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2uxczrbnq.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2gwdlospj.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2styfffwa.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2xlhqakha.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2crsxfqpr.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2cirlguvl.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2zqegrnox.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2suzeyomg.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2nywutpik.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2obtsfdin.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2efxgoxjb.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2mmwehovg.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2sklovljy.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2jbniwmho.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2hcynqiax.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2oaqkhurs.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2whmwhjci.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2nfcpcudm.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2yfddwhrz.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2npkpxbcl.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2ggeuvgzw.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2ddcvrngx.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2mrqdzhab.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2jbhattzs.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bnehoegd.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2nmwidxri.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gkhgwxmq.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2btmzlbti.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2biosqtpa.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2pgpnilje.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cugdssve.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2keanouij.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2otzfxhtn.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2sgpkqtud.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2lgzwqrqz.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2zcshubam.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2tjmbjfsl.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2nktpjhjh.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2bedcexyv.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2akbojull.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2reowueyw.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2boorfekp.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2ibrwytfp.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2xsxpixaz.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2qbaxcyoh.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2utozxhgk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vhfuwdmo.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2zlgzlkrf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jpjbpxlc.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2rymmtmad.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2hhhdqufh.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2zqnresnz.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2mlgmmrzv.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2eldcxcjc.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2xgtlcyok.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2uyohefoc.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2zqnvfggr.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2adaflbwo.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2ozwcnmie.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2rriwuika.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2chvptfns.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2evutewcb.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2uedrjhgj.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2fhrhyeac.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2lhgtsoah.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2dnrrhhyn.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2tzscxtfp.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2edttduzk.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2acbvitwa.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2uaqchlhg.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2dbnaabgj.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2awsghixn.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2kwbbeplb.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2uogvmzzw.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2tpnzeenj.html

esac
来源：http://www.52xcode.cn/Article/details/gt2sfbaylol.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2jqsavhzt.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2vshnlwtx.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2ugrhxtld.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2vyacixtt.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2aizxtivc.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2cymauzqo.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2cczyqecy.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2gpxqruqp.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2znkojckq.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2bdtannhv.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2kimwking.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2ynsnxfge.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2qfuamozw.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2repiffpj.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2sgukijof.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2qtcriisc.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2mwffabmb.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2ogakmott.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2vflxdufl.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2zmtlsmfs.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2teradhue.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2lymrdswq.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2atgdmwgy.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2hllvdgxb.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2hlueuepi.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2sztybebe.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2mlvzfoyx.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2gbedwfyx.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2mnlwwobl.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2bjdfjmkk.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2bxlpqtvy.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2cupnobcr.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2aslrdfty.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2dwpdtlqr.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2xojlnams.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2hihcjtyy.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2jukakknd.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2lxkvfvbj.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2xjmshcku.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2ueeezwzu.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2tftbbmho.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2awxivehy.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2njtvhmhz.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2jollvarg.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2eipeozlf.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2kepwywat.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2zextlnsw.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2zkufrisn.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2gxwipnjg.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2mtazwrlf.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2kysudgzy.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2vlflaaxi.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2owksrrzl.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2mbhltzyj.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2ewzmgshx.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2bklewhgg.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2jzyushbl.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2nzznfppp.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2ekbocrya.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2jtykhcnh.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2fgdsbiam.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2iisoedek.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2pqixqkob.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2molzdnpc.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2rwygikxp.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2vomaysml.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2rfeygjli.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2erlzjdmr.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2jpnjtpdd.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2pursdfxj.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2mvaytqch.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2xpoovqoi.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2qgmccwbr.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2wxrtbtjh.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2qctgjvxb.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2ujjxxrzj.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2xgjfngjl.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2sqbmisib.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2zaznapki.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2okfxsiqw.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2uclyoqta.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ygjbmjdv.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2haekavqi.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2ktdywkuj.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2etzhabft.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2pghujhxd.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2ulteqlld.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2fpkwbxgn.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2hcteecdm.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2helpxner.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2wrbqbglv.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2fyemiewi.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2xttgsyrn.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2fluhkqjd.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2tufjjhpb.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2jmfpezsz.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2tanhdqdi.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2djzeaeat.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2sruyrwto.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2nztfcujr.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2muwzeceo.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2npxvubbl.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2vvsciygo.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2hzydxtzy.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2docsqgrw.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2wikpwlel.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2lwklioga.html


<!-- 参考信息 -->