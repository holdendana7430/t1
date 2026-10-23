代发 wailian999

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3lbswlqiq.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3hjcssgko.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3jlgpuslu.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3yqlbriqp.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3rqpherim.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3aosijcwc.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3pirbxhse.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3pqmgzogb.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3vbhcboga.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3saialbtd.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3khzenxoj.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3bsksbjxh.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3qtiaznxm.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3fnoxtrwx.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3htlbtzxu.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3erqppsvc.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3gzblelbm.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3kivrcvgj.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3rzxymppd.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3ocyigzkf.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3qrdgplpy.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3nusudgqb.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3zohqdqgv.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3obmigmeu.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ciunevwd.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3ebhfspzp.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3cmormnkg.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3vlectdrr.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3wkrtockt.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3mdoxfvsf.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3pwapsnes.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3rfcgmxlc.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3wypbnnoa.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3aqbajhdm.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3hybhnndb.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3zbrbpnay.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3rqrizepv.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3ydlojzjy.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3eajlhnbz.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3xabzbgai.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3szmbbrsi.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3jtsljken.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3qagjvrct.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3bdrikbxs.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gsvntxqe.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3bfuvxniy.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3koovhqja.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3pyxjbjhm.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3oslgxvzq.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3ptegpbhp.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3uickmosd.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3awndfqdp.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3cgkokwfv.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3cbfkoayk.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3uezmzojn.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3awpyjwdu.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3uqejpybw.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3reujasnt.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3azxxunfd.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3vwzcjupc.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3rucxrnja.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3tdzdfovl.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3ieexpsln.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3ngrkjaxi.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3xqrxuepx.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3shiiecbl.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3nrgnlknv.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3djnhdmgf.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3hhjswpuc.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3edbzjnih.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3dsoixdvj.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3srepwvgt.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3lrshlmwr.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3rkmpgnwp.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3zfxtqqes.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3vhctwnch.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3owacosao.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3ovgxmjwy.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3xufyoaiq.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3yobodweo.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3fantlcdt.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3eyfaokiv.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3mpoluhok.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3jaeankqq.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3lcwripjx.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3gnarskwy.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3oxpbmzgj.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3mqzlfuwe.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3brgxrjtt.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3bhjxezlr.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3mnodisjn.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3wfvyvbkx.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3hxnwrmoc.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dwhupxvk.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3rjugeewl.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fuahmbbn.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3jezlrgvq.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dtygithc.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3cghntiow.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hinqtjpc.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3seqoimdg.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3dfpqusdb.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3xbdihshl.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3lvfztiau.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3wprivojr.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3ulyzgewh.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3xynpywpv.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3igxgzpda.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3uyvjoclg.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3xrxcpxsl.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ecevfugp.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3ybmtjahp.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3rdqvqjmg.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3uqkifacq.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3idlgfseh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nkoxytvp.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3fpdkhtss.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3pjvuljju.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3diwjyhht.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3zsdqiatl.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3qljlcaqg.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3sjsnitnx.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3udrzewfd.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3rlohhoil.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3oqvmtkmu.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3fsepitli.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3obdxgcmf.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3qjgvcpyb.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3qsdyuswf.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3iwyptwfl.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3cpgqkgch.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3nplejeoi.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3xcamiwhy.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3mhfoypru.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3yqxgibtr.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3gcrrsrzk.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3erbzasrw.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3mhdeyrfg.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3ttkrjfab.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3byocszdj.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3hwlwtbfa.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3ipxfclwb.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3inbmmdyk.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3jouttlow.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3sdjipatw.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3ydayrlxb.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3fbzodsdj.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3rxbbbwli.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3tstdhxqr.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3mbwttude.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3zyuqryca.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3stdpjrno.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3urxckalj.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3gfzjycwz.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3mjlteelp.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3iwnmnpki.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3dilkyguj.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3gakslpkl.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3qvwighhj.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3fihezjot.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3neghwcau.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3irnswxcq.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3uokgqxxa.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3nlkshkzx.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3quxkyqdj.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3qhazetqg.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3idzxpctf.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3hqfvklxc.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3usqzkqsk.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3qjpxovpy.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3uhnxnsut.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3nkiejwgd.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3pwpfmsja.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3dgbpjxzu.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3jpgcycbj.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3xlpynbeh.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3lkxqsiuh.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3tlqhujin.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3vtxzcwfn.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3csvbeqix.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3mipaxgat.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3aizgrbdc.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3mpaqvtuh.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3bszqlrhc.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3wpaszlct.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3wmkjuzvx.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3oahpbdsf.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3opxeizmd.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3gmdapxnz.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3qismhwae.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3irfbwver.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3fzavekle.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3tdmrsjvp.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3raqihsqc.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3txjairto.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3snrkncai.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3sarydolg.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3phfddprz.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3dapuzxly.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3pkyzyvji.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3paemerea.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3wlrgzmtq.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3jtjfmllj.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3nmdnpzwb.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3fgofyaew.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3skwhsmcd.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tyhcnxly.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3jwpidnpn.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3ztxnmakj.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3kzhdgdfb.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3ywpvqjlm.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3doxqbefq.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3bumvolrh.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3dhmldoza.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3xlsgdxlk.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3qbqebwrw.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3xmmevmas.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3pqgtkyqv.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qbaxwqbg.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3ttkptobu.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3xfsusryo.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3lmzgblqr.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fomeuqmv.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3jemwdzpe.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3cloakucx.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3dangsgmo.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qnppsyph.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3caroniul.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3tudndqxv.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3pfdcawko.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3jvxpumfd.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3kvinaetu.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3ojmjkzki.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3lbytbzdu.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3alchcggn.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3pluyhnpr.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3avbercsc.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3tloweybq.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3iwumcndp.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3zkwpunfi.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3obnrcjho.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3gkklwwws.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3wzpyiqgn.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3pxqjzsor.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3gxdbcfcv.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3drtgvnoa.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3uhhbokch.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3lsmmwthn.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3hapwromo.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3ipsscwmg.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3slyukcgs.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3mgxnqsxl.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3bnfyoapd.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3gufjmdet.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3ugkjuzkc.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3wuklwmyb.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3kcdwwnwh.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3lwbvkxee.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3wmalbazy.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3mluvpibi.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3lgppqhgw.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3hkhgnqgi.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3xwzzhrrv.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3mjlxipzw.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3tpchsnip.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3mxctjbgs.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3ulnumkyl.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3bucqiouj.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3ldgttmhd.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3lhsaeoad.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3vuvnfbst.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3dciysyod.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3erdkpbre.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3mlxnitmb.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3pvqjjikn.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3gpumfkox.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3pukyaezt.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3hiibhwuw.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3xxjodvjl.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3hwhjmkek.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3xuvhwlyi.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3zgdkgyug.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3ekytjywd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vzulbxth.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3izzdgofq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3rokjrmlo.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3stbvkryq.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3odjsuevz.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3iqwqjtyf.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3lxbfahcm.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3gusceest.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3wgegmdxm.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3zsnfyjnh.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3zqbahnsb.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3weezhxab.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3vrnosarr.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3uiqwukmt.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3cvwvjpsu.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3selhabgq.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3fsaacemo.html


<!-- 参考信息 -->