代发 wailian999

[Q67] 设置隔离级别
来源：http://www.52xcode.cn/Article/details/gt2xzbdcsvm.html

SET TRANSACTION ISOLATION LEVEL READ COMMITTED;
来源：http://www.ydjk.org.cn/Article/details/gt2xmptztlk.html

[Q68] 保存点
来源：http://www.52xcode.cn/Article/details/gt2icaeeqal.html

SAVEPOINT sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2xocehcdm.html

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2qmzoxhhy.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2czyangwh.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2rxrhdbrj.html

[Q70] 更新统计信息
来源：http://www.ydjk.org.cn/Article/details/gt2ogfainjs.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2jjpkvkhj.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2jktgqbpy.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2wfmysved.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2xkkrtisi.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2lopgxwbn.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2ncmfeorm.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2hsreyjzo.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2poinzulp.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2nvhmaltc.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2nbtxvzep.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2ajqbjdgt.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2jxpgyyiw.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2wvjjazzc.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2lcatdeap.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2sydqgbic.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2ekgaosff.html

[Q78] 当前时间
来源：http://www.ydjk.org.cn/Article/details/gt2iykfrmuw.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.52xcode.cn/Article/details/gt2bpakiiqz.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2cmydwnsz.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2uxyppnkq.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2efctmtia.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2upaqyynl.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2lkaydkup.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qadizgua.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2qmmviolx.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2qtfwcqgw.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2xgyhlnlp.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ggvudaqz.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2byzkiuew.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2dlamxusk.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2qbscnydx.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.52xcode.cn/Article/details/gt2qsicyitt.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2otadaupz.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2ypprxmeb.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2hufdvawx.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2miufehbr.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2iszejqhy.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2mctsxcjw.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2kxjvlaca.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2bifdgsrk.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2xegpobqz.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2auzoizge.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2uzqqccyz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2mohzfobg.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2fujryzxo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dfnfuscv.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2yacqyplt.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2clrxfvrw.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2vkbebjoj.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2bhadfkdr.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2astbusga.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2tfqtting.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2dnuawdki.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2jmrsgggg.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2lsqrbwnn.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2ekkxprkn.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2fntrbvun.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2lgeztkyi.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2fexjloyh.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2nudunnlx.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2pkfqhhjl.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2ksqlnwgh.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2wagixapr.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2amhtdiqi.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2zvbtglhk.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2iruzkgma.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2bwmlvhlo.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2rtddjfku.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2owgamvby.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2cqeqrsbc.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2zkzrrvqd.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2mqfoccbv.html

