代发 wailian999

readonly PI=3.14
来源：http://3g.hesvh.cn/Article/details/gmhnluynx.sHtML

[R04] 位置参数
来源：http://baike.fehbvm.com/Article/details/gbpthhtzr.sHtML

echo "$0 $1 $2 | 全部: $@ | 个数: $#"
来源：http://wap.zdbjq.cn/Article/details/gfeizjhzb.sHtML

[R05] 参数默认值
来源：http://read.share.fehbvm.com/Article/details/gspjrykhu.sHtML

name="${1:-default}"
来源：http://www.blog.zdbjq.cn/Article/details/gbnuihalb.sHtML

[R06] 判断命令是否存在
来源：http://baike.hesvh.cn/Article/details/gejlmcydm.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://wap.hesvh.cn/Article/details/gvqlnmcke.sHtML

[R07] if 判断文件
来源：http://blog.zdbjq.cn/Article/details/gwpaimtzu.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.hesvh.cn/Article/details/gbgstjqyr.sHtML

[R08] 数值比较
来源：http://www.blog.fehbvm.com/Article/details/gqqbsfgqc.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://www.share.fehbvm.com/Article/details/guzqitldh.sHtML

[R09] 字符串比较
来源：http://blog.hesvh.cn/Article/details/gufaqmjej.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://blog.hesvh.cn/Article/details/gxfyvepti.sHtML

[R10] 正则匹配
来源：http://baike.hesvh.cn/Article/details/gotioyzuz.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.fehbvm.com/Article/details/gqzvluryl.sHtML

[R11] case 多分支
来源：http://wap.fehbvm.com/Article/details/gbdbfsrms.sHtML

case "$1" in
来源：http://read.share.zdbjq.cn/Article/details/gkkhhaxix.sHtML

start) echo "启动" ;;
来源：http://m.share.zdbjq.cn/Article/details/gklsoczvt.sHtML

stop)  echo "停止" ;;
来源：http://mobile.zdbjq.cn/Article/details/gxaocmors.sHtML

*)     echo "未知命令" ;;
来源：http://wap.zdbjq.cn/Article/details/gwemkcuwb.sHtML

esac
来源：http://www.m.share.fehbvm.com/Article/details/gtecqmzyp.sHtML

[R12] for 遍历文件
来源：http://m.share.zdbjq.cn/Article/details/gvpygsoww.sHtML

for f in *.txt; do echo "$f"; done
来源：http://blog.fehbvm.com/Article/details/glqubzcds.sHtML

[R13] for 计数循环
来源：http://www.blog.zdbjq.cn/Article/details/gnbykpgbs.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.hesvh.cn/Article/details/grurxpnuf.sHtML

[R14] C 风格 for
来源：http://wap.hesvh.cn/Article/details/gndncfich.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.fehbvm.com/Article/details/gccivnsiv.sHtML

[R15] while 逐行读文件
来源：http://baike.hesvh.cn/Article/details/gwirzfweh.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://mobile.fehbvm.com/Article/details/gdnaartha.sHtML

[R16] until 等待条件
来源：http://wap.fehbvm.com/Article/details/grxuqiedq.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://www.m.share.zdbjq.cn/Article/details/gzlugvfmx.sHtML

[R17] 数组定义与取值
来源：http://read.share.fehbvm.com/Article/details/gwkcgvfkh.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://3g.fehbvm.com/Article/details/ggnrvssif.sHtML

[R18] 遍历数组
来源：http://www.m.share.zdbjq.cn/Article/details/gcczyztlo.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.hesvh.cn/Article/details/gjgxvtdal.sHtML

[R19] 数组长度
来源：http://wap.hesvh.cn/Article/details/guhbuowyi.sHtML

echo "${#arr[@]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gfupiptva.sHtML

[R20] 关联数组（字典）
来源：http://blog.fehbvm.com/Article/details/ggdiridvg.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.hesvh.cn/Article/details/gkapxoovf.sHtML

