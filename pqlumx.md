代发 wailian999

ROLLBACK TO sp1;
来源：http://www.ydjk.org.cn/Article/details/gt2ajlhcvcy.html

[Q69] 查看执行计划
来源：http://www.ydjk.org.cn/Article/details/gt2yaiudhqj.html

EXPLAIN SELECT * FROM users WHERE email = 'a@a.com';
来源：http://www.ydjk.org.cn/Article/details/gt2fvyrtzkg.html

[Q70] 更新统计信息
来源：http://www.52xcode.cn/Article/details/gt2oalycbcu.html

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2lujhokxu.html

[Q71] 查看建表语句
来源：http://www.52xcode.cn/Article/details/gt2kwxhsrpk.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2cgyauanb.html

[Q72] 查看索引
来源：http://www.ydjk.org.cn/Article/details/gt2rochuyan.html

SHOW INDEX FROM users;
来源：http://www.52xcode.cn/Article/details/gt2merwqtgi.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2eqzuyuld.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2eeqnpqjc.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2ghoaaxgc.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.52xcode.cn/Article/details/gt2snbyhnjh.html

[Q75] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2zujyofyp.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.52xcode.cn/Article/details/gt2tjrmbqty.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.52xcode.cn/Article/details/gt2gkfztkez.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2bewhperq.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.52xcode.cn/Article/details/gt2qzyrhtye.html

[Q77] 时间加减
来源：http://www.ydjk.org.cn/Article/details/gt2fxtvisyo.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.52xcode.cn/Article/details/gt2xtyrgxoc.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2ksyagpwu.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2grfkvhvo.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2fexxnfpg.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.ydjk.org.cn/Article/details/gt2ucqgpnxt.html

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2yeiglvyf.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ojpixtks.html

[Q81] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2qzizdbzo.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2nfsukeji.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2eeviespo.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ovmexgzr.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2stfjvefx.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2jkchazln.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2uywhlslk.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ztjtkzim.html

[Q85] 数值取整
来源：http://www.52xcode.cn/Article/details/gt2ahgrycxq.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2svttbqcp.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2jfcqyeeh.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2wzxvxulr.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2psmgmgbj.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2vdwwiluf.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2svjobiak.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.52xcode.cn/Article/details/gt2vbwoaiuw.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt2lhfboclv.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2vifiglfp.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2uxvpvaej.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2hypnqrwx.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2ilbnkcsf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2poqncdve.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2hceuzbga.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2bkuqefaq.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2xjdgsrgf.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2lpnertuc.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2vxzlgbrx.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2rksmaktn.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2zzudmdxy.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2iodbrgvv.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2xkrisrpq.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2gmcyxyij.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2vrdfmuxg.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2ybzwpmfw.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2ypginjpf.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2zsedkkas.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2ykdobups.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2ozcimrlv.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2kocfscdq.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2kuexzunq.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2jlbgfhge.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2idmxhkhn.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2kekdxjfz.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2oztgwtcx.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2aewcykvd.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2vnogtdmo.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2alhjwnem.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ydgyyfpn.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ipsurwzw.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2tcewcfvf.html

esac
来源：http://www.52xcode.cn/Article/details/gt2dnhathbl.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2nvfcmvgn.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ozqtjekt.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2lgqnfdzj.html

for i in {1..10}; do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt2gpxcicef.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2hcrtuzbz.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2kfrnspyb.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2jrpxkujq.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ulevudwt.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2lkdjtdtn.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2gapkxcoq.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2bwdwtavp.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2szpuembq.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2lmuhtcad.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2srulqdlh.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2fqefcwcv.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2tnbrudva.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2qcxdzoal.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2udjuancc.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2tcnyewdd.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2sansxlbn.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2sglsjdqq.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2qottsoye.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2qbjodjqn.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2tftxahba.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2cluvesav.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2juehxrpk.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2xbgrakqr.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2rrasijms.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2wbaxxcpg.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2oywjojbi.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2yjlmxvko.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2fttildrr.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2qhrsvaur.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2wgbyhzxp.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2rdersxvl.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2tkvovbra.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2eeaobtzl.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2ybnaffin.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2eillbgzj.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt2qidxrpyc.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2byuhiswh.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2orpjpyrz.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2grvtsawk.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2diaviszc.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2vkhbwdbk.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2bzekzupa.html

