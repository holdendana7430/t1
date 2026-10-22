代发 wailian999

SELECT * FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ghxlthmr.html

[Q16] 查询指定列
来源：http://www.52xcode.cn/Article/details/gt2almdbwsq.html

SELECT id, name FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mntimdiz.html

[Q17] 条件查询
来源：http://www.ydjk.org.cn/Article/details/gt2yhjzrpat.html

SELECT * FROM users WHERE age > 18 AND status = 1;
来源：http://www.52xcode.cn/Article/details/gt2jowzymkk.html

[Q18] 模糊匹配
来源：http://www.ydjk.org.cn/Article/details/gt2xstrmswn.html

SELECT * FROM users WHERE name LIKE '张%';
来源：http://www.ydjk.org.cn/Article/details/gt2hxpsakfl.html

[Q19] 范围查询
来源：http://www.52xcode.cn/Article/details/gt2gbzbhrqw.html

SELECT * FROM users WHERE age BETWEEN 18 AND 30;
来源：http://www.52xcode.cn/Article/details/gt2kiuicleq.html

[Q20] IN 列表
来源：http://www.52xcode.cn/Article/details/gt2jkfrnifm.html

SELECT * FROM users WHERE id IN (1, 2, 3);
来源：http://www.ydjk.org.cn/Article/details/gt2fghcqumx.html

[Q21] 空值判断
来源：http://www.ydjk.org.cn/Article/details/gt2yvfxhpec.html

SELECT * FROM users WHERE email IS NULL;
来源：http://www.ydjk.org.cn/Article/details/gt2octudwxe.html

[Q22] 排序
来源：http://www.ydjk.org.cn/Article/details/gt2uxicbtnr.html

SELECT * FROM users ORDER BY age DESC, id ASC;
来源：http://www.ydjk.org.cn/Article/details/gt2xgdxknhf.html

[Q23] 分页
来源：http://www.ydjk.org.cn/Article/details/gt2gjgzjipl.html

SELECT * FROM users ORDER BY id LIMIT 20 OFFSET 40;
来源：http://www.ydjk.org.cn/Article/details/gt2htrwaxos.html

[Q24] 去重
来源：http://www.52xcode.cn/Article/details/gt2jvtvausp.html

SELECT DISTINCT city FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cshrxwuh.html

[Q25] 只取前 N 条
来源：http://www.ydjk.org.cn/Article/details/gt2amecmyui.html

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2ygdmoxub.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2mtybkplz.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2khlxxuwo.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2zicmkbij.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fowyaolu.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2lbfmnbil.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2daylluei.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2czuvydfp.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gaxxnoqj.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2auqadqhq.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2xtjfjack.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2gourabrw.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2vjjicocd.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mhdmqxlb.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2rtbxvgru.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2lydvqcvs.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2onhehcee.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2gplinzzl.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2nmiicvqo.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2ulknfgup.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2qfhsrkmo.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2qvryxwcm.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2wchnfqcx.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2hxiuekbz.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2rvkupykx.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2balgdueg.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2jxlwfzaq.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2wcirbgxw.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2zfcmrosy.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2wsrdrvho.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2gmwfhgow.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2cpsfkoun.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2kmnsxqen.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2sinlulqb.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2lscvzvyy.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2wpjavata.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2enzqjuij.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2pxnzcqdy.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2gkpqnchz.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2wjinrevm.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2iaowyxtv.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2zcrjpwwl.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2lehfmcto.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2ruzuznxh.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2zmyhmkej.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2tgtpbgtl.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2pnioghmu.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2bidnrqlk.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2ecsbveiv.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2sdkpdnzb.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2ecjpuyta.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2lfvqvnkx.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2djvbfncg.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2oeininyf.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2ifwjgeti.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2yqdeiyfd.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2hzfnfzzz.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2lecjgpzh.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2jhhjkioq.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2lzyevnxl.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2cgrdzgtn.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2yihsjlex.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2mosgjpfo.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2odqnzhxw.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2qcawxmkp.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2xzmwokov.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2msfqjmlc.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2bjdqgfoy.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2ftogmiry.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2jpgpnios.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2rqsuhkfk.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2tnycugms.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dzucippt.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2dltjldqw.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2kfbjcfwr.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2edccaxqu.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2kucwzjuh.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2dtoymxio.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2vzdasszu.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2wiavvwtr.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2myhnmygz.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2gievekdj.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2lgubobeg.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2wfkvfoaq.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2xfokovne.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2ubcrqhpr.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2znximdwx.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2iwtibmyc.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2ieilsxhl.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2nxxhyqvd.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2otbqldxg.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2qhdkvlin.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2pwqdtoss.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2yneildyl.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2zzxgqeln.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2nhmadjbr.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2yemtgmhs.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2gltwmkzl.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2nfqospfw.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2olbspbib.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2cxpvffgl.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2hhfctmwm.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2wrcyxern.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2txcyvrrd.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zslvsgbh.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2iemweeyf.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2mskbtrsf.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2sgstaoxb.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2uwdguzln.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2atfmyteu.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2fnmcswoo.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2khmolvun.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2ybswrdej.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2vihkxiky.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2edskjocg.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2iyywrsjp.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2mljtrlvh.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2rteqpupe.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2idlqwzvu.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2xofwocyq.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2jrolilla.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ceifksqr.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2yukgnupl.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2bvkcohfg.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2aomumeaf.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pjzqnjkl.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2muonzhbd.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xffsxszx.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2qcilbdfx.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hjicryfc.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2jpbdsrny.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2svstpuex.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2yqzibcqt.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2owtzkdih.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2xwnwghcb.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2ydhnuwjm.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2pofmnieq.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2hwezvcic.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2neexhzxp.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2ncqmlkxs.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2typtukzw.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2vacursuu.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2xbygqcfs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zvtqhbaw.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2ottjejmz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kemnmgah.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2vtfwpifa.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2nxqxbymb.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2fswhygwa.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2gkbtjbhj.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2vfuzmiyk.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2emzsblty.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2movrwfip.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2snnkckjg.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2rhfugqdz.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2tekannxk.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2pijixqmy.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2cboznjkc.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2mmgnxodf.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2dcimffhd.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2gkesogsd.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2epajzlhc.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2izrvqrcj.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2fufszfwf.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2tnwfhqwx.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2olryplcp.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2rvgzrrvt.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2uesrtoqk.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2nffmdbte.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2eeynkfzv.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2laeaqycc.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2xgqvglba.html

