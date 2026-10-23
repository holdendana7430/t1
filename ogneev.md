代发 wailian999

[Q38] 全外连接（PostgreSQL）
来源：http://www.52xcode.cn/Article/details/gt3zkgxofkc.html

SELECT * FROM a FULL OUTER JOIN b ON a.id = b.a_id;
来源：http://www.ydjk.org.cn/Article/details/gt3ksrhsuip.html

[Q39] 自连接（查上下级）
来源：http://www.ydjk.org.cn/Article/details/gt3ubhrwynu.html

SELECT e.name, m.name AS manager FROM employees e
来源：http://www.ydjk.org.cn/Article/details/gt3eqwddnvp.html

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.52xcode.cn/Article/details/gt3emzmeiic.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt3wkrxeoll.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.ydjk.org.cn/Article/details/gt3fniqwqpu.html

[Q41] 多表连接
来源：http://www.ydjk.org.cn/Article/details/gt3sqymzkpq.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.ydjk.org.cn/Article/details/gt3cefnhvcn.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt3qqmsrttx.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt3ndlrzxqk.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt3iyjmaerq.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt3hqcgdjql.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt3bsniqbaj.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt3qeowfhwc.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.ydjk.org.cn/Article/details/gt3zdhiaeqo.html

[Q44] IN 子查询
来源：http://www.ydjk.org.cn/Article/details/gt3zutbbsdo.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.52xcode.cn/Article/details/gt3tmdajseq.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt3plqadmav.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3yhbcdjxw.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt3kquxqqfg.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt3waughksr.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt3rgpjaqdl.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.ydjk.org.cn/Article/details/gt3qcsfgrmy.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt3naxmnjib.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.52xcode.cn/Article/details/gt3amawaqqh.html

SELECT * FROM t WHERE c > 5;
来源：http://www.52xcode.cn/Article/details/gt3euontoej.html

