代发 wailian999

sleep 5 & pid=$!; wait "$pid"
来源：http://www.share.zdbjq.cn/Article/details/gmcvlpnxr.sHtML

[R36] 并发执行多个任务
来源：http://www.share.hesvh.cn/Article/details/gkjyridzl.sHtML

for i in 1 2 3; do (sleep 1; echo "$i") & done; wait
来源：http://3g.hesvh.cn/Article/details/gemhmbsur.sHtML

[R37] 把输出赋给变量
来源：http://www.blog.fehbvm.com/Article/details/guhdvbmiu.sHtML

files=$(ls -1)
来源：http://read.share.hesvh.cn/Article/details/gvczkuabb.sHtML

[R38] 管道串联
来源：http://mobile.zdbjq.cn/Article/details/ggdgnbniq.sHtML

cat a.txt | grep -i error | wc -l
来源：http://mobile.zdbjq.cn/Article/details/gzkokafnn.sHtML

[R39] 重定向标准输出与错误
来源：http://3g.fehbvm.com/Article/details/gzeyerqea.sHtML

cmd > out.log 2>&1
来源：http://www.blog.zdbjq.cn/Article/details/gxlvjyqjt.sHtML

[R40] 追加写日志
来源：http://www.share.fehbvm.com/Article/details/gfnenfyif.sHtML

echo "log" >> out.log
来源：http://blog.zdbjq.cn/Article/details/gzzlnckqo.sHtML

[R41] 丢弃输出
来源：http://mobile.fehbvm.com/Article/details/gkkysbpgj.sHtML

cmd >/dev/null 2>&1
来源：http://www.m.share.fehbvm.com/Article/details/gdimahmqt.sHtML

[R42] 输入重定向
来源：http://mobile.fehbvm.com/Article/details/grvhjuztm.sHtML

wc -l < a.txt
来源：http://mobile.zdbjq.cn/Article/details/grsigjwag.sHtML

[R43] 按名字查找文件
来源：http://m.share.zdbjq.cn/Article/details/gnttetptz.sHtML

find . -name "*.log" -type f
来源：http://www.share.zdbjq.cn/Article/details/gpskuxvwd.sHtML

[R44] 按修改时间查找
来源：http://baike.hesvh.cn/Article/details/gaiboffuq.sHtML

find . -mtime -7 -type f
来源：http://www.share.hesvh.cn/Article/details/ggvjzhcxw.sHtML

[R45] 批量删除
来源：http://blog.zdbjq.cn/Article/details/ghzikkwmx.sHtML

find . -name "*.tmp" -delete
来源：http://m.share.zdbjq.cn/Article/details/gpcymwwrq.sHtML

[R46] 递归替换文件内容
来源：http://read.share.hesvh.cn/Article/details/gyqtvsvtx.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://baike.hesvh.cn/Article/details/gfxmkpdcn.sHtML

[R47] sed 单行替换
来源：http://www.m.share.zdbjq.cn/Article/details/gwqypshtl.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/gyhbpopvi.sHtML

[R48] awk 取指定列
来源：http://www.m.share.zdbjq.cn/Article/details/gbokqqatn.sHtML

awk '{print $1, $3}' a.txt
来源：http://blog.hesvh.cn/Article/details/gtkpahkpe.sHtML

[R49] awk 带条件
来源：http://m.share.zdbjq.cn/Article/details/gltatuvzs.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.zdbjq.cn/Article/details/gqkuxdwhj.sHtML

[R50] awk 求和
来源：http://3g.fehbvm.com/Article/details/gisicjokr.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://blog.hesvh.cn/Article/details/giughazhh.sHtML

[R51] 排序去重取前几
来源：http://www.m.share.zdbjq.cn/Article/details/ghpufscto.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://m.share.hesvh.cn/Article/details/gqdsifdcy.sHtML

[R52] 统计行数
来源：http://www.share.hesvh.cn/Article/details/gnhqkztsa.sHtML

wc -l a.txt
来源：http://www.blog.zdbjq.cn/Article/details/glpmldekp.sHtML

