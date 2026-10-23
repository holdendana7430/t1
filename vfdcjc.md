代发 wailian999

SELECT ROW_NUMBER() OVER (ORDER BY id) AS seq FROM users;
来源：http://www.52xcode.cn/Article/details/gt3gkdpkitn.html

[Q58] 累计求和
来源：http://www.52xcode.cn/Article/details/gt3pctxtlgm.html

SELECT id, amount, SUM(amount) OVER (ORDER BY id) AS running FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3jjmdwncq.html

[Q59] 分组内累计
来源：http://www.52xcode.cn/Article/details/gt3acgqccrz.html

SELECT city, id, SUM(amount) OVER (PARTITION BY city ORDER BY id) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3qrgwsqmk.html

[Q60] 取上一行 / 下一行
来源：http://www.ydjk.org.cn/Article/details/gt3xdibssex.html

SELECT id, LAG(amount) OVER (ORDER BY id) AS prev,
来源：http://www.ydjk.org.cn/Article/details/gt3rsoanvqq.html

LEAD(amount) OVER (ORDER BY id) AS next FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3vvywjskx.html

[Q61] 移动平均
来源：http://www.52xcode.cn/Article/details/gt3qvjmtrtw.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt3dfneqguj.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt3gcehyvxj.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt3wxldwidm.html

[Q63] 开启事务
来源：http://www.52xcode.cn/Article/details/gt3gjtxdahc.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt3lovwcucc.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt3kwpiepgv.html

COMMIT;
来源：http://www.52xcode.cn/Article/details/gt3wjrlregr.html

[Q65] 回滚事务
来源：http://www.ydjk.org.cn/Article/details/gt3xkcxogth.html

ROLLBACK;
来源：http://www.ydjk.org.cn/Article/details/gt3htfffbyr.html

[Q66] 行锁查询
来源：http://www.52xcode.cn/Article/details/gt3lnceovib.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.ydjk.org.cn/Article/details/gt3sxdvjmzv.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt3eombzitp.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt3wmczkzyh.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt3cqyduvbr.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt3arnvsull.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt3ihtqflys.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt3ztywuwwd.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt3xifttjsp.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt3oivgcqco.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt3onunacxb.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt3sjyrxirg.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt3vpbzbubk.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt3negttygp.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3fyhmieng.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt3qabfiuhs.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt3xhsfbqoe.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt3iharjkac.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt3bpslnlij.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3uyqyuujp.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt3urizrznb.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt3srercmuu.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt3euzzkfiz.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt3dytjttzv.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt3vdedxrqn.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt3lzebbcsu.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt3vkpjvdmq.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt3qjrawvrr.html