[R21] 字符串长度
来源：http://blog.zdbjq.cn/Article/details/gtlpqexhz.sHtML

echo "${#s}"
来源：http://blog.zdbjq.cn/Article/details/gvmvngzvj.sHtML

[R22] 截取子串
来源：http://www.share.zdbjq.cn/Article/details/gsuveemut.sHtML

echo "${s:0:5}"
来源：http://www.blog.fehbvm.com/Article/details/gaudcxwor.sHtML

[R23] 字符串替换
来源：http://www.m.share.fehbvm.com/Article/details/gcfwlgalv.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.zdbjq.cn/Article/details/gtldeqzvk.sHtML

[R24] 大小写转换
来源：http://mobile.zdbjq.cn/Article/details/gnirxvpse.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://blog.fehbvm.com/Article/details/gvahpusdl.sHtML

[R25] 去后缀 / 去前缀
来源：http://baike.fehbvm.com/Article/details/glldmqolf.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://blog.fehbvm.com/Article/details/gkqrsqdbw.sHtML

[R26] 命令替换
来源：http://www.blog.zdbjq.cn/Article/details/grezpkovx.sHtML

now=$(date +%F); echo "$now"
来源：http://www.m.share.zdbjq.cn/Article/details/gucaqlhrj.sHtML

[R27] 算术展开
来源：http://www.m.share.zdbjq.cn/Article/details/gzgecdvzk.sHtML

echo $((1 + 2 * 3))
来源：http://baike.hesvh.cn/Article/details/gplbipeyw.sHtML

[R28] 浮点运算
来源：http://read.share.fehbvm.com/Article/details/glzkolmxz.sHtML

echo "scale=2; 10/3" | bc
来源：http://baike.zdbjq.cn/Article/details/gqwefshjo.sHtML

[R29] 定义函数
来源：http://m.share.zdbjq.cn/Article/details/gniczfqvw.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.hesvh.cn/Article/details/gxshxigui.sHtML

[R30] 函数返回状态码
来源：http://www.m.share.fehbvm.com/Article/details/gnrfwcard.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://blog.fehbvm.com/Article/details/gxfqpvrpo.sHtML

[R31] 局部变量
来源：http://mobile.hesvh.cn/Article/details/gmfqfqxvk.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.fehbvm.com/Article/details/gjglunter.sHtML

[R32] 参数个数校验
来源：http://3g.fehbvm.com/Article/details/gfhwnnkbr.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.share.hesvh.cn/Article/details/giziebkii.sHtML

[R33] 捕获错误并提示行号
来源：http://read.share.zdbjq.cn/Article/details/gcbutfjrn.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.fehbvm.com/Article/details/gjzfjvdvz.sHtML

[R34] 退出时清理
来源：http://m.share.zdbjq.cn/Article/details/glruqmyiz.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.zdbjq.cn/Article/details/gjcwfhbbq.sHtML

[R35] 后台执行并等待
来源：http://read.share.hesvh.cn/Article/details/gdupodyde.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://wap.zdbjq.cn/Article/details/gghigekif.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fehbvm.com/Article/details/gxqslvuzh.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.share.zdbjq.cn/Article/details/gxunqkskn.sHtML

[R37] 把输出赋给变量
来源：http://m.share.hesvh.cn/Article/details/gtsthchdl.sHtML

files=$(ls -1)
来源：http://m.share.zdbjq.cn/Article/details/gtunatlgk.sHtML

[R38] 管道串联
来源：http://mobile.zdbjq.cn/Article/details/gsyiwnzfx.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.share.fehbvm.com/Article/details/gfhfplddk.sHtML

[R39] 重定向标准输出与错误
来源：http://www.share.zdbjq.cn/Article/details/ggjiganoa.sHtML

cmd > out.log 2>&1
来源：http://read.share.zdbjq.cn/Article/details/gjfwiseai.sHtML

