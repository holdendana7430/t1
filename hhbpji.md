代发 wailian999

[Q86] 读取 JSON 字段
来源：http://www.ydjk.org.cn/Article/details/gt2ardwvwic.html

SELECT data->>'$.name' FROM t;    -- PostgreSQL: data->>'name'
来源：http://www.52xcode.cn/Article/details/gt2vipepuok.html

[Q87] JSON 字段做条件
来源：http://www.ydjk.org.cn/Article/details/gt2itzqorij.html

SELECT * FROM t WHERE JSON_EXTRACT(data, '$.age') > 18;
来源：http://www.52xcode.cn/Article/details/gt2ypowkcpi.html

[Q88] 行转列（条件聚合）
来源：http://www.ydjk.org.cn/Article/details/gt2iskaeodj.html

SELECT SUM(CASE WHEN status = 1 THEN 1 ELSE 0 END) AS s1,
来源：http://www.ydjk.org.cn/Article/details/gt2lyaicpxy.html

SUM(CASE WHEN status = 2 THEN 1 ELSE 0 END) AS s2 FROM users;
来源：http://www.ydjk.org.cn/Article/details/gt2omukvztx.html

[Q89] 判断表是否存在
来源：http://www.ydjk.org.cn/Article/details/gt2effjvtpq.html

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.52xcode.cn/Article/details/gt2ltdoylra.html

[Q90] 生成序号列
来源：http://www.ydjk.org.cn/Article/details/gt2fyrfvguu.html

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.52xcode.cn/Article/details/gt2ybkjopsk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jvmxcwvp.html

R. Bash 专题
来源：http://www.52xcode.cn/Article/details/gt2vdoitrwj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2eweayggf.html

[R01] shebang 与严格模式
来源：http://www.52xcode.cn/Article/details/gt2krstiygu.html

#!/usr/bin/env bash
来源：http://www.52xcode.cn/Article/details/gt2lmsyevxm.html

set -euo pipefail
来源：http://www.52xcode.cn/Article/details/gt2gjoljrhg.html

[R02] 变量赋值与使用
来源：http://www.52xcode.cn/Article/details/gt2wxxztmyt.html

name="Tom"; echo "$name"
来源：http://www.52xcode.cn/Article/details/gt2korykhld.html

[R03] 只读变量
来源：http://www.ydjk.org.cn/Article/details/gt2jlofdxex.html

readonly PI=3.14
来源：http://www.52xcode.cn/Article/details/gt2igddoipn.html

[R04] 位置参数
来源：http://www.52xcode.cn/Article/details/gt2ywrpjvgu.html

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.52xcode.cn/Article/details/gt2jvjteakt.html

[R05] 参数默认值
来源：http://www.52xcode.cn/Article/details/gt2zvjsmhfn.html

name="${1:-default}"
来源：http://www.ydjk.org.cn/Article/details/gt2lrsnxftt.html

[R06] 判断命令是否存在
来源：http://www.52xcode.cn/Article/details/gt2nndbigda.html

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2ipihzook.html

[R07] if 判断文件
来源：http://www.52xcode.cn/Article/details/gt2bnbtmqtu.html

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2hhhhivtv.html

[R08] 数值比较
来源：http://www.52xcode.cn/Article/details/gt2nnlgqpaj.html

if (( a > b )); then echo "a 更大"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2zcxhfrby.html

[R09] 字符串比较
来源：http://www.52xcode.cn/Article/details/gt2tbshgzcp.html

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2lxtqxigl.html

[R10] 正则匹配
来源：http://www.ydjk.org.cn/Article/details/gt2cpkcpvpf.html

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.ydjk.org.cn/Article/details/gt2ehzljbpy.html

[R11] case 多分支
来源：http://www.ydjk.org.cn/Article/details/gt2tmqtwswf.html

case "$1" in
来源：http://www.52xcode.cn/Article/details/gt2bgymonma.html

start) echo "启动" ;;
来源：http://www.52xcode.cn/Article/details/gt2vbrieqox.html

stop)  echo "停止" ;;
来源：http://www.52xcode.cn/Article/details/gt2iouqmbas.html

*)     echo "未知命令" ;;
来源：http://www.ydjk.org.cn/Article/details/gt2cnfnxyod.html

