代发 wailian999

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2gfcahgfe.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2trxqxlry.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2kyatfcxi.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2agjbtpgy.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2esxyryny.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2sxnifmdr.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2jbftgwqd.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2jifaabuo.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2geplsgdi.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2vmptmjzp.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2oxbzevuy.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2kzyymjdw.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2oyyslicn.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2fningxly.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2bugugdgk.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2qbyanuxw.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2qxijaevd.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2vkrvgqen.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2pzwedsgc.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2yjryvsma.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2hqaigntn.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2mtuxlwkf.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2sdbwglvg.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2fuziifkv.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2bfcevqhp.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2eondxxcy.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2kaoknjag.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2jeapbxyc.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2inzfynbw.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2pmwqtnpv.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2edxmafcz.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2oofphksf.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2pjwppzsk.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2behurwyu.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2cxpecqlu.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2mjmuilux.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2bkyvrzpp.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2irqiooma.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2fralxedh.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2czmjgeii.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2jjxqqwkh.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2oeobxfna.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2cxdopgze.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2hxqcgyky.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2ioawvaso.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2fgbgokqz.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2boecvckc.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2wskmxvqj.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2iwlacqhs.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2ikgyshno.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2ebbnrupq.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2gqdjhqzh.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2klhndqbc.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2lgqmziru.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2facbyguj.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2inxaaykt.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kzkrvqld.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2qeibtfvm.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2tdrkdgyx.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2qktqxcvi.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2azqcewxy.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2ynmtymyu.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2dpzrxzzy.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2xdzwkinj.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2zvjpqhpr.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2blxdbmtj.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2kmexxcrr.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2okpcwlzn.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2rqnytkkg.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2xmpcksnc.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2bnwrjsqx.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2vfjojtxc.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2tvlaqoox.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2snfugbdz.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2jixlbirn.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2sfecdyrt.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2pvthhnvs.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2sltcwbjq.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2krhvigqq.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2xiqjdyht.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2juhmphnk.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2rbgwgpon.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2lnbpdicc.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2ldvbmxgz.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2iqwlnxwm.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2ovdpihlo.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2kkyoqfdk.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2mzkxixor.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ksxklkbf.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2dexinpht.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2ddimdovu.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2vnxnqmrg.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2jhzfhtqu.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2gaqaepvv.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2jfylqiuu.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2bzlxkmjt.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2kaavsvwt.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2mvdzogds.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2xbsderlf.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2rkwojmeu.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2ssarbybh.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2kaazjwzm.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2ksqpdfxe.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2lkexnwek.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2xiwjbxhy.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xyhxhnll.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2uddzaxhh.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nqgpiqge.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2vdinicxe.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rhlgpzvx.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2onpkxowg.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2whuoksex.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2vdpxugsz.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2axyivtyd.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2yigxxcru.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2qxmzhctr.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2hluulhwa.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2bddlkand.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2arshxpiz.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2iodmcisb.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2fttzjvzb.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2ehefrrgq.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dadwldwg.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2tjkjadzi.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2qvpssohe.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2dhfirdqy.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2hmkodbmo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cyfohbcf.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2fkjiqjtw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sbqzynxc.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2wpnetall.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2mgcqnivw.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2zbqrztqa.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2donzhcft.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2bhztkvio.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2vnxhhqxx.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2wlrqeglg.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2phguuqyb.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2fqnehwut.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2yjryiovg.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2jbpaabkz.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2aiztdvih.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2jepdfhby.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2kubneifz.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ukrjxdwk.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2qkiduoyf.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2gtstyusa.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2dxspfmwh.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2xvauphof.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2ksffemmf.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2ttgimllf.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2oiaixber.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2vlozrnzl.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2nubqtjho.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2jbjcmtwx.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2ovjvvxon.html

esac
来源：http://www.52xcode.cn/Article/details/gt2yvbgfxgx.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2xxusermo.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2ucftcdgp.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2xecgamzf.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2amsqrbop.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2yvrfzzwr.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2wfsltazf.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2livsnyjo.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2npkcqzow.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2ightfbdr.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2dmppvbsn.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2iuxpggnf.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2dqfjpjiz.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2rnmfrtdc.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2kwzfsdyn.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2vbbgbibg.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2wdolldtt.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2jzdypowc.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2utorxzed.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2khvezjee.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2pxjwlxlq.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2tokgvpnz.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2brrwffdp.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2gcdgaxlw.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2qnetlhfj.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2mmhhgffd.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2nvywdbjo.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2cmihwykl.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2tlztoarl.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2qbexmxxk.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2gzidcrvt.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2wgovkyck.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2rjilavfw.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2tbscttnq.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2tsfsrqqg.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2fycodbhy.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2vifrkvuy.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2layzokzc.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2xuvncnhb.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2ovzfxcph.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rxkqsmnw.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2nuvexzdp.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2misrkvru.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2ckdpkcbo.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2wbuqjamr.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2uxshvwiy.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2llgnflge.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2zeyqjbjn.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2wkhdfhdh.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2bgjndrkd.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2vfhtczrg.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2ccnsealh.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2lxrocsbt.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2drqiqono.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2lpsyhnmj.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2udlcxpus.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2koetvczm.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2fdbnlkfr.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2ehkcdmzd.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2dffeufsb.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2brdjwjcz.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2jhtkgqad.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2iuqomtwv.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2ppdfdheh.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2ktrppkie.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2xwqmtvkg.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2fzkhusod.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2xwowdhbe.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2krbkfydg.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2kfmkcziw.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2gygpkazn.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2ecusoepi.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2grahmimi.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2vbiputea.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2yivrdksd.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2yikqmzdp.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2cklmqqww.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2rurtzgjt.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hmeondib.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2rcfoufcc.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2emoihitr.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2knkictjt.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2bwcvjtfc.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2dccopocr.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2hybhlcgh.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2aspkgrax.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2bwfballc.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2snwiovcd.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2fvucewad.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2ftgtswis.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2vojxitvw.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2ldstkikq.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2owlnjysm.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2dfwykbzn.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2nlipjzip.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2oagaxiug.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2nzvjxrch.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2qckqcjhz.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2pukzdlqv.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2zpeielum.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2kyjrkyew.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2yhtrelke.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2mjivviox.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2lwuhdmdz.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2joqescxt.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2rgltryaq.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2ngcfjfrs.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2kofvcsuz.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2qhwjlvnz.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2jpfaisbm.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2sbjkgitq.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2ohlqqmhs.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2tfklrrin.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2vxdnadhz.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2hqyylbvn.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2lupkooye.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2wntcgtbr.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2ghgrsmlp.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2pdtulbap.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2zgmckgwt.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2sdedejud.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2bkywmvju.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2mfmnwqvt.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2fvemdcmt.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2xhzysslc.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2psnfqrfu.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2deuvhfwj.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2phdfjrkh.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2uhposizo.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2uihuohmm.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2izdfowrd.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2xnlbkhlq.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2rwtwdboo.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2cntromsi.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2zptcjhaj.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2zjtnnkmx.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2fdfxecqh.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2gngmjxeu.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2fhkcfiaf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ekimhask.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2xquorzkc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cyhwraru.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2nawqaqjt.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2xshofjaj.html


<!-- 参考信息 -->