esac
来源：http://www.52xcode.cn/Article/details/gt2dyfwpaup.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2onasuoos.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2zjlgddhj.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2dyxskpui.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2mxbylskr.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2rkaffuyp.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2qysacmjm.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ucjlcwgj.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2lpchcahx.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2jiaocplv.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2odhllltd.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2vmvbjaqj.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2azdmuura.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2xcndguky.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2wsqgsvnd.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2eqbiuucj.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2zuciimvv.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2pkpplshd.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2bfofsjnl.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2hzvsvmfe.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2jtoopjit.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2golxocch.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2cgenqtct.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2erfnwaix.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2gcpemhfi.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2pmijgdsr.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2ajyyhxlx.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2xwvdxnxj.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2nniwvthf.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2hlxkdhhv.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2pmqyrjpl.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2smigcxbp.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2pxmioazb.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2ueuxgnvr.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2nhyfwpsx.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2sqablmge.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2hyqkgwrj.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2vqavlffw.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2feszamms.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2vlquhvms.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2sbxwzdzv.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2wmhmying.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2lsitijzi.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2qhhydzpr.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2ttzxcvln.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2qoockmck.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2urbojhfa.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2gfjmmvqw.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2dfbcqzim.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2hrxiypzo.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2sqqtqsso.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2elhaoewy.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2xolowtmq.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2lhwqsovo.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2bkqejszv.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2lvgavyzs.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2emejqlzd.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2qcatmtdy.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2sjacvchq.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2ircznaed.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2fntuetrx.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2iinctfyc.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mzxywwpx.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2ngbxtrpl.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2gaygslcq.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2cquhsmrn.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2izbglzej.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2yqudqvnu.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2noodawul.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2dfqcdnbl.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2kfbxibwl.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2qzwgyyax.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2lizbikzm.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2nerkymmk.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2bmamlfav.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2qscypias.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2yuoongsd.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2kwraqpjx.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hpxsaadx.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2tdcbiqoz.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2bwrplwgo.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2dvefuokh.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2eznerebh.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2lpwiijue.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2svlhsxyi.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2cczloalq.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2mngdkjtq.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2ewrlnttn.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2gabdcqhy.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2brdhjqqs.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2ehkhdcgs.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2vsycpjut.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2ggkkqnhw.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2texkoung.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2oqbafxwu.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2xylepywg.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2dnpplwfo.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2daoepcvh.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2eocswdjy.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2cabaxcjx.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2abqelsqf.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2tummvqko.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2ybhtmyzs.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2fzmjzxuv.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2yrjfkeaf.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2lkgpmuzx.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2tlgovxbt.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2gnpjltnu.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2xxscvzps.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2czggfnck.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2mthuioqz.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2hlvznrkq.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2jklakuhl.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2skkerwod.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2ufomcvdw.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2ojifvwit.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2yueefeal.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2efjxsbgy.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2fqztsjgb.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2xgkwtpmk.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2kpichfna.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2zkuhiogm.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2odribwcv.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2hgwddjxu.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2kabugxpb.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2pavjmqon.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2tkawrzbg.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2kjyojgdc.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2jubvizse.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2beabvtfy.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2bsnnyqws.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2afffhnms.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2cstkmpir.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2jkrzbfjd.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2hnvkxakq.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2jkhtgqun.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2wahsdszm.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2gaummzgi.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2vvxmswfh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2bsnzyvlr.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2edsuhntw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mjjtdxfb.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2jhnjcskg.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2ymffjavz.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2ulvlfpyl.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2tzuxnzrq.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2bhmhmbuc.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2byapsztw.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2pbzvcnfd.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2xlfexqwh.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2cjllshqs.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2mtscqpte.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2iahiqtqe.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2zqxtvlfj.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2nlzpwvrl.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2owwzyizi.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2anjhuujx.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2ztxywecf.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2oneykgmo.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2gdumzqbw.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2cdctgpya.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2pqxvbiqs.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2nuzwufmp.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2qthfmqsg.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2fxkcjfqv.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2grrzqhvv.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2gjssamag.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2sylomdor.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2wqpzksfw.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2lcblhakv.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2zhcsjrfz.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2onfmmlmf.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2fhuppght.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2hhwpioqn.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2emmzmwmb.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2vzktdcuu.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2qyrftamw.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fggqaekb.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2wxongcsc.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2bnhmnjaf.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2byxnmhif.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2lgdohjwl.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2groelyfw.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2alpmgzxm.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2kgpqoarg.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2aeqmmnpo.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2ikhmyonb.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2hzfeoocw.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2dxifxbsp.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2ciynsrrk.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2zgwqjurw.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2hodcefip.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2tchxiknd.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2mokpsnug.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2hexnabso.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2qmckxdrm.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2mjaencnx.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2aslnarsn.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2zcvonbiz.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2cicemfpf.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2trefiunw.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2hnryknyw.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2htjvhejy.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2ktrjvmoc.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2ghozwmtk.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2xdjrjjxi.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2pocftpbf.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2wxwaynkw.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2dpnhdfrr.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rfsempeb.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2twwcdmir.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2srbgcpja.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2qqecndfe.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2ghthvlne.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2ibdzjadx.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2cqvwigvm.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2uisxqmmc.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2hkmlhceo.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2frbnltmq.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2iptyazcd.html


<!-- 参考信息 -->