代发 wailian999

echo "${f%.txt}"; echo "${f#./}"
来源：http://wap.fehbvm.com/Article/details/gsgpsynoi.sHtML

[R26] 命令替换
来源：http://www.share.zdbjq.cn/Article/details/ghvpfxnqe.sHtML

now=$(date +%F); echo "$now"
来源：http://wap.zdbjq.cn/Article/details/gcozsywsd.sHtML

[R27] 算术展开
来源：http://m.share.fehbvm.com/Article/details/gygojoxnu.sHtML

echo $((1 + 2 * 3))
来源：http://www.blog.hesvh.cn/Article/details/guuwftzpm.sHtML

[R28] 浮点运算
来源：http://www.blog.zdbjq.cn/Article/details/gfzsaicwt.sHtML

echo "scale=2; 10/3" | bc
来源：http://wap.fehbvm.com/Article/details/gukhmbtqq.sHtML

[R29] 定义函数
来源：http://blog.zdbjq.cn/Article/details/grfyiaklp.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://www.blog.zdbjq.cn/Article/details/gbrysnyzj.sHtML

[R30] 函数返回状态码
来源：http://mobile.hesvh.cn/Article/details/gnydvxhmq.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.share.zdbjq.cn/Article/details/gapcmdjwk.sHtML

[R31] 局部变量
来源：http://3g.zdbjq.cn/Article/details/girvjcwhl.sHtML

f() { local x=1; echo "$x"; }
来源：http://m.share.fehbvm.com/Article/details/gqycuuqrp.sHtML

[R32] 参数个数校验
来源：http://wap.fehbvm.com/Article/details/grotphvnb.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.hesvh.cn/Article/details/gifgyihjs.sHtML

[R33] 捕获错误并提示行号
来源：http://mobile.fehbvm.com/Article/details/gqezjdhax.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://wap.hesvh.cn/Article/details/gjymipenh.sHtML

[R34] 退出时清理
来源：http://blog.hesvh.cn/Article/details/gaudhhmrf.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/gvaearhiu.sHtML

[R35] 后台执行并等待
来源：http://baike.fehbvm.com/Article/details/geqglemrh.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://blog.hesvh.cn/Article/details/gbpehuthg.sHtML

[R36] 并发执行多个任务
来源：http://wap.zdbjq.cn/Article/details/gpmieskdl.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://read.share.hesvh.cn/Article/details/gkxsxzclg.sHtML

[R37] 把输出赋给变量
来源：http://blog.fehbvm.com/Article/details/gtqzjxsfw.sHtML

files=$(ls -1)
来源：http://wap.zdbjq.cn/Article/details/gdumlfauz.sHtML

[R38] 管道串联
来源：http://www.share.zdbjq.cn/Article/details/gvvuijhjh.sHtML

cat a.txt | grep -i error | wc -l
来源：http://wap.zdbjq.cn/Article/details/gapwyjqto.sHtML

[R39] 重定向标准输出与错误
来源：http://blog.hesvh.cn/Article/details/ghhorozut.sHtML

cmd > out.log 2>&1
来源：http://mobile.fehbvm.com/Article/details/gauqsggob.sHtML

[R40] 追加写日志
来源：http://m.share.fehbvm.com/Article/details/gamncfxwh.sHtML

echo "log" >> out.log
来源：http://www.blog.fehbvm.com/Article/details/gddswualy.sHtML

[R41] 丢弃输出
来源：http://read.share.hesvh.cn/Article/details/gafvfghft.sHtML

cmd >/dev/null 2>&1
来源：http://wap.hesvh.cn/Article/details/gpwdlkzqr.sHtML

[R42] 输入重定向
来源：http://www.m.share.zdbjq.cn/Article/details/gjxjsaqar.sHtML

wc -l < a.txt
来源：http://m.share.fehbvm.com/Article/details/gabtoodvb.sHtML

[R43] 按名字查找文件
来源：http://wap.hesvh.cn/Article/details/gjyclbcpq.sHtML

find . -name "*.log" -type f
来源：http://read.share.hesvh.cn/Article/details/gwdnykdrt.sHtML

[R44] 按修改时间查找
来源：http://wap.hesvh.cn/Article/details/gjguptvvi.sHtML

find . -mtime -7 -type f
来源：http://wap.hesvh.cn/Article/details/gpjklkxkg.sHtML

[R45] 批量删除
来源：http://www.share.zdbjq.cn/Article/details/gaglkjcfm.sHtML

