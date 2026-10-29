代发 wailian999

for i in {1..10}; do echo "$i"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gfxboynnm.sHtML

[R14] C 风格 for
来源：http://www.share.zdbjq.cn/Article/details/gimhpufls.sHtML

for ((i = 0; i < 10; i++)); do echo "$i"; done
来源：http://wap.zdbjq.cn/Article/details/gkycshywn.sHtML

[R15] while 逐行读文件
来源：http://blog.fehbvm.com/Article/details/grgpownmk.sHtML

while IFS= read -r line; do echo "$line"; done < file.txt
来源：http://read.share.hesvh.cn/Article/details/ggccjvepa.sHtML

[R16] until 等待条件
来源：http://baike.fehbvm.com/Article/details/gzuauwrwp.sHtML

until [[ -f done.flag ]]; do sleep 1; done
来源：http://read.share.fehbvm.com/Article/details/gfcxxvqiu.sHtML

[R17] 数组定义与取值
来源：http://www.m.share.hesvh.cn/Article/details/gnxyjgtov.sHtML

arr=(a b c); echo "${arr[0]}"
来源：http://wap.zdbjq.cn/Article/details/gnbderbea.sHtML

[R18] 遍历数组
来源：http://www.blog.fehbvm.com/Article/details/gyxxzukhb.sHtML

for x in "${arr[@]}"; do echo "$x"; done
来源：http://wap.fehbvm.com/Article/details/gnpyqbjnu.sHtML

[R19] 数组长度
来源：http://www.m.share.fehbvm.com/Article/details/gtybtsdjk.sHtML

echo "${#arr[@]}"
来源：http://blog.hesvh.cn/Article/details/gqakgiroj.sHtML

[R20] 关联数组（字典）
来源：http://www.m.share.hesvh.cn/Article/details/gzrqzpqlf.sHtML

declare -A m; m[k]=v; echo "${m[k]}"
来源：http://mobile.hesvh.cn/Article/details/gwcuetyfd.sHtML

[R21] 字符串长度
来源：http://m.share.hesvh.cn/Article/details/garffhorz.sHtML

echo "${#s}"
来源：http://blog.fehbvm.com/Article/details/gxrzqgnze.sHtML

[R22] 截取子串
来源：http://read.share.fehbvm.com/Article/details/gtjcijoek.sHtML

echo "${s:0:5}"
来源：http://www.blog.hesvh.cn/Article/details/gjjocgojv.sHtML

[R23] 字符串替换
来源：http://blog.fehbvm.com/Article/details/gonhrxpct.sHtML

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.hesvh.cn/Article/details/grijkemwf.sHtML

[R24] 大小写转换
来源：http://read.share.fehbvm.com/Article/details/giwefjxuu.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://3g.fehbvm.com/Article/details/gvhbmegvz.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.zdbjq.cn/Article/details/gudgehfgc.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://read.share.fehbvm.com/Article/details/giwojhkig.sHtML

[R26] 命令替换
来源：http://3g.fehbvm.com/Article/details/gcdgeefey.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.zdbjq.cn/Article/details/gqhimmdqj.sHtML

[R27] 算术展开
来源：http://www.blog.zdbjq.cn/Article/details/gfkxhypmu.sHtML

echo $((1 + 2 * 3))
来源：http://m.share.fehbvm.com/Article/details/ghczjpoer.sHtML

[R28] 浮点运算
来源：http://m.share.fehbvm.com/Article/details/gzidkhvia.sHtML

echo "scale=2; 10/3" | bc
来源：http://3g.fehbvm.com/Article/details/gbytnxioh.sHtML

[R29] 定义函数
来源：http://baike.hesvh.cn/Article/details/gtuvkevop.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.share.fehbvm.com/Article/details/gzfrhgbmi.sHtML

[R30] 函数返回状态码
来源：http://mobile.zdbjq.cn/Article/details/gpequbznk.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.hesvh.cn/Article/details/gkphbteaq.sHtML

