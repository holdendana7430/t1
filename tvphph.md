代发 wailian999

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2atnmideh.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2mtxvhsne.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt2reqaaaxq.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2eciurjnd.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2ofijcnva.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2fgqadyaz.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2avnzzxel.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2bggzjgtz.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2rxpymljd.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2osvoxcjr.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2fogxnkds.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2cbvybuvg.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2kygxljqd.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2vzxpqneu.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2kuufbsft.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2lecjoqkn.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2agqocaqx.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2briyyqhj.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2rdnwveuh.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2bodkcbst.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2zgwxjikc.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2whuuiell.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2xicsbbjy.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2gosxlxbv.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2gdbwjeew.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2jhbrfnpg.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2jvnurtet.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2hxnqqdmy.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2rnrcohfh.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2jgxuqbwm.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2nhphiynu.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2lanbyzxg.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2iewnlodw.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2dqiwpbgg.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2hpapczvw.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2dkzcflhh.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2akddgmqv.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2waavqfbs.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2ousjlyek.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2lohzmyjl.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2uwqpgpta.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2rmpgyelb.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2wttxcmcy.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2cxnimrtj.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2vwjigwru.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2oujoefpa.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2iplpnpux.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2yxxozdin.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2xfawtjss.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2vriewjks.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2qiiifqir.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2tammovtc.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2ldcmappa.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2xrlwefus.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2bvqwshei.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2iubtezwz.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dhamcyvy.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2kjmqfmsh.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2mzwjuhip.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2fvpsuqdm.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2obkyrvlj.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2lcxigfuu.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2uegsmpbd.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2gfslehvv.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2dxlpoduy.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2vbvxodlv.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2fjjfxprc.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2ywgpsgzz.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2oxfadmje.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2yoihmtfv.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2fczvvjcb.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2umdbswdq.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2ivztplqb.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2ktekzpza.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2muwuiazh.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2pfagyjrr.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2nerfjwsx.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2qczjfzki.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2lvogiddh.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2ehpwrdxl.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2dwvtabht.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2sscmzirj.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2vfpzbjco.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2gmgdnxfp.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2vemsglyy.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2xkjvlcyb.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2puvuoflp.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2vlcbtyvb.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vqrjrwoy.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2uyyvnbbl.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2vqdwewux.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2yvosxblk.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2grbgtjhu.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2yjyppvnk.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2wbntfibz.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2vmhebjph.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2rlrdktne.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2bcbolxyz.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2kkttzgvy.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2djdskzcr.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2pxqawrmu.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2udgkmkqj.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2vziksbng.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2wbyxbwmk.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2qixnwisu.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ibmgirui.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2swgmujdu.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2yqepfsay.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2yzryarqg.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rsxzevxr.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2emswxvwl.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ufeflofy.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2ngabqcsi.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ldkrpqgs.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2dsazorph.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2jmhaixxq.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2afoyosis.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2kmyjvgwy.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2cgjuhhwf.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2pexfqvtu.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2puktwpkz.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2scbjmorb.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rjjbmtyj.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2orjvzmuf.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2zfdpooha.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2dwwcnkbr.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2pfgeuuyy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hqeumbqw.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2qzppjqrn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gyvowcje.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2adkazrqu.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2jwwbjslb.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2yhgrwzsj.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2vsajyfue.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2eetastmu.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2mqhpxhbx.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2ydyhucod.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2yavdiewl.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2eoqbxtev.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2cjwaeovy.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2zeknznxj.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2uufsgwqf.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2auccpcqh.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2pusrqjfi.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2gibyftaw.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2lykvyndd.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2hsflnaso.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2ygknqdsk.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2bqrhftis.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ikddsrko.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2kfwetvjm.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2lwjfnhuy.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2doukkdzv.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2tigeghdc.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2xoupxqkz.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2rbhmmtmz.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2jlkxiuse.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2zvrfbzbv.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ysehfmoy.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2pdnqlafe.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2zsysjfiz.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2ejvrilkg.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2suihufcq.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2tnsgrolm.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2sgfwcxzx.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2hbmkxswy.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2kbpirmba.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2dtrbvjze.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2minqwhdn.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2axmlubaa.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2kxzpkoak.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2seiyzujz.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2zlcyzrya.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2owrmggtx.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2jpqkdmbc.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2qyzegyrf.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2kfkuccjd.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2wbgwardt.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2ahgkrvcz.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2rcfvmclp.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2xpwrzjxf.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2kyvpmkwi.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2pkmvriur.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2wfllzzlt.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2wzcdlwcd.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2bvzevlwj.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2wutjevku.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2uzyrjlye.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2zzquwboo.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2fgkuwuip.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2icleizib.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2eilsigmp.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2fnvuztam.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2vznboiei.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2cvmsxktw.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2sdfqvdkw.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ksvqqunj.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2ewefxlrz.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2zukjgcve.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2agenvnqk.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2wpzpbxmp.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2ktxirrwo.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2lwqejoaj.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2pqxwuyfx.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2gwjqfbfz.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2nmibwzsf.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2tgclzqcp.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2xpqskfwm.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2jzrxspyp.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2rkvemnvb.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2duhpzems.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2fdypgbuf.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2xpmjmnry.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2xsbebmir.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2ruymtdmz.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2vznderje.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2guvicnjd.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2vbkwfryn.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2xvajqxjt.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2inamuuiz.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2fqcivgpy.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2ryoktizp.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2tsbmrret.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2cfjmhbze.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2mdugvcxk.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2hbbshqrk.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2xxwseycr.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2adssxixd.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2nvhjfqxl.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2gxjaptvl.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2dakgqgfc.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2elhjvfgu.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2duptkwil.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2mhlusaxb.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vzivvfqd.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2pqgijtlt.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2cyksgksb.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2emervffs.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2nzjeoyie.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2tlcdvrrc.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2nkystmrt.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2prhqylzb.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rcdewzhi.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2ozquwhhv.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2dysoxslm.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2lgaelrzw.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2rfskzxde.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2mmddtkpa.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2scmtjnwz.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2oxkpxgfj.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2zbvvxbfh.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2patnzypl.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2duyjybfd.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2qgbfgzax.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2vyaqivfr.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2xejflvkf.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2korkowgf.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2hffjppvy.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2mmbslocn.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2dztowvdj.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2vthfiumx.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2trugrrup.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2lngfrnwk.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2gtcgdpou.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2zjyosnva.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2ensqnkyb.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2vfoaquau.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2jyszxzmr.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2rzekcrnt.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2jomafyla.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hjcwhwzj.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2udtmbdmo.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2xllzakxu.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2dftcucsc.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2gpujgcpi.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2hfavroen.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2svjkuakc.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2dhfnkgzh.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2cvpeghen.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2pzkkjvet.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2vzhkuomj.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2lekcsrrj.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2mwpgnxqb.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2xjdfuhjp.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2fahodxwd.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2raivbmlz.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2iajkeund.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2ltzxignk.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2buqmqkpb.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2hbxmgirb.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2yvhjubnp.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2klpufhke.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2kklanwlb.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2qkysujqo.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2xlkpmibh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zhnypqqw.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2zrtvicud.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eeqqbrfq.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2dqcpuseq.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2lfpzpfus.html


<!-- 参考信息 -->