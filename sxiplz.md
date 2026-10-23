代发 wailian999

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3rbahnlut.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.52xcode.cn/Article/details/gt3kfkxoyru.html

[Q39] 自连接（查上下级）
来源：http://www.52xcode.cn/Article/details/gt3zpkfzttl.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3xvedmpho.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt3knfrjdhp.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.ydjk.org.cn/Article/details/gt3wkberdau.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt3vwthqutu.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt3evnjixhx.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt3aamrjfuz.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3azkgohxg.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3hlutadwo.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3mgghpiek.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3srrkkhcy.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3suvrwvnp.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3zgljtlqm.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt3kusiinmr.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt3phuaxszk.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt3xqhvlsmf.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3djrcfmpe.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3zdagzxyz.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3xqwegosu.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3doqxgqcf.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3xmqbhahq.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt3orxfyuxs.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3wwucyxnu.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt3linxrpwj.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3taijnflz.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3qaotnrrg.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3teoswfsw.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt3dyuwbtqz.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3azvdgqrc.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt3odxprpdp.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt3untvztlz.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3icfbdipx.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3istoyfzm.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3txafwzxr.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3cqvmbjbx.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt3faeyxqyr.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3kybmttyy.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt3seerkapo.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3rupsxxkd.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3kztbokwi.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3hukqrzww.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt3hccgpbfg.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bswhuscx.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3slirgnsq.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3pdudsxfx.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3cywmvjwm.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3vqydlzon.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3zrtmzkxr.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3vdpkhqcl.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3acezuala.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3vueojqxx.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3tyqyghiu.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3nrxuphyh.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3aqumoytt.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3qdfjkfuh.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3jbdofafl.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3jdhqjqnk.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3kzjsxswn.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3vwsfulbv.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3gcdcaakj.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3aydrvwdo.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt3qbvsvauk.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3pmahzpns.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3clrdrcuq.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3texhpvfz.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3vjwkwjeh.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3emiknuej.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3wmbjdpuq.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt3zaxhklxh.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3bzeootna.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3yrxqxvgn.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3ylxuxudx.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3qlycdfhq.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3nxdtmonn.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3kbcqhwxc.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3hvphmqde.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3nbxruyrv.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3kuhbdued.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3hpxzvlnd.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3kyiyuben.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3bxughvlm.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3plroyfyu.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3vqqhqakm.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3wtyryhgl.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3ubduchyj.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3tulfkrye.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3knsybmeg.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3vgiufjnn.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3abetdlqi.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3oyzyxsbs.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3mhthnswa.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3sdabfxwk.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3nlbejehy.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vucirpwb.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3ttyxoudu.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3uyhvhwnl.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3xrclvvod.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3ezxnvgcg.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3gyldyblh.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cieybdfb.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3swntxxns.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3rhzvhdrx.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3sqdhbsco.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3ceyluikm.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3gxaacply.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3dcijxzhw.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3cgkfukau.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3zcggqtvi.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3xtaztwfp.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3ihdrbfwj.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3lccmmhgm.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3jzjzumwm.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3tvrytdoo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tqxnrkxh.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3acdrdjza.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pswfpkhi.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3gvmmqjxf.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3tfopbolm.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3sxvpolgk.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3kfyzfhnd.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3tbfkbcsl.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3vvqujloa.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3luyvyfev.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3zvfqgmxj.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3qijzlsyk.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3mhqghmtd.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3wvsrtbts.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3neinfqlb.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3itfwxxmu.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3vddmhdfd.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3uxeybmyd.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3fhsyinqb.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3lyidxhiv.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3hrhwjxue.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3qgbtqohd.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3murxzfjl.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3ezrryfjr.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3eaffqgeo.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3uubpqjaa.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3myyepcrq.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3gcobywpp.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3llrazmjg.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3byerjqxp.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3nqvxjvtq.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3iwrourhz.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3hmajgshs.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3sqproqkz.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3mfhyncpa.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3ikgdwrcs.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3qgaelxzk.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3osyicdfc.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3mocfxgyi.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3dgaqektl.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3elfjxjgp.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3owrhexbw.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3xqptebom.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3jmpstknn.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3vzombqce.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3wblpyfsw.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3iljvkgkl.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3fwtrkzfv.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3dbtrwaeb.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3uwotrfyd.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3tcjnpvho.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3mfcmioxo.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3guaixbym.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3mcxixaqc.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3zpyvralq.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3jnmqidaf.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3hiykgtzs.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3krhbafkr.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3rtlzjqur.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3iwnqsywe.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3rcerzdex.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3eiwjfoxs.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3wvtukcqm.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3oukjopso.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3cxhguovz.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3ebkhmkts.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3utlswdtq.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3adohjhmm.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3fvhtovku.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3xvauxaav.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3chajuwvt.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3tvcsoqth.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3kpvwabjg.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3fhqfwmmp.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3alzwmlqb.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3nlzwazys.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3mvdcuwsz.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3rugcctmt.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3oizdjcip.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3msgiitve.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3qvepvdqg.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3ekebdxks.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3gqcxltwm.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3xvvjgexy.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3duizaxnw.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3qjnwetcq.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3bnjkqmvj.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3awnammld.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3omuwjdrm.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3pmppklbb.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3qliqzqgt.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qfohsyog.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3lkntlytj.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3mfvfuboa.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3dcqgttep.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3wggzyqyz.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3cioomihh.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3mhztcywx.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3bqcgqnbp.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3sburgnmr.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3zzcdzpsq.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3mjdlgsds.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3kwegryfk.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3ckdobfuu.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3cybheenk.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3ltulfmvf.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3nnbrgybn.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3mlnznwps.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3ebnkkxbe.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3gteftavb.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3cadrxoht.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3dctedshs.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3hxzkuxse.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3zgepxqps.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3qheerfuo.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ijhbnnkl.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3dsqragpz.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3jscuvfhu.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3vdkpjmmk.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3bfbymwqc.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3kfzhrnkf.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3taatwgys.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3jrkzntzh.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3jxaqfyej.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3rctvyjim.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3lckaplbf.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3hujfgwzp.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3nfxadsck.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3xjicytnj.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3kkhoeykl.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3pzcqxskw.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3pffvrtug.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3bcasvjqq.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3dbemozme.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3kttthuho.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3yhepwptu.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3pqdjeysi.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3procycxr.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3fgcjhdym.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3emifkuuf.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3rkaubwce.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3irrexgef.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3mtjgpgzc.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3qnxjolms.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3okaijnqy.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3xjlbdqon.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3pgoulflx.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3leomntho.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3pbfrdfay.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3maarwljk.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3qhlpmgja.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3fleejoyo.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3cxqrqksi.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3zlyvsivp.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3rnxincyo.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3tswaraym.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3llzmsjze.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3sauelzyx.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3vlcyelli.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3dwaatufi.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3dmtkyvoj.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3arjzcled.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3zzcujmml.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3fhnvwqxt.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3knlzflvy.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3wnbhuhrm.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3buhatcfy.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3qnzgbdmi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ehszklne.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3sdramiqu.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uujgrqjn.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vbrotoyn.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3coxmmmvs.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3bnwujytd.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3fyitfgut.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3kwbsrrcd.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3hozylwpj.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3czidnswe.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3ifsjezok.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3xdgkmzcg.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3hqruhpuq.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3mutctftj.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3ljrwtxny.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3adomstfk.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3tucrihnt.html


<!-- 参考信息 -->