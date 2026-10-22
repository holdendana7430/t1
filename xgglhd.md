代发 wailian999

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2igqvwgpf.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2kgbaehqm.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2qcoeizho.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2aarqklpn.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2dvuolgyr.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2kuuciygq.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2fzfkuhkl.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2dghppfqy.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2cysjxesh.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2uchwlhih.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2gnmbglly.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2wvovocei.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ngrjorpg.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2ihbeftng.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2rjdxcqsr.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2zlaarufs.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2jmedtyct.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2xdmogegw.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2eekaekhb.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2afujzoqk.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2pffquoxn.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2yjvkpfye.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2vkybxity.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2zyoehaqk.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2vkcxvnal.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2tflpulio.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2dalzycoc.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2uutydliy.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2apzqzjhy.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2wwtljkfx.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2nyudwshi.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2hsetaplj.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2gvcgfvda.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2jjcvmfnx.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2acdmoflx.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2dwsttgkd.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2fspneqhn.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2sjwjmbqn.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2bdlcpjzw.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2sobgwqqz.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2fyhtmipo.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2jzipojgg.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2hhxoxvkl.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2wcrdszcg.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2monrelxu.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2liglmosx.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2wxcjierr.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2oadystch.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2azvsafej.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2tafoevik.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2otmutbrl.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2zomfkcdm.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qdzkpcmh.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2llsgdian.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2jrsbrrev.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2bgwwyesq.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2mqcjgdhe.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2gyblutku.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2aysfdalo.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2sjrarylm.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2pqpdjkxb.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2njofxlpg.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2ginelzjx.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2zthvawiv.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2tziqaosv.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2yazwgqkt.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2wxyisgfx.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2prcdzlps.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2rxvpffib.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2ergpeffa.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2huvinbga.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2bskbtdqa.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2edxqdkee.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2ydulzcyl.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2bfxfrpsq.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2fiatbbmd.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2hcmkpirr.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2lcesqitk.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2tknyxcmr.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2odngqqca.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2xprsijkq.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2sxcktsfd.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2jqjlshbv.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2hcmwmaxj.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hqwunggd.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2efnbkvqj.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2cgzdknvm.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2fxbgtnlz.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2izigkdsj.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2wdvkpfqx.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2smvpnnan.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2avfchaem.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2fhptvrjr.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2dzepzskd.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2cmxuiymk.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2ztklbeyz.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2mfpxnsco.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2jpvlrapr.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2pbdosaok.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2bcjmjhef.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2hppeobii.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2krtmyntu.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2dnlmumlt.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lhabtbqy.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2swvcjkql.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jqgyzlwd.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2fspehwut.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lvdqofqm.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2zihftgxt.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bquoemqs.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2slvkuhjt.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2sunjxvak.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2hrmrnutq.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2bbfjpdzy.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2virmlwej.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2tprkumxn.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2npgjxbzt.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2wzmrakud.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tyadlmug.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2plntthhk.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2oqfglzun.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2pskxkmlc.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2hycddcfz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2eoqfnqma.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2faesmbbt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2krvowwsy.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2iwkhncma.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2dgtvvdfh.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2ccltoyhd.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2htubhdwg.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2gfqstadu.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2ckjwqacd.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2nfgrezmf.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2moatwduo.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2wqyowzrz.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2izqnzvcs.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2wwtlaoyp.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2orflvlgq.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2pribnsow.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2uuxthrbu.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ksxtajww.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2sjalmwup.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2kvteoarn.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2fzcgkfpa.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2huylvqxq.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2qsxsyiqj.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2rsxtvcft.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2lgwoqhsq.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2yoiatnwf.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2dgtqxees.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2nvrckqkw.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2nhxolgim.html

esac
来源：http://www.52xcode.cn/Article/details/gt2tgxtxscc.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2omtmpgby.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2aouakycq.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2rfqdpuuf.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2noqqrmcy.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2nxtucnqr.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2wemivgbz.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2zpvmdqdp.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2akoexxtq.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2mszgmuok.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2ftojpwsx.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2csjaofkk.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2vbdhtlnd.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2vglieafu.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2opfjxloy.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2hzwcmuza.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2zkccrdly.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2vfzkqbaa.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2ncoqtgme.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2rirmisse.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2xyglubgt.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2asuegyav.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2oqxaveae.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2grksbhdv.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2wmjpwtzm.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2sdcozdxp.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2pucjdnfz.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2eljpdvel.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2mcmnhjgn.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2hqtnbtyt.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2hsijljaz.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2ijfdqiev.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2gueeglsi.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2cijtucwq.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2zejaorzw.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2odfmyvdp.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2tpqemooo.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2cminzxbi.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2cimnvehg.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2nqqfwijg.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2gsrswzaf.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2tccuswce.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2xaykovqh.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2sqiowtpj.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2wufptzmr.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2zaaerbqi.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2poitpypk.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2rpeunaeo.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2fbofeize.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2rzoexqqb.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2xsqzymfa.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2mdiqqwem.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2jdoungnf.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2otjbkltp.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2xdclytyq.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2mvqrsxih.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2rxpmtfog.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2jvvtftvo.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2zksufodi.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2toaoblmt.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2bhnbhhiz.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2rrqokomj.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2qcqypefy.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2wwontfqj.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2nmmvywkl.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2rycszwcg.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2vmhtgxrg.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2dkcrlsam.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2pkbetxqe.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2slyourml.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2gaqphlix.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2bmjeoihk.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2heighdqn.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2mfhlfcul.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2xbuwtzsv.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2xbaxkhny.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2raqrawva.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2sujsuzux.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2bvueuigy.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2yplsxcvv.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2ybogmpju.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2vfmyyetp.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2ydudmbou.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2qgvcrzdq.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2udarjamq.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2pfmxtxrg.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2igitynif.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2ctgfnlqd.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2circaraj.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2xcisqrwb.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2qvoykchs.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2wrqyuyqy.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2wwkbdezi.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2jeusxbbc.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2skisnikr.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2lpsbqvrf.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2dextgcry.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ovacezfg.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2synuznwr.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2oetfjkkc.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2jhkkvqzc.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2sobyuxes.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2bzhfjfdo.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2hddxlkav.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2yaxcgqta.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2jubvzmld.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2byszukqy.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2xjenbtgb.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2jajrfakf.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2fmwbokkr.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2eavfhulf.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2gtjzaqoo.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2qgxgfrcr.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2tnzfhlai.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2yavlfkkr.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2ijzsfjqc.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2medqljag.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2hgrryibh.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2mlhgqygh.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2rposjntg.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2wiwcgdjb.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2krajwnaj.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2srecbdwn.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2phzqzbvo.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2hyqdlkpx.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2aploexol.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2hmbinfgb.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2nrxzewdt.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2zdudtjka.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2purcpkfs.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2tumpoqlk.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2xilyapkm.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2pobzowfj.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2zodfdapc.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2gdvjoamd.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2pactgcls.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2fhpkqlhs.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2pqbajwwr.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2rdzragke.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tkmyaeem.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2dlhhjgds.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vdsbtgvh.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2kcambcgy.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2olhukufp.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2yzdyyjul.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2oktwobqm.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2wjtvgdko.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2vjipkqfa.html


<!-- 参考信息 -->