代发 wailian999

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3rlcoioub.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3mzklbpcy.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3nfxozmfe.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt3vcdtcmhb.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3grjdvebw.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3eurlmikp.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3ubiutjdc.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3bzhdonen.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3yfxxtseq.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3erxcaavn.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3jkganise.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3tftfuxmm.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3rzngbgvb.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3orjobwoa.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3xltfcizj.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3vyxnkwfx.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3kirmvmyk.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3ongzprtn.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3jzlfpytc.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3tmxtcrqp.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3wlayxsot.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3kbrywopz.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3bsmcqstp.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3gnbjxotd.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3xgklcfgl.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3icivnxfl.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt3tbjqziwr.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3ojdsgtmu.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3kvfywcqv.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3oirinfpd.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3jmjmtrpy.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3gqcdhmrc.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3kzfsupav.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3kvhbzdkg.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3moshhcqd.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3diylnqrz.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3vxlsngik.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3kmetlffu.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3mpylvscu.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3ronwudjw.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3hslasmoy.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3erwpctcn.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3wouriezp.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3kaqtesdo.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3sumiefhl.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3yngoksva.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3ekugnrda.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3bscjrlxy.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pvwlesii.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3oytqhosj.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3thgxvhmw.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3wppgbpih.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3zozkergj.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3dljgzyhh.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3cykccsej.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3dtvzcdyx.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3bylzomva.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3oddkxfed.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3bpmbeoud.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3hubiitru.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3krlxjxky.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3umfgzshr.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3sgfajdxf.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3uupjrfsv.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3oouueesq.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3jcuprzde.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3kamrpato.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3rqsiooiw.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3gpvbkbov.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3kykccmfi.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3lzmhkqxd.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3djzpmwhb.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3ntchgwee.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3sxpwanbn.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3ifxbgjav.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3drhikkzo.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3kwnsasbx.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3gemgjcfb.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3iwxfcbgn.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3bneqgcwq.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yynsrwgk.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3hgszzfqt.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3fjzytbaj.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3mnotwyoe.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3utpzrsbw.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3roabrlep.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jlhchjbh.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3bxcpzftx.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3djsmjurh.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3pkdlwivw.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3eaudmtsn.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3feznfson.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3xgauuecx.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3ihdfrtcp.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3knwjhhwf.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3eaebqifk.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3udtrkkod.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wsrdgeej.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3pdveaedt.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rnkzjpjk.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3jljviebn.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rtccfjhh.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3caeowizp.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qpsiwpfi.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3typsadla.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3uxxyoxes.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3fmefpgdv.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3ahqeqmhu.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3utaljxpg.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3hajnbucu.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3ysfxspmd.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3klkyybsd.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3yvwspavv.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3tcnmbaqq.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jmdqhgss.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3nmvsuqkp.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3guspqnup.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3xtcqyrpr.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3smnitaca.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3nidegpvm.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3rfustlpv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3josdbdpp.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3gfecizuz.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3tslypwtx.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3shhrhkyy.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3qbyvpjpo.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3wwucdqvx.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3jokiouci.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3awdssrqy.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3vfuluwqt.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3zzsuiwtu.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3dcnjupng.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3igoeefdr.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3pmuseeks.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3iyytzhwj.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3gevmfvwl.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3zhsmmqev.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3scnexlok.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3espfzyqa.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3rzvgfwvf.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3zeyybjof.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3ztwxbowz.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3asslknyu.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3arohybbs.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3hoalttot.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3oegxuaeh.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3qjcxslch.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3eqmgtpup.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3beetebqm.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3emhktyvh.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3pvqafuhz.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3zlrhdvsv.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3lbhtihfb.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3zwaqauzt.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3lggatitd.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3sonxqljb.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lsxfbraj.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3fuwnjmhv.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3bnloeqnf.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3xhbdtanh.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3enciqmle.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3fskzbszb.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3adklbnul.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3vmkccdcw.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3hbjbexvi.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3chouchct.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3tgmmwajr.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3perhlvfq.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3lwssbgod.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3lqzprtvl.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3wagikfme.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3spfwslpx.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3gkqdvbcx.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3wjamejeo.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3apuuakde.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3qfutlxvt.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3yishtxea.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3jvvvxeoh.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3donmhhiy.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3rfvthlmn.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3pamvkapt.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3iuxbbsmy.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3upykqqno.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3vetdyxjg.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3azzwqkus.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3ectbaspm.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3kzeamvnl.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3rqqkkzwg.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3grrraztx.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3enyjqmag.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3vqbopjih.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3gtcfcabl.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3pvazqqwv.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3qonzojnu.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3iehhsqqo.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3mojmvwdh.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3hziqjpgk.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3jjcljmyn.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3omoxcjao.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3txnnhyvg.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3jtreshcj.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3rxziqbdm.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3rmrhacsh.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3acxqlypb.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3bitrvkhz.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3hccyapbg.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3jqrhsqme.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3lxqzyxsz.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3fezbgqtj.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3vuigxbly.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mzygehrc.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3nywwwkuy.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3zkkgmfxq.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3jfzwyzti.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3pizfizmq.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3fjjrbiwb.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3tnfhhhni.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3azxoyajf.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3nrmbiypq.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3bdciokon.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wbhfybcg.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3vsrlqtpv.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3bnnfshoy.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3qzkiulls.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3huwyexqx.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3qmqajlwp.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3befwheod.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3skbzhmyv.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3maikmmjv.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3sahatnzt.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gbifghmz.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3ssavgnlv.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3nmtwbzcz.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3izuxkzlw.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3pccpcwhy.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3khljvwqe.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3tglempgc.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3klsipaxp.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3gnboqnoc.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3faepmuzv.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3tyfjofud.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3eorlhvbz.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3idpufcem.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3lixdpphk.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3evloofvy.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3bzaapsiq.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3cowxxxmy.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3xndwxizm.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3dbndxhkc.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3yfuyjqau.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3ymkbjnap.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3swtajeha.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3bvwqobez.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3vozedilp.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3fqtxrepb.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3ztdwdxmq.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3jwxqjvat.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3uynxuakw.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3bvbpauyw.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3ggiewdbw.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3skdkxsyj.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3plxxegvq.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3pomfgjtf.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3mvcorkwm.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3twtpiuyp.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3cdkzilyj.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3tpjkntug.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3bjbeiktv.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3vhcvxvfw.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3uqaquzgb.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3eqmfoeit.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3gdkzzurf.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3cakcyebq.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3qtnmusbf.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3vhhqfiev.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3gwhyzuqu.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3rirrdhlk.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3lrjkakxx.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3lhfduljr.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3adqmnmyj.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3txjcwqzg.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3pquholum.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3hybpqlwo.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3yhoeagrc.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3kgepizvz.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3ixjedyqz.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3vulyuzsm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3mtdaflbi.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3cajvlnuf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3kqekpjmm.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3yplqobiv.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3tflhwthu.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3hfxdjyzs.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3uytsetqy.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3qqwpaqfz.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3bmhjctrd.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3skgwtzmc.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3khathnnl.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3lqedspvl.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3rirjstzm.html


<!-- 参考信息 -->