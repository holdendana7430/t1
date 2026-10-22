代发 wailian999

[Q61] 移动平均
来源：http://www.ydjk.org.cn/Article/details/gt2bgrdbkza.html

SELECT id, AVG(amount) OVER (ORDER BY id ROWS BETWEEN 2 PRECEDING AND CURRENT ROW) FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2linsrtpn.html

[Q62] 分组占比
来源：http://www.52xcode.cn/Article/details/gt2dxwcfteq.html

SELECT city, COUNT(*) * 100.0 / SUM(COUNT(*)) OVER () AS pct FROM users GROUP BY city;
来源：http://www.52xcode.cn/Article/details/gt2ondjaskz.html

[Q63] 开启事务
来源：http://www.ydjk.org.cn/Article/details/gt2ltcxhbpb.html

START TRANSACTION;                -- 或 BEGIN
来源：http://www.52xcode.cn/Article/details/gt2quqzhnci.html

[Q64] 提交事务
来源：http://www.52xcode.cn/Article/details/gt2aqmysrta.html

COMMIT;
来源：http://www.ydjk.org.cn/Article/details/gt2rlbibhzq.html

[Q65] 回滚事务
来源：http://www.52xcode.cn/Article/details/gt2llheamtt.html

ROLLBACK;
来源：http://www.52xcode.cn/Article/details/gt2vfkxpwed.html

[Q66] 行锁查询
来源：http://www.ydjk.org.cn/Article/details/gt2mefaykvi.html

SELECT * FROM users WHERE id = 1 FOR UPDATE;
来源：http://www.52xcode.cn/Article/details/gt2czdgnvsq.html

[Q67] 设置隔离级别
来源：http://www.ydjk.org.cn/Article/details/gt2jvsyorub.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.52xcode.cn/Article/details/gt2fngcpxza.html

[Q68] 保存点
来源：http://www.ydjk.org.cn/Article/details/gt2gaxwwnds.html

SAVEPOINT sp1;
来源：http://www.52xcode.cn/Article/details/gt2ertwrnac.html

ROLLBACK TO sp1;
来源：http://www.52xcode.cn/Article/details/gt2sxzrfjec.html

[Q69] 查看执行计划
来源：http://www.52xcode.cn/Article/details/gt2qvaxaxbu.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.52xcode.cn/Article/details/gt2elrdvwgs.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2mjdmcbkx.html

ANALYZE TABLE users;
来源：http://www.ydjk.org.cn/Article/details/gt2baqeoonm.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2qgwegymp.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.52xcode.cn/Article/details/gt2qavtjquh.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2istgsobl.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2gorclbii.html

[Q73] 查看表状态
来源：http://www.ydjk.org.cn/Article/details/gt2txrlfaph.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2mnrfnxzt.html

[Q74] 强制使用索引
来源：http://www.ydjk.org.cn/Article/details/gt2kvjgpkya.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2wavjfbbs.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2xesjhreb.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ndghungm.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2isfyrymj.html

