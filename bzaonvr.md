代发 wailian999

set -euo pipefail
来源：http://m.share.fanxiaobao.xyz/Article/details/gyhcjcfxo.sHtML

[R02] 变量赋值与使用
来源：http://read.share.fanxiaobao.xyz/Article/details/ggvbjywho.sHtML

name="Tom"; echo "$name"
来源：http://m.share.fanxiaobao.xyz/Article/details/ghrwgkmfr.sHtML

[R03] 只读变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/grviggotj.sHtML

readonly PI=3.14
来源：http://mobile.fanxiaobao.xyz/Article/details/gxwfazbhx.sHtML

[R04] 位置参数
来源：http://www.blog.fanxiaobao.xyz/Article/details/giwgefeeh.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://m.share.fanxiaobao.xyz/Article/details/ghmklldpb.sHtML

[R05] 参数默认值
来源：http://baike.fanxiaobao.xyz/Article/details/gprjfdlom.sHtML

name="${1:-default}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gfymmvyxp.sHtML

[R06] 判断命令是否存在
来源：http://baike.fanxiaobao.xyz/Article/details/gatuijjmb.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/guifqupgg.sHtML

[R07] if 判断文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsidrswop.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjaahmzma.sHtML

[R08] 数值比较
来源：http://3g.fanxiaobao.xyz/Article/details/gxaeabqnu.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfoxerurs.sHtML

[R09] 字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/gogcvpntb.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjlqrwtmo.sHtML

[R10] 正则匹配
来源：http://baike.fanxiaobao.xyz/Article/details/ggyybujvp.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://baike.fanxiaobao.xyz/Article/details/gthwtjors.sHtML

[R11] case 多分支
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfqymvlzk.sHtML

case "$1" in
来源：http://3g.fanxiaobao.xyz/Article/details/gjxkdcajk.sHtML

start) echo "启动" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghmhigrxv.sHtML

stop)  echo "停止" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gfplwfepn.sHtML

*)     echo "未知命令" ;;
来源：http://3g.fanxiaobao.xyz/Article/details/gnlxnovxm.sHtML

esac
来源：http://wap.fanxiaobao.xyz/Article/details/gfrwekbbo.sHtML

[R12] for 遍历文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gjxceerdv.sHtML

for f in *.txt; do echo "$f"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gilbaxhza.sHtML

[R13] for 计数循环
来源：http://baike.fanxiaobao.xyz/Article/details/gdkpqkprk.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/grbhfzoai.sHtML

[R14] C 风格 for
来源：http://3g.fanxiaobao.xyz/Article/details/gdvkgknwi.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gmagswtuw.sHtML

[R15] while 逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyybttwmv.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdwfaddlu.sHtML

[R16] until 等待条件
来源：http://www.share.fanxiaobao.xyz/Article/details/galzldwho.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/grapuhnsx.sHtML

[R17] 数组定义与取值
来源：http://m.share.fanxiaobao.xyz/Article/details/gbombpswg.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gsmcmlcvk.sHtML

[R18] 遍历数组
来源：http://wap.fanxiaobao.xyz/Article/details/gqyajvtnp.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdbagptpa.sHtML

[R19] 数组长度
来源：http://www.share.fanxiaobao.xyz/Article/details/gesazcoay.sHtML

echo "${#arr[@]}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gvtttinrf.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtigvocmz.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://baike.fanxiaobao.xyz/Article/details/gwytlhjvn.sHtML

[R21] 字符串长度
来源：http://mobile.fanxiaobao.xyz/Article/details/gxreetsdv.sHtML

echo "${#s}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghatxlbsr.sHtML

[R22] 截取子串
来源：http://wap.fanxiaobao.xyz/Article/details/glpecwaad.sHtML

echo "${s:0:5}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gedktvzdo.sHtML

