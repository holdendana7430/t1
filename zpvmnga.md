代发 wailian999

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.fanxiaobao.xyz/Article/details/gdszrxcqj.sHtML

[R10] 正则匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gdbybdmpy.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://www.blog.fanxiaobao.xyz/Article/details/gttejmivi.sHtML

[R11] case 多分支
来源：http://mobile.fanxiaobao.xyz/Article/details/gpaucwcfy.sHtML

case "$1" in
来源：http://mobile.fanxiaobao.xyz/Article/details/gsixrynck.sHtML

start) echo "启动" ;;
来源：http://www.share.fanxiaobao.xyz/Article/details/gmwvfbayo.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goxnogibl.sHtML

*)     echo "未知命令" ;;
来源：http://wap.fanxiaobao.xyz/Article/details/gsvhegkuw.sHtML

esac
来源：http://read.share.fanxiaobao.xyz/Article/details/gjejvqqll.sHtML

[R12] for 遍历文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdrnnupwz.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gigvlvhea.sHtML

[R13] for 计数循环
来源：http://3g.fanxiaobao.xyz/Article/details/grygarbjg.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://blog.fanxiaobao.xyz/Article/details/gxtdazwpa.sHtML

[R14] C 风格 for
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gooexsarn.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gflysdqdl.sHtML

[R15] while 逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/giyomtvfu.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.fanxiaobao.xyz/Article/details/gfgovtkda.sHtML

[R16] until 等待条件
来源：http://mobile.fanxiaobao.xyz/Article/details/gklcvtvcs.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gfkhqkebc.sHtML

[R17] 数组定义与取值
来源：http://wap.fanxiaobao.xyz/Article/details/gppzdeift.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.fanxiaobao.xyz/Article/details/gljpzuekn.sHtML

[R18] 遍历数组
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqbrvbpzc.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkvjtlfkr.sHtML

[R19] 数组长度
来源：http://3g.fanxiaobao.xyz/Article/details/gwekrkfnp.sHtML

echo "${#arr[@]}"
来源：http://3g.fanxiaobao.xyz/Article/details/gkyozrgox.sHtML

[R20] 关联数组（字典）
来源：http://baike.fanxiaobao.xyz/Article/details/gjlpvylmn.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://m.share.fanxiaobao.xyz/Article/details/gpfgjompv.sHtML

[R21] 字符串长度
来源：http://blog.fanxiaobao.xyz/Article/details/gpgwwzndw.sHtML

echo "${#s}"
来源：http://mobile.fanxiaobao.xyz/Article/details/gdvjzcsaq.sHtML

[R22] 截取子串
来源：http://baike.fanxiaobao.xyz/Article/details/gqutozqse.sHtML

echo "${s:0:5}"
来源：http://blog.fanxiaobao.xyz/Article/details/gwduvdpiq.sHtML

[R23] 字符串替换
来源：http://mobile.fanxiaobao.xyz/Article/details/glejywpiu.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://www.share.fanxiaobao.xyz/Article/details/gwoikdzpa.sHtML

[R24] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gfmtnsqvl.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtbrkirpv.sHtML

[R25] 去后缀 / 去前缀
来源：http://m.share.fanxiaobao.xyz/Article/details/gotmzbufn.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fanxiaobao.xyz/Article/details/gnzqfbnhk.sHtML

[R26] 命令替换
来源：http://blog.fanxiaobao.xyz/Article/details/grkxhqlbu.sHtML

now=$(date +%F); echo "$now"
来源：http://www.share.fanxiaobao.xyz/Article/details/gebjedrpm.sHtML

[R27] 算术展开
来源：http://blog.fanxiaobao.xyz/Article/details/guktmsuec.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fanxiaobao.xyz/Article/details/gjpszjfbl.sHtML

[R28] 浮点运算
来源：http://www.blog.fanxiaobao.xyz/Article/details/glpwzdtnm.sHtML

echo "scale=2; 10/3" | bc
来源：http://m.share.fanxiaobao.xyz/Article/details/gxbikrigq.sHtML

[R29] 定义函数
来源：http://www.share.fanxiaobao.xyz/Article/details/genzgocrs.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gmtqmcuem.sHtML

[R30] 函数返回状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gtlukidxq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fanxiaobao.xyz/Article/details/gefblefiu.sHtML

[R31] 局部变量
来源：http://wap.fanxiaobao.xyz/Article/details/geffvewfi.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gufkpywje.sHtML

[R32] 参数个数校验
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdgohmfky.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.fanxiaobao.xyz/Article/details/gzojzzryz.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.fanxiaobao.xyz/Article/details/gpuknoylq.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.fanxiaobao.xyz/Article/details/gfexhafgv.sHtML

