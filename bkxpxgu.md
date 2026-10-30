代发 wailian999

[Q48] CTE 公用表表达式
来源：http://read.share.fanxiaobao.xyz/Article/details/grxcybykh.sHtML

WITH t AS (SELECT city, COUNT(*) AS c FROM users GROUP BY city)
来源：http://blog.fanxiaobao.xyz/Article/details/gzbfpbgjf.sHtML

SELECT * FROM t WHERE c > 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/gxyjyebmj.sHtML

[Q49] 更新单行
来源：http://read.share.fanxiaobao.xyz/Article/details/gwdeztpmb.sHtML

UPDATE users SET status = 1 WHERE id = 10;
来源：http://blog.fanxiaobao.xyz/Article/details/gnlswhlxp.sHtML

[Q50] 批量更新
来源：http://read.share.fanxiaobao.xyz/Article/details/gsviypcby.sHtML

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://blog.fanxiaobao.xyz/Article/details/giytsdpkk.sHtML

[Q51] 用子查询更新
来源：http://mobile.fanxiaobao.xyz/Article/details/gkwbvpzgu.sHtML

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gkxxbefjv.sHtML

[Q52] 删除指定行
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzkcwajsl.sHtML

DELETE FROM users WHERE id = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/ggdxibjoh.sHtML

[Q53] 按条件删除
来源：http://3g.fanxiaobao.xyz/Article/details/ggzrporkj.sHtML

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://wap.fanxiaobao.xyz/Article/details/glbbcjrve.sHtML

[Q54] 清空表
来源：http://www.share.fanxiaobao.xyz/Article/details/ghxtojqed.sHtML

TRUNCATE TABLE logs;
来源：http://baike.fanxiaobao.xyz/Article/details/glzfopkaf.sHtML

[Q55] 排名（并列占位）
来源：http://m.share.fanxiaobao.xyz/Article/details/gprqptnal.sHtML

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://mobile.fanxiaobao.xyz/Article/details/gcrfnwdtg.sHtML

[Q56] 密集排名（并列不占位）
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghjtrtybw.sHtML

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaiutpzuu.sHtML

[Q57] 行号
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdnnkryfz.sHtML

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/ghzdpyyve.sHtML

[Q58] 累计求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gzrohklxm.sHtML

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://wap.fanxiaobao.xyz/Article/details/grbbfwxbb.sHtML

[Q59] 分组内累计
来源：http://read.share.fanxiaobao.xyz/Article/details/gznbiwcba.sHtML

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcgqkkgqt.sHtML

[Q60] 取上一行 / 下一行
来源：http://read.share.fanxiaobao.xyz/Article/details/gdlosuqzg.sHtML

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://read.share.fanxiaobao.xyz/Article/details/gyofutwbv.sHtML

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://3g.fanxiaobao.xyz/Article/details/ggyutbzcy.sHtML

[Q61] 移动平均
来源：http://www.blog.fanxiaobao.xyz/Article/details/gooxviwgl.sHtML

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://read.share.fanxiaobao.xyz/Article/details/giwnlcuxd.sHtML

[Q62] 分组占比
来源：http://baike.fanxiaobao.xyz/Article/details/gbfpispjn.sHtML

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.share.fanxiaobao.xyz/Article/details/ghjycwgjo.sHtML

[Q63] 开启事务
来源：http://read.share.fanxiaobao.xyz/Article/details/guxgzxxyu.sHtML

START TRANSACTION;                -- 或 BEGIN
来源：http://www.share.fanxiaobao.xyz/Article/details/gkogxnrgs.sHtML

[Q64] 提交事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giqojbyqq.sHtML

COMMIT;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqktfgohz.sHtML

[Q65] 回滚事务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnxgsbzxp.sHtML

ROLLBACK;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzcqbrvnz.sHtML

[Q66] 行锁查询
来源：http://mobile.fanxiaobao.xyz/Article/details/gvktclkdw.sHtML

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.share.fanxiaobao.xyz/Article/details/gecbnswrr.sHtML

[Q67] 设置隔离级别
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjcblwnsu.sHtML

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://3g.fanxiaobao.xyz/Article/details/gdkrbrsdq.sHtML

[Q68] 保存点
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmmbmrcxx.sHtML