esac
来源：http://www.ydjk.org.cn/Article/details/gt2wnxvntal.html

[R12] for 遍历文件
来源：http://www.52xcode.cn/Article/details/gt2zdmcbotq.html

for f in *.txt; do echo "$f"; done
来源：http://www.ydjk.org.cn/Article/details/gt2gnopozmy.html

[R13] for 计数循环
来源：http://www.52xcode.cn/Article/details/gt2fbqgortu.html

for i in {1..10}; do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2fcfggbrd.html

[R14] C 风格 for
来源：http://www.ydjk.org.cn/Article/details/gt2yflbsjlo.html

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://www.ydjk.org.cn/Article/details/gt2kyhqrtqj.html

[R15] while 逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2kjvxbftt.html

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.ydjk.org.cn/Article/details/gt2gnncxrdn.html

[R16] until 等待条件
来源：http://www.52xcode.cn/Article/details/gt2iggqjflg.html

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2ahlgjnez.html

[R17] 数组定义与取值
来源：http://www.52xcode.cn/Article/details/gt2zfzxlqgm.html

arr=(a b c); echo "${arr[0]}"
来源：http://www.ydjk.org.cn/Article/details/gt2clahewhk.html

[R18] 遍历数组
来源：http://www.52xcode.cn/Article/details/gt2xcfattus.html

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.52xcode.cn/Article/details/gt2qlhnuwrp.html

[R19] 数组长度
来源：http://www.52xcode.cn/Article/details/gt2bwfmqlol.html

echo "${#arr[@]}"
来源：http://www.52xcode.cn/Article/details/gt2mipdhudl.html

[R20] 关联数组（字典）
来源：http://www.52xcode.cn/Article/details/gt2aylniakr.html

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.ydjk.org.cn/Article/details/gt2byupwxxc.html

[R21] 字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2oekubboz.html

echo "${#s}"
来源：http://www.ydjk.org.cn/Article/details/gt2atdubcyi.html

[R22] 截取子串
来源：http://www.52xcode.cn/Article/details/gt2vukbpaua.html

echo "${s:0:5}"
来源：http://www.52xcode.cn/Article/details/gt2bhafzkhb.html

[R23] 字符串替换
来源：http://www.ydjk.org.cn/Article/details/gt2anlrdgft.html

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.ydjk.org.cn/Article/details/gt2tcciehkf.html

[R24] 大小写转换
来源：http://www.ydjk.org.cn/Article/details/gt2cdshmzis.html

echo "${s^^}"; echo "${s,,}"
来源：http://www.ydjk.org.cn/Article/details/gt2wlubswba.html

[R25] 去后缀 / 去前缀
来源：http://www.ydjk.org.cn/Article/details/gt2zyfznbgi.html

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.52xcode.cn/Article/details/gt2fqdhdtvt.html

[R26] 命令替换
来源：http://www.ydjk.org.cn/Article/details/gt2mmbacmic.html

now=$(date +%F); echo "$now"
来源：http://www.52xcode.cn/Article/details/gt2usxpxxze.html

[R27] 算术展开
来源：http://www.52xcode.cn/Article/details/gt2wvkcdqzm.html

echo $((1 + 2 * 3))
来源：http://www.52xcode.cn/Article/details/gt2hkdhauph.html

[R28] 浮点运算
来源：http://www.ydjk.org.cn/Article/details/gt2xgyjpxwg.html

echo "scale=2; 10/3" | bc
来源：http://www.52xcode.cn/Article/details/gt2elwgogmw.html

[R29] 定义函数
来源：http://www.52xcode.cn/Article/details/gt2ejthsjte.html

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.52xcode.cn/Article/details/gt2icljxxhq.html

[R30] 函数返回状态码
来源：http://www.ydjk.org.cn/Article/details/gt2gpcnywjm.html

f() { return 0; }; f || echo "失败了"
来源：http://www.52xcode.cn/Article/details/gt2jhlnvyuo.html

[R31] 局部变量
来源：http://www.52xcode.cn/Article/details/gt2kkhbucum.html

f() { local x=1; echo "$x"; }
来源：http://www.ydjk.org.cn/Article/details/gt2egxpafzv.html