find . -name "*.tmp" -delete
来源：http://blog.hesvh.cn/Article/details/gjtbyhqny.sHtML

[R46] 递归替换文件内容
来源：http://wap.zdbjq.cn/Article/details/gfdkziqrg.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.zdbjq.cn/Article/details/goiqcbtfm.sHtML

[R47] sed 单行替换
来源：http://www.share.hesvh.cn/Article/details/gcopbibqk.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://3g.zdbjq.cn/Article/details/gcwnhgsuj.sHtML

[R48] awk 取指定列
来源：http://www.share.hesvh.cn/Article/details/guqqhwjpg.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/glndeztqr.sHtML

[R49] awk 带条件
来源：http://wap.hesvh.cn/Article/details/gifsuoahj.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.share.fehbvm.com/Article/details/gawfabztw.sHtML

[R50] awk 求和
来源：http://blog.zdbjq.cn/Article/details/gchyouerf.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gzoorhtbi.sHtML

[R51] 排序去重取前几
来源：http://www.blog.hesvh.cn/Article/details/ghehtmyeu.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.hesvh.cn/Article/details/gdbrevirb.sHtML

[R52] 统计行数
来源：http://www.blog.fehbvm.com/Article/details/gniodpnfo.sHtML

wc -l a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gokwfydvs.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.hesvh.cn/Article/details/gujtlolys.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.hesvh.cn/Article/details/gxwxylrfr.sHtML

[R54] 比较两个文件
来源：http://www.m.share.fehbvm.com/Article/details/ggbwycqmo.sHtML

diff a.txt b.txt
来源：http://3g.fehbvm.com/Article/details/gijbritaf.sHtML

[R55] 压缩与解压
来源：http://wap.hesvh.cn/Article/details/gvlzetwjc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.zdbjq.cn/Article/details/gjbdjrulz.sHtML

[R56] 远程拷贝
来源：http://blog.zdbjq.cn/Article/details/gpoycsjzy.sHtML

scp file user@host:/path/
来源：http://www.blog.zdbjq.cn/Article/details/gpljysspb.sHtML

[R57] 远程执行命令
来源：http://m.share.zdbjq.cn/Article/details/gtkisczda.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fehbvm.com/Article/details/gjilqpxim.sHtML

[R58] 下载文件
来源：http://blog.hesvh.cn/Article/details/gzvsmxqjv.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.fehbvm.com/Article/details/gruqjaapk.sHtML

[R59] 发 POST JSON
来源：http://wap.fehbvm.com/Article/details/gwbpofrxg.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fehbvm.com/Article/details/gcpngywow.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.hesvh.cn/Article/details/gibovkbbf.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.hesvh.cn/Article/details/gwjbprzcm.sHtML

[R61] 磁盘占用
来源：http://www.m.share.hesvh.cn/Article/details/gdbkhjqsj.sHtML

df -h;  du -sh *
来源：http://3g.hesvh.cn/Article/details/gcronypku.sHtML

[R62] 找最占空间的文件
来源：http://baike.fehbvm.com/Article/details/gwtcclano.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fehbvm.com/Article/details/gojjxmnee.sHtML

[R63] 内存与进程
来源：http://baike.fehbvm.com/Article/details/glapdrras.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.hesvh.cn/Article/details/geqnzylvv.sHtML

[R64] 结束进程
来源：http://read.share.zdbjq.cn/Article/details/gglezamzh.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.zdbjq.cn/Article/details/gprtxpksg.sHtML

[R65] 查看端口占用
来源：http://m.share.zdbjq.cn/Article/details/glxfgbwrp.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.zdbjq.cn/Article/details/gptshrwva.sHtML

[R66] 定时任务
来源：http://read.share.fehbvm.com/Article/details/gquxoapfm.sHtML

crontab -e;  crontab -l
来源：http://blog.hesvh.cn/Article/details/gsdhgzwov.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.hesvh.cn/Article/details/glgzuoapr.sHtML

openssl rand -hex 16
来源：http://www.m.share.fehbvm.com/Article/details/gudiopfvg.sHtML

[R68] 计算文件校验值
来源：http://wap.zdbjq.cn/Article/details/grfqyttwe.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.zdbjq.cn/Article/details/giakeiooo.sHtML

[R69] 生成随机密码
来源：http://read.share.hesvh.cn/Article/details/gejyszgfc.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.hesvh.cn/Article/details/geyzebusr.sHtML

[R70] 时间戳与互转
来源：http://3g.fehbvm.com/Article/details/gnohujvhz.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.hesvh.cn/Article/details/gaarhoivt.sHtML

