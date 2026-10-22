代发 wailian999

SELECT MAX(age), MIN(age) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nnkvenpq.html

[Q30] 分组统计
来源：http://www.52xcode.cn/Article/details/gt2jgalzdte.html

SELECT city, COUNT(*) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2xelrkxqw.html

[Q31] 分组后过滤
来源：http://www.52xcode.cn/Article/details/gt2dhxoaavr.html

SELECT city, COUNT(*) AS c FROM users GROUP BY city HAVING c > 10;
来源：http://www.ydjk.org.cn/Article/details/gt2ismfsfwf.html

[Q32] 分组拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2gjesdoka.html

SELECT city, GROUP_CONCAT(name) FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2kosvbfrm.html

-- PostgreSQL: STRING_AGG(name, ',')
来源：http://www.ydjk.org.cn/Article/details/gt2srskislu.html

[Q33] 多列分组
来源：http://www.ydjk.org.cn/Article/details/gt2alpvinke.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.52xcode.cn/Article/details/gt2iigoopop.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2ywaannby.html

SELECT * FROM (
来源：http://www.52xcode.cn/Article/details/gt2siexplwy.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.ydjk.org.cn/Article/details/gt2wxbyetoo.html

) t WHERE rn = 1;
来源：http://www.52xcode.cn/Article/details/gt2rpcgxkte.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2tvrhahna.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2vakufmsf.html

[Q36] 左连接
来源：http://www.ydjk.org.cn/Article/details/gt2fzfjzyfb.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2ebdlbuur.html

[Q37] 右连接
来源：http://www.ydjk.org.cn/Article/details/gt2ecxfmvoi.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.ydjk.org.cn/Article/details/gt2ycgygccc.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt2akfvxiif.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt2cprjampz.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt2egqgqqtv.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2wbtlrupv.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt2erftvjeh.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt2kpvzkgfb.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2riwiotny.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2mjcbuaqh.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt2qwrbysbq.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2phprudkk.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2ymyoktos.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ltmcrpht.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt2svjqyzgz.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.ydjk.org.cn/Article/details/gt2jgssczwz.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2ggzxpgwb.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2dxnaxpjy.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2gaxfjxxf.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2bvgvqfvg.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2wjjxctwx.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2xlbafind.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2cubazfcj.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2vzbntjjf.html

[Q47] 与平均值比较
来源：http://www.52xcode.cn/Article/details/gt2zxhcaxls.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt2siifphyz.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2ozthzhmy.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2bcfbylwv.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2jtducfxu.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2qfdwkaem.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2dldrscvb.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2ssyboazo.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2qmkwqiaj.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2onthxjmu.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2eovmtzot.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2vdqhynyl.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2tsbtfrdb.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2ogbymnfn.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2iwahapfp.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt2cjtyerua.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2jnlidgop.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2vxajqaue.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2hygjtrxo.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2zlltrwes.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2glfeshnk.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2ilvfmzfe.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2njjfnxfw.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt2bplzypck.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2tacdhmha.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2ioerszey.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2kscmxdal.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2pqazeklz.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2wivkqaxl.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2qvdrhwan.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2hrqblpkl.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2nguafswd.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2ctnxpazf.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2lznjmcab.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2vfxmycwt.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2qkxhexmk.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2wgvqzbcc.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2riwqktfp.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2ottwnqii.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2swqybycf.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2cvcuhajw.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2xeeecdgx.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2ovtawfag.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2zbeorxtd.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2evnqgrlg.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2bbfuanyp.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2qktejlya.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2rbnplyst.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2niloaqjy.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2ddmvvnwn.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2doudsawa.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2eteskrlr.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2dddkbmvf.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2fagulnag.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2boluxeeb.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2dqmooxpu.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2mbhqryye.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2jhemsygo.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2siyfuogo.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2wjdutsli.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2pxvsgsmu.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2jyaxbavy.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2lxijdkpr.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2nmzsouwp.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2kcuvftsw.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2lykvtecg.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2mglujcyi.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2eunzxvmj.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2phphtwxg.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2wcywzswe.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2hhhemtbn.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2xqjmorcs.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2lrzbyfoa.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jnpjyuxm.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2amigpxzi.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xnmzhifc.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2nffpnnoc.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fltckler.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2pfuqnhmw.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jywlhqnm.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2yyjwidus.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2emgedtqf.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2buqcxakj.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2zgqtimvc.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2ciwyqimg.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2jcjqgvez.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2yvyzciji.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2wyjksuxs.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tjdjxrcd.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ysxezsym.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2atjrzsbg.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2gpbkfoqk.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2xxaackiy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2kvhgwqbi.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2lsnmhslb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gpcxmikh.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2nfsgdpfd.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2davelnvt.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2tkiptoeg.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2drjqjypy.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2jdzcsbow.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2dmxxopdb.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2qcpvomoc.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2vzanqemw.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2gmjevolb.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2yarfzlus.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2zedbjdqd.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2rdkguexr.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2uvgwsbhd.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2nyoulbun.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2cthxtifi.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2pkbsxhai.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2ylotsile.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2imjtephi.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2wbkfdneq.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2lmsseots.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2pommajct.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2fffpkvvq.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2uuhqtraa.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2mtrldeks.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2mqtjmskn.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2rnbujncl.html

