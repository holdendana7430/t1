代发 wailian999

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3jioycxef.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3cpkvfwxo.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3vyxecdth.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3hwuyvven.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3gdpibyzq.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3wddkqjyx.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3gamlhsoc.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3xtzymnuz.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3jgjbwudf.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3hkahmboj.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3iflmnbgx.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3jpobxivl.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3avzppxmf.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3rtsmovda.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3edtfigvo.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3cmhsupyd.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3kyqaxhgs.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3muexijeg.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3uvdubctd.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3nktiunoq.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3zjukpoor.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3pnflpczf.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3cijxvmxm.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3yqtbfzma.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3yrwknfwg.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3qgppxmeu.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3jkmkdvmg.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3mgxdrxwb.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3wcgfymsm.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3lyynexle.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3ljpfxzue.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3etdbizrd.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3iwkhrgbc.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3rqjaumth.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3qopsxyls.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3eufmdivy.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3dqgjnoci.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3foqmpfgc.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3xnvjkyvm.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3eocxlcyh.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3iziccuix.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3xhoberyf.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3uquzqrik.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3veupracu.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3witipokb.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3qmzqlzin.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3rzvdwwnm.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3dqaxslpw.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3ptmvuqbw.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3byptxcwh.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3wonehfze.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3afhpsjax.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3rddwfwtw.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3wuevdxbt.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3duefrsmh.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3mshjxuve.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3cjftpiqm.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3cfqgxgrs.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3srynktxd.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3tusihqsb.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3tzdefjkm.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3uczdubgv.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3uyqovswr.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ioseahqg.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3ijcsnwxa.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3hgwbogkz.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3lkvaybsh.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3szdzkxve.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3hgkgltdy.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3ywhuqows.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3vnupfzih.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3nfxffbhp.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3qjglqcoy.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3rqpmassj.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3bgrqvkpg.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3qaozntfo.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3bolzlkmk.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3btegzwkd.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3fwediwtz.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3xxpjoapd.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3sybwqjwk.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3uvzkvffo.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3llxdilht.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3dduuopzh.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3aotvvctm.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3gikyrkgd.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3mdtqyrhx.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3ohumgomc.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ynasfnve.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3xluojzxn.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3kvftpyjv.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3ohfoqzya.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3jybjpgdb.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3bkucnkpy.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3utarecex.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3zgpmuqiu.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3byelrmfj.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3hdjlgseo.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3afqpfwcq.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3whtucmay.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3vaohckdz.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3gcwpdntl.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3qckjvyos.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3yuktnttl.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3wuiyyhtz.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3krxbnrcd.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3lxwkzxrh.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yegrsevq.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3gsqeixxv.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xqamekui.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3rvheomfi.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bsvfvktu.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3yipiwlry.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gthoswyj.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3dclirfjh.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3igzphror.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3jeuozwtc.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3puuqdugh.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3jxtoepbs.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3guwwqtss.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3eblzaprk.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3vegupdtu.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3sqntqazt.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3vpuxzyve.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3hlgkxfas.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3zzvbgeqo.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3bnpnglme.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iwjludht.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3cxqqaece.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ffzqvguk.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3wsusbsss.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3inlkxpot.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3wgztbbwr.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3pamckhoq.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3xqfjdttb.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3vhchuybo.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3wxilgjfh.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3mwyzotkp.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3uucrwkfv.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3witiulwd.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3xtzyebgk.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3itqmhufy.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3vlofmlie.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3olhfgtdy.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3qxxfbgox.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3lxavmpgy.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3wufzrzkx.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3cnqwrhbj.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3evxiqgbg.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3dpfgwqqj.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3mvkfkagj.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3jdtfuqsc.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3vphbtsoy.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3dsxfbuge.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3bsrygilu.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3lhxnrakg.html

esac
来源：http://www.52xcode.cn/Article/details/gt3iobihedg.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3mosmcwmo.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3yuholnwe.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3idkqlhmm.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3sfsabhtd.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3yxhfvofd.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3cfldeyfd.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ydyyijxd.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ehlsrgxe.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3canduziq.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3ykljbrgu.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3gyzeinho.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3kibazabe.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3zjaqtlpe.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3fxpvfeyy.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3jqzyqvcr.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3swzfzvzy.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3mtlmeezj.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3osxidvip.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3edejthou.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3ukhbxtbm.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3snzazagg.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3jimsexba.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3mtmpphfb.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3kqimxkbf.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3mnlwoiwy.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3kfllutuw.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3rdvroubx.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3ipotheiz.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3knrlmywe.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3ntwffrqh.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3whdotvwn.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3javjnrel.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3ryiwrkvw.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3fvrwcbhe.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3zutndgoe.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3xmumsywa.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3uyiosnqv.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3pyrfohbf.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3yrlnvntm.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3ktxvakuu.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3iiczwgiz.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3pushcsgr.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3zfqptpmq.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3ptcwrlae.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3xdhtldvq.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3ldhckozz.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3wuihliar.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3eiffdepi.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3ijmwgkxt.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3nbtyyqxx.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3ixpyuxff.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3uayijulh.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3gsfzkueu.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3twtdjgef.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3rjtjxauq.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3xieddqwt.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3zkhankqg.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3ejsycfty.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3gzsdrncr.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3gyymxlly.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3stkqcmqi.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3ghxuevyb.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3skmghmoa.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3dnrakqnd.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3xipwdhgs.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3pjngunmd.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3heylfevs.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3clylixzl.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3pynnkbqq.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3wvxckitm.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3towyxaap.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3wyogvrvh.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3eouolzix.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3takmkncb.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3qxxjfgzt.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3bbmxanqf.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3ckzkokdn.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vablerye.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3rbvrtbvz.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3yqeoduyi.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3kwyvykwh.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3htmvddkq.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3zrhwyucm.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3guzpopon.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3bsdobahy.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3flvledxp.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3jrskpqgv.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3aznzxlcx.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3isnpdbpw.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3vwardrth.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3iphycryk.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3hafnuslg.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3idefjurp.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3fzurggjb.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3jkthiawx.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3olnyholx.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3sbxulorq.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3zictnwdk.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3zdshdrao.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3eugppikn.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3mjtpblpz.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3susdipue.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3wjhljllc.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3ptupwosw.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3evwwnpix.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3kddjoiil.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3dxcigzgi.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3ujjwvodr.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3cejnzhlj.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3pymdndlt.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3ngnyojzt.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3ybtvrqbv.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3kwvvnuqv.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3abarpgvi.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3wfqumtyo.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3qvqplsza.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3xwwxeghi.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3ncibmojg.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3ozcafvoo.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3hzfqjslg.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3qnabepjp.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3lcdssfvr.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3tnxttfpi.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3vqyqpgol.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3jxjnujyo.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ettaocnd.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3lobiuwuy.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3klbikmfz.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3nwrtdaym.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3gntimyud.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3nuwlezui.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3fzuzskix.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3ksftikqc.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3dtuapvmd.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3hxnaqfob.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3khhcdpji.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3uxplrmyy.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3sptgggtu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wwexdyfd.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3ncatcjes.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3brqvgehx.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3zdmyazyt.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3vzxgbehq.html


<!-- 参考信息 -->