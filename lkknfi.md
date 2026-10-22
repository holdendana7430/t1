代发 wailian999

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2otltngtf.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2fgysjfee.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2ktyekbwf.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2cilqoqqz.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2zcchvcve.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2xwkvdnhv.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2utmexrng.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2eiqbenup.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2vnsuadcy.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2kupnygcz.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2ozgyqbhd.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2jomhzgrp.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2nlshgwrt.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2pcdumtkx.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2atgkxlaa.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2cqrazlpf.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2itrkqoaw.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2zufretta.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2ubrcritg.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2puxhpsgw.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2djckxsui.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2hrcujptb.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2ttpltsgf.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2cngoffvg.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2wtijsrev.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2zecnjysk.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2eefvylog.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2knnizcho.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2nwdlpaus.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2sgfbvqrz.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2iikbdhzx.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2ysyvaxtx.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2zpxzpxgo.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2jhikvldv.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2jwdhifqz.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2gjwdczvp.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2oaumwltj.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2uvbpitkp.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2ltakldmy.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2vejsdxqe.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2flzxaftw.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2tyqevcxi.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ejaydgro.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2wwyxjbqo.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2mxdgwuff.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2uufjmjvz.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2wzptturj.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2lwmbabkl.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2ahcpbcgf.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2qaaxvfim.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2xyntzbcw.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2hlaxeszr.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cfyzapab.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2olxbvbrb.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2jjexhnje.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2igpvlrmv.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2tbqdqshq.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2iefmzyli.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2fnydovsk.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ursuemhb.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2wjgvzmjd.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2pimvuwjc.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2offqibxj.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2yijfaqjk.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2qkmztluy.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2aowsuovi.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2tublqhqk.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2ykuwgvqj.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2eftqhtao.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2vlzazwaz.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2wmzsenbp.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2nxjhmxaz.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2kdmfzwbe.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2fdvdznzj.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2kugfjkws.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2pjtwoazr.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2nteqadgt.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2xkxbnxpi.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2kpxdxohu.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2mwljabfi.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2zjanhrcj.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2uezcrwdp.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2ykqcylhw.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2ntetcxgn.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2embunohn.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2ajcqiihc.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2kiwyudfg.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2rfbmvtte.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2jlxhdwwt.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ysohdzzg.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2yczphgqd.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2opyuvncy.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2cfmrscsy.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2oldqnxlv.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2ytzryzpt.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2oawgkirk.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2wzamqzlf.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2hfqpmwnh.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2zsrjhnyq.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2takriibd.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2ywticgjq.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2uiypavcp.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2fofererv.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nnupvuar.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2clmoyyqa.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2edtqpyyl.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2bnenrusv.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2yzvoitow.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2zggcowhg.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qpwhwupf.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2dsisbdqy.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2vrkkvwjz.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2nxdouphh.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2tyzjuofe.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2ppraznxo.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2izpzcpit.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2laiibbhv.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2hbuffhir.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xzqrfogq.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2rxavuhtb.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2mgzqgcjm.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2ewewrdth.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2ssjerfrm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qgmtfcxa.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2htuzkpvb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bgpooptl.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2vxdshjpg.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2qisruoep.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2jvetqxlu.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2audwejph.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2wyekbxne.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2rqiklvup.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2chvdytky.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2almwusnn.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2miqwdmdd.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2geeintsu.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2yvwxzjxy.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2wvchvghi.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2pjedzjgv.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2bgfnchue.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2nfcrstfi.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2ilqbhbog.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2vvtwpchy.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2vmwjfxgx.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2dgvcqvth.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2vkwmiwok.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2gsokkeoq.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2pvflagga.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2qcmkbfyq.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2pwjygtlv.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2aybpguxq.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2rueuxvxt.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2nowdfnyf.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2vawrlqeh.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2vabacfqh.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2qgtgvywz.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2mfbrdxho.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2hpopvmms.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2suobnqrc.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2yzqddjss.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2txmnkybj.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2rxkxqiqw.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2lycewhhh.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2wgeqiaxd.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2hrsvgkpx.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2gerijubv.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2wcirvdjp.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2vevnhaxh.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2blkqyoyz.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2segfdpbh.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2bciifjfk.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2blyteiyp.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2cezbpuco.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2qwtkujgh.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2vxokgqeg.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2pwsywfcl.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2owdmjzte.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2drfqvnyc.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2okrchcym.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2dvtfcmyu.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2cxygwvwt.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2cxnlzwsb.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2jhsuzylk.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2dhvutrtz.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2tkaqrdjo.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2svpetdkj.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2mdqmelln.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2cgtsawmk.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2jpsxflgl.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2bljbzpoz.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2occkbubo.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2ziywkkeu.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2myiousrb.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2mmwibasx.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2iukqiwhy.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2zjfzcdrz.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2ptwmcfbo.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2tqucedcc.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2ebuidpmq.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2oinfucex.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2eblvjptx.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2ztllwlvn.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2utvymtty.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2kfkjuxzd.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2dzhgkcbo.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2dqmoqqtw.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2ggggazgm.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2xuphwwgj.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2hdvcrmdp.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2faiwvvvm.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2hucjzrqg.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2ovyoawjo.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2jsyfdtni.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2afvtmlht.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jggfhpog.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2kponswph.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2rlzitzsm.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2aaogqeht.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2qpjpgjoc.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2fyxfxuxt.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2mdtdudwk.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2tbqlimxi.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2hsbrsybz.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2vjmwszed.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2qnjovnor.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2suontrhz.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qlhqtpyi.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2qqqxuhgs.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2vzqcroqk.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2okcdrzqb.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vitxmtol.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2nhujxirw.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2zyhuklry.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2pgvqxsna.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2upfjhyvf.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2rnhwawcr.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2pztjqidc.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2uzrfezwe.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2uapkcgyt.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2codcodsy.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2nsxkvmec.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2srpuuryq.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2kmbhljni.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2iegpnvzr.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2hlqxwsor.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2spmjrgoj.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2mldrdoxi.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2tcyscqiz.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2siaxlkwy.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2darxtfrw.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2aeqvrlwk.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2ctnlekxd.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2tcnbtpeg.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2tdnbnhcf.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2geatykgh.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2vftdcclr.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2wulkxfzn.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2frvygbah.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2hgtixedz.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2rsapibrg.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2jfmhhxbt.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2rhdilrks.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2oyfnttlk.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2xajvyrdl.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2xpfuxbfn.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2qrkvclpm.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qcwbdicc.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2hdnoigrj.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2ftmsdzur.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2rmanbmwp.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2xnmtofcn.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2fphliowi.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2cuyqpkyw.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2mdohuioe.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2txjwgzth.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2qelalcfg.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2luqitlww.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2cpxyrqwp.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2ndosjmsp.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2prgunynz.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2qzopcked.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2ijyadosh.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2lqhnnmzw.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2utyyrjfg.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2fgknyzjq.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2omlholho.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2oxkjkgck.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2tobksfli.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2oybwepck.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2ukljffow.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2edmdddcu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2purhileb.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2grquesox.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fioibwvv.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2qbtfyxag.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2puobsipf.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2garjmhev.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2vyafeqhz.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2jguaemjt.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2qixbnsgm.html


<!-- 参考信息 -->