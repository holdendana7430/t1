代发 wailian999

[Q33] 多列分组
来源：http://www.52xcode.cn/Article/details/gt2oohiizsc.html

SELECT city, gender, COUNT(*) FROM users GROUP BY city, gender;
来源：http://www.ydjk.org.cn/Article/details/gt2lztwplft.html

[Q34] 每组取第一条
来源：http://www.ydjk.org.cn/Article/details/gt2gsfyjims.html

SELECT * FROM (
来源：http://www.ydjk.org.cn/Article/details/gt2mtbyqfkg.html

SELECT *, ROW_NUMBER() OVER (PARTITION BY city ORDER BY age DESC) AS rn FROM users
来源：http://www.52xcode.cn/Article/details/gt2aduwmmjm.html

) t WHERE rn = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2mgreefyy.html

[Q35] 内连接
来源：http://www.ydjk.org.cn/Article/details/gt2fbgohnfl.html

SELECT u.name, o.amount FROM users u JOIN orders o ON o.user_id = u.id;
来源：http://www.52xcode.cn/Article/details/gt2wfvdgimx.html

[Q36] 左连接
来源：http://www.52xcode.cn/Article/details/gt2hksilmze.html

SELECT u.name, o.amount FROM users u LEFT JOIN orders o ON o.user_id = u.id;
来源：http://www.ydjk.org.cn/Article/details/gt2unmbilxr.html

[Q37] 右连接
来源：http://www.52xcode.cn/Article/details/gt2onzcnaly.html

SELECT * FROM orders o RIGHT JOIN users u ON u.id = o.user_id;
来源：http://www.52xcode.cn/Article/details/gt2jaqnlazf.html

[Q38] 全外连接（PostgreSQL）
来源：http://www.ydjk.org.cn/Article/details/gt2uvkltwnh.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt2wtiyexur.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt2nhfcmxcj.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.52xcode.cn/Article/details/gt2yhzezyhc.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2rsdmkrjw.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2trssjkml.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt2xkgyecag.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2amfqwuxs.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2vxdcdeeb.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt2rrkkfvmo.html

JOIN products p ON p.id = o.product_id;
来源：http://www.ydjk.org.cn/Article/details/gt2aornvfql.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2tfmvmezn.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2jicspixx.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2rmzznnaa.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt2sdytbkgw.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt2hmmdmmiw.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2eoonmijm.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2tjcgltyy.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2puqdgbrp.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2lqizsoxl.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt2cywqdnhv.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2bdceqysy.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2nqporkwq.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2qqfllgyn.html

[Q48] CTE 公用表表达式
来源：http://www.ydjk.org.cn/Article/details/gt2cbhemyej.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt2oebpgenk.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2traukdnv.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2hikoubhl.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2tpecbmdk.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2pfwoodbp.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2gynsimxc.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2msmgsnzf.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2skqbkyff.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2xgwcazta.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt2peyretph.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt2aoytjfmd.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2csemqqyw.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2fwgwyobu.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2blqxhyen.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2ytnqqmrs.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2lfjoygta.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2bsomxanc.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2ehxjpqvr.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2lagejwah.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2oalpmbip.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2ilyhxiez.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2soudiplx.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2onvvknap.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ukjinsvh.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2hfmtaepa.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt2iuckmjiy.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ufmseosk.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2xxycrpwh.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2velejlgn.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2rtnwzvej.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2sprwtfzn.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2eelrlves.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2asajheae.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2xiuyxbql.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2kraopooj.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2vliomkbj.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2tmkjlkys.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2bppsdohh.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2zpnxfuao.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2xiowjdtj.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2yzjfbmft.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2xmxzptqk.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2baeamnsl.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2awxokqms.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2dwnzpgun.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2zcvamphz.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2upywblfd.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2gazlhqgz.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2zemdfwrp.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2tqaodeqg.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2bbbpsxrh.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kuiuodut.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2oqkuejas.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2omkbqsdk.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2ygfwnjzb.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2fueztorw.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2paxuijik.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2lwpbexuy.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2esnkyeex.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2rpxahirz.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2ieanrvmn.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2uryekfln.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2mifiemma.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2lczwfrfj.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2perfcqkq.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2gyaoycdk.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2bbrydeyw.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2eblepfph.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2yljurome.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2kwigxfbf.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ixzfapbh.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2ihcwehge.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2cvumdpcd.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2etwduvgk.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2niemcwfg.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2rishulgf.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gbcadwnb.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2sfrpulza.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2dltrewea.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2oxopkwew.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2ikeftsbc.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2fwbodovl.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2szzcsamw.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2mnjwmipj.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2mfkhlhki.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wyqgxvyc.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2budwybuf.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2acwjqjzz.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2jfnyghms.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2cgtjpxta.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2axfoarga.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2emkccooz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2elwtiybc.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2topszssh.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2wjdngbhl.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2gkkidfel.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2zwzzoqng.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2ramwdmqj.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2dhdharom.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2mxfytzfn.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2vmbawoem.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2kqkgsiwf.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2utvwpnwt.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2suldwxen.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2ssvurjjl.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2oqbbmvxn.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2zkfpuheg.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2xbamidyy.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2cnioroys.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2jpjgykhj.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2acdroklf.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2zjwrbvst.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2kzasprze.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2mpgmlxzz.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2migmcwxq.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2wurpbuho.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2spujwuuh.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2fktsxqzr.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2wjyanfnv.html

