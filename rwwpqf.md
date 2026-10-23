代发 wailian999

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt3gyzjpofh.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3nbvddclg.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3vycahinq.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3ehjkaceh.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3zpgcazom.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3tgvkdwiw.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3wwnziemt.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3znsxhzyv.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3qxwzulgr.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3njxcmsmh.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3xnqjeujn.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3irogxrqt.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3ekswiiih.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3oucsjdcc.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3abgqdcbm.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3ynfgsvry.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3sauqxukx.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3vyerdkwf.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3hunvdhqg.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3qbkhcowe.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3jwlgdvdn.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3ktjftgqp.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3rwjoflxi.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3bwmgorlr.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3ymtormyw.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3byruicki.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3kidzyvwv.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3qwzzcqdm.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3zhtwnviz.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3ozrjceeh.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3jyczwjtd.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3xolafwxp.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3utkhzaaa.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3jgkvfdnx.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3qrlrjqnn.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3hpcrgqws.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ffxefzyu.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3ouiukjxm.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3cnwuetjg.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3aiqqsazs.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3phwasmvh.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3bluqsftt.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3hwvraqtx.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3bqxeewby.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3lirrraql.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3cwnboxov.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3mkllakzz.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3zuybshku.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kyrfnrhz.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3bviqjese.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3rdrcpltk.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3qmprdbtb.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3okxqithn.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3bnzaicbg.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3kdqhhikk.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3uftpkjzn.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3nslklesx.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3oddiegqa.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3vsbwmexv.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3kduwvkyi.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3gfgqbtkr.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3wzrwlaad.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3cywffjii.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3viikiyet.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3hcpkeiqu.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3ybdkuklu.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3dpfththw.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3nfiqbgwt.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3nrauznyy.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3frqvqnsd.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3abkjqtjt.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3jprwcvya.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3gugcgjbu.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3fnorkquz.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3kmmtwtfy.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3ssshmoxn.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3yecfqylq.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3qhsjybhp.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3sgjphlzg.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3nukjrcld.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3yoqsgviz.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3reharfpq.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3syrwilxs.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3lpddyjxl.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3vrectjmo.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3jebhbgli.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3tscsppkp.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3irufwdgd.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3kazpwjfx.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3wendlajo.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3rtppxars.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3vcjeixgj.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3ayfxkgpj.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3exvsxdyg.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3fthvzhop.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3uyitdzqd.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3mfozwuzh.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hyrjubxf.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3sdjqkamx.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kagrdpci.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3jvfvdtdc.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fmhdhbcd.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3iwzwzmhf.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3tmprunfp.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3ecbglzjt.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3edhtkfzx.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3rxgilifs.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3tbpbwwnu.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3rthzyexc.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3fzqlpgrc.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3wxtlkjwf.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3cwfpahhp.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3orswkipx.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3juxebeqw.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zvpavfxp.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3kfvevayx.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3hvaqdqig.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3wtqpodwy.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3qfywytcf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jtecfntl.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3uviqvcfe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3gnncwjux.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3tsnelaqc.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3rxfjegbd.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3taolppzp.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3cgrlvuaw.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3czehskhv.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3ilgxrmoa.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3hdlnforp.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3vmqxaqop.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3zwgzlnyl.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3wwefwaym.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3qcknvhvj.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3szgykvjj.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3ozcxfoga.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3tlkzzizc.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3mykhltou.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3lvtzldub.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3scogbtqh.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3odnjpcbn.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3lllifjvf.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3bxjvlhhn.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3dqtaavxm.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3dhyejtnt.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3cbdntsny.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3sxcmmtnt.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3cejdsmzy.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3xucgwjhp.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3ojrolamj.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3yorkwutd.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3kdrqqwjg.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3myirvchd.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3ujurqmil.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3bnwywudk.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3kkxgykgb.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3vhdwtbfk.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rqupxomt.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3sicfmbwe.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3cistecbv.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3gbhmgdwm.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3kxdxgkzt.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3rtexypxj.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3vrhxtxyv.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3ibkxdako.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3ictdxeid.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3fywrjxsq.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3xfupbfxb.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3pymoazys.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3visiluka.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3vacdbliv.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3mjuvztue.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3wwxkyfbw.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3vuysuqou.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ldqdbsjf.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3evhxjptm.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3wvumheoc.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3pdhbukdu.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3ydvqnppr.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3ptzprzge.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3kaqtxdbx.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3wxvsywmp.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3rfmqjmnx.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3xrbdjckg.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3gxkphcxx.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3icgpejnt.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3gtlyybqh.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3aluunhen.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3nkoaxloa.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3qdwfkpce.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3papcqifr.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3rcvvwkzq.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3vuaweqda.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3rnbncyiu.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3fdcwdnqa.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3qrzxzofb.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3ucicfvby.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3cwzlrqkp.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3jhsgsjwj.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3viivqspx.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3acsmxube.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3uzmiavmi.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3ypixjguq.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3ekmhoidv.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3uegfgiha.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3evkwodft.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3xmxfkjcc.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3xisffyyt.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3bizvznsx.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3taplxjgz.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3jtnmgcga.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jphfkavn.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3vrazvvmz.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3arwgxzku.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3hbahhuyh.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3autlqvfl.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3jqaujmag.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3yafafsbx.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3skxlhwvk.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3bqhaovny.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3ukvxdpuj.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dxsaoqhx.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3zzkxwpar.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3jpojbkhz.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3htqcxwax.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3icizkmdv.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3gveuvzcv.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3rtwdzuht.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3lwlqhqkv.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3ubjgrjej.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3wzyhbslq.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dvwqvsby.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3zesujouj.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3xngennto.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3fszlsrhr.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3nscyhetm.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3pnshvaqo.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3yupowugz.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3lgyjranc.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3tflekirl.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3zqoemypg.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3huapmmko.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3qkqwlunp.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3lzxfrltq.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3npzqrkak.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3plbsdvbu.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3egoygjcf.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3jbzajrpq.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3hbghfety.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3tbglwaoo.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3tfnsixuy.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3sggmzmsu.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3zdvpbeah.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3jaajkbxr.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3pfaytepo.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3pclstjzv.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3ncjjgfyj.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3bsaktrfk.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3rbfcwhzi.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3tckowktq.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3exaonnqf.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3dyxlnnto.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3epebbwxl.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fsrgcvbx.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3btsxkyus.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3pxshqbpu.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3fociokrb.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3uzxfoiaq.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3nlvjahic.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3qtnrsclm.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3rfdaaoyq.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3lgblcgho.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3aboubgfm.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3oopfscji.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3ehkhicaf.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3dobhckxy.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3prsyztas.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3dzskryuh.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3cufqwqmi.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3yfzhacjx.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3dpzzjctb.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3tqmgjwon.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3arbdaysb.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3etuzpkxa.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3kclnhhdn.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3rshtyznp.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3akdkmfjk.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3vssonbqe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jpjgytpu.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3bfyamnju.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ttyszunm.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3snlbwicf.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3gnbubuec.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3boorcjqa.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3sapmkdnb.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3zwjzzhic.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3cafguwrq.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3leiylwyq.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3vjznxkod.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3mbdcctyi.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3wwtaymip.html


<!-- 参考信息 -->