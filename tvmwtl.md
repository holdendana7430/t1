代发 wailian999

UPDATE users SET age = (SELECT MAX(age) FROM users) WHERE id = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3hgpapoid.html

[Q52] 删除指定行
来源：http://www.ydjk.org.cn/Article/details/gt3dosutony.html

DELETE FROM users WHERE id = 10;
来源：http://www.52xcode.cn/Article/details/gt3jckylzvz.html

[Q53] 按条件删除
来源：http://www.ydjk.org.cn/Article/details/gt3djmqpbpl.html

DELETE FROM orders WHERE created_at < '2020-01-01';
来源：http://www.52xcode.cn/Article/details/gt3etjprldk.html

[Q54] 清空表
来源：http://www.52xcode.cn/Article/details/gt3kdwycgas.html

TRUNCATE TABLE logs;
来源：http://www.52xcode.cn/Article/details/gt3pswtdjii.html

[Q55] 排名（并列占位）
来源：http://www.ydjk.org.cn/Article/details/gt3vomsypgo.html

SELECT name, RANK() OVER (ORDER BY score DESC) AS rk FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3ayigavgr.html

[Q56] 密集排名（并列不占位）
来源：http://www.52xcode.cn/Article/details/gt3qgkpvkae.html

SELECT name, DENSE_RANK() OVER (ORDER BY score DESC) FROM scores;
来源：http://www.ydjk.org.cn/Article/details/gt3tmiystbu.html

[Q57] 行号
来源：http://www.52xcode.cn/Article/details/gt3ghadeyrt.html

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kedgtyaq.html

[Q58] 累计求和
来源：http://www.ydjk.org.cn/Article/details/gt3zvmyftwf.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ckmjuujf.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3yvyfytif.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3cuhofcrp.html

[Q60] 取上一行 / 下一行
来源：http://www.52xcode.cn/Article/details/gt3sqgukdfy.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3nphtqqvu.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3idiejwqa.html

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt3tuaqfvzf.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3ubimtgmx.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3ltvrqaln.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3qlcilito.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt3jtvpfbke.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.ydjk.org.cn/Article/details/gt3xqqeuloe.html

[Q64] 提交事务
来源：http://www.ydjk.org.cn/Article/details/gt3ejnfymgd.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt3irslntjl.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt3kdahgvxt.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt3cdavhnzs.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt3rsnkqtxx.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3zfigdnfj.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3sqvphpyi.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3gqjzgxpx.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3xbrpyxiq.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3oohmjcoc.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt3zckpeqvk.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3golevbmj.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3utqsupsz.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt3agcudllq.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt3ihozikss.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt3jzombtbg.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3rpxxeddf.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3ykimosuu.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt3umqlrkta.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt3aakmosjg.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3uchtfdlk.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt3mrhzclho.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3mmvqxnjh.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3mkzlvmcu.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3sktwffaz.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3fllriciu.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3lsabldeb.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt3uxzhwwth.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3tbpcunsd.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt3ewuwqeka.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3euyldjfy.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt3zvgwtzjw.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3zwgqjxay.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt3dcttmnke.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3bqukibwu.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3hyytsokd.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3ofmdnsdg.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3cmeagfcb.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3jgmzsers.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3luenhdxn.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3ypogtwiy.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3qvicudwo.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3ejnsepxf.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mqwdwhod.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3pwcawbwj.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3marsvhyo.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3yzcpbake.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3rmjzwqtm.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3muiglukv.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3asofdswd.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3vbslryat.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3obclkcew.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3hzhldsaz.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3vdtvtdbn.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt3csgjzblv.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt3povkmgyg.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt3rvosmhqc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3gpvxunoj.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3vboohect.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3cqinbodj.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3cloqubal.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3byejarkx.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3hbibudpi.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3mnctvvwm.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3tvpyqzrk.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3opugrtaa.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3mbaphuma.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3tqihleio.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3tjozgolo.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3ysmhnzve.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3jegchfvr.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3lckaddpi.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3jqbzlsaw.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3zqdbwqos.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3mbfayxph.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3enjxsmkc.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3wyarlmqb.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3xgajymrl.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3lyqycdqw.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3bjgzucrt.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3bclluord.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3zoisupiv.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3ajiqgjko.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3hhhmlaed.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3fsgvkihc.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt3vmaxvnln.html