[R23] 字符串替换
来源：http://blog.fanxiaobao.xyz/Article/details/gsgepmnat.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://mobile.fanxiaobao.xyz/Article/details/ghxmblpyf.sHtML

[R24] 大小写转换
来源：http://3g.fanxiaobao.xyz/Article/details/ggwftrolj.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fanxiaobao.xyz/Article/details/gyhakppgh.sHtML

[R25] 去后缀 / 去前缀
来源：http://read.share.fanxiaobao.xyz/Article/details/gwavbkkpo.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gsmphsgls.sHtML

[R26] 命令替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gkwxtzybf.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.fanxiaobao.xyz/Article/details/gczjcjokc.sHtML

[R27] 算术展开
来源：http://baike.fanxiaobao.xyz/Article/details/gakjjzrxj.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fanxiaobao.xyz/Article/details/gpdcpniet.sHtML

[R28] 浮点运算
来源：http://read.share.fanxiaobao.xyz/Article/details/gfhqpfgzi.sHtML

echo "scale=2; 10/3" | bc
来源：http://mobile.fanxiaobao.xyz/Article/details/gaghvxyxz.sHtML

[R29] 定义函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gluwocbqf.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://baike.fanxiaobao.xyz/Article/details/gtuvzwetm.sHtML

[R30] 函数返回状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gtgevrvnn.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fanxiaobao.xyz/Article/details/ggzwfrecm.sHtML

[R31] 局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gznycclmy.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gunjvxvyj.sHtML

[R32] 参数个数校验
来源：http://m.share.fanxiaobao.xyz/Article/details/gdmxujybw.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://baike.fanxiaobao.xyz/Article/details/gwlasmflm.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fanxiaobao.xyz/Article/details/gxkdahiyl.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://3g.fanxiaobao.xyz/Article/details/gtdtfinuj.sHtML

[R34] 退出时清理
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghmhokslz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.fanxiaobao.xyz/Article/details/goezuacjd.sHtML

[R35] 后台执行并等待
来源：http://read.share.fanxiaobao.xyz/Article/details/gxueedtvd.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://m.share.fanxiaobao.xyz/Article/details/glciwnxis.sHtML

[R36] 并发执行多个任务
来源：http://blog.fanxiaobao.xyz/Article/details/gtkpsutil.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.fanxiaobao.xyz/Article/details/gxojaantk.sHtML

[R37] 把输出赋给变量
来源：http://wap.fanxiaobao.xyz/Article/details/gtryfauuz.sHtML

files=$(ls -1)
来源：http://www.share.fanxiaobao.xyz/Article/details/goienelbt.sHtML

[R38] 管道串联
来源：http://wap.fanxiaobao.xyz/Article/details/gqssculcl.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnjrkrofx.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.fanxiaobao.xyz/Article/details/gwszbpwvy.sHtML

cmd > out.log 2>&1
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyamlwulr.sHtML

[R40] 追加写日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gulyimoug.sHtML

echo "log" >> out.log
来源：http://mobile.fanxiaobao.xyz/Article/details/gxbrzkwkd.sHtML

[R41] 丢弃输出
来源：http://blog.fanxiaobao.xyz/Article/details/giihqstxu.sHtML

cmd >/dev/null 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/ghlmzinks.sHtML

[R42] 输入重定向
来源：http://baike.fanxiaobao.xyz/Article/details/gjuyjlifl.sHtML

wc -l < a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvvkxnjak.sHtML

[R43] 按名字查找文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gpofhayqi.sHtML

find . -name "*.log" -type f
来源：http://3g.fanxiaobao.xyz/Article/details/gakfyqelw.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcqestusi.sHtML

find . -mtime -7 -type f
来源：http://wap.fanxiaobao.xyz/Article/details/gljhdacms.sHtML

[R45] 批量删除
来源：http://blog.fanxiaobao.xyz/Article/details/ggcfmthma.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fanxiaobao.xyz/Article/details/gwtanpwrj.sHtML