[R71] 日期格式化
来源：http://3g.hesvh.cn/Article/details/gvvzccpsn.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.hesvh.cn/Article/details/gaaquvneq.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fehbvm.com/Article/details/gsjgahhwl.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.fehbvm.com/Article/details/gsxbzvwkb.sHtML

[R73] 分割大日志
来源：http://mobile.zdbjq.cn/Article/details/gbwpqbxnz.sHtML

split -l 1000 big.log part_
来源：http://3g.fehbvm.com/Article/details/gtssxswlz.sHtML

[R74] 批量重命名
来源：http://www.share.zdbjq.cn/Article/details/gxyovzgko.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.hesvh.cn/Article/details/gaxizjrpz.sHtML

[R75] 导出环境变量
来源：http://www.share.zdbjq.cn/Article/details/ggdsmddzm.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.hesvh.cn/Article/details/garimbigw.sHtML

[R76] 使用临时文件
来源：http://www.m.share.hesvh.cn/Article/details/gxbcgoaic.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.hesvh.cn/Article/details/gyumlgolm.sHtML

[R77] 读取用户输入
来源：http://m.share.fehbvm.com/Article/details/gdaxmyuhl.sHtML

read -rp "请输入: " ans
来源：http://3g.fehbvm.com/Article/details/grxkekmlh.sHtML

[R78] 交互式菜单
来源：http://blog.fehbvm.com/Article/details/giqomyuyf.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.zdbjq.cn/Article/details/gxbdiotfo.sHtML

[R79] 解析命令行选项
来源：http://www.share.zdbjq.cn/Article/details/gykwvrkat.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.zdbjq.cn/Article/details/giovleanb.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.zdbjq.cn/Article/details/gjkbaehgl.sHtML

time ./run.sh
来源：http://www.share.fehbvm.com/Article/details/gdpdihyll.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gqyytcwgo.sHtML

S. C / C++ 专题
来源：http://blog.zdbjq.cn/Article/details/gpwgoslzi.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gkdirdabn.sHtML

[S01] C：Hello World
来源：http://baike.zdbjq.cn/Article/details/gsyfnuuwk.sHtML

#include <stdio.h>
来源：http://www.blog.hesvh.cn/Article/details/gwjubfhts.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.zdbjq.cn/Article/details/gihonzqlk.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fehbvm.com/Article/details/gmaximdaq.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fehbvm.com/Article/details/grjrxyofr.sHtML

[S03] C：读入整数
来源：http://www.m.share.hesvh.cn/Article/details/gtatmnnqn.sHtML

int x; scanf("%d", &x);
来源：http://wap.hesvh.cn/Article/details/grpvdiddx.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fehbvm.com/Article/details/gxpuvufhf.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.hesvh.cn/Article/details/guewkuamh.sHtML

[S05] C：字符串长度
来源：http://3g.hesvh.cn/Article/details/gaeqtzbgj.sHtML

strlen(s)
来源：http://mobile.fehbvm.com/Article/details/gvldnuquj.sHtML

[S06] C：字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/gtnkydolk.sHtML

strcmp(a, b) == 0
来源：http://baike.fehbvm.com/Article/details/gtodajllf.sHtML

[S07] C：数组遍历求和
来源：http://blog.zdbjq.cn/Article/details/glwjdunwq.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.hesvh.cn/Article/details/gadayowtz.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fehbvm.com/Article/details/grdodnvom.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.hesvh.cn/Article/details/gdovhunnp.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.zdbjq.cn/Article/details/ginsnunrb.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fehbvm.com/Article/details/gdzfyziwp.sHtML

[S10] C：指针与解引用
来源：http://mobile.hesvh.cn/Article/details/ghzofcutn.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fehbvm.com/Article/details/gtvrjaaho.sHtML

[S11] C：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gibmbmdcf.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.hesvh.cn/Article/details/gxwbypkup.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.hesvh.cn/Article/details/gxhysapgn.sHtML

fclose(f);
来源：http://m.share.zdbjq.cn/Article/details/gxxezkkuq.sHtML

[S12] C：写文件
来源：http://www.share.zdbjq.cn/Article/details/gchmlulpa.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.zdbjq.cn/Article/details/gxtmewtek.sHtML

[S13] C：宏定义
来源：http://mobile.fehbvm.com/Article/details/gieyvmlmz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.hesvh.cn/Article/details/gpyltatpm.sHtML