[R31] 局部变量
来源：http://wap.zdbjq.cn/Article/details/gacdemjim.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fehbvm.com/Article/details/gvvwjnmtr.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fehbvm.com/Article/details/glqlkabac.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://m.share.hesvh.cn/Article/details/gygpxugpv.sHtML

[R33] 捕获错误并提示行号
来源：http://3g.fehbvm.com/Article/details/geeuvqawp.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fehbvm.com/Article/details/gtbdysueg.sHtML

[R34] 退出时清理
来源：http://www.share.hesvh.cn/Article/details/gvmvkpzmg.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://m.share.zdbjq.cn/Article/details/gocekfhoc.sHtML

[R35] 后台执行并等待
来源：http://3g.zdbjq.cn/Article/details/gymesluff.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.hesvh.cn/Article/details/gardglqzu.sHtML

[R36] 并发执行多个任务
来源：http://www.m.share.hesvh.cn/Article/details/gfihhuqmh.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.hesvh.cn/Article/details/goqjxzxdf.sHtML

[R37] 把输出赋给变量
来源：http://wap.fehbvm.com/Article/details/ggcmfxmto.sHtML

files=$(ls -1)
来源：http://m.share.fehbvm.com/Article/details/gfndpncbu.sHtML

[R38] 管道串联
来源：http://3g.zdbjq.cn/Article/details/gkardqtix.sHtML

cat a.txt | grep -i error | wc -l
来源：http://www.m.share.hesvh.cn/Article/details/grlkvlgqs.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.hesvh.cn/Article/details/gvlvbfmqg.sHtML

cmd > out.log 2>&1
来源：http://read.share.hesvh.cn/Article/details/geppqqoyp.sHtML

[R40] 追加写日志
来源：http://blog.hesvh.cn/Article/details/gaufxkxuh.sHtML

echo "log" >> out.log
来源：http://blog.zdbjq.cn/Article/details/gaxatlybu.sHtML

[R41] 丢弃输出
来源：http://www.share.hesvh.cn/Article/details/glljnxwsc.sHtML

cmd >/dev/null 2>&1
来源：http://blog.zdbjq.cn/Article/details/gxqtxkmfo.sHtML

[R42] 输入重定向
来源：http://www.share.zdbjq.cn/Article/details/gnfchicrp.sHtML

wc -l < a.txt
来源：http://read.share.fehbvm.com/Article/details/glgezgckn.sHtML

[R43] 按名字查找文件
来源：http://blog.hesvh.cn/Article/details/gdgoubnjl.sHtML

find . -name "*.log" -type f
来源：http://blog.fehbvm.com/Article/details/gxgbmikwo.sHtML

[R44] 按修改时间查找
来源：http://mobile.hesvh.cn/Article/details/gpwxjutch.sHtML

find . -mtime -7 -type f
来源：http://read.share.hesvh.cn/Article/details/ghvmtlkic.sHtML

[R45] 批量删除
来源：http://read.share.zdbjq.cn/Article/details/gexgydnrf.sHtML

find . -name "*.tmp" -delete
来源：http://wap.fehbvm.com/Article/details/gvpkvakso.sHtML

[R46] 递归替换文件内容
来源：http://www.blog.hesvh.cn/Article/details/gxsxrqxcq.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fehbvm.com/Article/details/gteomcdsm.sHtML

[R47] sed 单行替换
来源：http://www.blog.zdbjq.cn/Article/details/gclvxqajv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://read.share.zdbjq.cn/Article/details/gmdjbiuvb.sHtML

[R48] awk 取指定列
来源：http://read.share.hesvh.cn/Article/details/gtkpbxsls.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.share.hesvh.cn/Article/details/gwnjhwdkq.sHtML

[R49] awk 带条件
来源：http://3g.zdbjq.cn/Article/details/gfctkeqfi.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wap.zdbjq.cn/Article/details/ghwynaags.sHtML

