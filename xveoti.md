代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2kjqeatvu.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt2yvjqmosi.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2etijuunn.html

[Q59] 分组内累计
来源：http://www.ydjk.org.cn/Article/details/gt2escwzqla.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2nsfsarrd.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt2wlexpytd.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt2agqydokb.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2najzztcw.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2gbcbvzdm.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2sollrman.html

[Q62] 分组占比
来源：http://www.ydjk.org.cn/Article/details/gt2noiezhdo.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2xtbvkzhm.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt2gevmpgwc.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2wupypkyh.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt2kxasxwif.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2vbrbazhh.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt2vrifrvwd.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2hsbkkczi.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt2ivpkjolh.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2nqgysbcx.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2tswagbgf.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2aejpfzbb.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2fkmsoiig.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2nxvfxsgm.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2bdvhxskr.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2jdxkbnlb.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2ilctaqcn.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2yrzbsmrq.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2ihmeblrc.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2jytlcwcz.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2mayvfbyn.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2asckllwf.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ogfqpdby.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2kyhdests.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2yhggxofy.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2xsgcxmzd.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2wxbcobjm.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2bugatqdf.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2qtcfmewg.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2oclnaqey.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2tjldumgu.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2nsdtvrcc.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2eqjzjnqv.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2lwtxxbhr.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2sdfwrtlo.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2fylmdmdf.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2cnlbwghn.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2niykyrhw.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2guaktnuv.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2fpnyclcx.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2ofwdgkbi.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2trivdyzn.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2xwbqhsnq.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dzfpvfbq.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2oplfenvp.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2drburyrk.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2ntrntuiu.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2hghzasre.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2anxwgrue.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2sqfhdtnn.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2urncbsha.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2tpgmzbzo.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2dmupeouo.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2yzubwcrb.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2guekvfhs.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2ocrasyee.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lcoiuqpb.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2gtgwtgok.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2wrhkehtm.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2lueqeent.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2kgobgtkd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tjqtinjb.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2lffnimnw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2tqtcziib.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2jtfidrcs.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2qflkicyw.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2otggzoxa.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2drvmkcdo.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2ywsvcths.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2ipsqktsz.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2niwqnpnm.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2wutpguss.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2aruekivm.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2hljckyjq.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2jpdzbdxb.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2nlajkkyu.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2ierinfqh.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2wmbdqfyy.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2vrxbuoqq.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2iveahvqj.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2dkzzofuk.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2ktolxvtj.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2qrerfqmu.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2uwqzsjwu.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2tqdyrkkp.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2cyqflchk.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2swwvcnyg.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2izyppddz.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2zhygtiub.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2exnrnzat.html

esac
来源：http://www.52xcode.cn/Article/details/gt2xsgbizwn.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2cvlfufve.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ihdzimzc.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2qsrbzxli.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2yqltyjqp.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2vusqvmxc.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2bqdljdhk.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2gamtzesh.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2eoyxevvj.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2czsljzod.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2luajloge.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2mvlacmxv.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2jgxcnuiz.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2aabftcrz.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2vzbbfzsh.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2lpybapzs.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2tlgmgwxb.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2kbzsvwjt.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2odbkoelc.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2qqqeefzp.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2pekwzcuv.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2marwsfrn.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2qsrqekur.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2skauaeii.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2biabraxn.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2vfhnpkdk.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2uxzvqcfl.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2gzmfrotj.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2mcfonchm.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2jenlnucd.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2bwjgmkhk.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2eohadfkh.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2xnzxasiw.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2lgconuch.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2wjfcmokv.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2hlkfatvi.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2wzeasubm.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2zboaszbw.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2hthfyfrk.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2ojhzjsuc.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2mhrsfjal.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2zjajtzyh.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2wgybruwo.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2byemposf.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2zowlceza.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2cyucxald.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2bfeaalfz.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2tuuqfiql.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2dckkytmi.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2zpyklppi.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2pakrtuyk.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2uloafbwd.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2xulbqjkb.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2slzqukvp.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2cwjbvsbf.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2hueicbcb.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2ybjwvrse.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2xnpslsxu.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2walanhfi.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2jnuioezz.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2zzxjdvoa.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2zdkjgngc.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2lowayrvv.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2nophycdm.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2rctpiyvn.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2nzdgican.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2fnxvmdrb.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2nijuvldz.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2nzeinywv.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2ydoesqlj.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2raxrelwa.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2hovrbojr.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2lmwejfgq.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2ijsbfzob.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2sckvlfed.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2yahgdcbf.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2cgqludiw.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2gxcvagab.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2gaelcvry.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2ajmaeonl.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2htuzatih.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2oihigbqb.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qditngih.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2kllilqxt.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2nfkkvjra.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2jcbuhlwa.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wujuvtnk.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2nzndqwdv.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2pumqqhgw.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2efmmbdmz.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2uxuiipih.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2ovcdlxoq.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2ynlertpr.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2zcurkgkc.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2afgsgznb.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2rqsigoar.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2ocurjfua.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2wnhwqsge.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2geepbuco.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2kipfipze.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2xdhepwtf.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2swijalfl.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2kfobcaxx.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2dsnggipf.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2rupyummi.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2rgqtbucf.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2uclummep.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2giqqpqhg.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2xwwhelsl.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2jnyrbivb.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2ifnbikqu.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2xziongpi.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2lynycesk.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2ztxdhwfb.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2uemeggnk.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2rqqpvmaw.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2rbvgdkvs.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2jnpnhnto.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2yamvisaq.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2ydmmegit.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2absvjpir.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2qrejxjzz.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2soypeawk.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2wdhqfptr.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2bqfvpjrh.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2lwybwwsk.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2qczwezfv.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2egkrmrpi.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2mxwxscqp.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2ychlvzac.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2mibqxwsa.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2emcgwmag.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2oyismvfa.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2mgnwentv.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2ojhxstkn.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2efcsnjdj.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2imxjpelp.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2otvzpqqm.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2yofzmcvo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2cclrnqri.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2acqhtpfk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gxxtmtvy.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2tndntwoi.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2goxnstxw.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2cdblbgar.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2kzvvrhgz.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2fhvmhnpy.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2xkcendkk.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2llqnvnss.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2tndfukac.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2mxomoexw.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2kxijdjrq.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2kweiinmy.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2gemtsqlv.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2bzzbvmym.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2kpklcbhk.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2ibybohna.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2uaojhuco.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2biagyghg.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2xjbjcdwb.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2tmebgbag.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2rcvuhxrt.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2vmfreqjg.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2wxzbliaf.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2mpymequp.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2rpuxezjs.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2ibpignum.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2cervyxgf.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2vurtdzeb.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2qzhaanxp.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2rdqnpqyo.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2bzdadwzp.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2qxvkjuoo.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2vhhdgqgo.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2mgjxinvb.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2tvbvtsag.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2djvphbmw.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fgpdzztd.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2jnmobhoh.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2cmqfgeuw.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2ejwvonio.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2sghkrcau.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2vvlhcvmr.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2rthpenzn.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2tdscwnfd.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2mazsgjha.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2nuyvjhqn.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2xjvzzhcy.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2qocatleg.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2fszczkte.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2koqwdspa.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2vbwdwlvg.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2hbvybdzu.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2hbmcchot.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2ixfebejb.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2ywmosoks.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2vutruuzt.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2zbluogqm.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2qvggaaue.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2tqljrvrx.html


<!-- 参考信息 -->