[R32] 参数个数校验
来源：http://www.52xcode.cn/Article/details/gt2upmvlkgo.html

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.ydjk.org.cn/Article/details/gt2hlbbyjph.html

[R33] 捕获错误并提示行号
来源：http://www.ydjk.org.cn/Article/details/gt2eyvrbrlx.html

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://www.52xcode.cn/Article/details/gt2myalzvvy.html

[R34] 退出时清理
来源：http://www.ydjk.org.cn/Article/details/gt2vuyuqzts.html

trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2zszjupyi.html

[R35] 后台执行并等待
来源：http://www.ydjk.org.cn/Article/details/gt2ytqxqnfk.html

sleep 5 & pid=$!; wait "$pid"
来源：http://www.52xcode.cn/Article/details/gt2wgukxpvb.html

[R36] 并发执行多个任务
来源：http://www.ydjk.org.cn/Article/details/gt2xsjbrmla.html

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.52xcode.cn/Article/details/gt2sjbgpivr.html

[R37] 把输出赋给变量
来源：http://www.ydjk.org.cn/Article/details/gt2qrlclxee.html

files=$(ls -1)
来源：http://www.ydjk.org.cn/Article/details/gt2ahoqblwl.html

[R38] 管道串联
来源：http://www.ydjk.org.cn/Article/details/gt2rqoynynj.html

cat a.txt | grep -i error | wc -l
来源：http://www.52xcode.cn/Article/details/gt2jnwnytkk.html

[R39] 重定向标准输出与错误
来源：http://www.ydjk.org.cn/Article/details/gt2uukvezbp.html

cmd > out.log 2>&1
来源：http://www.52xcode.cn/Article/details/gt2twyxzrmp.html

[R40] 追加写日志
来源：http://www.ydjk.org.cn/Article/details/gt2upfpvrju.html

echo "log" >> out.log
来源：http://www.52xcode.cn/Article/details/gt2mlrsbjzh.html

[R41] 丢弃输出
来源：http://www.ydjk.org.cn/Article/details/gt2wdqfxvmo.html

cmd >/dev/null 2>&1
来源：http://www.ydjk.org.cn/Article/details/gt2byljhqne.html

[R42] 输入重定向
来源：http://www.ydjk.org.cn/Article/details/gt2rviedhbs.html

wc -l < a.txt
来源：http://www.52xcode.cn/Article/details/gt2srclqlfg.html

[R43] 按名字查找文件
来源：http://www.52xcode.cn/Article/details/gt2webjranx.html

find . -name "*.log" -type f
来源：http://www.ydjk.org.cn/Article/details/gt2ozuhdjsy.html

[R44] 按修改时间查找
来源：http://www.52xcode.cn/Article/details/gt2ksubzsgp.html

find . -mtime -7 -type f
来源：http://www.ydjk.org.cn/Article/details/gt2jqlvvwvs.html

[R45] 批量删除
来源：http://www.52xcode.cn/Article/details/gt2tnujewjg.html

find . -name "*.tmp" -delete
来源：http://www.52xcode.cn/Article/details/gt2ghnhayns.html

[R46] 递归替换文件内容
来源：http://www.52xcode.cn/Article/details/gt2sfzkpsuj.html

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.52xcode.cn/Article/details/gt2xcjedmhl.html

[R47] sed 单行替换
来源：http://www.ydjk.org.cn/Article/details/gt2mtaxvjxv.html

sed -i 's/foo/bar/g' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2yxxcnsji.html

[R48] awk 取指定列
来源：http://www.ydjk.org.cn/Article/details/gt2mtjjrlzv.html

awk '{print $1, $3}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2xnldnccz.html

[R49] awk 带条件
来源：http://www.52xcode.cn/Article/details/gt2cwomymut.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2okqjjirn.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2blydevck.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2yphjvdlq.html