[R50] awk 求和
来源：http://www.blog.zdbjq.cn/Article/details/gzvommeoj.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://baike.fehbvm.com/Article/details/gzsxftaui.sHtML

[R51] 排序去重取前几
来源：http://read.share.zdbjq.cn/Article/details/ggalnmwxx.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://mobile.hesvh.cn/Article/details/gtupqjoul.sHtML

[R52] 统计行数
来源：http://read.share.fehbvm.com/Article/details/goekgmjbd.sHtML

wc -l a.txt
来源：http://wap.fehbvm.com/Article/details/gabsnffvd.sHtML

[R53] 查看文件头与实时尾
来源：http://wap.hesvh.cn/Article/details/gtuywmfbg.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://baike.zdbjq.cn/Article/details/gylruydwu.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fehbvm.com/Article/details/gevqotbpr.sHtML

diff a.txt b.txt
来源：http://mobile.fehbvm.com/Article/details/gubvkevoo.sHtML

[R55] 压缩与解压
来源：http://wap.zdbjq.cn/Article/details/gdgldowxi.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.blog.hesvh.cn/Article/details/galagrwky.sHtML

[R56] 远程拷贝
来源：http://m.share.zdbjq.cn/Article/details/ggceseybe.sHtML

scp file user@host:/path/
来源：http://www.share.fehbvm.com/Article/details/gkzizpkwh.sHtML

[R57] 远程执行命令
来源：http://wap.hesvh.cn/Article/details/gyuqdytjj.sHtML

ssh user@host 'uptime'
来源：http://baike.hesvh.cn/Article/details/getznkepe.sHtML

[R58] 下载文件
来源：http://www.share.fehbvm.com/Article/details/glgjgdpua.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fehbvm.com/Article/details/gdznsjntj.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fehbvm.com/Article/details/gahhppafn.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fehbvm.com/Article/details/gcagbrhti.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.zdbjq.cn/Article/details/gktdpvfif.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fehbvm.com/Article/details/gbciskzuu.sHtML

[R61] 磁盘占用
来源：http://read.share.fehbvm.com/Article/details/grobamgat.sHtML

df -h;  du -sh *
来源：http://3g.fehbvm.com/Article/details/gizwpronf.sHtML

[R62] 找最占空间的文件
来源：http://blog.zdbjq.cn/Article/details/grytfhdbu.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fehbvm.com/Article/details/gkezurnhl.sHtML

[R63] 内存与进程
来源：http://3g.hesvh.cn/Article/details/gcrnxztci.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.zdbjq.cn/Article/details/glpzqynks.sHtML

[R64] 结束进程
来源：http://www.m.share.hesvh.cn/Article/details/gmvryowtl.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.zdbjq.cn/Article/details/gwoejdrfb.sHtML

[R65] 查看端口占用
来源：http://blog.hesvh.cn/Article/details/gsxgocydn.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.hesvh.cn/Article/details/gzgfaupcs.sHtML

[R66] 定时任务
来源：http://read.share.hesvh.cn/Article/details/glyzyippt.sHtML

crontab -e;  crontab -l
来源：http://3g.zdbjq.cn/Article/details/gkjwwpgzy.sHtML

[R67] 生成随机十六进制串
来源：http://blog.hesvh.cn/Article/details/gxujofbut.sHtML

openssl rand -hex 16
来源：http://www.blog.fehbvm.com/Article/details/gkgfiytid.sHtML

[R68] 计算文件校验值
来源：http://mobile.zdbjq.cn/Article/details/gqkdikxtk.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fehbvm.com/Article/details/ghasswayl.sHtML

[R69] 生成随机密码
来源：http://wap.zdbjq.cn/Article/details/gqiptdimb.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.zdbjq.cn/Article/details/gcdmdsbzt.sHtML

[R70] 时间戳与互转
来源：http://mobile.fehbvm.com/Article/details/gqxuwycmn.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.fehbvm.com/Article/details/gumriqpld.sHtML

