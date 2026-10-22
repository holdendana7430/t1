代发 wailian999

LEFT JOIN employees m ON e.manager_id = m.id;
来源：http://www.ydjk.org.cn/Article/details/gt2liiovqnz.html

[Q40] 交叉连接（笛卡尔积）
来源：http://www.52xcode.cn/Article/details/gt2vknbifog.html

SELECT * FROM colors CROSS JOIN sizes;
来源：http://www.52xcode.cn/Article/details/gt2hfcouevx.html

[Q41] 多表连接
来源：http://www.52xcode.cn/Article/details/gt2hgyicsso.html

SELECT o.id, u.name, p.title FROM orders o
来源：http://www.52xcode.cn/Article/details/gt2hlcgiqpe.html

JOIN users u ON u.id = o.user_id
来源：http://www.52xcode.cn/Article/details/gt2misueygt.html

JOIN products p ON p.id = o.product_id;
来源：http://www.52xcode.cn/Article/details/gt2iepgofax.html

[Q42] 连接条件附加过滤
来源：http://www.ydjk.org.cn/Article/details/gt2nxixhbsz.html

SELECT u.name, o.amount FROM users u
来源：http://www.ydjk.org.cn/Article/details/gt2ejncvivl.html

JOIN orders o ON o.user_id = u.id AND o.amount > 100;
来源：http://www.52xcode.cn/Article/details/gt2hpedepfv.html

[Q43] 标量子查询
来源：http://www.52xcode.cn/Article/details/gt2eqttfzjf.html

SELECT name, (SELECT COUNT(*) FROM orders o WHERE o.user_id = u.id) AS cnt FROM users u;
来源：http://www.52xcode.cn/Article/details/gt2uaidgisv.html

[Q44] IN 子查询
来源：http://www.52xcode.cn/Article/details/gt2fdirnzku.html

SELECT * FROM users WHERE id IN (SELECT user_id FROM orders);
来源：http://www.ydjk.org.cn/Article/details/gt2orgivfwx.html

[Q45] EXISTS 判断存在
来源：http://www.52xcode.cn/Article/details/gt2noojcnfp.html

SELECT * FROM users u WHERE EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.52xcode.cn/Article/details/gt2zlzhdlso.html

[Q46] NOT EXISTS 判断不存在
来源：http://www.52xcode.cn/Article/details/gt2inezoqdy.html

SELECT * FROM users u WHERE NOT EXISTS (SELECT 1 FROM orders o WHERE o.user_id = u.id);
来源：http://www.ydjk.org.cn/Article/details/gt2enyxmnod.html

[Q47] 与平均值比较
来源：http://www.ydjk.org.cn/Article/details/gt2ilxfyfqr.html

SELECT * FROM users WHERE age > (SELECT AVG(age) FROM users);
来源：http://www.52xcode.cn/Article/details/gt2tedvyfwb.html

[Q48] CTE 公用表表达式
来源：http://www.52xcode.cn/Article/details/gt2lnpzwcrh.html

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://www.ydjk.org.cn/Article/details/gt2yoafaypu.html

SELECT * FROM t WHERE c > 5;
来源：http://www.ydjk.org.cn/Article/details/gt2jicrazax.html

[Q49] 更新单行
来源：http://www.52xcode.cn/Article/details/gt2yuxxnzdn.html

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2fgskljrd.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt2yyqkxtgm.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2ztvwhgjr.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt2hvnqtkyi.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.52xcode.cn/Article/details/gt2atiajgbn.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt2rtvrxaeo.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2aqiaawfp.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2nxmekmyi.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2fqyfsqcr.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2qfxzmmeb.html

TRUNCATE TABLE logs;
来源：http://www.ydjk.org.cn/Article/details/gt2luhgoyui.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt2tofyjior.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2zdtpgohy.html

[Q56] 密集排名（并列不占位）
来源：http://www.ydjk.org.cn/Article/details/gt2tnudzbgn.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2thodfqfb.html

