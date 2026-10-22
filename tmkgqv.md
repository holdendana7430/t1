代发 wailian999

UPDATE users SET status = 1 WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2dcwoyrlq.html

[Q50] 批量更新
来源：http://www.ydjk.org.cn/Article/details/gt2zumwtymk.html

UPDATE users SET status = 2 WHERE created_at < '2024-01-01';
来源：http://www.52xcode.cn/Article/details/gt2savyzejn.html

[Q51] 用子查询更新
来源：http://www.52xcode.cn/Article/details/gt2brwisvww.html

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2mcuquzuh.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt2mswbtulm.html

DELETE FROM users WHERE id = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2srterhhe.html

[Q53] 按条件删除
来源：http://www.52xcode.cn/Article/details/gt2ftsboczs.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt2jgcqdoeu.html

[Q54] 清空表
来源：http://www.ydjk.org.cn/Article/details/gt2eqeiiiem.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt2spmdoolo.html

[Q55] 排名（并列占位）
来源：http://www.52xcode.cn/Article/details/gt2yusxrlzm.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt2jqgeoazu.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt2xznfugav.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.52xcode.cn/Article/details/gt2mjgjkkuo.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt2pebejxbx.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt2cdcdetxj.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2wpsebzwg.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2rtjwpkwc.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2spcybvlz.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2mvotuoth.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2ndsegcbz.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2rkgroznc.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2gpicjdpc.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt2vecgiymz.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2wecztbbt.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2wiacftdk.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2tlkhaiap.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2qmcnshqt.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2sbrcezun.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2svireiky.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2zaawfoqy.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2azbhibhd.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2blkyekqy.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2jsoammvh.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt2ulfescap.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2zppjnogp.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2oyzeqfim.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2feuraxhn.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2fcxagqri.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2usxxnnow.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2jmorbymj.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2ibhgpxvd.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2bvaotlrq.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2wqraulha.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2ylwfdgcr.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2suoltudr.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2mitjtoha.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ibhvuzyo.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2lmjavmox.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2edandssv.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2ylfaeivc.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2eaahqyth.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2fguoyfgc.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2qmxvtmvv.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2egsbjvih.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2kqhkilwy.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2hpmwtiam.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2hvixbblt.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2ssgmlysf.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2kcuwjkgk.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2emnqliui.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2ihaainkx.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2emeagbvl.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2jzfblrqs.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2mxercvca.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2vfkmmjxi.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2jcxbsdhe.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2qbmwncoo.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lvxqsfjn.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2xgshtacd.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lrkzbkbc.html

