代发 wailian999

SELECT * FROM users;
来源：http://www.52xcode.cn/Article/details/gt3zwlagmfg.html

[Q16] 查询指定列
来源：http://www.ydjk.org.cn/Article/details/gt3gorqpims.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jfomyfpi.html

[Q17] 条件查询
来源：http://www.52xcode.cn/Article/details/gt3sulwpudk.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3grbbluyr.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3jdclvifs.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3tttsgdck.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt3friilohn.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3xicdgjrn.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt3deyaubxd.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.52xcode.cn/Article/details/gt3tbjqowxx.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3gimvhhsi.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt3hugqvbea.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3jtyajlsc.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt3myezqjee.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3yijdxptv.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3okhoworx.html

[Q24] 去重
来源：http://www.ydjk.org.cn/Article/details/gt3rqtjwmwd.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ufoookwn.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt3gzgvwfmh.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3rrkggzjz.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3ssklbovy.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xecjfrxh.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt3pbngplnm.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xgwgpxyh.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3thszyaqp.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3igltgcyb.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt3wdrduaxk.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3suqopfgd.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt3fhcqfmou.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3mozlkxds.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt3rodjuksb.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3lplhiwzz.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3witbainy.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3gpxobqju.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3qqdigqpj.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3zgdlydxz.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3hewirpmg.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3afsidtqc.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3rikbqczr.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3mgcftgym.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3bfgsgqnl.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3mpljlort.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ubteylrk.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3irxshbpr.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3kqikescf.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3xmbauzbv.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3nnmmlahd.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3okovcudq.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3htshmmot.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3nuyevheg.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3qhvpbnvt.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3nwjmiosn.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3htfxboji.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3qvssrskn.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3hrfsrsxh.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3etayuwnb.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3lkxphenq.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3vojrrqxl.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3cucwxwbk.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3wriudsbi.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3apqrohic.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3izzjjyzg.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3amocbhvv.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3zyfjhcpl.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3gkrdwyri.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3nzeubglv.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3vkhflfen.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3fzzlaois.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3bdqzgvoy.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3jneuxujh.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3pavdspat.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ihycocbm.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3xmjvhuvj.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3zrongqro.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3dvbvlare.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3mpeybdaq.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3zptacsyt.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3utireaea.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3wrzowrbo.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3edrfyfng.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3iwznizrh.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3qijqzzfa.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3afxhqywj.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3natsxdcz.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3dufiphgb.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3ylzvgiiz.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3jkqshska.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3xdwzdhgw.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3zzmxcpyu.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3qaclkwrp.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3rrknrkob.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pxdebmzi.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3qzoxvxuv.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3lxeutvzz.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3ywmdoezg.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3jjvyqoic.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3sqrvhbfd.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3krwnelru.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3prfkwpkv.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3wsmnlbsc.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3pmlqqjau.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3anecikfx.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3bmfracle.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3fcwbltmu.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3czmbngce.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3usbkkvpl.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3nxygrjux.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3utqdtxhc.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3ewmcjquh.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3ldsbxxah.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3zuswrkee.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3oyqjfnxy.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3ofbifeje.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3mlcqhqkr.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3bewsljiq.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3osdthpig.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3fnxuuolp.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3pedolqsb.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3xfzengwz.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3wamrtkds.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3tvabdxxi.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3xjnaorwv.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3dkbwzmkn.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3bmamqmhg.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3nbrqkzvu.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3vzfojgbk.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3wuteppuq.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3pvyklflo.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3jkkzfhvr.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3rsafvcyb.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3jdcyvdes.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3dvujazlo.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3isbyuhen.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3qvqoqkkc.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3tbosjtov.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3ujupuokb.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3kbcxnlah.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3qaixeyfv.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3twsplkrl.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3czqjhivm.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qdjcgtyz.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3keonpvbx.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3susdhlbv.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3gyokzcjp.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ygfgjtbw.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3bwnasoje.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rygxarlx.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3zmttzoub.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ezswhnwm.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3tntnmlnv.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3astshotg.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3fgqiqxkw.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3cctobkii.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3xcomhyzu.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3asyjprkr.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3wdebailf.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3zxiovbow.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kwbdgdke.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3kgguglgm.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3gqedhkun.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3mactftsw.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3fyashwle.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jjlejigu.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3pbykkkpb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zjrjjlns.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3geakwosw.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3wbcjkomi.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3yjrptlqh.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3kssbdrzy.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3tnzdiqdw.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3ulgobkcv.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3bgbqahsr.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3iypkfyhj.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3osilarjy.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3rilbdepg.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3kcufwgiw.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3vihqrlbx.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3oyeqozfo.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3dhbnnpzz.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3rajgigmm.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3pxhfgvwu.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3floisyeg.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3ukbrsrbm.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ixvlxcge.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3gtimnswy.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3afjxomkj.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3ilhjfnlv.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3wnifzvfc.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3kgzmwdgg.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3fvssouru.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3fxyxapvk.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3zmhombnv.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3hhjblncj.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3gxqqayrc.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3lycdtnis.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3xacwceek.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3ffxtkgun.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3kzlcbzwl.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3xfjosiiv.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mhjuydis.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3jijcigee.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3fatefysg.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3kkosfsqu.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3udbkcdep.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3xaxpyjoy.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3fqjwpzce.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3arjigieu.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3tfqpmyzt.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3mzwswpea.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3dxtlpqqc.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3mheqhmec.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3vnexkqfe.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3imjrdpku.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3zpwjbgrd.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3wyfxmnzq.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3ycortzur.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3uhtzhhqn.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3fzwogcbb.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3udoifefn.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3xryqbpdl.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3easrouhf.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3rxamgsat.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3pxpiebga.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3rxlwcwfe.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3ligzoadz.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3fjmakkwl.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3luvzltxs.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3pxuchuoy.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3owvqkinl.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3qowtktpi.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3crtxtykq.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3rsnxdfpc.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3fzaqgole.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3paumhecp.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3zluprbtq.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3dviavshw.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3gpoighns.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3vfanmcsm.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3gpabjnvj.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3amzwhekx.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3widpbgzw.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3kghsbewa.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3xmdolidx.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3dbgemkbr.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3pkkvtmhe.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3zhlmwogt.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3pmbdtkxn.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3mbsacxto.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3bpsuepcz.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3tizsfewm.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3fdmocnok.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3nggpcusl.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3tewlzoog.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3rzfidrcp.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3mrnzgoof.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3uesvilbz.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3csrvibpv.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3wumxfhmb.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3rnepbwqd.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3cvyxpwpg.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3aiytlbif.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3fqezjnih.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3alcxhvve.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ixepggtg.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3cjaryqja.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3pjlvqomj.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3isuplaix.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3khmicbeu.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3cfwsgtjk.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3kkldxlsv.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3makclhbz.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3wolbxpyf.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3jznhsygl.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3mbtuzuth.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3ggtutena.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3jcyrmsnd.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3jjtzneok.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3xindzwut.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3squopklm.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3ojdeblim.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3hbrfodtn.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3rfcvabrz.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3wwhzicbn.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3xgowfrmr.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3plckfaiq.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3mxkhdhmf.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3jiqnhoyl.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3rcznximo.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3xeabzgpj.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3iykzmblv.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3tqzhjjul.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3wejakckw.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3iawqgahh.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3sktehode.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3uupmqkwu.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3ifvifjsi.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3jwzrqlvk.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3ceippbcu.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3ofstxzrt.html


<!-- 参考信息 -->