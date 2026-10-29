代发 wailian999

name="${1:-default}"
来源：http://blog.zdbjq.cn/Article/details/gkirkdqkq.sHtML

[R06] 判断命令是否存在
来源：http://3g.fehbvm.com/Article/details/gowupedvx.sHtML

command -v git >/dev/null || { echo "缺少 git"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/gqixvocxf.sHtML

[R07] if 判断文件
来源：http://3g.zdbjq.cn/Article/details/gasfrfrhi.sHtML

if [[ -f "$f" ]]; then echo "是文件"; fi
来源：http://baike.fehbvm.com/Article/details/gngkvliun.sHtML

[R08] 数值比较
来源：http://baike.zdbjq.cn/Article/details/gsrrmvxor.sHtML

if (( a > b )); then echo "a 更大"; fi
来源：http://m.share.fehbvm.com/Article/details/gmuhhsjya.sHtML

[R09] 字符串比较
来源：http://www.m.share.zdbjq.cn/Article/details/gemxljusl.sHtML

if [[ "$a" == "$b" ]]; then echo "相等"; fi
来源：http://mobile.zdbjq.cn/Article/details/glaxsrhjy.sHtML

[R10] 正则匹配
来源：http://wap.zdbjq.cn/Article/details/glmuhgrqs.sHtML

if [[ "$s" =~ ^[0-9]+$ ]]; then echo "纯数字"; fi
来源：http://mobile.zdbjq.cn/Article/details/gntavruvg.sHtML

[R11] case 多分支
来源：http://www.blog.hesvh.cn/Article/details/gzdyvxwcb.sHtML

case "$1" in
来源：http://mobile.zdbjq.cn/Article/details/gecyfdimv.sHtML

start) echo "启动" ;;
来源：http://www.share.zdbjq.cn/Article/details/gsjxnrceo.sHtML

stop)  echo "停止" ;;
来源：http://www.m.share.hesvh.cn/Article/details/glnqogwjm.sHtML

*)     echo "未知命令" ;;
来源：http://mobile.hesvh.cn/Article/details/gccrwqxih.sHtML

esac
来源：http://blog.fehbvm.com/Article/details/glouzzhdb.sHtML

[R12] for 遍历文件
来源：http://read.share.fehbvm.com/Article/details/gwfuqbokp.sHtML

for f in *.txt; do echo "$f"; done
来源：http://www.share.hesvh.cn/Article/details/golmlhmok.sHtML

[R13] for 计数循环
来源：http://blog.hesvh.cn/Article/details/gssbcbdgs.sHtML

for i in {1..10}; do echo "$i"; done
来源：http://www.blog.hesvh.cn/Article/details/gxfxsfpiz.sHtML

[R14] C 风格 for
来源：http://www.blog.fehbvm.com/Article/details/gycbmtnxh.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://read.share.zdbjq.cn/Article/details/gvwxxfzuo.sHtML

[R15] while 逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gmlvsqbei.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://www.blog.fehbvm.com/Article/details/gfbkxriyo.sHtML

[R16] until 等待条件
来源：http://3g.hesvh.cn/Article/details/gvaotgovl.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://m.share.fehbvm.com/Article/details/gzmtfcpof.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.fehbvm.com/Article/details/gazyovllk.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://www.m.share.hesvh.cn/Article/details/gfxthosxb.sHtML

[R18] 遍历数组
来源：http://www.share.hesvh.cn/Article/details/gwfefnrvd.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://m.share.fehbvm.com/Article/details/ghqkpgajg.sHtML

[R19] 数组长度
来源：http://wap.hesvh.cn/Article/details/ggbgdndkx.sHtML

echo "${#arr[@]}"
来源：http://read.share.fehbvm.com/Article/details/guljvawic.sHtML

[R20] 关联数组（字典）
来源：http://blog.hesvh.cn/Article/details/gxgqowikk.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://www.m.share.zdbjq.cn/Article/details/gztkzxgua.sHtML

[R21] 字符串长度
来源：http://m.share.zdbjq.cn/Article/details/gupyuxijq.sHtML

