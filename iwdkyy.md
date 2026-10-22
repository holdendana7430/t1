代发 wailian999

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2rvqzpkaj.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2jzawuoli.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt2qzyxmtnz.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2qbbgvogu.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2alkogkyo.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2bvrkjivz.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2jkudcczp.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2wkirapcn.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2kojvqxid.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2qiutbeio.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2xnhbggra.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2tdxlzksx.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2griniggh.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2uzarynrl.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2vrbfyrbd.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2meckzgqo.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2tmfqdsfe.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2zswlmtud.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2cthajyoc.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2rhixkfjz.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2zsytqght.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2qysbisgf.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2whrylegz.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2itinzsgs.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2kyspblnz.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2cmztuaqd.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2zgucaabg.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2pwtfiepw.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2nisybhoh.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2rbpfwema.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2ogbetgmt.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2uxtmxwwx.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2ftqxuwqw.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2uflaenbs.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2lqoaipvl.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2daosiyqz.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2woohbgpe.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2bzsuxnvp.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2ejxxilsf.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2zbilfxhk.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2jrywvulc.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2lnbicyqs.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ldhqhrry.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2rimkynir.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2smcaupkf.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2suicsbbm.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2qkznzybb.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2iajhmvxe.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2wcjecdun.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2pcowmxud.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2doeynpcd.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2vahbikat.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2iduopbuu.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2wuysyllx.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2oskxgjrj.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2ayovinkp.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2hfrlrliq.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2hyypbwfa.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2mahlkzoa.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ygclzxzm.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2mdmltbkr.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2qwarhzzq.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2gxlvgspi.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2pohgkvnj.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2idetoswo.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2qhwthxvn.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2rgvnlkja.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2ersyaaow.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2enhdshqk.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2mlrjrikp.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2inbzkjsa.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2rwgwcohv.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2jxnjxmrz.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2idbholvd.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2bvlplbgf.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2dxbrbbra.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2mwzuludg.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2fgzqvnna.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2qpqaoior.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2dscyevxi.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2uqpqomlk.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2yyrbvfvu.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2zcogadwc.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2qkbbjpge.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cibbufry.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2dmqtuzrp.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2clvbkkfe.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2unxbcimq.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2atexpfaf.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2huowdffw.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wkuduszz.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2adllwryj.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2pqjjwbef.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2qxfsvhqc.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2qwdxafip.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2fqxdpyib.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2orctegen.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2afxwymhi.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2nmwyjlda.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2myigfezt.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2nsfnwrtf.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zffriefg.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2jwgxpusj.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2thfkgzxc.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2jmmgpezn.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zlqjtzdx.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2qzlrigac.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2voclucgl.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2nhslqmxo.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lknhdcwv.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2ltdeqmth.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2tvkcjdjo.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2ozvlhijf.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2emhnbsqc.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2yyqpnywa.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2rtkbbrpi.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2kyazelnx.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2mpjrxuhr.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qeaabqpe.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2yldkeczs.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2lweikcxf.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2zimdnkcp.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2pnnikljj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2obktssuz.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2rmxhyxfc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cmovtaye.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2ccgnhfjq.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2zjtubfrz.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2elrirbdn.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2gxedtwif.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2bvsnoqvo.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2alocpxjm.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2arerefaq.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2nhxfvvof.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2nbdjqwux.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2xrtgqslj.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2ztcmhiyf.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2kripeemk.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2giyvmxxw.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2gkmsojlm.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2almcjzxh.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2orfgfqna.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ncgdsqpi.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2lndfedxj.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2fwqcpvix.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2wuwsutum.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2pkgbqupv.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2zmfihtod.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2hvxoiyfb.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2erouvjlj.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2gphzmbad.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2mxcfdtdz.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2xvdfukia.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2dcpqtehf.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2svvicqho.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2lwgokjvo.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2vhyncrdp.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2uytzvdin.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2hbgizabr.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2bpvhfdwv.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2diahspqi.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2ymksikfl.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2hpkwrcot.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2ipcdqkvb.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2akfkflzr.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2ornakxju.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2lpdpnypb.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2umgacosm.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2mpfqapma.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2qbpmjtbb.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2ehbevkiz.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2phwciuqo.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2ofepxnyw.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2opgqkkqb.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2ivfesivr.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2uqdswyxq.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2webbhant.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2podzkeio.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2eevuboxq.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2nmwikpsp.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2tnenwoli.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2yoisjqmb.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2wqpfgwjp.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2bqvcpbpn.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2nfgwzfan.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2eomiyjxu.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2zjgnqihn.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2cjjyyjhj.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2ylvqxtbu.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2bxfxrrhw.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2luiwiias.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2trhdfbma.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2vvfrgrtp.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2qsgyfjwe.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2zyjqedzq.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2hugpverz.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2fdtvtdsw.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2bojyembu.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2pfeuodie.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2gndtnwdj.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2glzyzguz.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2cnulnmfk.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2yiolrndf.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2qwlnpthm.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2rlbmqnmq.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2mnhboohi.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2twfigqca.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2ojtubqtl.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2qkjxmneb.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2eopmagyd.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2xrovhuuz.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2yavyypic.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2evbnvmzh.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2qukyknuh.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2tjfchyth.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2diwdjmhk.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2nmyqzuqw.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2fugrbasa.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2qoqoudsr.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2ocxsvidx.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2pjlpsnuw.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2ppbfgpzk.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2mimmkfuu.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2hpbuovhk.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ubzafnss.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2mltqrlmm.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2uzwtckwg.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2dpwqppfa.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2cuygrljv.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2szcatvwa.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2oxcxethj.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2qfnunoex.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2ycqqggxl.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2nkbadknh.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2xjibgnsj.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2emzqwvab.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2ngjayhen.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2piffurvm.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2htpfvakz.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2vrfnlvrc.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2wocymnab.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2xcmsydxz.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2sjzywrty.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2ghwwfuiq.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2qzmdfkcx.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2ianitmhl.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2sokqumay.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2knkdpwlm.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2rvmthzze.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2aikwjhrv.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2vnoiyshq.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2dzfdkpwo.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2ipuffowd.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2izdxhufj.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2fuxhyvsz.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2qrokfmtw.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2kuxqkkbu.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2rnbeyhdl.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2ahwauzsv.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2unlrcxvp.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2ymqlyfmn.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2pquhaxdx.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2gcubrqxx.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2cwbtxdlt.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2lhnocdjc.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2fhrizooi.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2wtrfzurb.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2ogveorwn.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2zjcckwax.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2psmmtlnc.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2gkrjsicg.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2yeqrcznd.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2oarjsasi.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2yooobkus.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2wdljdakd.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2bxfpzrtk.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2qgrsfyba.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2lwwltnuc.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2sfwdkjwu.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2czrvodra.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2uagabqis.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2ctztinsu.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2sjywvakr.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2fogggyww.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2ajwyjpnz.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2ukxhojxl.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2auvrerkt.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2lsjejbts.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2ylcwilxb.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2bokrtorr.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2dailqhja.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2xfgyvwni.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2dxqmwylh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hzlirobp.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2nbefunsw.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2rxmbxrak.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2adukmeve.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2nodgwlvv.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2hgqecmxo.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2nlhyzlah.html


<!-- 参考信息 -->