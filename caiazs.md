代发 wailian999

[Q80] 字符串截取
来源：http://www.52xcode.cn/Article/details/gt2wjiczqtd.html

SELECT SUBSTRING(name, 1, 3) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2xmyxxcmw.html

[Q81] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2uuabltvq.html

SELECT REPLACE(name, 'a', 'b') FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2ggpgknsw.html

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2yfnehlis.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2ginxjfez.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2eauhpjjo.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2nelvkqsd.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2kohvqqhs.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2qhqzkpkd.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2bosawvwu.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2jyhouyqz.html

[Q86] 读取 JSON 字段
来源：http://www.52xcode.cn/Article/details/gt2foxqbaay.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2mshrwfsc.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2wgrywzcp.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2ofrsfdhp.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2qimvolhg.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2rybtnkpp.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2uoyjcoex.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2bitveypu.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2lrphwpnb.html

[Q90] 生成序号列
来源：http://www.52xcode.cn/Article/details/gt2dfnwyear.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2qyiecmjh.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2blpgdblw.html

R. Bash 专题
来源：http://www.ydjk.org.cn/Article/details/gt2uprsjrvx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qoeqsrul.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt2xxiezmqb.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2rkarrnrr.html

set -euo pipefail
来源：http://www.ydjk.org.cn/Article/details/gt2yyqbpczg.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2yomzlgic.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2trejdkpk.html

[R03] 只读变量
来源：http://www.52xcode.cn/Article/details/gt2mulvonie.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2zuvcvocb.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2jliqvfge.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.ydjk.org.cn/Article/details/gt2rrrrxugp.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2mdogkxng.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2hadctraz.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2olzoxety.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2htykfkxd.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2zfwnjymj.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2mxxknqou.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2qhxjdysa.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2ezdurldi.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2kartyezb.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2oswadisp.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2sndkwsnc.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.52xcode.cn/Article/details/gt2napjdtff.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2uhsnnblg.html

case "$1" in
来源：http://www.ydjk.org.cn/Article/details/gt2bjaxhfcx.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2zbqbngkq.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2ukgoezrq.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2bgmgntuw.html

esac
来源：http://www.52xcode.cn/Article/details/gt2bidsocvw.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2spexrkue.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2xpbegjwj.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2cnfrhcoi.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2ercmjull.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt2wxrcrfkv.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2pomgmyzd.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2gtthmmcn.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt2rlvdpnmp.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2tpihxyiz.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2icuvtbqi.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2vuipflmv.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2zmidghff.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2zwksxmhm.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2nmtrgtsr.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt2ghtrhktt.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2nagqhdkf.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2wkdhueag.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2cfijffol.html

[R21] 字符串长度
来源：http://www.52xcode.cn/Article/details/gt2ghjvogbp.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt2uedciihv.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2vhyktmrj.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2airlmgdq.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2htjpssxq.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt2oozsaxhq.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2wucdiuav.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2juwakvkf.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt2ewsoncpf.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.ydjk.org.cn/Article/details/gt2gxjfztmn.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2oongwvwz.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2zyulclhn.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2zmtmkqcv.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2unujgmwt.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2gfvaccpa.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2cilgdtzt.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt2kloilofv.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.ydjk.org.cn/Article/details/gt2zdxunylg.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt2ymyfubbo.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2jdntpujm.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2swwvhvdt.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gdarogrv.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2exmpdvnd.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2imqdljdd.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2xukcpmsn.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2ghczijkd.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt2dmowkwbj.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2zvergdcz.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2hjgbgxxa.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2helsdwad.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt2fdlawddh.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2ynteqhes.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2ecnrfbqh.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2djpnqarg.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt2naikgnkb.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2ysofymcl.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2dszbahqd.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2kggrubqd.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2cohqxbhx.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2bfrgwxdj.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2qqbzglvz.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2swlmuxop.html

[R42] 输入重定向
来源：http://www.52xcode.cn/Article/details/gt2yeegctam.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2jmymzmok.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt2mdrizsaj.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2ayrfidpi.html

[R44] 按修改时间查找
来源：http://www.ydjk.org.cn/Article/details/gt2djlycccc.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt2qslcuxkn.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2yireipim.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2xcezmqvu.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2fuczwzqs.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2dtrdspas.html

