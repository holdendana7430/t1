代发 wailian999

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt3gmjmljos.html

[Q32] 分组拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rnylkazb.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3bueysnst.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3rvrnmwup.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3miuqhczc.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt3eaxjitem.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3iztmlauc.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt3dcoevlpp.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt3fqodztyr.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3rslflrea.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3fahqvgou.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3gtzenklm.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3ajoszrmd.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3vwjsbcms.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3tediwiyk.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3gvmncdwb.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3rzlswivv.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3nfylqjtd.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3ujowfxen.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3qclzdghs.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3vmjeivzm.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3mmahtnap.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3nphoknds.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3hjkbrsqx.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3vbgenihx.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3fnjsniur.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3skpxtaep.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3vqmrmhgr.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3llyblnmv.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3xutpcnma.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3nwwizdbt.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3ikiyuyse.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3xrhczfds.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3hukffkfj.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3lygobdlf.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3cyfvtgfq.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3mwqgjpoh.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3lbxqcvrc.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3ajecltok.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3vnlngrru.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3fpkynxlj.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3phvetrcd.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3awpxeoxz.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3amhhfzwq.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3oykqocfb.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3qxjdcoel.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3aeuontek.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3vactwaax.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3fcrylgge.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3dgknwtia.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3rkbwqbcs.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3nwpcgjpu.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3ekurknza.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3ffpzrxqx.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3spfyfgta.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3zsxxwvij.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3npjxpxgz.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3lxbxwrby.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3aprbluoj.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3hesyvhua.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ierllude.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3ynyzmqib.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3slbjwldx.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3xlshlucc.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3spvbtcny.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3czhfllos.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3vrahtgcp.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3xyxwvrvx.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3tozogyyf.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3xdllgyny.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3uiaislhl.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3kftzlrrz.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3cvghmuyx.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3xqzbmgye.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3cqtbmaba.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3abrisyjn.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3yvfnvlth.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3emcworht.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3vteyeeab.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3pbezojyu.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3uslksjdt.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3kikthiqs.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3zbuicica.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3tkbxwerz.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3hcdgygty.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3mfyossxi.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3dqzlwkrj.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3blbqfyfm.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3pmvkbzbp.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3ozhykndr.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3hcctwnba.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3oqbitrkh.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gcavbhuf.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3gbeeeejp.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3jrqgmvdw.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3ocskyucl.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3eyvoojqn.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3atdehcft.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ekvsndni.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3uffkrlvt.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3xnbsnnmz.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3hyeqriue.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3krxhwbqy.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3wfeswkco.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3gxyyvjoc.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3kxvsvdmd.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3xsmheibo.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3ypsvbvjc.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3kslwfsln.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lesbvglo.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3hoswtlfa.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hprbwdme.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3lhjmjlic.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gvgpppgo.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3njrbiojf.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yaiyfxsn.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3qnkwlbuy.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rvchgpnq.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3ijyepbpn.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3eavbqhdb.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3agteynem.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3xplvnnzj.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3pqtjpmgx.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3yywtjlbi.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3gfmzspmd.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3sitymwox.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3evzmhpfz.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3mftzqbut.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3zssxsmcd.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3krbkmeep.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3dtjowddq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hjhotugl.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3lcbxthnh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hurvnvne.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3dmnxoqqy.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3yiccpxcr.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3zdjgonyq.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3uaevwmds.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3zadhhihm.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3jtyimfae.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3filsxmpo.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3kkywqomu.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3jkuaxfiw.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3uwnbytja.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3aowpgnyb.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3hluppqwx.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3ifujtplv.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3omxkyemx.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3mlvdntny.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3tbccizie.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3ddbkczve.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3fpvfdddz.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ziiveqnm.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3vvjxsboe.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3hzpsjwra.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3pgrmzxur.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3vvwtcnsu.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3dfkwwsnq.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3vpsdzmye.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3aqhhdjor.html

esac
来源：http://www.52xcode.cn/Article/details/gt3nsfbiefw.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3jxstnfmy.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3rbvrfhpl.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3oxnqqxcm.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3uljjwwux.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3hvvgdkmu.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3xopxhzgo.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3tgezuiny.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tzpefymc.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3jhbaehmj.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3qumfhhzs.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3omaqngzk.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3fpotplrc.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3uedosgkv.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3nngjmjqm.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3vivuznao.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3ninizppi.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3icacrqbc.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3sauwiece.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3fbqxtirf.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3ozpxjthc.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3ezpomvlf.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3incbpkqc.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3shsojxcx.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3edduypao.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3mghfdihu.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3tpjtncht.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3uzbuqmsr.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3jenombza.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3whuuygri.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3ozpjijtk.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3tsncmake.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3empqlyxq.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3fdjhocke.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3cqhempgd.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3ivmzzokw.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3psdjlmej.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3zepdlask.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3cjsyprvt.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3hktjsqlx.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3zbsjolfk.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3kecyyylj.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3expovjmt.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3gpixmpuo.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3ukfgggfu.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3jxahufxy.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3cmufmhfp.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3dkxylbpo.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3wsqroiqu.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3xgemfsyl.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3rnlpnsky.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3gnkslfya.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3ptgulkdx.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3fhaakqtw.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3shvlmkop.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3grspatun.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3mdvoelug.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3hxdxgnsy.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3obqszoaq.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3lskhnzjp.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3tdjugtgd.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3lufsemdi.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3trhndatl.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3yabsxfve.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3igfysgvv.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3slgltenk.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3bixephnu.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3tndkbvts.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3zqwffpub.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3xixqhanm.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3blaonuku.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3mxinxolp.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3pbetwbph.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3bsshtdsk.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3kkyqpasf.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3mzbalkjg.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3nccvtyid.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3laqcmody.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3rbhwrjro.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3jylwsyqx.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3mwsmvmkw.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3auuhnqsu.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3uuwruvck.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3yppgnnet.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3cafvmqfv.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3inwywomk.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jqkughne.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3vdkuoajs.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3pmzldaqm.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3qcfdhuhd.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3cnlfsezx.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3zetztrtw.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3vrqfgknc.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3uitxthdc.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3mfbjteyu.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3xxhngbgr.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3wfzmoybf.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3alsterlj.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3klamjeex.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3ydmsfiot.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3ujgtagqk.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3qcdjyfgp.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3pcfainap.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3botldiij.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3bgxdlyeb.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3vlaxdgfe.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3gupqtkys.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3oenznzza.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3fftaubgl.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3nncokjmw.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3bowpljst.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3prcajuak.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3ximgwsam.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3pagxtisu.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tqtuhcnt.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3iwsdenwx.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3urrvlcwx.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3kddvxabh.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3rxtqtxuc.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3sprplxrd.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3iibmwgcv.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3xkcgfdoi.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3ibsldmrq.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3wzwjugwb.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3qqykwsxv.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3jeebguho.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3nlrbhkob.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3fdlrcypi.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3ffwqukec.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3zaufyrza.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3jqnorzlg.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3uktcjizh.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3garuvtlz.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3nuqqczrg.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3twsnmsvu.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3qcxcespd.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3dtfkqmqp.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3pgdevbqq.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3tdxlimvy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3moswersx.html


<!-- 参考信息 -->