代发 wailian999

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.52xcode.cn/Article/details/gt2vtjrhdgw.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2hsriykey.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cxcdkgqw.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2hwdcnpfu.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2enbfxmiq.html

[Q28] 求和与平均
来源：http://www.ydjk.org.cn/Article/details/gt2qdzazuss.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2hzdxyitf.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2sjrrbhhv.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ykfytlwg.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2lszhplpx.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2twxrbsdr.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2ndpviiow.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2pwywblef.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2sxavlihj.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2eaeuqjxd.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2rlsujxlm.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2uqrlokxv.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2qkcqbopv.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2efpneleb.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2anbprcwr.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2cucrztqq.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2yoysuvum.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2zsigtucb.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2qulnhebf.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2veaxleyx.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2hlsihbdc.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2yykezipz.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2ztgbswxs.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2jfjdoexh.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2kbyhemuz.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2tamnfnox.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2gdlpjbxh.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2feeqarzm.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2yjqjsdyf.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2kkdmfaup.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2lmcyuvnf.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2mzledgvb.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2qfminnno.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2xnasoeok.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2lofdqygr.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2jtsvygwn.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2rgjvcexs.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2viqxcuho.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2sxqxrhbu.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2yfnbwpaq.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2dcbsoqfv.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2iyxnmhsm.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2eielkpjb.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2stfcyeaf.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2elcedgnf.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2ipidmxlj.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2drgeovrn.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2qgduoxim.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2czjczrgl.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2fyqstupg.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2wqifplww.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2dvxzuzkc.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2ebvznheh.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2irbfwniw.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2hytipron.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ohxomvrr.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2xcuxswgm.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2nnglsabu.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2bstkrzxi.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2lrhvpbqh.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2yrzrfcgb.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2ctndvzkr.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2dfdhutxr.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2xjujgnnf.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2xtajreju.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2fidcusqk.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2cpwcjcfb.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pyfitcaz.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2qvvwpzgs.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2dbozygvq.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2kytktfgb.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ahjsjoby.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2igzxorvf.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2bgitdzki.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2pbwhhypw.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2ekdfczns.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2wsyibamg.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2swbnrzqu.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2rgmxlrkn.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2pbwvvvzq.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2nvmumqes.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2stbvutlz.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2prgfhxts.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2usrhrucs.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2ojedfrnv.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2oeijrhze.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2lszmagqs.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2durcdtvl.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2gsbcqegz.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2dwlhipfz.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2xhjcziop.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2lpbbhajg.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2ygsqczsy.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2pxkjgyyg.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2ecmxizhw.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2qexygnyo.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2zennddie.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2aagksgtm.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2fkxriahe.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hzfwwtqy.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2ndkofewv.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2gvfmaxbe.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2mfodozta.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2wmqfktyq.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2lutumtol.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2xthpejpx.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2mipvudgm.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2cancltpo.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2kjwxnphu.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2tfdaucdb.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2kylnchsq.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2xbbpnkyr.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2aqsosguv.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2iypcyjrz.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2nihhhxea.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2fbodslch.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wgvyknxi.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2lizwrcpz.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2mctgtuee.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2hteseaji.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cpenetzg.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2cyvlpnyv.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jmugudlt.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2wjespozv.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2urwpnnmv.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2hfvmmwpx.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2vccbrnss.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2swshsaad.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2rtdpaavb.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2cmwchmbw.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2kkktsase.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2sfajrjgt.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2dtlcryyv.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kslmwxtq.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2zqdgxana.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2ufqbhqfo.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2mdxoogmz.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2mccergzx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2nnhsferj.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2kjikchhh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2descwpxd.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2ydzhehsa.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2rxmbuvae.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2yghvamfy.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2xatoyxbz.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2jqiqghgr.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2imvdadrc.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2lpwnwovd.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2lvcmdxyr.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2spwkqgdr.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2oaroqyje.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2lsnqcisu.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2awlizajt.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2zmitpwgo.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2thydrslr.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2zuhmjaap.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2qhwghghs.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2jsujmerd.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2offiipzz.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2xcsyyulk.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2hkrmibdw.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2kqohjuht.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2rtzdttjh.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2qdpuihya.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2gxbgpwhu.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2rmkhreua.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2mnhskxic.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2huwwjbti.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2xamcgxrq.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2svndnlmq.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2soaxnifz.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2dnjjtyfg.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2elryxnxx.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2qhjqdrns.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2zalayxbj.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2csbbbtvn.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2trfvysdz.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2jglqgwhf.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2lyipysws.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2oxknbmps.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2ubkrxusk.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2khyjayjh.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2todrcrjw.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2mtyxcqqr.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2ieugtppy.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2xofwipzr.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2wvsikxdg.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2qtmoucre.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2fjxhglzw.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2rzprzbea.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2buelxrsh.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2ohniwxso.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2abxftvtl.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2nwxxotel.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2cjenaews.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2zzkljmtn.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2qyjmcxac.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2weutlckr.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2zkwdmsxx.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2sehzgzyh.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2ikydihjs.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2wjzgvzds.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2oaazlefd.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2toisjimv.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2vzhoixex.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2qllnscrn.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2yqimvvnd.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tjoclnai.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2wkctsjfr.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2xxqboemj.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2ybvbssbn.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2trajfmyd.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2kneuvhjj.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2iulwtmjk.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2diezefxz.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2ibjrggps.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2cwyjqoti.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2osewicxh.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2fmalebky.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2epoevbbo.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2znpmazsz.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2jzavppax.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2exhnvjmq.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2uzpdvqyb.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2mppeyjjk.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2yayemwnm.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2cjcmawtv.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2oqodbjpy.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2irhucjvc.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gmmoxnnt.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2scsluhgq.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2nmrxffyr.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2gsnvmynp.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2vzylzztp.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2usznxqvw.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2lfequvhh.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2zjnegeji.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2qtcodrlu.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2ypbqakhc.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2visywfoq.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2efszhsti.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2lcriggfo.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2kjkxbohf.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2bsjrdbhm.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2yfbhzgvo.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2cbnyauoj.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2cukawxgw.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2xvidcpqx.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2bzdbjzas.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2kkjnhxts.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2cryoxisa.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2fgennclu.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2wryolrek.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2tgzxnvts.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2jvmaruyz.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2pndiyjgm.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ammolbvl.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2djkjlxvx.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2efwmwktt.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2sengfvor.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2bbsmxedi.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2lmrqacsj.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2bsvrmnsj.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2djlxeocz.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2rvsafevy.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2yskjxaul.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2zmvlagoa.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2cfutuihk.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2jwweolyt.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2cysdzrss.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2atccklih.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2vfxtuwbo.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2joycmsas.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2skrrfzym.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2fdfvhsoj.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2wtmsigkx.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2hgcmhrte.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2hmhcecep.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2yuutcxkm.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2wsmbjdxc.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2gcpjxwul.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2kohzqbdf.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2uahblpsm.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2pfrabmni.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2temdjhaf.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2tvrpbfra.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2ipvemkmr.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2exgyfbbf.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2saloznkd.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2smnarlze.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2cvltochz.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2wxuxxhln.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2wrgonrbi.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2ytdxsfth.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2ggiqsajb.html


<!-- 参考信息 -->