[R40] 追加写日志
来源：http://www.share.fehbvm.com/Article/details/gekhfndqi.sHtML

echo "log" >> out.log
来源：http://read.share.hesvh.cn/Article/details/ghhvsajks.sHtML

[R41] 丢弃输出
来源：http://baike.zdbjq.cn/Article/details/ggpgvsemy.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.hesvh.cn/Article/details/gjhtojrmv.sHtML

[R42] 输入重定向
来源：http://baike.hesvh.cn/Article/details/gxqadimam.sHtML

wc -l < a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gchquigha.sHtML

[R43] 按名字查找文件
来源：http://baike.zdbjq.cn/Article/details/gzvruarkv.sHtML

find . -name "*.log" -type f
来源：http://www.blog.zdbjq.cn/Article/details/gavfzcouu.sHtML

[R44] 按修改时间查找
来源：http://baike.fehbvm.com/Article/details/gwalxbkqm.sHtML

find . -mtime -7 -type f
来源：http://www.share.hesvh.cn/Article/details/gqocezxdh.sHtML

[R45] 批量删除
来源：http://read.share.fehbvm.com/Article/details/gxoocdxrg.sHtML

find . -name "*.tmp" -delete
来源：http://www.m.share.zdbjq.cn/Article/details/gqrwooyll.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.zdbjq.cn/Article/details/gcykrowcb.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.blog.hesvh.cn/Article/details/gwbzcioam.sHtML

[R47] sed 单行替换
来源：http://mobile.fehbvm.com/Article/details/gbzpfnzrt.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fehbvm.com/Article/details/guwslrdpk.sHtML

[R48] awk 取指定列
来源：http://www.share.hesvh.cn/Article/details/gnstakegb.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.zdbjq.cn/Article/details/gkdosryxd.sHtML

[R49] awk 带条件
来源：http://m.share.zdbjq.cn/Article/details/gqxzjoeoi.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.blog.fehbvm.com/Article/details/gikgautko.sHtML

[R50] awk 求和
来源：http://www.blog.fehbvm.com/Article/details/gtyiuocmz.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://wap.hesvh.cn/Article/details/gtlymjqks.sHtML

[R51] 排序去重取前几
来源：http://mobile.zdbjq.cn/Article/details/gztprztpk.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.share.zdbjq.cn/Article/details/gvanocsom.sHtML

[R52] 统计行数
来源：http://www.blog.fehbvm.com/Article/details/gizgffcny.sHtML

wc -l a.txt
来源：http://blog.zdbjq.cn/Article/details/gkasfviph.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.fehbvm.com/Article/details/gwjbakxjr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.fehbvm.com/Article/details/gmoufboek.sHtML

[R54] 比较两个文件
来源：http://mobile.fehbvm.com/Article/details/gajzncyxw.sHtML

diff a.txt b.txt
来源：http://3g.fehbvm.com/Article/details/gxoyrxkyl.sHtML

[R55] 压缩与解压
来源：http://www.blog.fehbvm.com/Article/details/gfmpjvwkm.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fehbvm.com/Article/details/gzhmtlgrr.sHtML

[R56] 远程拷贝
来源：http://read.share.zdbjq.cn/Article/details/gxcqjdlhr.sHtML

scp file user@host:/path/
来源：http://baike.fehbvm.com/Article/details/gifgobfcp.sHtML

[R57] 远程执行命令
来源：http://3g.zdbjq.cn/Article/details/gtoctqvlx.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.zdbjq.cn/Article/details/gnptvknra.sHtML

[R58] 下载文件
来源：http://www.m.share.hesvh.cn/Article/details/gcfbcepvn.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.hesvh.cn/Article/details/gsofyqybb.sHtML

[R59] 发 POST JSON
来源：http://www.share.fehbvm.com/Article/details/ghetnylfn.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fehbvm.com/Article/details/gofdmmctf.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.zdbjq.cn/Article/details/gsvbiystj.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.hesvh.cn/Article/details/gdpkcfqvb.sHtML

