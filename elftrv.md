代发 wailian999

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2yxqowdez.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xecmtebs.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2tmqmtdjw.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt2gystrgom.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2bbegkdli.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2zcfragbf.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2ahjlfjbl.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2qjpvereo.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2obbxlrdj.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2pxzhuozr.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2vcyselnf.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2gjmtnxhp.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2ppqnlozj.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2szahskvd.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2monizouq.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2dlorkllo.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2vykepbgf.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2kfolbmbn.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2gtucezfc.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2gwdnrsxb.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2hmnuvmig.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2pxhezqxq.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2bkiikhjr.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2rmakscge.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2xijindrn.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2iyildqnc.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2zbwjjtsc.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2qlxnixku.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2ejsbtyxj.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2axdezvzm.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2ltuivnzd.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2hzehuwai.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2vhhtjprd.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2eizfjdhb.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2gnfejnvm.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2izrqrlkb.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2aspmdqpt.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2kyuaybyb.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2zeydyzdi.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2lnlylmzd.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2czfkpswz.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2dwlyebqb.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2aesqvjtl.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2iegqivgh.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2nznuvdya.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2mhzgqjnt.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2nxqabftf.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2dssmssly.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2fnjdypai.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2ibwyvohp.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2dlucieto.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2fgorsavw.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2zcxdnaqk.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2mfdhzjmw.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2khdmiicd.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2yhbyrail.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2akfqdnxw.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2gxyimtwo.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2yxknlnkv.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2nmuwhsdv.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hiowtttj.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2xjqlexse.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2vlicrwtx.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2bflfzsxl.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ukxqbtpe.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2ridkerne.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2sdauckxp.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2crvgafur.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2uofixplc.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2qxsdigid.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2mfsganau.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2qfwzlvoz.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2edfazkks.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2hvvvklkz.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2kdoszpbs.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2fjhfsdge.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2vccbakcx.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2ugdogwrg.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2gudieowu.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2udycuqfg.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2hvpsdioo.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2oglbsfqc.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2rtuqheft.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2bsodbgsz.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2gjtwoucd.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2edyppqzk.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2njgoispw.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2dipsixvs.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2ddjwagfm.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2uuiibwdm.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2niaaewir.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2gefcbmgq.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qsvlmssk.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2kpbitshg.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2krvfchvv.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2laiqdxve.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2uedsrozy.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2azxlwfhs.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2cyqercvr.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2nwvwgwhh.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2voobtiqd.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2avmkklzd.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2arldjtjc.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2cmkvnewb.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2jygyhnni.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2focqzhue.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2mzvfqlak.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2fyibrork.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2vobyozzm.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wepiczhd.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2upjeslwb.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2iawzfiil.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2ldzywmip.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zmlpfbag.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2jsfkjutg.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nqknmxqk.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2glgtkqbt.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mlunnkjo.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2dubfwoav.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2qyahedqu.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2ylymuony.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2kjwjopge.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2loqfnkdm.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2prpqbdld.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2xveuzwve.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2tscbsdky.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gjwfgqeq.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2wymmolon.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2thasjmxl.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2nxqgbqkm.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2mzrbjrcl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eorunjhq.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2tffjqpac.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iqgmuhwp.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2xgjezydl.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2wtyygipa.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2eaxssfcc.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2xmioquld.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2usedocfl.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2fbakqctn.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2ivfuirfy.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2ziznbrxu.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2oyaogevx.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2hnmgypws.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2pzngoeig.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2bnjjljsb.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2mwpwpkto.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2tuvvqkmi.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2unmzlxug.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2psgzcztj.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2vnajfvmf.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2tmzbspfd.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2xgqtprip.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2snbrubsy.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2nkxicsgd.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2upyiswsp.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2mnlepysn.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2naruhkvd.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2hxqnouve.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2dqfjqbfr.html

esac
来源：http://www.52xcode.cn/Article/details/gt2swlnflbh.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2wpnldyad.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2wlsjpvzv.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2ojdrkods.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2nqqxwdfg.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2jtyfnefo.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2uuaoexwz.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2olzpqdyz.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2wittarwf.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2dtddtpyl.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2mtkgwwps.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2uzrlxhrc.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2tbyrfgwf.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2klbtwaav.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2oysuxisi.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2onlzlknr.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2nawexuic.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2wjwogbdt.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2fkodwnym.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2pqghjats.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2dpocnrea.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2hkuieyty.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2kigqwdxh.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2tyglkynn.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2uppooxue.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2cqqexyuq.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2ojjmfomj.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2zlsgiqbq.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2vynskvsh.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2exftflhq.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2fcpsdnzw.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2mrwyagxo.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2syupdvuu.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2okcfuoae.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2rlfudndt.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2nljqcbgf.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2kalfcrdm.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2yjnmjldm.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2uzzqsuqv.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2jnssbmvo.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2kxjpjmzy.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2szucipbr.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2sdqxhavk.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2lazxkvsa.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2ppsrnliv.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2guozsurr.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2vlddrdrp.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2tclpgida.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2hemikxmz.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2maslqxpz.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2chgwuzjt.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2cyabicxs.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2nzcguylz.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2kepvpufm.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2apkestlz.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2yiovysve.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2prhasggu.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2kktonsim.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2qvmuzyuk.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2kesbvpva.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2lnbnrdqm.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2vrnzhefe.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2irkxxusq.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2ezkgfrmt.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2oubrxyny.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2ivpisbve.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2knylyuri.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2jtqhbboc.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2ewljduwi.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2eebwhjyq.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2chnrtilm.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2fzesdpyn.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ybswkjfy.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2uppwezaf.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2faotrdwb.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2lhyywdqg.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2huzzrccg.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2onbjtngl.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2dwnnkpoj.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2bdgdiumo.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2bslpljjr.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2vnylpdye.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ilrxtxbr.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2beyeujxf.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2xpppwqzt.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2miaaicmv.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2kmdkabhz.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2yhdkjuxi.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2hmfgnjnk.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ivqyefjj.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2gbhoyihs.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2xyzctuiy.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2syimosbs.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2jmtpnzcd.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2wtnwbhkd.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2itjtlkwm.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2nlcwijgq.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2vvnqlewr.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2fuxuzycq.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2xpoxigyx.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2pcdupjpq.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2jvgpthuq.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2jdjczflj.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2lrkxjzzm.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2xoyfezaw.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2kkltmyzf.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2mbfooahx.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2ctbpoprk.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2iwzmcddl.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2owjteyhr.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2bgywiuxf.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2aoooogei.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2oqdnylsf.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2qumejdry.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gkqrtbji.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2uxqwhkib.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2mvrlgnvd.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2jwasqvsf.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2gqwshoas.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2aiqdzyst.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2tnsxabin.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2sgdbcner.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2nvmjvzak.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2kglybsvm.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2tejracxf.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2bojowjxd.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2qxuazrij.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2rkzmdddg.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2eqhsfqnk.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2abmncxjf.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2knqpuiyz.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2wbhtbbkt.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2diwvzwww.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2vaaaecdu.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2dvvscfrw.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2glkeuvzi.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2osdyjzpc.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2wvrtcwug.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2kezcupeb.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uihhtnqq.html


<!-- 参考信息 -->