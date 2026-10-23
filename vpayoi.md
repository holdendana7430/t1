代发 wailian999

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3plhpwisu.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3esdvkcrh.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3bbdfzafs.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt3cpegqxxc.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3ousdyhcf.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3iqvnzvrp.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3yrufezoj.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3mwbreino.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3hpzpggrp.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3wdcypvdb.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3shgrlkvd.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3quywmusc.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3gbvmajdt.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3lvhlvdzf.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3bszcoisv.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3ivrtsnhe.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3dmdfrdjd.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3xukmrjsi.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3gmyecbwm.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3oglfbimz.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3bkidpzsx.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3vkbfbric.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3bstuecyf.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3nbbkqglu.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3bdxxrgtb.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3aoaqyhlh.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3kuyeaqvj.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3idbxtgnu.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3gipmtoou.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3lszsfmma.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3ukarbqwi.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3jaxlswig.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3pvyecrip.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3qwdapnae.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt3vyzhqugo.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3swafwcew.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3ddiauutg.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3vjbgoffx.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3koavtrie.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3plicfdor.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3vgxrdhzp.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3fddwognw.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3sakjmidb.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3wxzksmrp.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3nckxfwnk.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3rnobhcxl.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3hmntpedb.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3kaiiktah.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3knmnqtqa.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3slwxdkot.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3pvdamxyb.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3rkbznrxz.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3rknuewee.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3sdjovudp.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3xwxtnabc.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3kjosberz.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3pjrqudwn.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3tnuhpfyb.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3sysfzleb.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3lajsvudr.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qrhkpewu.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3mkkihncw.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3znzgwcdu.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3nmrpaxky.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3pkgqghli.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3excrtzoz.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3lnpxcchc.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3whkwvkge.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3krlyzreg.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3sisjxqmo.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3dtzkizdh.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3wdxndxmj.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3qvmqibvl.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3diwjygsk.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3xhxmaran.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3ebuclcvd.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3nbmwhkck.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3rivzayul.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3nwvqfuzy.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3yrcknpct.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3ygqlnicq.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3vtpzgohg.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3lqhaoezz.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3ivazlqhf.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3bfdzwotr.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3adrpyffb.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3hhllngdp.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3mbunsnay.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3kzxrrbvy.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3mocvxxwf.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3bwxmkxfu.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3dowhkiil.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qbvmoqhn.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3xnoathsk.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3xmglgukg.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3wajmawmk.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3pwlyaqeq.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3dzyhxubf.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3adfmqprs.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3axdspecq.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3jyqkakov.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3sfckfrqp.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3jqigysjv.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3gqiahelu.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3ltvinqbq.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3mxrzuvih.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3vntflrxy.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3hnvubadx.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3glujfghs.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ycgiypmh.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3vmgqgiby.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yknsagjq.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3oaepvitg.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3psugnfme.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3xwjcsbbc.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kbaaqfcf.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3jcwbkwho.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ifnwvmsm.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3rdrvffes.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3drvicdjy.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3nattzncz.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3nojvfpzn.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3fqqdxsfs.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3binelrry.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3ojbgnipw.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3roskaelz.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3drqtnijj.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3gggoneqj.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3qejvtina.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3tquyouxh.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3hyrdoekh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3orlomrls.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3kdiwjfmm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3flvelrut.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3uwxyfnrc.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3csgelgzj.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3ayyqighd.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3lcnxpvws.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3jqxaglqr.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3epvxdhdn.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3gnffjihy.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3pcrnutbe.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3pczeohca.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3suwjogyp.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3eacgnjbd.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3nqsdbnsy.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3pvprrlzj.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3zkkzsgtr.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3zqekcgns.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3zpcidddw.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3fmeqkpin.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3ndiytqcz.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3azjfgpcx.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3fvmswkvw.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3rtzguuws.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3hrwrckfm.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3vhthsmzb.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3nswswqyw.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3ppmgsrvm.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3tmjrozbe.html

esac
来源：http://www.52xcode.cn/Article/details/gt3widuxdrq.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3zkmqgqux.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3fvkpevtl.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3ajozcreh.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3qkiqywpc.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3bjokrpia.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3tiqhaueu.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3bdjgxrob.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3wzszgzmx.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3uxudcdeo.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3iiimjnpj.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3nfqelbwx.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3ndvqvysv.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3odrmqwpz.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3qwnsvtjr.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3rlqvqxix.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3gknltenx.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3bjhjxern.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3wgaggpbt.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3qfrhusgv.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3dyayhkwm.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3ykghzecj.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3mvqpvedr.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3gqadgjrg.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3uaetgtvr.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ecgqptlp.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3xggbfxaq.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3ncpnatdz.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3osehfevb.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3xizxnpla.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3itklmhsg.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3vdximcdf.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3thupygjv.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3kpqhaunj.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3pfvroroj.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3mkfbbtnq.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3hiheehvd.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3vlwxtdia.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3heogjmii.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3fbnclgak.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ncgyzgpd.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3cuviiqnm.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3wszlknvm.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3rujycikj.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3zgpmiiog.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3edmkxekh.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3iynepvza.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3wtkrigns.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3syvucfqc.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3txwlnzsv.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3zxxhrtxn.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3qcnwqxzm.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3mxwigvjs.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3ngiiejdp.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3kgxacubs.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3cwisxeuw.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3slbbhupm.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3zmxwvihk.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3gmonmikv.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3engpbeuu.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3mqytlogs.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3ncckvuke.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3ctvvjiwu.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3hlkpadvc.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3ijspfbzb.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3pwfjzcqw.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3vjblxqyw.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3nazintla.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3qfteejgk.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3gwzponii.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3vrqxefho.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3cyufjqqb.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3nbrmkass.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3xdhftfcq.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3iypofzdy.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3hvscmlbm.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3psklogap.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3ygerftsp.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ofogigyr.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3sjsnxkzn.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3hsgorvur.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3rxcgjvkt.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lnspgxnc.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3yfwbjkbw.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3khtphjfd.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3ykibojel.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3bvquuirc.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3nparttyy.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3wqpbylnv.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3awevagqn.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3knvbeufo.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3zeudnkpg.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3cpuutpoq.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3crewfyxd.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3nvymzmic.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3lnolslsj.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3uqzwshux.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3qeclcbpw.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3gbdmqnal.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3ozwwsika.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3ztxuwpdu.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3htmeiqrt.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3kaimbufl.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3opfrwpeo.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3lfjhzsyg.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3nqynhnok.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3sebzvljp.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3ukbyrpya.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3qbcqcocg.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3qlcuophr.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3lifizixp.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3uoxqjkgc.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3yzditlcg.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3tombmuug.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3hqpsjfos.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3lhuxmytt.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3pmghnaxv.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3kvyzwubu.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3vkfepadb.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3pwykdppa.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3zatmzlne.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3mcmymxmq.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3bdmzsuzr.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3pvbbynhs.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3vysoydfh.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3qzgjdmzu.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3mtaztihf.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3lpvdfnag.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3oforbizq.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3vzbnxgos.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3urjqlwbf.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3xbmujljp.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3vrjrwcda.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3pbfejaii.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3ajjixdgf.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3ecrcjhyl.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3mjmnmgls.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3jreqqdrq.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3rknfncna.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3usfyusin.html


<!-- 参考信息 -->