[R61] 磁盘占用
来源：http://read.share.zdbjq.cn/Article/details/gycsdmems.sHtML

df -h;  du -sh *
来源：http://www.blog.zdbjq.cn/Article/details/gocdhflsa.sHtML

[R62] 找最占空间的文件
来源：http://read.share.hesvh.cn/Article/details/gudsaoofw.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.hesvh.cn/Article/details/gwuhwlygx.sHtML

[R63] 内存与进程
来源：http://3g.hesvh.cn/Article/details/grytantcx.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fehbvm.com/Article/details/gvztrlbca.sHtML

[R64] 结束进程
来源：http://mobile.fehbvm.com/Article/details/gdhldkxwm.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.zdbjq.cn/Article/details/gcxeohdsb.sHtML

[R65] 查看端口占用
来源：http://m.share.fehbvm.com/Article/details/gygdcxqxj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.zdbjq.cn/Article/details/gzlbppxbh.sHtML

[R66] 定时任务
来源：http://www.blog.fehbvm.com/Article/details/grawdoqbp.sHtML

crontab -e;  crontab -l
来源：http://wap.zdbjq.cn/Article/details/guxvnaofd.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.hesvh.cn/Article/details/gebvilxtf.sHtML

openssl rand -hex 16
来源：http://www.m.share.hesvh.cn/Article/details/grvmbargb.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.zdbjq.cn/Article/details/gwkuxafpq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.hesvh.cn/Article/details/gbbkkvybr.sHtML

[R69] 生成随机密码
来源：http://mobile.zdbjq.cn/Article/details/gswjprvlm.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.zdbjq.cn/Article/details/gighqqfca.sHtML

[R70] 时间戳与互转
来源：http://3g.zdbjq.cn/Article/details/gvnlqbmhn.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.zdbjq.cn/Article/details/gtugzkees.sHtML

[R71] 日期格式化
来源：http://wap.fehbvm.com/Article/details/garewbwkt.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.zdbjq.cn/Article/details/gctlrmyaf.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fehbvm.com/Article/details/gnpstpbzl.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.zdbjq.cn/Article/details/gfvzobtgb.sHtML

[R73] 分割大日志
来源：http://blog.fehbvm.com/Article/details/gnnirvxfa.sHtML

split -l 1000 big.log part_
来源：http://baike.zdbjq.cn/Article/details/gubmqsmwg.sHtML

[R74] 批量重命名
来源：http://m.share.hesvh.cn/Article/details/gkwnpasbc.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.hesvh.cn/Article/details/glajnqgnz.sHtML

[R75] 导出环境变量
来源：http://blog.hesvh.cn/Article/details/gxqzlcabp.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fehbvm.com/Article/details/gadbnyenj.sHtML

[R76] 使用临时文件
来源：http://www.m.share.hesvh.cn/Article/details/googicepl.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/ghgovhchy.sHtML

[R77] 读取用户输入
来源：http://www.share.hesvh.cn/Article/details/gbbyjxwmt.sHtML

read -rp "请输入: " ans
来源：http://3g.hesvh.cn/Article/details/grfcxmsnc.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fehbvm.com/Article/details/gddivsaqh.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.hesvh.cn/Article/details/gozotnqoy.sHtML

[R79] 解析命令行选项
来源：http://www.blog.fehbvm.com/Article/details/gzsklejei.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fehbvm.com/Article/details/glvxqmjoc.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.hesvh.cn/Article/details/gjpqduerw.sHtML

time ./run.sh
来源：http://read.share.zdbjq.cn/Article/details/ggnjtilgc.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gecmrwsgk.sHtML

S. C / C++ 专题
来源：http://mobile.hesvh.cn/Article/details/gfitwdiou.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ghsofbmuc.sHtML

[S01] C：Hello World
来源：http://mobile.hesvh.cn/Article/details/gbsyhgpoa.sHtML