[Q49] 更新单行
来源：http://www.ydjk.org.cn/Article/details/gt3crkgfbme.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3bvezfdsi.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3wnvqsovu.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt3jmodvwzz.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3zzxgasge.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3jodxoybs.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3jvkgwbkp.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3hznttgdp.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt3rwuogakp.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3jxrjebhm.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3muppmvsn.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt3hvuscfok.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3ivmxafur.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3hxxwgyof.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt3fgafmaxi.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3trjmqmje.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3hlpspebq.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vxjurcsy.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3mjoxmlrl.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3mmnkorvg.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3omwtpsrq.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3bifnapbj.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3paimhqfc.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.52xcode.cn/Article/details/gt3laetazhn.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3wtztpayo.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3vbrliejt.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3zvhofgzp.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3dsaghvim.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3ojndqfrc.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3rtztqbdt.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3oliopopm.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3jgopxfwx.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3mqlaifei.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3smdfaxpe.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3miyhvdrv.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3bplmrfde.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3emfcbqmz.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt3vmyzoxvg.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt3slifdakc.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt3agnzvzkb.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3bgcsymej.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3tsdfobto.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3aovvxpod.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3rqukalvs.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3ypwitzpj.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3wiqpdsjl.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3lwtffovs.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3dngeyzzs.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3azazcatt.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3qwxoairz.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3ttcdbdlj.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3wzmydjww.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3xefovihv.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3rhheahla.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3lxqcnasc.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3vopqjxey.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3styczqvw.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3vreonxui.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3ivqquqgg.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3kipcgmxj.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3gqhfxcua.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3jadnebja.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3nkwfmtgo.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3heltbwnz.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3dredsjaq.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt3hvmjtgkd.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3wedrokwx.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3rckblxge.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3swplncyl.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3iegimwkz.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3rhfkbzrq.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3vpggtool.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3pdcvenmg.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt3kbjrsmma.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3jrhbiwbb.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3ygzrevia.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3jkjbejiq.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3hwzkqlwv.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3tyjfpimp.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3ijcsqtsd.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3jutlamdc.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3hlwjzoig.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3veklymlf.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cgfjvsej.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3kyqcpncd.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3zdutwazh.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3lbvbtmuq.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3hhifigtd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gxylrvcv.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3mdnjecmi.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ieopggxw.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt3libiaxbw.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3juycgowh.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3tlutgvho.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3pymmqiyr.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3ngeyzour.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3mrbytxib.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3lcqvzkqa.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3qrejtxpf.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3ysktayou.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3okxdvimy.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt3pchdarbm.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3mgbyuzpu.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3dhuhsqyx.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3zhpirfpy.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3pkixjbto.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3ouuqhegq.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3eqjzrgoa.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3sdngniis.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt3pdcxkagk.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3svixobwb.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3hrsikdrb.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3egfnwcxu.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3ivmvhupr.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3exrmpueu.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3vlcomwqu.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3ttujeijn.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3mbnhovje.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3zrgindim.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3gzpgsclc.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt3sjpapqgn.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3qvebwamn.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3knskvlhd.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3nmhumbcx.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ccjicdjo.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3elffvzgm.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3xolxxyba.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3uqmeexts.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3aifkoncr.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3bmtbligd.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3itqoynpo.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3enoxufpi.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3tssnzayx.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3ednktnqc.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3pontfaxk.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3ibfgbacg.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3xlqdldlw.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3rqsgvvkn.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3gcbvscav.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3daphpsdu.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3cbbiurnj.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3neoaxpus.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ewmhgctn.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3dsslbmjq.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3qeodjmcg.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3dwyxbyrd.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3zhmlsfip.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3ocdullre.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3fdpooxui.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3jedotdse.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3kscjpgqb.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3ltrsblep.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3vflpeyhk.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3wrchqujy.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3fauxakcc.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3bygrujpe.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3maqulafu.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt3sjymrfhy.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3dnxzkpoa.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3relmumup.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3kjdfoxyu.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3xefunolh.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3rawqpfad.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3zahtfjgy.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3sjgasste.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3brcgkdvo.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3kxvtvxkv.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3bxpcdigh.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3vhjxezic.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt3yqkkewzp.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3ruxipzya.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3tngpiyqv.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3prijndbp.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3ltrgtitc.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3ovcarylk.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3jfmmudqr.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3pezskaed.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3ogrbmtqw.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3kcuhyefz.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3cckxhkoh.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3tssktder.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3aqdjuemy.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3dwmdlywu.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3tolrtmfh.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3ljkvghqu.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3vzvytkuy.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3hfzlyhgr.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3nrflhuah.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3kdrrrpzg.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3fmwbzdbj.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3cffygmpy.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3jxxzpkpv.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3szmfbacv.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3exmdygie.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3srpezawi.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3jfvgefla.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3bosrelqr.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3ixgrhnlw.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3bfopflpj.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3scbvvxpf.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3wjhpdans.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3tqnsdkmi.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3qdzfksfw.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3khfcaypn.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3kcpdyhse.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3qledljbb.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3nmpbagfe.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3gukirdja.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3nmhtmobu.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3qabddpbg.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3haqlkxkw.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3zojoonwr.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3fcpivvfh.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3bhnaogzf.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3jsqkntsv.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3puctmjat.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3bpdoctxs.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3tqnfvxli.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3rrgpjrun.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3jcaismfs.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3xtmohjnm.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3ltttgplw.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3ydfprucv.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3cyegsapv.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3scrvuhkp.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3kpojwxsp.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3ixklcvji.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3ekgkygdm.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3hbswndgu.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3lhdhkvmq.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3nxzuimlq.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3mqwlmdtu.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3cjlbfhld.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3vlvtzigq.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3aqruugmk.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3akagzuwt.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3bdrxabaq.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3tcogwavs.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3qyquilii.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3zyyqwzak.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3ekurpmno.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3nbeapiqq.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3czhpcbpi.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3lsjuvwrj.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3nzwueyks.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3cdwudlji.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3titifgde.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3exauqqkn.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3zedngoxi.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3yykawxci.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3itzelvrz.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3hiufxdyr.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3natjipnh.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3bjfppbon.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3hnvmfpzh.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3hzuxdevf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hfrlcnap.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3zvslzfjj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wavjkduf.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3tbdgzbxc.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3sliioxqt.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3yhxxxpta.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3zorfbqxp.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3izzwzwyh.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3lcaivyul.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3aqjivhzf.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3azaanobl.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3zqaobsgx.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3qktinqac.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3jilzcwjr.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3nqldaxwi.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3wfgmbudr.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3cgaykuwt.html


<!-- 参考信息 -->