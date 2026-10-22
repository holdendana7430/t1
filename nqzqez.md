代发 wailian999

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2npmyrjbi.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2javpnfql.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2iugnrucl.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2ltozgcvn.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2qyviypva.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2eoirbjyk.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2eqqzyjmn.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2schocelo.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2juhazico.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2wdgwdjfu.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2tzkfgxbj.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2njafjvwf.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2zucldbhr.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2tcbqmngr.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2ixtkfdno.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ocqfmaqr.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2imddrerf.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2lvxasvqc.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2vmfpxvrr.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2ljslejtp.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2zmjviqrx.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2ockwdvyo.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2wanzghbp.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2hicskmwu.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2lxtuvpwg.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2guqngaaa.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2parxwjwe.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2lskwuvjs.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2gwgqjcgi.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2fxbcawzy.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2mlxlytjv.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2izphkqmx.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2fnihvjaw.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2sgkzlrxd.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2lmmfqfcq.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2ycxuzqdt.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ubljzfac.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2djfzfunf.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2lwnehbcn.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2yqtonggl.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2zialhqys.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2dveatwnu.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2qtmtnesl.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2mubkzowj.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2daixmjvu.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2swwjrddt.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2okftgzhd.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2lylbcaxc.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kpfcfdmy.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2xvbwzkfl.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2kdayaopx.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2pqqtczuc.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2gllvjwuy.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2jasdayba.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2cxkauiaq.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2dwdlvltm.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2xbfmhyhs.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2bohbyofv.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2sljwxoom.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2ihxeidsb.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2xxwdzqjf.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2csmlzeqk.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2hvuydjcg.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2hmtwkqjf.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2pvhwylcv.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2fohierhy.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2rzfrasgx.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2vsqbqfso.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2qzeshgph.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2exebyfbo.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2ukzhgtsa.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2aukpwheo.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2oocjgafp.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2inwzynjg.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2kythegyk.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2kelzqmxr.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2hxixhiyb.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2bbmtkqqu.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2cuwgeole.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2sbkvwdqz.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ffysefwb.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2tertajcp.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2lqmgjdic.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2vlulrujj.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2pkrijoua.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2nlgxjmbq.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ffbdpdpa.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2ahfnuyqk.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2cmivczie.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2nvukdjdg.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2rktsqbme.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2xxcyojzm.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2krgraahl.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2tevlpuls.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2bvuwhmbi.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2rvgzhmwf.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2ampdcofm.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2riuknohy.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2znlrxpyi.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pyuyuith.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2londrktg.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tnaejflp.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2hxsdnmsz.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2waqhmrcb.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2yvmtsema.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hdbitguu.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2hoxpkwob.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2kyzvkalr.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2wxvnusds.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2okshyxki.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2yvlakwhe.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2ulyzidoo.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2cvezzhth.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2dbsroknd.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fvhhnpje.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2foltroqn.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2baxdmqjk.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2afypkaiw.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2valpqsqq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ltlusdqs.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2pnauyepj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rxzemrfq.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2tgbfqjqz.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2epjuflja.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2bensoopm.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2jupgfvog.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2osexfwrc.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2tnbcginy.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2esfyuxwd.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2ohteuned.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2mqdbisqg.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2qbmhfvzq.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2zoktzlgq.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2oxbtipaf.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2ecyttstq.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2uzfpmnsj.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2pjbwhndc.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2ynvjnvds.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2kynwcnmf.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2bsnnsawq.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2udluljts.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2ddrvoyxa.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2ylqgxseb.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2keglilgh.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2fricwpic.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2xlbcxkto.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2aadiqhzt.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2csthspru.html

esac
来源：http://www.52xcode.cn/Article/details/gt2iseqksus.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2oamckzga.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ihjnfdjc.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2ntqgiemi.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2qdmybswg.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2xworlayu.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2fvvonktu.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2hzsrdyxo.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mrwokygs.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2wkezahid.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2qbqogjvd.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2xodrades.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2brevolbr.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2fzxlfqex.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ahtiuooo.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2ijnfqpri.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2malhhayb.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2meezehio.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2skcrcjmp.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2nlbiwxap.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2kuzszdwv.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2zipxfmqe.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2rrlqwjrj.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2rwqsswpe.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2lqwiiqfr.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2rbjxbmnn.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2ppjwjybd.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2pwbhkinl.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2okamuxor.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2hmxrozit.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2uivzmuvw.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2sxhxspaa.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2fijwfrcb.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2llvywhmm.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2mhanwtdx.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2kvygscif.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2fwvmzynf.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2cqyxdjht.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2rocutxfw.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2jyepkilj.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2okiwwjce.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2vezjnphz.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2tfkezwlo.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2hmtcojnu.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2fkyxvpfo.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2qgslyuxw.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2omvqqkwv.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2fkoktnzq.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2lbrqkzsg.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2rrovrjdj.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2dizeimgr.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2wsuduqla.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2tlylegdu.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2bnmtslah.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2oduogzus.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2vkmxiuvw.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2rqfwuaem.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2zwozkhui.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2jmohroxb.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2poltrpkj.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2cpfyxnaj.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2kotwjekm.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2stvhfsxc.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2cprcjbwe.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2ibzrybza.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2ochudhjg.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2fytrjhea.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2dvvsvyjt.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2idznlvup.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2gzjcxmva.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2pchliekj.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2kynvedaf.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wbamfqoc.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2vtljlomy.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2qranssob.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2jadpztjv.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2eemugcyn.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2aylncvtv.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2aqzrmzat.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2zcxrdmxr.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2baxaesqk.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2nesadslx.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2lzelnazb.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2ljufcfjb.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2cbtepstk.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2juykwvyb.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2kpluqdtv.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2hxrjikkh.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2nbepbavp.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2ovrtzdcm.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2venyvdge.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2jssmxksu.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2ohcxpgtt.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2fwfehasw.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2pmximmdp.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2dpynhksy.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2pdowmrfl.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2ihqmvvmb.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2wakicsjc.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2kvyutsgq.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2oukzxpdg.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2mitjwejo.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2nhdewnvu.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2yajtijco.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2ljpvyxam.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2fivrfsnm.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2zmtpgsvf.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2cjwmshqx.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2zbswzkoz.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2xfcqwyeh.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2nabetspc.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2afwsforj.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2zpjyekst.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2ibdejugw.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jpuebdkd.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2kxenlvre.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2dobedzzh.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2phzhqccj.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2pialvncs.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2htofkvwg.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2dgdxqddc.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2eovwmujh.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2jwfyxmlp.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2soyisunx.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2vqguffyj.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2zovcnbnd.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2llxxcxoe.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2qdmlgjdb.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2gskigxxm.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2jqueacqi.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2bqcqkyot.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2gzmfrdjx.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2abtvwruz.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2zbcafztg.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2pohdyrop.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2ulkfxfum.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2iqlfrjmp.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2ldxhomyt.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2twnqzomg.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2saoobfgn.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2nmnomlbv.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2krfpkalj.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2glehlxlc.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2evvysous.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2clshvbjb.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2smhrucxd.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2xjqiqbot.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2pbqkbyvk.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2yhvpxsfk.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2tjwbdgpw.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2uaeoslkr.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2ztbyoosp.html


<!-- 参考信息 -->