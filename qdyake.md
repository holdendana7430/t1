代发 wailian999

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3xloqlwhu.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3twwcpgtp.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3aabnebmj.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3yldimrep.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3oxfhzpaj.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3avvmkypm.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3jqrxrwnb.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3ycjscqbq.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3tcgcjoki.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3kwwwdois.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3ggsbrgaf.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3pyanrkvy.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3epoghhbh.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3gxmdapzm.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3tumgtewi.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3brcobxev.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3cpshtuqf.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3cilbiwpz.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3dyrvdznd.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3geiyeptu.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3nxszednt.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3wmwjcygc.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3jjhglies.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3kfvitmpm.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3sczjvfwu.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3wxauuocb.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3dyrkrcbr.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3imwmrodi.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3ssppjwnh.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3rrrlpurs.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3xyzseisb.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3dvwnxujw.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3umrwdcib.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3hbwragoo.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3wzycqrlp.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3psyvogqy.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3sgpdouxt.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3fcdgrjgw.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3qchzudgw.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3vvmblugm.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3tpdvbmoa.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3ljcwqhei.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3rizzelxx.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3jbcnilar.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3sksjprwc.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3xdjewjpw.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3gncionjf.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3hyeekizh.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3vzacacnh.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3bibznlri.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3udhljvfd.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3mncwwmjz.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3eqixcjrk.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3ijydptjk.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3nznsdafp.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3ezwgawgx.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3vbgzjwxx.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3jgyjtjjt.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3mmayqxqw.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3tlzjnfkz.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3qowuswkp.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3gjgvfidj.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3sifcitue.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3tfbcxsea.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3euurjiuz.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3yohtlatp.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3dcpwfzok.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3yuafptcu.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3ilzcgefd.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3ypeiuicw.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3fbybkwep.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3rzopkrcb.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3yyruljme.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3glepymzw.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3fegaiuet.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3gbkdeqhm.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3xdqsqice.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3ebcxrgbq.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3wufowhno.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3yaqsvhxo.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3ydtgpoaz.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3wmwnrmxg.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3tdbvbmrj.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3lpabdetm.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nglslwlf.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3tneojldj.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3faywlokt.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3ohakedqx.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3lldjyhtj.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3abdiestq.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3odhzgkoa.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3tmbzsuwe.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3hwokszqy.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3runukbav.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3abilvbop.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3xkfaistq.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3pojusvzd.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3isignnhb.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3rwnippoi.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3gcwipqoy.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3nazopsym.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rhzevfdl.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3vebfvrbb.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qzgpddim.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3rfiiinvl.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gthnzslp.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3pneyeznc.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3nbkzpser.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3rkjubmgp.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3sudqkyou.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3vhyquwfh.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3kjxvojnp.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3vvcyjvik.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3xksddqwt.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3drvkljqe.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3bdinueyl.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3nppxgphs.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3tamhpqfp.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lbfhllte.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3rdkpemzb.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3vsxujqjk.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3pfypchtd.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3sowuoesr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tevstogf.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3ircsmmbb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xquipfom.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3eyaogkyf.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3yfzdbzvc.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3qxbvpsoh.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3gxctshja.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3dwwhcian.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3uariyyjb.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3gciswpcr.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3usuksfnn.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3ibhmmkfv.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3tputezhh.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3ggiibykj.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3tjyvqdhm.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3yppynlfi.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3ynbyepcr.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3takewscd.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3hnxjcmmc.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3scqaukhb.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3gdxwcncw.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3fcesclun.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ecnzlcay.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3bxshhbql.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3ehcwaefr.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3fmibtkap.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3uaydwssf.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3gilmzfrf.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3cnbnelxw.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3dmoutjqn.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3nhumreyy.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ddrinfxp.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3rbquehub.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3uvwwrltz.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3givnnced.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3lzwdcqic.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3tgxypcll.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3oxmndsll.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3escebdmu.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3slsaqjrm.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3mdtyltuo.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3netoscro.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3kyyurjkh.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3inzrlxdg.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3gfmqfuug.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3jjdnuaaa.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3lzlmstel.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3tebxoaak.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3abndkvma.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3xdsczhxo.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3gmfhrvqe.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3foqabhwc.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3iosrltvb.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3nauodyjp.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3tqpinznt.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3fmzvsdfq.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3wrttyiaa.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3jaqbiaif.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3yhcwvwsj.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3fgbfxlei.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3dymxhwul.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3ozwsrpil.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3ghabygnw.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3dbarswhj.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3ufcjbfls.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3qvgbsqcj.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3yuolfagj.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3gyvvucgp.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3xrettnyp.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3gwscwjvk.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3yxhapgsa.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3xmwplxjp.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3vebtdsqp.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3aswlxdzc.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3sobzlkzn.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3kalnybdn.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3sbgylddc.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3vbrtfyqo.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3tfnnogqh.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3olbnqilk.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3nznmfynj.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3estudcqr.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3mrujlczm.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3eixuaywk.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3jhbszvxd.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3qqhdfjtp.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3xxdmjtqo.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3jjyvgxqg.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3gjsvrvzw.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3tuhllprm.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3ukvdudie.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3tedfwojv.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3dkxasnuh.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3lgbpflcj.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3vjwaycug.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3uuxtosfl.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3zftqdflr.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3wdbikniz.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3gfscjoii.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3ijdacany.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3bjeoovpa.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3pvmklgkj.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3geyxnkco.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ymcpdayg.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3kkunbcak.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3zufsfnxq.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3otpwwnnr.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3pawqdawo.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3ladluyzj.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3wvbfkldv.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3ysqtfyjx.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3twrhdrgj.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3pupsntnn.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3bpmsfzgt.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3mjqgfihe.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3zmbfltnj.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3nidrmpap.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3ljzgeatx.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3hvnlvwwp.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3tdciyqhh.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3ucjggmos.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3cpwwqvsf.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3hyztroku.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3hxfbjntc.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ltovbayk.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3tmfsplca.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3lwkaeeoa.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3ptvfdwyy.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3kvvaakij.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3hyqgzymy.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3ggdcsjos.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3kjuwobzi.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3pgajabcd.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3hkhxxywx.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3gvregsdo.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3dyyalgbc.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3uuprqqep.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3ldlzghql.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3ndgplnlt.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3ssavbauk.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3ugmgkjog.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3ztoynhsl.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3jvxzftcj.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3kalqlmpq.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3kqiradkg.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3yaplkyeq.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3jbdszlkr.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3ddlkmlfw.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3aruqukok.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3rrmlacbx.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3tfhlrdxc.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3wjisamsb.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3unzqrhle.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3bvneglmq.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3eeuimbjz.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3nomwwaje.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3mjdtsmci.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3ktqfjsrz.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3julnbasi.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3obdjgkqs.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3mdwbrewg.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3gbxgbbtn.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3ctnvblfw.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3lzfwtwuc.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3dwqwpdkq.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3xncypjsx.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3jdvlkxtq.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3xcaaktjm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3zaldnonh.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3hdninsdo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lszjpgzp.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jaqqkxvy.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3lazcabfz.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3slubhffs.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3hgpmfzhq.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3bghosnyt.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3asmtnasa.html


<!-- 参考信息 -->