代发 wailian999

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2bxmholch.html

[Q18] 模糊匹配
来源：http://www.52xcode.cn/Article/details/gt2hpmtrncj.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.52xcode.cn/Article/details/gt2wraboqvc.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2qlhgvktz.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2tijkkntr.html

[Q20] IN 列表
来源：http://www.ydjk.org.cn/Article/details/gt2wrgsqczs.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2iwkumlvn.html

[Q21] 空值判断
来源：http://www.52xcode.cn/Article/details/gt2kikmpxpp.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2rrzvxqfn.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2clmzxeem.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.52xcode.cn/Article/details/gt2ipoiztxv.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2kqkicvpc.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2reitnrtb.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2ebthdfer.html

SELECT DISTINCT city FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tsyravrk.html

[Q25] 只取前 N 条
来源：http://www.52xcode.cn/Article/details/gt2vsavtjtg.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2zfarjcrw.html

[Q26] 计数
来源：http://www.ydjk.org.cn/Article/details/gt2ohcvqzcp.html

SELECT COUNT(*) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xmgsurpz.html

[Q27] 条件计数
来源：http://www.ydjk.org.cn/Article/details/gt2mvpbmdmi.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rzecpodg.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2cyijpnuh.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2yxpzbpze.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2bnekrard.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gmlpljkx.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2ceygkjcg.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2ncxavogi.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2jrsyxtkg.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2uznktakq.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xgjwgszn.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2hrqbvccj.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2ormxpuwl.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2fzrcqrlo.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2pqgmlmja.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2bdwnbwwm.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2hhllsddv.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2eglifeuf.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2uhpkxqxi.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2ihlsflcy.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2jxesorxm.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2xnmvfmvd.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2qpmpvbgs.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2tororzla.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2tbylinmk.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2jzbaohvr.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2pyoynbdh.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2htvhhhgk.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2jjryllmg.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2lzpzscqa.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2cxkhnfcq.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2ycugpudv.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2ljbnduur.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2leklclgs.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2tqmurlbs.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2wnchvube.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2kyldfook.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2pdxrzzda.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2nsesoxdm.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2gnmzuodq.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2yeuklfis.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2wumatilq.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2qsitdpfj.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2smdmemxe.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2yenljcif.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2idwxnoby.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2pfoqeqrv.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2pehdckjf.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2uvthcrlm.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2btdlhigt.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2baiejbru.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2xzpeudcx.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2pasgovuj.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2hyuyfsvw.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2jcrfiopg.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2plfwkzmm.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2vsomzqqc.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2elwnlenp.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2sitmmszw.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2gcuucmie.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2pxtvjrrx.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2pfgkkjdv.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2nukhhrou.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2nzjqaotu.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2ynyxapro.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2lqfvrlou.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2zmsmgpth.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2vtbjkbie.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2bulhlzzd.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2liynsojt.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2hrneuqvt.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2onjdqrrg.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2heuktugn.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2whgrefuc.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2hmdohbzi.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2tpcwgraa.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2jlajwofe.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2ujelmugc.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2qrlaqtco.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2cssvdupb.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2nfazwcca.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2zxfmzfxu.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2xxneqqpv.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2fubkpmtb.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2kvbsyaud.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2bgsdkptu.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2qbfgmsts.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2ytbqhxbp.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2wkrdifko.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2zsilnwgp.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2ffoeysvv.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2zelrizml.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2cbfckxkm.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2ufyagqhh.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2kbsfpckw.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2gmcugiqm.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2lnaeovhx.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2ynoyuaau.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2tyloisyg.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2qzerkhio.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2lczksydx.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ooanajih.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2hlnlxpno.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2ulgxygip.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2mtvlusfb.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2qptqiyfq.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2pyqnepgb.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2xxvdijjj.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2epfnpskd.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2yrppalyr.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2uelhbakw.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2spdzzcxz.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2aklyhydi.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2oyallbxz.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2udvqyojm.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2crmqhdqt.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2isqabjnv.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2kyldgnsm.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2aoptacxt.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2igpyttmi.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bhskkewk.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2ctxzstme.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jkzhlwyv.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2ztiqqukg.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hgbjzhtz.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2raxdyafl.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pwmkoodm.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2czmzcqfw.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2iucprsya.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2qcldeqbm.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2wahufvlm.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2bctsubxl.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2kqdqxbsp.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2dvhtuvkc.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2rilhifud.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qshtwuee.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ywaiylab.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2ztsywgef.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2btizpigu.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2lqleokcg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wedssmeh.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2deuzdrdk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dglrrurh.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2rvqjmuqs.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2clcvbnva.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2nsqfuulb.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2excqkgmi.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2xfrfoyyi.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2zcwxynzi.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2lpimtpzl.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2dfycvgik.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2giitjhjw.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2olsfdlfm.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2jpbeyvfk.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2xnjsbqav.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2ibqafugx.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2jborjhhw.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2rkizqtvc.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2ixgvosgr.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2plzlxpkb.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2khedpezv.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2sqjvnlcl.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2xyhqrlef.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2nztduapr.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2wnpcrxxe.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2jvrkcini.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2nynjquaa.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2wuooulqf.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2tumtbqam.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2zojsisfd.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2unyfzrbu.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2cnudadjg.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2ybaklkcs.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2srjaismo.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2lonajbca.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2bgcqvflr.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ynkcenfv.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2iqpazfea.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2xqwblxrc.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2zonexzmt.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2hpuetrmh.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2juajtxxh.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2mghgefvo.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2fcrpnsol.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2agvnlful.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2ophzffhh.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2mvnwkjbk.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2hgroalqe.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2rbjnbxhv.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2acobzfdl.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2nllesbvm.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2phccopij.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2gptkvght.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2foalodig.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2cchggfws.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2zuinbbtd.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2nusxakkv.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2ibbdmsne.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2idxkqwrb.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2hygouhtx.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2wkltousd.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2wmhyicsa.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2ouwnrhnl.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2btbkvzga.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2sepkopox.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2zwbvnzvg.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2npzvbcwu.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2mexzwhhu.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2eiruzrse.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gkjzpdtv.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2biceqcuo.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2fmlgajky.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2izxomwpd.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2rvsduhef.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2piklsaoy.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2zoreqzoz.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2plsqaona.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2jemhxgfj.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2jabvxqej.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2qakbfyoh.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2jqvhweym.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2blsdiblv.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2qjirqfkd.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2xoxurttn.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2riksypkg.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2msvqfnke.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2kbijhbml.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2qycbyjer.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2gigfoeok.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2gyjqrczd.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2qgyphtwj.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2aftcrgem.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2uuyzuxfc.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2apychfgj.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2cloeykyk.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2yzumnrir.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2zonagrqe.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2yfaojofs.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2tflqcwpe.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2zshvksbw.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2bczmlfsx.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2oxbdausj.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2klcpgkpg.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2coxhdwgk.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2gxrmxvna.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2nbamtogm.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2vjddcohh.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2wxotagox.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2ritcfcxw.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2cklwprfv.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2qyfthkor.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2msxhrmxl.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2ywcamvme.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2kockhpam.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2twlzsycy.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2gebswsyt.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2omkjpmea.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2uilumovm.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ldmiqqhd.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2hmneliya.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2ilmviimy.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2bnbxruni.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2lbxetxnw.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2bevbhjvm.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2zodmoxbl.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2zsibvzmk.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2caxzfiuc.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2rjceljwo.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2sojcidbf.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2xpwwmtvg.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2rcknmftp.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2svuogonm.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2dizjqnst.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2ezjhepqm.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2kfrvjhtk.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2axaalrgd.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2imoqhnfl.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2ljbyznui.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2ixfooycn.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2memjxlwu.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2xnewnnht.html


<!-- 参考信息 -->