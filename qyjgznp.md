代发 wailian999

echo "${s/old/new}"; echo "${s//old/new}"    # 后者全部替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gmlhfietm.sHtML

[R24] 大小写转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gwboretss.sHtML

echo "${s^^}"; echo "${s,,}"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxfqjzkru.sHtML

[R25] 去后缀 / 去前缀
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyidkbaig.sHtML

echo "${f%.txt}"; echo "${f#./}"
来源：http://www.blog.fanxiaobao.xyz/Article/details/glgfdqqfg.sHtML

[R26] 命令替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/getxgvsti.sHtML

now=$(date +%F); echo "$now"
来源：http://read.share.fanxiaobao.xyz/Article/details/gjessvdan.sHtML

[R27] 算术展开
来源：http://baike.fanxiaobao.xyz/Article/details/gltzpexar.sHtML

echo $((1 + 2 * 3))
来源：http://3g.fanxiaobao.xyz/Article/details/glcwbxxtz.sHtML

[R28] 浮点运算
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbmzzghkz.sHtML

echo "scale=2; 10/3" | bc
来源：http://blog.fanxiaobao.xyz/Article/details/gariwggvq.sHtML

[R29] 定义函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvgkftlca.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://3g.fanxiaobao.xyz/Article/details/gvgqpmpgk.sHtML

[R30] 函数返回状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/grnwmzhjb.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://m.share.fanxiaobao.xyz/Article/details/gxdxndpuh.sHtML

[R31] 局部变量
来源：http://blog.fanxiaobao.xyz/Article/details/grqnfyiij.sHtML