SAVEPOINT sp1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghzkpbyao.sHtML

ROLLBACK TO sp1;
来源：http://mobile.fanxiaobao.xyz/Article/details/giyowikie.sHtML

[Q69] 查看执行计划
来源：http://baike.fanxiaobao.xyz/Article/details/gztfdsdsj.sHtML

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://wap.fanxiaobao.xyz/Article/details/gwpugbaqw.sHtML

[Q70] 更新统计信息
来源：http://baike.fanxiaobao.xyz/Article/details/gzqxwgczc.sHtML

ANALYZE TABLE users;
来源：http://3g.fanxiaobao.xyz/Article/details/geokduwdh.sHtML

[Q71] 查看建表语句
来源：http://baike.fanxiaobao.xyz/Article/details/grvfjcrzv.sHtML

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.share.fanxiaobao.xyz/Article/details/gxyazeilb.sHtML

[Q72] 查看索引
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtkxpnmol.sHtML

SHOW INDEX FROM users;
来源：http://wap.fanxiaobao.xyz/Article/details/guogssqun.sHtML

[Q73] 查看表状态
来源：http://mobile.fanxiaobao.xyz/Article/details/govgvrygu.sHtML

SHOW TABLE STATUS LIKE 'users';
来源：http://m.share.fanxiaobao.xyz/Article/details/gdnagzxgi.sHtML

[Q74] 强制使用索引
来源：http://blog.fanxiaobao.xyz/Article/details/gbxqfwrhv.sHtML

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://baike.fanxiaobao.xyz/Article/details/gmqdfkkaj.sHtML

[Q75] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gkqmahwck.sHtML

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.share.fanxiaobao.xyz/Article/details/gidqivpzz.sHtML

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://read.share.fanxiaobao.xyz/Article/details/gsigugjml.sHtML

[Q76] 按天统计
来源：http://blog.fanxiaobao.xyz/Article/details/gsgkedecf.sHtML

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://blog.fanxiaobao.xyz/Article/details/gfdwcknkq.sHtML

[Q77] 时间加减
来源：http://baike.fanxiaobao.xyz/Article/details/gqrilomfk.sHtML

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://wap.fanxiaobao.xyz/Article/details/gonwfcuan.sHtML

[Q78] 当前时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gobwfdowi.sHtML

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://wap.fanxiaobao.xyz/Article/details/gqfweecze.sHtML

[Q79] 字符串拼接
来源：http://m.share.fanxiaobao.xyz/Article/details/ggqyftobh.sHtML

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://blog.fanxiaobao.xyz/Article/details/gwiibdolz.sHtML

[Q80] 字符串截取
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvnquhbij.sHtML

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://read.share.fanxiaobao.xyz/Article/details/gkvbmsmit.sHtML

[Q81] 字符串替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gppiusdhg.sHtML

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gascseptv.sHtML

[Q82] 字符长度与字节长度
来源：http://read.share.fanxiaobao.xyz/Article/details/gahmoeefg.sHtML

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.blog.fanxiaobao.xyz/Article/details/goqtnigez.sHtML

[Q83] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwnjmmcir.sHtML

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://m.share.fanxiaobao.xyz/Article/details/gpgybnvos.sHtML

[Q84] 去除首尾空格
来源：http://wap.fanxiaobao.xyz/Article/details/gphdrxxee.sHtML

SELECT TRIM(name) FROM users;
来源：http://www.share.fanxiaobao.xyz/Article/details/gznfyfjmc.sHtML

[Q85] 数值取整
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbjylkkyx.sHtML

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.share.fanxiaobao.xyz/Article/details/ggnujqxpw.sHtML

[Q86] 读取 JSON 字段
来源：http://mobile.fanxiaobao.xyz/Article/details/gdrlaorwe.sHtML

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://3g.fanxiaobao.xyz/Article/details/ggkksygzl.sHtML

[Q87] JSON 字段做条件
来源：http://baike.fanxiaobao.xyz/Article/details/gpfvpijzm.sHtML

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://mobile.fanxiaobao.xyz/Article/details/gwggfhxyg.sHtML