echo "${#s}"
来源：http://3g.zdbjq.cn/Article/details/gfmvnzhip.sHtML

[R22] 截取子串
来源：http://mobile.fehbvm.com/Article/details/ggyfgpvfn.sHtML

echo "${s:0:5}"
来源：http://www.m.share.zdbjq.cn/Article/details/gkccdenfx.sHtML

[R23] 字符串替换
来源：http://read.share.zdbjq.cn/Article/details/gedalhnab.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fehbvm.com/Article/details/gfeksnqxv.sHtML

[R24] 大小写转换
来源：http://mobile.hesvh.cn/Article/details/getbsruxs.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.share.fehbvm.com/Article/details/gbiylsbrx.sHtML

[R25] 去后缀 / 去前缀
来源：http://blog.fehbvm.com/Article/details/glemkdduf.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://m.share.fehbvm.com/Article/details/gctfszvaz.sHtML

[R26] 命令替换
来源：http://baike.fehbvm.com/Article/details/ggkkqmeck.sHtML

now=$(date +%F); echo "$now"
来源：http://m.share.zdbjq.cn/Article/details/gciatmcyl.sHtML

[R27] 算术展开
来源：http://mobile.zdbjq.cn/Article/details/gtkuotjym.sHtML

echo $((1 + 2 * 3))
来源：http://mobile.zdbjq.cn/Article/details/givwhmfez.sHtML

[R28] 浮点运算
来源：http://mobile.zdbjq.cn/Article/details/gunfgeflp.sHtML

echo "scale=2; 10/3" | bc
来源：http://read.share.zdbjq.cn/Article/details/gioolhwwr.sHtML

[R29] 定义函数
来源：http://m.share.zdbjq.cn/Article/details/gjckkevri.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://read.share.fehbvm.com/Article/details/gjgfzuptz.sHtML

[R30] 函数返回状态码
来源：http://3g.zdbjq.cn/Article/details/gshysnttw.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://mobile.fehbvm.com/Article/details/gsvmtrxma.sHtML

[R31] 局部变量
来源：http://www.m.share.zdbjq.cn/Article/details/gboydwpmi.sHtML

f() { local x=1; echo "$x"; }
来源：http://wap.hesvh.cn/Article/details/gebtxmrax.sHtML

[R32] 参数个数校验
来源：http://m.share.zdbjq.cn/Article/details/gmhbmnnbo.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://3g.hesvh.cn/Article/details/gskwskdfq.sHtML

[R33] 捕获错误并提示行号
来源：http://baike.fehbvm.com/Article/details/gvzseemqi.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://blog.hesvh.cn/Article/details/ghnecdjnw.sHtML

[R34] 退出时清理
来源：http://blog.zdbjq.cn/Article/details/gerdpruqc.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/gjftumsjz.sHtML

[R35] 后台执行并等待
来源：http://mobile.zdbjq.cn/Article/details/gjjhrdaud.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.zdbjq.cn/Article/details/gwqhycljj.sHtML

[R36] 并发执行多个任务
来源：http://m.share.zdbjq.cn/Article/details/gfbmbpvqh.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.zdbjq.cn/Article/details/ghafatqhu.sHtML

[R37] 把输出赋给变量
来源：http://baike.zdbjq.cn/Article/details/gzltsqeod.sHtML

files=$(ls -1)
来源：http://3g.fehbvm.com/Article/details/gauvipzyd.sHtML

[R38] 管道串联
来源：http://www.share.fehbvm.com/Article/details/gbuzfkedw.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.fehbvm.com/Article/details/ghuwxeory.sHtML

[R39] 重定向标准输出与错误
来源：http://www.m.share.zdbjq.cn/Article/details/gvieoprce.sHtML

cmd > out.log 2>&1
来源：http://m.share.zdbjq.cn/Article/details/gzqprbeyr.sHtML

[R40] 追加写日志
来源：http://www.m.share.zdbjq.cn/Article/details/gjyprqjit.sHtML

echo "log" >> out.log
来源：http://baike.fehbvm.com/Article/details/gwuisvxqg.sHtML

