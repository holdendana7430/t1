代发 wailian999

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2jhdjfecl.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2twprtlxx.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2qzfswtap.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2demwxwdk.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2rjrpqwov.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2tzedthpp.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2hkgmwkuu.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2xazsswmp.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2xpgoltih.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2mlzvetzt.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2eymynekl.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2uhykcxhx.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2vmqxnhfi.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2wawhleza.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2nnbekwbo.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2dgddiros.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2vpzplbml.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2fljlenqq.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2ipielgav.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2vsbalxzi.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2padhcnkf.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2fqphkmnr.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2epowpypv.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2mpgdczlx.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt2ejdwqgdj.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt2zvnlxxak.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2fpiuyvkr.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2oslcyuwv.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2vygqtokn.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2fiyxakpw.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2khbyhfqy.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2irahjdcp.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2dewoxvph.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2jijmliig.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2giccjnkk.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2uvlopidk.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2fjollhba.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2hbxsxgla.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2jtkojzyx.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2tvoeujmu.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2pucbiuok.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2obbgoqpt.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2fzwivybl.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2ikpeyilq.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2vjuipbbv.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2zzmxsery.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2smkzibfn.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2vqkprugx.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2oejlpmku.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2fshqsckd.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2subpjxio.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2afgswomj.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2uugywsjs.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2infjgkvp.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2phicmuuk.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2rzngkkmf.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ltfpvlvf.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2ecnhlkyw.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2slnywsnb.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2cvfmtoky.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2pfoycbve.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2uchfluwv.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2skucrnhp.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2gqjgopjl.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2gafqrzeo.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2fvrjvrux.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2grsflnzh.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2amyivhni.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2eltqocbj.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2jcsefhiv.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2jhcchreh.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2cvfbaqgr.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2bvpnxpcv.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2flbijmih.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2arftskqg.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2wqpjgmsr.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2ospovzvn.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2spulaxkd.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2gqseowqa.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2tlbwccgp.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2ynpiuicv.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2fvgvrajy.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2chyjomqa.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2rljxteiv.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xbexubkn.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2urmbcakh.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2odlqchnw.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2ashgmclw.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2mnetyryj.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2jxdzwhdm.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2xovidtxj.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2btthcqnd.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2pbrinxem.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2mqihwxlm.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2gxbknvex.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2iupdwxkp.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2oiruwkfr.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2kblluasi.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2dmomrgyn.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2utwlccby.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2advttkmj.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tpkkdwmn.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2eyqqfnli.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2irdhjxfi.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2itcrjbxe.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ljbhnltu.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2efwfyjyk.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2zxrolyxb.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2iuvrxfrn.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ohzakpak.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2kfdhmlat.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2qohadcjr.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2xwfymvgi.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2hmfvgbtw.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2sisykgcf.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2gemuaesb.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2jpiujrgs.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2xkrxsrha.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2edicmwdm.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2aogynzrh.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2ochbbspa.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2nuwcpviy.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2cchmlqta.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cysaylqg.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2khnwlpgz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mbxaztaa.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2zbyocrji.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2astsbzbi.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2xthydqco.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2wbjhchgq.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2rsdjvmoa.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2lwprzahu.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2ibpiryro.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2bdjnpxhb.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2lrbicmep.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2rybwvjmb.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2qomcfywm.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2srysdjoh.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2uvwyzvwo.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2nvefplre.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2mzwqcljh.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2fgwmqwia.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2bhltgwul.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2qaiasalt.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2tcxroihc.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2epznnedi.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2qgmgtjeu.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2mhrsxngt.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2mivblotl.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ctdgsqdq.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2dyughyxy.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2jewxanss.html

esac
来源：http://www.52xcode.cn/Article/details/gt2reclcqmt.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2ydakvuqi.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ientoxvz.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2tqixnzrf.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2dypejpdp.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2rinykrwg.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2zjybxtba.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ucmimtom.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gfdehnkq.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2ckucxipm.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2sjemsyeo.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2sifjnqst.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2znblufsf.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2kyvmwtjm.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2tbjzfbrz.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2qjecdcws.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2mspqhilc.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2vxlbybrp.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2bqbipoun.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2ivczvtaf.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2vsecexqt.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2dqtxjurz.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2kqdidqhn.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2ecyafvjv.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2jbeoznpf.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2rdablmkv.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2lqflxqsu.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2ajrsmheb.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2cwcpriwz.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2yjzebruz.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2jihiziaq.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2uvcsnttb.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2qghxtefl.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2uthcmdol.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2rbkrmvml.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2sblqbltq.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2rihjwrso.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2zirmmkkn.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2awxarako.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2xkontjit.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2cfjtmglv.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2hcghikbn.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2sysfsitd.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2tdvujcde.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2vcvoptxn.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2rjkazwzg.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2dghyhpzq.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2jfmfuiad.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2tpfntqry.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2krkxxxqk.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2gqvdbgch.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2jlhegvcx.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2fbujkqzb.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2okxekztw.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2rwbzwekc.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2phpranxr.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2amgwumxq.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2ugmnygoy.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2mrzoaack.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2gmapueqn.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2vfhqjsgh.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2xyuvadcg.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2nlozmduq.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2bnlkarcc.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2vsfcpojp.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2ivmmhcah.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2krtnkpew.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2mhsuxpma.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2uyucijfp.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2jtemqyav.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2nurbpqvr.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2gxhxacvk.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2fkwmygmj.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2ouatnkyk.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2rmwnffnr.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2pxiahxly.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2sljxwuqm.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2yuuisddi.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2aunprnkz.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2gltykvzk.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2stcmjhvm.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2eglbamgr.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2hisrwtsn.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2kqqdbpzo.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2muwwfvqv.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2qyyxdwxb.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hueplqsa.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2qpawddsy.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2ciajhdwl.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2rvxxbpdc.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2ppxrmhnx.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2gdxzldnd.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2bidttozn.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2axqajwxd.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2yrmuxhro.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2smhctlxt.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2tcgzybcx.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2cizgmfwt.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2vmvaebqv.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2lsbsgwsu.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2rsydqpyd.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2uksbdrgr.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2qgjmoruw.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2kzxbcqsr.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2kjdoiwpa.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2ztoauuwg.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2rgvktvmm.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2ycmvzigr.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2ambfcedb.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2qdfkitjc.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2cfoccuqe.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2bihyrgaa.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2zlzpxkih.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2kdgtntik.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xtlgktba.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2fgummzfr.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2vpmjbgur.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2cxutsqkv.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2fbzxuedb.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2afidzrpq.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2rdimjxip.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2zugblfqe.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2wxhxmclz.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2qzbaogos.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2vfqqrrcu.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2kxlgowki.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2byjkvekl.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2jsnhqcyp.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2slglndom.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2tqjjvuuu.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2tlxzwgln.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2kbnjhgcq.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2ndbcqulk.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2kqppcbwo.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2jvpggleh.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2tlmdhoax.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2bxnvzvjt.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2cnunrcvt.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2tlxwcnst.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2jzxlgdub.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2woaksrbt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wnlhskua.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2rtmqbtmp.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2kgwbonli.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2ebppeikp.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2unusiuvz.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2zzevjieo.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2nvwgfobj.html


<!-- 参考信息 -->