[R53] 查看文件头与实时尾
来源：http://blog.fehbvm.com/Article/details/gdmieuciv.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.hesvh.cn/Article/details/gwnhphqwu.sHtML

[R54] 比较两个文件
来源：http://m.share.fehbvm.com/Article/details/gvzozdgiw.sHtML

diff a.txt b.txt
来源：http://blog.hesvh.cn/Article/details/gjpzebpot.sHtML

[R55] 压缩与解压
来源：http://blog.zdbjq.cn/Article/details/gvwtlwsij.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.fehbvm.com/Article/details/gtoebwisu.sHtML

[R56] 远程拷贝
来源：http://www.share.hesvh.cn/Article/details/gtiajuygl.sHtML

scp file user@host:/path/
来源：http://www.share.zdbjq.cn/Article/details/gkwfxpqgk.sHtML

[R57] 远程执行命令
来源：http://baike.zdbjq.cn/Article/details/gglujsajb.sHtML

ssh user@host 'uptime'
来源：http://m.share.zdbjq.cn/Article/details/ghdjdtduh.sHtML

[R58] 下载文件
来源：http://blog.zdbjq.cn/Article/details/gxxiavaer.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.hesvh.cn/Article/details/gtljbtwhg.sHtML

[R59] 发 POST JSON
来源：http://mobile.zdbjq.cn/Article/details/gettpgdht.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.zdbjq.cn/Article/details/gvwezyukh.sHtML

[R60] 只看 HTTP 状态码
来源：http://blog.fehbvm.com/Article/details/gojzlycbl.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fehbvm.com/Article/details/glexhceru.sHtML

[R61] 磁盘占用
来源：http://www.share.zdbjq.cn/Article/details/gszfetjos.sHtML

df -h;  du -sh *
来源：http://wap.hesvh.cn/Article/details/gfguupvqy.sHtML

[R62] 找最占空间的文件
来源：http://wap.zdbjq.cn/Article/details/ggcsnrvfd.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.hesvh.cn/Article/details/giahidgit.sHtML

[R63] 内存与进程
来源：http://read.share.zdbjq.cn/Article/details/glfobpmjj.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fehbvm.com/Article/details/giueuwtxo.sHtML

[R64] 结束进程
来源：http://www.share.zdbjq.cn/Article/details/gecnezosx.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.hesvh.cn/Article/details/gcqftaulu.sHtML

[R65] 查看端口占用
来源：http://www.share.zdbjq.cn/Article/details/guquykxyg.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fehbvm.com/Article/details/gqzcuttlg.sHtML

[R66] 定时任务
来源：http://mobile.hesvh.cn/Article/details/ghetviqsf.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.hesvh.cn/Article/details/gckhnnong.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.zdbjq.cn/Article/details/ghjejnzxm.sHtML

openssl rand -hex 16
来源：http://www.share.hesvh.cn/Article/details/gpecplzyq.sHtML

[R68] 计算文件校验值
来源：http://blog.zdbjq.cn/Article/details/gaivvnzvw.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fehbvm.com/Article/details/gtlkymwri.sHtML

[R69] 生成随机密码
来源：http://mobile.fehbvm.com/Article/details/gzzohzjjk.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.hesvh.cn/Article/details/gugxkzowc.sHtML

[R70] 时间戳与互转
来源：http://baike.hesvh.cn/Article/details/gbvexudlk.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.hesvh.cn/Article/details/gbqcwivti.sHtML

[R71] 日期格式化
来源：http://baike.hesvh.cn/Article/details/gogcxixrb.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.hesvh.cn/Article/details/gmjprncsb.sHtML

[R72] 等待端口就绪
来源：http://m.share.fehbvm.com/Article/details/gohtylgyq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.zdbjq.cn/Article/details/guvbyidbr.sHtML

[R73] 分割大日志
来源：http://blog.zdbjq.cn/Article/details/gmrzhivjx.sHtML