esac
来源：http://www.52xcode.cn/Article/details/gt3mqibrkgm.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3ngomeapk.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3doyomxdp.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3noinwqei.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3jkyhqgsc.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3reptrycx.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3xapgbhly.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3hhtpvlbb.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3qlbicury.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3bhyliveq.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3hrspyjcp.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3xytdajhy.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt3rjfydsfd.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt3gxzdzytd.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3fixgmcye.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt3dcfwwptr.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3uoaykoir.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt3lptftvrc.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3mpniexya.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3dtifzzrm.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3cmpanrov.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt3albkabgn.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3vjxyrxvv.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3lwxlhmed.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt3wdamgclb.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3ychkhymu.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3xnlfuxfa.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt3cjdftxsz.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3zrfieael.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3zijlbokd.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3jrpeuoln.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3gszxlubq.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt3jfhehjyg.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3prurrown.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3hxxjzgnm.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt3uvpbovsj.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3vlzuhdxy.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt3womecdiz.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3fanuppfy.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3pfdyaiwz.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3genevnfd.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3yupoxifc.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3dmiseorq.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3jitjzuah.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt3ildmydhx.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3tcjnzhkf.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3nobigmon.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3lgvfequu.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3gfcvtepj.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3pgbohcit.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt3wirxygic.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt3pxmlsymk.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3rllbjxhx.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3akjjqkzo.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt3pyfvfjrx.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3ccckxmjw.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3ufjhqdfx.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3zaheunin.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt3tzifedwc.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3zwpuhnle.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3tsepmzhw.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3amccmwfp.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt3ruojasbb.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt3qufdbsux.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3ubfjlroo.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt3ntqcmtzr.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3dzevtgwy.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3stupzung.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt3ruzwalhr.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3ljtuzwno.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3pmzsjqpl.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt3ddugvpvj.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3kuuukdos.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3yliaezns.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3jgxmimhs.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt3waervigh.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3undrwuve.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3eqcgfths.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3whamfake.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3qoespljv.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3aawbgdmw.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3stsxjdmg.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3qfivvqly.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3ncfgypsr.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3ztlpvezu.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3txqtdxzk.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3gksqvuct.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3gllgvdkl.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3ibonskxv.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3ibyymrhu.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3dsnnmuay.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3ngguxqls.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3hbptocof.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3haylkiay.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3fryysgtj.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3lhtdlxsc.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3kienrnpz.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3bdomwpgf.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3dafmskkw.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3jzadaoej.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3vljckjdj.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3pxacvqfz.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3fsvbljyb.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3jboblwrw.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3sbvlwbng.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3clxmbyce.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3viknpjlb.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3mwawalkd.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3hsgrgybo.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3oluesvpd.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3bvrabxya.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3jppgeevw.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3wmjexsye.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3avfdrwnq.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qqimvpud.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3vjcjarmr.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3wofzkghr.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3uzgmvhxj.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3xxvjhwsh.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3hovkjgud.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3uhfydksg.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3feemdmvm.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3wnlteirr.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3ihtubkuw.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3otgimfmt.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3kmngwswp.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3gpnuzfqv.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3gisvmspt.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3yrcermtn.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3pzfpscyc.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3ihemouke.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3dzxemmij.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3uxncrpry.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3zmwkxnnu.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3lcwsgizg.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3ggbhqyvp.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3fvaxcmne.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3xmhpjipw.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3fmtntnlm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tlizdiyn.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3jfhryfga.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qagkoume.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3iqvbiqer.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3hrolkuxf.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3ojyfppuc.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3ygwcjtzg.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3jcasrvcd.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3zhdptwhy.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3fqturmqw.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3apzmwzfo.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3airslqvv.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3rfpvjjjw.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xydojluy.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3ydrasycw.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3ivhyishh.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3bktjwpby.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3sfwdzasb.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3bvtjjvtk.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3rgpymvqd.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3xiadutkk.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3lvkgjlbs.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3tknfepir.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3mkngasaq.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3mukfehaa.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3hunrxyeg.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3iqruzaca.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3tcqekhfq.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3jggkmbir.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3kmfbtmmk.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3zypovtxy.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3urayuzbo.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3xgeiphrq.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3nnubxcdc.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3fdxykeup.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3btlarpij.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3dnjhcyeh.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3jiliprjj.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3yhbombiw.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3swpslmgq.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3cmrcfvbc.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3nxehatbf.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3vztzmudv.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ibbrewwt.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3oggbrofw.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3klrjilxb.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3nowvintu.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3gakptgzk.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3anzcujmd.html


<!-- 参考信息 -->