[S14] C：枚举
来源：http://read.share.hesvh.cn/Article/details/gyaubcpbp.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.hesvh.cn/Article/details/gxypjnvis.sHtML

[S15] C：类型转换
来源：http://blog.fehbvm.com/Article/details/gfyjijkdg.sHtML

(double) a / b
来源：http://mobile.zdbjq.cn/Article/details/giyhosllf.sHtML

[S16] C：位操作置位
来源：http://read.share.fehbvm.com/Article/details/gxoagrvhw.sHtML

x |= (1 << 3);
来源：http://blog.zdbjq.cn/Article/details/gkskfjbny.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/grjakehhg.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.hesvh.cn/Article/details/gaymbaojx.sHtML

[S18] C：命令行参数
来源：http://wap.fehbvm.com/Article/details/gjhkerypz.sHtML

int main(int argc, char **argv)
来源：http://baike.hesvh.cn/Article/details/gpixshagy.sHtML

[S19] C：快速排序
来源：http://www.share.zdbjq.cn/Article/details/gxekobdlt.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.hesvh.cn/Article/details/ghrrpcsic.sHtML

[S20] C：二分查找
来源：http://baike.fehbvm.com/Article/details/gdcktkozl.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.zdbjq.cn/Article/details/gqhejgowb.sHtML

[S21] C：字符类别判断
来源：http://wap.zdbjq.cn/Article/details/ghupmocoo.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.zdbjq.cn/Article/details/gaujfcahk.sHtML

[S22] C：字符串转数字
来源：http://3g.zdbjq.cn/Article/details/gnudszfoo.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fehbvm.com/Article/details/gziuedjvr.sHtML

[S23] C：随机数
来源：http://www.share.hesvh.cn/Article/details/gtfoawzom.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.fehbvm.com/Article/details/ggsndjkyl.sHtML

[S24] C：获取本地时间
来源：http://blog.fehbvm.com/Article/details/gyrmdfdvr.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fehbvm.com/Article/details/gmdqzlrfq.sHtML

[S25] C：内存拷贝
来源：http://mobile.fehbvm.com/Article/details/gasvtmjmx.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fehbvm.com/Article/details/gonblbhay.sHtML

[S26] C：内存清零
来源：http://m.share.fehbvm.com/Article/details/gcfsobxqp.sHtML

memset(a, 0, sizeof a);
来源：http://3g.zdbjq.cn/Article/details/griuqqcsb.sHtML

[S27] C：定义常量
来源：http://www.blog.zdbjq.cn/Article/details/gactbkugn.sHtML

const double PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gajzuftnh.sHtML

[S28] C：静态变量
来源：http://mobile.fehbvm.com/Article/details/gdouesnaa.sHtML

static int counter = 0;
来源：http://3g.zdbjq.cn/Article/details/gltehnqqz.sHtML

[S29] C：变参函数
来源：http://www.share.fehbvm.com/Article/details/gwczpwkck.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.zdbjq.cn/Article/details/guzzqxutv.sHtML

[S30] C：头文件保护
来源：http://3g.fehbvm.com/Article/details/gzbhxwmgg.sHtML

#ifndef X_H
来源：http://www.m.share.zdbjq.cn/Article/details/gutxhbwkn.sHtML

#define X_H
来源：http://baike.fehbvm.com/Article/details/gllalnwzn.sHtML

#endif
来源：http://www.blog.zdbjq.cn/Article/details/giiwzjuqw.sHtML

[S31] C++：Hello World
来源：http://mobile.fehbvm.com/Article/details/geoupbnuh.sHtML

#include <iostream>
来源：http://baike.hesvh.cn/Article/details/gycececnj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gudaswscw.sHtML

[S32] C++：字符串
来源：http://read.share.zdbjq.cn/Article/details/grhdgfavj.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.hesvh.cn/Article/details/gdqviqtte.sHtML

[S33] C++：vector 增删
来源：http://wap.zdbjq.cn/Article/details/genaaiicm.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.zdbjq.cn/Article/details/gsjpdwntz.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.zdbjq.cn/Article/details/gvtpkavyr.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fehbvm.com/Article/details/gmgzilqln.sHtML

[S35] C++：map
来源：http://www.m.share.hesvh.cn/Article/details/gosxyxxun.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.zdbjq.cn/Article/details/gginhloud.sHtML

[S36] C++：unordered_map
来源：http://m.share.zdbjq.cn/Article/details/gztrimvqb.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.hesvh.cn/Article/details/gzuhstuia.sHtML