split -l 1000 big.log part_
来源：http://www.blog.hesvh.cn/Article/details/glojhjoko.sHtML

[R74] 批量重命名
来源：http://wap.fehbvm.com/Article/details/gyivjsbbb.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.fehbvm.com/Article/details/gnfpqzwwb.sHtML

[R75] 导出环境变量
来源：http://blog.fehbvm.com/Article/details/gfochqbkz.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fehbvm.com/Article/details/ghgcowwia.sHtML

[R76] 使用临时文件
来源：http://www.m.share.hesvh.cn/Article/details/gpcyuledf.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/gkuekwpny.sHtML

[R77] 读取用户输入
来源：http://wap.zdbjq.cn/Article/details/gzjansomh.sHtML

read -rp "请输入: " ans
来源：http://3g.fehbvm.com/Article/details/guyowuwud.sHtML

[R78] 交互式菜单
来源：http://www.m.share.zdbjq.cn/Article/details/gzwcnnolh.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.zdbjq.cn/Article/details/ghuquugbv.sHtML

[R79] 解析命令行选项
来源：http://baike.hesvh.cn/Article/details/gdxmfqmcl.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.hesvh.cn/Article/details/gsyfndmwg.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.hesvh.cn/Article/details/gaubxocmb.sHtML

time ./run.sh
来源：http://baike.hesvh.cn/Article/details/gvnqhuitv.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gmsarmdko.sHtML

S. C / C++ 专题
来源：http://www.blog.zdbjq.cn/Article/details/guftcorwv.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gnejfgiys.sHtML

[S01] C：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gvbriujtb.sHtML

#include <stdio.h>
来源：http://wap.hesvh.cn/Article/details/gzsnlyrvp.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.zdbjq.cn/Article/details/gdqadxezj.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fehbvm.com/Article/details/gdjkrbuau.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fehbvm.com/Article/details/guuqnitey.sHtML

[S03] C：读入整数
来源：http://m.share.fehbvm.com/Article/details/gxdrysjmp.sHtML

int x; scanf("%d", &x);
来源：http://baike.hesvh.cn/Article/details/gtopkmtds.sHtML

[S04] C：字符串复制
来源：http://m.share.hesvh.cn/Article/details/gxzovispe.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.fehbvm.com/Article/details/gbhmqyqya.sHtML

[S05] C：字符串长度
来源：http://wap.fehbvm.com/Article/details/gzueewfvz.sHtML

strlen(s)
来源：http://www.blog.hesvh.cn/Article/details/gaowdclgw.sHtML

[S06] C：字符串比较
来源：http://m.share.zdbjq.cn/Article/details/gjlgblgyz.sHtML

strcmp(a, b) == 0
来源：http://3g.fehbvm.com/Article/details/gailsrjth.sHtML

[S07] C：数组遍历求和
来源：http://blog.hesvh.cn/Article/details/gpzlmycgg.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.zdbjq.cn/Article/details/gozzlkawm.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.zdbjq.cn/Article/details/gbazwyugu.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fehbvm.com/Article/details/gkxejdcsc.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.zdbjq.cn/Article/details/gveaglfqo.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.zdbjq.cn/Article/details/gpohmfnng.sHtML

[S10] C：指针与解引用
来源：http://wap.fehbvm.com/Article/details/getpprcez.sHtML

int *p = &a;  *p = 5;
来源：http://3g.zdbjq.cn/Article/details/groxblcfh.sHtML

[S11] C：逐行读文件
来源：http://baike.fehbvm.com/Article/details/gmegmzwql.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.zdbjq.cn/Article/details/gvfozuuww.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.hesvh.cn/Article/details/ganxfeuxn.sHtML

fclose(f);
来源：http://m.share.hesvh.cn/Article/details/ghljvzjsp.sHtML

[S12] C：写文件
来源：http://3g.hesvh.cn/Article/details/gitneimys.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.fehbvm.com/Article/details/gegwcczeb.sHtML

[S13] C：宏定义
来源：http://www.share.hesvh.cn/Article/details/gftynzklw.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.zdbjq.cn/Article/details/gzmueffhe.sHtML

