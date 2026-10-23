代发 wailian999

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3kfoqehcg.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3mvliwpla.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3dapzpldg.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3akqhzgps.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3wnrhszhe.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3vnkucgpi.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3msuqygoo.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3jgvfnoae.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3poajclxj.html

JOIN users u ON u.id = o.user_id
来源：http://www.ydjk.org.cn/Article/details/gt3uzehjibe.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3yimjltkt.html

[Q42] 连接条件附加过滤
来源：http://www.52xcode.cn/Article/details/gt3qmkzkzre.html

SELECT u.name, o.amount FROM users u
来源：http://www.52xcode.cn/Article/details/gt3zinmuoxk.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3vwxlszfw.html

[Q43] 标量子查询
来源：http://www.ydjk.org.cn/Article/details/gt3vtaydwyn.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3hvjzkjpf.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3tjfnyeor.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3fuclbsqx.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3vdaibyte.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3pxyzqktv.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.ydjk.org.cn/Article/details/gt3wowedcpd.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt3typcevxq.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3mwmytmct.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3txlhzian.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3xxgyrpvg.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3hzltuunh.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt3mwzatxre.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt3hpnbyoqm.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3xslteexo.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3chvvdscz.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3bjvstbbl.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3usyrggzv.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3hlgaldao.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3pstrtlff.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3lkffjpkm.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3suwqyfoz.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3ehrktcrx.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3sqrybift.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3fxayjvax.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3odbhldzh.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3mxygmlyn.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3clxulljt.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3cwqdctni.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3ntcftnix.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ecxgqesy.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3haepozli.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ycloxdve.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3rddkxdiy.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3etlvofop.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3mafqvlhb.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3wiisuckg.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3sybpvyri.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3fzzfecix.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3kyrufiml.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3zcywaeop.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3bhabtrad.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3xikgjick.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3bhfaohsu.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3fbsvxcvz.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3igdfpgdo.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3shuoygnn.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3eaufhqxu.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3pxtvhhfp.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3lsefagzk.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3lergsjrk.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3nwbkoavv.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3yrehubqr.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3jcoyhyqr.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3gpwwlbfv.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3ufwbvbnh.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3sfyginfw.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3oykmbmiv.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3waaruugy.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3pngzgxxh.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3vxxpqzrj.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3ksvhdlgj.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fazfwaqg.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3nmmfiihh.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3kzveysfp.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3enbuwqcl.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3mwjmnwbl.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3liinkykc.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3tnoouvkj.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3tmqkqnkw.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3nuoituqh.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3zwmyzoos.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt3qotneczs.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3qgcczkag.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3gcvjaeuy.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3zzadkmhp.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3slwxpedr.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3qvurnkhn.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3gzhguphi.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rucneesd.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3fudarnwr.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ggnhiyob.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3sxmmmmai.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3epoehvbs.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3jqaeegyu.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3phkotuhl.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3rkuigtlg.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rdtevfep.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3tiaxdmzc.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3sbbfaktv.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3kyfxrisu.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3qycslkil.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3nfilttsm.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3jbghbodc.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3nkeokxlw.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3avngreme.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ockcmufo.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3fvoaeglo.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3afyxlviq.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3zawfpqdy.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3muzvusbt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3djengcat.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3vcrzgzfa.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bpglexhf.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3cratuzpu.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3acgtlmbq.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3hlinnnne.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3kmrwdddl.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3wkjqtoxr.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3cpnxkloq.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3cfacrcyh.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3asjmakpe.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3ccaaxtqs.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3ocgnpces.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3tsjwwcyx.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3jxjyjxku.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3vgbwgstc.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3vfctgncw.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3qasuxibn.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3ntnzesrk.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3iiuutgvm.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3kxizwcam.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3rappnanr.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt3tephehrx.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3glltaxnr.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3tosfjswt.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3iadewagg.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3nolcyucm.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3xbhrnzff.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3eayrhfyd.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3dyhtsyqp.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3rpmsytrg.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3jezmekyv.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3outwltld.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3tkukpebs.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3wfwzkwne.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3apjmiluj.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3aulzxcek.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3zocmrhgm.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3mkcwkgnk.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3qjjhzoyo.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3utlwcyzw.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3nqkbpotg.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3bjpaiqbh.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3stpdcbac.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3lhxlhcgm.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3wbvslgwe.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3twtpkrkv.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3slqvlakf.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3zicjiuvj.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3rfqduzyn.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3vosmqelf.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3xosdwzkh.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3fxtwyfzn.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3ctzvpifk.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3gfunlhnj.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3fcfsjuij.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3xvahhjti.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3vvlrlouf.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3cleibmyx.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3srhacywn.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3ebfngblu.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3eakagfnn.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3uxkrkzzh.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3vlmznmjn.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3darqpslx.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3upootmnf.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3oyvwcplk.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3ntinnbiy.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3pbdcdwzw.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3qwindiaz.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3atwrbtwi.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3ktwhsctj.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3shgkqymh.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3eiobhmeb.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3frjrknzx.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3fkcqnljr.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3qlqeawsr.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3ltflsycj.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3omefbhjv.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3vbhvempf.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3axnqsajt.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3cdjjeyvx.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3rbajrjpf.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3wvpiqwrr.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3jspvkrvb.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3jxdgkezt.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3bgqflltp.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3jncuztis.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3wxmdgckh.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3gakcydfu.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3ddhrmaep.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3weurmpvv.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3qhxycaof.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3hjzjzksy.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3flrptkxb.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3zgsldxmb.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3vhpyregn.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3xbizjdsf.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3hfficphv.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3lesatdxx.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3nbkzjctx.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mpzfoyqy.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3hcpxvsaa.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3eskfsnpc.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3qakdhnfw.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3aomcjthv.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3jdbkmhjw.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3cvpwngbl.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3tgwpcsha.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3iqicbveq.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3ahxvamkt.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3kxvhsxpa.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3qrzcjgdd.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3zasaclfz.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3jnoaoqwd.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ytjbqzpq.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3cibzjzqo.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3nlkfveby.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3eqdvlgvc.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3ealmhebb.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3cjldbglc.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3cncisckr.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3zhilhhwa.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3yolswbyl.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3bhrcwqfx.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3wjdvtxex.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3oqcgkiss.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3ruoyraot.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3roptckmm.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3uktevnpa.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3kwkkmtkf.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3suvwyslh.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3ltzdvmfr.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3glbynfsm.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3szdzpims.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3vcwebhal.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3kauxvnrs.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3yhdqfsyr.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3dbjfpxyd.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3igvyqups.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3xssekeix.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3dzkkoakt.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3nrufarpu.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tuzlsxxd.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3mxkcverm.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3kjtymcna.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3ocllqthf.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3pavymoua.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3lwpxkkma.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3dhgqhouq.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3wcnpcrnv.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3grwocuug.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3jjfmyatc.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3kyerlcdr.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3bwhhbtpl.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3mputhqzl.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3twtdgtry.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3dtluqcbn.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3odtviotu.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3mgadhryn.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3enltfqmx.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3wbulamdm.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3tavkxsas.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3uknngzlp.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3dugqtwwd.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3wzhuuqii.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3fjednzlr.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3ohyrjfvu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hiqdwrxp.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3aosbxbcg.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yztwjdrs.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3wpxgpxed.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3hoaapyjp.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3wppezfmv.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3tysgdfrb.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3ihhaxkkj.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3mzmedoaz.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3jwliebcv.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3dqnzwujw.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3vqennfos.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3qvtklzoe.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lbrwgwzj.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3wnazagbb.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3ynnltecm.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3igfnmtjr.html


<!-- 参考信息 -->