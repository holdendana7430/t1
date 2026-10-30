代发 wailian999

SELECT COUNT(*) FROM information_schema.tables WHERE table_name = 'users';
来源：http://www.blog.fanxiaobao.xyz/Article/details/gopjclxha.sHtML

[Q90] 生成序号列
来源：http://wap.fanxiaobao.xyz/Article/details/gpjuehkrl.sHtML

SELECT @i := @i + 1 AS seq, name FROM users, (SELECT @i := 0) x;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/getholqlc.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/glgojotyw.sHtML

R. Bash 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkjnkfzmw.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gqpfqtqsb.sHtML

[R01] shebang 与严格模式
来源：http://wap.fanxiaobao.xyz/Article/details/gadwixdmv.sHtML

#!/usr/bin/env bash
来源：http://mobile.fanxiaobao.xyz/Article/details/gpbmefsvs.sHtML

set -euo pipefail
来源：http://www.share.fanxiaobao.xyz/Article/details/gakynhpaz.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fanxiaobao.xyz/Article/details/giszkndfh.sHtML

name="Tom"; echo "$name"
来源：http://www.share.fanxiaobao.xyz/Article/details/ggtsjawwb.sHtML

[R03] 只读变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsxqxmugh.sHtML

readonly PI=3.14
来源：http://mobile.fanxiaobao.xyz/Article/details/gmwfevvyp.sHtML

[R04] 位置参数
来源：http://blog.fanxiaobao.xyz/Article/details/gjavvrkve.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfgcqsusd.sHtML

[R05] 参数默认值
来源：http://blog.fanxiaobao.xyz/Article/details/gngbtseqo.sHtML

name="${1:-default}"
来源：http://wap.fanxiaobao.xyz/Article/details/gjxokcwmy.sHtML

[R06] 判断命令是否存在
来源：http://read.share.fanxiaobao.xyz/Article/details/gqulbkcfs.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://blog.fanxiaobao.xyz/Article/details/gwbjqwwbu.sHtML

[R07] if 判断文件
来源：http://3g.fanxiaobao.xyz/Article/details/gkurrhllt.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/gikeaocvu.sHtML

[R08] 数值比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gmuwjmxxk.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/grywnueyp.sHtML

[R09] 字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gifhfkfxu.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfzpdrmps.sHtML

[R10] 正则匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gosjlkrim.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://blog.fanxiaobao.xyz/Article/details/glhagmizi.sHtML

[R11] case 多分支
来源：http://www.share.fanxiaobao.xyz/Article/details/glhdkqqsn.sHtML

case "$1" in
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfrqutwju.sHtML

start) echo "启动" ;;
来源：http://baike.fanxiaobao.xyz/Article/details/glftwapho.sHtML

stop)  echo "停止" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gthnzomfr.sHtML

*)     echo "未知命令" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gghlweopb.sHtML

esac
来源：http://www.share.fanxiaobao.xyz/Article/details/gkstbtoap.sHtML

[R12] for 遍历文件
来源：http://m.share.fanxiaobao.xyz/Article/details/guyxszrel.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gnzduyrgv.sHtML

[R13] for 计数循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/grfwkwdol.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gbirknhrd.sHtML

[R14] C 风格 for
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdmhtfcup.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gwbnyqpee.sHtML

[R15] while 逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gymjhqroh.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gcfvgeuka.sHtML

[R16] until 等待条件
来源：http://m.share.fanxiaobao.xyz/Article/details/gfzxleutq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gizijbncs.sHtML

[R17] 数组定义与取值
来源：http://m.share.fanxiaobao.xyz/Article/details/gcjkdaurr.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkwnumoat.sHtML

[R18] 遍历数组
来源：http://blog.fanxiaobao.xyz/Article/details/gvmhffywm.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gqkyfnspn.sHtML

[R19] 数组长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gjhelhndm.sHtML

echo "${#arr[@]}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkwwlvgmf.sHtML

[R20] 关联数组（字典）
来源：http://www.share.fanxiaobao.xyz/Article/details/gabxkfomo.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gxslikowy.sHtML

[R21] 字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/gzsbpywya.sHtML

echo "${#s}"
来源：http://blog.fanxiaobao.xyz/Article/details/gphhhinpz.sHtML

[R22] 截取子串
来源：http://www.share.fanxiaobao.xyz/Article/details/gdazjlnpp.sHtML

echo "${s:0:5}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gbtvbdmdz.sHtML

[R23] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gzsiawiet.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://m.share.fanxiaobao.xyz/Article/details/ggrdrhbvp.sHtML