[Q57] 行号
来源：http://www.ydjk.org.cn/Article/details/gt2bewrzuuv.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2tnthdwzo.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2unslwldo.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2vjcyhuuv.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt2iwcrsvaq.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2dkbrcoqo.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt2fomsmxua.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2wbzxtxkr.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2elirmavs.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2umsdazjo.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2vltuukgu.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2wmjogrhd.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt2xuabyhlz.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2xtnestls.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt2iewwfjhg.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2wbkzvkhi.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt2ywiesjrw.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2hvlyoeig.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt2wmrevusi.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2wjjavxdp.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2nljxevax.html

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2mdnagepl.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2tpxwtezu.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2dohoibkt.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2mrvjxjjt.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2jeuiwult.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2tzhidtgr.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2eigqskwl.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2obpyjmnv.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2mpmowfal.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2palpanfx.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2drhmebwx.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2qgjtfkth.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2acqocoqp.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2htihqjqc.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2jpozhkjc.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2ebsdhurf.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2cbhzeopz.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2dftmiirf.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ryahvhtq.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2zpdyxtls.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2uhoteaqh.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2fkmgmbrz.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2bubltnxz.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2ofrnmxsb.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2levcpuna.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2gewuuesq.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2howajzmt.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2zguvpsqo.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2iwmcoxzo.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ilqaknjv.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2kohjqxep.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2wkfldiiv.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2gqeivqbw.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gprmjlbw.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2egeyjrwv.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ctcbqbcy.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2tokvgqqo.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2pkpiztdu.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2hrvlyowp.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2uospugnm.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2sdfjjmmc.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2ywccztzq.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2mdxpkqai.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2uphyddgi.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2vricaaqz.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2ggbrvlgp.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2upfbndnr.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2msozeald.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2kthnchcu.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2pirhgfid.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2rajvxbby.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2crbjpexq.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2jmhyzdka.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iuqpvpjd.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2igppjeha.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2eftyzkom.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2pqrxxwdy.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2qjhtlijy.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2gnitpjct.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2yeeltyfp.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2prokfbrl.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2tkvgdgcb.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2jpvnrbuq.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2rqlnzswy.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2qgkcpknc.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2lwscyjyi.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2bxupmxzb.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2mmgisyib.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2pcxhhjtt.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2ilucssfe.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2tjubgrxy.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2qpfpguae.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2roczlnue.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2mexiehqf.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2ivxvodha.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2vqzfqxeu.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2ihsooqhy.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2qvgusjbe.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2yuzyysxy.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2cnlgicny.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2ygynkmep.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt2xacmnmsr.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ublfnfuo.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2airgkgkz.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2phmnpnoe.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2lqmyqyex.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2smkjgozz.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2qjqjrmyu.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2xunnxwau.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2qptexuqg.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2nuxyoogu.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2csjedfyz.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2riaxgogd.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2qilodhry.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2rbefcsac.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2tmbymfyt.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2nsoybfnt.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2syguiduk.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2nauvuiht.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2gwbfrjdc.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2trqrrnhy.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2zfzmpdmk.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2sigsfvxj.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2nkedvrhx.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2blkdzhnx.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2lmgqtrku.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2eqwgvcgu.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2tjnfcihv.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2orctlfxh.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2umdmnqcv.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2treulgfx.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2jbbwrmcu.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2mmdtnvuo.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2elxnuhtm.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2wpxykzen.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2eeclixvs.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2hnhsdwih.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2rmrvimqw.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2dbgtdzlv.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2owxuxnap.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hqrovkbd.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2lknkfxlm.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2mwrcgnvv.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2dfkaooei.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2mbtlqugf.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2rylqyzgw.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2eadzbznm.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2jnwimkkb.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2gcmupmms.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2lfaipybq.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2vgegabbi.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2pquhwxaz.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2lvnpuxjv.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2exudnvah.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2aoishkbf.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2bxwokdul.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2lrhmtgru.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2saoawear.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2qhiwauoh.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2vtqzvxdo.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2pcppqxtz.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2eaeutpbb.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2xsnnvgun.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2delyicdh.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2aqyfjtjq.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2evdmhsqj.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2rmhqkpay.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2nleuirqd.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2fxprlfvr.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2zmbstkgn.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2pstdoioi.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2yyuwpmsh.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2eyfdnfrk.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2paejofdz.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2sxmytprc.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2vbmcpoqu.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2ylvnngvw.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2qjecbfmt.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2otjltlqu.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2yuqosunb.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2ybklagod.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2mezoshkj.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2knjvlpao.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2dhqqhuhk.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2ctalpjul.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2bpknncxa.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2jpqgcxpc.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2zldyrufk.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2qjthgthg.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2ihavxvkl.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2itcghqof.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2flgewlrz.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2nyecgceh.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2rqhatdhb.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2cmmijpml.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2gipamjhx.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2kprlkdia.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2jlnttbhl.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2wahzqtnj.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2jocvkxli.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2adbgsezt.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2igwtnqvu.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2yocxasyh.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2prfkthqj.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2msalxpux.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2vkandchy.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2pwouxiql.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2crvpieee.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2svpzphpo.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2jrbdsbvb.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2gysysxnz.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2lqcqnkvz.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2wuxmrfet.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2jnstwbqd.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vxpddxim.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2bftplcnk.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2dgtfedcd.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2htjulrzn.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2fhtwmsoi.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2dsfczkvs.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2xigvijpp.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2gqtfbsuy.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2paudnprq.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2inbthecd.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2nriucavy.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2ewzlfdmf.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2wpfyrfzj.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2vmperknq.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2looxseop.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2zruyrzwt.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2xyuizjav.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2bkvozkkj.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2fuizcavq.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2lnyjnblu.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2zartjhai.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2tmiorecz.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2ysejcqdq.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2vuwwoaij.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2bvrjvjpq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mvvwymgw.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2bvocyyje.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2csqorzbb.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2uhnoyjgm.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2msufapff.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2ksxgpkmj.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2cxsrifsy.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2ixduzojb.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2ysfhsvyo.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2cekdcxan.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2hgqvjfhn.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2rsdeivqj.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2gibvwezg.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2misxuesa.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2jektucft.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2kinxjdwx.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2apneyitj.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2xjlmueex.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2bfbwfjwl.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2tkhjidws.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2dtachrne.html


<!-- 参考信息 -->