[R71] 日期格式化
来源：http://wap.fehbvm.com/Article/details/gbysixdhw.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.zdbjq.cn/Article/details/gfytsverk.sHtML

[R72] 等待端口就绪
来源：http://blog.zdbjq.cn/Article/details/geepgyrmv.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fehbvm.com/Article/details/gwmbhigwt.sHtML

[R73] 分割大日志
来源：http://www.m.share.fehbvm.com/Article/details/grkvgfwpe.sHtML

split -l 1000 big.log part_
来源：http://baike.fehbvm.com/Article/details/gwtelddoj.sHtML

[R74] 批量重命名
来源：http://blog.hesvh.cn/Article/details/gewmcamkz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.hesvh.cn/Article/details/gmenzuwlo.sHtML

[R75] 导出环境变量
来源：http://www.share.hesvh.cn/Article/details/gdispgsca.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.zdbjq.cn/Article/details/gccztbdgb.sHtML

[R76] 使用临时文件
来源：http://baike.fehbvm.com/Article/details/gigcixceq.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fehbvm.com/Article/details/gddzujskw.sHtML

[R77] 读取用户输入
来源：http://blog.hesvh.cn/Article/details/gpvzscopq.sHtML

read -rp "请输入: " ans
来源：http://read.share.hesvh.cn/Article/details/gbnazfhlz.sHtML

[R78] 交互式菜单
来源：http://www.share.hesvh.cn/Article/details/gevirnkav.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fehbvm.com/Article/details/gzvenrbtd.sHtML

[R79] 解析命令行选项
来源：http://www.m.share.hesvh.cn/Article/details/gjidzshwh.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.hesvh.cn/Article/details/gtizbjnue.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fehbvm.com/Article/details/gwtrogpdy.sHtML

time ./run.sh
来源：http://read.share.fehbvm.com/Article/details/gpghpfdth.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/giclgdjyy.sHtML

S. C / C++ 专题
来源：http://www.share.zdbjq.cn/Article/details/gzdxawqme.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gtwzidwmt.sHtML

[S01] C：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gzkdykusa.sHtML

#include <stdio.h>
来源：http://read.share.hesvh.cn/Article/details/gxuxvznqp.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.zdbjq.cn/Article/details/gzojluxgx.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fehbvm.com/Article/details/gkiyqywoa.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.zdbjq.cn/Article/details/gtnqanool.sHtML

[S03] C：读入整数
来源：http://www.blog.zdbjq.cn/Article/details/gdgolymms.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.hesvh.cn/Article/details/gjyiagvra.sHtML

[S04] C：字符串复制
来源：http://read.share.hesvh.cn/Article/details/ggvydowfx.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.zdbjq.cn/Article/details/gxitmzhlh.sHtML

[S05] C：字符串长度
来源：http://wap.fehbvm.com/Article/details/ggvblncpn.sHtML

strlen(s)
来源：http://wap.fehbvm.com/Article/details/gmbcizcen.sHtML

[S06] C：字符串比较
来源：http://www.share.fehbvm.com/Article/details/gumdlwroz.sHtML

strcmp(a, b) == 0
来源：http://read.share.fehbvm.com/Article/details/gzlpuorzb.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.zdbjq.cn/Article/details/gmtrgxost.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.zdbjq.cn/Article/details/gnrmwaisu.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.hesvh.cn/Article/details/gbbddhzsi.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.zdbjq.cn/Article/details/galsoivqo.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.hesvh.cn/Article/details/ghkszjhjn.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.zdbjq.cn/Article/details/gadpoqogo.sHtML

[S10] C：指针与解引用
来源：http://blog.hesvh.cn/Article/details/gqtxecglk.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.zdbjq.cn/Article/details/gzogsvhkf.sHtML

[S11] C：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gotkjijsy.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.hesvh.cn/Article/details/gtfepdxyw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.hesvh.cn/Article/details/gtzggzpxk.sHtML