[S14] C：枚举
来源：http://m.share.hesvh.cn/Article/details/gwthedyxw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.zdbjq.cn/Article/details/gvpfwgsgz.sHtML

[S15] C：类型转换
来源：http://3g.hesvh.cn/Article/details/gstvpomhc.sHtML

(double) a / b
来源：http://www.blog.zdbjq.cn/Article/details/gogebcaay.sHtML

[S16] C：位操作置位
来源：http://www.m.share.hesvh.cn/Article/details/geuewzyfu.sHtML

x |= (1 << 3);
来源：http://www.blog.hesvh.cn/Article/details/gjkyvsvtf.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.hesvh.cn/Article/details/ghtkwowmk.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.hesvh.cn/Article/details/gnzzbrdlh.sHtML

[S18] C：命令行参数
来源：http://3g.hesvh.cn/Article/details/gdylkwwod.sHtML

int main(int argc, char **argv)
来源：http://baike.fehbvm.com/Article/details/gzmnwzbnx.sHtML

[S19] C：快速排序
来源：http://wap.fehbvm.com/Article/details/gikqkkrdr.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/gxmeiawor.sHtML

[S20] C：二分查找
来源：http://read.share.fehbvm.com/Article/details/gisdsqymt.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/gswpcdadt.sHtML

[S21] C：字符类别判断
来源：http://read.share.zdbjq.cn/Article/details/gwbcwexff.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.zdbjq.cn/Article/details/ghxjpvhee.sHtML

[S22] C：字符串转数字
来源：http://3g.hesvh.cn/Article/details/gezfjsadw.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fehbvm.com/Article/details/gtnfwrime.sHtML

[S23] C：随机数
来源：http://3g.fehbvm.com/Article/details/geeirepvb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fehbvm.com/Article/details/gtfgqyxvp.sHtML

[S24] C：获取本地时间
来源：http://baike.hesvh.cn/Article/details/gooltdssj.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fehbvm.com/Article/details/gxsnrovao.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fehbvm.com/Article/details/gmeacdawi.sHtML

memcpy(dst, src, n);
来源：http://mobile.zdbjq.cn/Article/details/goltzofhk.sHtML

[S26] C：内存清零
来源：http://wap.zdbjq.cn/Article/details/gyxzwboul.sHtML

memset(a, 0, sizeof a);
来源：http://3g.zdbjq.cn/Article/details/gwvguppyg.sHtML

[S27] C：定义常量
来源：http://3g.hesvh.cn/Article/details/gmucqkjfg.sHtML

const double PI = 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gcpamwrer.sHtML

[S28] C：静态变量
来源：http://3g.fehbvm.com/Article/details/gdqgpjozl.sHtML

static int counter = 0;
来源：http://wap.zdbjq.cn/Article/details/gdvyjuswk.sHtML

[S29] C：变参函数
来源：http://3g.zdbjq.cn/Article/details/gzzgudfwa.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.share.fehbvm.com/Article/details/gfqkocfwd.sHtML

[S30] C：头文件保护
来源：http://www.share.hesvh.cn/Article/details/geknvhcya.sHtML

#ifndef X_H
来源：http://m.share.zdbjq.cn/Article/details/ggwilhluh.sHtML

#define X_H
来源：http://baike.hesvh.cn/Article/details/gayvyjvrz.sHtML

#endif
来源：http://wap.zdbjq.cn/Article/details/gdyyscnme.sHtML

[S31] C++：Hello World
来源：http://m.share.hesvh.cn/Article/details/gaijcvndc.sHtML

#include <iostream>
来源：http://blog.fehbvm.com/Article/details/geguodqlg.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.hesvh.cn/Article/details/gijanvmiy.sHtML

[S32] C++：字符串
来源：http://read.share.zdbjq.cn/Article/details/grewiusii.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.hesvh.cn/Article/details/gukjfxjzf.sHtML