[Q79] 字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3yvxiwqep.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt3ymdnqlvb.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt3dryntwsw.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3eavoncae.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3xwnqvcnb.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt3unucmlhl.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3irwtencp.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vwzkbwxv.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3pxvnvdsh.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3mpkrwyiz.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3ddjxxgib.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3vubenorf.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3vijnbdpn.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3vqbvkeue.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt3kzwygctp.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt3pgwvktza.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt3ptfcpipy.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3isgkijlv.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt3vyazhtbr.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt3wdoklorb.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3rbggkxnr.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt3hlcwcupq.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3lrqwgczu.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3ouswkydm.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3ibilkkta.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jlntaaew.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt3tlkzukhj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3eqrnupzp.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3csmhcoht.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt3ntluchzk.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt3goixvskz.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt3rttabuyn.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt3uneusjeo.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt3xqkfeqwt.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt3fwnhbjua.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt3nwdpsyyt.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt3npvorhys.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt3xudvelaz.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3fzyhhumi.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3uvpttnss.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3klahpeil.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt3whmotdmj.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3lsembfvm.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt3vbnjveyi.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt3xajlvvbx.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt3sudtxvli.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3xuqzytlf.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3qciyirba.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt3arsxmaqh.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt3tlhsicvd.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt3nbhekxsf.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3dgyfpjao.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3qviwwmwm.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3fxvbqbjk.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt3xcgpefvg.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt3tcedvhxm.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt3qfsqsdqf.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3ppunysfz.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3meacfdop.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt3krkgvzgg.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3gheqqozm.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3eshfbmzf.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3jppczyxc.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3wlkoqohq.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3lmyzukms.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt3utevwmhe.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3fesztsko.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3oxrppjwq.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt3bbxnalmn.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3zwtftyzh.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt3mbwqegpc.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3jcrtkvpq.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt3qwpzkjig.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt3eeazxgcc.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt3wgnhciqf.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3rfgrdhyn.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt3rdrkqkgk.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt3kkgqftpk.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3rdlhfppz.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3foriobwl.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3cxwpiagy.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3dgxeqthq.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt3qwvdgnch.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt3rkydgnzk.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt3mqotnnvx.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt3ynkyokwi.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3pqjypybt.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3gbrgsfwo.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt3hqmceura.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3whjpyjnz.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3jiylaoza.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3qmmbidqi.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt3cniyqveb.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt3bkloxsph.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3xwaqsero.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3gkhpmmpo.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3tgjwwymd.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt3mxeznfpm.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3jjnpvzrf.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt3oenllyal.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3jbbfvydz.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt3cpyvgzcm.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt3xlpubaef.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt3yobctigw.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3viteqxuz.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3chyjihsq.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3hejjgrok.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3zhdbycyo.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3qdidvbsw.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt3qsidmvfv.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3gfbeoxzt.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3guaxpzmw.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3wojrwuhw.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3zpcoieux.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt3penmkiij.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt3gcpmqszn.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3cqqgcrsz.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3ahoazxqm.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt3mbhplkji.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3cmxogswa.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt3hafqimlw.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt3pcrpftix.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3bzvgixpr.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt3fcvwrymw.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt3afampuei.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3slsnudar.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3sccnmwtn.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt3quwjahve.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3saqkirpv.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3lckhwrsb.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt3wroogluz.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt3jsdzyyzx.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3egkzrige.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt3lckehkkz.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3gyzjcyke.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3fygnacot.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3djeezdnw.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3tehbetfm.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3jeptldsq.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3bszvgkcc.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3wemaxwhr.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3voytechi.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3zrimuhiu.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3wsdpxppg.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3pfldjhsr.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3rebpxfcz.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3qqpbfplu.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3dxtponjo.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3xvpzdiha.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3sesppwdr.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3tgfxkgnh.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3zvuxvili.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3xesnhqgs.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3nmkkmrww.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3eyhpkqgd.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3qysnrwhh.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3qazsnobu.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3ccxarbwr.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3yderhlqz.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3spxgoszr.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3qcjvbxgp.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3hynprdpd.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3cwgkttze.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3jejakmfm.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3pflrkbps.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3wckctikj.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3yhvnhxnj.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3hpopriil.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3fteirdau.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3dgzqtijg.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3gxxejvyh.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3mrqupqxw.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3xfyntzay.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3rlsdednr.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3lpsypxkn.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3bpdfdias.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3yusfnrzs.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3vrblyqbt.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3sfftzbgi.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3ybpvuhqj.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3fnxdqeoz.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ygdiyeyx.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3axdgjvqv.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3xboxnxcs.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3xvohbjjt.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3zvuvecgb.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3oswnjhus.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3vpbwdznh.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3znxpwsjk.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3nkohkcew.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3qwyfurxy.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3xqodlgim.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3fhpwhzeo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3msrhfxjf.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3krsyqcal.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3emggycnt.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3kezugmsw.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3oyfrrktb.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3rgdnxqlw.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3hgdqkafb.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3thecxaka.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3srelabma.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3favwsotq.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3qokclshv.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3plolhnxi.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3mtbcvfux.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3sulijcbw.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3wxworvpr.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3piilmyfd.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3pohugsqk.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3stqnggbr.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3nztisbft.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3cjdwibcg.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3lnclivpj.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3vszvhgya.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3rnclnrib.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3ewjsrgfn.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3clttkgdd.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3phkmhfkb.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3dsswegmd.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3rafnxefw.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3hlnwcqds.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3mtdfimnl.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3gzdltmsv.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3ahmybqyr.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3lefuijbm.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3ewdmtavk.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3xdznnada.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3cvtehjna.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3bbhcyucg.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3frfpmbgm.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3xcrfkwal.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3efwntgny.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3uekmhdaj.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3geevqohx.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3vvfybfnm.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3utakvyry.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3ovhhsysh.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3fwrynjga.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3dckcfpax.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3arvhorke.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3mrbxljky.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3qeopycko.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3psemkcyd.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3igsqoifd.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3myvdmfha.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3vbgasgif.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3ipkevfru.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3tnjklkrm.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3coszliqn.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3taaugsry.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3suejbltl.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3azopnfmh.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3fsljtmmm.html


<!-- 参考信息 -->