fclose(f);
来源：http://www.share.hesvh.cn/Article/details/gyexoghnb.sHtML

[S12] C：写文件
来源：http://www.blog.hesvh.cn/Article/details/gkcvlbuzd.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.hesvh.cn/Article/details/gqxvoqekl.sHtML

[S13] C：宏定义
来源：http://www.blog.hesvh.cn/Article/details/gbwhovhxg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fehbvm.com/Article/details/gpmhflbob.sHtML

[S14] C：枚举
来源：http://read.share.hesvh.cn/Article/details/gzbnqgobs.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fehbvm.com/Article/details/gyafgiawv.sHtML

[S15] C：类型转换
来源：http://mobile.fehbvm.com/Article/details/gmifrffab.sHtML

(double) a / b
来源：http://mobile.fehbvm.com/Article/details/gwtelxxfz.sHtML

[S16] C：位操作置位
来源：http://3g.fehbvm.com/Article/details/ghflsyhcp.sHtML

x |= (1 << 3);
来源：http://read.share.fehbvm.com/Article/details/gguaxiecu.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gfjdpzclv.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fehbvm.com/Article/details/goxndckwv.sHtML

[S18] C：命令行参数
来源：http://mobile.zdbjq.cn/Article/details/gzzlpdcmy.sHtML

int main(int argc, char **argv)
来源：http://blog.zdbjq.cn/Article/details/ggrxbdokj.sHtML

[S19] C：快速排序
来源：http://blog.fehbvm.com/Article/details/ghjuovyls.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.hesvh.cn/Article/details/gmqthxomi.sHtML

[S20] C：二分查找
来源：http://3g.hesvh.cn/Article/details/gajtettxk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.zdbjq.cn/Article/details/gustafmld.sHtML

[S21] C：字符类别判断
来源：http://m.share.hesvh.cn/Article/details/gnadbchix.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.zdbjq.cn/Article/details/gvdkyejie.sHtML

[S22] C：字符串转数字
来源：http://www.share.hesvh.cn/Article/details/gjnzfrejb.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fehbvm.com/Article/details/gmyoxlkdk.sHtML

[S23] C：随机数
来源：http://www.m.share.zdbjq.cn/Article/details/gtyqhjktq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.hesvh.cn/Article/details/guezfnxjk.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.hesvh.cn/Article/details/gtwizejtd.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.hesvh.cn/Article/details/grtejiotk.sHtML

[S25] C：内存拷贝
来源：http://baike.hesvh.cn/Article/details/gfryxeppr.sHtML

memcpy(dst, src, n);
来源：http://3g.zdbjq.cn/Article/details/ghuiaqhnj.sHtML

[S26] C：内存清零
来源：http://m.share.hesvh.cn/Article/details/gipcgwcpx.sHtML

memset(a, 0, sizeof a);
来源：http://blog.hesvh.cn/Article/details/gwojvvkpo.sHtML

[S27] C：定义常量
来源：http://www.share.zdbjq.cn/Article/details/gvhfnzhlm.sHtML

const double PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/gnbolzotq.sHtML

[S28] C：静态变量
来源：http://baike.fehbvm.com/Article/details/gzegsboeh.sHtML

static int counter = 0;
来源：http://blog.zdbjq.cn/Article/details/ghdujbqvo.sHtML

[S29] C：变参函数
来源：http://www.m.share.fehbvm.com/Article/details/glupyqtqg.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.hesvh.cn/Article/details/gkembglzz.sHtML

[S30] C：头文件保护
来源：http://blog.zdbjq.cn/Article/details/gflbooaed.sHtML

#ifndef X_H
来源：http://read.share.fehbvm.com/Article/details/gkuemtyzg.sHtML

#define X_H
来源：http://www.share.zdbjq.cn/Article/details/gihhwykpe.sHtML

#endif
来源：http://mobile.hesvh.cn/Article/details/gzcklvnjf.sHtML

[S31] C++：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gsryvbakm.sHtML

