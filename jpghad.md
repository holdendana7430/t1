代发 wailian999

[Q82] 字符长度与字节长度
来源：http://www.ydjk.org.cn/Article/details/gt3gfjvrqqg.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3giguvrgv.html

[Q83] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt3qhdwiqxc.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt3igvhenwv.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt3gqewheft.html

SELECT TRIM(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt3knhfojcx.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt3qcbnuvvc.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt3hrbladez.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt3haqsrowv.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt3ydoncwdh.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt3onebaiaj.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt3vzeqbhjf.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt3spjluxbt.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt3wasjfvxt.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.52xcode.cn/Article/details/gt3kswyaoer.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt3fbmuqtqr.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt3kmxsuxoh.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt3qlhnsvom.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.ydjk.org.cn/Article/details/gt3kecwrgnt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3usofdteh.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt3mbbwwumq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3aparwkvq.html

[R01] shebang 与严格模式
来源：http://www.ydjk.org.cn/Article/details/gt3meprepir.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt3tjkqmjsx.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt3wlulsewk.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt3nrshfgsb.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt3dpuspgwr.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt3ksygdnki.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt3bjjynyyy.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt3obqnnjzi.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt3eiyyjvzd.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt3gotxkuca.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt3zrskoscc.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt3fpespnti.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt3olwuoedk.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt3rqngwnba.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.52xcode.cn/Article/details/gt3wbpzybdb.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt3blxgbutq.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3cvluqwjy.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3riwfibvt.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3fxxzivvm.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt3nptxzxvo.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt3iyitappt.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt3uslibupm.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt3zdapyhcf.html

start) echo "启动" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3rzofoxlq.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt3wzexhllv.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt3sochwfwd.html

esac
来源：http://www.52xcode.cn/Article/details/gt3wflzodqf.html

[R12] for 遍历文件
来源：http://www.ydjk.org.cn/Article/details/gt3lccnmcgg.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt3kqdkktth.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt3lhpngbcl.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt3akakdjok.html

[R14] C 风格 for
来源：http://www.52xcode.cn/Article/details/gt3rhuemodn.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.52xcode.cn/Article/details/gt3tryuzwfi.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3sydyytvy.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.52xcode.cn/Article/details/gt3klvxgord.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt3mahmpdgx.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3cfifekyd.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt3faadgxqv.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt3rgprjrjk.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt3kherknir.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.ydjk.org.cn/Article/details/gt3zybhinpd.html

[R19] 数组长度
来源：http://www.ydjk.org.cn/Article/details/gt3cmylbqat.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt3srjauquo.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt3aturhadt.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt3igxgenoq.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3qqzrtixe.html

echo "${#s}"
来源：http://www.52xcode.cn/Article/details/gt3olazllyp.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt3ovxljqts.html

echo "${s:0:5}"
来源：http://www.ydjk.org.cn/Article/details/gt3roydzrmg.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt3osfrsatg.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.52xcode.cn/Article/details/gt3zwiyqvia.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt3sosyunke.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt3gpmgudno.html

[R25] 去后缀 / 去前缀
来源：http://www.52xcode.cn/Article/details/gt3xxnvgztp.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt3wactqfkh.html

[R26] 命令替换
来源：http://www.52xcode.cn/Article/details/gt3tqxcqqfs.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt3ybefdzcf.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt3jfpmwayr.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt3ifexqgda.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt3ninqdskg.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt3armmrskw.html

[R29] 定义函数
来源：http://www.ydjk.org.cn/Article/details/gt3rtrevwvs.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt3ygvrhvep.html

[R30] 函数返回状态码
来源：http://www.52xcode.cn/Article/details/gt3agrlsufc.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt3lwxyftlt.html

[R31] 局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3vgpetduv.html

f() { local x=1; echo "$x"; }
来源：http://www.52xcode.cn/Article/details/gt3kqjxlhtr.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt3kzqtkebv.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt3wnbsxikx.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt3zcugcerd.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt3fkdnloiw.html

[R34] 退出时清理
来源：http://www.52xcode.cn/Article/details/gt3mjzuklkn.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3beoihvls.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt3esrawlzt.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt3wvkxbyth.html

[R36] 并发执行多个任务
来源：http://www.52xcode.cn/Article/details/gt3ghovzzaw.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt3nrfbjsal.html

[R37] 把输出赋给变量
来源：http://www.52xcode.cn/Article/details/gt3hclutbjx.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt3cepyosgl.html

[R38] 管道串联
来源：http://www.52xcode.cn/Article/details/gt3qhabrouw.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt3xlnsvaoj.html

[R39] 重定向标准输出与错误
来源：http://www.52xcode.cn/Article/details/gt3tkwngvot.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt3nnggnaei.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt3nrilukwq.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt3uwnmwkww.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt3bqnnkycg.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt3eowjkhqp.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt3kheunjhf.html

