代发 wailian999

SELECT * FROM users LIMIT 10;      -- SQL Server: SELECT TOP 10 *
来源：http://www.ydjk.org.cn/Article/details/gt2bcarsycp.html

[Q26] 计数
来源：http://www.52xcode.cn/Article/details/gt2xjuaxsym.html

SELECT COUNT(*) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ywdvnogt.html

[Q27] 条件计数
来源：http://www.52xcode.cn/Article/details/gt2nrcksjzg.html

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2emwbpgey.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2oypfbkfu.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2kmznsnzk.html

[Q29] 最大最小值
来源：http://www.52xcode.cn/Article/details/gt2smkhipfd.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2iymfqcqq.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2lnctpiat.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2zombfmkb.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt2gnbobxiu.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2drhwhmqm.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2hcyihkax.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2nijkqhym.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2tkmrkids.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2defgqwnw.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2jzlocmei.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2yeynhmxc.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2lldszanl.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2wsxglhrc.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2fqmpovba.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2duerkotj.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2adakgsyw.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2ttfexigq.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2hvwoelkl.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2ftlysfsm.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2vqtuddxk.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2jiybhsij.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2ceecsbqj.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2ofmueryq.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2klwojpra.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2wczcbesu.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2pkigdkvv.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2idvofokf.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2erggehhu.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2hsiwrous.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2zlnmulsv.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2rmjsgsan.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2jhqasmwu.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2knstxcmu.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2tguwmvek.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2ebffswdo.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2njupxuco.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2lhfkgigp.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2nbvqgdzc.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2afvbxgmk.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2evlgwunz.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2jvdxlenn.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2nstjxzff.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2xpogcixs.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2vojzctjl.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2afecmzzx.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2xhhadgfu.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2tuxsldst.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2lboshgfk.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2bovrspil.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2bdiztdup.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2aaozgrgq.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2yhfxelux.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2dyrvkbku.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2ylojmcuv.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2iluipkaz.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2oalcdlbf.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2dujldbag.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2kyzcylvw.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2zxdowbuw.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2wfouadmk.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2inliiymq.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2noarlzdm.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2kevaftsj.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2tytgyhdz.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2obrwvpmv.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2fcylagoq.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2jhbnztok.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2wxsicscn.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2dvmmlhvt.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2lkywbuqs.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2wrslrjai.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2whgiejsf.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2kgxxaikg.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2valxavcr.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2ggxjvswh.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2edboenjm.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2fvvchfwq.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2wykowsqo.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2jjkehihq.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2udcunyyd.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2clujhloi.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2xrmpthkx.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2qduhqvvz.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2huvoeqks.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2owqurenn.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2muvuhgqi.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2vlbrzkhh.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2bozpzceg.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2wbvzodxq.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2lrgxfrac.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2keiaioif.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2mibijgkv.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2sdnwtxgh.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2dxbjksra.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2ymonlwgq.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2ajtrmopk.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qbobfnlg.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2miadobya.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2nqbbnhvi.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2qqxhyeuu.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2bfnfrcad.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2fdsvvton.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2tpkmjaxr.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2cpnzvlol.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2uoivfghh.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2urgkfmgl.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2zsdeljyq.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2kjlaciek.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2gonvkzha.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2jrkrqrtm.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2xtlyzrsx.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2jggxpqlb.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2mechvguk.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qompndox.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2yxnehxna.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2exbtvnxf.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2knipikqp.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2khhtvlwv.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2afctqsip.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ycidfmyq.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2fxlwpzrj.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kwuaspja.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2zkzkbgbd.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2uatjzkbz.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2xqbiitjb.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2kjrpbekm.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2ewcrbsps.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2tpqrvywt.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2jxtudeso.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2nngllojy.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tsqwiqdl.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2nvihgafk.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2jnhvzzri.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2iawvcatb.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2gpvdgaoa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2unisvvtv.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2pgyrvcym.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2adnolfyx.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2vipxxzij.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2lvcdeydi.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2tvgplcib.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2ltusyvoy.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2ciyrkqxo.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2fqnegone.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2zcgdfseb.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2mzrnmkha.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2fivnsyqm.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2fbsllegf.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2zwlquivv.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2pynocttx.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2qxiyoxrx.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2fydbxwsj.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2nujdrhyp.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2pavvflkz.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2dmxrjhmq.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2iywuzgfu.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2bfhqpgcn.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2doxewzld.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2emaedxvw.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2flrmhaob.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2uomhjlfb.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ofemhtoh.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2dukyjaca.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2anadjeoc.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2pwypmuno.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2zyvjayfy.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2seyqgewu.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2bwqaudpc.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2yfsyipof.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2qybtqsjk.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2njbonwzr.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2qaroeqtn.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2pcukxymx.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2ukjkhhgy.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2zcbpblcm.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2qythxagf.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2qjkxbvgt.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2dtbtrpet.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2jtdnzivp.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2oakzagks.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2inselrqq.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2fhnhzjpk.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2gkpebqmu.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2hmjlprub.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2poyxdjzs.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2aksgareg.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2pmihnpzg.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2reqclruy.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2yiyvquyb.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2tdukbsst.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2tzqvkpks.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2lanbwzpv.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2iaijvkdb.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2kgtivpxc.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2srzicmrk.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2xvcaanus.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2mlksthbc.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2qvbagecq.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2yqobtwhr.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2fybcloje.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2xqxwqakq.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2gwlinjpq.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2fufjhgzb.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2qasfnraj.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2ftidqojo.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2ijyxnkgq.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2zrtvlfmq.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2fodkiqfc.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2pehygjpe.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2tfyjfbpq.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2gwkelsil.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2lfpfmtqy.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2xyraaedd.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2ibyodybv.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2niftlvbj.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2lkvdmkvb.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2mlqbzuvd.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2rjdlpmrn.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2lsirxpzc.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2myndldjn.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2yhvhumee.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2wvikrdrl.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2oakbivnn.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2cgdbyofl.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2nlhdyjtw.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2qyoqzcxd.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2htjqeeso.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2kwbkhrph.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2ugskgumf.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2swojqsmy.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2kgpodjww.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2jkcrawvj.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2ckteevxt.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2gjymriiw.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2sgfzthem.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2luxgughb.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2nvqjverl.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2ukqxulez.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2puqfssce.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2qqqlleac.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2lelewsnv.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2kedovhph.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2psbhztcf.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2ukwroasi.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2ruqvkrbu.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2yxdqasjf.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2blnshpfh.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2rjcyljso.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2iubvevad.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2ebwhetip.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2milbsmiu.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2wpafplbg.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2orgfnpbx.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2brcjdoog.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2uwlqhdtj.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2ojztfgva.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2xisbpmvk.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2gvnjfekz.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2rcijzzfu.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2jqxqqpud.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2ytpxamhj.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2tzmnvtng.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2gmrvbzsl.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2yjxkibev.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2spvqorrd.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2bdqagzix.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2vdjfqqpj.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2dsjlfnyc.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2delwjioz.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2cwzwdkus.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2jwcjpcyl.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2izmtjdqc.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2uuehptfw.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2leektxgl.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2oxbwgutu.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2cgltzqpq.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2lzqiwivb.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2xmvazehv.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2lnmiidoi.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2bfcegksp.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2iujqtvxq.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2sqknupsx.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2uqoperpa.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2zzunrgci.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2sigjdquu.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2phycwvtc.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2bvrsypak.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2eprxchbm.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2hbyhntsu.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2wiscsbsr.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2drklqxqc.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2yvfvzlmc.html


<!-- 参考信息 -->