[Q88] 行转列（条件聚合）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggyofdwca.sHtML

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://blog.fanxiaobao.xyz/Article/details/gsqytoiag.sHtML

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://3g.fanxiaobao.xyz/Article/details/ggdjwmdui.sHtML

[Q89] 判断表是否存在
来源：http://wap.fanxiaobao.xyz/Article/details/gsvnyyzkk.sHtML

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://blog.fanxiaobao.xyz/Article/details/grkuluwup.sHtML

[Q90] 生成序号列
来源：http://www.share.fanxiaobao.xyz/Article/details/gghtkwzzi.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpzjdrjif.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gzlytwvai.sHtML

R. Bash 专题
来源：http://blog.fanxiaobao.xyz/Article/details/gnfjsslok.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gcivkmutm.sHtML

[R01] shebang 与严格模式
来源：http://read.share.fanxiaobao.xyz/Article/details/gsaarhkhz.sHtML

#!/usr/bin/env bash
来源：http://blog.fanxiaobao.xyz/Article/details/geogmvcjz.sHtML

set -euo pipefail
来源：http://mobile.fanxiaobao.xyz/Article/details/gpchspaza.sHtML

[R02] 变量赋值与使用
来源：http://mobile.fanxiaobao.xyz/Article/details/gehvrvuub.sHtML

name="Tom"; echo "$name"
来源：http://3g.fanxiaobao.xyz/Article/details/goocwabzf.sHtML

[R03] 只读变量
来源：http://blog.fanxiaobao.xyz/Article/details/grxnpfofu.sHtML

readonly PI=3.14
来源：http://mobile.fanxiaobao.xyz/Article/details/gclbagpak.sHtML

[R04] 位置参数
来源：http://3g.fanxiaobao.xyz/Article/details/glndbcxso.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkzfzkolj.sHtML

[R05] 参数默认值
来源：http://wap.fanxiaobao.xyz/Article/details/gsponhvna.sHtML

name="${1:-default}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxbmsmhsg.sHtML

[R06] 判断命令是否存在
来源：http://blog.fanxiaobao.xyz/Article/details/gmfwidurq.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gxgcqmmte.sHtML

[R07] if 判断文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gymvsyapo.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/gxvxpzbkq.sHtML

[R08] 数值比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gdyurvncu.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://read.share.fanxiaobao.xyz/Article/details/gvapswzyv.sHtML

[R09] 字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gxiutirog.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/grfgpfpvu.sHtML

[R10] 正则匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gkjqedmld.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjnpclryb.sHtML

[R11] case 多分支
来源：http://read.share.fanxiaobao.xyz/Article/details/gdjbhyrbl.sHtML

case "$1" in
来源：http://m.share.fanxiaobao.xyz/Article/details/gfbghabab.sHtML

start) echo "启动" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gxxuyeudb.sHtML

stop)  echo "停止" ;;
来源：http://mobile.fanxiaobao.xyz/Article/details/gkbstqokt.sHtML

*)     echo "未知命令" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gtfwjrkve.sHtML

esac
来源：http://baike.fanxiaobao.xyz/Article/details/gpdvgyxlr.sHtML

[R12] for 遍历文件
来源：http://wap.fanxiaobao.xyz/Article/details/gycoocbuh.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmxqvuxdo.sHtML

[R13] for 计数循环
来源：http://blog.fanxiaobao.xyz/Article/details/gocipugsi.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gsfoeffpp.sHtML

[R14] C 风格 for
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxriqmmxq.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gipciovix.sHtML

[R15] while 逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gsuxqecfl.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gtsuyqtcl.sHtML

[R16] until 等待条件
来源：http://3g.fanxiaobao.xyz/Article/details/gjsjutshv.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gbnbfhrcg.sHtML

[R17] 数组定义与取值
来源：http://read.share.fanxiaobao.xyz/Article/details/gdcslsdwy.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gledwjwje.sHtML

[R18] 遍历数组
来源：http://mobile.fanxiaobao.xyz/Article/details/gqfgnnlri.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/glteyuspk.sHtML

[R19] 数组长度
来源：http://blog.fanxiaobao.xyz/Article/details/gsptfvgaq.sHtML

echo "${#arr[@]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gswkfaugy.sHtML

