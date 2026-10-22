代发 wailian999

ANALYZE TABLE users;
来源：http://www.52xcode.cn/Article/details/gt2pgsecrlk.html

[Q71] 查看建表语句
来源：http://www.ydjk.org.cn/Article/details/gt2jjhccvwi.html

SHOW CREATE TABLE users;          -- PostgreSQL: \d users
来源：http://www.ydjk.org.cn/Article/details/gt2oluhlbsq.html

[Q72] 查看索引
来源：http://www.52xcode.cn/Article/details/gt2ajzaetob.html

SHOW INDEX FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2aysryrri.html

[Q73] 查看表状态
来源：http://www.52xcode.cn/Article/details/gt2alnamzot.html

SHOW TABLE STATUS LIKE 'users';
来源：http://www.52xcode.cn/Article/details/gt2fgcppvff.html

[Q74] 强制使用索引
来源：http://www.52xcode.cn/Article/details/gt2rgvcqwme.html

SELECT * FROM users FORCE INDEX (idx_users_email) WHERE email = 'x';
来源：http://www.ydjk.org.cn/Article/details/gt2rqswbbbw.html

[Q75] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2cuppwjck.html

SELECT DATE_FORMAT(created_at, '%Y-%m') FROM orders;
来源：http://www.ydjk.org.cn/Article/details/gt2ylmxussl.html

-- PostgreSQL: to_char(created_at, 'YYYY-MM')
来源：http://www.ydjk.org.cn/Article/details/gt2tyhtkrsl.html

[Q76] 按天统计
来源：http://www.52xcode.cn/Article/details/gt2nlxzqeqx.html

SELECT DATE(created_at) AS d, COUNT(*) FROM orders GROUP BY d;
来源：http://www.ydjk.org.cn/Article/details/gt2sruiemil.html

[Q77] 时间加减
来源：http://www.52xcode.cn/Article/details/gt2blcbaobe.html

SELECT DATE_ADD(NOW(), INTERVAL 7 DAY);   -- PostgreSQL: now() + interval '7 day'
来源：http://www.ydjk.org.cn/Article/details/gt2ttmtmdzb.html

[Q78] 当前时间
来源：http://www.52xcode.cn/Article/details/gt2gvzobqgx.html

SELECT NOW(), CURDATE(), UNIX_TIMESTAMP();
来源：http://www.ydjk.org.cn/Article/details/gt2jcmngiwv.html

[Q79] 字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2nxrgfzbp.html

SELECT CONCAT(first_name, ' ', last_name) FROM users;   -- PostgreSQL: ||
来源：http://www.52xcode.cn/Article/details/gt2jlkrykao.html

[Q80] 字符串截取
来源：http://www.ydjk.org.cn/Article/details/gt2jiiqhydd.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nampkrob.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2wbkyvbgw.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gumjuzcn.html

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt2lkcajsqz.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2vhftduzi.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2vewmltyh.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2uznictvy.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2ysjowiiw.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2klerqbie.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2amvhqtpi.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2olwsqosi.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2bauoxvat.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2ehbmgkkr.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2vhwudgsx.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2uikwwlsd.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2dkldmlem.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2wdyqjnsv.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2auicdxpz.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2lssqozkv.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2bkmlashb.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2njhfyhuj.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt2xaykrlmh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2rxqlzjrp.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2jltuzgms.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zpnlbjkv.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2vpejbida.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2jbrmtdqf.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2oosuesbs.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2fkbmbjwv.html

name="Tom"; echo "$name"
来源：http://www.ydjk.org.cn/Article/details/gt2mpdiamrt.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2fbdazrsq.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2hnxohkry.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2qotdjazf.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2itnodpsp.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2eoaglzqo.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2zmkqeoko.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2flwcslnv.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2yumrcmbf.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2ifiiqfuq.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt2fxvptjpm.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2mhlaoyhr.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2dnfeusum.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2paztuogj.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2khnkcqie.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ogxearqw.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2guwivqtg.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2juauerlj.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2toajnkyo.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2yvyzzjxj.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2cembwuyc.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2wlguznqi.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2ufzrmgqt.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2sudafaje.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ezkopvii.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2fenwmvsx.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ejhhtiwy.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2beojschu.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2sgspjdtx.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2melhvqew.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2zaotwzwq.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2raziodbe.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2ovsakipf.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2rqykhbnk.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2zepjifvu.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2zicuciqt.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt2nqsuejij.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2flotstkz.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2cmlbeinx.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2xpmypgsx.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2pdoyzpns.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2pjmxixrt.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2qqnuxihp.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2nuugeivc.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt2cptscpjz.html

