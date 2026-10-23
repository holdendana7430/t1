代发 wailian999

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vtgrlaib.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt3zmietmsv.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3qetrfncy.html

[Q31] 分组后过滤
来源：http://www.ydjk.org.cn/Article/details/gt3vriyolzi.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.52xcode.cn/Article/details/gt3wdolpfyo.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3gaglojov.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3kovtvogw.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.52xcode.cn/Article/details/gt3fdvagllh.html

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt3enldpasp.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt3kajucjlr.html

[Q34] 每组取第一条
来源：http://www.52xcode.cn/Article/details/gt3axcfxrpa.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt3rstnuyam.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt3ntpwgqic.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt3jjppvlac.html

[Q35] 内连接
来源：http://www.52xcode.cn/Article/details/gt3ptheogct.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt3vmqzvrbn.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3ptdkupnr.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3ocbazqkp.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3xsoxfzsw.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3xcqfdbqf.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt3rrydxjhm.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3slqdfijc.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3frtwyqgf.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3gpsbhsjg.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3ncphrjsp.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3apdthgxm.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3nnzfxwnc.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3epmmzqcd.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3mjtlllfl.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3hlixmlkf.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3hoogfubp.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3szrrdkbm.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3pjurbfud.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt3nhxngrvt.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3uggyuzcc.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3oiyesiti.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3qqfsvplg.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3qajtqymf.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3huvxzmsq.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3qqamtwaf.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3jewpxjkj.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3vxqrevzn.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3ezznvpha.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3vpqmzomv.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3qdpxbrhs.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3ixeyxrtl.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3llpcbiol.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3rljeqwzz.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3moeuaius.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3apuosdpk.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3nxguitjq.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3odirqxtw.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3kxxzkyhu.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3nnxkqjjw.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3jmrtqcsn.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3ygejkzcm.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3ejhfkitf.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3yvpiwwyp.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3ebwdoudl.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3zokdfdwi.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3gkxifuoe.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3jstqxjla.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3lwtronif.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3eufsojpa.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kfutzvki.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3ytdbbxvj.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ahgglbql.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3byoawieu.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3wdfebvcs.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3mrkjctua.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3kckdztoa.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3mlcdfkzp.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3pvlobvfy.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3wboyueqx.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3cywnwyyk.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3pzhitzgo.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3rcjvelwc.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3uzpinqqx.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3qbxkyvew.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3ybwgylxa.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3poqjhpnv.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3iptdetdm.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3bbcumsqm.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3iyjpfikn.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3awwrephn.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3uxidvvlt.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3xhlnzgdo.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3kwdxhmdm.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3aaxiyeip.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3wpfvtmub.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3rmxwgwjg.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3vtsupntq.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3aubujbqt.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3lxafsiiz.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3zgqjgblw.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3cgubnuqh.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3feewhsxr.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3lgvmxbdx.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3msshowom.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3vvcfvytl.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt3cboubmqt.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3qpdtrhjp.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3xacslybx.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3dkzmrkrq.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3hfarsndw.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3ctehargw.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3gxslmmrr.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3guzttqdc.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3qomqmyhk.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3vdbywxik.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3ewiumrhu.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3gtawpqco.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3mbsysgxo.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3zeqgreko.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3lblfwcpf.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xlnedydf.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt3nobzhazq.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gvmqfyob.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ulrudjwo.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3tlkvkxkk.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3dbsmvrje.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3oqiprbxo.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3qwvcunkl.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3ityakgtr.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3ojcnkirl.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3nlwmlyza.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3gvymsgrz.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3uohifjws.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3anlorrjb.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3xobjydqx.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ybisjsig.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3qejxkilw.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3dpmfyxgt.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3dxonjvgg.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3aqhckrou.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xunzfkys.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3xqfjlzmd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qaalolwu.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3ezfllyhv.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3yajyjglc.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3kktmgoly.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3yxdvdlxn.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3smgdybwu.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3biqkmtmr.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3iulbjtxa.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3jyiwabod.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3hphvorau.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3qgynjbvg.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3ellyxboe.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3mqqbqzlw.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3bsnprkhi.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3suibizzg.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3ckxdimeb.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3ufcxspht.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3lpvsgqbm.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3exumxjxa.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3qqiqaiww.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3sjdgttje.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3cfoiogvf.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3dfebxgpj.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3buxqdush.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3ffvplnbz.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3jyfsohha.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3ufqatkyd.html