#include <stdio.h>
来源：http://baike.zdbjq.cn/Article/details/grfdigmqr.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.fehbvm.com/Article/details/ghhtefggj.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.hesvh.cn/Article/details/gosohaalq.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.zdbjq.cn/Article/details/gelwbnxln.sHtML

[S03] C：读入整数
来源：http://wap.fehbvm.com/Article/details/gwulwteqt.sHtML

int x; scanf("%d", &x);
来源：http://mobile.hesvh.cn/Article/details/gpmiawvpv.sHtML

[S04] C：字符串复制
来源：http://3g.zdbjq.cn/Article/details/gvgzuzdcl.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.zdbjq.cn/Article/details/gsophmtku.sHtML

[S05] C：字符串长度
来源：http://read.share.fehbvm.com/Article/details/gozczumtq.sHtML

strlen(s)
来源：http://m.share.zdbjq.cn/Article/details/gmubzlflm.sHtML

[S06] C：字符串比较
来源：http://baike.hesvh.cn/Article/details/gpuzbmhpu.sHtML

strcmp(a, b) == 0
来源：http://m.share.hesvh.cn/Article/details/gdzycpmmk.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fehbvm.com/Article/details/grezuuzzc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.zdbjq.cn/Article/details/gwuutiyvq.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fehbvm.com/Article/details/gnhosffrt.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.zdbjq.cn/Article/details/glfjbkenf.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.zdbjq.cn/Article/details/gqrgdzcfw.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.zdbjq.cn/Article/details/gthyjwptb.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fehbvm.com/Article/details/gjbsvyweu.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.zdbjq.cn/Article/details/gkvyjnudl.sHtML

[S11] C：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/gpvtawbmk.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.fehbvm.com/Article/details/gikhlwjym.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.zdbjq.cn/Article/details/gercaaeio.sHtML

fclose(f);
来源：http://mobile.zdbjq.cn/Article/details/ghvwqngng.sHtML

[S12] C：写文件
来源：http://baike.zdbjq.cn/Article/details/gkxavadcf.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.zdbjq.cn/Article/details/gzzbphpnw.sHtML

[S13] C：宏定义
来源：http://read.share.fehbvm.com/Article/details/gjywiyrcc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.hesvh.cn/Article/details/gymakcahe.sHtML

[S14] C：枚举
来源：http://www.share.fehbvm.com/Article/details/gezxyzbug.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fehbvm.com/Article/details/goiqmpojx.sHtML

[S15] C：类型转换
来源：http://www.m.share.hesvh.cn/Article/details/galgfknga.sHtML

(double) a / b
来源：http://baike.hesvh.cn/Article/details/ghdkcgifx.sHtML

[S16] C：位操作置位
来源：http://wap.hesvh.cn/Article/details/gzunifqzi.sHtML

x |= (1 << 3);
来源：http://3g.fehbvm.com/Article/details/gflejhsgg.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fehbvm.com/Article/details/gvfgosipi.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.hesvh.cn/Article/details/ghnaxenub.sHtML

[S18] C：命令行参数
来源：http://3g.hesvh.cn/Article/details/gujxxxtxn.sHtML

int main(int argc, char **argv)
来源：http://m.share.hesvh.cn/Article/details/gwqlpwnsn.sHtML

[S19] C：快速排序
来源：http://m.share.fehbvm.com/Article/details/gdaauxkqs.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.zdbjq.cn/Article/details/gdoogovui.sHtML

[S20] C：二分查找
来源：http://mobile.fehbvm.com/Article/details/gynfummay.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.zdbjq.cn/Article/details/gncocximl.sHtML

[S21] C：字符类别判断
来源：http://3g.zdbjq.cn/Article/details/gqhwqmjto.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.hesvh.cn/Article/details/giqncukbl.sHtML