esac
来源：http://www.52xcode.cn/Article/details/gt2zccwjagd.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2mkmaozvr.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2egdhmpdb.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2fyhhyyug.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2qfaskapa.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2kdkzzyre.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2xrhssjha.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2rbmbyvot.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2unjivgec.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2ewnnlupv.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2xqbvtmpo.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2jkryhbrl.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2tlkylxpn.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2uombxmxw.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2zjlpcmhn.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2atjvjohw.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2bgrkhenc.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2ogmqhekb.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2qweathhd.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2chswunlh.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2etelndpo.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2axjwnimw.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2mvpzujcz.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2acxaicus.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2peyfbhoa.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2apwndkqb.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2hfmjauwj.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2xhalkpzm.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2xurngvjy.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2dzxyzgqq.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2vyfmvyaf.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2uymhvszl.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2qnhujrkk.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2glqsethe.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2xhtneaho.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2vmlkavlp.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2mqsnglqh.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ffjseqim.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2dczewwqb.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2wthgqhzu.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2grnnfezf.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2vdjrqdkj.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2iprrrhjq.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2irmkjnqf.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2uzwphsrh.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2afugeirz.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2jhgxwwsa.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2aftdtikk.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2vneacrvv.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2klimhjyt.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2wjytlbvv.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2rhphtqqx.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2pyerwczj.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2vbcrqdge.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2ucpwlias.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2ekpocjyl.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2wiqdnrnx.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2pomfxdaa.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2auavpijr.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2jqgojggy.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2geqmvtko.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2vhlobdze.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2tojynysi.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2kwvsaqhu.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2xzmpcwzv.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2rnkjgmqg.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2maoxjtup.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2tnomdngn.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2uwpkxhvv.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2xrfacqht.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2vvtohgpk.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2xlnopjqc.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2zlhwzhnx.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2gxlerhgu.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2tmqqoakw.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2ziomfqfv.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2oaufvfjv.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2stmmguyl.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2lajdmxra.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2ztrmyyut.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2kjadtxil.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2fmlqkrhe.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2skkscgey.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2uunupvdl.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2htiewkgd.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2cltnlufv.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2xwkdqnjj.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2batfadwx.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2sbymppqs.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2kavdrsfs.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2msmbycls.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2cszjvhrp.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2dssdimav.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2nxjhhknx.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2gplihvva.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2oiouxqer.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2zldphoxy.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2sdxyyonl.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2qhoipshp.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2ihlhjayz.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2ivdabjqh.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2pbxpmzan.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2ihbvdfkv.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2smipjlhz.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2etmtlwnx.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2kjslradb.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2myuiiavr.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2vwhezzzb.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2uaxqbmlk.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2ouygicgf.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2ajrhndfv.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2iamijwpe.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2bibvtbzb.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2ffmsgysy.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2ubenrfcm.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2ggojbyta.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2jbafhuyn.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2gbmdulrm.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2kvrdofqy.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2foblblsl.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2nxtqgdze.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2anxgiidw.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2cfptpntk.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2yhsxtgts.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2lwbjnhxd.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2wiphqbue.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2fyxhpxdj.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2qzqdxzth.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2kohjsklo.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2gweaiyxw.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2iyritdvm.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2vuxwmmqf.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2xuzhwlfi.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2fnmeulza.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2ommnqyjl.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2qlnmhigj.html


<!-- 参考信息 -->