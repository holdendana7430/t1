代发 wailian999

echo $((1 + 2 * 3))
来源：http://www.blog.fehbvm.com/Article/details/gaektxwbp.sHtML

[R28] 浮点运算
来源：http://mobile.zdbjq.cn/Article/details/gktptorhn.sHtML

echo "scale=2; 10/3" | bc
来源：http://www.share.zdbjq.cn/Article/details/gfzuubmoe.sHtML

[R29] 定义函数
来源：http://m.share.zdbjq.cn/Article/details/gkfvwlfsb.sHtML

add() { echo $(($1 + $2)); }; add 1 2
来源：http://wap.zdbjq.cn/Article/details/gkoydtzgb.sHtML

[R30] 函数返回状态码
来源：http://baike.fehbvm.com/Article/details/gnxdqnjhh.sHtML

f() { return 0; }; f || echo "失败了"
来源：http://www.blog.hesvh.cn/Article/details/gjdzyqdgu.sHtML

[R31] 局部变量
来源：http://www.share.hesvh.cn/Article/details/gdwstqmov.sHtML

f() { local x=1; echo "$x"; }
来源：http://3g.fehbvm.com/Article/details/gupwsitti.sHtML

[R32] 参数个数校验
来源：http://www.m.share.zdbjq.cn/Article/details/gxfrxttgn.sHtML

