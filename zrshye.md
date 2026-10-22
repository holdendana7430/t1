代发 wailian999

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2ueratgbh.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2bgzwsccq.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2dkprrlah.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2ddncqqvn.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2zzmkbswo.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2zauioeob.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2qqpvzino.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2zstjtwwx.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2uvgvheat.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2oaiilgqq.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2empodchq.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2novjjrrg.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2scffgmdl.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2wwcnmjem.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2qtisoynr.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2qgvzpnzp.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2hlqjiaqx.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2ltzzlyak.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2vloypjiq.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2xzpvguys.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2wftsotgq.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2vnkzkqhj.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2qfzcgajn.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2rgunlyll.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2isyqlsgj.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2kjkximfp.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2ygjradsj.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2vesjvcaz.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2fwlueqla.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2yztyvvfb.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2hthutrbd.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2btfiffqc.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2dxkimzww.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2ultszcva.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2snlbxkfs.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2pyzolgix.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2xciipehs.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2kzhxfuwj.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2xwmstpnm.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2wzzoejlr.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ekzlkynv.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2nqfhqjyj.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2pyihhril.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2zxhcjsvm.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2jhwdudhe.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2jtsgderf.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2tczdnuiw.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2pjnqzemq.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2iulmjple.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2vndnmlvi.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2tvqjwnpq.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2dknyuqas.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2cuwapuej.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2asrwntfs.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2cqamauft.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2mtpguxlg.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cootokgy.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2alxnpiar.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2vwquhfdk.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2dyavhtwp.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2svecnozd.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2fkcozepj.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2ivblhizf.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2lyblbjbk.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2kfyprzym.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wtbtujwf.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2dfsepbyo.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2bbikcans.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2damksmem.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2kthwxoib.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2zkfkhvbz.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2mjewxedb.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2sdqzcjtn.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2oqujtcjc.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2icjmnfgs.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2vwxxmxte.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2cfaxcwwv.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2krepawnj.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2auerzgop.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2jlehrrcu.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2qumxqjrf.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2cojomxkr.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2fnfidvjq.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2laxwxgak.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2jybndisr.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2uwivhfik.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2jaqwlfmv.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2rtrynsxx.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nnarmwjg.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2yytoloik.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2univqeuh.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2dposogco.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2dlrtiwqk.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2auyjlnes.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2kjrkvnha.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2jemzmqxl.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2snbahoff.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2yhehbgyo.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2ghpfnoev.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2repjmzcy.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2cfpgdilt.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2kidgpzuq.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2xqturomo.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2xnwmzskw.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2xzutcgrv.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2aydjgypl.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2jpfywqnr.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2rreberws.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2mhsfritd.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cayxsgtg.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2wjjzkjzn.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dryclgvq.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2howjfial.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2twelzrhq.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2bcjgmsah.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2zrkbasah.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2gnxirgjd.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2dkoqimcx.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2tlajbiek.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2nhqwkjzj.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2xgoamhww.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2qxcsrmhd.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ciostkag.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2dyittmwe.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2kgklwjec.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2repqhtha.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2thduliba.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ubmjshwp.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2frumowow.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rzidyiib.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2bnkckcpb.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2ykgycpte.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2msjacwcj.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2ufzchjtk.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2nrrjmtno.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2oifhbaoh.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2fsspdnyg.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2rjvhyqfz.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2ebwcwcxq.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2kkyoeyac.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2qucdpddd.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2laoutgmd.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2jraudrww.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2rfogncql.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2tvmuwoan.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2nxgpmtpq.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2igplogzl.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2oxhplwyr.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2gtfjepci.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ghapltxb.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2srywwwhi.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2xcpceema.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2fpbiifjl.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2jgnfdjpe.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2khruobqm.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2aitotopn.html

esac
来源：http://www.52xcode.cn/Article/details/gt2avpiafuj.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2sheeefpz.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2zpezjkdd.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2fwsttbxd.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2kjkpmfgr.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2dbejipxg.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2livmabve.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ycdroxiu.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2astqquxj.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2wavgcnre.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2dvhncfde.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2asocwyja.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2kfeafmlx.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2wqmfirev.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2bqnkzozy.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2cswrckfy.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2sohxvaja.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2uyoonoju.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2kocagzrt.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2jkedaumq.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2bjsqorwo.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2pkwtelvm.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2uusacptc.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2nyszgbjt.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2cnpnqjyk.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2zpnivslg.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2evqzzylp.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2bsaqylaj.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2jfyubdjm.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2llkjdtjk.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2fecwscop.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2gmukcqqe.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2dffeauhs.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2orrsehyl.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2bqruvide.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2zngsejyz.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2mhpnlmry.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2lgpyetxw.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2leajbpvy.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2itsaidak.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2lmcefnnk.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2jwcqxess.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2xetxgsht.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2nktufluh.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2dbapwplf.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2dtgtzivn.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2qppnnetu.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2hphdcbfs.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2nlhyabmr.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2lzegwknd.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2ixakeenm.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2doxhnsjv.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2bdajdriw.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2ygmvrcmt.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2ldplpmwd.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2ynykiwxn.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2jbxrybih.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2txnvsqeb.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2pfiraqrj.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2kqdcqaki.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2zqhrtvme.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2nillicte.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2vxelfxyj.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2qdoibcgn.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2nwfnorsz.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2ykreezlt.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2yznjhpzc.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2zbsjitrg.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2bqhomcym.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2ayqjiorl.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2aaxaxcom.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2ivpchngo.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2udwbvqtn.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2uwozsqgt.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ykvrljzi.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2hwmnruxg.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2kocmarbj.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2ttzchqkn.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2donsmvxt.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2ctkeztoc.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2lcgurbie.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2erhxtjgj.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zlkxjayo.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2camlnweg.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2jrxfrkny.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2vntfmrkv.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2dttnoxsa.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2ijbhsrdc.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2uwiwttpn.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2shwdcucu.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2bpiewwit.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2xfaqpcdj.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2doxnaiod.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2nmdzrqdy.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2lqdemakv.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2roztxzuv.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2xvxgkjjk.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2xfaqoiag.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2cholgeli.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2alqyguwm.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2qxpptjyh.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2rnkwbtmp.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2bqxlyzjc.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2jkhjhyrm.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2aqhlhlmm.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2lawkcgck.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2yumbsspn.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2rmkqtawj.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2yttnkhcy.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2wrlbwerk.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2xscgzlqk.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2igjggyws.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2pydvipix.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2gbhnybdq.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ivddiyvm.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2nskelwrx.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2wzabmjwv.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2tetkdmbg.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2kxfzoyzh.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2asgesyzv.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2ufyzpknz.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2ckotnidt.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2huanrijl.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2jgqqqjpo.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2pncvcgre.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2jmmebfeb.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2muqcjchd.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2miuynnec.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2gcvxuqhv.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2ghzbxkgx.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2mpwtivde.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2yimuaxhj.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2ybzfpvyw.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2qqzvgkfj.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2btdkvqos.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2xznbjsub.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2ztvhjqiq.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2swrxgbbz.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2isvjndon.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2khlwjhqq.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2yfdcojis.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zgfjudnc.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2osquvonu.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2zlmglzdz.html


<!-- 参考信息 -->