[S37] C++：set
来源：http://blog.hesvh.cn/Article/details/ghvunxgcx.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fehbvm.com/Article/details/gcuspvssg.sHtML

[S38] C++：排序
来源：http://m.share.hesvh.cn/Article/details/gmvtofgbr.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.hesvh.cn/Article/details/ghbzwhtcp.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.zdbjq.cn/Article/details/gyeyowkqp.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.hesvh.cn/Article/details/gjxliclou.sHtML

[S40] C++：查找元素
来源：http://www.m.share.fehbvm.com/Article/details/glzaucwjd.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.hesvh.cn/Article/details/gmtmwuscy.sHtML

[S41] C++：类与构造函数
来源：http://baike.fehbvm.com/Article/details/ggowmkmbj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.zdbjq.cn/Article/details/geejnjtns.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.hesvh.cn/Article/details/gxclrgtqk.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.hesvh.cn/Article/details/gqhqdfeak.sHtML

[S43] C++：智能指针
来源：http://wap.zdbjq.cn/Article/details/gcxaymhgw.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.zdbjq.cn/Article/details/gpfffksxy.sHtML

[S44] C++：引用传参
来源：http://www.share.fehbvm.com/Article/details/gyljshevg.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.hesvh.cn/Article/details/gwihsrylk.sHtML

[S45] C++：lambda
来源：http://m.share.zdbjq.cn/Article/details/gyfephcss.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.hesvh.cn/Article/details/gwbujewzc.sHtML

[S46] C++：函数模板
来源：http://read.share.hesvh.cn/Article/details/ghsjjehhi.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.hesvh.cn/Article/details/ghbtqdczp.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fehbvm.com/Article/details/gyqzdxesw.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.fehbvm.com/Article/details/glewvinza.sHtML

[S48] C++：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gohewmekt.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fehbvm.com/Article/details/gwwnglvzl.sHtML

while (std::getline(in, line)) { }
来源：http://blog.hesvh.cn/Article/details/glldaxnbx.sHtML

[S49] C++：写文件
来源：http://baike.zdbjq.cn/Article/details/ghbarjpnk.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://read.share.zdbjq.cn/Article/details/grydvdixh.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fehbvm.com/Article/details/gjgkkejvl.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.zdbjq.cn/Article/details/gatxxbioi.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fehbvm.com/Article/details/gdyxllytr.sHtML

static_cast<double>(a) / b
来源：http://read.share.zdbjq.cn/Article/details/golmkicqo.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.hesvh.cn/Article/details/gydavoajo.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.zdbjq.cn/Article/details/gqbnzqodw.sHtML

[S53] C++：移动语义
来源：http://www.share.fehbvm.com/Article/details/gatbklypz.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fehbvm.com/Article/details/gpxsmqgxc.sHtML

[S54] C++：异常处理
来源：http://blog.hesvh.cn/Article/details/gdgbbhwft.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.hesvh.cn/Article/details/gqoryfalf.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fehbvm.com/Article/details/gmikpkkzo.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.zdbjq.cn/Article/details/gyoxxqyae.sHtML

[S56] C++：optional
来源：http://read.share.hesvh.cn/Article/details/gfowmejoo.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fehbvm.com/Article/details/gbrhvthbl.sHtML

[S57] C++：编译期常量
来源：http://read.share.zdbjq.cn/Article/details/gizsjjrxd.sHtML

constexpr int N = 10;
来源：http://read.share.fehbvm.com/Article/details/ggxwglixt.sHtML

[S58] C++：命名空间
来源：http://www.share.zdbjq.cn/Article/details/gljgzpihn.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.zdbjq.cn/Article/details/gdpkqdagx.sHtML

[S59] C++：静态断言
来源：http://wap.zdbjq.cn/Article/details/gpttsikfu.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.hesvh.cn/Article/details/gbbsqppsk.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.hesvh.cn/Article/details/gtglfgoel.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.fehbvm.com/Article/details/gprysgpet.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gpbnevrrh.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fehbvm.com/Article/details/gglfeagpj.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/grvphbyst.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gvtofhpnu.sHtML

println("Hello")
来源：http://blog.zdbjq.cn/Article/details/gqqdfamng.sHtML

[T02] Kotlin：变量
来源：http://mobile.fehbvm.com/Article/details/gmchhurzv.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://3g.fehbvm.com/Article/details/giemmjeup.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.hesvh.cn/Article/details/gtwqhxhqm.sHtML

"值: $b"
来源：http://www.blog.zdbjq.cn/Article/details/gpcgqgfxa.sHtML