[R41] 丢弃输出
来源：http://m.share.fehbvm.com/Article/details/gpyemdpbc.sHtML

cmd >/dev/null 2>&1
来源：http://blog.hesvh.cn/Article/details/gmtqfbfhu.sHtML

[R42] 输入重定向
来源：http://m.share.hesvh.cn/Article/details/gcvyesqln.sHtML

wc -l < a.txt
来源：http://read.share.zdbjq.cn/Article/details/gymznwalo.sHtML

[R43] 按名字查找文件
来源：http://www.m.share.hesvh.cn/Article/details/glbsuhmdt.sHtML

find . -name "*.log" -type f
来源：http://m.share.fehbvm.com/Article/details/gmnyhrlrf.sHtML

[R44] 按修改时间查找
来源：http://m.share.zdbjq.cn/Article/details/ghvrtgbud.sHtML

find . -mtime -7 -type f
来源：http://blog.zdbjq.cn/Article/details/ghlsknmls.sHtML

[R45] 批量删除
来源：http://mobile.fehbvm.com/Article/details/gokcfxrmr.sHtML

find . -name "*.tmp" -delete
来源：http://baike.hesvh.cn/Article/details/gtxrxzncm.sHtML

[R46] 递归替换文件内容
来源：http://m.share.zdbjq.cn/Article/details/gcujepdky.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://blog.zdbjq.cn/Article/details/gfsipprga.sHtML

[R47] sed 单行替换
来源：http://blog.fehbvm.com/Article/details/gexiaalvk.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.fehbvm.com/Article/details/gthtujyqv.sHtML

[R48] awk 取指定列
来源：http://baike.fehbvm.com/Article/details/ginxfvqxv.sHtML

awk '{print $1, $3}' a.txt
来源：http://read.share.hesvh.cn/Article/details/gpdtjksdp.sHtML

[R49] awk 带条件
来源：http://blog.zdbjq.cn/Article/details/gqzpitohe.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://blog.fehbvm.com/Article/details/gpawwmsvh.sHtML

[R50] awk 求和
来源：http://blog.fehbvm.com/Article/details/gglyseqks.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fehbvm.com/Article/details/glawhcurf.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.zdbjq.cn/Article/details/gxdrlazpw.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fehbvm.com/Article/details/gdmjyhfsk.sHtML

[R52] 统计行数
来源：http://www.m.share.hesvh.cn/Article/details/gxsluultx.sHtML

wc -l a.txt
来源：http://mobile.fehbvm.com/Article/details/gozhgadqh.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fehbvm.com/Article/details/gctytiwsb.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://m.share.zdbjq.cn/Article/details/glgiovhjm.sHtML

[R54] 比较两个文件
来源：http://m.share.fehbvm.com/Article/details/gkeilgjnx.sHtML

diff a.txt b.txt
来源：http://wap.hesvh.cn/Article/details/guznjdnsm.sHtML

[R55] 压缩与解压
来源：http://wap.zdbjq.cn/Article/details/gjohadncc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.fehbvm.com/Article/details/gndfispjj.sHtML

[R56] 远程拷贝
来源：http://www.share.hesvh.cn/Article/details/gcnyxpowx.sHtML

scp file user@host:/path/
来源：http://read.share.hesvh.cn/Article/details/gafqsunrk.sHtML

[R57] 远程执行命令
来源：http://www.blog.zdbjq.cn/Article/details/gofblkdsc.sHtML

ssh user@host 'uptime'
来源：http://www.blog.zdbjq.cn/Article/details/ghkcqyxiy.sHtML

[R58] 下载文件
来源：http://blog.fehbvm.com/Article/details/gfrjzosfz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fehbvm.com/Article/details/guhyvevxu.sHtML

[R59] 发 POST JSON
来源：http://3g.fehbvm.com/Article/details/gzxmgxiaw.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.hesvh.cn/Article/details/gnoduzvlt.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.zdbjq.cn/Article/details/guhnfrwge.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.hesvh.cn/Article/details/ghdkmvrlo.sHtML