f() { local x=1; echo "$x"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/goylkvnij.sHtML

[R32] 参数个数校验
来源：http://www.m.share.fanxiaobao.xyz/Article/details/godcbeixv.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/guxwxznci.sHtML

[R33] 捕获错误并提示行号
来源：http://blog.fanxiaobao.xyz/Article/details/gbzxyrvfk.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://baike.fanxiaobao.xyz/Article/details/gbjurwofb.sHtML

[R34] 退出时清理
来源：http://baike.fanxiaobao.xyz/Article/details/gjyvtmlur.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://baike.fanxiaobao.xyz/Article/details/gfwpzutkd.sHtML

[R35] 后台执行并等待
来源：http://baike.fanxiaobao.xyz/Article/details/gzbihwkxi.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://mobile.fanxiaobao.xyz/Article/details/gicfylbmd.sHtML

[R36] 并发执行多个任务
来源：http://www.share.fanxiaobao.xyz/Article/details/ghcemhloj.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://baike.fanxiaobao.xyz/Article/details/gqvlrmqba.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gumgpcrcj.sHtML

files=$(ls -1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkinkafbu.sHtML

[R38] 管道串联
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbvkmejoz.sHtML

cat a.txt | grep -i error | wc -l
来源：http://read.share.fanxiaobao.xyz/Article/details/glpmrdvmi.sHtML

[R39] 重定向标准输出与错误
来源：http://read.share.fanxiaobao.xyz/Article/details/gebssqkld.sHtML

cmd > out.log 2>&1
来源：http://m.share.fanxiaobao.xyz/Article/details/gvggxtnuo.sHtML

[R40] 追加写日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gctswyjql.sHtML

echo "log" >> out.log
来源：http://blog.fanxiaobao.xyz/Article/details/gecrgatpd.sHtML

[R41] 丢弃输出
来源：http://3g.fanxiaobao.xyz/Article/details/ggbvkvrcy.sHtML

cmd >/dev/null 2>&1
来源：http://mobile.fanxiaobao.xyz/Article/details/gynodjiqd.sHtML

[R42] 输入重定向
来源：http://baike.fanxiaobao.xyz/Article/details/gzzzjyljn.sHtML

wc -l < a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcajowvmz.sHtML

[R43] 按名字查找文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gzrdbjuoj.sHtML

find . -name "*.log" -type f
来源：http://read.share.fanxiaobao.xyz/Article/details/glvnmkxqx.sHtML

[R44] 按修改时间查找
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvulkqezq.sHtML

find . -mtime -7 -type f
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdyubtqbq.sHtML

[R45] 批量删除
来源：http://wap.fanxiaobao.xyz/Article/details/gdawxmevs.sHtML

find . -name "*.tmp" -delete
来源：http://mobile.fanxiaobao.xyz/Article/details/gltdxrzub.sHtML

[R46] 递归替换文件内容
来源：http://blog.fanxiaobao.xyz/Article/details/gzcyijfdi.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://wap.fanxiaobao.xyz/Article/details/gesnsvmys.sHtML

[R47] sed 单行替换
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmxmzzujv.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://baike.fanxiaobao.xyz/Article/details/gqekbkiya.sHtML

[R48] awk 取指定列
来源：http://blog.fanxiaobao.xyz/Article/details/gkkmsxxsg.sHtML

awk '{print $1, $3}' a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gidtvkdtt.sHtML

[R49] awk 带条件
来源：http://blog.fanxiaobao.xyz/Article/details/gjxwfexpz.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://baike.fanxiaobao.xyz/Article/details/gkmvbyenh.sHtML

[R50] awk 求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gtmroezby.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gckupnqvc.sHtML

[R51] 排序去重取前几
来源：http://www.share.fanxiaobao.xyz/Article/details/gjygdtfby.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqqaurcgq.sHtML

[R52] 统计行数
来源：http://wap.fanxiaobao.xyz/Article/details/gbhvmumxc.sHtML

wc -l a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwzhklotn.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fanxiaobao.xyz/Article/details/gqeeremmn.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.fanxiaobao.xyz/Article/details/gytkdyubr.sHtML

[R54] 比较两个文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gduparigt.sHtML

diff a.txt b.txt
来源：http://www.share.fanxiaobao.xyz/Article/details/gknurxhwu.sHtML

[R55] 压缩与解压
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqlletmaj.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fanxiaobao.xyz/Article/details/gvikjoffs.sHtML

[R56] 远程拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbqvjpqoy.sHtML

scp file user@host:/path/
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gahxfrnfe.sHtML

[R57] 远程执行命令
来源：http://baike.fanxiaobao.xyz/Article/details/gzmepbbaj.sHtML

ssh user@host 'uptime'
来源：http://m.share.fanxiaobao.xyz/Article/details/gjmicwmwk.sHtML

[R58] 下载文件
来源：http://baike.fanxiaobao.xyz/Article/details/gadradopl.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fanxiaobao.xyz/Article/details/ghbpqvvkr.sHtML

[R59] 发 POST JSON
来源：http://wap.fanxiaobao.xyz/Article/details/ggdrbmzmm.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fanxiaobao.xyz/Article/details/gdxjwgnri.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fanxiaobao.xyz/Article/details/gggbvstup.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fanxiaobao.xyz/Article/details/gfrvdelmr.sHtML

[R61] 磁盘占用
来源：http://blog.fanxiaobao.xyz/Article/details/gkpekdvon.sHtML

df -h;  du -sh *
来源：http://3g.fanxiaobao.xyz/Article/details/gflzqupii.sHtML

[R62] 找最占空间的文件
来源：http://baike.fanxiaobao.xyz/Article/details/gckbtoxdt.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.fanxiaobao.xyz/Article/details/gfhaouxxp.sHtML

[R63] 内存与进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gpioudjrk.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fanxiaobao.xyz/Article/details/gkfezayff.sHtML

[R64] 结束进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gpzkgqxqy.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.fanxiaobao.xyz/Article/details/gzdeotfom.sHtML

[R65] 查看端口占用
来源：http://wap.fanxiaobao.xyz/Article/details/gbwmdqhki.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.fanxiaobao.xyz/Article/details/gijcrrreh.sHtML

[R66] 定时任务
来源：http://m.share.fanxiaobao.xyz/Article/details/galugkman.sHtML

crontab -e;  crontab -l
来源：http://baike.fanxiaobao.xyz/Article/details/gaedvutfe.sHtML

[R67] 生成随机十六进制串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwkruaiis.sHtML

openssl rand -hex 16
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkmofxkea.sHtML

[R68] 计算文件校验值
来源：http://wap.fanxiaobao.xyz/Article/details/gncbhyizm.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtntlchjt.sHtML

[R69] 生成随机密码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gemqkiooj.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fanxiaobao.xyz/Article/details/glqilloch.sHtML

[R70] 时间戳与互转
来源：http://baike.fanxiaobao.xyz/Article/details/ghlcesnfn.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fanxiaobao.xyz/Article/details/gkkxbzkgi.sHtML

[R71] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxgujqxrg.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fanxiaobao.xyz/Article/details/gdsvwqfkp.sHtML

[R72] 等待端口就绪
来源：http://blog.fanxiaobao.xyz/Article/details/guasyvrcc.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gcqivnldh.sHtML

[R73] 分割大日志
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtpvjmnqv.sHtML

split -l 1000 big.log part_
来源：http://wap.fanxiaobao.xyz/Article/details/gdymmunbn.sHtML

[R74] 批量重命名
来源：http://blog.fanxiaobao.xyz/Article/details/geynuopiz.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gshugzppk.sHtML

[R75] 导出环境变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gehexspfy.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fanxiaobao.xyz/Article/details/gjrmkvzay.sHtML

[R76] 使用临时文件
来源：http://mobile.fanxiaobao.xyz/Article/details/glskubtrg.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/ggfcwfadf.sHtML

[R77] 读取用户输入
来源：http://baike.fanxiaobao.xyz/Article/details/gwkcwtlzn.sHtML

read -rp "请输入: " ans
来源：http://baike.fanxiaobao.xyz/Article/details/grwwbtrju.sHtML

[R78] 交互式菜单
来源：http://wap.fanxiaobao.xyz/Article/details/gothpsqed.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gflosavhj.sHtML

[R79] 解析命令行选项
来源：http://mobile.fanxiaobao.xyz/Article/details/gcvjtattv.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fanxiaobao.xyz/Article/details/ghzkyqlfz.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fanxiaobao.xyz/Article/details/gxrqtdrem.sHtML

time ./run.sh
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnnfutnul.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/ghmuosukz.sHtML

S. C / C++ 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gldrmpjma.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghfjywcma.sHtML

[S01] C：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gwjfpculb.sHtML

#include <stdio.h>
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkhiuszew.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gqehcqrys.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.fanxiaobao.xyz/Article/details/gfwyjaujo.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gntcstxrr.sHtML

[S03] C：读入整数
来源：http://blog.fanxiaobao.xyz/Article/details/gowdupesm.sHtML

int x; scanf("%d", &x);
来源：http://blog.fanxiaobao.xyz/Article/details/gnfpolnxg.sHtML

[S04] C：字符串复制
来源：http://m.share.fanxiaobao.xyz/Article/details/gdxhewckp.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fanxiaobao.xyz/Article/details/gvjmunumt.sHtML

[S05] C：字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gimmaimqe.sHtML

strlen(s)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmqptrcel.sHtML

[S06] C：字符串比较
来源：http://mobile.fanxiaobao.xyz/Article/details/gwpctgbed.sHtML

strcmp(a, b) == 0
来源：http://wap.fanxiaobao.xyz/Article/details/gnjwrzntx.sHtML

[S07] C：数组遍历求和
来源：http://mobile.fanxiaobao.xyz/Article/details/gaifavbdo.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.fanxiaobao.xyz/Article/details/gnduthgys.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fanxiaobao.xyz/Article/details/gncedpevn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fanxiaobao.xyz/Article/details/gjtazgxok.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gonphtyxu.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fanxiaobao.xyz/Article/details/gpwhkeuhu.sHtML

[S10] C：指针与解引用
来源：http://3g.fanxiaobao.xyz/Article/details/gnljbcvpv.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.fanxiaobao.xyz/Article/details/gompppxxa.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gczairkxy.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://3g.fanxiaobao.xyz/Article/details/gsihgkztn.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.share.fanxiaobao.xyz/Article/details/guwnseeel.sHtML

fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwnokidim.sHtML

[S12] C：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gyntcnwuu.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gmufaynyz.sHtML

[S13] C：宏定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/galrootsy.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fanxiaobao.xyz/Article/details/gzzjsgugd.sHtML

[S14] C：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/gwbozvqiy.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fanxiaobao.xyz/Article/details/gzbsvxliu.sHtML

[S15] C：类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/gjpbmkvsa.sHtML

(double) a / b
来源：http://m.share.fanxiaobao.xyz/Article/details/ggnbbaicw.sHtML

[S16] C：位操作置位
来源：http://blog.fanxiaobao.xyz/Article/details/gvurhpcmo.sHtML

x |= (1 << 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gvajjqzgk.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gyppntoud.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fanxiaobao.xyz/Article/details/gocyulcfz.sHtML

[S18] C：命令行参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gnjlffxjv.sHtML

int main(int argc, char **argv)
来源：http://www.share.fanxiaobao.xyz/Article/details/gqvwpcgzv.sHtML

[S19] C：快速排序
来源：http://read.share.fanxiaobao.xyz/Article/details/gurkhvaiw.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gxsbymcwp.sHtML

[S20] C：二分查找
来源：http://m.share.fanxiaobao.xyz/Article/details/gzuwytxux.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gqvtstvef.sHtML

[S21] C：字符类别判断
来源：http://blog.fanxiaobao.xyz/Article/details/gbqdswvtj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fanxiaobao.xyz/Article/details/gxlycbnmn.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxehlnvab.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjidtoioq.sHtML

[S23] C：随机数
来源：http://3g.fanxiaobao.xyz/Article/details/gevtsqydr.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.fanxiaobao.xyz/Article/details/gjprwcsfg.sHtML

[S24] C：获取本地时间
来源：http://mobile.fanxiaobao.xyz/Article/details/ghhnchquu.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnytxovqt.sHtML

[S25] C：内存拷贝
来源：http://3g.fanxiaobao.xyz/Article/details/ghaluikeo.sHtML

memcpy(dst, src, n);
来源：http://www.blog.fanxiaobao.xyz/Article/details/guefrvxfe.sHtML

[S26] C：内存清零
来源：http://read.share.fanxiaobao.xyz/Article/details/glmakjjvl.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fanxiaobao.xyz/Article/details/gskidilad.sHtML

[S27] C：定义常量
来源：http://read.share.fanxiaobao.xyz/Article/details/geigmdpji.sHtML

const double PI = 3.14159;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzrjtfdjz.sHtML

[S28] C：静态变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gwrxqwbuf.sHtML

static int counter = 0;
来源：http://blog.fanxiaobao.xyz/Article/details/gdmzttgvg.sHtML

[S29] C：变参函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gfidbbexj.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fanxiaobao.xyz/Article/details/gbheepzpt.sHtML

[S30] C：头文件保护
来源：http://m.share.fanxiaobao.xyz/Article/details/glypdmimx.sHtML

#ifndef X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gmyulwvly.sHtML

#define X_H
来源：http://wap.fanxiaobao.xyz/Article/details/guedcxfdd.sHtML

#endif
来源：http://m.share.fanxiaobao.xyz/Article/details/gdxvyeuzo.sHtML

[S31] C++：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gbtuuqrdh.sHtML

#include <iostream>
来源：http://m.share.fanxiaobao.xyz/Article/details/gtdzcwodw.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/goxxoxkjs.sHtML

[S32] C++：字符串
来源：http://blog.fanxiaobao.xyz/Article/details/grjtakqxx.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fanxiaobao.xyz/Article/details/gklyvnjtu.sHtML

[S33] C++：vector 增删
来源：http://wap.fanxiaobao.xyz/Article/details/gijeaglzo.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gaacbrtif.sHtML

[S34] C++：遍历 vector
来源：http://baike.fanxiaobao.xyz/Article/details/gpjxrmsqz.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gyopvkonl.sHtML

[S35] C++：map
来源：http://mobile.fanxiaobao.xyz/Article/details/gpspgtugm.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fanxiaobao.xyz/Article/details/gwauyvbwy.sHtML

[S36] C++：unordered_map
来源：http://baike.fanxiaobao.xyz/Article/details/gvqmcmojk.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gygpficez.sHtML

[S37] C++：set
来源：http://m.share.fanxiaobao.xyz/Article/details/gutobcvjx.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/grpozidbc.sHtML

[S38] C++：排序
来源：http://blog.fanxiaobao.xyz/Article/details/gpbwbngqq.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/gdlpoizul.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fanxiaobao.xyz/Article/details/gdpvafoxw.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fanxiaobao.xyz/Article/details/grrdcrnks.sHtML

[S40] C++：查找元素
来源：http://wap.fanxiaobao.xyz/Article/details/gesoqelds.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fanxiaobao.xyz/Article/details/gzomlnghw.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gvufiaozv.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fanxiaobao.xyz/Article/details/ghalqeton.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gepozggoc.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fanxiaobao.xyz/Article/details/gddjeacrp.sHtML

[S43] C++：智能指针
来源：http://m.share.fanxiaobao.xyz/Article/details/gcnnhhmbe.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fanxiaobao.xyz/Article/details/ghcdjqnnc.sHtML

[S44] C++：引用传参
来源：http://baike.fanxiaobao.xyz/Article/details/gellkczfk.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gawujpfam.sHtML

[S45] C++：lambda
来源：http://wap.fanxiaobao.xyz/Article/details/gbnilfohg.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gszlgaqud.sHtML

[S46] C++：函数模板
来源：http://blog.fanxiaobao.xyz/Article/details/gpdvjxyuz.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gotxugknb.sHtML

[S47] C++：结构化绑定遍历
来源：http://wap.fanxiaobao.xyz/Article/details/ganvsnsax.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gleulazjf.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/geynawyab.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggfffgeic.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjalhsxtm.sHtML

[S49] C++：写文件
来源：http://wap.fanxiaobao.xyz/Article/details/glagxmnvp.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fanxiaobao.xyz/Article/details/gfeqydzhb.sHtML

[S50] C++：格式化数字
来源：http://m.share.fanxiaobao.xyz/Article/details/glrivqysl.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gvzpcspbo.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqgzdykhy.sHtML

static_cast<double>(a) / b
来源：http://m.share.fanxiaobao.xyz/Article/details/ghcozsviz.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.fanxiaobao.xyz/Article/details/gdwdovxfz.sHtML

int size() const noexcept { return n_; }
来源：http://blog.fanxiaobao.xyz/Article/details/gmoxxerzz.sHtML

[S53] C++：移动语义
来源：http://wap.fanxiaobao.xyz/Article/details/gdbrwftdt.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdzviiduz.sHtML

[S54] C++：异常处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gmfqitehf.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gunghapgx.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fanxiaobao.xyz/Article/details/gunqzizza.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/gsoijreyd.sHtML

[S56] C++：optional
来源：http://mobile.fanxiaobao.xyz/Article/details/guqrfrcgv.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gchstlnpl.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpapgbsde.sHtML

constexpr int N = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkkmciiys.sHtML

[S58] C++：命名空间
来源：http://wap.fanxiaobao.xyz/Article/details/gnjoyqfpn.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gbvwcsczi.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfnaypmoe.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fanxiaobao.xyz/Article/details/gjdyprayg.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fanxiaobao.xyz/Article/details/gtisdcnfi.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsiqswlqf.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gjukrtiif.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gerpnqzfi.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gltmrzlkz.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gppoenixp.sHtML

println("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/guxofpftx.sHtML

[T02] Kotlin：变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gkjxakfmd.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fanxiaobao.xyz/Article/details/gojbcckbi.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.fanxiaobao.xyz/Article/details/gcqemwpbd.sHtML

"值: $b"
来源：http://wap.fanxiaobao.xyz/Article/details/gxqtbcsot.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmddrkufg.sHtML

val n: String? = null;  n?.length
来源：http://wap.fanxiaobao.xyz/Article/details/gbjjdyhxd.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.fanxiaobao.xyz/Article/details/goclhbquf.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://3g.fanxiaobao.xyz/Article/details/gimiignwm.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fanxiaobao.xyz/Article/details/gdfppmotu.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.fanxiaobao.xyz/Article/details/gdqdkhdgs.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gixqoccau.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fanxiaobao.xyz/Article/details/geqrmvbcp.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fanxiaobao.xyz/Article/details/ggfirmkou.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fanxiaobao.xyz/Article/details/gnyzyetdb.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfmvsljqm.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ginpgqnti.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fanxiaobao.xyz/Article/details/gzrzxzpua.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.fanxiaobao.xyz/Article/details/gyowhqwfn.sHtML

[T11] Kotlin：协程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfsysiyup.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.fanxiaobao.xyz/Article/details/grmwujjol.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.fanxiaobao.xyz/Article/details/gjrdaptvg.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.fanxiaobao.xyz/Article/details/gvkxdlvpj.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fanxiaobao.xyz/Article/details/gitnalqxs.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdiousdre.sHtML

[T14] Kotlin：循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gzpkihken.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gltnlvggl.sHtML

[T15] Kotlin：接口
来源：http://3g.fanxiaobao.xyz/Article/details/gzbrxclbz.sHtML

interface Shape { fun area(): Double }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmbkedqei.sHtML

[T16] Swift：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/ghbqewfym.sHtML

print("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gahbsyrum.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfgmmjexm.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjgnywius.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfbpfzgkb.sHtML

"值: \(b)"
来源：http://baike.fanxiaobao.xyz/Article/details/gwbrpsjjy.sHtML

[T19] Swift：可选绑定
来源：http://wap.fanxiaobao.xyz/Article/details/ghfyddmql.sHtML

if let n = opt { print(n) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtklurzfu.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmmysyzha.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.fanxiaobao.xyz/Article/details/gxdjnznuu.sHtML

[T21] Swift：遍历
来源：http://read.share.fanxiaobao.xyz/Article/details/ggrzwllsw.sHtML

for x in a { print(x) }
来源：http://baike.fanxiaobao.xyz/Article/details/gdlxryxnh.sHtML

[T22] Swift：字典
来源：http://wap.fanxiaobao.xyz/Article/details/gdyotyhxa.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gguriwnwp.sHtML

[T23] Swift：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gtcbajxgx.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.fanxiaobao.xyz/Article/details/gikrkffdm.sHtML

[T24] Swift：闭包
来源：http://m.share.fanxiaobao.xyz/Article/details/gmbwprfjj.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://mobile.fanxiaobao.xyz/Article/details/gjbsgyyqx.sHtML

[T25] Swift：结构体
来源：http://baike.fanxiaobao.xyz/Article/details/glsepykob.sHtML

struct P { var x: Int }
来源：http://mobile.fanxiaobao.xyz/Article/details/gyyyrkaio.sHtML

[T26] Swift：类与重写
来源：http://baike.fanxiaobao.xyz/Article/details/gzltuovjn.sHtML

class A: Base { override func f() {} }
来源：http://3g.fanxiaobao.xyz/Article/details/galvmvtxy.sHtML


<!-- 参考信息 -->