[R23] 字符串替换
来源：http://www.52xcode.cn/Article/details/gt2atdvehgx.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2hiqwxmvf.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2iqwlhfga.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2bihjhrgg.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2onjtknty.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2frutyobr.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt2oufmvbgu.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2yoqsdhdr.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2kebqgpfh.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2apaheppg.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2iewouwoh.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2uxbdztlj.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2xodlhnma.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2lgzzkmkm.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2wimjqzcv.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2npxybgjj.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2vxymyjng.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nkzkonaq.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2xmbwxchi.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2lfxfhcap.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2dmrdgpei.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2xdzuvsbu.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2kamhfcfz.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2yrdunvsq.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2noqojhnc.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2ajvsubjf.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2fsdcwebs.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2kofzpttf.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2llyccvml.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2qrimheih.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2bcyjeczu.html

cat a.txt | grep -i error | wc -l
来源：http://www.ydjk.org.cn/Article/details/gt2vxliuwpe.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt2mtxmybim.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2fiqbpwke.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2qvqtfhyf.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2nwdthggo.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2orghetip.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2gsodzzqu.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2glqnyqsr.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2bpgtbppt.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2bgoirtib.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2ihtsnhia.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2kjbhlzbs.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2olpewekz.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2kixrnean.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2tcmuqfor.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2gvlbrcop.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2pmbhxneg.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2vdzfthrc.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2cwddrsuj.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2grqpgykk.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2bshjznde.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2efrgaafv.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2bjaalakw.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt2hltywekk.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2vobiggnp.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2utpontcp.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2asqrzyel.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2epklbfot.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2izkygyfo.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2xgtjwjnc.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2odikezhk.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2ieoycscv.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2djblqkuu.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2bqrhaojq.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2prypszcd.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2lxypxwcf.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2nzvshtvk.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2oanznrro.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2wrhzxtjx.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2gopkfqye.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2coxpdbxq.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2atrkxzqh.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2dydaemvd.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2zsyzjlnh.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2pbigushn.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2lscppygy.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2buzscpbc.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2aafgwcep.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2mhnzmyfq.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2ftymvnbt.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2yezynifk.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2arnfcboq.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2yewcpaqh.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2eldftqdk.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2upcwgwxu.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2cuqkmtke.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2vuizvgwq.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2whopacuq.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2qkieswuv.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2pcrttgme.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2ofefvilx.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2tyhffsxw.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2qkohltxv.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2puqipwoh.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2ejlxvvqk.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2vznfvcvj.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2jkuuvvtw.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2buuxyccc.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2cvytftub.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2wvbcbmok.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2ncxzruww.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2voorugca.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2grhipwxm.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2uitextfk.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2kreemrlq.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2rdxauqkf.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2dryauboo.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2axipieuk.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2xeasfqyg.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2qhdwwqon.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2okkcsuwl.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2cztqnahh.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2mcpwxgws.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2msoqmeuh.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2vgvgbzjw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xxgxndsj.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2zrmoeeae.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ibzzdduv.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2mnigxovp.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2zyqzycrl.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2cjsythux.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2hamkhdzj.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2onhuxkwv.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2meybfgdk.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2mbwqkrsi.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2bcwfiiot.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2kcdvrkrh.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2ulomznyv.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2oilzuqnr.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2vhsdtand.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2lqnpsufc.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2dqccnghk.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2zyfqwedv.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2xauadsig.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2bjwjxknw.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2udnygala.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2dhfdpdzv.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2qfxrmmum.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2emrlxlmj.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2kcjodqsb.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2ivitttpz.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2vauiwkek.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2uaoeqvwx.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2vkcxrtmm.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2qllzjbdt.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2kzmxzrqr.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2nrzsqcyo.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2kcytdaaf.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2bfqnysky.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2halyfwqa.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2clgwpsos.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2mjqflbfx.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2sqdrbyfw.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2aohoujnl.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2qybibwsl.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2ebtxhjac.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2dunpsnvw.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2gijbmcqj.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2zqjkforl.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2qduaygog.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2bctybskq.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2tximuqku.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2ultpxjvv.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2acnmoseh.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2mhohalrv.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2jaqkbsvy.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2aeaffdjf.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2aachittg.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2duyiycov.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2gohomrmj.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2nxdnqdnk.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2deodlsiq.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2siezgmmy.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2sbwwlqvu.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2kcmgrvpw.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2qeextdrf.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2kljsslif.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2sjhhhgog.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2trgrdjsa.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2gahgyzgx.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2epppnnrh.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2vubzmuwa.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2isjtlazm.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2gttbujqt.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2dxmcprub.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2frnltbxz.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2rfkydxjt.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2cgcqfoeq.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2ovxiggre.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2esbplwmg.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2jpqicpxg.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2fjuwbxpv.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2vwbemmcp.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ttnclyzn.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2swbntlbf.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2vfqrztps.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2npkphcjl.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2tkexwrln.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2dpdwaorl.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2avqpiocq.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2vrwiiokd.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2ccqvjota.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2xlxnindv.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2jhoxgsmz.html


<!-- 参考信息 -->