[R47] sed 单行替换
来源：http://www.52xcode.cn/Article/details/gt2iyfzoqct.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2fosevlbq.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2gsonjazr.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2pnnjsqol.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2soxrvdwc.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.52xcode.cn/Article/details/gt2ginfexaa.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2svgdccta.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2scndzilh.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2ebahgivp.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2bmebynxf.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2hgsegsjm.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2luvgmcbb.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2mdhqpbqu.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2javwfzut.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2xreszjwd.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2jjyspfju.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2lcqynokz.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2badmsmyo.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2jhdtwvsd.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2tggzkgja.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2eavzkroc.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2nofjqbeu.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2gclrmsko.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2ybauowan.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2tgnnsiqb.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2prdkiyid.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2lslvxgod.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2gdajuzks.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2ywufzphh.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2qciisonk.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2euryeonq.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2qhbztpxv.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2kendnyeu.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2qobfcshr.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2oufdfktm.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2htldzzrm.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2msnxvfrv.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2ueiqnjkm.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2ovwwadqe.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2onbsnbxr.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2mtlaejeb.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2kyocwxyf.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2typgrazn.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ouxhwdnf.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2dcenhqtp.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2wngigqlk.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2exlsdsgz.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2ldpmiebl.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2otiohrpj.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2kijrmhrm.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2dnsrrlia.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2oexwqrlw.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2ngirwwzq.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2wywzjxhv.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2jcastnsi.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2buzwernk.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2yxiyjfyb.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2ycohjtkq.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2zyekcxkc.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2dlirrfwr.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2tmlnvstb.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2nwxduldo.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2awocebdp.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2fprwfvuw.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2fnjgubjl.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2mvumsrky.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2hukmihud.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2fzywtgoj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2zbsixsfa.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2sscuhogs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2psgjjzio.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2pgrzuxiw.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2vuielhws.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2ewjcauft.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2qhgyoeen.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2cptyjuxc.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2xvlaytie.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2hgjrebmj.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2xdcjaobj.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2eqaxstui.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2ymtjxelc.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2jamxgzhe.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2pnueauwc.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2otljshgg.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2qvznzbzj.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2arvfjsfb.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2grxmfvad.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2ijlngpje.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2mhnvcsgl.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2dzgrmpdo.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2jcbfratb.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2foajugij.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2ooevwogu.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2bglrfkov.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2gsqjskyz.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2ivvhnthn.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2gkgtlyga.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2iuzlkdas.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2wyrtoren.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2znebjeur.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2sgilccxc.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2kgjyscuv.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2leplxgui.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2dqqtebfk.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2aukghcia.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2mxikclys.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2pxbxmxnl.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2nieqzxfw.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2hgdvykqo.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2xjitebrb.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2fclncqsl.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2ndhhhbya.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2rxlgyebs.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2krsofxgm.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2sdlzhwco.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2ahlydlhy.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2kcgosrdq.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2crfekxau.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2rqegupft.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2jqdalrxn.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2lylbqlse.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2jvbjclyg.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2weuwhdch.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2rmfuzbat.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2kfnovymn.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2iaypvusl.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2tijdasqj.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2shaoajlt.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2drzzydxe.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2sogkgubp.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2ivsysowt.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2resfywjs.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2ttflfkly.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2gwslxztf.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2seplgiiy.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2frtstjkz.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2smkyobuc.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2evymdotc.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2govqowvz.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2kqhibrxo.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2zwhcelep.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2siuqkpey.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2onybohgn.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2zxrjqugg.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2etdvvydw.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2vbmmgyxh.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2nhqykjge.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2jtiigooe.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2xsnpcgpc.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2oedpsasq.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2cozjqolb.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2owenjadu.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2wctvhmne.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2whenqrxt.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2mppotppr.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2wxbulozo.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2lcnsixkg.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2ezamxuxr.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2yxmwmybr.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2wttrvqyz.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2bchtqmud.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2vmxctbrq.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2vsydqnwg.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2gobruwve.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2skdxhfpg.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2lpzijtqr.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2qmocadft.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2dcjnwzln.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2madvyicc.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qwndunor.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2owkxelyp.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2rxvejgrx.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2jrwkdbuo.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2clopujlc.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2hxlyxxrn.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2ukajsbky.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2rsbezmgk.html


<!-- 参考信息 -->