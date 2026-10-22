代发 wailian999

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2ornxdbql.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2blqavaaz.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2fiuzftth.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2lxmststj.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2phxaqvrb.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2rlsjtovx.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2zbpucuix.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2cgkeevdp.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2xqaxjpqk.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2oimwmnez.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2wmeidxhk.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2eusmmpnl.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2oiwvlxxq.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2cbdzjmet.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2xumjpupm.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2okpjgpcu.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2xzpbyenh.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2ulrquomr.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2uobqcafv.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2xbymnyav.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2qvewlndd.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2ckaccmka.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2qaryxqwm.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2cqazgvlb.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2kgjqhlpn.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2ssdarvxz.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2rluxicke.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2xgenhpwb.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2wnpmqrip.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2spccmzcn.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2ztgnercq.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2yubyljll.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2fctfvnza.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2cxwzikwd.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2zluebqha.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2eysyffqm.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2nswndmih.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2eegtetjq.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2nerjgtza.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2irzrcqzm.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2ljsbmauy.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2iyyqlqgj.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2kwjuhhfv.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2yxitfgaq.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2yyjdkaay.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2xfeqzxcw.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2tilvatgg.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2uivtwsrd.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2vsddcelj.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2qvzbjjua.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2dvppwmud.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2cmbevdpo.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2roitkedq.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2spuamsvm.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2akkxydbc.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2cvhobrew.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dfcxrswt.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2qbnsqmty.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2dieahixl.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2pxgdtrjo.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2uujhjorb.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2ydlkcviw.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2tfvhqchi.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2vrfkujav.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2qxsarpwf.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2xooynwjj.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2xoysdayw.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2rtazixwy.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2pkdtlfrt.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2xasgxjus.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2ypetuacs.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2uwllnkyg.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2zyvwqgdo.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2zyjtsyhq.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2efjywkst.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2imecfixd.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2tdbsxyhb.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2hffzuzus.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2ivfztiaf.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2apsmlnmp.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2afwblron.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2xfztcjuv.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2fhoenbpg.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2rvxzivsd.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2fdumhwle.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2vuaidkms.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2abafqnds.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2vvsufxny.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lpmgbdna.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2yenbukxd.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2qlreobzt.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2wzsmahjj.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2sxbwwmom.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2zovjyblt.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2cplqdsza.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2gatcsshc.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2fthkymyu.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2ltaoalwf.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2dxdvagqr.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2qebwkvnw.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2dnspcwwu.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2mcezlwoz.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2yjgncdew.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2qgjqahfy.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2ndybfkya.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tvixfbfo.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2hznwluay.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2sujqgewa.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2dtzottwl.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pghobqrj.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2xcfkojcf.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ajhuahhr.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2cjzrzcfn.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2uufnvsfl.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2kzdyxknw.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2uqagjoci.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2yhyvzkqi.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2ceehnedv.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2vvuzakhs.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2czvwlltb.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2xrmkosdc.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2ajaxzizr.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2yziorusw.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2kxeebqmg.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2qbhviixu.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2rgseaibg.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2wwutizrf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tsezktgo.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2bvovtnxl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2hpfmjwcb.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2ppqwowxx.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2kfzpfnmv.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2fsitjpar.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2wpspemuw.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2vzbuqsrl.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2zuwmywua.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2oinzlygk.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2gzjgcjse.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2xozvnfda.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2icrknzne.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2aqirfonv.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2mdvdufzg.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2nvltheul.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2kiukkier.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2txlicbga.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2dgzhbnum.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2nscrwwpp.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2ydjrawbq.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2aouyadev.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2wsioutig.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2njbtfnzh.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2zkhhicbr.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2qzonbbfi.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2fkkqzbhn.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2zmjiroem.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2cwkgdnvj.html

esac
来源：http://www.52xcode.cn/Article/details/gt2kqyngtln.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2usgqqgdz.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2heangxns.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2ukdbscbj.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2mvjjqvbw.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2djutquzc.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2rwihaxbi.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2bkiqrwgt.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2ezjaiihk.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2nzsqaici.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2xadzbvqj.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2qeyjzcje.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2gokjuehf.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2uadujsgl.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2nifwddmb.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2qxxqsqqf.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2iygkhjtw.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2scblzryo.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2qhimxxyc.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2ulaqzvsu.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2flgrjatf.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2exntzeut.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2khdowbex.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2fqdarmsa.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2mvptsyds.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2hktlverk.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2rqepovpq.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2pyxxxsoc.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2sngqqhkr.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2cbcrjwkc.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2xyzbffbw.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2fliksfbc.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2fdqrrurr.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2lynszboc.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2mgkpwgdu.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2dkpyfxoh.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2yqbdblpm.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2wlzwysfd.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2blepwhua.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2gaubtsrq.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2dkwcaatn.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2rsruqwbj.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2kqabmdno.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2zhuxcxko.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2jzntxuac.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2rprswhid.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2nzklcvbu.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2yobmlgwf.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2lpodznmq.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2icpoyoxg.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2pfzhnkum.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2btgrrqke.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2fdcbnerz.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2tunzlsjc.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2jkygpeee.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2rydpvojn.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2snrggkcs.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2iudspzim.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2umrbmmdn.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2ssjfeowe.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2atbsltjy.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2tammoeou.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2tfxocrwb.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2rlitdqys.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2otpkncbm.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2mwbzedlk.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2zsavueys.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2qhrfmlgx.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2hbzjdsvz.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2jznyokif.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2dilvrdpj.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2zicvgjnv.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2qowpqfnj.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2lbjfvood.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2dxyorjzs.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2srlmggwp.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2gwqydezw.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2knltjptv.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2zzumeran.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2ykecocbe.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2xtutskrx.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2cwgiotbi.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2deolndom.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2xdqbuxas.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2gekbrimo.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2mltkuhdt.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hehjhuly.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2yatoatqj.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2hltbpxbo.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2vadhusjb.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2sgmpgyex.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2ksfmefxc.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2ikcjfkgc.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2xgoeqoum.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2uiochfcn.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2yemmvpwg.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2lmmqlvjf.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2erzjcjqd.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2lhvmabpe.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2sswgoash.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2nfqcaujv.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2cflhhrfw.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2hbivhpkh.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2xqmxbrdg.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2snwksjvj.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2mpqlfgtr.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2yirtrdml.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2lpothotk.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2hpfzzzbn.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2qzxbofee.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2xodmkifh.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2lohsswik.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2nzxaibyb.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2kytxgoxc.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2lncrwkaa.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2epshisgz.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2dwrcgdfc.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2pmcuadkw.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2rgxdtgib.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2mbpbebyg.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2dgskqhoo.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2rwdkuwja.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2awlytgvs.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2qpfwomfg.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2cszkonrf.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2kvcyfkex.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2qbxeslza.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2kbvvwtbx.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2tvuvbeob.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2ddoliydz.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2djfgyhnn.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2ncohirwi.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2cygabpxb.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2xuvewcrw.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2gvtmthjk.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2bmfohure.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2cvxqprjl.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2kqbxfzhq.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2xldvaffo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aydungew.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2zdnpfqxl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2qzcqyclp.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2dmvahvhv.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2oprgelha.html


<!-- 参考信息 -->