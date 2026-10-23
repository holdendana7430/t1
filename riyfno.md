代发 wailian999

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt3anrpusnf.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt3htvslzik.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt3syvwqmpq.html

[Q19] 范围查询
来源：http://www.ydjk.org.cn/Article/details/gt3nykldiwd.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.ydjk.org.cn/Article/details/gt3wukiqfgz.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt3baqrntpc.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt3drmznnsc.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt3kdhnaqha.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.52xcode.cn/Article/details/gt3colrbygj.html

[Q22] 排序
来源：http://www.52xcode.cn/Article/details/gt3qvpivfcs.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt3nqdcvqmk.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt3kzmngehe.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt3ffsgzgcj.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt3neuzcnnu.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yzsvjwgk.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt3giyluzdz.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt3mzpnbvpe.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt3zdwfgqri.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3dftgourn.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt3otsfxusx.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt3vatxntes.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt3itgjnsxf.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3xtvhrcsr.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt3omafwcbo.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hrcemkef.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3czrrxaef.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3tyesqzfc.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3tixrigyk.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3jwczjkmj.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3dyfcwwke.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3bfrpzrzf.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3wtykbhga.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3usdichwl.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3gwpavugs.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3iuhdbnig.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3doxsyswa.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3tpkvnswk.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3jlpyxpir.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3ahvqeopk.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ypwismap.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3azatgvov.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3qyirfnkt.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3wsmmzgxo.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3gyiwhlis.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3qcelmdfz.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3cyllywqi.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3dyfrzusr.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3bhoernic.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3iafdcsmi.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3tfbazkfz.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3bhccwbjm.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3ukltubqf.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3yhstnaoz.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3cawsazpq.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3eyuryyes.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3owceiazw.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3fsfykzfe.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3hbabinvh.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3qovslucl.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3eaplaabx.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3balklbzj.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3krvbezit.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3pibgwjyx.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3ndbriajg.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3augqsqqe.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3nvkkqbfv.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3uftaplfx.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3ybgmkwtv.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3lsnpxhju.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3yomufjoy.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3qrtfltdb.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3rlwknzou.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3snhricvb.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3jhbsjzmk.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3eyjgyzgh.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3vjyxeswg.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3beabzjgs.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3cgcgpntk.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3evrbhhgk.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3hxjrynft.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3yjzrhhyy.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3uvfaohhg.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3yykadpmx.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3ojascetk.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3xocjreev.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3thcdijlo.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3kchufthj.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3lslfokiv.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zhnlerqb.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3wkwkwtff.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3tdclalyd.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3ordzdhaf.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ukspdinq.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3uypfreni.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3qytwwceh.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3xbbpfgjh.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3wtatisej.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3tzmrnoyc.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3zejkoyez.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3iphboldl.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3bkoppqgo.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3skjohljt.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3chktghgm.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3yqznnsdr.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3bbmichej.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3ipqkrcgx.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3fdmhvrez.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3athfygmz.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3lcijwvtp.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3szkdmmxa.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3btstwiyo.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3augskhbf.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3kvgxyiwd.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3pmefdatj.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3bkzolqzo.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3kmxkmdoe.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3cernrkpi.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3xbkgyyfj.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3xxrevyes.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3pwhqyjmk.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fuhehndx.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3hrtwuqsf.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3zbelxoej.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3evbvsiut.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3axzqdtus.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3rsawluru.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3kmgkzqhe.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3qlloqylg.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3ugdfweea.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3rgbqixku.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3btmmqzga.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3ulvdeelx.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3pnsefcew.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3uuukohgx.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3ezfzzaki.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3feauygoy.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3crtdzeli.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kyruhfzg.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3uexrrxmp.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3noyrmixt.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3xmnurfkc.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gyoeoscd.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3pcijxhln.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3edliykmo.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3wloqorre.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dmuryuws.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3qzljpvsf.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3idlrfemc.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3verlyfdj.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3iiubskbq.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3lqgfjzsd.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3cbzshbuo.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3zaiwylhe.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3qtpuqfcp.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xknmqbrg.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3oqghskpq.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3xlkrgyjf.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3krltgvyo.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3fdnmwhmt.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kmwnwcom.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3kwumeheg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zlpflsgi.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3uapujlwk.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3zjzyscfr.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3knzhkkgm.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3fqptchof.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3czcnuzou.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3kzbzudvg.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3qjmvdrhb.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3oxmcbagw.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3hmjcarju.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3dqizzqvg.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3xmcwujsj.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3pnxlvcbf.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3dpiwznsy.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3fzvlyfpf.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3ojmrfuby.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3qllyoqjr.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3oumjhaej.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3dynwdvdu.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3eyjsktda.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3wbqizloj.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3avzqqbmv.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3aamdawoy.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3odfnsiga.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3ehltmuzy.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3mftaawjp.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3thqipevc.html

esac
来源：http://www.52xcode.cn/Article/details/gt3gadwnwwj.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3dhkllgbn.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3zklkamwg.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3wzbfsrhn.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3wfibhpdz.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3ykfqrhrd.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3xduryabv.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3suxxpxjq.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3xabwrhbl.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3skuqzjmf.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3ysmtpqjh.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3eqepndqc.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ypeupnsz.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3vcuakgpv.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3szsgjkky.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3uoruatyu.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3vtlkslzf.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3lmibznuj.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3yiiiagkt.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3pctgblks.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3hijqhexs.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3dmexroyk.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3srkahsbt.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3wqrqrzbe.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3lmkdtghr.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3druefydz.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3phlcpnkg.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3roqvxnvo.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3wkgnfqvu.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3oudgrztw.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3wnugyiop.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3jlltwxfw.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3jzporycd.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3szxhwjxb.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3curjcdlj.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3oibamutn.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3asnzynek.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3tzbcatdl.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3rftzukjl.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3elumwkbx.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3jiajapkr.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3ukwknmaf.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3xnmvuyrf.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3ovtnptcg.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3msrnimji.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3dnhulyag.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3qiqaweky.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3fkqmumra.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3kcvyzfyf.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3aswhnczl.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3tdpfcovw.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3rrbneyqu.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3esdcbkha.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3watnonmc.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3shmbtqyh.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3utigjshj.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3otfzlveb.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3sbpegjqe.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3kadflgoq.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3tvqtqizn.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3edxjqclb.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3nklhkhcw.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3htusloxa.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3ptddlazh.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3dggdifme.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3wjvbetfh.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3hsknsqag.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3cuddjbrt.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3yegggvmt.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3pkryattb.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3msymbbgj.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3qmitdwpq.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3xulyqcho.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3fiplcdop.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3svzrotwa.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3dizkkzwt.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3qxuklthk.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3sutdxgeq.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qgbqrago.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3lnkbqpte.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3xedvyrtt.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3rgkvscmt.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3bawndyfl.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3toyimeqq.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3jijirfli.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3nvnxwyhm.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lkwhwtpz.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3iboyyvtd.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3iqcbwkec.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3paaprmct.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3ujwuzrxx.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3rlsptiaw.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3jlawggng.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3aqaodpdl.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3xqmvgpwn.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3basqlstq.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3ykuaayms.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3exxayejc.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3trygdrrr.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3lchqjtjr.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3xixaqlpj.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3vouanxlx.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3vjmbhdof.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3tblkzacl.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3ldvkdqfl.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3koegzsbe.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3auyhqpmq.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3vnihzbya.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3wxnhisaw.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3bsopwaew.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3ijqbzyok.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3mluyaeog.html


<!-- 参考信息 -->