[S22] C：字符串转数字
来源：http://read.share.zdbjq.cn/Article/details/gicmrmsre.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.hesvh.cn/Article/details/gqtzkmjxe.sHtML

[S23] C：随机数
来源：http://baike.hesvh.cn/Article/details/gpceoaoey.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.hesvh.cn/Article/details/ggbyeimxh.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.hesvh.cn/Article/details/gacvlmdzt.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.hesvh.cn/Article/details/gmppiwnhh.sHtML

[S25] C：内存拷贝
来源：http://www.blog.zdbjq.cn/Article/details/ghnbqcnzn.sHtML

memcpy(dst, src, n);
来源：http://www.share.fehbvm.com/Article/details/govhtwoxc.sHtML

[S26] C：内存清零
来源：http://3g.zdbjq.cn/Article/details/gionywhgk.sHtML

memset(a, 0, sizeof a);
来源：http://read.share.zdbjq.cn/Article/details/gmovptdja.sHtML

[S27] C：定义常量
来源：http://blog.zdbjq.cn/Article/details/grlzphvue.sHtML

const double PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/grbrtjmgr.sHtML

[S28] C：静态变量
来源：http://wap.fehbvm.com/Article/details/grdwducae.sHtML

static int counter = 0;
来源：http://3g.hesvh.cn/Article/details/gsiexhtuo.sHtML

[S29] C：变参函数
来源：http://www.share.hesvh.cn/Article/details/gkknksgey.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://m.share.hesvh.cn/Article/details/giwfzyvax.sHtML

[S30] C：头文件保护
来源：http://mobile.fehbvm.com/Article/details/gxsuvsguy.sHtML

#ifndef X_H
来源：http://www.blog.zdbjq.cn/Article/details/gmxgpisrb.sHtML

#define X_H
来源：http://m.share.zdbjq.cn/Article/details/gipvgpoes.sHtML

#endif
来源：http://www.m.share.hesvh.cn/Article/details/gzqxzfxuo.sHtML

[S31] C++：Hello World
来源：http://wap.fehbvm.com/Article/details/gysiixlgo.sHtML

#include <iostream>
来源：http://www.blog.zdbjq.cn/Article/details/gsyysfvls.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.zdbjq.cn/Article/details/gvthtilao.sHtML

[S32] C++：字符串
来源：http://blog.fehbvm.com/Article/details/gcmpnwpwb.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fehbvm.com/Article/details/ggwjisjzs.sHtML

[S33] C++：vector 增删
来源：http://baike.zdbjq.cn/Article/details/gkxcdpumv.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.hesvh.cn/Article/details/ggfiqzgzz.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fehbvm.com/Article/details/gxpnifptu.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.hesvh.cn/Article/details/ghqfethqy.sHtML

[S35] C++：map
来源：http://blog.zdbjq.cn/Article/details/gkjmkmfaa.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gaynzrjsa.sHtML

[S36] C++：unordered_map
来源：http://www.blog.hesvh.cn/Article/details/gvyjarnyp.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/gkhyvcuar.sHtML

[S37] C++：set
来源：http://www.share.fehbvm.com/Article/details/gnrfxrdes.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fehbvm.com/Article/details/gmveokxuq.sHtML

[S38] C++：排序
来源：http://mobile.fehbvm.com/Article/details/gllrkxafc.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.hesvh.cn/Article/details/gklehcyfr.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fehbvm.com/Article/details/ghwkqzwib.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fehbvm.com/Article/details/geunaibqp.sHtML

[S40] C++：查找元素
来源：http://3g.hesvh.cn/Article/details/gfxqojecw.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.zdbjq.cn/Article/details/gpubxrowv.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.fehbvm.com/Article/details/gpspxsajs.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fehbvm.com/Article/details/grqkksacv.sHtML

[S42] C++：继承与虚函数
来源：http://3g.hesvh.cn/Article/details/gmvuhnuns.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fehbvm.com/Article/details/gukcnlavh.sHtML