[R35] 后台执行并等待
来源：http://www.52xcode.cn/Article/details/gt2krillzbd.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2tiwnxwte.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2xmbobsnb.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.ydjk.org.cn/Article/details/gt2qllaycvq.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt2ddkqgabm.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2dgadxjly.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2vulkmhwb.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2ptyveecn.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2yfyabgzf.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2bxzavoru.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2lvfvclej.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2kxyjmqzv.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2clmprrrs.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2erqfyvsx.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2ffzzlkft.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2tfadiehl.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2llqnymwa.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2kzwvsaec.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2olpbugtd.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2wayiqrrj.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2yodqpwcl.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2jtjtgivs.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2qvvcaruy.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2forvrtsc.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2vvhmijcw.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2xdpqyase.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2uyykwcnn.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mdldieih.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2vhdbpmsc.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2arflgpnu.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2shtnyerq.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hsnlcikm.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2bpfucavf.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2prqcbcvk.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2ksroreux.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2wmcsthsc.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2rhntoiwz.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2rdugigba.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2kbuazxnw.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2obrpwohj.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2qmtevjcb.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2ttocihzi.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2reuzmqwl.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2qxbklqmh.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2rhlwdrzw.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2urnjbwli.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2uahokynu.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2njcrtdyk.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2kcqarisz.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2clbrbbrr.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2uetjwcoc.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2knpsaeqx.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2ahqvvfsr.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2ximyskfe.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2nroteclr.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2dizyymty.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2deehoqov.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2yzturqlf.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2nhpfgiqc.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2kbgexbol.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2wnjpdyec.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2yecsseqv.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2dzkpxzor.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2poroljrs.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2cisohyjo.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2kfpccdbl.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2arfoogmt.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jdudmxkk.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2fbxdmoyd.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2koavziaa.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2ewcdtkdm.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2vfwtrqmi.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2degdtfxw.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2gpspplgu.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2vanrnpuy.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2pgqnckmb.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2vfjwdqpk.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2vtrglteg.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2jwnpxmve.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2oascmtna.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2zfxxsbmo.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2jghlubrc.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2rmkyyliv.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2llqnmqrd.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2iktahimy.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2yohdzops.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2zfmmyuaz.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2azhiqezv.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2sjstcgib.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2etrnmwuw.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2hzfjuago.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2kvvahitl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nwvuggjb.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2dmwcqdpk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ldbxeamm.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2zsynhbvb.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2qngmoity.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2izyzvyvi.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2bvxqpeoe.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2fvgzzcur.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2optlkaxl.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2cflykmaz.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2psknkjbz.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2pxptagjb.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2lcxsrwuj.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2gtbffsyy.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2ljtmhfdd.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2bupvpmdx.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2zreormwl.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2pydssoge.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2exvwbzsx.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2cvmmcbwm.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2brmjatcf.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2bnzzprzp.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2rhqpbiva.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2gcxqsxdq.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2cuqqylem.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2kaprutia.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2zelxvoze.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2rlkjgtbh.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2axqcxqds.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2ravdvbfr.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2spnuhsgk.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2vtxjiuem.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2ogfzfxtp.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2ifowvuqe.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2unwjndas.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2uldorxjv.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2eoxsicpl.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2njhxtuui.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2uwvdwkkz.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2ewmgtdgx.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2dkxlwvgf.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2ldmaisdk.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2zacekuoz.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2jlojisuq.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2wuvhxreh.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2bifyahrv.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2txuvwoxw.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2zalbxxtx.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2apodimmn.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2bmewwsxi.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2mdwzxdft.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2ekokmrqb.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2ufvzlwli.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2cmgbcdlt.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2uecrvryj.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2sufxrzve.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2rswogtll.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2pbgfjgtj.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2laojneko.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2nlqjtdth.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2fdxxolha.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2dnvjtaxp.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2bqcpjtjy.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2ealyhmac.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2cfwjxioh.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2vevpceyi.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2cnnuzbit.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2whnsrrlx.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2skkjsroy.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2atykpegu.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uisbpolh.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2fmzinkol.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2ykzhsier.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2vihcugwa.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2auoghdkv.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2ksxlokja.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2ahadgrtl.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2pheczaal.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2vzokqqtw.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2exmhdbol.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2ificnsji.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2llollnym.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2penrqhsq.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2pikplvmb.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2mlrbvzgd.html


<!-- 参考信息 -->