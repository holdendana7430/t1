代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3jnfohdwl.html

[Q50] 批量更新
来源：http://www.52xcode.cn/Article/details/gt3xiwcgdts.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3lubcydnj.html

[Q51] 用子查询更新
来源：http://www.ydjk.org.cn/Article/details/gt3cophedib.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3zexxnxyk.html

[Q52] 删除指定行
来源：http://www.52xcode.cn/Article/details/gt3twtkdafp.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3dairytwh.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3uyvejjyu.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.ydjk.org.cn/Article/details/gt3bciuyeuh.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3dxalbrot.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3ijqdkkir.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3wdhaavio.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3ebjdqrln.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3vuuiqkne.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt3bymluthz.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3ykebjpoy.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rgmmzxwr.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3puqrkjjq.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3nxbeomdz.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt3ukknwpqx.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3rwsumkfn.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3haykbxan.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3ryjqrmvz.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3hmkciigg.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3puvrhwie.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3qyugymuh.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt3vyowntql.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.ydjk.org.cn/Article/details/gt3ukxltudo.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3msyetmos.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3mgwvzrla.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3yqlbweej.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3pcwgteca.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3ssqzaelu.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3jnjtqqmv.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3znlprfqu.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3uuythrtj.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3zbxqbeqz.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3byhbkbsu.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3zmmckfiv.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3wvqzjzup.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3spvdjymf.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt3qfumyote.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3jywwdfpu.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3ihbmnhcv.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3kxqtmnox.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3jpazwkiq.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt3uttkoxlk.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt3mvehzgsx.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3xtfvzacf.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3mdtryvzd.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3uflkvjxp.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3sutbluzz.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3mzboutav.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3oysolmtv.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3ykgenftq.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt3rspgsnft.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt3knklnhhy.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3reqtsusx.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3tdkvhffi.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3obspytxn.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt3pplrtgxw.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3unydpfpy.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3zhkbyurt.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3ygvecgax.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3jsbyvixh.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3fpxftovp.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3djpdxzwj.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3ukkfbiow.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3qghzmltn.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qsgafztw.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3mxgnvgdz.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3bdmxagub.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3cynfrtpf.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3yuaukmar.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt3towcncka.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt3tfokyghn.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3qwudzdjr.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3ftzmfkbd.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3tuheeyez.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt3fikceshg.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3wakcowmw.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3efhrfmrc.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3sunszgft.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3isfiklni.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3evqkhcts.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3pudprovf.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3udxuczgq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hnwidjhn.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3xxsmfumu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ykbjwyvk.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3jamucpmh.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3zcmijurp.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3kdzfljsc.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3bydvcaks.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3hewhugxt.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3qeglodda.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3ncyynwfm.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3grnwcmlt.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3pdeypsvr.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3pvxpvyhy.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3ttknincw.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3gfllazyi.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3upbaclys.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3ivkwrlam.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3wezdhrul.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3jcrisihs.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3dbvnkvof.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3vlfvccjb.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3yayfgcfc.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3uxfoajzm.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3ldvnjwgs.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3gcickjny.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3rpvzjrne.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt3ckdaawxn.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3jfslumms.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3hybsmegd.html

esac
来源：http://www.52xcode.cn/Article/details/gt3flvzpcdf.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3aeiqjetm.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3eriuwqsl.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3peopwsko.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3icldqmrb.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3wbvvkdse.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3kcurhypu.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3kjlbzjzx.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qcugjttr.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt3ggkmokrn.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3bxdfkyvi.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3fvaogdzy.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3xrruzveg.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3pzpxjphs.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3wkekvwom.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3mlkdiceo.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3ofzoklyu.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3qxpxnqsy.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3bloxvgam.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3fvjdfoah.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3mvauzxbj.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3dqpjzekl.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3rnpkprgk.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3avurxttx.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3tbtsfiwa.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3bvlnatla.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt3mlxcaarz.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3oqbwmowq.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3uzpcselc.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3ghbhjxdu.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3okmjokpw.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3efkofszv.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3rfsewttm.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt3bocynoej.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3wyfpxjvd.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3dyxxyhyj.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt3oadscrzn.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3wifjxgbp.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3xvsmeioq.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3velgtuwd.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3ddbtktbw.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt3dpdjhzie.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3bugeoqav.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3cagmwevk.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3bkqoluys.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3rsjbtmwe.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3nrzqvaqb.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3kmxqtoue.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3npkemwur.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3wpnrpnyp.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3ehnewbxf.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3mbyxnjwy.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3zroomnbs.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt3vmqdvamb.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3vseobfvs.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3jtkarwgb.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3agwctssn.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt3fzdxhifd.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3onbvosmg.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3iwbebebm.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3lyemgibf.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3zzcwkkxn.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3fwuifzbz.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3drmimoxi.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3ierafwij.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3xyuabgzf.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3unykleaj.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3bihztzow.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3kaueazlr.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3ejvligyh.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3fhmuteyt.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3xeuajoit.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3lekcgylh.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3mxfvwyfv.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3tgcqkjov.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3oeiwoofi.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3tbsvlasz.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3owactgml.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3qekxooxn.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3wvcsszyr.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3cmdnychm.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3igaytget.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gptynxua.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3otceqpzj.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3mrjoojpk.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3deazquxd.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3htjbsxli.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3iqodwokm.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3qfenwymc.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3wkgeyxfx.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3aogjzcyi.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3mgyfqsqu.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3qudlpxwn.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3hqdkuqsz.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3nhukypvl.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3hvulokus.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3kppjszue.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3tftwhmih.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3uoknmwun.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3dpceadsv.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3ncotmmqt.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3jtatdsvz.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3ejzrdtfo.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3hiroiawt.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3jjaaktqz.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3cyujanrf.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3mipcoing.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3sopfcnvi.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3wzlflegx.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3pqpagowy.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3wvmlbcjp.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3qdtzrzuy.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3gpumdkjr.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3mzkmeijs.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3fxvtczkh.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3pkuqzcth.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3wigyuwmy.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3aspjlpkq.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3bpqsewzs.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3pppkvoot.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3hafcxrkt.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3flbdzoyk.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3awmtxsmc.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3bbjsumye.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3fruzgwuu.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3cvpbumhz.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3qgmwvubr.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3monpcooy.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3xbjneyar.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3bkjybpwm.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3xtvaddsv.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3clmyggkt.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3wutapouy.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3xywrgkzx.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3bmuxkvje.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3jfudkiit.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3foyyjqev.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3gwlzxhhq.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3pmkwzqro.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bbsycboq.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3hgympght.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jowyvvlh.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3oxunubvy.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3bgvmdayt.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3bhvyervf.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3apuyhidz.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3mktoaeds.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3pooxwovk.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3nwrycjyo.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3mvtjhxcc.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3iloxvrxw.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3kppqxjbg.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3ybjugbnh.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3lgssclpu.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3trsbshtv.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3ytvcqvfc.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3ydqtxggj.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3prugvbmg.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3evnrekqs.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3abiqkmlp.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3kgfjohhm.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3uzljnejd.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3wgudrtxe.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3nzbzinwe.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3xxtnzxme.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3jdgqvbxu.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3yimdcbym.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3dvbvbwtu.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3sthkjfev.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3owbbkdpi.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3afvdyzwf.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3oxxccaik.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3wkzyieux.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3fkzbzcbp.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3fjyngqkw.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3idupcaga.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3tbyfoyec.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3anmjssee.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3xzlcprfr.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3mqbrhtwx.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3hizpameg.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3swlipzms.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3cbohdghn.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3aaiphmsx.html


<!-- 参考信息 -->