[R24] 大小写转换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gucjgziiq.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gzjigipen.sHtML

[R25] 去后缀 / 去前缀
来源：http://3g.fanxiaobao.xyz/Article/details/gezxmqgob.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://3g.fanxiaobao.xyz/Article/details/gocnltkbu.sHtML

[R26] 命令替换
来源：http://mobile.fanxiaobao.xyz/Article/details/glvsmjduh.sHtML

now=$(date +%F); echo "$now"
来源：http://mobile.fanxiaobao.xyz/Article/details/gymdtbzmc.sHtML

[R27] 算术展开
来源：http://baike.fanxiaobao.xyz/Article/details/glbtwszxb.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghwinnrjw.sHtML

[R28] 浮点运算
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjnecobia.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.fanxiaobao.xyz/Article/details/gmtqikiri.sHtML

[R29] 定义函数
来源：http://wap.fanxiaobao.xyz/Article/details/gkmitfccd.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fanxiaobao.xyz/Article/details/gdapgdncw.sHtML

[R30] 函数返回状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gyjdrlrhl.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdgcdmmsl.sHtML

[R31] 局部变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjgkvzasg.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gjdfmcctg.sHtML

[R32] 参数个数校验
来源：http://www.share.fanxiaobao.xyz/Article/details/gibdodrpc.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/grauypqep.sHtML

[R33] 捕获错误并提示行号
来源：http://m.share.fanxiaobao.xyz/Article/details/gjmpiikmu.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://m.share.fanxiaobao.xyz/Article/details/gmvtfijph.sHtML

[R34] 退出时清理
来源：http://m.share.fanxiaobao.xyz/Article/details/gdbyahlza.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/gurticwzd.sHtML

[R35] 后台执行并等待
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcaqvkvcj.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://3g.fanxiaobao.xyz/Article/details/gnitysolc.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkwujrqwb.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fanxiaobao.xyz/Article/details/gfroataky.sHtML

[R37] 把输出赋给变量
来源：http://mobile.fanxiaobao.xyz/Article/details/guvdbrsua.sHtML

files=$(ls -1)
来源：http://www.share.fanxiaobao.xyz/Article/details/gdothvrtq.sHtML

[R38] 管道串联
来源：http://www.share.fanxiaobao.xyz/Article/details/gufzjhfoz.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gthnjsnhc.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fanxiaobao.xyz/Article/details/gwswmtlbb.sHtML

cmd > out.log 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gspoflwiv.sHtML

[R40] 追加写日志
来源：http://baike.fanxiaobao.xyz/Article/details/gzijzpuxn.sHtML

echo "log" >> out.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gpbxsbjjt.sHtML

[R41] 丢弃输出
来源：http://3g.fanxiaobao.xyz/Article/details/gkokrfecp.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/grgsqsiiz.sHtML

[R42] 输入重定向
来源：http://blog.fanxiaobao.xyz/Article/details/guelhfger.sHtML

wc -l < a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gzlaztugo.sHtML

[R43] 按名字查找文件
来源：http://baike.fanxiaobao.xyz/Article/details/gmyppexcw.sHtML

find . -name "*.log" -type f
来源：http://www.share.fanxiaobao.xyz/Article/details/gnckxscqc.sHtML

[R44] 按修改时间查找
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmpiutkwi.sHtML

find . -mtime -7 -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gcwmoekyt.sHtML

[R45] 批量删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvfsovowd.sHtML

find . -name "*.tmp" -delete
来源：http://baike.fanxiaobao.xyz/Article/details/gfexwugpo.sHtML

[R46] 递归替换文件内容
来源：http://3g.fanxiaobao.xyz/Article/details/ggqoviftf.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://3g.fanxiaobao.xyz/Article/details/gjuuaolms.sHtML

[R47] sed 单行替换
来源：http://3g.fanxiaobao.xyz/Article/details/gbveoemrp.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gjengcbsg.sHtML

[R48] awk 取指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/geapyaark.sHtML

awk '{print $1, $3}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/ghvwfdnly.sHtML

[R49] awk 带条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmzekdlta.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdbgmuppx.sHtML

[R50] awk 求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gaybaepbj.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbhdqjkoj.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtqzzcrly.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.fanxiaobao.xyz/Article/details/gfiytfarr.sHtML

[R52] 统计行数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gviyhiied.sHtML

wc -l a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfzyyxxfv.sHtML

[R53] 查看文件头与实时尾
来源：http://baike.fanxiaobao.xyz/Article/details/glhzuthka.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gidsjeqgr.sHtML