[R61] 磁盘占用
来源：http://read.share.hesvh.cn/Article/details/gzxcwwiwe.sHtML

df -h;  du -sh *
来源：http://www.m.share.hesvh.cn/Article/details/gvkmbjfai.sHtML

[R62] 找最占空间的文件
来源：http://baike.zdbjq.cn/Article/details/gnfhuhkku.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.hesvh.cn/Article/details/gseracqbu.sHtML

[R63] 内存与进程
来源：http://baike.hesvh.cn/Article/details/gwkkfmlov.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.zdbjq.cn/Article/details/gwkujdfrv.sHtML

[R64] 结束进程
来源：http://mobile.hesvh.cn/Article/details/gweacyrhg.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.hesvh.cn/Article/details/gqcqrmbfo.sHtML

[R65] 查看端口占用
来源：http://baike.zdbjq.cn/Article/details/gfxgzoyrh.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fehbvm.com/Article/details/gxjxoiftg.sHtML

[R66] 定时任务
来源：http://www.m.share.zdbjq.cn/Article/details/gnvtskayt.sHtML

crontab -e;  crontab -l
来源：http://m.share.zdbjq.cn/Article/details/gendqqfcp.sHtML

[R67] 生成随机十六进制串
来源：http://blog.hesvh.cn/Article/details/gqjmiiwrq.sHtML

openssl rand -hex 16
来源：http://www.blog.fehbvm.com/Article/details/gdedykvbz.sHtML

[R68] 计算文件校验值
来源：http://m.share.zdbjq.cn/Article/details/gozsewdxp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.hesvh.cn/Article/details/gvncccpke.sHtML

[R69] 生成随机密码
来源：http://www.share.fehbvm.com/Article/details/gnumjwgid.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.zdbjq.cn/Article/details/gelxozklb.sHtML

[R70] 时间戳与互转
来源：http://blog.hesvh.cn/Article/details/grahqhara.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.hesvh.cn/Article/details/gxkyqiruk.sHtML

[R71] 日期格式化
来源：http://wap.hesvh.cn/Article/details/gdqtiufpl.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fehbvm.com/Article/details/gvbcfoooh.sHtML

[R72] 等待端口就绪
来源：http://mobile.fehbvm.com/Article/details/gmxahpzhs.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gpwtmiulk.sHtML

[R73] 分割大日志
来源：http://m.share.zdbjq.cn/Article/details/gjzurswyx.sHtML

split -l 1000 big.log part_
来源：http://www.share.zdbjq.cn/Article/details/gvnsewsjf.sHtML

[R74] 批量重命名
来源：http://3g.fehbvm.com/Article/details/gsebxfhxp.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.hesvh.cn/Article/details/gbrjuuqfz.sHtML

[R75] 导出环境变量
来源：http://www.m.share.hesvh.cn/Article/details/gflfpfixn.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fehbvm.com/Article/details/gytzxdlnu.sHtML

[R76] 使用临时文件
来源：http://mobile.fehbvm.com/Article/details/gxarnavpj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fehbvm.com/Article/details/gnqhdobys.sHtML

[R77] 读取用户输入
来源：http://blog.zdbjq.cn/Article/details/gqzswnyss.sHtML

read -rp "请输入: " ans
来源：http://blog.fehbvm.com/Article/details/gilhbohfi.sHtML

[R78] 交互式菜单
来源：http://read.share.zdbjq.cn/Article/details/glohmxzrt.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fehbvm.com/Article/details/gyetghlqd.sHtML

[R79] 解析命令行选项
来源：http://mobile.zdbjq.cn/Article/details/gtlwyauhc.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fehbvm.com/Article/details/guksoxsll.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.hesvh.cn/Article/details/gnjjqgqsc.sHtML

time ./run.sh
来源：http://mobile.fehbvm.com/Article/details/gbwtkhprt.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gowjwotex.sHtML

S. C / C++ 专题
来源：http://blog.fehbvm.com/Article/details/gtbcyzida.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gupfrozjx.sHtML

[S01] C：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/ghwtcjede.sHtML