[R20] 关联数组（字典）
来源：http://mobile.fanxiaobao.xyz/Article/details/gldplprwj.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fanxiaobao.xyz/Article/details/grpdlkjnq.sHtML

[R21] 字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gkkhebygb.sHtML

echo "${#s}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gsyrjbmzh.sHtML

[R22] 截取子串
来源：http://baike.fanxiaobao.xyz/Article/details/gfahpxsxb.sHtML

echo "${s:0:5}"
来源：http://3g.fanxiaobao.xyz/Article/details/gmeoruhxg.sHtML

[R23] 字符串替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqbdijkww.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://baike.fanxiaobao.xyz/Article/details/gfsbwklfd.sHtML

[R24] 大小写转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gtoepfjaw.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fanxiaobao.xyz/Article/details/glvkbrshd.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fanxiaobao.xyz/Article/details/gevksmnvy.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://mobile.fanxiaobao.xyz/Article/details/glkoiognn.sHtML

[R26] 命令替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gdbvoresd.sHtML

now=$(date +%F); echo "$now"
来源：http://blog.fanxiaobao.xyz/Article/details/geptutotz.sHtML

[R27] 算术展开
来源：http://www.share.fanxiaobao.xyz/Article/details/gobhfslqy.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fanxiaobao.xyz/Article/details/gearyuebo.sHtML

[R28] 浮点运算
来源：http://read.share.fanxiaobao.xyz/Article/details/gczewijnd.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fanxiaobao.xyz/Article/details/gtdccsnbv.sHtML

[R29] 定义函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gizzmvzxh.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fanxiaobao.xyz/Article/details/gkjwbhrsd.sHtML

[R30] 函数返回状态码
来源：http://mobile.fanxiaobao.xyz/Article/details/gtaxmmnbu.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://3g.fanxiaobao.xyz/Article/details/ganqzyykb.sHtML

[R31] 局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gvgzcvrsb.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gferktmul.sHtML

[R32] 参数个数校验
来源：http://mobile.fanxiaobao.xyz/Article/details/gknifnfpc.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/grsnnmxcn.sHtML

[R33] 捕获错误并提示行号
来源：http://www.share.fanxiaobao.xyz/Article/details/gmmhftzir.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fanxiaobao.xyz/Article/details/gcutiyxkc.sHtML

[R34] 退出时清理
来源：http://read.share.fanxiaobao.xyz/Article/details/glalyrzpl.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxipgfeuq.sHtML

[R35] 后台执行并等待
来源：http://baike.fanxiaobao.xyz/Article/details/gfnyvehvp.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fanxiaobao.xyz/Article/details/ghajjczdv.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gszmdatil.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.fanxiaobao.xyz/Article/details/gbltqzamr.sHtML

[R37] 把输出赋给变量
来源：http://blog.fanxiaobao.xyz/Article/details/gvounwpbl.sHtML

files=$(ls -1)
来源：http://www.share.fanxiaobao.xyz/Article/details/grfrktrxe.sHtML

[R38] 管道串联
来源：http://read.share.fanxiaobao.xyz/Article/details/gcoxiadyw.sHtML

cat a.txt | grep -i error | wc -l
来源：http://baike.fanxiaobao.xyz/Article/details/ghoyapbfa.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fanxiaobao.xyz/Article/details/gskuserij.sHtML

cmd > out.log 2>&1
来源：http://baike.fanxiaobao.xyz/Article/details/gzrkknhju.sHtML

[R40] 追加写日志
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaivmvrna.sHtML

echo "log" >> out.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gmbzkueex.sHtML

[R41] 丢弃输出
来源：http://3g.fanxiaobao.xyz/Article/details/gfpxzwglf.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/getosqcyf.sHtML

[R42] 输入重定向
来源：http://blog.fanxiaobao.xyz/Article/details/gstlvgqxd.sHtML

wc -l < a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/glbcvdilv.sHtML

[R43] 按名字查找文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gwddqkmpc.sHtML

find . -name "*.log" -type f
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdjhhruff.sHtML

[R44] 按修改时间查找
来源：http://blog.fanxiaobao.xyz/Article/details/gwixburee.sHtML

find . -mtime -7 -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/geqxngdzb.sHtML