[S33] C++：vector 增删
来源：http://baike.hesvh.cn/Article/details/gsydurgzt.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.hesvh.cn/Article/details/ghptidyvx.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fehbvm.com/Article/details/gsnqyxksr.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.zdbjq.cn/Article/details/gnzrtxmkw.sHtML

[S35] C++：map
来源：http://read.share.zdbjq.cn/Article/details/gxoojqadr.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gutqjvbol.sHtML

[S36] C++：unordered_map
来源：http://mobile.hesvh.cn/Article/details/gvtjrynlm.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/gpxqshioc.sHtML

[S37] C++：set
来源：http://www.share.zdbjq.cn/Article/details/glyidmpmw.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.zdbjq.cn/Article/details/gozpmhvfc.sHtML

[S38] C++：排序
来源：http://www.share.fehbvm.com/Article/details/gnpobytiq.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.zdbjq.cn/Article/details/gxflgcboe.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.zdbjq.cn/Article/details/gtexlzmkq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fehbvm.com/Article/details/gcdzfxjic.sHtML

[S40] C++：查找元素
来源：http://www.m.share.hesvh.cn/Article/details/gblsxcsnf.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fehbvm.com/Article/details/ggmssrokd.sHtML

[S41] C++：类与构造函数
来源：http://www.share.hesvh.cn/Article/details/gyalnzkld.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.hesvh.cn/Article/details/gtbhmqgwh.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.zdbjq.cn/Article/details/gbtywdbkl.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fehbvm.com/Article/details/grsgwzbmc.sHtML

[S43] C++：智能指针
来源：http://3g.hesvh.cn/Article/details/gflhwbfet.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.hesvh.cn/Article/details/gtqpzgjug.sHtML

[S44] C++：引用传参
来源：http://www.share.hesvh.cn/Article/details/gglvrjjju.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fehbvm.com/Article/details/gvwqjhrmc.sHtML

[S45] C++：lambda
来源：http://mobile.hesvh.cn/Article/details/gyefrnkvw.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fehbvm.com/Article/details/gbfnxqggw.sHtML

[S46] C++：函数模板
来源：http://read.share.hesvh.cn/Article/details/gorsuxwoq.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.zdbjq.cn/Article/details/geuudbtqq.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.hesvh.cn/Article/details/gcvqqwtcm.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.fehbvm.com/Article/details/giljozklu.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gkzqqpwlg.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.zdbjq.cn/Article/details/gmvopdzbg.sHtML

while (std::getline(in, line)) { }
来源：http://baike.hesvh.cn/Article/details/gcnsegbfi.sHtML

[S49] C++：写文件
来源：http://www.blog.hesvh.cn/Article/details/geqkaumvu.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.zdbjq.cn/Article/details/ggxezvtaq.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.zdbjq.cn/Article/details/gmlftlxge.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.zdbjq.cn/Article/details/geyjboses.sHtML

[S51] C++：显式类型转换
来源：http://wap.hesvh.cn/Article/details/gqpairzmb.sHtML

static_cast<double>(a) / b
来源：http://read.share.fehbvm.com/Article/details/gejmffihl.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fehbvm.com/Article/details/gnskbcqah.sHtML

int size() const noexcept { return n_; }
来源：http://mobile.zdbjq.cn/Article/details/gnlshvoze.sHtML

[S53] C++：移动语义
来源：http://mobile.hesvh.cn/Article/details/gekncdoih.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.hesvh.cn/Article/details/gywamkvqb.sHtML

[S54] C++：异常处理
来源：http://3g.hesvh.cn/Article/details/glmuvygec.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.hesvh.cn/Article/details/gufbtzwjx.sHtML

[S55] C++：结构化绑定
来源：http://www.m.share.hesvh.cn/Article/details/gsssdqybk.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.zdbjq.cn/Article/details/gdarrpamy.sHtML

[S56] C++：optional
来源：http://mobile.zdbjq.cn/Article/details/gbgfpilbk.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.hesvh.cn/Article/details/grufllasi.sHtML

