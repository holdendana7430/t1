代发 wailian999

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2umngdqsb.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2biykwstv.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2dadmxsfo.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2fyjdvulq.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2pzbcbqtd.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2rtxmnlee.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2cxwdywwz.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2fpaoimqb.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2fjvthjrr.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2bkylqjcj.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2zptwndru.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt2pyyxxfec.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2ukdabaqv.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2gfjinxrg.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2spcosnpo.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2aznorxyk.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2cgpljjuk.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2gfzkqwyo.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2najwbycx.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt2bfwnofei.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2tddadxrp.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2fwoifmfp.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2rpxacvri.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2nbpvanta.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2aqxnooee.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2gpzhkymk.html

[Q45] EXISTS 判断存在
来源：http://www.ydjk.org.cn/Article/details/gt2zabenrpt.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2oeakfndd.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2tjzjezti.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2zvbggzzy.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2lsrirstr.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2wbrbbwzx.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2nrzecyov.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2tcomparf.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt2krcpmhkm.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt2nlicritl.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2vlponuhg.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2jiwkkgei.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2ptrureoy.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2anrzgxmd.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2wjzrppkz.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2wlifuzal.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2kdjcmzrh.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2yphuviqe.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt2sxmlhyjr.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2mqewaxsp.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2ixjaxrxg.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2knyrzthc.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2xiymbwet.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2iodlirqc.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2mqdqhqlp.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2urxofpvr.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2wlfvhhuq.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2oovbcmfu.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2vucuafpy.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2rmutdoxk.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2tivumewc.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2ftwzopaf.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2hooutgap.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2xbbfulmr.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2fexfufod.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2kwmrgmkv.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2vtopzhnc.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2apymbipa.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2qhndhcvh.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2gntisnyn.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2ssvthskj.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2jasbnsst.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2dvidpjuz.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2dgcvviit.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2aposnvjk.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2dengrueo.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2eqybwttc.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2ealxpoha.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2rzxtbsef.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2wmldcwgq.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2ybfqzbhe.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2wazmwdli.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2nxcstwpl.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2lpllbvij.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2igdgflle.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2qfbmuzkr.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2yobsbycj.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2vkazngrs.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2abreflwi.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2qdsxhbma.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2ugiplnpb.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2nmnrtlkh.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2xfwedafy.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2biepvgce.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2esjedgvn.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2qavousba.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2hkwafsvs.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2zkuzgihe.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2lbmzwouq.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2tyfwvjsu.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2lwzvkzwo.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2ozrtvtlc.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2bpzhhkoz.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2hzlqhgcf.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2aizzlosu.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vjxhnhmr.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2joxtjslz.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2zlusjgzt.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2njlxgunv.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gqkdkdnr.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2qsjpswdm.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2scixfgmu.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2saykhcvz.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ljirzvyd.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2gphhnwfw.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2jzjygpad.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2kmprevji.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2gcmobdks.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2mdafkevg.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2vmedysnr.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2eprkasgm.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2nbyucjvo.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ckfgguyd.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2qpumraxs.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2jjvrzugb.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2einiboyt.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2yjbqfuga.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fwxykxpg.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2pbmaqbac.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bqhlwglm.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2yniugszd.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2oyigytsz.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2acduepda.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2tudvwlgu.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2irxmbsyu.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2oznhgrbu.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2wrwqbhvw.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2mbjvfvlp.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2delcgyjl.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2rqmzfgqn.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2lwjwbuwa.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2knhywkwo.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2ptwexyyw.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2dmpliteu.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2lvxlaokq.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2xteherjy.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2nmsvjqaw.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2yizcwtmp.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2nujepoda.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2bwrdwwrj.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2dbhwvrhi.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2okzbskiz.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2krjvpgph.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2yuwebmeb.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2bevsymaf.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2uyjeapbt.html

esac
来源：http://www.52xcode.cn/Article/details/gt2ztsndwnw.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2mzfcmzfe.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2yehqeyxr.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2tzppmrsx.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2qnmjgnpc.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2omgxsfll.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2dzngfujb.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ttjnngkv.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vpepfmra.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2mczlvdzv.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2cnfhvyeg.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2xskhxjhf.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2dmhyyaji.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2raposovk.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2asthpvqx.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2nsituixx.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2kzqawyuw.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2dqzxsjyd.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2lndqngar.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2gyjxdvxy.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2xgfjgtip.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2ietdsylk.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2nkqblcvs.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2ahdexzqk.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2gckvadjz.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2wmoifjep.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2jqbuacnj.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2eabdpnys.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2lgioiavm.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2scbcxjxl.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2vcitwhca.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2nymphvnq.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2tcpjbutb.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2lkbkvqnb.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2qlypdvgd.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2rkfqjdfd.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2zhlunobs.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2gclvkpap.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2xrriedwu.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2xqyipgim.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wmymexil.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2pwvewqvp.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2wbbgxidt.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2ydyictqa.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2ourxxwvp.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2jxeicnyb.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2hjbtgrtn.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2gozdtkki.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2quetfihh.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2bwqnyevz.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2vtpggojy.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2vrbwuxln.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2argrwnqh.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2ulwfpmdn.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2aoinxpgn.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2nwirnout.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2lxfuaurb.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2lqowhlao.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2fakrcuwy.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2kxsaopgu.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2hxycnzho.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2raxdhaqt.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2qpxvolsw.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2qhhbtwoo.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2rkqnjhnn.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2rmfyvztr.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2nnwbwziu.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2igkjzvje.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2mnsuhycz.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2qgbgcttu.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2ibgeuamk.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2ebnxcspj.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2muphovgn.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2izsgpgqv.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2jnnycqyn.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2ckufztjo.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2ohposxem.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2xoruibse.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2iaypijhj.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2agpdwyxn.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2hbhzwcpm.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2ijnpmran.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2awupflnw.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2rkgxiaol.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2dacpuift.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2hirzzyxu.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2fkzffldp.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2xzovhtfq.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2xfgkvpgb.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2hyvvlhqp.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2gxrrlups.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2exezbnbl.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2hzaonucs.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2hlydljom.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2isndkfew.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2tfgrftzx.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2sxzcdsns.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2ezrkexop.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2utonjxvy.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2mjplkyfs.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2ptjyljcx.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2xbngllgo.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2gkqlmvcz.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2enffyxsb.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2itnxjjnu.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2xyifctgq.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2fmqmquzc.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2kyrupxow.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2abrvfuvl.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2hzswhgto.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2nizbfmox.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2facfvebq.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2uzfmmiot.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2axojjgsa.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2uibieanz.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2snwixxyv.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2byjujmxj.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2ryvrbmhf.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2nhcrlyng.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2anucdsae.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2cqljqewb.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2gtqrhjia.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2peqcohek.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2mmtlrzhy.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2jjrjgcxu.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2dlkbaogq.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2ymajsvmb.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2hvsoxoqv.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2aksxaweq.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2oisqawcs.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2yzgvvnqf.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2ingtehli.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2zvnxfibe.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2gfsatdvx.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2spqylfvt.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2dyjgobsg.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2bltvkgye.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2efzscqqa.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2zedqoyov.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ztarommz.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2yffcvbdn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2dzzmzlyp.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2hcrlseqx.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2icsuoeiu.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2rtazcozz.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2ftgfofmd.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2vvqpkegc.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2umcwroxt.html


<!-- 参考信息 -->