[R45] 批量删除
来源：http://m.share.fanxiaobao.xyz/Article/details/gcncasxyy.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.fanxiaobao.xyz/Article/details/gftvwhcvc.sHtML

[R46] 递归替换文件内容
来源：http://read.share.fanxiaobao.xyz/Article/details/gzjalkyay.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.share.fanxiaobao.xyz/Article/details/ghjagvpge.sHtML

[R47] sed 单行替换
来源：http://mobile.fanxiaobao.xyz/Article/details/gfejkemmy.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/grdderpql.sHtML

[R48] awk 取指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/gcvtplwmw.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gagyrivmj.sHtML

[R49] awk 带条件
来源：http://wap.fanxiaobao.xyz/Article/details/giuiqmzns.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.fanxiaobao.xyz/Article/details/gtnnkpmxk.sHtML

[R50] awk 求和
来源：http://m.share.fanxiaobao.xyz/Article/details/geqvkmvud.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gikvgbljx.sHtML

[R51] 排序去重取前几
来源：http://m.share.fanxiaobao.xyz/Article/details/gamvnzwfb.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fanxiaobao.xyz/Article/details/gwpchiuxd.sHtML

[R52] 统计行数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gftwqkdsb.sHtML

wc -l a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwoayozbt.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gijiklcdv.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.fanxiaobao.xyz/Article/details/gwroyyrnt.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gquvuvecu.sHtML

diff a.txt b.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmgsfnoim.sHtML

[R55] 压缩与解压
来源：http://mobile.fanxiaobao.xyz/Article/details/ghpiosmyq.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fanxiaobao.xyz/Article/details/gqqejgzlr.sHtML

[R56] 远程拷贝
来源：http://wap.fanxiaobao.xyz/Article/details/gebmoguxu.sHtML

scp file user@host:/path/
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpaysoxyi.sHtML

[R57] 远程执行命令
来源：http://blog.fanxiaobao.xyz/Article/details/gfuutcdhm.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfccnstwh.sHtML

[R58] 下载文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/goilobxbu.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fanxiaobao.xyz/Article/details/gssdzvstm.sHtML

[R59] 发 POST JSON
来源：http://baike.fanxiaobao.xyz/Article/details/gtosclfui.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fanxiaobao.xyz/Article/details/gtfsxzgfn.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gmsdtkwop.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gijejlxcz.sHtML

[R61] 磁盘占用
来源：http://wap.fanxiaobao.xyz/Article/details/gxzvkcowm.sHtML

df -h;  du -sh *
来源：http://m.share.fanxiaobao.xyz/Article/details/gumfkspvk.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fanxiaobao.xyz/Article/details/giduaiefk.sHtML

du -ah . | sort -rh | head -10
来源：http://baike.fanxiaobao.xyz/Article/details/gupuqumib.sHtML

[R63] 内存与进程
来源：http://wap.fanxiaobao.xyz/Article/details/grjumasze.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsrdrehpd.sHtML

[R64] 结束进程
来源：http://3g.fanxiaobao.xyz/Article/details/gafnopdxd.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fanxiaobao.xyz/Article/details/ggtgenvdz.sHtML

[R65] 查看端口占用
来源：http://wap.fanxiaobao.xyz/Article/details/grksudqca.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fanxiaobao.xyz/Article/details/greqoqadv.sHtML

[R66] 定时任务
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdwqdymep.sHtML

crontab -e;  crontab -l
来源：http://wap.fanxiaobao.xyz/Article/details/guirtdvlz.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gypfkaeys.sHtML

openssl rand -hex 16
来源：http://mobile.fanxiaobao.xyz/Article/details/ggefiakth.sHtML

[R68] 计算文件校验值
来源：http://wap.fanxiaobao.xyz/Article/details/ggkcjdukp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gkltzhjfx.sHtML

[R69] 生成随机密码
来源：http://www.share.fanxiaobao.xyz/Article/details/gnfdqhqkt.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fanxiaobao.xyz/Article/details/geqiglucc.sHtML

[R70] 时间戳与互转
来源：http://wap.fanxiaobao.xyz/Article/details/gnnybcpgs.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fanxiaobao.xyz/Article/details/gjjzznzgz.sHtML

[R71] 日期格式化
来源：http://wap.fanxiaobao.xyz/Article/details/gxnblmctq.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fanxiaobao.xyz/Article/details/gokpmpoqc.sHtML