[R46] 递归替换文件内容
来源：http://wap.fanxiaobao.xyz/Article/details/gzgyhojrl.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzmrsiily.sHtML

[R47] sed 单行替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcoiewrfn.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gzjhmugxy.sHtML

[R48] awk 取指定列
来源：http://mobile.fanxiaobao.xyz/Article/details/grigxxcpf.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gsatglngv.sHtML

[R49] awk 带条件
来源：http://baike.fanxiaobao.xyz/Article/details/gydigsfay.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://3g.fanxiaobao.xyz/Article/details/gefvzosrp.sHtML

[R50] awk 求和
来源：http://wap.fanxiaobao.xyz/Article/details/gpglxdjzk.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.fanxiaobao.xyz/Article/details/gaqqodflj.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtugtplxh.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fanxiaobao.xyz/Article/details/gwrueyiqt.sHtML

[R52] 统计行数
来源：http://wap.fanxiaobao.xyz/Article/details/gsjykozup.sHtML

wc -l a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/grbsiewkl.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fanxiaobao.xyz/Article/details/ghfnfyscm.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdqvpmtrh.sHtML

[R54] 比较两个文件
来源：http://baike.fanxiaobao.xyz/Article/details/gdckbfwmg.sHtML

diff a.txt b.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gqzbterdr.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grwnulwgq.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.fanxiaobao.xyz/Article/details/gmugtchwr.sHtML

[R56] 远程拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/gfpqvcrsi.sHtML

scp file user@host:/path/
来源：http://blog.fanxiaobao.xyz/Article/details/gndqjghte.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbpnulltp.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyasqyoyi.sHtML

[R58] 下载文件
来源：http://blog.fanxiaobao.xyz/Article/details/goyavccjc.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.fanxiaobao.xyz/Article/details/gnzvenalz.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbfmqrgwh.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gcghqajgh.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.fanxiaobao.xyz/Article/details/gulfhstlx.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqxrkyejw.sHtML

[R61] 磁盘占用
来源：http://baike.fanxiaobao.xyz/Article/details/gljjhsvnd.sHtML

df -h;  du -sh *
来源：http://baike.fanxiaobao.xyz/Article/details/gzckuiyhp.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gbjvavpuh.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fanxiaobao.xyz/Article/details/gmkwqykpd.sHtML

[R63] 内存与进程
来源：http://wap.fanxiaobao.xyz/Article/details/gwcdujayq.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fanxiaobao.xyz/Article/details/glsveznzd.sHtML

[R64] 结束进程
来源：http://wap.fanxiaobao.xyz/Article/details/gxusqxeps.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fanxiaobao.xyz/Article/details/gvjyclrgn.sHtML

[R65] 查看端口占用
来源：http://mobile.fanxiaobao.xyz/Article/details/gypgcwflb.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.fanxiaobao.xyz/Article/details/gkkgiuqix.sHtML

[R66] 定时任务
来源：http://3g.fanxiaobao.xyz/Article/details/gifyltutr.sHtML

crontab -e;  crontab -l
来源：http://m.share.fanxiaobao.xyz/Article/details/gfenmuqzt.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fanxiaobao.xyz/Article/details/grvbnxojq.sHtML

openssl rand -hex 16
来源：http://blog.fanxiaobao.xyz/Article/details/gzkidvjzf.sHtML

[R68] 计算文件校验值
来源：http://3g.fanxiaobao.xyz/Article/details/grmuhoiqq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/glatvxzrp.sHtML

[R69] 生成随机密码
来源：http://wap.fanxiaobao.xyz/Article/details/gnnpnuihf.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gstpcspah.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fanxiaobao.xyz/Article/details/gagaupoek.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fanxiaobao.xyz/Article/details/gbxlcjpux.sHtML

[R71] 日期格式化
来源：http://baike.fanxiaobao.xyz/Article/details/gqthsbrwy.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.fanxiaobao.xyz/Article/details/gkqpkcltr.sHtML