[R51] 排序去重取前几
来源：http://www.52xcode.cn/Article/details/gt2vurrmxsf.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2zumbcdco.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2odmrlfce.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2jvcwfsej.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2fbzttajj.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2fjwiyfhh.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt2ctiiqycb.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2djtvyqih.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2wlkumslf.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2kpozuafn.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2lkfglqwy.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2xmmrszgn.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2yzzowjzj.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2bhgubacu.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2vratccjf.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2veuuprtc.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2ncnqthdn.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2oorrrcfp.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2ynbwkblt.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2qfrsvzzz.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2sfdlqiaf.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2pjlmbygx.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2alhcidgp.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2kwgfzenn.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2plppwzej.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2wlmjqjmj.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2enbfyjcc.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2cdcmlrkr.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2thgcqedt.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2hgbtpvyo.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2rdkdqoex.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2hawtvxdy.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2hmkomykp.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2csbclwtj.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2sayeqcvv.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2tembaabz.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2twvqfvhs.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2xcskyhsd.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2dexmuatw.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2dzvfrdlf.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2knkukebf.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2lqwcplbu.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2mxwlyevb.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2hzzkvmqh.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2bebtkuvd.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2qnjafoli.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2psrwbtab.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2gyrtiqcb.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2pfixraas.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2wdkitxmf.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2zgfoezaz.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2pvqgmlax.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2qojjoawv.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2kzrweyom.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2bdzzqqot.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2odabjypo.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2cyycqxcz.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2xmolhada.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2yhdilfkv.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2rwmtfjhr.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ovidpiqd.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2bitcetry.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2fuixzoqm.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2wxgsbixd.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2tviplnwe.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2mwvmkzss.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2rltseesc.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2edjqcdse.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2lubkhbhp.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2jsgzkuza.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2qqskwhql.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2gcwerkdy.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2vjipkglf.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2jqvksyem.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2uzzncqng.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2wmjbfavd.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2kzouioms.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2hkzpeobh.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2nmqwtuub.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2xrncemmn.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2cffkidxp.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2rdoruohd.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2uihgrune.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2pdrwhtyx.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2uaphelqd.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2gibpjacu.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2kucdhqsr.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2ucjybraq.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2pdautyso.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2quoyvoci.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2mzwpinwx.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2tkzdheht.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2xdepfdol.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2tonpgdxj.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2tyrsomme.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2pktodjqs.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2bnxtloco.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2ninzzlyu.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2etoljcvr.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2uutirbdv.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2jxmfshes.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2zbywvsnh.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2qvwxmbwf.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2yrqqmmht.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2lmlkeoyq.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2ezoqjihi.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2yklugfex.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2fthmjqju.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2elliodry.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2qtdzkgrl.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2vuzoobbx.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2ihkytnui.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2swzcrnxm.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2eoptgcdl.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2aylhmuwa.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2bnkidnts.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2jmbepulp.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2tqzhnkiz.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2wsudexqq.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2bjthfyyv.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2obmdpgxm.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2ihwbkdsp.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2bhpgdqgm.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2ldvdogem.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2wgdquhgl.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2mizpwoei.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2hrawuinr.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2ztxdhnqo.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2edwaohpk.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2hjfwmzhr.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2ibvmcuvi.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2jhsyatkr.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2okfoxdzn.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2paxtjzdd.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2mkbkpbrf.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2oxdozbun.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2dsccyjvj.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2omhlkxxm.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2zohzgkxv.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2pcqgtgmf.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ykwbhgfs.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2emlnuqhh.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2dnevzduh.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2sgbrtiou.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2pmpnvmkv.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2dajkewff.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2kmafkexu.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2grhezotd.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2batarvml.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2rrglrbjf.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2hhoojxzd.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2jijxdoaa.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2rlnjoqwy.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2qnowlbcx.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2lotwyunp.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2scxrclzo.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2mxzctfiz.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2qludijrt.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2ishbhpme.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2pvuffsqa.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2zgdcjzvr.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2utnwyupm.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2wxtsrvuo.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2mottnztp.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2cwhwpbjn.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2ndocnsoy.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2hilzrgsr.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2yvqgznud.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2ayjmobfl.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2pfgdtmyx.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2wrrnnnyk.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2sidodrgy.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2pohgvjas.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt2rizabcpn.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2umixkyqp.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2wgyivsxd.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2iazbdhiv.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2lnigqlhn.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2svmxfosh.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2xcselqeo.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2wwhwlrlh.html


<!-- 参考信息 -->