[S43] C++：智能指针
来源：http://blog.zdbjq.cn/Article/details/gnqgluvaa.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.zdbjq.cn/Article/details/gigfpllvy.sHtML

[S44] C++：引用传参
来源：http://www.blog.fehbvm.com/Article/details/gbhxjtyiv.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gfbagsbrr.sHtML

[S45] C++：lambda
来源：http://www.share.zdbjq.cn/Article/details/gdqprayru.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fehbvm.com/Article/details/gmxynbsmb.sHtML

[S46] C++：函数模板
来源：http://www.m.share.fehbvm.com/Article/details/gvqyfuobt.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.zdbjq.cn/Article/details/gvousiblt.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.hesvh.cn/Article/details/goegcrcgm.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.hesvh.cn/Article/details/gfyesdrgj.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.zdbjq.cn/Article/details/glbxutueu.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.zdbjq.cn/Article/details/gfsugtmfs.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.hesvh.cn/Article/details/gztxxqkee.sHtML

[S49] C++：写文件
来源：http://wap.zdbjq.cn/Article/details/gfzikqdfu.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.hesvh.cn/Article/details/gpeqjapil.sHtML

[S50] C++：格式化数字
来源：http://3g.zdbjq.cn/Article/details/ghgrytxoh.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fehbvm.com/Article/details/ggwiwdbsc.sHtML

[S51] C++：显式类型转换
来源：http://baike.zdbjq.cn/Article/details/gbgrazrrs.sHtML

static_cast<double>(a) / b
来源：http://read.share.hesvh.cn/Article/details/gyiwetpmp.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.fehbvm.com/Article/details/gxoxjlfgd.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.hesvh.cn/Article/details/gvdgfprsb.sHtML

[S53] C++：移动语义
来源：http://baike.zdbjq.cn/Article/details/gueqdsoap.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fehbvm.com/Article/details/gyhcftdwz.sHtML

[S54] C++：异常处理
来源：http://blog.hesvh.cn/Article/details/gcbpdcpbl.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fehbvm.com/Article/details/gohaqoghy.sHtML

[S55] C++：结构化绑定
来源：http://m.share.hesvh.cn/Article/details/gmyyubcey.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.hesvh.cn/Article/details/glbgfwstd.sHtML

[S56] C++：optional
来源：http://baike.hesvh.cn/Article/details/gspuhgurj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.zdbjq.cn/Article/details/gczidfmje.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.zdbjq.cn/Article/details/gbtxkajam.sHtML

constexpr int N = 10;
来源：http://baike.hesvh.cn/Article/details/goowypgzn.sHtML

[S58] C++：命名空间
来源：http://wap.fehbvm.com/Article/details/gpfhcrqnm.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.zdbjq.cn/Article/details/gxxcpzncm.sHtML

[S59] C++：静态断言
来源：http://read.share.fehbvm.com/Article/details/gasvppfid.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fehbvm.com/Article/details/gbakrdcca.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.zdbjq.cn/Article/details/gyxarfuns.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.zdbjq.cn/Article/details/gdfdttthj.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ggfjgbfdx.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.hesvh.cn/Article/details/glhgzcket.sHtML

================================================================================
来源：http://m.share.fehbvm.com/Article/details/ghikxghxb.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fehbvm.com/Article/details/gkwkfctyh.sHtML

println("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/ghfvjhrzh.sHtML

[T02] Kotlin：变量
来源：http://wap.hesvh.cn/Article/details/gqstezyms.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.zdbjq.cn/Article/details/gciwykbfy.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.hesvh.cn/Article/details/gpfquxtki.sHtML

"值: $b"
来源：http://mobile.fehbvm.com/Article/details/glkifyncn.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fehbvm.com/Article/details/gadlqiidd.sHtML

val n: String? = null;  n?.length
来源：http://m.share.hesvh.cn/Article/details/gogtrbdko.sHtML


<!-- 参考信息 -->