[R72] 等待端口就绪
来源：http://m.share.fanxiaobao.xyz/Article/details/gxalczqup.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fanxiaobao.xyz/Article/details/golvsrpfw.sHtML

[R73] 分割大日志
来源：http://3g.fanxiaobao.xyz/Article/details/gjegcpzmd.sHtML

split -l 1000 big.log part_
来源：http://mobile.fanxiaobao.xyz/Article/details/gyypphjop.sHtML

[R74] 批量重命名
来源：http://blog.fanxiaobao.xyz/Article/details/gcljxvdjl.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fanxiaobao.xyz/Article/details/gxnmtywac.sHtML

[R75] 导出环境变量
来源：http://3g.fanxiaobao.xyz/Article/details/gswccjolg.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fanxiaobao.xyz/Article/details/gfdxuhcpm.sHtML

[R76] 使用临时文件
来源：http://wap.fanxiaobao.xyz/Article/details/gqfbwknle.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gbdxkxftc.sHtML

[R77] 读取用户输入
来源：http://mobile.fanxiaobao.xyz/Article/details/gmfxmktrb.sHtML

read -rp "请输入: " ans
来源：http://3g.fanxiaobao.xyz/Article/details/giqotayxy.sHtML

[R78] 交互式菜单
来源：http://3g.fanxiaobao.xyz/Article/details/gaiszozae.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdmzmkmhl.sHtML

[R79] 解析命令行选项
来源：http://m.share.fanxiaobao.xyz/Article/details/ggdubhjhv.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwhisokdx.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.fanxiaobao.xyz/Article/details/grtrlshhs.sHtML

time ./run.sh
来源：http://www.share.fanxiaobao.xyz/Article/details/gfuwdywuo.sHtML

================================================================================
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvxtdulxm.sHtML

S. C / C++ 专题
来源：http://wap.fanxiaobao.xyz/Article/details/ghbhukmgk.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/govtqoobp.sHtML

[S01] C：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gxpviwyhn.sHtML

#include <stdio.h>
来源：http://m.share.fanxiaobao.xyz/Article/details/gvpjwilsf.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfucnzfuq.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gptnrdwsm.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gosjsnabr.sHtML

[S03] C：读入整数
来源：http://www.share.fanxiaobao.xyz/Article/details/ghtmhbcyx.sHtML

int x; scanf("%d", &x);
来源：http://wap.fanxiaobao.xyz/Article/details/gktmwwxfo.sHtML

[S04] C：字符串复制
来源：http://blog.fanxiaobao.xyz/Article/details/grxpbjoex.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fanxiaobao.xyz/Article/details/gfgfwjwoj.sHtML

[S05] C：字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gxydatlpk.sHtML

strlen(s)
来源：http://www.share.fanxiaobao.xyz/Article/details/ggvcgvqpk.sHtML

[S06] C：字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gbczqtqyw.sHtML

strcmp(a, b) == 0
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gejdilrwk.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/getpronwd.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fanxiaobao.xyz/Article/details/gpqcidbry.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxbcnpgsl.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fanxiaobao.xyz/Article/details/gbrrsicnl.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fanxiaobao.xyz/Article/details/gmcvwbtxl.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fanxiaobao.xyz/Article/details/gpwxesruu.sHtML

[S10] C：指针与解引用
来源：http://3g.fanxiaobao.xyz/Article/details/gywkhyprc.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/gnsttyxaa.sHtML

[S11] C：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/ghdepknlh.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.fanxiaobao.xyz/Article/details/grrfdfqdf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmphqkxjy.sHtML

fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/ggwdacheb.sHtML

[S12] C：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwlzgwpyk.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/ghrtdalgg.sHtML

[S13] C：宏定义
来源：http://mobile.fanxiaobao.xyz/Article/details/ghnmxoeyp.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fanxiaobao.xyz/Article/details/glpmlgbnk.sHtML

