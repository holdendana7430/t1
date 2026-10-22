代发 wailian999

[Q82] 字符长度与字节长度
来源：http://www.52xcode.cn/Article/details/gt2ffziomgw.html

SELECT CHAR_LENGTH(name), LENGTH(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2hddpklcd.html

[Q83] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2pukaajky.html

SELECT UPPER(name), LOWER(name) FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2dcyriaao.html

[Q84] 去除首尾空格
来源：http://www.ydjk.org.cn/Article/details/gt2hftpaund.html

SELECT TRIM(name) FROM users;
来源：http://www.52xcode.cn/Article/details/gt2gilexpzw.html

[Q85] 数值取整
来源：http://www.ydjk.org.cn/Article/details/gt2tshxijsx.html

SELECT ROUND(3.567, 2), CEIL(3.1), FLOOR(3.9);
来源：http://www.ydjk.org.cn/Article/details/gt2hxfnnoeo.html

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2wlgvqqqt.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.ydjk.org.cn/Article/details/gt2pjqbjmkg.html

[Q87] JSON 字段做条件
来源：http://www.52xcode.cn/Article/details/gt2focxpeyf.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.ydjk.org.cn/Article/details/gt2ywzvwkig.html

[Q88] 行转列（条件聚合）
来源：http://www.52xcode.cn/Article/details/gt2fxxqnsey.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2eselrplo.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2exdigyyg.html

[Q89] 判断表是否存在
来源：http://www.52xcode.cn/Article/details/gt2jemuzdwp.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.ydjk.org.cn/Article/details/gt2ztcpwinq.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2avnlxctd.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2jsldykkx.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rzsrbmya.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2oldpicug.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2uqdmclcg.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2nbfaosph.html

#!/usr/bin/env bash
来源：http://www.ydjk.org.cn/Article/details/gt2pelwyvxq.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2aszeyrsy.html

[R02] 变量赋值与使用
来源：http://www.ydjk.org.cn/Article/details/gt2ipvasjgi.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2cnepmlbb.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2tstrnlll.html

readonly PI=3.14
来源：http://www.ydjk.org.cn/Article/details/gt2btpqqimi.html

[R04] 位置参数
来源：http://www.ydjk.org.cn/Article/details/gt2rnilevqx.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2lntbclgr.html

[R05] 参数默认值
来源：http://www.ydjk.org.cn/Article/details/gt2nfhmizey.html

name="${1:-default}"
来源：http://www.52xcode.cn/Article/details/gt2dogxmbcy.html

[R06] 判断命令是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2vwjaqyqa.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2yvsucyxm.html

[R07] if 判断文件
来源：http://www.ydjk.org.cn/Article/details/gt2rnnsejns.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ivqbzohd.html

[R08] 数值比较
来源：http://www.ydjk.org.cn/Article/details/gt2jrsybjjt.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.52xcode.cn/Article/details/gt2daejpaaw.html

[R09] 字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2lqgilawq.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.52xcode.cn/Article/details/gt2ktpaudiw.html

[R10] 正则匹配
来源：http://www.52xcode.cn/Article/details/gt2hidblobk.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2xysowprl.html

[R11] case 多分支
来源：http://www.52xcode.cn/Article/details/gt2mtpghlvl.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2jfuiqpud.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2xebmpxwt.html

stop)  echo "停止" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2trgrsraf.html

*)     echo "未知命令" ;;
来源：http://www.52xcode.cn/Article/details/gt2naznlzul.html

esac
来源：http://www.52xcode.cn/Article/details/gt2frponhad.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2jrkvakkn.html

for f in *.txt; do echo "$f"; done
来源：http://www.52xcode.cn/Article/details/gt2uejtiaik.html

[R13] for 计数循环
来源：http://www.ydjk.org.cn/Article/details/gt2gglczusy.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2cdlkokgo.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2znejrhbw.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2inazyixf.html

[R15] while 逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2uhdsmeoa.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2hesuzirl.html

[R16] until 等待条件
来源：http://www.ydjk.org.cn/Article/details/gt2nbgciqio.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2hzduxtqj.html