[R54] 比较两个文件
来源：http://mobile.fanxiaobao.xyz/Article/details/girrylelc.sHtML

diff a.txt b.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gbhagbpfm.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjhvuoxqo.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fanxiaobao.xyz/Article/details/gmckkmdvk.sHtML

[R56] 远程拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gxpnrmhqp.sHtML

scp file user@host:/path/
来源：http://www.share.fanxiaobao.xyz/Article/details/gykvabyll.sHtML

[R57] 远程执行命令
来源：http://3g.fanxiaobao.xyz/Article/details/gvljwqvgc.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghavvpdyv.sHtML

[R58] 下载文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gpgzpryrk.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fanxiaobao.xyz/Article/details/gcnuvluwk.sHtML

[R59] 发 POST JSON
来源：http://3g.fanxiaobao.xyz/Article/details/gcblvknos.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fanxiaobao.xyz/Article/details/gxjtpuudj.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gwmuqitfn.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.fanxiaobao.xyz/Article/details/gbjezyesc.sHtML

[R61] 磁盘占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwkmlhbut.sHtML

df -h;  du -sh *
来源：http://read.share.fanxiaobao.xyz/Article/details/gqvxibifh.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvqxwykdp.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fanxiaobao.xyz/Article/details/gzqejwjlw.sHtML

[R63] 内存与进程
来源：http://blog.fanxiaobao.xyz/Article/details/gnztwnkjv.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fanxiaobao.xyz/Article/details/gsorhciwj.sHtML

[R64] 结束进程
来源：http://read.share.fanxiaobao.xyz/Article/details/grbezjjcr.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gulzqfyrc.sHtML

[R65] 查看端口占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqrzkillv.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fanxiaobao.xyz/Article/details/gclbcmoxy.sHtML

[R66] 定时任务
来源：http://3g.fanxiaobao.xyz/Article/details/gpppaumze.sHtML

crontab -e;  crontab -l
来源：http://baike.fanxiaobao.xyz/Article/details/gygrewzjc.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fanxiaobao.xyz/Article/details/gvfnvgqpv.sHtML

openssl rand -hex 16
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfdtpmeit.sHtML

[R68] 计算文件校验值
来源：http://wap.fanxiaobao.xyz/Article/details/gnmglvnjg.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gwbttaftm.sHtML

[R69] 生成随机密码
来源：http://www.share.fanxiaobao.xyz/Article/details/gmkkhfgij.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fanxiaobao.xyz/Article/details/gklxqadtd.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbclraqei.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fanxiaobao.xyz/Article/details/gnulghzes.sHtML

[R71] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/gsvievbtj.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fanxiaobao.xyz/Article/details/geyxuknek.sHtML

[R72] 等待端口就绪
来源：http://blog.fanxiaobao.xyz/Article/details/gmkarifhk.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gdumbggol.sHtML

[R73] 分割大日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/galjeoocf.sHtML

split -l 1000 big.log part_
来源：http://www.share.fanxiaobao.xyz/Article/details/gdptxhque.sHtML

[R74] 批量重命名
来源：http://www.share.fanxiaobao.xyz/Article/details/gotvwcccp.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/glkxyycjs.sHtML

[R75] 导出环境变量
来源：http://3g.fanxiaobao.xyz/Article/details/gtsecbjrq.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fanxiaobao.xyz/Article/details/gcxcnqqiw.sHtML

[R76] 使用临时文件
来源：http://3g.fanxiaobao.xyz/Article/details/gmnaveoox.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gfqzfylkd.sHtML

[R77] 读取用户输入
来源：http://m.share.fanxiaobao.xyz/Article/details/giajtxqhm.sHtML

read -rp "请输入: " ans
来源：http://mobile.fanxiaobao.xyz/Article/details/gxjhrfwep.sHtML

[R78] 交互式菜单
来源：http://blog.fanxiaobao.xyz/Article/details/gvjubzjyy.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fanxiaobao.xyz/Article/details/gmgmhucdj.sHtML

[R79] 解析命令行选项
来源：http://mobile.fanxiaobao.xyz/Article/details/gjtofiltb.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fanxiaobao.xyz/Article/details/gleketcmh.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fanxiaobao.xyz/Article/details/gsaerhlxs.sHtML

time ./run.sh
来源：http://www.blog.fanxiaobao.xyz/Article/details/guyylgdpa.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbylepiur.sHtML

S. C / C++ 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gqvqrzpuq.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gdgfhxpdy.sHtML