#include <iostream>
来源：http://m.share.hesvh.cn/Article/details/gkapcxsmn.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.hesvh.cn/Article/details/gtclknvnf.sHtML

[S32] C++：字符串
来源：http://m.share.zdbjq.cn/Article/details/gxdblrzxj.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fehbvm.com/Article/details/gkkkciudo.sHtML

[S33] C++：vector 增删
来源：http://blog.zdbjq.cn/Article/details/gepkgxsmk.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.hesvh.cn/Article/details/gdknfruza.sHtML

[S34] C++：遍历 vector
来源：http://m.share.zdbjq.cn/Article/details/gfrdgxbun.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fehbvm.com/Article/details/giilmjytb.sHtML

[S35] C++：map
来源：http://mobile.zdbjq.cn/Article/details/gyukgdesj.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gbzwpxwlp.sHtML

[S36] C++：unordered_map
来源：http://wap.hesvh.cn/Article/details/gmayrzmge.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.hesvh.cn/Article/details/gqllpktfr.sHtML

[S37] C++：set
来源：http://wap.zdbjq.cn/Article/details/gdodtmntg.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.hesvh.cn/Article/details/gjnorjtzn.sHtML

[S38] C++：排序
来源：http://read.share.zdbjq.cn/Article/details/gzawrgwlc.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.zdbjq.cn/Article/details/gzhzcpvtp.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.zdbjq.cn/Article/details/gkhpnhzny.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fehbvm.com/Article/details/gqzcdkmnf.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fehbvm.com/Article/details/ggaumxzex.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fehbvm.com/Article/details/gudubfivl.sHtML

[S41] C++：类与构造函数
来源：http://blog.fehbvm.com/Article/details/gsijwfvli.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.zdbjq.cn/Article/details/gdqilgkdc.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fehbvm.com/Article/details/ggmoonrmw.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.hesvh.cn/Article/details/ggyhxiicn.sHtML

[S43] C++：智能指针
来源：http://m.share.fehbvm.com/Article/details/godsydicl.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.fehbvm.com/Article/details/gbcxwciwh.sHtML

[S44] C++：引用传参
来源：http://www.m.share.zdbjq.cn/Article/details/gqwqyxsjo.sHtML

void inc(int &x) { ++x; }
来源：http://read.share.fehbvm.com/Article/details/gzhzspvuy.sHtML

[S45] C++：lambda
来源：http://mobile.hesvh.cn/Article/details/gvdhqupjj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.zdbjq.cn/Article/details/gsqjvbclh.sHtML

[S46] C++：函数模板
来源：http://wap.hesvh.cn/Article/details/gjvigjcyu.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.hesvh.cn/Article/details/glslrusvb.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.hesvh.cn/Article/details/gjgimmdxo.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.hesvh.cn/Article/details/gzaloedda.sHtML

[S48] C++：逐行读文件
来源：http://baike.fehbvm.com/Article/details/glfpfzgby.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.hesvh.cn/Article/details/gxeuwxllm.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.zdbjq.cn/Article/details/grieehjhz.sHtML

[S49] C++：写文件
来源：http://www.blog.hesvh.cn/Article/details/gwcvqbtdv.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fehbvm.com/Article/details/gfepjceun.sHtML

[S50] C++：格式化数字
来源：http://mobile.zdbjq.cn/Article/details/gwmddvtbu.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gdzqdmugl.sHtML

[S51] C++：显式类型转换
来源：http://blog.fehbvm.com/Article/details/gymaxskjq.sHtML

static_cast<double>(a) / b
来源：http://baike.hesvh.cn/Article/details/gzittojhr.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.hesvh.cn/Article/details/gsalkjjko.sHtML

int size() const noexcept { return n_; }
来源：http://baike.zdbjq.cn/Article/details/gcklmtcko.sHtML

[S53] C++：移动语义
来源：http://read.share.hesvh.cn/Article/details/guzkcohri.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fehbvm.com/Article/details/gdwvokikm.sHtML