esac
来源：http://www.52xcode.cn/Article/details/gt2oindwsvf.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2jsuczmug.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2uxjwcpbh.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2drcclops.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2zttpnfts.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2qekwjrju.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2nypdyfll.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2pnowkvbd.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2yfnlsdxf.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2wmhzgomw.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2njnbtgcn.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2ncytksmm.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2zruskfpm.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2bjtdvojj.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2gutjprmf.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2czgjqkbo.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2xxpqaivt.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2gefzdjvq.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2njzrjbrc.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2pbhfalfz.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2lgqpjjby.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2qczheaxt.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2kysapvbn.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2ypyvtuld.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2jsjwbpsb.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2chjndelq.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2vjunlqls.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2axestkyq.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2vnbeiwmv.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2vfixcweq.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2hjvghlhf.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2ikrlduds.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2dceaejvm.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2wezdchow.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2fukjvntk.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2gnizmtmb.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2rkhkjmrs.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2bmtzzbeq.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2ssflantc.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2nfcnettr.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wkjyeeob.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2gxkfjmem.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2nyxyzjiw.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2aybjoedz.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2nminhzan.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2deefldxr.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2qbcwcjqp.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2ynbapkyi.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2qkbcavro.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2jfcijhmi.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2xreltxey.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2tbpfpbzo.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2llmltvyy.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2flmalubr.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2qzueqibe.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2obqosoxt.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2rqojztvj.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2urfwzajy.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2ytqyuptc.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2kefzoofd.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2hfrzpdcr.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2ftzepmiz.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vttwkjos.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2adfuvpql.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2pkgxjdag.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2mxacxrye.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2ixhmdmsi.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2fyuxkgfs.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2eljiuaby.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2izxbsbzq.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2ictofenp.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2sewmyyrx.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2kawegvdx.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2brbulhvf.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2tkdjcyff.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2hyxewkfe.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2zqumpkva.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2ciafyoow.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2bbtfcarr.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2magkphsk.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2oaunurhe.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2mfbjvkrf.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2pxuwjcdq.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2zixrpxhi.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2qyjgacyt.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2ngaqfwyk.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2jjbukoff.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2ofvzarov.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2aczmirdp.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2sbpelcsm.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2pfdihaqp.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2izgnjlew.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2zohvvcob.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2gjxtgbeb.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2wykawzsh.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2sobzxhvu.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2dsoiwksn.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2aojfteml.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2giqwjias.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2omhyztij.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2ypujjfvv.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2wehbqqfx.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2siusebaw.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2chrzkehx.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2fuwsidvf.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2qzgrlpmm.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2levsddiy.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2iupkxupi.html


<!-- 参考信息 -->