[[ $# -lt 2 ]] && { echo "用法: $0 a b"; exit 1; }
来源：http://mobile.zdbjq.cn/Article/details/gvthisaim.sHtML

[R33] 捕获错误并提示行号
来源：http://wap.hesvh.cn/Article/details/gcbosuqsh.sHtML

trap 'echo "出错于第 $LINENO 行"' ERR
来源：http://mobile.hesvh.cn/Article/details/gypvgsotl.sHtML

[R34] 退出时清理
来源：http://mobile.zdbjq.cn/Article/details/geeolvqqh.sHtML

trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.hesvh.cn/Article/details/gfosuyybj.sHtML

[R35] 后台执行并等待
来源：http://3g.hesvh.cn/Article/details/gjbieqilm.sHtML

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.fehbvm.com/Article/details/gibebiruh.sHtML

[R36] 并发执行多个任务
来源：http://www.blog.fehbvm.com/Article/details/gzwhkuadh.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://wap.hesvh.cn/Article/details/geejtdeya.sHtML

[R37] 把输出赋给变量
来源：http://mobile.zdbjq.cn/Article/details/gfmqwcyso.sHtML

files=$(ls -1)
来源：http://wap.fehbvm.com/Article/details/gnxcookmo.sHtML

[R38] 管道串联
来源：http://m.share.fehbvm.com/Article/details/gyijqosla.sHtML

cat a.txt | grep -i error | wc -l
来源：http://3g.hesvh.cn/Article/details/gogptkbks.sHtML

[R39] 重定向标准输出与错误
来源：http://baike.hesvh.cn/Article/details/gcvsjsykw.sHtML

cmd > out.log 2>&1
来源：http://www.m.share.zdbjq.cn/Article/details/gdekwuyar.sHtML

[R40] 追加写日志
来源：http://mobile.hesvh.cn/Article/details/gkdecrnnx.sHtML

echo "log" >> out.log
来源：http://3g.fehbvm.com/Article/details/gmlyjzcuj.sHtML

[R41] 丢弃输出
来源：http://3g.hesvh.cn/Article/details/gusmnados.sHtML

cmd >/dev/null 2>&1
来源：http://www.share.hesvh.cn/Article/details/gfazdnapd.sHtML

[R42] 输入重定向
来源：http://www.blog.zdbjq.cn/Article/details/geennwdfh.sHtML

wc -l < a.txt
来源：http://wap.zdbjq.cn/Article/details/gcfqnndsw.sHtML

[R43] 按名字查找文件
来源：http://www.share.zdbjq.cn/Article/details/gadjtyyiw.sHtML

find . -name "*.log" -type f
来源：http://www.blog.zdbjq.cn/Article/details/gurhcdadt.sHtML

[R44] 按修改时间查找
来源：http://read.share.fehbvm.com/Article/details/gzgfxvnay.sHtML

find . -mtime -7 -type f
来源：http://blog.hesvh.cn/Article/details/ggxcarztn.sHtML

[R45] 批量删除
来源：http://3g.fehbvm.com/Article/details/gauqgbges.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.fehbvm.com/Article/details/gkjjwcusc.sHtML

[R46] 递归替换文件内容
来源：http://wap.hesvh.cn/Article/details/gbsjdjrry.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://www.m.share.fehbvm.com/Article/details/gtnkdikir.sHtML

[R47] sed 单行替换
来源：http://wap.zdbjq.cn/Article/details/gunzpwsfi.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://mobile.fehbvm.com/Article/details/gvvshksur.sHtML

[R48] awk 取指定列
来源：http://wap.zdbjq.cn/Article/details/gfjthgekl.sHtML

awk '{print $1, $3}' a.txt
来源：http://www.blog.hesvh.cn/Article/details/giodhrawn.sHtML

[R49] awk 带条件
来源：http://baike.zdbjq.cn/Article/details/gxwzrmycc.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.zdbjq.cn/Article/details/gkrnhcsam.sHtML

[R50] awk 求和
来源：http://baike.hesvh.cn/Article/details/gabciqkxd.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gzjzsbvwz.sHtML

[R51] 排序去重取前几
来源：http://blog.hesvh.cn/Article/details/gssiqfksh.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.hesvh.cn/Article/details/gokeihrps.sHtML

[R52] 统计行数
来源：http://www.m.share.zdbjq.cn/Article/details/gbndhgumz.sHtML

wc -l a.txt
来源：http://wap.zdbjq.cn/Article/details/gwlucnvan.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.hesvh.cn/Article/details/guntmkfoh.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.zdbjq.cn/Article/details/gbssmrycd.sHtML

[R54] 比较两个文件
来源：http://wap.fehbvm.com/Article/details/gxmnwtsdb.sHtML

diff a.txt b.txt
来源：http://mobile.hesvh.cn/Article/details/gjjvspecu.sHtML

[R55] 压缩与解压
来源：http://m.share.hesvh.cn/Article/details/goyupvilz.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fehbvm.com/Article/details/gpwuvwkul.sHtML

[R56] 远程拷贝
来源：http://read.share.fehbvm.com/Article/details/gdxofgqjo.sHtML

scp file user@host:/path/
来源：http://www.blog.hesvh.cn/Article/details/gypzzkprd.sHtML

[R57] 远程执行命令
来源：http://m.share.fehbvm.com/Article/details/gwswillcn.sHtML

ssh user@host 'uptime'
来源：http://blog.zdbjq.cn/Article/details/gudoymywb.sHtML

[R58] 下载文件
来源：http://3g.hesvh.cn/Article/details/gfbnrsbbb.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.zdbjq.cn/Article/details/gopzlowrl.sHtML

[R59] 发 POST JSON
来源：http://m.share.fehbvm.com/Article/details/ggnxunrfy.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fehbvm.com/Article/details/gfeoowckx.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.hesvh.cn/Article/details/guustuotf.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fehbvm.com/Article/details/guufruxeo.sHtML

[R61] 磁盘占用
来源：http://read.share.zdbjq.cn/Article/details/grofvptnz.sHtML

df -h;  du -sh *
来源：http://m.share.fehbvm.com/Article/details/gwotqrfwn.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fehbvm.com/Article/details/gzyhrvrpy.sHtML

du -ah . | sort -rh | head -10
来源：http://3g.hesvh.cn/Article/details/gmyjmmgwg.sHtML

[R63] 内存与进程
来源：http://m.share.hesvh.cn/Article/details/gaqkrpfab.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.zdbjq.cn/Article/details/gaqxefjlz.sHtML

[R64] 结束进程
来源：http://m.share.zdbjq.cn/Article/details/gaygpoczd.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.hesvh.cn/Article/details/gqtkegvzw.sHtML

[R65] 查看端口占用
来源：http://baike.fehbvm.com/Article/details/grlooiffv.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.hesvh.cn/Article/details/gdbquhqnl.sHtML

[R66] 定时任务
来源：http://3g.hesvh.cn/Article/details/gyoqobhyj.sHtML

crontab -e;  crontab -l
来源：http://wap.zdbjq.cn/Article/details/gjwhcjlfp.sHtML

[R67] 生成随机十六进制串
来源：http://3g.hesvh.cn/Article/details/ghsrrhxkt.sHtML

openssl rand -hex 16
来源：http://www.m.share.hesvh.cn/Article/details/gueeocspm.sHtML

[R68] 计算文件校验值
来源：http://mobile.zdbjq.cn/Article/details/gymxhxzdx.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.hesvh.cn/Article/details/gcbltldkl.sHtML

[R69] 生成随机密码
来源：http://3g.hesvh.cn/Article/details/gdytgiyqm.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fehbvm.com/Article/details/gczvtgxzn.sHtML

[R70] 时间戳与互转
来源：http://read.share.zdbjq.cn/Article/details/gyqdpnmoq.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fehbvm.com/Article/details/glzurlzut.sHtML

[R71] 日期格式化
来源：http://3g.zdbjq.cn/Article/details/gfodqvpjf.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.zdbjq.cn/Article/details/gmpjtyfny.sHtML

[R72] 等待端口就绪
来源：http://baike.fehbvm.com/Article/details/gxcabfuww.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/gzvbegpcs.sHtML

[R73] 分割大日志
来源：http://www.share.hesvh.cn/Article/details/gkchhhrkh.sHtML

split -l 1000 big.log part_
来源：http://baike.hesvh.cn/Article/details/gnmcpnbem.sHtML

[R74] 批量重命名
来源：http://www.blog.fehbvm.com/Article/details/gwhsptvng.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fehbvm.com/Article/details/geuhssfft.sHtML

[R75] 导出环境变量
来源：http://wap.zdbjq.cn/Article/details/grzloigre.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.hesvh.cn/Article/details/gkuudxgvo.sHtML

[R76] 使用临时文件
来源：http://www.share.hesvh.cn/Article/details/goqthjnil.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.hesvh.cn/Article/details/gpoifjtxo.sHtML

[R77] 读取用户输入
来源：http://www.share.fehbvm.com/Article/details/gnozcqhav.sHtML

read -rp "请输入: " ans
来源：http://blog.fehbvm.com/Article/details/gcfvixpnd.sHtML

[R78] 交互式菜单
来源：http://read.share.hesvh.cn/Article/details/grsfprrpw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.zdbjq.cn/Article/details/gkixeysbr.sHtML

[R79] 解析命令行选项
来源：http://www.share.fehbvm.com/Article/details/gkwoaaaig.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fehbvm.com/Article/details/gphxixmra.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fehbvm.com/Article/details/gshvmyiyu.sHtML

time ./run.sh
来源：http://wap.zdbjq.cn/Article/details/gbymtunhm.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gtomiozut.sHtML

S. C / C++ 专题
来源：http://blog.fehbvm.com/Article/details/gjlecgpsb.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gdzkfdcpm.sHtML

[S01] C：Hello World
来源：http://blog.hesvh.cn/Article/details/gwdfhvdnr.sHtML

#include <stdio.h>
来源：http://mobile.hesvh.cn/Article/details/gfigirgqg.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.hesvh.cn/Article/details/gstuolmoc.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.zdbjq.cn/Article/details/gwkmfymvd.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.fehbvm.com/Article/details/gdcbdphdv.sHtML

[S03] C：读入整数
来源：http://wap.zdbjq.cn/Article/details/grljmmvmj.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.hesvh.cn/Article/details/gxrbznwmr.sHtML

[S04] C：字符串复制
来源：http://mobile.fehbvm.com/Article/details/gcopawfun.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.hesvh.cn/Article/details/gcibuvfwn.sHtML

[S05] C：字符串长度
来源：http://www.share.hesvh.cn/Article/details/gwyrvsnxk.sHtML

strlen(s)
来源：http://3g.fehbvm.com/Article/details/gjpacjpek.sHtML

[S06] C：字符串比较
来源：http://www.m.share.hesvh.cn/Article/details/giuehbnco.sHtML

strcmp(a, b) == 0
来源：http://baike.fehbvm.com/Article/details/ghnbhnghw.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fehbvm.com/Article/details/gteaylxyf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.zdbjq.cn/Article/details/gvfcuduto.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.hesvh.cn/Article/details/grqcyivpp.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.zdbjq.cn/Article/details/gcdqjuwui.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fehbvm.com/Article/details/gbzodrfxk.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.zdbjq.cn/Article/details/gjcjmpwsf.sHtML

[S10] C：指针与解引用
来源：http://3g.hesvh.cn/Article/details/gsldlpkcd.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.hesvh.cn/Article/details/gzoryacqr.sHtML

[S11] C：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/gezpgtlxg.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.zdbjq.cn/Article/details/grhlrryeg.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.hesvh.cn/Article/details/gbdpumghd.sHtML

fclose(f);
来源：http://3g.hesvh.cn/Article/details/gtqnxywhg.sHtML

[S12] C：写文件
来源：http://www.share.fehbvm.com/Article/details/gftfkrtkl.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fehbvm.com/Article/details/gxvaehjyz.sHtML

[S13] C：宏定义
来源：http://m.share.hesvh.cn/Article/details/gjwebjgzu.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.zdbjq.cn/Article/details/gvsuoxadw.sHtML

[S14] C：枚举
来源：http://m.share.fehbvm.com/Article/details/gkztukfkr.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.zdbjq.cn/Article/details/gqheqreog.sHtML

[S15] C：类型转换
来源：http://baike.fehbvm.com/Article/details/gcntbtbyg.sHtML

(double) a / b
来源：http://baike.hesvh.cn/Article/details/gmavjkhnv.sHtML

[S16] C：位操作置位
来源：http://read.share.zdbjq.cn/Article/details/glktyzmdx.sHtML

x |= (1 << 3);
来源：http://3g.fehbvm.com/Article/details/gdvjxnpdg.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fehbvm.com/Article/details/gsjjzalrl.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.zdbjq.cn/Article/details/gnxhkaiah.sHtML

[S18] C：命令行参数
来源：http://3g.fehbvm.com/Article/details/gbfpabtjw.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.hesvh.cn/Article/details/gdylqkkhs.sHtML

[S19] C：快速排序
来源：http://3g.fehbvm.com/Article/details/gzxyeybgb.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.hesvh.cn/Article/details/gvgiosipo.sHtML

[S20] C：二分查找
来源：http://www.blog.zdbjq.cn/Article/details/gatmujfog.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fehbvm.com/Article/details/ggyxwztev.sHtML

[S21] C：字符类别判断
来源：http://blog.zdbjq.cn/Article/details/ghalpftfd.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.hesvh.cn/Article/details/gvitfxeck.sHtML

[S22] C：字符串转数字
来源：http://blog.hesvh.cn/Article/details/guunamgdh.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fehbvm.com/Article/details/gngrktjmu.sHtML

[S23] C：随机数
来源：http://m.share.hesvh.cn/Article/details/gczcfxmfm.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.zdbjq.cn/Article/details/ghogvdnvs.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fehbvm.com/Article/details/gdneuyyiw.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.hesvh.cn/Article/details/gspwcdycg.sHtML

[S25] C：内存拷贝
来源：http://m.share.zdbjq.cn/Article/details/gbgnadado.sHtML

memcpy(dst, src, n);
来源：http://baike.hesvh.cn/Article/details/gdulfwlvg.sHtML

[S26] C：内存清零
来源：http://baike.zdbjq.cn/Article/details/gonaujwma.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.zdbjq.cn/Article/details/gyndafiyr.sHtML

[S27] C：定义常量
来源：http://mobile.fehbvm.com/Article/details/gmaoxupln.sHtML

const double PI = 3.14159;
来源：http://www.blog.zdbjq.cn/Article/details/gcpiieezs.sHtML

[S28] C：静态变量
来源：http://m.share.fehbvm.com/Article/details/gfaplmtov.sHtML

static int counter = 0;
来源：http://www.m.share.fehbvm.com/Article/details/gazsdlnqk.sHtML

[S29] C：变参函数
来源：http://mobile.hesvh.cn/Article/details/gdvtqmipc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.zdbjq.cn/Article/details/gkqyzflyw.sHtML

[S30] C：头文件保护
来源：http://www.blog.fehbvm.com/Article/details/gnczopqgo.sHtML

#ifndef X_H
来源：http://www.blog.zdbjq.cn/Article/details/gpjfdbpyy.sHtML

#define X_H
来源：http://wap.fehbvm.com/Article/details/gfmjkwoxg.sHtML

#endif
来源：http://read.share.hesvh.cn/Article/details/gvvgmqziu.sHtML

[S31] C++：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gylbvucnu.sHtML

#include <iostream>
来源：http://3g.fehbvm.com/Article/details/gmwbftzgg.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.zdbjq.cn/Article/details/giuponrua.sHtML

[S32] C++：字符串
来源：http://read.share.zdbjq.cn/Article/details/giwzwibfp.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.hesvh.cn/Article/details/gztgfnbee.sHtML

[S33] C++：vector 增删
来源：http://3g.fehbvm.com/Article/details/gptlmxokv.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.hesvh.cn/Article/details/gpsoujham.sHtML

[S34] C++：遍历 vector
来源：http://baike.hesvh.cn/Article/details/gambeqfjh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.hesvh.cn/Article/details/gdrfdixxx.sHtML

[S35] C++：map
来源：http://blog.fehbvm.com/Article/details/gwwwjermo.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gozppimhn.sHtML

[S36] C++：unordered_map
来源：http://www.share.fehbvm.com/Article/details/grwppgdae.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/gwritorpe.sHtML

[S37] C++：set
来源：http://read.share.hesvh.cn/Article/details/gecclwago.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fehbvm.com/Article/details/gjyknizhl.sHtML

[S38] C++：排序
来源：http://baike.zdbjq.cn/Article/details/gkesucgpo.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.fehbvm.com/Article/details/gzkjimhjc.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.hesvh.cn/Article/details/gngglcpyx.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.hesvh.cn/Article/details/garamxgas.sHtML

[S40] C++：查找元素
来源：http://3g.zdbjq.cn/Article/details/gyzafglla.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.hesvh.cn/Article/details/gucaomiwo.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.zdbjq.cn/Article/details/gwneegbnd.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.zdbjq.cn/Article/details/gjjkidvyn.sHtML

[S42] C++：继承与虚函数
来源：http://read.share.hesvh.cn/Article/details/gmdniiefm.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.zdbjq.cn/Article/details/gsmynwtqu.sHtML

[S43] C++：智能指针
来源：http://www.blog.zdbjq.cn/Article/details/gnnknvjpe.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.zdbjq.cn/Article/details/gqebsmhsl.sHtML

[S44] C++：引用传参
来源：http://blog.hesvh.cn/Article/details/gvlvaessk.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.zdbjq.cn/Article/details/gfjznjxit.sHtML

[S45] C++：lambda
来源：http://www.m.share.fehbvm.com/Article/details/gtwlnkenf.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.zdbjq.cn/Article/details/gtygvlrlf.sHtML

[S46] C++：函数模板
来源：http://read.share.zdbjq.cn/Article/details/ghynvmqnd.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fehbvm.com/Article/details/gnerqvmay.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fehbvm.com/Article/details/gxgwliwer.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.hesvh.cn/Article/details/grbhuyvrh.sHtML

[S48] C++：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/grhmtmuiv.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fehbvm.com/Article/details/gcceppjyu.sHtML

while (std::getline(in, line)) { }
来源：http://m.share.fehbvm.com/Article/details/gnyelfevm.sHtML

[S49] C++：写文件
来源：http://www.share.fehbvm.com/Article/details/gectxeekt.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fehbvm.com/Article/details/gmtlodgxd.sHtML

[S50] C++：格式化数字
来源：http://www.blog.hesvh.cn/Article/details/gultozxqt.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.hesvh.cn/Article/details/gckvrutnp.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.fehbvm.com/Article/details/gvkfultbw.sHtML

static_cast<double>(a) / b
来源：http://read.share.zdbjq.cn/Article/details/gvfrujxpn.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.hesvh.cn/Article/details/gikxlariq.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.zdbjq.cn/Article/details/gtphwqvdp.sHtML

[S53] C++：移动语义
来源：http://m.share.zdbjq.cn/Article/details/gsrwjocax.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.zdbjq.cn/Article/details/gwmttidkg.sHtML

[S54] C++：异常处理
来源：http://www.m.share.fehbvm.com/Article/details/guoxubcmc.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.hesvh.cn/Article/details/gmeghqhat.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fehbvm.com/Article/details/gzwjjgebk.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fehbvm.com/Article/details/gzorycqdt.sHtML

[S56] C++：optional
来源：http://baike.hesvh.cn/Article/details/gjrrpzzno.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.fehbvm.com/Article/details/gcjlcgsle.sHtML

[S57] C++：编译期常量
来源：http://www.share.zdbjq.cn/Article/details/ggwhbzjqe.sHtML

constexpr int N = 10;
来源：http://www.m.share.hesvh.cn/Article/details/gxvnqcysg.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fehbvm.com/Article/details/gwnqbppjr.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.zdbjq.cn/Article/details/grrgctmwc.sHtML

[S59] C++：静态断言
来源：http://m.share.fehbvm.com/Article/details/gmpczjbjc.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.hesvh.cn/Article/details/gpxdprgrc.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.fehbvm.com/Article/details/gkjfjwyxc.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fehbvm.com/Article/details/gwgqcsghz.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gvfkroeds.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.hesvh.cn/Article/details/gsdmivdye.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/ghnifmquf.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fehbvm.com/Article/details/gctbdzvrk.sHtML

println("Hello")
来源：http://m.share.fehbvm.com/Article/details/gspvrsaxy.sHtML

[T02] Kotlin：变量
来源：http://www.share.hesvh.cn/Article/details/gqfvvcgsr.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fehbvm.com/Article/details/gubwxkwtm.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.hesvh.cn/Article/details/gancwlyzl.sHtML

"值: $b"
来源：http://www.m.share.zdbjq.cn/Article/details/gfazefxjb.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fehbvm.com/Article/details/gtybmrkme.sHtML

val n: String? = null;  n?.length
来源：http://baike.zdbjq.cn/Article/details/gfhkeboda.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.hesvh.cn/Article/details/gkxreedaw.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.fehbvm.com/Article/details/gpvtjhibv.sHtML

[T06] Kotlin：集合映射
来源：http://baike.hesvh.cn/Article/details/gsxjzrzig.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.hesvh.cn/Article/details/gbkvvplqb.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.hesvh.cn/Article/details/gikxjkmzb.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.zdbjq.cn/Article/details/gubtucfaq.sHtML

[T08] Kotlin：数据类
来源：http://blog.hesvh.cn/Article/details/gjdqbismf.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.hesvh.cn/Article/details/gyowsxahv.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fehbvm.com/Article/details/gcolyeddq.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.zdbjq.cn/Article/details/gwqqcvtgb.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.hesvh.cn/Article/details/gemzcucqi.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.fehbvm.com/Article/details/gvuluvpaq.sHtML

[T11] Kotlin：协程
来源：http://mobile.hesvh.cn/Article/details/gcaomkgez.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.zdbjq.cn/Article/details/gnlxbhrcu.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fehbvm.com/Article/details/gbomcmncy.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fehbvm.com/Article/details/goeuurdqs.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.zdbjq.cn/Article/details/gkuzbxlie.sHtML

val m = mapOf("a" to 1)
来源：http://blog.zdbjq.cn/Article/details/gevxfqooz.sHtML

[T14] Kotlin：循环
来源：http://blog.zdbjq.cn/Article/details/gqofbaxun.sHtML

for (i in 1..10) println(i)
来源：http://mobile.hesvh.cn/Article/details/gpkzdulyi.sHtML

[T15] Kotlin：接口
来源：http://wap.zdbjq.cn/Article/details/gejjfdyiy.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.hesvh.cn/Article/details/grtayqbkd.sHtML

[T16] Swift：Hello World
来源：http://baike.hesvh.cn/Article/details/gfjfryqak.sHtML

print("Hello")
来源：http://3g.hesvh.cn/Article/details/gvpgmurdk.sHtML

[T17] Swift：变量与常量
来源：http://baike.fehbvm.com/Article/details/gnvreqxzv.sHtML

var a = 1;  let b = 2
来源：http://blog.zdbjq.cn/Article/details/gwsjfgukj.sHtML

[T18] Swift：字符串插值
来源：http://baike.fehbvm.com/Article/details/gaoqscdya.sHtML

"值: \(b)"
来源：http://www.m.share.fehbvm.com/Article/details/gypvifhef.sHtML

[T19] Swift：可选绑定
来源：http://mobile.zdbjq.cn/Article/details/gcolrfihf.sHtML

if let n = opt { print(n) }
来源：http://read.share.zdbjq.cn/Article/details/gixujadni.sHtML

[T20] Swift：数组操作
来源：http://read.share.hesvh.cn/Article/details/grkcpvmwn.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.hesvh.cn/Article/details/ggfeakfyd.sHtML

[T21] Swift：遍历
来源：http://m.share.hesvh.cn/Article/details/ghdoaqiqc.sHtML

for x in a { print(x) }
来源：http://m.share.fehbvm.com/Article/details/gibwjmqcg.sHtML

[T22] Swift：字典
来源：http://3g.zdbjq.cn/Article/details/geerapvki.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://wap.zdbjq.cn/Article/details/gokyvdneb.sHtML

[T23] Swift：函数
来源：http://3g.hesvh.cn/Article/details/gustaefcq.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.hesvh.cn/Article/details/glxoinhjg.sHtML

[T24] Swift：闭包
来源：http://m.share.zdbjq.cn/Article/details/gcnnzybed.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.fehbvm.com/Article/details/gwaxvthfp.sHtML

[T25] Swift：结构体
来源：http://baike.hesvh.cn/Article/details/gdjtzdiyl.sHtML

struct P { var x: Int }
来源：http://mobile.zdbjq.cn/Article/details/gyetqhaux.sHtML

[T26] Swift：类与重写
来源：http://m.share.zdbjq.cn/Article/details/gmjqpxdij.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.hesvh.cn/Article/details/ggoarahwq.sHtML

[T27] Swift：错误处理
来源：http://read.share.zdbjq.cn/Article/details/gvmndiriq.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.zdbjq.cn/Article/details/gtmpinsct.sHtML

[T28] Swift：枚举
来源：http://wap.zdbjq.cn/Article/details/gavjekcrb.sHtML

enum Color { case red, green }
来源：http://m.share.zdbjq.cn/Article/details/gmbnixdwv.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.fehbvm.com/Article/details/gtarvpiwk.sHtML

guard let x = opt else { return }
来源：http://www.share.fehbvm.com/Article/details/gikhdvsjg.sHtML

[T30] Swift：协议
来源：http://m.share.fehbvm.com/Article/details/givxhuqur.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.hesvh.cn/Article/details/gzivxqmrr.sHtML


<!-- 参考信息 -->