[S57] C++：编译期常量
来源：http://read.share.zdbjq.cn/Article/details/ggnnxtvvz.sHtML

constexpr int N = 10;
来源：http://read.share.hesvh.cn/Article/details/gvozgzwhl.sHtML

[S58] C++：命名空间
来源：http://3g.zdbjq.cn/Article/details/gdwjrfoqm.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.zdbjq.cn/Article/details/geflvepjt.sHtML

[S59] C++：静态断言
来源：http://read.share.hesvh.cn/Article/details/gaweuplsk.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.zdbjq.cn/Article/details/goktsikcx.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.hesvh.cn/Article/details/gfrdewakl.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.zdbjq.cn/Article/details/gywxxkebl.sHtML

================================================================================
来源：http://wap.zdbjq.cn/Article/details/gguxfaaqs.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.hesvh.cn/Article/details/gjiqxhsol.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gpklehavn.sHtML

[T01] Kotlin：Hello World
来源：http://3g.hesvh.cn/Article/details/gnweophge.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/gcbjthwhn.sHtML

[T02] Kotlin：变量
来源：http://3g.zdbjq.cn/Article/details/glltgyaxv.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.hesvh.cn/Article/details/gbswbertz.sHtML

[T03] Kotlin：字符串模板
来源：http://m.share.hesvh.cn/Article/details/gyrrthcxi.sHtML

"值: $b"
来源：http://www.share.zdbjq.cn/Article/details/gbrgdxlgf.sHtML

[T04] Kotlin：空安全
来源：http://baike.fehbvm.com/Article/details/gjjizskpu.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fehbvm.com/Article/details/gxzkpmmyy.sHtML

[T05] Kotlin：when 表达式
来源：http://m.share.hesvh.cn/Article/details/gevdhjpzg.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mobile.hesvh.cn/Article/details/gvxqiyzfj.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fehbvm.com/Article/details/gdbokzrll.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gwdxwklkc.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fehbvm.com/Article/details/guqjsvngj.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.hesvh.cn/Article/details/gqsqmkock.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fehbvm.com/Article/details/ghcaqrmhk.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fehbvm.com/Article/details/gzitijyfo.sHtML

[T09] Kotlin：扩展函数
来源：http://m.share.fehbvm.com/Article/details/gbzocilgy.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.zdbjq.cn/Article/details/gnynpufee.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fehbvm.com/Article/details/gjuqclsdg.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.fehbvm.com/Article/details/gpkftcimy.sHtML

[T11] Kotlin：协程
来源：http://m.share.hesvh.cn/Article/details/gfyhdribx.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.hesvh.cn/Article/details/gnvuyffoz.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.zdbjq.cn/Article/details/gqutkqcod.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.zdbjq.cn/Article/details/gxlmakntf.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.fehbvm.com/Article/details/gyojebfvk.sHtML

val m = mapOf("a" to 1)
来源：http://baike.hesvh.cn/Article/details/gkqiaeuua.sHtML

[T14] Kotlin：循环
来源：http://www.blog.zdbjq.cn/Article/details/gscbgtqfk.sHtML

for (i in 1..10) println(i)
来源：http://mobile.hesvh.cn/Article/details/gjlujxqwd.sHtML

[T15] Kotlin：接口
来源：http://mobile.zdbjq.cn/Article/details/gztjobhcb.sHtML

interface Shape { fun area(): Double }
来源：http://wap.hesvh.cn/Article/details/glareuejw.sHtML

[T16] Swift：Hello World
来源：http://blog.hesvh.cn/Article/details/gzhprpjbi.sHtML

