代发 wailian999

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2jzvkxbdr.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2zonymogl.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt2oifphxhu.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2tzhfuyce.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2aovclckq.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt2mmldzzoq.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2onhkchgr.html

[Q23] 分页
来源：http://www.52xcode.cn/Article/details/gt2gudylhoi.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2kzryythf.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt2igxgbpjz.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kxltfilc.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2xtlmxxof.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2tufyygmv.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2ucdlxdbm.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2muzwjtfa.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2wcfvpzmm.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ntjnnhpq.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2smmmnnop.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2hwhhgqam.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2meolkmcu.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jvjjgied.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2uwuedqyb.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2ggcpotxb.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2lgdllbtg.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2zxjtgwfm.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2wmzgzhgf.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2nayqrhps.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2qewvdqzv.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2gpiaggsw.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2zvmknjdo.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2qytksnqa.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2fysqfyou.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2fhktzntn.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2fmwsptal.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2hvltucfs.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2nhtkbnzb.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2xdypnrex.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2vfticzkl.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2qltiugmz.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2pcshxfsx.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2hkerzair.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2ehksdebz.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2vwgqbonn.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2llgeohan.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2oyosxxos.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2ymedefnr.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2scqidswz.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2roczfxwp.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2dvjdiadx.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2notipmdp.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2bbygzllb.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2cymsijcd.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2bxbazrgt.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2dliyfeko.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2mkotavas.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2lvojmjhz.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2prrtewoo.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2wowaetwv.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2iizakeac.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2szqcmoee.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2uneherfx.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2fomoujmx.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2otnyrvfv.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2ukmwxavf.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2grqglwtw.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2uofwdqoy.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2lgsksjls.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2qjljdkwx.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2fpfaczgg.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2beagrfxv.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2gcpmdurb.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2qxeoxzve.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2gouenkbi.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2qrusqibh.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2jtbtntql.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2zhbvntji.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2dzzuyvns.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2nfmuhhtn.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2rxeorsyi.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2zcynszuv.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2zecxetug.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2rqfkielh.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2jevvwinr.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2tsnnbgcp.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2phxvbsej.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2ehwmutzu.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2lowlznma.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2hguleetx.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2mkmxaqks.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2nncjcory.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2mbwhnbja.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2mqgcwgfj.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2otmxfwej.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2spadexfa.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2hossyvxe.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2qpuzlbra.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2suyuidbn.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2cnmxrizr.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2mgpkflvy.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2cxsidrxb.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2gxtutcnq.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2zbknctet.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2cjiyizmd.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2vvazxjbc.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2ugewbmgh.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2grmdugdf.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2qmmsnhfj.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2xcqnbihd.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2lvqjkccb.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2yoqcufbh.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2zolpngal.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2pbqlutpf.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2uzwcoaor.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2uifeiqxh.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2bjusurrz.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2ftvnxsqw.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fzmtjncq.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2mwutlhjx.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2hfmrqsxq.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2nzoqkyuy.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2mmiczczg.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2dtyliztc.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2fxalqvmc.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2mlgunxyx.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2obgjidlj.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2gdofanrk.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2iyuancis.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2mjybuuws.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2bzcvxlmv.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2gtulsuiz.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2juhdauds.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2ocgtdvlg.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2jzpwikap.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bjabppfa.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2hejicqur.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2rrhfgmeg.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2ucuuzsce.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pbhcsvoi.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2zdairhwu.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kwreundt.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2jvceqqeb.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kwniylly.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2lgaxdqhq.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2szibnftv.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2ohzetipd.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2irzhnoyw.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2aavkmupc.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2ybxayvvv.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2dthyleff.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2oodlwwuz.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xlpwzrji.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2oshvrkmu.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2qypkirgb.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2kwivprva.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2bdousufp.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2pkzphyed.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2zhzmptbe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rzartcbp.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2qmiwxzyb.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2amyrifxe.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2vrypxlny.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2nfqsnypm.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2xwbdvyuk.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2bhrkbpim.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2gifxmrej.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2nlniycll.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2ryfzjwvs.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2rdpzohif.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2exowqxfd.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2fwiuleuf.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2ilyawxig.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2cskabjno.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2gmqgjusf.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2jmgaqkmm.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2uftpzddr.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2fmzlqzox.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ahsmcllt.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2lbopovrz.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2cfwmlkjh.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2jrkxodgi.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2qgirmiqq.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2ujlzbujj.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2upxxiygs.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2hprijcob.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2wpygsagk.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2tbcbqmhp.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2onwymmdf.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2nizkpetu.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2nowcxirn.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2tglnwicc.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2jhhilotk.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2mwypkrxe.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2hgxuzjvg.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2nlioepcn.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2wpsnbcgn.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2torsqroh.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2bxlpgzas.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2ronudotp.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2cdtoqurt.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2irlewtlh.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2gvevibug.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2cizzzfha.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2jbwbvdkd.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2bedqewps.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2xpgcaety.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2yqngfgzk.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2mvqeexkw.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2sqwgwclc.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2smialici.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2lmjemghb.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2ybxtisol.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2unyhclso.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2lwlwllss.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2gikqrtcv.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2zhcjqtyd.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2ugvxwede.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2wfdqcnic.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2dvwohzcz.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2skiujort.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2ikwhtmfp.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2fhbngrfp.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2lihqdhqx.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2pjvembfd.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2xmjukrkl.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bzjvshlt.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2cmwmmmyg.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2rvabuyvn.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2fzjylmrm.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2jiszwtjc.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2jujjorte.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2betvadqg.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2jruxunrz.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2hmanmvqo.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2trpivudp.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2tdminprr.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2ifoqjtfg.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2zexvdgnq.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2ubkoegtp.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2ychziopu.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2frbafgwb.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2uxfqkegx.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2rcyusewk.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2lxaghgdl.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2abmqwqhp.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2grzmkpla.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2phtjoyvp.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2fhgjdzli.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2ktmokmok.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2ckmcpgdu.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2ovbarqzy.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2htettmsh.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2fgkvcqlf.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2zoxwywxb.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2uasswttz.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2wkpwcdnv.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2aukbsyqq.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2pjmlwwgz.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2rlykbdqu.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2opdlvxxv.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2joidsdjj.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2ckxuulma.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2zzoxldtn.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2sqecoqtj.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2utheswzk.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2swzwlzna.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2drjynxhl.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2pwfqzoge.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2kypoaohm.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2lrsbhvqy.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2bkagnffw.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2tosqfqlk.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2riqfieqt.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2kntknwwb.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2kpdmrqou.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2vvkcxxkk.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2gpxabpsm.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2mwykppij.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2ifvjynrz.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2qmsjihsi.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2hhiaxkyj.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2rguyngao.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2yooxtcgq.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2ubzyslsi.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2dyoejzbi.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2gbofevay.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2ogxlkrbm.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2jocztjkx.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2shfzaqrf.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2hruaxljs.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2tsbdrwdq.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2uiccgmci.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2xsvetijl.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2pzxzqcuc.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2fcfrronu.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2ilunbofr.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2rjsmlxcu.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2oxwekspv.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2udulgbtz.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2lxbviepr.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2oxocwdtz.html


<!-- 参考信息 -->