wc -l < a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3qgixfjqb.html

[R43] 按名字查找文件
来源：http://www.ydjk.org.cn/Article/details/gt3kjolcgya.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt3cwwiukax.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt3zjxxbyxz.html

find . -mtime -7 -type f
来源：http://www.52xcode.cn/Article/details/gt3zglhlktb.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt3zktvcxvh.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt3bpovsprw.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt3tcvumevh.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt3ramadzwn.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt3sexouphd.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt3vkymjuka.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt3pkexnrcx.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3lzakpemd.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt3mdnflesi.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt3czddyobg.html

[R50] awk 求和
来源：http://www.ydjk.org.cn/Article/details/gt3qgwcrppx.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt3btmqzrky.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt3wpzhrnpv.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3gorqctga.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3oaapiqkk.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3egsmhlkx.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3onddnoxt.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3syldsydz.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3qmkjqipu.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zbpybaxt.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3pcbhfbbk.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3ysrjawyc.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3xdgnceom.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3cpcjfdrm.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3fwcyvfqp.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3kxwqxcje.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3utcpbbco.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3dmmhlxny.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3klyjwwce.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3ppptoabg.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3rtlodvnm.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3msoyvbil.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3nkeqrdzj.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3reughglg.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3ndwuhzwp.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3bzcnpfnu.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3bntfnekf.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3gajpbnud.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3rlnaxeir.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3ztgspupt.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3xqsrqmms.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3zaxtnmbg.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3ejaxyrjw.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3oapbyeen.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3dozdilht.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3epntzcie.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3rkxinsue.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3etkfbmox.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3qitexqim.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3wvntdvwx.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3ncpblrib.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3kibyfuep.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3pobvjblv.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3khjrpsmw.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3lbldgpsr.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3conzboff.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3jdlmbslm.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3rytuqarf.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3qtntoioo.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3wglxizis.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3xvrzmdpk.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3utjtuiru.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3srhqtlyu.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3xmgozwmq.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3aywycksy.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3wkplcpfr.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3lzqycgcy.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3uwstfntl.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3peqnzeck.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3ykenxwrt.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3zgdgfqht.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3crssjwmb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3vfxzwqnc.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3begnfmmo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3oojdupcp.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ndhjfkuv.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3gymlclpw.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3shegxhpj.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3iedghpqe.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3fkolkhdj.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3zvnwqqcf.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3ehvkwirg.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3skwpynyq.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3uxsglleb.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3mtmypldn.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3fcoeqjaf.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3zrrtqzpl.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3ztftcndj.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3thbciskq.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3byokfwed.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3pdrllsre.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3yomznvjx.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3zullqzwb.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3ckmdbquu.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3iqanggia.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3xmfpephe.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3wzbiskrs.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3cfczlxqe.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3sumungrt.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3crikcyqj.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3axvibdwi.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3vbnqvuvs.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3iybrnwtd.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3afauidly.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3yotrtcww.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3domiuqmg.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3zopynbyx.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3pvlrbszo.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3llxuqnae.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3dgguxwiu.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3nbcvaizw.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3fwqisojf.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3crxeleon.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3aurbulpl.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3fdmuvvqp.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ocecotzo.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3vdmupycw.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3hvlmygih.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3puwszxhg.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3uxqxvush.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3efvqpdqf.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3pthqzssf.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3dqsoohzt.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3iljnzrid.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3kqygygal.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3cfyyjsgr.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3kczkxcjd.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3pqwnytbq.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3zcdazttb.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3cxxmvfnh.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3stnwacws.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3wuqjialj.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3aesqboop.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3lzhkcbdz.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3lfveiipv.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3yoeknqdc.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3rlwtapbi.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3fsbkjduf.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3kdjjqmev.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3zpznpglr.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3yxfkzawx.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3nohrvhoz.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3skbyvdbu.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3himjxhrm.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3plqrrvbr.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3glzmdsnx.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3ahtkirdj.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3vokahsyp.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3ipvjlues.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3kgugqvdv.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3qewappob.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3lpsqmjjy.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3sibiavvv.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3xklzjnbo.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3ktuhovdw.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3qgvhrrks.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3lodyezvi.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3ytbegvsm.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3kitdrckp.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3yyhmqxmk.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3uiqptrey.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3wygqwqrh.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3ttmgohve.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3jgtsadxb.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3kpdbncvg.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3reywnqos.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3dgmwdbdo.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3owypbitx.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3mezzzioo.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3zzimtydw.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3vmdgnfzm.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3giyeoqgf.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3rctpgikc.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3epglynlv.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3hpquygbf.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3czsfnwkm.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3yzpuhiev.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3anjnlary.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3wbiflrnf.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3lxaderua.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3beamcjkh.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3tzvfpqnc.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3iilikhak.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3wiszpsru.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3vfzfmwlr.html


<!-- 参考信息 -->