esac
来源：http://www.52xcode.cn/Article/details/gt2bzanvrxd.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2vlgjjqwn.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ciwicyiw.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2lhpkdcbq.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2acdgtovq.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2jctlzmab.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2hvifrjdu.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2vytmsfhq.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2dkxqyehl.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2mdikvxiv.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2gzchagxs.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2qgsysmzh.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2dxmrfksc.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2iombdcyl.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2usiqngzo.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2rbbcgnig.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2sldxwaba.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2vyxdewvg.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2pirvfpsg.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2kjcwonuf.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2djybrbhm.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2rapxrcfa.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2rxzaidjz.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2nqmhykyf.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2rejyyipb.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2fdozxxxa.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2roqltano.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2rzgpzvvz.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2llzavyaj.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2xriczowu.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2qvngucrf.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2gnyfeizm.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2dsuzitwi.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2abhewjei.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2jwbvfjxn.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2ueessyzf.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2fbiaukus.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2wbdhykhb.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2cuuljbwq.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2wtssdvdo.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2tgroybwh.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2ltgykapo.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2njnjtumo.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2ohatotbt.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2pypmaban.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2gseilbin.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2hkceqtwb.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2fhqorzxk.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2gojbxwbb.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2cieeedff.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2ebfiwnlb.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2oeubjtuq.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2syxrofyh.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2yzqqayxk.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2pkepupag.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2naozwegf.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2yhgasqdt.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2glbykynu.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2zhzmofjp.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2waesjlho.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2rlllllmn.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2mdrqxhzy.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2rwprqcic.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2jmuemuqf.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2ljhyukmm.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2jqintzlg.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2fetargqb.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2zffhkeup.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2pfdzdsnn.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2gwyuhvoe.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2dbrxrnwx.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2vflmszsn.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2weaozjqa.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2toiumxgy.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vilnrlzy.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2iygswdqz.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2smpqenqc.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2jvtdfwvb.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2rhbrlqzm.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2geczolni.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2cnqzqfxl.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2vhyjlxwu.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zwfckpre.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2wcrsyruw.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2efwatbfr.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2xrljcozy.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2cjsrawpq.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2mvczpgut.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2kqhukyhw.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2keefeeln.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2pubkajtm.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2npxuhivc.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2zycyuodx.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2leqawfwp.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2zzcepocq.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2wpejtwmw.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2kigvtemj.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2jiasjnwx.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2dzqbocue.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2awbflhvs.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2znfdopmo.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2vaimrlon.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2lrakxvks.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2ewfyfiyv.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2qvludrsu.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2sitzmcvj.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2euysbmib.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2cqxvwbov.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2tbysxtks.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2ohpgzdsy.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2zillqxqt.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2mqnpujdf.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2hbrninwx.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2ctsckwuw.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2gllizjyc.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2vkktpkxm.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2arlgcjcb.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2vqzadxnv.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2cmsyqryy.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2hiswolmx.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2bopzgxpt.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2wysqwxfc.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2giddvqpa.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2khyunihs.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2fmjqxruc.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2xjxbwhda.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2xwbyeupe.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2qcppznjf.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2qjvvtrtf.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2vatqlrbr.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2bkrfwies.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2cqfjhebp.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2psxdfwam.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2pqyncsjw.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2hscvwnma.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2mcbwouij.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2mxiocphb.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2wztljivz.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2abtgndrq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fuivbdpa.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2iotavjfi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2omnyfeoj.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2zuzajqmn.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2tdisrkps.html


<!-- 参考信息 -->