[S14] C：枚举
来源：http://3g.fanxiaobao.xyz/Article/details/gwrnepuef.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fanxiaobao.xyz/Article/details/gbanrawel.sHtML

[S15] C：类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gevcqvbta.sHtML

(double) a / b
来源：http://m.share.fanxiaobao.xyz/Article/details/gnlnfcxyu.sHtML

[S16] C：位操作置位
来源：http://baike.fanxiaobao.xyz/Article/details/gzoprhltd.sHtML

x |= (1 << 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gehadreqj.sHtML

[S17] C：安全拼接字符串
来源：http://3g.fanxiaobao.xyz/Article/details/gyphphdnd.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvsjjwpxk.sHtML

[S18] C：命令行参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gxtwuouiu.sHtML

int main(int argc, char **argv)
来源：http://blog.fanxiaobao.xyz/Article/details/geuswniwu.sHtML

[S19] C：快速排序
来源：http://wap.fanxiaobao.xyz/Article/details/gvbbhvren.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjeehdlbq.sHtML

[S20] C：二分查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gzvbgddcc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gobjpesal.sHtML

[S21] C：字符类别判断
来源：http://wap.fanxiaobao.xyz/Article/details/gomfvpwhq.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fanxiaobao.xyz/Article/details/gvdstpvul.sHtML

[S22] C：字符串转数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gqfxauwce.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fanxiaobao.xyz/Article/details/gvovawuyx.sHtML

[S23] C：随机数
来源：http://blog.fanxiaobao.xyz/Article/details/gduuttqiz.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fanxiaobao.xyz/Article/details/gdgffcczp.sHtML

[S24] C：获取本地时间
来源：http://read.share.fanxiaobao.xyz/Article/details/gggadscra.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fanxiaobao.xyz/Article/details/gqihctgvw.sHtML

[S25] C：内存拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gggprmdjh.sHtML

memcpy(dst, src, n);
来源：http://www.share.fanxiaobao.xyz/Article/details/gpgwcoxns.sHtML

[S26] C：内存清零
来源：http://blog.fanxiaobao.xyz/Article/details/grilxylcm.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fanxiaobao.xyz/Article/details/gwodciktc.sHtML

[S27] C：定义常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gzhmkwgzc.sHtML

const double PI = 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gerhufsej.sHtML

[S28] C：静态变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gaqiknplf.sHtML

static int counter = 0;
来源：http://www.blog.fanxiaobao.xyz/Article/details/giooruazz.sHtML

[S29] C：变参函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gncjummrg.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fanxiaobao.xyz/Article/details/gtakxvdpx.sHtML

[S30] C：头文件保护
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsjujaphg.sHtML

#ifndef X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gnetohbcr.sHtML

#define X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/ghwwqdywh.sHtML

#endif
来源：http://blog.fanxiaobao.xyz/Article/details/gqfqxjfzu.sHtML

[S31] C++：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/grsrbcrau.sHtML

#include <iostream>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grljnqwog.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gopgwtlvn.sHtML

[S32] C++：字符串
来源：http://mobile.fanxiaobao.xyz/Article/details/guqakyyiz.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.fanxiaobao.xyz/Article/details/gmmtspgvv.sHtML

[S33] C++：vector 增删
来源：http://3g.fanxiaobao.xyz/Article/details/gleqwrdcg.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gcdcwaswc.sHtML

[S34] C++：遍历 vector
来源：http://www.share.fanxiaobao.xyz/Article/details/gqlgsyoax.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxrscqewt.sHtML

[S35] C++：map
来源：http://wap.fanxiaobao.xyz/Article/details/gtmhuappv.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fanxiaobao.xyz/Article/details/gpialnnnr.sHtML

[S36] C++：unordered_map
来源：http://mobile.fanxiaobao.xyz/Article/details/gfuawidwr.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggodzlzog.sHtML

[S37] C++：set
来源：http://3g.fanxiaobao.xyz/Article/details/gklqydxuv.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gwdqwvdfp.sHtML

[S38] C++：排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gxcqxssmr.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/guxktzesq.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fanxiaobao.xyz/Article/details/gxoulxnfr.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fanxiaobao.xyz/Article/details/gntbkgbbw.sHtML

[S40] C++：查找元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gftfmjfuw.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gtgsutdjr.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glftibqdp.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fanxiaobao.xyz/Article/details/grstgicml.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.fanxiaobao.xyz/Article/details/giwshmwum.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbbyhzkqq.sHtML

[S43] C++：智能指针
来源：http://read.share.fanxiaobao.xyz/Article/details/gouropasb.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpvhavpfc.sHtML

[S44] C++：引用传参
来源：http://baike.fanxiaobao.xyz/Article/details/gyiodxxwo.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gybdznauz.sHtML

[S45] C++：lambda
来源：http://www.blog.fanxiaobao.xyz/Article/details/gncalqycw.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gdsqiatth.sHtML

[S46] C++：函数模板
来源：http://wap.fanxiaobao.xyz/Article/details/gfosziyzq.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gquojnjsc.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gfqtggalk.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fanxiaobao.xyz/Article/details/gbhfwcynr.sHtML

[S48] C++：逐行读文件
来源：http://3g.fanxiaobao.xyz/Article/details/gglghckxz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.fanxiaobao.xyz/Article/details/guxadwvlw.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gaqtdhdmg.sHtML

[S49] C++：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/ghruacdgx.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fanxiaobao.xyz/Article/details/gqxzbjfur.sHtML

[S50] C++：格式化数字
来源：http://3g.fanxiaobao.xyz/Article/details/gidqykfhu.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gcwgvjhot.sHtML

[S51] C++：显式类型转换
来源：http://wap.fanxiaobao.xyz/Article/details/ggyhfgmfi.sHtML

static_cast<double>(a) / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gquekvcqi.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.fanxiaobao.xyz/Article/details/gzpohshyb.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gyezftdcc.sHtML

[S53] C++：移动语义
来源：http://mobile.fanxiaobao.xyz/Article/details/gpiosmnft.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fanxiaobao.xyz/Article/details/gvtsresgk.sHtML

[S54] C++：异常处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gbsvtlpbw.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fanxiaobao.xyz/Article/details/gchvrrbav.sHtML

[S55] C++：结构化绑定
来源：http://blog.fanxiaobao.xyz/Article/details/gscritxwf.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/gbwbgtnoe.sHtML

[S56] C++：optional
来源：http://read.share.fanxiaobao.xyz/Article/details/gnbnmonuv.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.fanxiaobao.xyz/Article/details/gngunadwm.sHtML

[S57] C++：编译期常量
来源：http://read.share.fanxiaobao.xyz/Article/details/geryvcvbb.sHtML

constexpr int N = 10;
来源：http://mobile.fanxiaobao.xyz/Article/details/gayggchyz.sHtML

[S58] C++：命名空间
来源：http://read.share.fanxiaobao.xyz/Article/details/gjcgjlswr.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fanxiaobao.xyz/Article/details/gwkhsaozp.sHtML

[S59] C++：静态断言
来源：http://blog.fanxiaobao.xyz/Article/details/gfhojjbal.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.fanxiaobao.xyz/Article/details/gwisvjrls.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fanxiaobao.xyz/Article/details/gfizqvjvn.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/gnpurfakt.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gkzcomjzk.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fanxiaobao.xyz/Article/details/gnyecnkim.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzamjoznp.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gfhcirszi.sHtML

println("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/gfpahjyzy.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbbttzouw.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fanxiaobao.xyz/Article/details/gjzxtgyqc.sHtML


<!-- 参考信息 -->