#include <stdio.h>
来源：http://www.blog.fehbvm.com/Article/details/grexemieg.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.hesvh.cn/Article/details/gdzgzuosf.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.hesvh.cn/Article/details/gwkgodqzf.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.hesvh.cn/Article/details/gwhkokzuo.sHtML

[S03] C：读入整数
来源：http://www.blog.hesvh.cn/Article/details/gzvclhxnb.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fehbvm.com/Article/details/giqljdmjh.sHtML

[S04] C：字符串复制
来源：http://read.share.zdbjq.cn/Article/details/gzyvncclh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.zdbjq.cn/Article/details/gqnsdawfs.sHtML

[S05] C：字符串长度
来源：http://mobile.hesvh.cn/Article/details/grthnyssn.sHtML

strlen(s)
来源：http://read.share.fehbvm.com/Article/details/glswaxdhu.sHtML

[S06] C：字符串比较
来源：http://read.share.fehbvm.com/Article/details/gspwkwzxq.sHtML

strcmp(a, b) == 0
来源：http://www.share.hesvh.cn/Article/details/gjpaigdwl.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.hesvh.cn/Article/details/gdqckkpeh.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fehbvm.com/Article/details/gkgqctdef.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.hesvh.cn/Article/details/glmiwrqgq.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://baike.fehbvm.com/Article/details/gkxluyzvz.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.hesvh.cn/Article/details/gipoezxyk.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.zdbjq.cn/Article/details/gisedvwkb.sHtML

[S10] C：指针与解引用
来源：http://baike.zdbjq.cn/Article/details/gjhudunpl.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.zdbjq.cn/Article/details/giqpbfvgc.sHtML

[S11] C：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gztvqzdyj.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fehbvm.com/Article/details/ghumncdrf.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.zdbjq.cn/Article/details/gyunydykh.sHtML

fclose(f);
来源：http://wap.zdbjq.cn/Article/details/gumyetuyy.sHtML

[S12] C：写文件
来源：http://mobile.zdbjq.cn/Article/details/gnceqripw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.hesvh.cn/Article/details/gwazemplk.sHtML

[S13] C：宏定义
来源：http://read.share.fehbvm.com/Article/details/gdsykzbkc.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fehbvm.com/Article/details/gfcfzdpob.sHtML

[S14] C：枚举
来源：http://www.blog.zdbjq.cn/Article/details/gmcpwecqs.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fehbvm.com/Article/details/geqjtnhpi.sHtML

[S15] C：类型转换
来源：http://m.share.hesvh.cn/Article/details/gusdchyav.sHtML

(double) a / b
来源：http://www.blog.fehbvm.com/Article/details/gruzazzga.sHtML

[S16] C：位操作置位
来源：http://3g.zdbjq.cn/Article/details/gqocafdfh.sHtML

x |= (1 << 3);
来源：http://www.share.hesvh.cn/Article/details/gtmdvfhtb.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gzillaqyx.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.fehbvm.com/Article/details/gqfpnqocr.sHtML

[S18] C：命令行参数
来源：http://www.blog.zdbjq.cn/Article/details/gsfztxeog.sHtML

int main(int argc, char **argv)
来源：http://read.share.fehbvm.com/Article/details/gjtsllifw.sHtML

[S19] C：快速排序
来源：http://wap.hesvh.cn/Article/details/gdrtgaset.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.hesvh.cn/Article/details/gvtqdkxya.sHtML

[S20] C：二分查找
来源：http://mobile.zdbjq.cn/Article/details/gpumakoda.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/gysxrhoxv.sHtML

[S21] C：字符类别判断
来源：http://wap.fehbvm.com/Article/details/glpedwbnp.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.zdbjq.cn/Article/details/gdtroubei.sHtML

[S22] C：字符串转数字
来源：http://3g.fehbvm.com/Article/details/gevctzmbh.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fehbvm.com/Article/details/gbatymdmq.sHtML

[S23] C：随机数
来源：http://3g.hesvh.cn/Article/details/gvizgufru.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.zdbjq.cn/Article/details/gpbmkciti.sHtML