[R34] 退出时清理
来源：http://mobile.fanxiaobao.xyz/Article/details/gioasolrn.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfwbxhyam.sHtML

[R35] 后台执行并等待
来源：http://www.share.fanxiaobao.xyz/Article/details/gbvnzqmoi.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fanxiaobao.xyz/Article/details/gchvwxgzq.sHtML

[R36] 并发执行多个任务
来源：http://3g.fanxiaobao.xyz/Article/details/gpymuhhqy.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyemjoqni.sHtML

[R37] 把输出赋给变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gapdepfzk.sHtML

files=$(ls -1)
来源：http://3g.fanxiaobao.xyz/Article/details/gwuivthje.sHtML

[R38] 管道串联
来源：http://wap.fanxiaobao.xyz/Article/details/gdwhosazf.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gnvczhzie.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.fanxiaobao.xyz/Article/details/gtdiibmkf.sHtML

cmd > out.log 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gghbrpoyf.sHtML

[R40] 追加写日志
来源：http://baike.fanxiaobao.xyz/Article/details/gjfqnlhvt.sHtML

echo "log" >> out.log
来源：http://3g.fanxiaobao.xyz/Article/details/gfkipcqar.sHtML

[R41] 丢弃输出
来源：http://www.share.fanxiaobao.xyz/Article/details/gsqhzmpef.sHtML

cmd >/dev/null 2>&1
来源：http://3g.fanxiaobao.xyz/Article/details/gcvfvrqqb.sHtML

[R42] 输入重定向
来源：http://m.share.fanxiaobao.xyz/Article/details/gspllwwfp.sHtML

wc -l < a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcsiulcii.sHtML

[R43] 按名字查找文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gwroihgyr.sHtML

find . -name "*.log" -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gevhaprmr.sHtML

[R44] 按修改时间查找
来源：http://3g.fanxiaobao.xyz/Article/details/gvtwqwchy.sHtML

find . -mtime -7 -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/gjchevdav.sHtML

[R45] 批量删除
来源：http://read.share.fanxiaobao.xyz/Article/details/ghmcjfofb.sHtML

find . -name "*.tmp" -delete
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxwmkexva.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.fanxiaobao.xyz/Article/details/gebomwytg.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://m.share.fanxiaobao.xyz/Article/details/gyipwudcn.sHtML

[R47] sed 单行替换
来源：http://m.share.fanxiaobao.xyz/Article/details/gfioiyyup.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gdmnpxzkm.sHtML

[R48] awk 取指定列
来源：http://m.share.fanxiaobao.xyz/Article/details/goddfyqpv.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gfgmkwkbi.sHtML

[R49] awk 带条件
来源：http://wap.fanxiaobao.xyz/Article/details/gtceydull.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fanxiaobao.xyz/Article/details/gvcunxtsa.sHtML

[R50] awk 求和
来源：http://www.share.fanxiaobao.xyz/Article/details/gmgmutzcb.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gsbdlupxx.sHtML

[R51] 排序去重取前几
来源：http://mobile.fanxiaobao.xyz/Article/details/gmahcrxtx.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fanxiaobao.xyz/Article/details/gnmolhitq.sHtML

[R52] 统计行数
来源：http://baike.fanxiaobao.xyz/Article/details/ghrhecjmo.sHtML

wc -l a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/grtrsbltl.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.fanxiaobao.xyz/Article/details/gobtdaeqt.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.fanxiaobao.xyz/Article/details/gnwgsevfl.sHtML

[R54] 比较两个文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjfgtvgdg.sHtML

diff a.txt b.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/givkstool.sHtML

[R55] 压缩与解压
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzshdlbeu.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvodzjigq.sHtML

[R56] 远程拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/gnphhpgev.sHtML

scp file user@host:/path/
来源：http://m.share.fanxiaobao.xyz/Article/details/gpozmziks.sHtML

[R57] 远程执行命令
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbeebmhid.sHtML

ssh user@host 'uptime'
来源：http://www.share.fanxiaobao.xyz/Article/details/gctuxilew.sHtML

[R58] 下载文件
来源：http://3g.fanxiaobao.xyz/Article/details/gzrbwonsa.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gieccmddy.sHtML

[R59] 发 POST JSON
来源：http://3g.fanxiaobao.xyz/Article/details/gsioaepdn.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fanxiaobao.xyz/Article/details/glhqsrbie.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gndzcfjqq.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gckqsswlv.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwtlzikqb.sHtML

df -h;  du -sh *
来源：http://blog.fanxiaobao.xyz/Article/details/gjtsrqyba.sHtML