[R17] 数组定义与取值
来源：http://www.ydjk.org.cn/Article/details/gt2nkaqzjjg.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.52xcode.cn/Article/details/gt2vwyimpkl.html

[R18] 遍历数组
来源：http://www.ydjk.org.cn/Article/details/gt2oulopikw.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2snxljmpx.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2lucibkfn.html

echo "${#arr[@]}"
来源：http://www.ydjk.org.cn/Article/details/gt2itbmuvxb.html

[R20] 关联数组（字典）
来源：http://www.ydjk.org.cn/Article/details/gt2kfdxrsne.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.52xcode.cn/Article/details/gt2yezkecny.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2vhweqwks.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2hazfxnlb.html

[R22] 截取子串
来源：http://www.ydjk.org.cn/Article/details/gt2vvjavcnc.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2fccrsfiz.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2conscylx.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2jtdccpez.html

[R24] 大小写转换
来源：http://www.52xcode.cn/Article/details/gt2mfiqgeof.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.52xcode.cn/Article/details/gt2lfiqstti.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2lbhucadd.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2eivqpspb.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2fypehnrr.html

now=$(date +%F); echo "$now"
来源：http://www.ydjk.org.cn/Article/details/gt2hetqknkw.html

[R27] 算术展开
来源：http://www.ydjk.org.cn/Article/details/gt2prcbudyu.html

echo $((1 + 2 * 3))
来源：http://www.ydjk.org.cn/Article/details/gt2vusxawwe.html

[R28] 浮点运算
来源：http://www.52xcode.cn/Article/details/gt2mgxytplu.html

echo "scale=2; 10/3" | bc
来源：http://www.ydjk.org.cn/Article/details/gt2ojcadqmi.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2jyfucuni.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2rfllyfwu.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2vvppukns.html

f() { return 0; }; f || echo "失败了"
来源：http://www.ydjk.org.cn/Article/details/gt2onqgulzr.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2vxcmwgjb.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hfgykcjw.html

[R32] 参数个数校验
来源：http://www.ydjk.org.cn/Article/details/gt2dkoyvuxz.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.52xcode.cn/Article/details/gt2gwxvwtdd.html

[R33] 捕获错误并提示行号
来源：http://www.52xcode.cn/Article/details/gt2hlocmvhz.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.ydjk.org.cn/Article/details/gt2fyefkqgv.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2hvvokuqk.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2ulfkjevc.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2dyvrrbps.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.ydjk.org.cn/Article/details/gt2bpbkfgff.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2zwekfatr.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2agjiocvd.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2zliahija.html

files=$(ls -1)
来源：http://www.52xcode.cn/Article/details/gt2peggvpse.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2dqbyyhxa.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2yvusalbg.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2vzfnqfqr.html

cmd > out.log 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2ctnxvjtt.html

[R40] 追加写日志
来源：http://www.52xcode.cn/Article/details/gt2yqfdowsu.html

echo "log" >> out.log
来源：http://www.ydjk.org.cn/Article/details/gt2dcupnyeh.html

[R41] 丢弃输出
来源：http://www.52xcode.cn/Article/details/gt2hawfwpcf.html

cmd >/dev/null 2>&1
来源：http://www.52xcode.cn/Article/details/gt2faqflrhc.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2wgbblgac.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2qjhhckip.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2ihiyhwlh.html

find . -name "*.log" -type f
来源：http://www.52xcode.cn/Article/details/gt2rojnhjtu.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2ezelghyb.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2rdslvdcy.html

[R45] 批量删除
来源：http://www.ydjk.org.cn/Article/details/gt2xnotrrpu.html

find . -name "*.tmp" -delete
来源：http://www.ydjk.org.cn/Article/details/gt2akejrlsm.html

