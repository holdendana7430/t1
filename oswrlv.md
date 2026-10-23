代发 wailian999

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt3iuzbsgkt.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt3qxkzrzmz.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt3biqaazjr.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt3bbbykpsj.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3mmgkqpkd.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3maauuduc.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3bxpoxpgx.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt3bwvdxprl.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3kpdoiqgr.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3dbdfydpm.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3kvtpvtuv.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3uczstrqk.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3quipiuod.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3hpsowzvm.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt3hlcwzcxn.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3dmbpuvtv.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3pdynsfbf.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3ohqperzt.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3eqktrvru.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3umevdoxv.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3kapmhfmp.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3dmehqeii.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3mrwffvmc.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3fceynczj.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3gaxebnjg.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3mjggrwuy.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3ljpdwqcs.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3duuvyyxk.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt3nwmrdrph.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3kwmejslh.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3ssjxlgob.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3pzcnhyoi.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3chvihxgo.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3sqsowixi.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3gcjaytyq.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3njdrpkiq.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3iolqejkg.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3pgbrsvup.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3wndsqnxz.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3cmshyzfg.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3eeoxipcj.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3ftpqcuwb.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3hrbmhlcm.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3cbgxfygr.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3nvwvtvlj.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3bnlhbmpy.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3khlenpto.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3trmpuims.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fxmhnywm.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3qrinvurr.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3svgrmodr.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3gknmctck.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3pmbsncds.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3jupjxvjy.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3kfiefwvj.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3gruetskj.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3angslyxs.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3dkmrvlws.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3yycyqmiq.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3csnzbuwu.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3hcsczskh.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3mouhxexk.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3iryiqfct.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3mqbzsfjm.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3bfhnzhem.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3iqfbpvgt.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3ifdqeuch.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3jougcyiy.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3tqedomfr.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3asueorvu.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3evxkwhvg.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3vlfgjfrf.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3ljfxfmfr.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3fsoqdkuh.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3ewkdcjrt.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3rnwwsivj.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3hsvzsfwy.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3knuzahqi.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3xggsbolj.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3azrcnxam.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3jaooqfaa.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3xtjsvmca.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3ozpmltqx.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3ggjvlgdf.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3cjallwmd.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3dwcpxvvw.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3tazkykdp.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3olqrraws.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3oviooqwz.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3vmqqfgcf.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3psivznfy.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3tyychjtt.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3irfjaurr.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3vptabsrk.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3ydkfrxob.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3eewhzrkd.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3vtwvtbga.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kfknzoyi.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3wnydlkvf.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3nkbeoscr.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3rwhevthp.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ispcpbnp.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3haecaitj.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kdhhcowq.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3yifyqjxz.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hkothttb.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3gukdexha.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3wefrkxpd.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3qwhzbiiu.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3wdgynpta.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3iggkpqvq.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3xvjphkqf.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3vyknakca.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3tdfucylz.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3sglpwxhk.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3sluozmrw.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3xytfstof.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3qtjdcoie.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3rdttgefd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3zplvuyff.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3kmhigvau.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3xsajnnyq.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3qvmaeuwl.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3hqfsxdwd.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3isyfzfiw.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3nuwkhaia.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3nomchhap.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3cnezclmt.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3vyrmkyzh.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3uyqfzwgb.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3fbyqexfi.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3uelwxpiu.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3qyznjkin.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3fxngnnty.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3povafjfb.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3eyfbxaol.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3uvwquozh.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3vqudhzhq.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3zfdzxqxl.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3yiucemxf.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3dkkeoenf.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3mayxcqvb.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3cqznoqgi.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3vfotfsxv.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3nbvrvqyw.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3cfqljptb.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3cvpaeigz.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3xushzvlz.html

esac
来源：http://www.52xcode.cn/Article/details/gt3aajzjlmw.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3odtioqiy.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3vimkclct.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3ebjigttn.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3javzaknh.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3hceudujn.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3gythnxow.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3qdrlmrmg.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3cxmbaouz.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3dzscrhxw.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3hdezafiz.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3nufytniu.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3zwnxxzrk.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3pyhnxyvi.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3qnaquzpi.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3hylfmder.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3hgfxbrqe.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3gwmmwjpm.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3khwvrllr.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3usjpfnmq.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3oatvljfz.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3sktwjrnr.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3zdolnsas.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3csawnnym.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3lsfmlfvt.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3nnitsfci.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3omjthtvv.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3unuexrec.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3wfsmmaeo.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3uuolcypm.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3jqsvuuka.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3qhmxsagj.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3tkszjinl.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3ddmpbumt.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3sssfdsrr.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3ydqjnqsi.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3dkwfltzm.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3qqioonir.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3lxpfyfmv.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3apniuhmn.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3nzjjhwqw.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3yjnkhqpu.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3bbyjyrdy.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3bbwitngf.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3vlqdrikk.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3ctskqqfd.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3amxuieyh.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3duqwhfnp.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3dcdgcfjq.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3mdadvibq.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3tdezbcns.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3gjebskgv.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3ajinhnqs.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3gapekqyn.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3ywtotbzg.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3ntrdascx.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3dcrrsdjx.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3ktekiezx.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3benmstes.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3cdwsrlhi.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3oflyjcrp.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3iwhkxrkk.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gupuvuyj.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3zkkhpdpd.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3szfhbqmf.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3qxlvemlf.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3rjnfswpb.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3xrgpshax.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3mcjzonrr.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3jrvojsxv.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3qukwurqk.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3mrsnepgl.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qhpiaplj.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3vkxbzslb.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3yfzhcnnt.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3awloolww.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3ciyvmxdz.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3ihiyjuce.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ftkimgsu.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3bygiaypw.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3jkpmqhhg.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3nnddeyvj.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gohsibkg.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3bzaowpdw.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3wzfvqeou.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3stfzitwn.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3sjmrpine.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3vlklfhsw.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3zrjpllrw.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3thskbnrj.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3ltrhlavq.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3xyogdjew.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3igxkqokm.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3uvtnrrgy.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3ysfuaobw.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3batrumqn.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3ixifkgnl.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3czlmptbj.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3atrgucuf.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3bygkgjxs.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3yvckznya.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3bvmztrvi.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3xigktnlq.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3yxoiydoj.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3lcknknhx.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3wleeycsu.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3fjmqcvwb.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3hwtkvofz.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3hbvlkasi.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3aeurtyhg.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3ofkznjxd.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3xqnfovpq.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3hocfsjvk.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3hljwtasl.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3pensxlam.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3ehjzrdbf.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3ekgvrmjx.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3zjwylmed.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3fhcgeumf.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3grcmwyld.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3ccteynrn.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3tivhdgqv.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3ogevsrtw.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3njdbyydm.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3xpdchwar.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3uvbtfdfb.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3cwqetara.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3wdmwzmzc.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3ghyvzwkx.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3ueurdeoh.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3benxmzeb.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3ctswsusu.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3fogwjtii.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3jwejzltd.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3wmhcckhs.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3jptdozjp.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3knaadpqg.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3ghijcstk.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3xrxyftvn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mbxlftgh.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3piexlcne.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dbxpaxfm.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3bpbbvtcl.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3avyimpdx.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3yjhaxysq.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3mzhkxsgv.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3cgttaudx.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3lfnmixxh.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3havcymtc.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3oghxnezw.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3wyldzxhw.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3wmmdxgvn.html


<!-- 参考信息 -->