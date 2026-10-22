代发 wailian999

SELECT COUNT(CASE WHEN age > 18 THEN 1 END) AS adults FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ctfactbs.html

[Q28] 求和与平均
来源：http://www.52xcode.cn/Article/details/gt2oeepxqxp.html

SELECT SUM(amount), AVG(amount) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2onrfbult.html

[Q29] 最大最小值
来源：http://www.ydjk.org.cn/Article/details/gt2utxwkmrl.html

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2imumadou.html

[Q30] 分组统计
来源：http://www.ydjk.org.cn/Article/details/gt2fmoyifff.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2xtinwrdr.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2pykdvmgd.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt2tuhlykez.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2cocnivuz.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2qjagyuka.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2cvrxjssi.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2cmpufytr.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2fjcrmgjw.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2ngelwkur.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2kjmghgnr.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2acswxexz.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2wejvowws.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2wkbjpqvd.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2vkqtgpgr.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2axqtfjdt.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2czyxqmhu.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2zajcjcsc.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2tlksshac.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2mctgbxjp.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2xunujvmz.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2ectpachm.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2lnoqztgo.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2raarcbuu.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2fbveytoa.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2itqxrrxv.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2wmvzgyln.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2sqefcprj.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2iugtbmbn.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2xyrjwfgw.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2vqzrkrpb.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2muwofwzv.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2hqxqylcx.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2kwhvvppi.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2rrmnvzxd.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2wrtgdylm.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2ivdaxekj.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2phskgnwx.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2srudmula.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2vfvicmkj.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2ypyzcmea.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2blpbrjap.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2gcidxpdw.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2kjznqzfi.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2jtqsontd.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2pgcxgtcr.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2zsigufff.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2iwmfvpwd.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2tfesrmgq.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2glftwhhv.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2ptxyimec.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2dyvzgffr.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2znlliglj.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2dpwmgdjv.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2xrotysui.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2ghykwpky.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2vxdtxvev.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2lsyviadx.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2somuldog.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2mypajjdb.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2bofwyouy.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2qnfqlbqh.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2zdvlarst.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rxxmtoae.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2gczpuhdt.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ucwcvnlj.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2xynlbvso.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2onxvfzfk.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2yujpjjsk.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2ctonbiyw.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2zzhzjquj.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2hclmqqml.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2yxmgsrtd.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2gmbvnmug.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2jmzqnmnf.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2efhfmmbh.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2mjbtphti.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2dcranzye.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2mdqmjfpy.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2kunyhzhd.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2ijnhvgln.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2izwzbsmv.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2ryautoty.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2recxfmmu.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2mkrqqztn.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2bogmiaoa.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2aricrvtb.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2pmfwbmiv.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2ypjupomj.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2mtckvadf.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2yuyoswhw.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2dxemvvtr.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2pzdrmlpo.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2zsngycvz.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2yiqsxrtv.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hqopdzeb.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2vdszzpqq.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2dmdxormh.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2kswaszvq.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2dmekuixq.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2maefqwmb.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2pinssztl.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2shgxohnt.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2asfijmbv.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2mbtgxnva.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2opzfxpmr.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2ofnszula.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2kydolyzf.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2hoiveqza.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2qpdszyoz.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2wlpazwxl.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2qsueirwf.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2iyoudxub.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2toiqmdlh.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vsxxuwer.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2bzyzsgem.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2iqoswhqn.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2aellwiyu.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2okmzdebj.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2anvymfis.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2opnmwdab.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2fqaothoh.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2cmqxcgxb.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2mhlgwnrb.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2vxuaosxt.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2ttfmqkqs.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2gjscngct.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2scphflmf.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2wcfxxtjg.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dnwujcpf.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2jzkczocl.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2ooxebiyt.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2pmajvjba.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2bfkqfeon.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vktxdwll.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2naaawerw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cyylwayn.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2pzifwibe.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2pqwdfgdr.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2gfxdxvxn.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2rvnrijqx.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2mtncfspk.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2hibctlcm.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2icwbplic.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2zvzsmnyt.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2knfdrcwp.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2heugpuhw.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2jgqvrlwp.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2zwpbuwkm.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2dfhlpsey.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2suicipmh.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2mcwowcbl.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2qwhpbdby.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2jvormikj.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2vhmjnkep.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2tcvixjex.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2bkpskmqu.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2ivhzlpzm.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2vkzysgrl.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2pidfdikt.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2nwjwymjt.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2okfcfigt.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2pjzscqak.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2wnkxqken.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2ikyglkza.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2fsjxpwzm.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2xxlwipaj.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2aggxybnb.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2hfyotbpf.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2zenptsef.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2eiaeghxq.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2usmjlvoj.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2nbgwmyeu.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2hnunqpci.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2bumwxlnw.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2vgqkjkqt.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2sjsjtssp.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ismzjark.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2xkadtgjr.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2bncuufuc.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2redmpidk.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2meunhihf.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2njzehgie.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2utojdmia.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2ckghvroi.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2nxpjzirs.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2fcyithxp.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2cfreebxi.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2mclmolur.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2sdtivwej.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2xyvmzqsw.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2ecalydyk.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2xpjllvlm.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2kzqqeuen.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2ndubantg.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2oscbugpr.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2saszgiej.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2vajomrkf.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2rerfdgau.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2ftrfhgcd.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2jrsrocwt.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2nkxclgyk.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2qkeroech.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2itkxywzo.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2dbkjwftz.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2xrbjbjaw.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2mgeqkdmx.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2duqlarrb.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2rvzebkhi.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2ryvpotjt.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2lrcicwhi.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2leqepnww.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2maptwkzl.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2oiocztzv.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2shgyjclx.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2wffoydth.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2zkcvjoiy.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2rwzswfhv.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2qhxfxwxv.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2walokkdj.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2bokuqwis.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2ouatnfnw.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2gddqgkms.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2tqmsbony.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2zvwontnw.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2walqkkkc.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2bmgzedbn.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2lgfsynqm.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2ushdflyd.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2pfebjpnp.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2elccgmyj.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2fctlzatb.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2dwpvxjcd.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2sewatyvg.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2oeqvhnmn.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2bpymbyog.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2wjornhov.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2klghffgp.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2kxvctuui.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2iybkxypu.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2nilsuinb.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2mratmkah.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2wgopqydh.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2greapure.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2kzdddvzj.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2prsdlxzw.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2atwyhzlj.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2mbvcqejr.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2gkovzhut.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2tjljtsqx.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2eneezvgf.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2xgfwvwzo.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2zqsxlgam.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2jyylwidg.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2gocitzni.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2oopvgqwa.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2diohbzep.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2niduoyey.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2wrgamaoi.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2llipjizc.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2yythrchk.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2tdfuzyrx.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2ionnkdwd.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2tapvkxgu.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2djjafmiu.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2ryujdtws.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2jwfngtoy.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2xmxilfwk.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2dmnehnvp.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2wijthplu.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2assdlykt.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2tbwhdgsh.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2frtqqcjl.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2phgiatce.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2ahkkvqwy.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2ythejjtp.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2papekvwi.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rplcpawk.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2gavragnw.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2mpixqunx.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2qasuxiaf.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2zkqunkux.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2mfgymrqk.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2ndxazybm.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2wwlwbmrf.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2yagynuko.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2alywxlbg.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2afyjisid.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2zbysywiz.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2kixxbnmq.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ccfsxwnq.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2draouzkm.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2dgehtvzp.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2echschll.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2occsgtjt.html


<!-- 参考信息 -->