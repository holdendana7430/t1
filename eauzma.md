代发 wailian999

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3wiwlrizg.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3troowhks.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3weiupsky.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3hhnyywfy.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3rdayzveu.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ussiixdw.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3qirfuqev.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3sopgpjks.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3fesajowg.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3dkcryral.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt3jfipmlfm.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3glmeveom.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3gocyzsrm.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3jjmsbvfx.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3wllvbjcf.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3esnneszq.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3auljcxtu.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3mnthtzyl.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3enkxibwb.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3xoblvvmw.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3dpiyejzm.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3ihuyhnfl.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3ihqpdgsv.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3esearcbs.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3tzlhkjsv.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3srvelgme.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3edvjpict.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3xyltprvt.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3apqrwegh.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3cntlcykp.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3ubkplvhd.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3ffmebiwz.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3naegejtz.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3luuyasjt.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3cfhbmdlr.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3bswiebmh.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ntxtwond.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3jolkgrel.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3mzhlanog.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3hyduzqxo.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3plnglocv.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3zjwrgcbi.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3kmkbpili.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3czmwiakv.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3oacwajqq.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3chbgxylp.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3jtmofcbq.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3ljuxayip.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3hhefoasd.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3wamhnwdn.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3dltksyvy.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3dkhjwqbv.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3ancynjrz.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3ajlsdepr.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3ostdexxg.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3ptnqcyam.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3sydlfdbe.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3xhtibcjx.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3jejqpmvk.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3tkzlszov.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3pkfdtrgp.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3iavhqwly.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3lowcbell.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3qsydwemt.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3iuvlhfra.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3jnzobspk.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3qzsegspl.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3kyiljhjh.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3qjupalxz.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3tikyhazs.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3bseujbla.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3dbegnwqk.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3ltjerwmp.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3oznprfoq.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3ibdlgatb.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3coufwkic.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3jtmdasqa.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3qbfkekzq.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3nfcerlqe.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3bfwkjpzq.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3rfiurizk.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3drbstxme.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3eysbcqpy.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3tzygrqlk.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3gxwrzmxl.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3xnpjghdm.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3pahrcwnq.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3krzxhuxy.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3asjqdibs.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3ngnevrjz.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3hfucbcpj.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3alnltpdd.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3ldpmpann.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3uwaowmnu.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3hhyoffex.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3vzfugqom.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3fvlfsodc.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3beqnamog.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3iyrafyjj.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3awfsrjyr.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3rvfjzopq.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3xideeutr.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3hushefeq.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3kkrmbkye.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3exfduvgo.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3uzxbcwmb.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3bvijbjzh.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3wvxlxrpn.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3efjuslpp.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3lkjtatek.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3hbtzdhwo.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pjpyyezi.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3hyiqcvup.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kzwrdpby.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3rjtmfyyb.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3xlmybonn.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3rgwvpvqb.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3kwntdouc.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3jltcaxrw.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3igfmthfq.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3stjhtozm.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3ngnitdpv.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3farkbcej.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3ocrizkya.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3qsmdiqug.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3smscctyy.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3fwebyjsz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yddpievb.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3pjxvpxvb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3kassvnbu.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3xdibjyhh.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3qdgylyac.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3hckkmcxo.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3pluplves.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3ffhzueag.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3yyrgyrlg.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3felvrzkd.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3vujbysxk.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3dyqdfgtu.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3nrjrzoft.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3rulhsnny.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3vkyrfjat.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3obirejow.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3yuozryew.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3uulrruly.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3iahawgnp.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3cxdhatwq.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3qnsafdje.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3jvbqlwqs.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3ztguihon.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3lxgurmtt.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3axuzxphi.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3fpvswufm.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3ukfaasur.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3pcqbcabb.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3xkpzwktk.html

esac
来源：http://www.52xcode.cn/Article/details/gt3ohelpptt.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3ufvqoiqx.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3tpuvioqw.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3qaunbtby.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3pyshdlsy.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3inejjpez.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3fkiwdjoq.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ahgnvnfe.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3itvzpsja.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3swhuskec.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3ijhtbgko.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3exedcmcm.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3ukrewico.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3vkovcicw.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3tbeswanp.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3fgdffebi.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3uiqxczxr.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3ciesnylu.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3npezunba.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3prihagzf.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3ulsbfysp.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3zqusbhtf.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3hzamwixe.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3anohkszd.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3blazbiio.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3whnfxwmx.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3baocmpka.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3cdqisvmf.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3ypqnrbjx.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3tofihxhk.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3epznzzpe.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3wcrydnut.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3caifximz.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3xwvcgqed.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3ctdldwjj.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3pltduwwy.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3buvfsncv.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3wxfpgkfw.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3kffvzzlb.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3ohsdzsyi.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nyfyakyh.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3gkqsepdj.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3walfntna.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3jnxchqak.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3qpfvhaox.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3gmqizgly.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3wptncsib.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3heprwwbr.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3mcevmkwg.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3bkneyvyb.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3hxxmqujb.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3cpvyaujt.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3tfabxihq.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3vfefusxy.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3onpfngtf.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3nddlrbeu.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3urrxyete.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3nafnxtjn.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3asivrbii.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt3fziytzxn.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3nqxfhazb.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3lgfrisgw.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qpngovvd.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3exntmkes.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3fkfwjdwb.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3qfkthytd.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3nhybfavo.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3kxiqyhwu.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3hpamsrka.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3dsdqygto.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3vxkvddba.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3jtnrnjhn.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3grcdgquj.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3krstssql.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3pqqkvcem.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3rqaxoiog.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3tncxjiku.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3geshfovi.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tkozibzt.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3sbwwmxfn.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3gsdhkwjo.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3kopxlwjg.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3bdzplasw.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3obbcbnon.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3cwnelryt.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3iormmtxp.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3skgnyrtx.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3cdtbcuuo.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3vvrxedbm.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3ecspmxla.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3ntodckhe.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3iyrgyvdk.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3oczcgbza.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3wgnqmyaz.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3vxjveybd.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3dlosmjki.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3wrimforr.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3ejnsmhgh.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3ylqslxff.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3jvbmfefu.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3mtptqlfp.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3sqvmihba.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3lyxtbdsl.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3zwbcfsqf.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3lbggbqww.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3kfbrpzsy.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3cjkaabrb.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3yaahmcqe.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3qjnnkyes.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3rezmtapw.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3qdumquuq.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3mqnbdbue.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3epcbcgyl.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3amxnzhdh.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ddtwsevb.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3mpgyyqyv.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3ggbymxad.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3qzmemqql.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3apizzljg.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3vvvfjjql.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3fioqjztb.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3rrfxmrob.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3nokmjaxu.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3xafyhcap.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3vgbqlspr.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3khagcshp.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3pospqoim.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3cipqweuo.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3lwgsgywa.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3pcoympkb.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3qltyrmuj.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3wfzzijkz.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3voblqwhm.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3uiorodjx.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3mjudptpt.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3sfrgykjs.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3nxikliyu.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3caabmxyk.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3yltcnnpx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3vqosoqhl.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3lsczwjko.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dfkulryq.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3xioawpih.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3brquvuun.html


<!-- 参考信息 -->