[R72] 等待端口就绪
来源：http://read.share.fanxiaobao.xyz/Article/details/gbicbzddu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fanxiaobao.xyz/Article/details/gictgurnk.sHtML

[R73] 分割大日志
来源：http://m.share.fanxiaobao.xyz/Article/details/gviwowpmf.sHtML

split -l 1000 big.log part_
来源：http://mobile.fanxiaobao.xyz/Article/details/gcufpvwdo.sHtML

[R74] 批量重命名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmwllmfsg.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gfiigrzen.sHtML

[R75] 导出环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/grpjutofr.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fanxiaobao.xyz/Article/details/gjluqvkfu.sHtML

[R76] 使用临时文件
来源：http://m.share.fanxiaobao.xyz/Article/details/ggcraemor.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gcggwvnzk.sHtML

[R77] 读取用户输入
来源：http://read.share.fanxiaobao.xyz/Article/details/gkpqpgore.sHtML

read -rp "请输入: " ans
来源：http://wap.fanxiaobao.xyz/Article/details/gqqnnajzl.sHtML

[R78] 交互式菜单
来源：http://blog.fanxiaobao.xyz/Article/details/gtxcdmpwq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fanxiaobao.xyz/Article/details/gdbdnqfll.sHtML

[R79] 解析命令行选项
来源：http://m.share.fanxiaobao.xyz/Article/details/gspxpzsqj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fanxiaobao.xyz/Article/details/gzyxmdzku.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fanxiaobao.xyz/Article/details/gjukgnhzj.sHtML

time ./run.sh
来源：http://www.share.fanxiaobao.xyz/Article/details/gzvcuydph.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gxpljgiyk.sHtML

S. C / C++ 专题
来源：http://blog.fanxiaobao.xyz/Article/details/grxbbipae.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gprmpqacm.sHtML

[S01] C：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gsmsgfbsk.sHtML

#include <stdio.h>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gefvtmotv.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fanxiaobao.xyz/Article/details/gtknxdeiw.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gecrxnnyc.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fanxiaobao.xyz/Article/details/gtzewculk.sHtML

[S03] C：读入整数
来源：http://wap.fanxiaobao.xyz/Article/details/gxxudkxjg.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fanxiaobao.xyz/Article/details/ggacurkji.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghjzzefdh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fanxiaobao.xyz/Article/details/gobwuzlav.sHtML

[S05] C：字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gkcszducq.sHtML

strlen(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gmtppcsra.sHtML

[S06] C：字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gtvmprcfu.sHtML

strcmp(a, b) == 0
来源：http://m.share.fanxiaobao.xyz/Article/details/gqnvfocwi.sHtML

[S07] C：数组遍历求和
来源：http://3g.fanxiaobao.xyz/Article/details/gdhihguke.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fanxiaobao.xyz/Article/details/gyzcincdn.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fanxiaobao.xyz/Article/details/gztsvwbns.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fanxiaobao.xyz/Article/details/gssylvaft.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.fanxiaobao.xyz/Article/details/gxuukpbkb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fanxiaobao.xyz/Article/details/gnqksvnqp.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gibxadrwh.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/gszcellmy.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzldnllso.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fanxiaobao.xyz/Article/details/gbdxbscon.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gfyccfsaw.sHtML

fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gmgrxjygw.sHtML

[S12] C：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggbvyahkm.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gusezkfbs.sHtML

[S13] C：宏定义
来源：http://read.share.fanxiaobao.xyz/Article/details/gmxiqkvss.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fanxiaobao.xyz/Article/details/gapzcozck.sHtML

[S14] C：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gzvvfiery.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkwntwouk.sHtML

[S15] C：类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/gbfypitka.sHtML

(double) a / b
来源：http://mobile.fanxiaobao.xyz/Article/details/gnyqwqxig.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpmkmjbzf.sHtML

x |= (1 << 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gotkpbuyb.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gleqctgqj.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fanxiaobao.xyz/Article/details/gzoecbkyd.sHtML

[S18] C：命令行参数
来源：http://wap.fanxiaobao.xyz/Article/details/gmitbzhls.sHtML


<!-- 参考信息 -->