[S01] C：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goxvubmsn.sHtML

#include <stdio.h>
来源：http://baike.fanxiaobao.xyz/Article/details/gctneeqwn.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fanxiaobao.xyz/Article/details/gxjjkdxus.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkmekkvlc.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fanxiaobao.xyz/Article/details/gaswpnthg.sHtML

[S03] C：读入整数
来源：http://mobile.fanxiaobao.xyz/Article/details/gdbahcspk.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbefasyhy.sHtML

[S04] C：字符串复制
来源：http://baike.fanxiaobao.xyz/Article/details/gdktkcbbu.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fanxiaobao.xyz/Article/details/gnhquygwr.sHtML

[S05] C：字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwgwyxhjf.sHtML

strlen(s)
来源：http://read.share.fanxiaobao.xyz/Article/details/gqbyxcblm.sHtML

[S06] C：字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfhnftmie.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goyigsbms.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grszshjeq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fanxiaobao.xyz/Article/details/ggqjircye.sHtML

[S08] C：动态内存分配与释放
来源：http://m.share.fanxiaobao.xyz/Article/details/gnjhfovhx.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gydgdcokl.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fanxiaobao.xyz/Article/details/gxlpglxce.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fanxiaobao.xyz/Article/details/gpwqaqffo.sHtML

[S10] C：指针与解引用
来源：http://baike.fanxiaobao.xyz/Article/details/gilhrqtsu.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fanxiaobao.xyz/Article/details/gfkfhfflg.sHtML

[S11] C：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/ghjwxfhck.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fanxiaobao.xyz/Article/details/gskgtisrj.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gsjviocqv.sHtML

fclose(f);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvfknkfod.sHtML

[S12] C：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gkhdnowfi.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gsixpsgox.sHtML

[S13] C：宏定义
来源：http://blog.fanxiaobao.xyz/Article/details/gmngwnnlr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fanxiaobao.xyz/Article/details/gauafckwk.sHtML

[S14] C：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gugqjdbii.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.fanxiaobao.xyz/Article/details/gaovehmik.sHtML

[S15] C：类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gogzqoqsi.sHtML

(double) a / b
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpnnsocie.sHtML

[S16] C：位操作置位
来源：http://wap.fanxiaobao.xyz/Article/details/ggnzlaqkf.sHtML

x |= (1 << 3);
来源：http://baike.fanxiaobao.xyz/Article/details/golxkdprw.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gywivyoly.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.fanxiaobao.xyz/Article/details/glxilemmt.sHtML

[S18] C：命令行参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwacmhuys.sHtML

int main(int argc, char **argv)
来源：http://m.share.fanxiaobao.xyz/Article/details/giatwsxfx.sHtML

[S19] C：快速排序
来源：http://baike.fanxiaobao.xyz/Article/details/gwktuksok.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gguftszia.sHtML

[S20] C：二分查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gzvtxissr.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbmftwfbt.sHtML

[S21] C：字符类别判断
来源：http://3g.fanxiaobao.xyz/Article/details/gubnqlady.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fanxiaobao.xyz/Article/details/gqupozais.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcbsynpbo.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fanxiaobao.xyz/Article/details/gjfiukhwj.sHtML

[S23] C：随机数
来源：http://wap.fanxiaobao.xyz/Article/details/gkketmnfb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.fanxiaobao.xyz/Article/details/gapupyoeu.sHtML

[S24] C：获取本地时间
来源：http://mobile.fanxiaobao.xyz/Article/details/gmoqhhocb.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxhphwfil.sHtML

[S25] C：内存拷贝
来源：http://m.share.fanxiaobao.xyz/Article/details/ggbmtprmk.sHtML

memcpy(dst, src, n);
来源：http://wap.fanxiaobao.xyz/Article/details/gufthlxju.sHtML

[S26] C：内存清零
来源：http://baike.fanxiaobao.xyz/Article/details/gycatlxmg.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gopasvxct.sHtML

[S27] C：定义常量
来源：http://wap.fanxiaobao.xyz/Article/details/grustpmqk.sHtML

const double PI = 3.14159;
来源：http://wap.fanxiaobao.xyz/Article/details/ggrmxacfv.sHtML

[S28] C：静态变量
来源：http://3g.fanxiaobao.xyz/Article/details/gsdxqkwjm.sHtML

static int counter = 0;
来源：http://blog.fanxiaobao.xyz/Article/details/gojgpznpa.sHtML