esac
来源：http://www.52xcode.cn/Article/details/gt3uldlvxst.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3dciapgjz.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3lwvfarzp.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3xmsxzrqh.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3knayphmz.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3rneuqzix.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3voyejsuo.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ewxqrghk.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gksypmvq.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3mbumjsjz.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3eguhinwd.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3qgfzozjg.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3nvrnjdkz.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3coadklls.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3uqiyanrp.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3pglrerht.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3beocbiyn.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3ghfjqrhm.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3mdtnwzzj.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3voihgrqb.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3fxksiqsi.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3lmwmnwuh.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3idhsyaqq.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3sadegitt.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3aenjbqxk.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3jjnipmeh.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3zezyizwy.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3hmbedesq.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3unpwrpue.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3aulzvyif.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3synwejcf.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3cjveuwaa.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3pxlcyglp.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3mjoicwlo.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3nauzxbnk.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3abgljqyx.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3uiymdscq.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3jfxbmwhk.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3wzxybaqg.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3etmsdhse.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3rjapbacy.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3qlxnzegr.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3uilzasic.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3yeswhfgq.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3amofpgjn.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3ktvnikzq.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3tsbodixk.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3hdlnntni.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3kqgllfyo.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3gmxajqcq.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3zudfsfih.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3qugliqma.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3xbicrejm.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3otmdbgpt.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3atpjwduq.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3tdkaueyn.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3yafybcbe.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3lwrvinmz.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3emofcixw.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3tcudegsb.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3ehuouvlb.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3uslazcdt.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fcxhyorz.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3zouelqdf.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3gjfcsebg.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3wyltkakn.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3yyyepygx.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3ovinxkcu.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3guyutsox.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3updkkcyq.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3gdukuiae.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3dxoiuuhu.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3lbixnooy.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3ebpzsqtj.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jqgooxbg.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3woxaptzp.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3ifjjynwm.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3ccyiradu.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3axmzqzpf.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3zaarlqsv.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3ezhhvook.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3vyjmbvad.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ptdobntv.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3lxlntmnj.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3oxqqvmjb.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3bsjjbcwn.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3udetnxjt.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3wvbbzdnb.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3yhigwdlg.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3fwrieecy.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3wqcjfoew.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3zkjdcvwz.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3bdpwzilj.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3rzpydrpp.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3ivyrpmtu.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3cijttdls.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3alddvdgw.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3gvzsczvq.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3htiherzr.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3jpwxsvjj.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3dzktxgmk.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3pelsluam.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3kiwnokqu.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3ssgjmoxq.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3ybeabmnp.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3aghdoisa.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3fcouvvjr.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3vgmvxjny.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3nzrvdivj.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3mfczqzfy.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3qboqicwo.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3czwubnwt.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3zbaxnkag.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3tmwlgjkt.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qsqlsmwq.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3pokgkiih.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3rbhituxk.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3hwibbxsl.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3pqeywnnq.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3fbfykybg.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3qbtonmtx.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3heoianik.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3ahkqtbyz.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3nsrxtpwj.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3hbtnnphp.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3izamintf.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3yqqjvexn.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3dvxvbsvj.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3hhokvrmf.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3aqdtklet.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3htoszkuh.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3juialmrc.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3lqwcnhrl.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3nqruzqid.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3nurnoidb.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3sqbxiokc.html


<!-- 参考信息 -->