[T04] Kotlin：空安全
来源：http://wap.zdbjq.cn/Article/details/gmgcijuvs.sHtML

val n: String? = null;  n?.length
来源：http://3g.fehbvm.com/Article/details/gjqwslhiz.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fehbvm.com/Article/details/gwwsemgcv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fehbvm.com/Article/details/gagirpjag.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fehbvm.com/Article/details/gikwxzqqd.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/grsybrofy.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.hesvh.cn/Article/details/gmnatqutw.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.hesvh.cn/Article/details/griesexsu.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.hesvh.cn/Article/details/glkivhecc.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.hesvh.cn/Article/details/gfifbzcvh.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.zdbjq.cn/Article/details/gzonmyvyx.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.zdbjq.cn/Article/details/gemlgjpkm.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fehbvm.com/Article/details/gyrvmyjwt.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.hesvh.cn/Article/details/gpxxtcgie.sHtML

[T11] Kotlin：协程
来源：http://m.share.hesvh.cn/Article/details/geaesvssl.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.fehbvm.com/Article/details/grcvpuvwc.sHtML

[T12] Kotlin：解构声明
来源：http://baike.fehbvm.com/Article/details/gycqszkhn.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.zdbjq.cn/Article/details/gyjrolcqu.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.fehbvm.com/Article/details/gvkijtwfr.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fehbvm.com/Article/details/ghieztifk.sHtML

[T14] Kotlin：循环
来源：http://blog.fehbvm.com/Article/details/grsonxhlp.sHtML

for (i in 1..10) println(i)
来源：http://read.share.zdbjq.cn/Article/details/gseywdxoz.sHtML

[T15] Kotlin：接口
来源：http://3g.zdbjq.cn/Article/details/gmtcxmdvb.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.hesvh.cn/Article/details/gjngbjvzh.sHtML

[T16] Swift：Hello World
来源：http://www.share.fehbvm.com/Article/details/gucciizuj.sHtML

print("Hello")
来源：http://baike.hesvh.cn/Article/details/guztzzzay.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.zdbjq.cn/Article/details/gqwudoyzm.sHtML

var a = 1;  let b = 2
来源：http://wap.zdbjq.cn/Article/details/gqzevowzp.sHtML

[T18] Swift：字符串插值
来源：http://mobile.fehbvm.com/Article/details/gwwmkidwl.sHtML

"值: \(b)"
来源：http://www.share.hesvh.cn/Article/details/gvvjipive.sHtML

[T19] Swift：可选绑定
来源：http://baike.hesvh.cn/Article/details/gcctvpofs.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.hesvh.cn/Article/details/gtkexpcco.sHtML

[T20] Swift：数组操作
来源：http://read.share.fehbvm.com/Article/details/ggxpoizdy.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.hesvh.cn/Article/details/ggnxknwrc.sHtML

[T21] Swift：遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gwqdfinhp.sHtML

for x in a { print(x) }
来源：http://www.blog.hesvh.cn/Article/details/geigdysmt.sHtML

[T22] Swift：字典
来源：http://mobile.zdbjq.cn/Article/details/ganczywfa.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.hesvh.cn/Article/details/ggduiahkf.sHtML

[T23] Swift：函数
来源：http://www.m.share.hesvh.cn/Article/details/gpcaygxqa.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.hesvh.cn/Article/details/getkllbfz.sHtML

[T24] Swift：闭包
来源：http://read.share.zdbjq.cn/Article/details/gqinjarnj.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.fehbvm.com/Article/details/ghkgqrwlp.sHtML

[T25] Swift：结构体
来源：http://baike.hesvh.cn/Article/details/gkhlbmgun.sHtML

struct P { var x: Int }
来源：http://blog.fehbvm.com/Article/details/gaskfisvd.sHtML

[T26] Swift：类与重写
来源：http://blog.zdbjq.cn/Article/details/gkzbpxvfx.sHtML

class A: Base { override func f() {} }
来源：http://m.share.hesvh.cn/Article/details/glzmsczem.sHtML

[T27] Swift：错误处理
来源：http://www.blog.fehbvm.com/Article/details/grxeqgcvi.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.zdbjq.cn/Article/details/gthflwdjw.sHtML

[T28] Swift：枚举
来源：http://baike.hesvh.cn/Article/details/gevkngywf.sHtML

enum Color { case red, green }
来源：http://blog.fehbvm.com/Article/details/gngrprmeb.sHtML


<!-- 参考信息 -->