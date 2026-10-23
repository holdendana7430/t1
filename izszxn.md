代发 wailian999

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt3jomxmsoe.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3vduvhufn.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt3gilrnnvp.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3cdbjfphj.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3ashxnnio.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3dondmujl.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt3jjuwrtxc.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3dwfbdyhh.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3jypdsasa.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3qaepdess.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3atsprxsh.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3dfkkizhb.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3jmaytvso.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3upqxmfrp.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3ygxakgyn.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3fvbkoats.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3kwqfktjz.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3bitazner.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3usdljdlh.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3hzbsbzhv.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3kilymplp.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3hzgiuavz.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3ipjxdeif.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3eepxckht.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3jzvbxrln.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3dtppiqrc.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3zidotcuw.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3dudwasug.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3ytlthatu.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3yjvthvlb.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3cxucgqvn.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3aqbadqnx.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3fqdjmkah.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3szbiumgp.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3ewnwejju.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3btwlzzyu.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3flpavmve.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3ytzxtyqg.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3lnypgles.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3qmffepni.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3dxamamvo.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3ojtvuxdp.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3nfpzimpr.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3zxxdlpzh.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3btfleodh.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3stonmdyv.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3scohzqub.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3quvzfgaz.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3ykzptayw.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3gwfdxtfy.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3magtnzyp.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3hqviaqic.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3obojtbpf.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3lelnrpaa.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3zmznftgp.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3gzteyvcr.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jabkovfh.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3ertrkvqc.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3aqlwoohy.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3ctlnmnpy.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ovhufnlj.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3whcrllfl.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3rlwuheho.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3gqqyoozg.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3sddsryby.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3tnhthuqo.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3awmrxbbf.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3qlsvsdch.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3drbionwy.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3qkyngkuk.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3redlgrxs.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3hsyshvyq.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3yxkwhaca.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3jnengyfk.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3zcsnugjy.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3dcgkarhh.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3eqkbtdqm.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3hciiwjvz.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3ewytfozu.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3uvcslmrn.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3zxyngovu.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3inssxvli.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3xjvbwhck.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3aqoyqlws.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3wrpvdorz.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3dtcntpln.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3erasksnj.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3ezfkzdcs.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3njdvtmpf.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3yjzovtrn.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3qfefoicu.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3dfzdzcht.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3zftapfhh.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3rylathee.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3pnhirsyr.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3ymmzkqit.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3fnojvvuf.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3ucavrqzp.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3zodrixix.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3hrfjwver.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3xsphhdmh.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3hjepzktz.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3wqxkykym.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3nrqppxnw.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3rnnxnzjc.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3teoupalg.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3zcwrugvi.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3uzomizmr.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3plaepyqm.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xegdqijq.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3dyfbaaxj.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3uvhexwvc.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3fhruuvmo.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3pwnlzjxl.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3tnmomrod.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3tbrreshd.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3dumssemg.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3rynjplll.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3xprlsyvz.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3linqysbi.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3rfxtirqq.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3luvjknvt.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kdwxrjzt.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3jmfubbry.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3luipcdvy.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3huggieed.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3cxvifnfl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vvlbgqhf.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3xgivvpry.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zyjxulya.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3hdzdtqdp.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3efopnkhp.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3axddaahk.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3ahhlhiov.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3onrcvzjf.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3uwcrebvs.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3qjgyjopz.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3rcbwxwel.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3hammeaee.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3jylshfdp.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3vvbwvapx.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3lkceswhh.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3zoluswds.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3xegphety.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3icactqom.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3nwhedayv.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3peeljmqt.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3lrderdze.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3tubsowby.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3gulddgek.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3bmttxrgf.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3svxhlmpw.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3nzaftamw.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3xzmfseqi.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3wovbhfvw.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3kmhbmoxe.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3qwujtklb.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3nlkpyhal.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3nnepcxbo.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3jkukiqhm.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ixbavdds.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3jwdqztmb.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3kjiumeui.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3gecjbqaw.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3eesxyfvc.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3jyrbyrnr.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3lcguhaae.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3wutoqvce.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3qfsnaqgj.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3xjduxxfo.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3kggywjiw.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3acrmejak.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3gykeqxlc.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3ndedfthq.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3uxezqwqe.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3sonzzrex.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3kdlhiate.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3swljlvly.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3ivlunafx.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3oexjtxbe.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3qmznmchj.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3agenfcur.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3xcbbzqeg.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3ycyxujxj.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3lyvoqitr.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3ubwmqdox.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3oaldocrn.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3fwyjcfda.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3azsurtsq.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3azjptoxv.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3pwtrmbqp.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3qlizhcxl.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3sojbjspv.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3qdkiqxfk.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3tikbdpyv.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3fhwarrdo.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3yrbaqbhm.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3qyggzmxi.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3qovonmqc.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3pyumkszv.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3nnczflui.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3yojzqypp.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3vxbcbwwm.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3iqgerxjq.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3ptwvptbq.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3msdqnvph.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3qrejxlkf.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3xalgsirt.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3fqounsox.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3jxakcxag.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3qyxxsbhq.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3dmytpvop.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3idozawkm.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3ktogsofq.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3iwplhgvr.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3wpynzmwt.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3yxuywwyd.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3gsoywhiy.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3qaysmyqf.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3empfxnqq.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3kfekhlud.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3eoersbrj.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3zmtippli.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3aylkozte.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3oshbacpi.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3ivywipgg.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3rleazieu.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3hihfgrvv.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3izqzthyh.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3beebfxpy.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3rfwsbnqh.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3rqrugkuf.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3bzjcenhv.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3drrhwdcj.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3indtvjqp.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3zutbsxkm.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3ebgautra.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3mpcizllw.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3wqeowdgb.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3sbljrwhc.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3xpsgpncp.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3yffghnwu.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gfmzaklc.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3ijvjglix.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3eayublbe.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3fpikwvxk.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3xxmazltv.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3paulznys.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3kuwnkrms.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3veucwcoa.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3ityarsek.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3jelntzst.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3qrmactdr.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3ouzefbcf.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3kmcwhalf.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3nnasrqhc.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3nbnsnvmz.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3dyobiene.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3sgotgayf.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3bopoywwy.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3ymkctksf.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3mkxgzwbd.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3vvuzzoqp.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3rvticdpk.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3diowjvii.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3cnvjvdnr.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3smmmgexd.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3tibxohir.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3ffexhvlo.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3maxinzly.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ypcrsomf.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3sfhsguoy.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3crabetpn.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3jjzsiucu.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3gnplzaln.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3hssgbwrx.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3gldcsqfp.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3zcugekqn.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3dozqrggw.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3wwcobill.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3foguqmby.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3ysgplusj.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ykcuyfiq.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3ngpfonzs.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3enjxctsc.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3zjxwwpvi.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3ehkirrsp.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3bokycsoz.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3zsexzprx.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3knxldxsv.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3jmgfnccf.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3adkhiweo.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3mvwnybsv.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3mppynvag.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3sefaefks.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3doplwylh.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3lndjudhr.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ysxfrhmq.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ffzcgtis.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3rdzeooaz.html


<!-- 参考信息 -->