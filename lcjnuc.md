代发 wailian999

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2nnxclhzs.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2zpypeoka.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2qehzayzm.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt2txkosktg.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt2mfvcdvfy.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2bjbeiqql.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2fdrjutmq.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2yywwjifz.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2acwpqwck.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2cpdfpsla.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2yasnjlcf.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2xkhppiae.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.52xcode.cn/Article/details/gt2lywstwsp.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2mrzogifh.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tvsqqeie.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2smocetof.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2updszzhl.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2mlxykvhq.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cumgeeho.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2nogkwhce.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ylycnhaf.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2gaehaxjw.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2zjdlyrte.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2zybwbsxo.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2brejpzpe.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2bfpgjzuf.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2noofqjnk.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2wwfesceo.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2jpfmfhhw.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2oirczpwu.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2adnygqrm.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2qqebzuhw.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2vefxgnps.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2vxnmzwjd.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2ogatncff.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2qpidowiw.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2kxqoddob.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2mshsiykt.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2foxsigsv.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2pedjbpdq.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2dieqhaqo.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2dwladjql.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2nyadsilp.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2wqvdhmje.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2pinzrkiv.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2bhukccyc.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2okiudzzg.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2vbiknowp.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2yzffnvld.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2vwzooapf.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2rhwnraok.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2wuiwbgya.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2mqyaozpu.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2zgpiclrj.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2nxbrzyik.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2zaeugmda.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2ybowtkua.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2uchrmpwa.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2zhltkbyv.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2nhoruzzt.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2uxfviyfl.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2frqxeljk.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2swxgiiyx.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2wlgztbdg.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2kqlajmte.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2swdkvfld.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2hqpukptk.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2nqkllcgg.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2adwedpei.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2gyxwdyvo.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2vfiwakoh.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2rawppwti.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2tovmwnuo.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2tidzexuh.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2hvcotvdb.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2coamisrl.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2nshloqjo.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2oahcdcuf.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2qpkhhfcu.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2mdpdficx.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2kwaqdvhf.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2gsxcshgs.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2mqttolah.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2yckazaao.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2piunjwiz.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2msgdgfdb.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2hqcztfgg.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2ovubczbv.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dahwqtbl.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2ulnpjfww.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wpnkqnsj.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2uhwwuacf.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2kftjehja.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2szgexesp.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2nfgccajk.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2xhobwyyk.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2ogfrvevf.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2nmuiytyg.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2umhwqdtn.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2gzixulqs.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2ymuymqdr.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2uicxrnum.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2tjjzoaup.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2ufswblpr.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2xwaqngfp.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2azjmhmdr.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2vbueavio.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2tjmryyim.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2ymiopodw.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2xxviwpzn.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2inziuzkt.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2teycjdbt.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2difeqrxn.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2gpijhkzb.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2aliydiaa.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2wbwuybsk.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2bbuixqag.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2rflncznw.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2zpbmuptq.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2yximuahc.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2oiuehhye.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2wjltthoo.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2qvnaqwsd.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2psrvtpnx.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2ztolxavi.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2lcfimdhb.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2mpyvfiwk.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2oxldksll.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2iznukxsl.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2cffftfgh.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2azjpsopw.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2qbgqexql.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2zgcxnknq.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2trvglpck.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2gifurjds.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2bahrhduj.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2vqvayeyq.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2exshrjrz.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2hzqnrlhj.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qxqdghui.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2cjfuzohx.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2shvaozko.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2qxbfuonw.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qryzwrrx.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2gwzybciy.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2holxueyf.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2glsmjykq.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2runopdbd.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2ipsemiuo.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2eturyuzn.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2npdeifcb.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2hjlkwvpl.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2lncvyjnm.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2dwqynfct.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2byaszxdt.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2kydbrkce.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2lojujsum.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2hrhmpxzt.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2ujosvkpl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wxabewmq.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2odljopom.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yxqxozki.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2kywbkfeu.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2lqqyrijq.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2hpteqmjd.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2lxagcraf.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2trhmofqt.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2unylokon.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2egrskvbn.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2htkxydvk.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2mfbjfqwr.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2qwgfiylm.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2xpxxdafa.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2dqyuinik.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2skekwqfj.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2odpzgtkl.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2lapbxsnz.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2pgkuasac.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2ufmzlxpb.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ixsufvqu.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2hjtaluaq.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2kanwpzpr.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2rmryoqrh.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2gbifaqcd.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2mwoiyplh.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2xudctpxf.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2nezhqbdy.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2wbyfizkw.html

esac
来源：http://www.52xcode.cn/Article/details/gt2jbklpdlz.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2jlvisdbi.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2lojfmerc.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2hzfscirj.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2ybercjxw.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2wksqovje.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2mobvdyva.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2owzlalmc.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2nuuxzewz.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2lgvkwsle.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2flezzmed.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2cplovxgh.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2xzeatlpg.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2fsjwbdbr.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2byhpcrbo.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2efimzbxr.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2yplzowdu.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2ebfhwgsl.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2chkfblsf.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2eemruusa.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2jriamwmw.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2sqkahrfe.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2jbtmdjuy.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2dnpvvtke.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2gkhjnsok.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2zvfaqfvn.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2tgsvbhen.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2lcwrgwoi.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2fsyaznfb.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2xdbddugl.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2ifidwcna.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2xogxfajo.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2osyzfylx.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2ibbytqvm.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2nyhsupqh.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2shzynucj.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2fkmquxvc.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2irgmeyej.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2krewllht.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2jqluojwi.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2qzyoetyh.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2rfkmlbvs.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2qkquvdof.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2gctvyfzl.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2inoitusg.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2graaxhxt.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2gnqblorq.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2yrzsfmys.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2mwcifbaz.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2hllqzxzd.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2pumrakga.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2yrpzbcde.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2cmltzutm.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2cdaoyqqp.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2kqkhedxc.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2lsoqmfrh.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2dojvthaq.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2ppumkbzb.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2pejrjyvy.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2owcddyos.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2hlwjuqqh.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2rfxktfaa.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2ohzucesz.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2bvgtbgmb.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2pzizhvkw.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2fvtskeoi.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2tzuqfpif.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2tppqqeij.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2dznbsvqs.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2nbvxjchn.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2lbjvijqw.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2raoxaacf.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2juwackoc.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2bwnfdhnu.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ufzzavba.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2qkakfaem.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2qyrlutur.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2estfxbok.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2cssstisx.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2usfjyszq.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2ngtzjuvr.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2jemmjntx.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vtiuqgvj.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2rakmzhkz.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2xuoiirbe.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2vwhlxnet.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2liihmgmz.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2kfxgsrkh.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2zediyfvj.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2mkqgnxvx.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2ybvkkpqf.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2voshthwd.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2mvylczkl.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2ukqnoroh.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2dvujzdbh.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ewgtbzsb.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2zjneuebh.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2qcsxrxbg.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2riekgjai.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2aanipnoy.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2dblqqqxc.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2hkeabtcp.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2xmpvstaq.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2pvjbwkpe.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2qulkihog.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2klinpivc.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2csgafnxc.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2amcotrre.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2kjurtolx.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2zgacotfs.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2yjbmlvji.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2gqirmtzt.html


<!-- 参考信息 -->