[R46] 递归替换文件内容
来源：http://www.ydjk.org.cn/Article/details/gt2tfjuimhd.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.ydjk.org.cn/Article/details/gt2swlhuvlz.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2usdysifv.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2lctdtspt.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2ixpkslra.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ocemjptv.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2cqiubivi.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2klpzdgck.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2sjtuahzo.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2axgcxifz.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2kxwnpvco.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2dzerqoiy.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2byeagjra.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2kdjzcdnl.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2xbkcajhh.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2docpzwip.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2fmxjyaus.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2xmjlohgu.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2fjsrrzue.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt2dvkegzgu.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2rwosaomk.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2iworcyis.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2jmjmwtlq.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2jjzywqkq.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2nesymvmg.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2efuqxbet.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ptfhybwe.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2albwadbg.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2dtosdsrv.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2eyazvovm.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2hjbryrfn.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2inndmywu.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2ycqhtqin.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2ftgziekr.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2vdytciwp.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2jkyzofyx.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2wwnnncrv.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2hnqamoul.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2pwtpweiv.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2gujwehpq.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2czzmdbqe.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2pdavjaaw.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2uscmalim.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2sucyweuz.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2mxqnqwaf.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2kbacwyjf.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2ezwgykoi.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2uysbviml.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2djrtfjoa.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2bzdjzfpk.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2frzulaop.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2jpfmnpxp.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2usupxqhf.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2fdzjwepb.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2jvgzyyca.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2uvxhbhjr.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2bsogwfzm.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2iuaivcxl.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2myzmymow.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2wuqtquqp.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2uvduvxwa.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2kloamoba.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2ardisnld.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2tlwjsekr.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2clzfaezt.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2zlllzpff.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2lormpeyo.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2cgnkomnq.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2fdddhcwv.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2twdztjtw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fvidouvg.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2hopwlfzn.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ytgqyork.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2qwbbfann.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2mtwoffbu.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2metaszaz.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2oynlyjlh.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2daantebk.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2qnynvyyj.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2specptkl.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2kbumdlzr.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2drieppyt.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2dgimnnla.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2vvzlsqul.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2qmikghlc.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2ogpsquvq.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2qviyyefb.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2qwrlmkeg.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2opxchcdy.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2ccoobjyg.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2kmuagufw.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2kkqdqrfd.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2malxrfbk.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2mzmfcdmx.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2buuvxkfo.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2zmdvesls.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2qgorvmni.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2jcelgswo.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2ehymbamp.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2ujqufouq.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2vpinqjxt.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2oaudqddw.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2dhhkodky.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2ttfipnxd.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2ochmducl.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2lhpupatn.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2ltwfniko.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2qrawbcwi.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2behgyscq.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2xfdhqsvv.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2vuawwnpp.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2ndxumezd.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2axjemwpf.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2aktpkfrh.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2pdvqpxov.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2kkcoiqaa.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2sinnspik.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2nmggmdpw.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2inwtahrm.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2onhvxkyd.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2ldpxknhz.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2isdsdrrj.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2rvbwtozw.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2mnakgxyw.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2csikjdaf.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2ltglnxrx.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2gybinpbd.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2bfxqayoj.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2jmnlvkro.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ojohxayc.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2dopcdhja.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2gdxfvfos.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2auvkxkeq.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2lwuwnnfw.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2wcnjngnu.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2pxbtufnc.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2samwqcyu.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2oiiphqjb.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2eolvqtsu.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2vkovqwqe.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2pzqvnuja.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2vbafkjje.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2mouxflrg.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2gryyfjpx.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2mpslkcma.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2qkjllgyd.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2vclmzbeu.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2hkalvncp.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2yndtwrnt.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2hxrkhjcj.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2zuyaytvx.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2dtjhjoop.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2hrufiijn.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2aqthzlhj.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2qosnpbaw.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2qgkadpvb.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2frqofvxk.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2iltnluxp.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2thbosrcf.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2xvumakob.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2qspieljk.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2gwwwcbxh.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2rgohyief.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2brywqkfd.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2lrtoaclg.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2hnistzen.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2aykdraiv.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2gvvooyzv.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2ycabgwvr.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2yyrcwyhs.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2pavffifl.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2uxzjgvrh.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2cugfixae.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2tttweatf.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2dkqenznr.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2dctkneuu.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2xhxhxyjo.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2wnaxjwth.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2pfwtkcri.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2tzchcvxa.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2fdyvkeer.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2vbkkzvxp.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2vzjxmvse.html


<!-- 参考信息 -->