[S24] C：获取本地时间
来源：http://mobile.fehbvm.com/Article/details/gzdgyyuww.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fehbvm.com/Article/details/gtkgxxpif.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/grhnpjyie.sHtML

memcpy(dst, src, n);
来源：http://blog.zdbjq.cn/Article/details/ggqjccxlo.sHtML

[S26] C：内存清零
来源：http://blog.zdbjq.cn/Article/details/gyzcormwm.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fehbvm.com/Article/details/grepiodhp.sHtML

[S27] C：定义常量
来源：http://www.blog.zdbjq.cn/Article/details/gmgjenhhe.sHtML

const double PI = 3.14159;
来源：http://3g.hesvh.cn/Article/details/givbyzkut.sHtML

[S28] C：静态变量
来源：http://3g.zdbjq.cn/Article/details/geswjlxrt.sHtML

static int counter = 0;
来源：http://wap.zdbjq.cn/Article/details/gplhhcrfn.sHtML

[S29] C：变参函数
来源：http://m.share.hesvh.cn/Article/details/gagdcxres.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.m.share.zdbjq.cn/Article/details/gowibxsbq.sHtML

[S30] C：头文件保护
来源：http://read.share.fehbvm.com/Article/details/gyutqnzkk.sHtML

#ifndef X_H
来源：http://www.blog.zdbjq.cn/Article/details/gwngfokkw.sHtML

#define X_H
来源：http://blog.hesvh.cn/Article/details/gwxfngpni.sHtML

#endif
来源：http://read.share.fehbvm.com/Article/details/gpypfdtxo.sHtML

[S31] C++：Hello World
来源：http://blog.hesvh.cn/Article/details/gdfrrpgxp.sHtML

#include <iostream>
来源：http://wap.fehbvm.com/Article/details/gsocjxszo.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.hesvh.cn/Article/details/gwddqrbkb.sHtML

[S32] C++：字符串
来源：http://mobile.fehbvm.com/Article/details/grcndcjxa.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fehbvm.com/Article/details/gvdieljxy.sHtML

[S33] C++：vector 增删
来源：http://blog.hesvh.cn/Article/details/gxqxugiuj.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fehbvm.com/Article/details/gspwxftpf.sHtML

[S34] C++：遍历 vector
来源：http://baike.zdbjq.cn/Article/details/gmmusdxlc.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fehbvm.com/Article/details/glajogxkp.sHtML

[S35] C++：map
来源：http://www.m.share.fehbvm.com/Article/details/gttluxrpr.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gpqwgkbkl.sHtML

[S36] C++：unordered_map
来源：http://www.share.hesvh.cn/Article/details/gmdfrgogj.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.hesvh.cn/Article/details/gevtjqvcv.sHtML

[S37] C++：set
来源：http://read.share.hesvh.cn/Article/details/gkyhhxmeq.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fehbvm.com/Article/details/gblplveav.sHtML

[S38] C++：排序
来源：http://mobile.zdbjq.cn/Article/details/ginmdqhft.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.zdbjq.cn/Article/details/gkclnnyoh.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.zdbjq.cn/Article/details/gthtzbqhj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fehbvm.com/Article/details/ghtcvyqrb.sHtML

[S40] C++：查找元素
来源：http://baike.zdbjq.cn/Article/details/gxrxcsvhj.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fehbvm.com/Article/details/grsyqcbgf.sHtML

[S41] C++：类与构造函数
来源：http://mobile.zdbjq.cn/Article/details/gstxopbdc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.hesvh.cn/Article/details/gtvokvxti.sHtML

[S42] C++：继承与虚函数
来源：http://3g.hesvh.cn/Article/details/gdpcygdwc.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.hesvh.cn/Article/details/gkhvvcjkv.sHtML

[S43] C++：智能指针
来源：http://m.share.hesvh.cn/Article/details/ggodtstnd.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.hesvh.cn/Article/details/gnidduuov.sHtML

[S44] C++：引用传参
来源：http://blog.zdbjq.cn/Article/details/gckfelxxs.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.hesvh.cn/Article/details/grbrnbosy.sHtML

