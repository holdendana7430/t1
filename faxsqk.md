代发 wailian999

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2hkbuuwob.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2azwaceuz.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2bveayllw.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2hyusskjl.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2owfomrzo.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2woxjwcpg.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2yxnghpsk.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt2gkjpqsrs.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2bvbumrat.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2zhcssain.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2ljzwbbuj.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2wilqcwsd.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2ebimsrtq.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2cnvtbvvu.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2dpivultj.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2qlvzeqqm.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2refqzkat.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2kmnfrsyh.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2iivtezip.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2bjszkjdb.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2gvflerwf.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2tctjizmu.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2iuiidwgh.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2pbrhilot.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2maoufqwj.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2sopmkdvd.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2kwiegrux.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2lxdkqyuv.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2wbvxmhzr.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2hymwgkkr.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2yyszwywc.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2izkpfvju.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2xefnhhyq.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2znqbiqou.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2gkjyzttc.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2cfgewxwn.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2viiorbkk.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2sxqzxqfm.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2qbwwpdsm.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2hrbicozy.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2ggnuubkp.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2nrcfqsjr.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2xaxeexmt.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2zyzlwwha.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xuevcqrj.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2cachjqow.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2cwyhmvzw.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2snrewgeb.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2crpjaymf.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2jucehazg.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2sincasyi.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2owkyoghu.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2rgcjddul.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2lmvnkdvq.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2ugzohjes.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2oojidnts.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2deqkqwfv.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2zsmpuyho.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2oypkkylb.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2govetyqc.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2rftlsidd.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2wlbtyqrf.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2qqaqdcoc.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2hnlgccur.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2dpaasyzc.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2lbhubswm.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2nggemumh.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2pgerrkfs.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2glidljab.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2rnemghmw.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2mqvnyosc.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2howmqhkk.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2fhzfixbt.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2opylrjxi.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2emtoocbg.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2scrheult.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2korcnzsk.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2cmttzetw.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2wnydzotu.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2mynkxeme.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2hpiuojpb.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2zjdpihdd.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2xfpkbxde.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2tyqndhcm.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2zltaxmfo.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2jopwgtrs.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2zbjrrkaz.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2fjlapxeb.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2jbeddhhg.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2gzjfwwrf.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2nulqqaef.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2nnzseqii.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2cppgunus.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bxsgsdnr.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2ooaaetqh.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2skxwcpae.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2xobcuxvr.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bzdoyynd.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2icusnkth.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dyojsigd.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2kzggqgjk.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qfpaecql.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2shmsvesd.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2btfwwnxb.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2jrvozdaz.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2jzophnni.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2egdojnic.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2moiooddi.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2eavfxuos.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2slnpvead.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jsewsszu.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2rufehdxa.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2axmkyiot.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2jswpmcjw.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2lsejycbu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rxmgseql.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2pyggjfwc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ihtuwiwc.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2nuioxbpi.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2ceujhwon.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2pujatdgu.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2gbzjjefv.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2ylbcrchm.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2qlzehdzr.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2ouubcigk.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2syogeppz.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2tjypvvid.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2utnpehqg.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2guuxobjl.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2hdwtrtys.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2atbvvjpa.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2oplgelid.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2alysrufh.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2oibihkmh.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2daksazas.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2iuyzrayq.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2dyqzvvbq.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2xgmechli.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2iowzgxkq.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2sgawokem.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2ficrzrrw.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2wapovmfx.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2idkuqgzx.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2cvuqhnvr.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2hyoruqtz.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2boaiyhlg.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2qgpvfqhn.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2vufgniwj.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2gifwcbdt.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2zsnwuruq.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2mshfmpxt.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2dykrfxod.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2aerfhcin.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2wnlxoqwj.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2mbnicocv.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2lcgihoov.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2bviziplb.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2shgavxzd.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2ozsmtsao.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2lbjxronx.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2dykebitt.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2qubkmobx.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2dclndyfw.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2nohcsblt.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2ymlpsnxf.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2iescwabu.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2gyvayqxk.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2citqcsmq.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2uujzmpft.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2zeknfeln.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2papwfien.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2fpblaicc.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2msmoloeg.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2eupcyqtw.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2nnnjdmma.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2tfzjhofa.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2buuwioze.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2kqwukhux.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2ktuddgdq.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2svzesent.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2dtxclxsz.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2eotgrrgn.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2yqelrhur.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2jqtbkubg.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2wdumymbw.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2aqthtjat.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2feafjduy.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2jjylkpen.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2knnmpkjw.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2eawllkuj.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2qkfqvfgk.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2tlhjjswa.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2jahtotkf.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2qvfphpvj.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2mqvjqrwu.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2hikpzrud.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2eyxbonro.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2dplonmwn.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2wdjidbtp.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2wtccgwbn.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2jgaxlvdc.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2alyzbdri.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2bhboslbp.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2bnocpwrb.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2wdkpvwrs.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2jpmfsrjd.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2coaofack.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2pfaxbybd.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2fywjcybk.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2rexnafee.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2ebobtqno.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2verypfsc.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2ktcebyuw.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2gyxmhyll.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2qgummkau.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2arajsuvj.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2klevuhyv.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2agwlbtgg.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2snfgyrln.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2viiacbjh.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2fmlxtcoa.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2yokttlbr.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2tnwpcwct.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2jepoeyef.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2rggbfrxq.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2rgsrutao.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2kysoojws.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2rmjhflch.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2oqhvnmsj.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2rveeyamg.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2oqizggso.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2dmuxskha.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2ddqyqotf.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2utolzasx.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2spjjoksv.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2gfpulihg.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2iwagspkg.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2pgcvgeft.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2txolvhie.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2rqbsvsfj.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2hqzobifp.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2pfubffny.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2vxqzncbg.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2lkpfoogt.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2auavkwni.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2nhalfnhg.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2jycrpueb.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2zpiuxmbd.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2ohlodeae.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2vqnscdjz.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2iaqyiazn.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2fbbstpbx.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2pqjxhjug.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2ulqugifa.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2uraavkds.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2ddxrhril.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2rhocgann.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2bnfngvye.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2gtmgchkj.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2endcuvbt.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2bktngkbw.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2lcqcnfoi.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2pfocrmfn.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2cmsftnmh.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2phctjqis.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2citusrdo.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2rcgzsoij.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2oekbikss.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2gphzglwt.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2noqitafl.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2xijvhkkl.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2foekxfwo.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2xcapuzzg.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2bovzfklq.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2ncvlhkgz.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2irsmfacb.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2kcucotxs.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2pqrsxibd.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2pxnvgmzb.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2mfcnynxq.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2ibqhtarv.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2ulqfegbu.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2dxgrhjff.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2izkrohae.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2sqvmulky.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2gpbwimxa.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ppaxkprx.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2pgmmfzrc.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2jushasxl.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2kjmugwfm.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2gwlmfvbp.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2vwlpxjtb.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2wgfrcyml.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2yosqaomm.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ldohsqjv.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2xwxxppkg.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2wmxhmnoc.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2yymwguee.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2vrapmdzf.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2wgtmpcch.html


<!-- 参考信息 -->