代发 wailian999

set -euo pipefail
来源：http://baike.fanxiaobao.xyz/Article/details/gkwjcdhmw.sHtML

[R02] 变量赋值与使用
来源：http://www.share.fanxiaobao.xyz/Article/details/givqnkqfk.sHtML

name="Tom"; echo "$name"
来源：http://baike.fanxiaobao.xyz/Article/details/gvxmeppjn.sHtML

[R03] 只读变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdtnathrj.sHtML

readonly PI=3.14
来源：http://mobile.fanxiaobao.xyz/Article/details/geowilqhz.sHtML

[R04] 位置参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gfzjuuqnb.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.fanxiaobao.xyz/Article/details/gselowvvq.sHtML

[R05] 参数默认值
来源：http://www.share.fanxiaobao.xyz/Article/details/gsjhelnsz.sHtML

name="${1:-default}"
来源：http://www.share.fanxiaobao.xyz/Article/details/geiudpvce.sHtML

[R06] 判断命令是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gcukmqzzh.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtmykdewp.sHtML

[R07] if 判断文件
来源：http://3g.fanxiaobao.xyz/Article/details/gvxdsjdri.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcthjgnxl.sHtML

[R08] 数值比较
来源：http://wap.fanxiaobao.xyz/Article/details/gqhkavvaf.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://wap.fanxiaobao.xyz/Article/details/gfsxkwskj.sHtML

[R09] 字符串比较
来源：http://blog.fanxiaobao.xyz/Article/details/gwxuyjpox.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://3g.fanxiaobao.xyz/Article/details/grvdhbwlv.sHtML

[R10] 正则匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gvyqzwxac.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmcsvmyoz.sHtML

[R11] case 多分支
来源：http://m.share.fanxiaobao.xyz/Article/details/gjyxwovbf.sHtML

case "$1" in
来源：http://www.share.fanxiaobao.xyz/Article/details/glqigskox.sHtML

start) echo "启动" ;;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdmvzxbuu.sHtML

stop)  echo "停止" ;;
来源：http://blog.fanxiaobao.xyz/Article/details/gfhkcscab.sHtML

*)     echo "未知命令" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gocipvwbe.sHtML

esac
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbwdckpgz.sHtML

[R12] for 遍历文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gjplxvvut.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/guylmeydw.sHtML

[R13] for 计数循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gswjufcrm.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkrtnhawe.sHtML

[R14] C 风格 for
来源：http://www.blog.fanxiaobao.xyz/Article/details/gamathmwp.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gxhsskxsf.sHtML

[R15] while 逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/guenafupk.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://3g.fanxiaobao.xyz/Article/details/ggmovbhwi.sHtML

[R16] until 等待条件
来源：http://3g.fanxiaobao.xyz/Article/details/golvttrrf.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/grwgpjmuk.sHtML

[R17] 数组定义与取值
来源：http://baike.fanxiaobao.xyz/Article/details/glyzguetl.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/giaumtksd.sHtML

[R18] 遍历数组
来源：http://read.share.fanxiaobao.xyz/Article/details/gjcxcmbgn.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gixzmnbih.sHtML

[R19] 数组长度
来源：http://baike.fanxiaobao.xyz/Article/details/gijasmjua.sHtML

echo "${#arr[@]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gsrbefcqw.sHtML

[R20] 关联数组（字典）
来源：http://blog.fanxiaobao.xyz/Article/details/gwqydogsy.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gyvbckdbr.sHtML

[R21] 字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gzkrjdlgc.sHtML

echo "${#s}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gnwamvjno.sHtML

[R22] 截取子串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkxcwburp.sHtML

echo "${s:0:5}"
来源：http://wap.fanxiaobao.xyz/Article/details/gusqqahmu.sHtML

[R23] 字符串替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gmofddlbq.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fanxiaobao.xyz/Article/details/grgegyoap.sHtML

[R24] 大小写转换
来源：http://3g.fanxiaobao.xyz/Article/details/gtbkqpvbc.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gucyhrjqj.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fanxiaobao.xyz/Article/details/gpfecnsyc.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fanxiaobao.xyz/Article/details/gnoxilxuh.sHtML

[R26] 命令替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gtawagilk.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fanxiaobao.xyz/Article/details/guzgdjwnr.sHtML

[R27] 算术展开
来源：http://wap.fanxiaobao.xyz/Article/details/grnzkyiuv.sHtML