[S45] C++：lambda
来源：http://www.m.share.zdbjq.cn/Article/details/gnqrfskli.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.hesvh.cn/Article/details/guhjgqblr.sHtML

[S46] C++：函数模板
来源：http://mobile.hesvh.cn/Article/details/ggaryhlvv.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.hesvh.cn/Article/details/gjvezgynd.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fehbvm.com/Article/details/gnjxrujyz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.zdbjq.cn/Article/details/gebngyfxn.sHtML

[S48] C++：逐行读文件
来源：http://wap.hesvh.cn/Article/details/gztmnacrd.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.zdbjq.cn/Article/details/gzxmbefmd.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.zdbjq.cn/Article/details/gkevyscgk.sHtML

[S49] C++：写文件
来源：http://blog.fehbvm.com/Article/details/gqleprwwl.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.hesvh.cn/Article/details/gjkmacyvd.sHtML

[S50] C++：格式化数字
来源：http://3g.hesvh.cn/Article/details/gywzduzwz.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.hesvh.cn/Article/details/gciwizsfv.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.hesvh.cn/Article/details/geazffkvz.sHtML

static_cast<double>(a) / b
来源：http://3g.hesvh.cn/Article/details/gnhfnhinp.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fehbvm.com/Article/details/gcfjwfoau.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.zdbjq.cn/Article/details/grxjsjimq.sHtML

[S53] C++：移动语义
来源：http://www.blog.zdbjq.cn/Article/details/geyhibkcz.sHtML

std::vector<int> w = std::move(v);
来源：http://blog.hesvh.cn/Article/details/gkxqzkwwv.sHtML

[S54] C++：异常处理
来源：http://wap.zdbjq.cn/Article/details/gkgiksbxg.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.hesvh.cn/Article/details/gmpahzouo.sHtML

[S55] C++：结构化绑定
来源：http://m.share.fehbvm.com/Article/details/ggqauvxea.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.hesvh.cn/Article/details/gzoquhhdq.sHtML

[S56] C++：optional
来源：http://wap.hesvh.cn/Article/details/ggczmyicr.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fehbvm.com/Article/details/ghjejysgs.sHtML

[S57] C++：编译期常量
来源：http://blog.zdbjq.cn/Article/details/girrwtiqe.sHtML

constexpr int N = 10;
来源：http://baike.fehbvm.com/Article/details/gtlshpnvr.sHtML

[S58] C++：命名空间
来源：http://read.share.fehbvm.com/Article/details/gwfpuvkak.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.zdbjq.cn/Article/details/gkrvqznke.sHtML

[S59] C++：静态断言
来源：http://wap.hesvh.cn/Article/details/gatgourlj.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.hesvh.cn/Article/details/gcyhqsriq.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.fehbvm.com/Article/details/gilcfazop.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://read.share.hesvh.cn/Article/details/gccotedsd.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gogxtdgcu.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.zdbjq.cn/Article/details/ggbywvvfj.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gpshhnrcn.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gmbwbestu.sHtML

println("Hello")
来源：http://m.share.hesvh.cn/Article/details/gluuxnyxl.sHtML

[T02] Kotlin：变量
来源：http://blog.zdbjq.cn/Article/details/gldkgusjf.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.fehbvm.com/Article/details/gcmeyuyvh.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fehbvm.com/Article/details/geiqogzap.sHtML

"值: $b"
来源：http://wap.zdbjq.cn/Article/details/ggrlllvsy.sHtML

[T04] Kotlin：空安全
来源：http://mobile.hesvh.cn/Article/details/gkdsrxuhx.sHtML

val n: String? = null;  n?.length
来源：http://baike.hesvh.cn/Article/details/gzeyjiemc.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.hesvh.cn/Article/details/gpfqcuyyj.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.hesvh.cn/Article/details/gpspjhekl.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.zdbjq.cn/Article/details/gcxkxcjsf.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fehbvm.com/Article/details/gtsnewpkq.sHtML


<!-- 参考信息 -->