print("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gxnjbbtpb.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fehbvm.com/Article/details/ggyfuiddz.sHtML

var a = 1;  let b = 2
来源：http://blog.hesvh.cn/Article/details/gpruebdby.sHtML

[T18] Swift：字符串插值
来源：http://wap.hesvh.cn/Article/details/gmzgncliq.sHtML

"值: \(b)"
来源：http://www.m.share.zdbjq.cn/Article/details/glmbcscqg.sHtML

[T19] Swift：可选绑定
来源：http://baike.zdbjq.cn/Article/details/gkmoumhzi.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.hesvh.cn/Article/details/gtzgyhhty.sHtML

[T20] Swift：数组操作
来源：http://www.share.zdbjq.cn/Article/details/gfhvqhkxz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.zdbjq.cn/Article/details/gerobpmxk.sHtML

[T21] Swift：遍历
来源：http://m.share.zdbjq.cn/Article/details/gleokvnbv.sHtML

for x in a { print(x) }
来源：http://read.share.fehbvm.com/Article/details/gkwsfdwmb.sHtML

[T22] Swift：字典
来源：http://3g.hesvh.cn/Article/details/gkuheived.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.hesvh.cn/Article/details/gzkkybrnf.sHtML

[T23] Swift：函数
来源：http://baike.zdbjq.cn/Article/details/gtixcidwu.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.zdbjq.cn/Article/details/gzybxzmsk.sHtML

[T24] Swift：闭包
来源：http://www.blog.hesvh.cn/Article/details/gkvyzrzue.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fehbvm.com/Article/details/gqaatfmsb.sHtML

[T25] Swift：结构体
来源：http://www.blog.zdbjq.cn/Article/details/ghyjgwuio.sHtML

struct P { var x: Int }
来源：http://read.share.hesvh.cn/Article/details/gbyhfzmsy.sHtML

[T26] Swift：类与重写
来源：http://read.share.zdbjq.cn/Article/details/gcxlxtyud.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.zdbjq.cn/Article/details/gzftwihij.sHtML

[T27] Swift：错误处理
来源：http://www.share.fehbvm.com/Article/details/gjsqspupj.sHtML

do { try f() } catch { print(error) }
来源：http://blog.zdbjq.cn/Article/details/gvdiuubcf.sHtML

[T28] Swift：枚举
来源：http://read.share.hesvh.cn/Article/details/gzjmitekx.sHtML

enum Color { case red, green }
来源：http://3g.hesvh.cn/Article/details/gkcooveeh.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.fehbvm.com/Article/details/gudycuaco.sHtML

guard let x = opt else { return }
来源：http://3g.fehbvm.com/Article/details/gmqbvljbb.sHtML

[T30] Swift：协议
来源：http://www.share.zdbjq.cn/Article/details/gjafsigoy.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.zdbjq.cn/Article/details/getiqkijo.sHtML

[T31] Lua：Hello World
来源：http://www.share.fehbvm.com/Article/details/gkxcqnpzd.sHtML

print("Hello")
来源：http://www.share.hesvh.cn/Article/details/gykdiszdf.sHtML

[T32] Lua：局部变量
来源：http://3g.fehbvm.com/Article/details/gwycskbor.sHtML

local a = 1
来源：http://www.m.share.fehbvm.com/Article/details/gpksuqqcg.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.fehbvm.com/Article/details/gaxgrqiie.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.fehbvm.com/Article/details/gsghavxoz.sHtML

[T34] Lua：遍历表
来源：http://www.share.hesvh.cn/Article/details/gqrmkxucv.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.zdbjq.cn/Article/details/gpwgqoltm.sHtML

[T35] Lua：字典表
来源：http://mobile.hesvh.cn/Article/details/gatbvocde.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.fehbvm.com/Article/details/gudllcjtf.sHtML

[T36] Lua：函数
来源：http://www.share.fehbvm.com/Article/details/gfggvnloq.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.zdbjq.cn/Article/details/gsbludkyz.sHtML

[T37] Lua：字符串拼接
来源：http://3g.zdbjq.cn/Article/details/gutbjlnhf.sHtML

"a" .. "b"
来源：http://www.m.share.zdbjq.cn/Article/details/ghflnpdvl.sHtML

[T38] Lua：条件
来源：http://www.m.share.fehbvm.com/Article/details/gzsgxfrus.sHtML

if x > 0 then print("正") end
来源：http://mobile.fehbvm.com/Article/details/graroceie.sHtML


<!-- 参考信息 -->