[R62] 找最占空间的文件
来源：http://baike.fanxiaobao.xyz/Article/details/gkysacvms.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fanxiaobao.xyz/Article/details/gjelnjsyo.sHtML

[R63] 内存与进程
来源：http://baike.fanxiaobao.xyz/Article/details/gbufewovh.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fanxiaobao.xyz/Article/details/gwdukfotr.sHtML

[R64] 结束进程
来源：http://baike.fanxiaobao.xyz/Article/details/gvpkcyxtw.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.fanxiaobao.xyz/Article/details/goaycdgjy.sHtML

[R65] 查看端口占用
来源：http://read.share.fanxiaobao.xyz/Article/details/gwipvpcaw.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fanxiaobao.xyz/Article/details/gxivtihap.sHtML

[R66] 定时任务
来源：http://3g.fanxiaobao.xyz/Article/details/grvmgfske.sHtML

crontab -e;  crontab -l
来源：http://wap.fanxiaobao.xyz/Article/details/gavjeahaa.sHtML

[R67] 生成随机十六进制串
来源：http://3g.fanxiaobao.xyz/Article/details/gbyddanwh.sHtML

openssl rand -hex 16
来源：http://www.blog.fanxiaobao.xyz/Article/details/gszrgbjvj.sHtML

[R68] 计算文件校验值
来源：http://mobile.fanxiaobao.xyz/Article/details/gqnwmviru.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fanxiaobao.xyz/Article/details/gzopahngd.sHtML

[R69] 生成随机密码
来源：http://mobile.fanxiaobao.xyz/Article/details/glrztmoxg.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fanxiaobao.xyz/Article/details/gngqovzzy.sHtML

[R70] 时间戳与互转
来源：http://m.share.fanxiaobao.xyz/Article/details/gbwfbfcll.sHtML

date +%s;  date -d @1700000000
来源：http://baike.fanxiaobao.xyz/Article/details/gfynwgzwy.sHtML

[R71] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gsgouxcli.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.fanxiaobao.xyz/Article/details/gynbiibog.sHtML

[R72] 等待端口就绪
来源：http://read.share.fanxiaobao.xyz/Article/details/gdkqdcpbc.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gvjuehoje.sHtML

[R73] 分割大日志
来源：http://baike.fanxiaobao.xyz/Article/details/gpdyhyrig.sHtML

split -l 1000 big.log part_
来源：http://mobile.fanxiaobao.xyz/Article/details/gyleeglmf.sHtML

[R74] 批量重命名
来源：http://m.share.fanxiaobao.xyz/Article/details/gfpmchspl.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fanxiaobao.xyz/Article/details/gtfajxwmo.sHtML

[R75] 导出环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gfnxsekje.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fanxiaobao.xyz/Article/details/girfsxxyq.sHtML

[R76] 使用临时文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/guvddkluh.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghwfvghpi.sHtML

[R77] 读取用户输入
来源：http://m.share.fanxiaobao.xyz/Article/details/gvgdqljlg.sHtML

read -rp "请输入: " ans
来源：http://wap.fanxiaobao.xyz/Article/details/ggqhltagz.sHtML

[R78] 交互式菜单
来源：http://m.share.fanxiaobao.xyz/Article/details/gbgogmlhy.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fanxiaobao.xyz/Article/details/gawyktlyb.sHtML

[R79] 解析命令行选项
来源：http://read.share.fanxiaobao.xyz/Article/details/gbkuelqjs.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghfqgoogh.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fanxiaobao.xyz/Article/details/gsesdacza.sHtML

time ./run.sh
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfkquwpei.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gsvictfuy.sHtML

S. C / C++ 专题
来源：http://mobile.fanxiaobao.xyz/Article/details/gdfqflkjj.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gycnetjrg.sHtML

[S01] C：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gqsgrdzsp.sHtML

#include <stdio.h>
来源：http://read.share.fanxiaobao.xyz/Article/details/gjsdsnkkw.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gxbhgohmc.sHtML

[S02] C：变量与格式化输出
来源：http://blog.fanxiaobao.xyz/Article/details/godvojmss.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fanxiaobao.xyz/Article/details/glqrwumdp.sHtML

[S03] C：读入整数
来源：http://m.share.fanxiaobao.xyz/Article/details/gcpsqhneh.sHtML

int x; scanf("%d", &x);
来源：http://3g.fanxiaobao.xyz/Article/details/gehkfbyau.sHtML

[S04] C：字符串复制
来源：http://mobile.fanxiaobao.xyz/Article/details/glxqdvufu.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gstuqkdnp.sHtML