[S54] C++：异常处理
来源：http://www.m.share.zdbjq.cn/Article/details/gtkruxduq.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.zdbjq.cn/Article/details/gdqthwxig.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.zdbjq.cn/Article/details/ghxlaajmo.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.hesvh.cn/Article/details/gvlakcick.sHtML

[S56] C++：optional
来源：http://wap.zdbjq.cn/Article/details/gbxfoevae.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.m.share.zdbjq.cn/Article/details/gkvrzlvit.sHtML

[S57] C++：编译期常量
来源：http://3g.hesvh.cn/Article/details/gtvlpreqg.sHtML

constexpr int N = 10;
来源：http://www.blog.hesvh.cn/Article/details/gctxovfpo.sHtML

[S58] C++：命名空间
来源：http://www.m.share.hesvh.cn/Article/details/gfdavspjf.sHtML

namespace ns { int f() { return 1; } }
来源：http://read.share.fehbvm.com/Article/details/gamicxtad.sHtML

[S59] C++：静态断言
来源：http://wap.fehbvm.com/Article/details/gqxijjuij.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.hesvh.cn/Article/details/gvvnkoiog.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.hesvh.cn/Article/details/gsgxcwtyh.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fehbvm.com/Article/details/gjoijyyvh.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/ggpezmcvi.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.zdbjq.cn/Article/details/guorutvgp.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gbezelqdr.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fehbvm.com/Article/details/gfjtkbjwb.sHtML

println("Hello")
来源：http://baike.hesvh.cn/Article/details/glckrzixu.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fehbvm.com/Article/details/gggpslikh.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.zdbjq.cn/Article/details/gflqjfthy.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.hesvh.cn/Article/details/gxffnzggg.sHtML

"值: $b"
来源：http://blog.zdbjq.cn/Article/details/gkutselxj.sHtML

[T04] Kotlin：空安全
来源：http://blog.fehbvm.com/Article/details/gsbwourwl.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.fehbvm.com/Article/details/gmylfqzxp.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.hesvh.cn/Article/details/ggjxylaez.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fehbvm.com/Article/details/ghxzeadlr.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.hesvh.cn/Article/details/gtmpqslyl.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fehbvm.com/Article/details/gbwxztbnx.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.fehbvm.com/Article/details/gghpgxqrl.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.hesvh.cn/Article/details/grgmlhlce.sHtML

[T08] Kotlin：数据类
来源：http://read.share.hesvh.cn/Article/details/gylkgxvia.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.hesvh.cn/Article/details/grbuskimz.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.fehbvm.com/Article/details/gzabfsenx.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.hesvh.cn/Article/details/gkkkkiaca.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fehbvm.com/Article/details/goehsuplh.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://m.share.fehbvm.com/Article/details/gvbdihbfs.sHtML

[T11] Kotlin：协程
来源：http://www.blog.fehbvm.com/Article/details/gbghmszmi.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.hesvh.cn/Article/details/gyeutujdp.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.zdbjq.cn/Article/details/gwanzcvay.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.zdbjq.cn/Article/details/grcfuwrjt.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.hesvh.cn/Article/details/gtgzhpizi.sHtML

val m = mapOf("a" to 1)
来源：http://blog.zdbjq.cn/Article/details/gauutvimk.sHtML

[T14] Kotlin：循环
来源：http://www.share.hesvh.cn/Article/details/gueezmxgb.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.zdbjq.cn/Article/details/grpvynzud.sHtML

[T15] Kotlin：接口
来源：http://wap.zdbjq.cn/Article/details/ghwwbvrsj.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.zdbjq.cn/Article/details/gorjinmuk.sHtML

[T16] Swift：Hello World
来源：http://blog.hesvh.cn/Article/details/grstbfulp.sHtML

print("Hello")
来源：http://3g.zdbjq.cn/Article/details/gxqryzxwc.sHtML


<!-- 参考信息 -->