[S29] C：变参函数
来源：http://wap.fanxiaobao.xyz/Article/details/guaskqrfg.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.fanxiaobao.xyz/Article/details/gzecapzhv.sHtML

[S30] C：头文件保护
来源：http://3g.fanxiaobao.xyz/Article/details/gnycadrcw.sHtML

#ifndef X_H
来源：http://blog.fanxiaobao.xyz/Article/details/ggryvscrz.sHtML

#define X_H
来源：http://3g.fanxiaobao.xyz/Article/details/grvtnyfyu.sHtML

#endif
来源：http://read.share.fanxiaobao.xyz/Article/details/gjhpftwmc.sHtML

[S31] C++：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gisbpttbq.sHtML

#include <iostream>
来源：http://www.share.fanxiaobao.xyz/Article/details/gkspdzrup.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gzptamhdh.sHtML

[S32] C++：字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpedcygzd.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fanxiaobao.xyz/Article/details/gjlgevglb.sHtML

[S33] C++：vector 增删
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkohhtjab.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fanxiaobao.xyz/Article/details/ggfzyhzuf.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fanxiaobao.xyz/Article/details/gwqrpeynf.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gepbabvcb.sHtML

[S35] C++：map
来源：http://3g.fanxiaobao.xyz/Article/details/gyenjojdx.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gpdgpomom.sHtML

[S36] C++：unordered_map
来源：http://read.share.fanxiaobao.xyz/Article/details/gasdzdinf.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gxskadrio.sHtML

[S37] C++：set
来源：http://m.share.fanxiaobao.xyz/Article/details/gbgwyfmlz.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gfuwbycxu.sHtML

[S38] C++：排序
来源：http://blog.fanxiaobao.xyz/Article/details/ggvkbrsdm.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fanxiaobao.xyz/Article/details/gaxfxxjtr.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.fanxiaobao.xyz/Article/details/gmfblnuve.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fanxiaobao.xyz/Article/details/gegukovwg.sHtML

[S40] C++：查找元素
来源：http://3g.fanxiaobao.xyz/Article/details/gygxaianz.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gtpvguqoc.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtlugfods.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fanxiaobao.xyz/Article/details/gvpzkxywd.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fanxiaobao.xyz/Article/details/gtzzrkfph.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fanxiaobao.xyz/Article/details/gbfbxtfgl.sHtML

[S43] C++：智能指针
来源：http://wap.fanxiaobao.xyz/Article/details/gevuoefqs.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fanxiaobao.xyz/Article/details/guunoqtgm.sHtML

[S44] C++：引用传参
来源：http://wap.fanxiaobao.xyz/Article/details/ghjgdtady.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gpuqzshch.sHtML

[S45] C++：lambda
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwkihjmhp.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gxyjnhzie.sHtML

[S46] C++：函数模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gmpkfhibv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/grdmooxsj.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gwpdonlou.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fanxiaobao.xyz/Article/details/gqrwfwryc.sHtML

[S48] C++：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gwgkowscp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzowjlvey.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gchbfindh.sHtML

[S49] C++：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gdumhkiwz.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fanxiaobao.xyz/Article/details/guwnhrvrk.sHtML

[S50] C++：格式化数字
来源：http://wap.fanxiaobao.xyz/Article/details/guhltuxpo.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghixigbrp.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/glvlfmrlu.sHtML

static_cast<double>(a) / b
来源：http://wap.fanxiaobao.xyz/Article/details/goanwhhis.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvjuvoqrf.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fanxiaobao.xyz/Article/details/gvmeyttnr.sHtML

[S53] C++：移动语义
来源：http://www.share.fanxiaobao.xyz/Article/details/ggifcefkx.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fanxiaobao.xyz/Article/details/guksuzeky.sHtML

[S54] C++：异常处理
来源：http://baike.fanxiaobao.xyz/Article/details/gzykmryzc.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/gytzbebyh.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjqafwdpa.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fanxiaobao.xyz/Article/details/gbkhenlib.sHtML

[S56] C++：optional
来源：http://blog.fanxiaobao.xyz/Article/details/gxqoxctzo.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gsyblnssr.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmwjrbsux.sHtML

constexpr int N = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gnywmjfaj.sHtML

[S58] C++：命名空间
来源：http://www.share.fanxiaobao.xyz/Article/details/gxenirsmu.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbcqdyfpb.sHtML

[S59] C++：静态断言
来源：http://blog.fanxiaobao.xyz/Article/details/gosapllen.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fanxiaobao.xyz/Article/details/gtblursdl.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gvhdpfcni.sHtML


<!-- 参考信息 -->