echo $((1 + 2 * 3))
来源：http://read.share.fanxiaobao.xyz/Article/details/gheuafhao.sHtML

[R28] 浮点运算
来源：http://wap.fanxiaobao.xyz/Article/details/ggqqyqmys.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fanxiaobao.xyz/Article/details/gxpacpsdm.sHtML

[R29] 定义函数
来源：http://blog.fanxiaobao.xyz/Article/details/gbfggicaw.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.fanxiaobao.xyz/Article/details/gzcrfllbb.sHtML

[R30] 函数返回状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gbcypcrku.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://read.share.fanxiaobao.xyz/Article/details/ggvggdvyd.sHtML

[R31] 局部变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gtqkhjeum.sHtML

f() { local x=1; echo "$x"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gjgyjiupf.sHtML

[R32] 参数个数校验
来源：http://3g.fanxiaobao.xyz/Article/details/gmpeuwzve.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxsppbsfc.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fanxiaobao.xyz/Article/details/gvkveyepf.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fanxiaobao.xyz/Article/details/gwgvaebtx.sHtML

[R34] 退出时清理
来源：http://mobile.fanxiaobao.xyz/Article/details/gsrrqbpnz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gntndplyg.sHtML

[R35] 后台执行并等待
来源：http://www.share.fanxiaobao.xyz/Article/details/gwyrnswdm.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.fanxiaobao.xyz/Article/details/gwglavwmn.sHtML

[R36] 并发执行多个任务
来源：http://blog.fanxiaobao.xyz/Article/details/gbhfkaije.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.fanxiaobao.xyz/Article/details/gvraosamk.sHtML

[R37] 把输出赋给变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gqhxvgbvz.sHtML

files=$(ls -1)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggleamqjk.sHtML

[R38] 管道串联
来源：http://www.blog.fanxiaobao.xyz/Article/details/gefpplbbc.sHtML

cat a.txt | grep -i error | wc -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gybmefghe.sHtML

[R39] 重定向标准输出与错误
来源：http://wap.fanxiaobao.xyz/Article/details/gripntrsx.sHtML

cmd > out.log 2>&1
来源：http://read.share.fanxiaobao.xyz/Article/details/gezjthzhx.sHtML

[R40] 追加写日志
来源：http://blog.fanxiaobao.xyz/Article/details/gwinhlzkp.sHtML

echo "log" >> out.log
来源：http://www.share.fanxiaobao.xyz/Article/details/gdbcvlqom.sHtML

[R41] 丢弃输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gzhckfugt.sHtML

cmd >/dev/null 2>&1
来源：http://wap.fanxiaobao.xyz/Article/details/gpxnnwomd.sHtML

[R42] 输入重定向
来源：http://blog.fanxiaobao.xyz/Article/details/gwrptkiin.sHtML

wc -l < a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gibmgblhc.sHtML

[R43] 按名字查找文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gbqjtezhw.sHtML

find . -name "*.log" -type f
来源：http://blog.fanxiaobao.xyz/Article/details/gkoiugotb.sHtML

[R44] 按修改时间查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gxbmvmizh.sHtML

find . -mtime -7 -type f
来源：http://m.share.fanxiaobao.xyz/Article/details/gtxndgrmy.sHtML

[R45] 批量删除
来源：http://www.blog.fanxiaobao.xyz/Article/details/giouoabgo.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fanxiaobao.xyz/Article/details/gtxxpnncw.sHtML

[R46] 递归替换文件内容
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcntlrryu.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.fanxiaobao.xyz/Article/details/gvtosonrr.sHtML

[R47] sed 单行替换
来源：http://3g.fanxiaobao.xyz/Article/details/gfkplfxpy.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gyzlfvygl.sHtML

[R48] awk 取指定列
来源：http://read.share.fanxiaobao.xyz/Article/details/gtifbtubj.sHtML

awk '{print $1, $3}' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/giseikyte.sHtML

[R49] awk 带条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/giqqismnw.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gukeqziug.sHtML

[R50] awk 求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gphwhueby.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqqinigeg.sHtML

[R51] 排序去重取前几
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvibheace.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.fanxiaobao.xyz/Article/details/gefzwbdwu.sHtML

[R52] 统计行数
来源：http://blog.fanxiaobao.xyz/Article/details/gpanixocg.sHtML

wc -l a.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gyypgxgqr.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fanxiaobao.xyz/Article/details/gyzxwgake.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.fanxiaobao.xyz/Article/details/gijhufhtm.sHtML

[R54] 比较两个文件
来源：http://blog.fanxiaobao.xyz/Article/details/gabyfnhcg.sHtML

diff a.txt b.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gzglfulsx.sHtML

[R55] 压缩与解压
来源：http://m.share.fanxiaobao.xyz/Article/details/gudoqjqxm.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fanxiaobao.xyz/Article/details/gdnyhwvae.sHtML

[R56] 远程拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gtzgrrtpq.sHtML

scp file user@host:/path/
来源：http://wap.fanxiaobao.xyz/Article/details/gsztlbfxc.sHtML

[R57] 远程执行命令
来源：http://baike.fanxiaobao.xyz/Article/details/gceugcshx.sHtML

ssh user@host 'uptime'
来源：http://mobile.fanxiaobao.xyz/Article/details/gywothlcw.sHtML

[R58] 下载文件
来源：http://baike.fanxiaobao.xyz/Article/details/glyjptcqo.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fanxiaobao.xyz/Article/details/glpcsmaip.sHtML

[R59] 发 POST JSON
来源：http://wap.fanxiaobao.xyz/Article/details/gqthuesms.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fanxiaobao.xyz/Article/details/gjovgzjzy.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gugghzwoa.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gszedvwht.sHtML

[R61] 磁盘占用
来源：http://blog.fanxiaobao.xyz/Article/details/ghyoajbqz.sHtML

df -h;  du -sh *
来源：http://mobile.fanxiaobao.xyz/Article/details/gbpuwttyi.sHtML

[R62] 找最占空间的文件
来源：http://wap.fanxiaobao.xyz/Article/details/gimwgifdr.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjawqowzx.sHtML

[R63] 内存与进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gtsnnrgyp.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.fanxiaobao.xyz/Article/details/gubghifly.sHtML

[R64] 结束进程
来源：http://read.share.fanxiaobao.xyz/Article/details/gsbmhpbqk.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fanxiaobao.xyz/Article/details/gknvfdjim.sHtML

[R65] 查看端口占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gzyqlnrqi.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsykicjer.sHtML

[R66] 定时任务
来源：http://baike.fanxiaobao.xyz/Article/details/giveegxcr.sHtML

crontab -e;  crontab -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gjqwapwyc.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyfprrmcx.sHtML

openssl rand -hex 16
来源：http://blog.fanxiaobao.xyz/Article/details/gbqslfijf.sHtML

[R68] 计算文件校验值
来源：http://www.share.fanxiaobao.xyz/Article/details/gfoqbqrvx.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gbooguagi.sHtML

[R69] 生成随机密码
来源：http://www.blog.fanxiaobao.xyz/Article/details/grgtdoyyo.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.fanxiaobao.xyz/Article/details/glwgkpuze.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gipltqgje.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggjzfixgm.sHtML

[R71] 日期格式化
来源：http://mobile.fanxiaobao.xyz/Article/details/gexczilht.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.fanxiaobao.xyz/Article/details/gfkdemgde.sHtML

[R72] 等待端口就绪
来源：http://m.share.fanxiaobao.xyz/Article/details/guzdrlnuv.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqbhuqruh.sHtML

[R73] 分割大日志
来源：http://m.share.fanxiaobao.xyz/Article/details/ggrjzwhcv.sHtML

split -l 1000 big.log part_
来源：http://m.share.fanxiaobao.xyz/Article/details/gqyxiolwh.sHtML

[R74] 批量重命名
来源：http://wap.fanxiaobao.xyz/Article/details/gvpdygaek.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gitwkygbe.sHtML

[R75] 导出环境变量
来源：http://3g.fanxiaobao.xyz/Article/details/gvemawuik.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fanxiaobao.xyz/Article/details/gjecyzkgz.sHtML

[R76] 使用临时文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggwhtaghf.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/ghcqfejnu.sHtML

[R77] 读取用户输入
来源：http://read.share.fanxiaobao.xyz/Article/details/gzsrkqsmz.sHtML

read -rp "请输入: " ans
来源：http://www.share.fanxiaobao.xyz/Article/details/gqaxwgbzl.sHtML

[R78] 交互式菜单
来源：http://m.share.fanxiaobao.xyz/Article/details/genwacske.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fanxiaobao.xyz/Article/details/ggowkiboq.sHtML

[R79] 解析命令行选项
来源：http://m.share.fanxiaobao.xyz/Article/details/gwobpkdji.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fanxiaobao.xyz/Article/details/glfazvzwz.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fanxiaobao.xyz/Article/details/griurfjta.sHtML

time ./run.sh
来源：http://3g.fanxiaobao.xyz/Article/details/gfhgxfhif.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/goztlupox.sHtML

S. C / C++ 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtgugtkor.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gxqpvonze.sHtML

[S01] C：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gqjopbshu.sHtML

#include <stdio.h>
来源：http://m.share.fanxiaobao.xyz/Article/details/gpaubkldw.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gwczwdvhj.sHtML

[S02] C：变量与格式化输出
来源：http://3g.fanxiaobao.xyz/Article/details/gjvkcfisz.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gajmexroi.sHtML

[S03] C：读入整数
来源：http://wap.fanxiaobao.xyz/Article/details/gjbmnwxdy.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fanxiaobao.xyz/Article/details/gwdwneerp.sHtML

[S04] C：字符串复制
来源：http://blog.fanxiaobao.xyz/Article/details/gkeaswcny.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fanxiaobao.xyz/Article/details/gxdzcxxnq.sHtML

[S05] C：字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gayvxjsyp.sHtML

strlen(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gszcvwmbl.sHtML

[S06] C：字符串比较
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqvaibwjs.sHtML

strcmp(a, b) == 0
来源：http://wap.fanxiaobao.xyz/Article/details/gamsiyaqz.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fanxiaobao.xyz/Article/details/gijrutbdr.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fanxiaobao.xyz/Article/details/gctkoftqw.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fanxiaobao.xyz/Article/details/gkuqhvlnn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpsndxlxk.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fanxiaobao.xyz/Article/details/gseezzvxr.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fanxiaobao.xyz/Article/details/guyixqbyn.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giypdaiia.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fanxiaobao.xyz/Article/details/guaghwlse.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gosaabrho.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fanxiaobao.xyz/Article/details/gsfluwdpr.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gdnmycppt.sHtML

fclose(f);
来源：http://baike.fanxiaobao.xyz/Article/details/gvpjwwnvz.sHtML

[S12] C：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/gmmqhwnju.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/ggmitzlff.sHtML

[S13] C：宏定义
来源：http://www.share.fanxiaobao.xyz/Article/details/gsmxxmfqw.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fanxiaobao.xyz/Article/details/guolzpkmw.sHtML

[S14] C：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gaomqovbz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fanxiaobao.xyz/Article/details/gnvcepmlo.sHtML

[S15] C：类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gmgnwwxep.sHtML

(double) a / b
来源：http://baike.fanxiaobao.xyz/Article/details/gpjoybctv.sHtML

[S16] C：位操作置位
来源：http://mobile.fanxiaobao.xyz/Article/details/grmhrhsmw.sHtML

x |= (1 << 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gndqjqiqo.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gcvslsamy.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfieylnoo.sHtML

[S18] C：命令行参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gawuiekmh.sHtML

int main(int argc, char **argv)
来源：http://www.share.fanxiaobao.xyz/Article/details/gmxvczqps.sHtML

[S19] C：快速排序
来源：http://3g.fanxiaobao.xyz/Article/details/gjtdiihgj.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gfbecucul.sHtML

[S20] C：二分查找
来源：http://www.share.fanxiaobao.xyz/Article/details/ggamezfsv.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/guhyntftl.sHtML

[S21] C：字符类别判断
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyquottix.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fanxiaobao.xyz/Article/details/gwvehxrda.sHtML

[S22] C：字符串转数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gwxzzhqrf.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpizubjxc.sHtML

[S23] C：随机数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gryikkstk.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fanxiaobao.xyz/Article/details/gmgxflruu.sHtML

[S24] C：获取本地时间
来源：http://m.share.fanxiaobao.xyz/Article/details/gnfeebyrw.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.fanxiaobao.xyz/Article/details/gfvkbxatx.sHtML

[S25] C：内存拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gxhbocivq.sHtML

memcpy(dst, src, n);
来源：http://3g.fanxiaobao.xyz/Article/details/gcqauywwv.sHtML

[S26] C：内存清零
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxzozjgml.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fanxiaobao.xyz/Article/details/guyrvravm.sHtML

[S27] C：定义常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbzaeoarj.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwpdyieuu.sHtML

[S28] C：静态变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqjejacgt.sHtML

static int counter = 0;
来源：http://read.share.fanxiaobao.xyz/Article/details/ghgutekfm.sHtML

[S29] C：变参函数
来源：http://wap.fanxiaobao.xyz/Article/details/gobepioon.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fanxiaobao.xyz/Article/details/grzhfgbde.sHtML

[S30] C：头文件保护
来源：http://m.share.fanxiaobao.xyz/Article/details/gciscblrl.sHtML

#ifndef X_H
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvygjwgsm.sHtML

#define X_H
来源：http://blog.fanxiaobao.xyz/Article/details/grcwmguye.sHtML

#endif
来源：http://read.share.fanxiaobao.xyz/Article/details/gowwmfpbt.sHtML

[S31] C++：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gkrbaxksc.sHtML

#include <iostream>
来源：http://www.blog.fanxiaobao.xyz/Article/details/geoofszpw.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gqcywbokl.sHtML

[S32] C++：字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gkggvpoal.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fanxiaobao.xyz/Article/details/gohyuqtmb.sHtML

[S33] C++：vector 增删
来源：http://m.share.fanxiaobao.xyz/Article/details/ggfvbdayz.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqjjxnxes.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxwcuiosb.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gllwjudqq.sHtML

[S35] C++：map
来源：http://www.share.fanxiaobao.xyz/Article/details/gjwunqgst.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gugilblpo.sHtML

[S36] C++：unordered_map
来源：http://m.share.fanxiaobao.xyz/Article/details/gntlqfkhf.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxlblgisf.sHtML

[S37] C++：set
来源：http://www.share.fanxiaobao.xyz/Article/details/gbaqznrlb.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbaarourc.sHtML

[S38] C++：排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gxzqwnptv.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtilzdhgp.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fanxiaobao.xyz/Article/details/gfemybxvq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fanxiaobao.xyz/Article/details/gcbeeamyn.sHtML

[S40] C++：查找元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gednnhvci.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fanxiaobao.xyz/Article/details/gzajeubhg.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaizrvolq.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gotkzdjoj.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ganhdirju.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fanxiaobao.xyz/Article/details/gjwnosntc.sHtML

[S43] C++：智能指针
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvjqjwuhx.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvyrflsjb.sHtML

[S44] C++：引用传参
来源：http://baike.fanxiaobao.xyz/Article/details/goqdlrhhb.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gzrkplqvk.sHtML

[S45] C++：lambda
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjnphqefs.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gpodevfjd.sHtML

[S46] C++：函数模板
来源：http://read.share.fanxiaobao.xyz/Article/details/gvrczjmku.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fanxiaobao.xyz/Article/details/ganjsgeze.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gfphywrtb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcwnyztmp.sHtML

[S48] C++：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gufhnkqjw.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzhfbgfst.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gnjefhhzu.sHtML

[S49] C++：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkmimabyj.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fanxiaobao.xyz/Article/details/ggumpixoo.sHtML

[S50] C++：格式化数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gfndslntm.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/ganbyqnha.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gmcztoxri.sHtML

static_cast<double>(a) / b
来源：http://baike.fanxiaobao.xyz/Article/details/grysuybzu.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gforbnkvp.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxjvpdgpe.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glqthivmn.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcfgxejbb.sHtML

[S54] C++：异常处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gwzoylsck.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcmajdlrq.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fanxiaobao.xyz/Article/details/gtzwlywuv.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.fanxiaobao.xyz/Article/details/gktvjjdue.sHtML

[S56] C++：optional
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggpispxno.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://baike.fanxiaobao.xyz/Article/details/gbzhssgaf.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghtkrubey.sHtML

constexpr int N = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gjilwvvee.sHtML

[S58] C++：命名空间
来源：http://blog.fanxiaobao.xyz/Article/details/goiwkcxsp.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzbfttule.sHtML

[S59] C++：静态断言
来源：http://baike.fanxiaobao.xyz/Article/details/gysezrtac.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fanxiaobao.xyz/Article/details/gjtcorazd.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvkegkrpv.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/gttywlsol.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtqyajfon.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fanxiaobao.xyz/Article/details/gnfaqsbff.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gndmkcphs.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gvsqxnamp.sHtML

println("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gcsvtxiyd.sHtML

[T02] Kotlin：变量
来源：http://read.share.fanxiaobao.xyz/Article/details/grbdiroph.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdkhzytxk.sHtML


<!-- 参考信息 -->