[Q84] 去除首尾空格
来源：http://www.52xcode.cn/Article/details/gt2uvalmsor.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2oeynuwtm.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2gfpaduci.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2mqzbrzrc.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2dwnefoaa.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2zkvfkgqb.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2wrpybzaa.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2aiuiyaez.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2cycespnw.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2tjsobsmc.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2iebjdjpf.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2wcppprwa.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2fharklbq.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2otsenkpt.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2okhmokax.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2trpkiedk.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2fmhrvzth.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gckndptx.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2yvnmrqmp.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2udbqqydu.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2empzamof.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2kvnauxhf.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2qtgmodan.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2nysvawxj.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2pzlnlbid.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2earorulg.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2oxkbkjsy.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2ijlumswg.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2rmhewclp.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2xlzgtrdz.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2adcsagwr.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2nosnqckc.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2bvvclfsl.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2ewlqsolm.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2vczbqanf.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2jfkvfzmg.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2uzflsshk.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2tvrdhkva.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2qahqssyw.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2okxulfyb.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2xunanvux.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2sfeztfop.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2yiqbcaay.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ywhbfunz.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2jhunnnec.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2gourthaw.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2jvncxrjv.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2yvronfuk.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2popoqqni.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2pcfzrpkp.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2jykvpufy.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2wgcjyrtq.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wewnkqkk.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2joprcwba.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2lhndsykd.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2eziycssq.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2ugrujbja.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2beazkosl.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2zhbokzoe.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2iepnlltx.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2xgnaftoz.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2haadwrss.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2ouhhozcq.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2vehcwgof.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2hjwahywl.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2dbxgejxe.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2xgiiqqxg.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2hwfrqhth.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2dqqnbunc.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2bqptbuir.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2gajkbtov.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2zwjdburw.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2xsagpnhg.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2jiglppkb.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2yqhuiggw.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2oyasnrma.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2mvuxpekb.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2nwgbjmkm.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2hzudlmkz.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2vujgvyxn.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2sfyfmueu.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2gcldijos.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2plycvkrz.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2gnghbofk.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2ituhzfyd.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2wbtjldvp.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2ynnaaltz.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2jgmteenk.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2estcjgip.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2scorbqox.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2wyrcszpi.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2utffrarc.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2gddwtyzg.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2iilumegg.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2ysuuiyfg.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2mhcyqoji.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2ewzysibp.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2qgbgqzdd.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2wiqxjqvz.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2mxwoqppy.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2mlefvrjz.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2xbeswtza.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2xlhjyfdc.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2wwlcgaww.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2gydvqlff.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2oxbzqnxn.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2qyvgtwbe.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2mfrhfcyf.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2judfydbs.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2nzetstbp.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2fyfnryyy.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2rjuygbtb.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2qgtkacys.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2xwsiepqw.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2odvdlola.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2bzovmylp.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2nltduazg.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2tjmyubbb.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qgegomnn.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2ejnhvfoi.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2axexanek.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2widdeexz.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2qleprtzg.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2oncaliea.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2ushpwrzy.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2mlfozgyo.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gkeufovj.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2iqtpvjlb.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2ryqichfj.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2xosavnti.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zwfhfqzg.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2dejolmwp.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2ipovdicz.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2wmzlxpmh.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2ekfbpuyc.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2umullpzn.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2iiltarqk.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2mlkickkl.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2jvfwuejf.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2fwkfthnz.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2qpmcviwm.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2ljihecxt.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2gteuvfvs.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2oxdjxvdn.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2fpwtscsv.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2mhpvrukt.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2edxhviqr.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2bxqlywhy.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2jxwhwpiw.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2bngbcvrs.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2ogwqtavl.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2wuxrzgqo.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2bhnhgokc.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2caoorkon.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2ubkaxbbe.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2gxslcitj.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2yrczlztt.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2dnuslzql.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mwyxuvfm.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2yktnryig.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2hgrfdhnp.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2smmcuvig.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2rezcelhz.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2omfydwiz.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2fgdafwyc.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2cjtfqvun.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2rabutppr.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2frtunhkw.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2fyevduls.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2qrktkvyr.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2bgzzxxtr.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2ukggtndt.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2zgltovtt.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2crcnjzzi.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2ymcxrfal.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2hpewgkjt.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2loudhizu.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2wfnwdgyk.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2kqdfvsnf.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2wjinhyot.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2ijqmfcrc.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2fhtxajgg.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2ancnsqhr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ncfxnmqn.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2ncplkoly.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ifgvzsyu.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ccvirgeh.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2igqhmofa.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2kxpukddb.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2ciyaxfiw.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2dwzgmcim.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2jbwfvenu.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2wuzwlmic.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2mdqiyjwq.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2kbupbzow.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2mghueykw.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2cmbhpthw.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2fivkndqt.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2sgpjswki.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2ppyyyqni.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2vgumhylf.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2bocrcize.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2qbdnrref.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2wuuxjtaw.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2qibnhdof.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2qfxmbckb.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2bneungpb.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2aurkyxcs.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2ephkplxx.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2yjldrzbc.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2gauvimfj.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2dbwflyyl.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2rxbvsmbf.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2vsdmgqdp.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2smxdbpik.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2pyhmzqjs.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2pzrivcyr.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2uhtnxwoc.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2svtpwtee.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2fsawfoqy.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2kmlsmdgo.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2dknrgmat.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2sbrmttln.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2ljtzhhey.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2dbyahzex.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2ihpbakph.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2bnznsfeg.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2ucynzgkw.html


<!-- 参考信息 -->