[S05] C：字符串长度
来源：http://www.blog.fanxiaobao.xyz/Article/details/gocpmrniq.sHtML

strlen(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxvlrkepe.sHtML

[S06] C：字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/graoppjqp.sHtML

strcmp(a, b) == 0
来源：http://read.share.fanxiaobao.xyz/Article/details/ghfgjnbey.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gdpjwkpkb.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fanxiaobao.xyz/Article/details/gwlabtutj.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fanxiaobao.xyz/Article/details/gzrkujjlu.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fanxiaobao.xyz/Article/details/gggrczjhz.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqdzpliyj.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fanxiaobao.xyz/Article/details/grccknbye.sHtML

[S10] C：指针与解引用
来源：http://m.share.fanxiaobao.xyz/Article/details/gtgnaqfbg.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fanxiaobao.xyz/Article/details/gvlpdndaf.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnksvmnsn.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fanxiaobao.xyz/Article/details/gkgxjzbao.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/glluhvovt.sHtML

fclose(f);
来源：http://blog.fanxiaobao.xyz/Article/details/gzohqnocd.sHtML

[S12] C：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/gzqgewxpw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gurjhixkt.sHtML

[S13] C：宏定义
来源：http://3g.fanxiaobao.xyz/Article/details/gkpzqocym.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtcrnrkgs.sHtML

[S14] C：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gftzzgpvx.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fanxiaobao.xyz/Article/details/gnoxkhxek.sHtML

[S15] C：类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gyvwjbbvq.sHtML

(double) a / b
来源：http://m.share.fanxiaobao.xyz/Article/details/gezgqkfqg.sHtML

[S16] C：位操作置位
来源：http://www.blog.fanxiaobao.xyz/Article/details/giisfqump.sHtML

x |= (1 << 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gshrtzyat.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gaxtjnoqi.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.fanxiaobao.xyz/Article/details/gphfgazcx.sHtML

[S18] C：命令行参数
来源：http://mobile.fanxiaobao.xyz/Article/details/ghnitnvkt.sHtML

int main(int argc, char **argv)
来源：http://read.share.fanxiaobao.xyz/Article/details/gaaqokrxd.sHtML

[S19] C：快速排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjdylcsri.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gdecsdyfw.sHtML

[S20] C：二分查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gznoomfse.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gvsqozcrv.sHtML

[S21] C：字符类别判断
来源：http://wap.fanxiaobao.xyz/Article/details/gawixjmxj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fanxiaobao.xyz/Article/details/ghdkpsrsy.sHtML

[S22] C：字符串转数字
来源：http://baike.fanxiaobao.xyz/Article/details/ggcybikfm.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbuyhluwb.sHtML

[S23] C：随机数
来源：http://m.share.fanxiaobao.xyz/Article/details/gjgwsnmfn.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fanxiaobao.xyz/Article/details/gcelzxnuz.sHtML

[S24] C：获取本地时间
来源：http://blog.fanxiaobao.xyz/Article/details/gvgcgvtpt.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fanxiaobao.xyz/Article/details/gminswitr.sHtML

[S25] C：内存拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/gsdkcrypb.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fanxiaobao.xyz/Article/details/guedeglay.sHtML

[S26] C：内存清零
来源：http://m.share.fanxiaobao.xyz/Article/details/gohnkwdxb.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fanxiaobao.xyz/Article/details/grnnbuykp.sHtML

[S27] C：定义常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqnzcpavd.sHtML

const double PI = 3.14159;
来源：http://www.share.fanxiaobao.xyz/Article/details/gzlryrbkk.sHtML

[S28] C：静态变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gsxyxvlrf.sHtML

static int counter = 0;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxoqsqrsl.sHtML

[S29] C：变参函数
来源：http://read.share.fanxiaobao.xyz/Article/details/giakizjtv.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcjagpjls.sHtML

[S30] C：头文件保护
来源：http://wap.fanxiaobao.xyz/Article/details/gglmvlvlf.sHtML

#ifndef X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gyoikgavd.sHtML

#define X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gggagrbab.sHtML

#endif
来源：http://m.share.fanxiaobao.xyz/Article/details/gfrkpdtzj.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkswspabr.sHtML

#include <iostream>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwimvfpsn.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ggjzljzaq.sHtML

[S32] C++：字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/guourhlaf.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fanxiaobao.xyz/Article/details/gcdxstxht.sHtML

[S33] C++：vector 增删
来源：http://baike.fanxiaobao.xyz/Article/details/gtsobbasq.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gffwccyws.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyhtxdwen.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gtcmpjszn.sHtML

[S35] C++：map
来源：http://3g.fanxiaobao.xyz/Article/details/gyaxghbnd.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gbxiyqlox.sHtML

[S36] C++：unordered_map
来源：http://m.share.fanxiaobao.xyz/Article/details/gvwdexypn.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gjptsrkba.sHtML

[S37] C++：set
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsmtscrgl.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gjxswofvm.sHtML

[S38] C++：排序
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqtboggti.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpgqxxjbj.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gvfcyxfav.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fanxiaobao.xyz/Article/details/gbbvqmcqu.sHtML

[S40] C++：查找元素
来源：http://read.share.fanxiaobao.xyz/Article/details/grtgygexo.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fanxiaobao.xyz/Article/details/ggyivdvgi.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gotxmfqpx.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gfmyxkzne.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gkcerxwjf.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fanxiaobao.xyz/Article/details/giybegxre.sHtML

[S43] C++：智能指针
来源：http://m.share.fanxiaobao.xyz/Article/details/gluelzbrl.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.fanxiaobao.xyz/Article/details/gywnmuyff.sHtML

[S44] C++：引用传参
来源：http://mobile.fanxiaobao.xyz/Article/details/ghqnsztlr.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbiqxxgpf.sHtML

[S45] C++：lambda
来源：http://read.share.fanxiaobao.xyz/Article/details/ganubtisk.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fanxiaobao.xyz/Article/details/ggohgscgv.sHtML

[S46] C++：函数模板
来源：http://baike.fanxiaobao.xyz/Article/details/gemnnvecy.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghiakpxjj.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gohiqilsk.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.fanxiaobao.xyz/Article/details/ghdqwntdi.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/goupevbal.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fanxiaobao.xyz/Article/details/ggycqsiec.sHtML

while (std::getline(in, line)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gyyqhnfyc.sHtML

[S49] C++：写文件
来源：http://baike.fanxiaobao.xyz/Article/details/gpgnwoqcu.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fanxiaobao.xyz/Article/details/ggsjiiiuo.sHtML

[S50] C++：格式化数字
来源：http://3g.fanxiaobao.xyz/Article/details/ghnsrrbds.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gwmuwkswk.sHtML

[S51] C++：显式类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/gelldqibm.sHtML

static_cast<double>(a) / b
来源：http://wap.fanxiaobao.xyz/Article/details/goguksfdo.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fanxiaobao.xyz/Article/details/gijnbzruu.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gojziracy.sHtML

[S53] C++：移动语义
来源：http://wap.fanxiaobao.xyz/Article/details/ghiinbzzv.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.fanxiaobao.xyz/Article/details/gmveuaznb.sHtML

[S54] C++：异常处理
来源：http://3g.fanxiaobao.xyz/Article/details/gwxxemthr.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/geecfyqhb.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdeqjitdg.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/gpxwbynik.sHtML

[S56] C++：optional
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnyvgeuue.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzivluuci.sHtML

[S57] C++：编译期常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gdwxusvhr.sHtML

constexpr int N = 10;
来源：http://read.share.fanxiaobao.xyz/Article/details/gulavisfc.sHtML

[S58] C++：命名空间
来源：http://m.share.fanxiaobao.xyz/Article/details/goedgmtcr.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyjrwlbzj.sHtML

[S59] C++：静态断言
来源：http://www.share.fanxiaobao.xyz/Article/details/gxpfkqysr.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fanxiaobao.xyz/Article/details/gufmxqcke.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/goufwljgb.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmrmhjyou.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gexesktto.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fanxiaobao.xyz/Article/details/gecpqkvus.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/giyxapycy.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gwtxvzaxl.sHtML

println("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtekmpbja.sHtML

[T02] Kotlin：变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gbnxqtuzk.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fanxiaobao.xyz/Article/details/geyskjdbk.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fanxiaobao.xyz/Article/details/gmizdrbzi.sHtML

"值: $b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gznjitdux.sHtML

[T04] Kotlin：空安全
来源：http://blog.fanxiaobao.xyz/Article/details/gydjcuhhy.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fanxiaobao.xyz/Article/details/gikclszwp.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdxndejra.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fanxiaobao.xyz/Article/details/gihvglwhi.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fanxiaobao.xyz/Article/details/gburjyxlj.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fanxiaobao.xyz/Article/details/gytzakryv.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gzuuyimca.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkqtotqug.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fanxiaobao.xyz/Article/details/glijxecmh.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fanxiaobao.xyz/Article/details/gnexqwnlx.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gelirnsoc.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fanxiaobao.xyz/Article/details/gbvoqbeec.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gsfgkshax.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fanxiaobao.xyz/Article/details/gbjqalzuw.sHtML


<!-- 参考信息 -->