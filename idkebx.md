代发 wailian999

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2abxhikhp.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2zujcjahf.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2nntmqoqe.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2ulmfavsg.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2dvzmzcyc.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2lbpywywr.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2kkqgdspd.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2hijnduuz.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2jrikxnvq.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2bssqjvog.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2bjhafrni.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2tviefezd.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2pmyzbcah.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2huywejjf.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2ijsgxzrg.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2xfeqexcb.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2lontlrxw.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2egaipikx.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2glhmtgtz.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2hwzwteua.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2lkquibsq.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2qolnxhxi.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2ibzoshsn.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2ehdophej.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2vlvqurkl.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2hvmojzyx.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2dmmominm.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2fdeyiuol.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2hittatcg.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2oyynnehi.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2vaoybrxn.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2yvjvialf.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2qolijuhs.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2mihhnqal.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2tntpjubk.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2gaxlvqhh.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2acaqjjoj.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2dlgtneof.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2nlvapndl.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2fflpbxma.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2qpkimwlv.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2abchbuzr.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2ehnletww.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2xtkwcfnd.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mtdeijry.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2elodwfax.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2njcgjxtq.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2ndsuoucf.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2mhehrocs.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2frgrdncb.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2junzxwex.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wtabhkje.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2oekyhbqt.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2jupeiwds.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2zerddmjw.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2vhwysjdg.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2tlqzksbe.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2meteecyn.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2mxtjcpbj.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2smtcwira.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2dfuejyvi.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2shdeaymi.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2asjynlwn.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2qkqcdoxe.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2gpxscyna.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2riuxmpml.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2vapqlwrl.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2fyvcpmhn.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2zdfnpmwi.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2cevcmicr.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2byiaykct.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2mdtauxjk.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2qgvgdlik.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2xoripmxy.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2qqygmend.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2iponikqo.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zevbeulu.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2srlcbhii.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2ukwsuwnf.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2etltomqv.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2qwwgkgnz.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2qsobyotc.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2txtkqdkx.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2teheuxic.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2ppvhkqld.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2tvoidqat.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2flatxghm.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2ampgqpuj.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2rbfodaah.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2jspvcqjw.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2buxeqdgz.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2yihubbkn.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2jigpwbhi.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mgbaagsv.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2ygrpkcnl.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ghjpmnoi.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2mgbuhrji.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kzwnijnf.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2evafbeyv.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2muewderi.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2pilqpmek.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wnopsdwn.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2xedlbjxo.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2imirmorg.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2nmhmwtjv.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2dsrszlih.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2wtzgeiqn.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2xuboafvr.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2wcmnxman.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2ephoappk.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2krxovbwq.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2pnslktmn.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2dxhbspoj.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2jkzbaqiv.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2qernhgso.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hozsgmsr.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2obhtwclm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2lbrduefw.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2hniiffiw.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2tlltbzhy.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2cpztcufd.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2iojhglpy.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2qlfrhquq.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2poefsvzl.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2dnrhstgl.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2owcwqxoj.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2qfmrnabq.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2cuswfzqj.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2yugvrbxq.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2myusxugl.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2utaiskou.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2oqdbmcbp.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2cguspjip.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2inrztjqd.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2axrpaont.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2glupchqj.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2btzuueby.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2iawsxcyn.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2scyvvgkn.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2keazhqmw.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2rzyuxyov.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2msoqdvkk.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2pgypvzfi.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2zxdrvvqy.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2dnrtrrnd.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2yuxlormi.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2nvofplts.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2jbmxmeul.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2dfjomkaq.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2ekvtsylf.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ouabnpqx.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2tappebmg.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2pvghnfgj.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2progafkt.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2bqdrzuds.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2eleyuyza.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2xvutddku.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2umwsoxdu.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2qinfodlc.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2lbukfloi.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2aavfdrsi.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2wxiyzswf.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2klcimpuc.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2fkrxinsh.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2cjuijfpz.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2ogjxajwb.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2jtlvvifq.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2vxtlumbm.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2vazteoua.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2boqmwqaz.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2tfuvxcyi.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2vhhbaqce.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2iolpgjxp.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2gcwalcrn.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2ufwtytrb.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2ohddkvts.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2omtgmvga.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2qdorohyo.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2pgbkdtqk.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2whihrccw.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2cmeazgbg.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2hvspfnwk.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2ufdhxwyd.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2pyboirvd.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2afysbcqz.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2igpxrtej.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2pzgjpfdh.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2qlcppacr.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2nmniwsst.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2mukdlhar.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2yoxzbnri.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2hqeluruq.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2tjobcimt.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2zvkageyt.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2izcilhbc.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2ibynfpda.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2utupzijc.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2wuqwxkpu.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2gdoamqhc.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2etdfjhwp.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2hmwfymqt.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2aakpsxtr.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2sevmmvjt.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2yscadkuw.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2vkoocwzm.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2lfursnxg.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hchlsklj.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2kgxxskth.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2ocusslqq.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2hutzeoeb.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2mneotcds.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2ojpfprdv.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2vwhxwnef.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2rhszhhkt.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2sbldosko.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2vnmyvmth.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mlfokolp.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2rrybkvkv.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gesbnmml.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2dfmgqwcn.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2nmdbwnmi.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2xufopcng.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2mjuzxerd.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2gbuuthlq.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2kqtneywn.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2aczrpxtd.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2luqcvkbp.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2rzyvdmlh.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2afepcdel.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2cpxeavho.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2iggwrxwu.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2jgglwdlz.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2btnjuipx.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2bbangebw.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2pzczaeaw.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2sdadpons.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2cafzlexn.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2qofmxxuj.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2taarzaac.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2hspmkoch.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2aixjnjrm.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2hgwltdjl.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2cfitgtbj.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2wmmrrsvl.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2uakhuwba.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2mhszogku.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2qnqpzjet.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2kjveqpex.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2rsfnisxq.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2dpisggti.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2dmckafaj.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2mzbtijyb.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2tabiznku.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2byqpxpnr.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2xnwzwvaz.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2zgciszsa.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2hwejinmk.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2wfyowfjj.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mlbogszf.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2yoynwwam.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2eaboofbm.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2xbpbzybm.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2yvhbpzoo.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2piedswhb.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2fimitfwx.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2qsffrluf.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2gtkpcgio.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2iwjboqzh.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2lesfjkgn.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2dmxlstmv.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ugwbxucn.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2qbcnlgvo.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2ditxlvah.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2upskxmre.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2uesbwswt.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2etxrbjyw.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2uohgaatp.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2sdwgtqor.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2etnldcxr.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2vtsworyc.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2kjwtrptj.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2jpvwkxgt.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2zgsiarwk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jrlkuvqy.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2ggdpecni.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wmexaeaj.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2scojhuiv.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2qurvmigb.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2lsbyncha.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2vcpanisd.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2ctgqseyg.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2lmbpjiok.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2gqvsqkaw.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2mdahiyzn.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2xspcziln.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2dwgpfgqy.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2ejetqvan.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2bfbccmft.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2ewgosqkw.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2fuurvlbr.html


<!-- 参考信息 -->