[Q76] 按天统计
来源：http://www.ydjk.org.cn/Article/details/gt2hykrxamu.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2odemdflg.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2vvuxcezw.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2ojusalab.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2izrnnjdo.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2cdmgkwrg.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2ogoipnjb.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2puviwzck.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2dxzcbpql.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2pkaodzwf.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2sdgezzrg.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2tuibwypq.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2lwmytsob.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2foocbjrg.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2kvfurnuq.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2bcvicgrz.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2ruknlura.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ogqpvaba.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2tnfsmfri.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2sweixzta.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2cshkbuwg.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2epyunstw.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2ugtmhxnt.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2vvisfzxe.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2gelzzbol.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2mxhallup.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2byzktapq.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2jggtljgp.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2lylchqya.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2ndfnxzne.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2ighvclpw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2kgsjlvul.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2qjdblhrj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2aqdsjakt.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2aynquuui.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2awozsjkq.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2vzhpmyhg.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2ldnmmwmh.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2zhqczvky.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2sgdauvwa.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2iyirkkxa.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2braacjhj.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2ddxjweoz.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2xwnacvli.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2ayytoreg.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2kbpkosfz.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2kpaozemv.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2eoptblqb.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2qojjwyfl.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2vswjouks.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2adyjatum.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2gfptaqpu.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2dpcrptdm.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2beozuvqf.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2suhmsrip.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2megifydf.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2zremeequ.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2brtqcyzl.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2fblgttks.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2nzorsliz.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2ujijyskt.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2dpbjjnun.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2evsrehoc.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2mboouijx.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2rhmgqdzc.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2ccodikhv.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2vhcszymk.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2lgnqawol.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ngetxojl.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2nknsgtsr.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2wmmdyyqt.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2ugvtvwqq.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2evhgvcvh.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2rtcgkatf.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2dggusmwr.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2ouextpze.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2ljyqcdib.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2pxktdfhs.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2hjunniro.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2fnjhfbdx.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2iohbupph.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2jtmklgzf.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2nklsnsyx.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2unghquta.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2ubczbuuq.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2gkgpfnim.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2kbqqhlmq.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2oathsszl.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2moicxuwf.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2sarlsqov.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2foneylzl.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2nomphhls.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2jltgfgbc.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2qjknznti.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2pvkmhnbt.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2tshggpzp.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2ytnjcxdn.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2rvfosjbl.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2rotvwztg.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2mjlvyaay.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pmmvnajn.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2tldzuuxd.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2coogefye.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2emifemnh.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2xjnjbpse.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2fnqpapxf.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2eubxxhtn.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2hbqgpour.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2tjhgybvt.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2hroeajng.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2xihpbzkl.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2vbdtacsv.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2yqydymrg.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2juxwxvpp.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2ufqayszi.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2fngqdlms.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2pqmegpmx.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2ltwkgstd.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2praekmot.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2sjxoujgd.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2rlocjogs.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2kyzrblxo.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2ygsnpteq.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2vmxdgwgx.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2nrsloaqo.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2qluroxqm.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2siyxwwbx.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2xqywdboh.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2iddtvlpe.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2cqcoegkr.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2cihsvfci.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2jaftocyv.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ypbnqjvq.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2cycqcctq.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2deiifkat.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2nxoyivvd.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2zyjxedau.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2swdgssgs.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2foypscui.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2gbnbiemr.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2smvacxwy.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2wuswzdrz.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2tsfaytja.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2rszdbqxy.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2hbsmesgg.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2vcgwiyby.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2ppzuafeq.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2bfkjzghw.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2sqqydszj.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2uyagmxdi.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2oqryaljo.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2qvejlnwd.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2dsxvziow.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2adcbffhf.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2hjltgxpi.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2zqwsvadd.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2wiiwidss.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2vhdokkqv.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2cnvnrrpv.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2vobsrfet.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2faajwavw.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2wkrzccmu.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2pgzektll.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2ptyvnkut.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2habdrkop.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2kgyitapd.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2ukopwylu.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2mbjrdcus.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2ejbdftjy.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2ysojfifh.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2vmeewxxr.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2hmphmxls.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2stchbjfw.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2cpkmmocn.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2flqaljff.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2dbszdamw.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2cfvnouyd.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2fzvdrzwh.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2kemuufgi.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2znnavlxn.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2uignvfky.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2zxobhxgp.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2bjevvfwp.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2esvijnwc.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2cbdschar.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2zacybchj.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2zdenewlt.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2mlepmted.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2cjnlcokc.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2gcrxwbkt.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2etujkkmc.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2ktrbmoms.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2pdrzyhxr.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2xuyaodyn.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2wtvhytng.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2dirodtlw.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2sqodyksr.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2xqpxtpnm.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2rgwrmvws.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nkpudnld.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2qudwrghe.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2spzsqshb.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ueafufhb.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2jdnnapwv.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2ublvztsb.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2ckrgfyrt.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2jctiyjhe.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2wjltnbdj.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2iuihcqti.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2hntbvolw.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2adcbokjy.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2khemslip.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2pjzoktvp.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2oqnrzfxz.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2vthmhzsh.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2iquqfgqj.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2lxbrjpxn.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2iyetzqem.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2gzgcwtgj.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2zsfucgzb.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2jsaxcoid.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2ypblvrnm.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2ojvsuisd.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2yhnxrmia.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2gngfzqmj.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2oslgyvyw.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2yrudoika.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2rgrejjgq.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2hngectfl.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2vumtdtea.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2hbfhfcbn.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2oarfuaus.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2jtqxtcvg.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2xggoalha.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2mourqrwc.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2jtaoyajd.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2bnyrndpk.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ijwgjulq.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2cyixfmbl.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2lvxdnmuc.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2ehunqjuc.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2rjwnzemn.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2nmobrlju.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2uqrzmtsu.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2lerjgzkt.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2tmgyjtgq.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2azbkilnm.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2clwhqazt.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2chfozsat.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2iqiletsv.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2afnttqhz.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2yabsdoul.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2azgdztut.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2dbzdowwt.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2ztjsxykz.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2zumkhisg.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2ggxgswmv.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2slzvznvn.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2vbuumecy.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2dgkbyvyv.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2kymjzvfj.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2zmxdwzdo.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2dugldrpy.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2mdxaivcc.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2iaxdjcxr.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2galzjprd.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2ceemzujc.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2vfyetini.html


<!-- 参考信息 -->