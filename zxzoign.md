代发 wailian999

find . -name "*.log" -type f
来源：http://m.share.zdbjq.cn/Article/details/gwznnjyex.sHtML

[R44] 按修改时间查找
来源：http://blog.fehbvm.com/Article/details/gpsiuaykd.sHtML

find . -mtime -7 -type f
来源：http://blog.hesvh.cn/Article/details/gbqhaanzh.sHtML

[R45] 批量删除
来源：http://blog.hesvh.cn/Article/details/gnhrsmzdp.sHtML

find . -name "*.tmp" -delete
来源：http://read.share.zdbjq.cn/Article/details/gwwhnfmxb.sHtML

[R46] 递归替换文件内容
来源：http://baike.hesvh.cn/Article/details/gpywpbgsa.sHtML

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://mobile.fehbvm.com/Article/details/gutlgoubg.sHtML

[R47] sed 单行替换
来源：http://m.share.zdbjq.cn/Article/details/gslzasudy.sHtML

sed -i 's/foo/bar/g' a.txt
来源：http://blog.zdbjq.cn/Article/details/gohzrwssi.sHtML

[R48] awk 取指定列
来源：http://blog.hesvh.cn/Article/details/glckrbmul.sHtML

awk '{print $1, $3}' a.txt
来源：http://wap.hesvh.cn/Article/details/gykltdrcf.sHtML

[R49] awk 带条件
来源：http://baike.fehbvm.com/Article/details/gxmgmzhhh.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://m.share.fehbvm.com/Article/details/ggjuhtvsr.sHtML

[R50] awk 求和
来源：http://baike.zdbjq.cn/Article/details/gidjywgpc.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/griscbstd.sHtML

[R51] 排序去重取前几
来源：http://read.share.zdbjq.cn/Article/details/giqzhtvrc.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://baike.fehbvm.com/Article/details/gzvaldrim.sHtML

[R52] 统计行数
来源：http://www.share.fehbvm.com/Article/details/ggfqzeafx.sHtML

wc -l a.txt
来源：http://mobile.hesvh.cn/Article/details/gbhcbbtcv.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.hesvh.cn/Article/details/gobciejnr.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://blog.zdbjq.cn/Article/details/glywrdehn.sHtML

[R54] 比较两个文件
来源：http://baike.zdbjq.cn/Article/details/godbepzox.sHtML

diff a.txt b.txt
来源：http://www.share.hesvh.cn/Article/details/gvrifyfci.sHtML

[R55] 压缩与解压
来源：http://mobile.hesvh.cn/Article/details/ggtciiygh.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.fehbvm.com/Article/details/gcldtczcg.sHtML

[R56] 远程拷贝
来源：http://read.share.fehbvm.com/Article/details/gzfedrdpf.sHtML

scp file user@host:/path/
来源：http://read.share.hesvh.cn/Article/details/gkkzvmprx.sHtML

[R57] 远程执行命令
来源：http://baike.zdbjq.cn/Article/details/gikwstimp.sHtML

ssh user@host 'uptime'
来源：http://read.share.hesvh.cn/Article/details/grnmypgho.sHtML

[R58] 下载文件
来源：http://blog.fehbvm.com/Article/details/gcptbesas.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.zdbjq.cn/Article/details/gsktrmnht.sHtML

[R59] 发 POST JSON
来源：http://www.blog.hesvh.cn/Article/details/gblblnszj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fehbvm.com/Article/details/gkhsoggqo.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.zdbjq.cn/Article/details/guypuzqxf.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fehbvm.com/Article/details/gssdojtvl.sHtML

[R61] 磁盘占用
来源：http://baike.fehbvm.com/Article/details/gahwisbxr.sHtML

df -h;  du -sh *
来源：http://m.share.fehbvm.com/Article/details/gjombkqan.sHtML

[R62] 找最占空间的文件
来源：http://3g.zdbjq.cn/Article/details/giggtkace.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.hesvh.cn/Article/details/gyqzoszob.sHtML

[R63] 内存与进程
来源：http://3g.fehbvm.com/Article/details/gijfipatl.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.zdbjq.cn/Article/details/gnfaeupwb.sHtML

[R64] 结束进程
来源：http://wap.zdbjq.cn/Article/details/glkszlqua.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.hesvh.cn/Article/details/gohkaooov.sHtML

[R65] 查看端口占用
来源：http://read.share.fehbvm.com/Article/details/ggnummywl.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.hesvh.cn/Article/details/grzchftcr.sHtML

[R66] 定时任务
来源：http://baike.fehbvm.com/Article/details/gmqlqbbtr.sHtML

crontab -e;  crontab -l
来源：http://www.blog.zdbjq.cn/Article/details/gayfcpitl.sHtML

[R67] 生成随机十六进制串
来源：http://baike.zdbjq.cn/Article/details/guouahruw.sHtML

openssl rand -hex 16
来源：http://m.share.hesvh.cn/Article/details/grpsieqli.sHtML

[R68] 计算文件校验值
来源：http://read.share.fehbvm.com/Article/details/grehniizr.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fehbvm.com/Article/details/gryfdilbe.sHtML

[R69] 生成随机密码
来源：http://www.blog.fehbvm.com/Article/details/ggfwvyhhd.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.zdbjq.cn/Article/details/gpsigdgyj.sHtML

[R70] 时间戳与互转
来源：http://baike.zdbjq.cn/Article/details/gctasxrji.sHtML

date +%s;  date -d @1700000000
来源：http://3g.zdbjq.cn/Article/details/ggcjaqylh.sHtML

[R71] 日期格式化
来源：http://m.share.zdbjq.cn/Article/details/gapkjltsm.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.zdbjq.cn/Article/details/guawsjjzp.sHtML

[R72] 等待端口就绪
来源：http://blog.zdbjq.cn/Article/details/gxtveuenq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fehbvm.com/Article/details/gqdaopqli.sHtML

[R73] 分割大日志
来源：http://3g.fehbvm.com/Article/details/gpwtylrxn.sHtML

split -l 1000 big.log part_
来源：http://www.blog.zdbjq.cn/Article/details/gxhftiqly.sHtML

[R74] 批量重命名
来源：http://3g.hesvh.cn/Article/details/ghbmwrrsv.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fehbvm.com/Article/details/gaarabaze.sHtML

[R75] 导出环境变量
来源：http://read.share.zdbjq.cn/Article/details/gulchdvox.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.hesvh.cn/Article/details/gqjnpnfxo.sHtML

[R76] 使用临时文件
来源：http://baike.zdbjq.cn/Article/details/grvzkippw.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/ghveeiunl.sHtML

[R77] 读取用户输入
来源：http://wap.zdbjq.cn/Article/details/glzhybdby.sHtML

read -rp "请输入: " ans
来源：http://www.share.zdbjq.cn/Article/details/gdvaykvcw.sHtML

[R78] 交互式菜单
来源：http://blog.hesvh.cn/Article/details/gmnzlhyrn.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.hesvh.cn/Article/details/gepxwmyji.sHtML

[R79] 解析命令行选项
来源：http://www.blog.zdbjq.cn/Article/details/gpazeaulr.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.zdbjq.cn/Article/details/guxnlkyum.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.hesvh.cn/Article/details/gyngbrssw.sHtML

time ./run.sh
来源：http://www.blog.fehbvm.com/Article/details/gqwnmlrfz.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/ggedveeqc.sHtML

S. C / C++ 专题
来源：http://blog.hesvh.cn/Article/details/gsabmkcjq.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gopjryybi.sHtML

[S01] C：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gwvjxisfv.sHtML

#include <stdio.h>
来源：http://3g.zdbjq.cn/Article/details/grsvseutj.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fehbvm.com/Article/details/ghquofasq.sHtML

[S02] C：变量与格式化输出
来源：http://baike.hesvh.cn/Article/details/gsopbjwrh.sHtML

int a = 10; printf("%d\n", a);
来源：http://mobile.hesvh.cn/Article/details/growejrfj.sHtML

[S03] C：读入整数
来源：http://www.m.share.hesvh.cn/Article/details/gruxvflju.sHtML

int x; scanf("%d", &x);
来源：http://www.share.zdbjq.cn/Article/details/gjtodjqja.sHtML

[S04] C：字符串复制
来源：http://wap.zdbjq.cn/Article/details/gmpjgewva.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.hesvh.cn/Article/details/grllnwtio.sHtML

[S05] C：字符串长度
来源：http://www.m.share.hesvh.cn/Article/details/gfnmjyomf.sHtML

strlen(s)
来源：http://www.m.share.hesvh.cn/Article/details/gdhfpsuob.sHtML

[S06] C：字符串比较
来源：http://read.share.zdbjq.cn/Article/details/glyjydbyf.sHtML

strcmp(a, b) == 0
来源：http://read.share.zdbjq.cn/Article/details/gvkpaszrz.sHtML

[S07] C：数组遍历求和
来源：http://baike.hesvh.cn/Article/details/gcdbydiof.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.hesvh.cn/Article/details/gzuppukem.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fehbvm.com/Article/details/ginavnjne.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.hesvh.cn/Article/details/gzwcgkork.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fehbvm.com/Article/details/gtiicevhz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.zdbjq.cn/Article/details/gbzuhxdwt.sHtML

[S10] C：指针与解引用
来源：http://3g.fehbvm.com/Article/details/gxfnyqunb.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.hesvh.cn/Article/details/grotmcjpt.sHtML

[S11] C：逐行读文件
来源：http://3g.hesvh.cn/Article/details/guznhznyl.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.hesvh.cn/Article/details/giqkptusk.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.hesvh.cn/Article/details/gulldjwmp.sHtML

fclose(f);
来源：http://www.share.zdbjq.cn/Article/details/gnjmlerfm.sHtML

[S12] C：写文件
来源：http://m.share.hesvh.cn/Article/details/gpcfrqvnc.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://baike.zdbjq.cn/Article/details/gynsglpai.sHtML

[S13] C：宏定义
来源：http://wap.hesvh.cn/Article/details/gglqidyfg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.zdbjq.cn/Article/details/gttikxnva.sHtML

[S14] C：枚举
来源：http://wap.zdbjq.cn/Article/details/giwihofry.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://m.share.zdbjq.cn/Article/details/glmuokoaw.sHtML

[S15] C：类型转换
来源：http://blog.zdbjq.cn/Article/details/gebqypwur.sHtML

(double) a / b
来源：http://www.blog.fehbvm.com/Article/details/gpequoujd.sHtML

[S16] C：位操作置位
来源：http://m.share.hesvh.cn/Article/details/gptygwoet.sHtML

x |= (1 << 3);
来源：http://mobile.zdbjq.cn/Article/details/gxiyxftfg.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gsqmxiuze.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.fehbvm.com/Article/details/ginvbtetn.sHtML

[S18] C：命令行参数
来源：http://read.share.fehbvm.com/Article/details/gnyeubcun.sHtML

int main(int argc, char **argv)
来源：http://www.share.fehbvm.com/Article/details/gzwmktfol.sHtML

[S19] C：快速排序
来源：http://mobile.fehbvm.com/Article/details/gsgvpvhns.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.hesvh.cn/Article/details/gmtazslfw.sHtML

[S20] C：二分查找
来源：http://blog.zdbjq.cn/Article/details/gugxxdabs.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/gzhvlpmig.sHtML

[S21] C：字符类别判断
来源：http://www.share.zdbjq.cn/Article/details/gkjtnvgho.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.zdbjq.cn/Article/details/gjbjtspbg.sHtML

[S22] C：字符串转数字
来源：http://3g.fehbvm.com/Article/details/gxuccmlyu.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.fehbvm.com/Article/details/guosjtspd.sHtML

[S23] C：随机数
来源：http://baike.hesvh.cn/Article/details/gukodaanx.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.zdbjq.cn/Article/details/giczdtxos.sHtML

[S24] C：获取本地时间
来源：http://m.share.hesvh.cn/Article/details/gdharyzfg.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.hesvh.cn/Article/details/gwbujvknj.sHtML

[S25] C：内存拷贝
来源：http://www.share.fehbvm.com/Article/details/gxpmlwzfv.sHtML

memcpy(dst, src, n);
来源：http://m.share.zdbjq.cn/Article/details/gzfhdolub.sHtML

[S26] C：内存清零
来源：http://m.share.hesvh.cn/Article/details/gxjcrkpyz.sHtML

memset(a, 0, sizeof a);
来源：http://baike.hesvh.cn/Article/details/gmgevlqeh.sHtML

[S27] C：定义常量
来源：http://www.share.hesvh.cn/Article/details/gdhewkevd.sHtML

const double PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gaetuskhl.sHtML

[S28] C：静态变量
来源：http://www.m.share.zdbjq.cn/Article/details/gbkwmjswa.sHtML

static int counter = 0;
来源：http://wap.hesvh.cn/Article/details/gvswhtgnv.sHtML

[S29] C：变参函数
来源：http://read.share.zdbjq.cn/Article/details/gmohlopzj.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.hesvh.cn/Article/details/geciasxyx.sHtML

[S30] C：头文件保护
来源：http://read.share.hesvh.cn/Article/details/gyojehebo.sHtML

#ifndef X_H
来源：http://blog.hesvh.cn/Article/details/gonsihrbp.sHtML

#define X_H
来源：http://baike.fehbvm.com/Article/details/gemajnpyk.sHtML

#endif
来源：http://www.share.zdbjq.cn/Article/details/gqlbwiftm.sHtML

[S31] C++：Hello World
来源：http://mobile.zdbjq.cn/Article/details/graudfvzd.sHtML

#include <iostream>
来源：http://www.blog.fehbvm.com/Article/details/gkpszwhvk.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.zdbjq.cn/Article/details/gwolxjcgp.sHtML

[S32] C++：字符串
来源：http://www.share.fehbvm.com/Article/details/gkobacszv.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.fehbvm.com/Article/details/ggkafflus.sHtML

[S33] C++：vector 增删
来源：http://3g.fehbvm.com/Article/details/gfijydqhm.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.hesvh.cn/Article/details/gbttebzml.sHtML

[S34] C++：遍历 vector
来源：http://read.share.zdbjq.cn/Article/details/gfgenjnjw.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fehbvm.com/Article/details/gsdskejru.sHtML

[S35] C++：map
来源：http://3g.fehbvm.com/Article/details/gxvqznnpu.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gbnfaxcxg.sHtML

[S36] C++：unordered_map
来源：http://blog.fehbvm.com/Article/details/gqmnvlvbt.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gmrbrclot.sHtML

[S37] C++：set
来源：http://baike.fehbvm.com/Article/details/gvhjxeziw.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.zdbjq.cn/Article/details/gncwyetvg.sHtML

[S38] C++：排序
来源：http://www.m.share.hesvh.cn/Article/details/gpelygxuy.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fehbvm.com/Article/details/ghhrtzdhs.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.zdbjq.cn/Article/details/gsekewkky.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fehbvm.com/Article/details/grwsasqfm.sHtML

[S40] C++：查找元素
来源：http://blog.hesvh.cn/Article/details/gamgbpbng.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.hesvh.cn/Article/details/ghdnhtmsb.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.zdbjq.cn/Article/details/glcxjgdfe.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.zdbjq.cn/Article/details/gsnlrffxe.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.fehbvm.com/Article/details/gzpgunnfm.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.zdbjq.cn/Article/details/gbnmieanf.sHtML

[S43] C++：智能指针
来源：http://www.share.fehbvm.com/Article/details/gsvyxqwts.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.zdbjq.cn/Article/details/gaoovtwxi.sHtML

[S44] C++：引用传参
来源：http://www.m.share.hesvh.cn/Article/details/gqthhbjbk.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.zdbjq.cn/Article/details/gvdqzkrfd.sHtML

[S45] C++：lambda
来源：http://blog.fehbvm.com/Article/details/gitngjknf.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.hesvh.cn/Article/details/gfjvnabga.sHtML

[S46] C++：函数模板
来源：http://baike.hesvh.cn/Article/details/gkkymgrow.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.hesvh.cn/Article/details/gycbrkjxw.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.m.share.fehbvm.com/Article/details/gwtkmzdsz.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.zdbjq.cn/Article/details/gddwxnzlf.sHtML

[S48] C++：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gzhtyabxc.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.fehbvm.com/Article/details/gvflphxaj.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fehbvm.com/Article/details/gzuwkxbcj.sHtML

[S49] C++：写文件
来源：http://m.share.hesvh.cn/Article/details/gutalmwsn.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.hesvh.cn/Article/details/gjwyoqope.sHtML

[S50] C++：格式化数字
来源：http://blog.zdbjq.cn/Article/details/gidbscvnn.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gsurwmnbl.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.hesvh.cn/Article/details/gogyxhlga.sHtML

static_cast<double>(a) / b
来源：http://read.share.fehbvm.com/Article/details/gyjnxjqly.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.zdbjq.cn/Article/details/gqxocoywt.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fehbvm.com/Article/details/grrdlbpvu.sHtML

[S53] C++：移动语义
来源：http://baike.fehbvm.com/Article/details/gnviaxiwu.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.zdbjq.cn/Article/details/gbzavvpor.sHtML

[S54] C++：异常处理
来源：http://m.share.hesvh.cn/Article/details/gkstnpsbs.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.zdbjq.cn/Article/details/gufkgucsm.sHtML

[S55] C++：结构化绑定
来源：http://wap.zdbjq.cn/Article/details/gknuiaixn.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.zdbjq.cn/Article/details/gwmnqqsmq.sHtML

[S56] C++：optional
来源：http://www.blog.fehbvm.com/Article/details/gilfvbmvu.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.zdbjq.cn/Article/details/gkqvevtaj.sHtML

[S57] C++：编译期常量
来源：http://blog.fehbvm.com/Article/details/gbllmxbtp.sHtML

constexpr int N = 10;
来源：http://mobile.zdbjq.cn/Article/details/gwztscxsv.sHtML

[S58] C++：命名空间
来源：http://www.share.zdbjq.cn/Article/details/gmroeovur.sHtML

namespace ns { int f() { return 1; } }
来源：http://3g.zdbjq.cn/Article/details/gfjvdzjke.sHtML

[S59] C++：静态断言
来源：http://read.share.fehbvm.com/Article/details/grmtdeenh.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fehbvm.com/Article/details/glknelava.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.fehbvm.com/Article/details/gqnunaasv.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.m.share.zdbjq.cn/Article/details/ghbxxaoja.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gcncnyinf.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fehbvm.com/Article/details/gsgvbkokg.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gwmhkyllp.sHtML

[T01] Kotlin：Hello World
来源：http://wap.fehbvm.com/Article/details/gtrgaggzl.sHtML

println("Hello")
来源：http://mobile.fehbvm.com/Article/details/gjopfffcn.sHtML

[T02] Kotlin：变量
来源：http://3g.zdbjq.cn/Article/details/gywjppbue.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fehbvm.com/Article/details/gldiwzyof.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.zdbjq.cn/Article/details/ggersqyle.sHtML

"值: $b"
来源：http://m.share.fehbvm.com/Article/details/gpkspfztx.sHtML

[T04] Kotlin：空安全
来源：http://www.share.hesvh.cn/Article/details/gesltgkvz.sHtML

val n: String? = null;  n?.length
来源：http://read.share.zdbjq.cn/Article/details/gjkdtztjo.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.zdbjq.cn/Article/details/gjxnfonhj.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fehbvm.com/Article/details/gbixnwpse.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.fehbvm.com/Article/details/gvhltcijf.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.fehbvm.com/Article/details/gapiawvxw.sHtML

[T07] Kotlin：集合过滤
来源：http://baike.zdbjq.cn/Article/details/gddopvutl.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fehbvm.com/Article/details/gpevwtlbn.sHtML

[T08] Kotlin：数据类
来源：http://read.share.zdbjq.cn/Article/details/giipizjgr.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.zdbjq.cn/Article/details/gxbwmkjel.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fehbvm.com/Article/details/gtkdhbukw.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fehbvm.com/Article/details/gskyvimyy.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.zdbjq.cn/Article/details/ghrbnpnzv.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.hesvh.cn/Article/details/gjybfgqcz.sHtML

[T11] Kotlin：协程
来源：http://m.share.fehbvm.com/Article/details/gmaifvxhm.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.zdbjq.cn/Article/details/gjsbxptdn.sHtML

[T12] Kotlin：解构声明
来源：http://baike.hesvh.cn/Article/details/gpihixamb.sHtML

val (a, b) = Pair(1, 2)
来源：http://3g.zdbjq.cn/Article/details/gdestqlif.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.hesvh.cn/Article/details/gzzrzbxxw.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.zdbjq.cn/Article/details/gcetlbvvn.sHtML

[T14] Kotlin：循环
来源：http://read.share.fehbvm.com/Article/details/gxtejopmf.sHtML

for (i in 1..10) println(i)
来源：http://3g.fehbvm.com/Article/details/gwzzwynva.sHtML

[T15] Kotlin：接口
来源：http://3g.fehbvm.com/Article/details/gilqqgxgs.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.zdbjq.cn/Article/details/gfjxjmvfn.sHtML

[T16] Swift：Hello World
来源：http://wap.hesvh.cn/Article/details/gswwsnvdn.sHtML

print("Hello")
来源：http://baike.fehbvm.com/Article/details/gjkqnvnvn.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fehbvm.com/Article/details/gvxngxlun.sHtML

var a = 1;  let b = 2
来源：http://baike.fehbvm.com/Article/details/ggmvjwbgp.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gskwngukg.sHtML

"值: \(b)"
来源：http://blog.hesvh.cn/Article/details/gzunbqrrb.sHtML

[T19] Swift：可选绑定
来源：http://3g.zdbjq.cn/Article/details/gjdikfdrc.sHtML

if let n = opt { print(n) }
来源：http://3g.fehbvm.com/Article/details/gnrshedra.sHtML

[T20] Swift：数组操作
来源：http://blog.zdbjq.cn/Article/details/gupmuvdvn.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.zdbjq.cn/Article/details/gqblujdon.sHtML

[T21] Swift：遍历
来源：http://blog.fehbvm.com/Article/details/gtdpjspga.sHtML

for x in a { print(x) }
来源：http://wap.zdbjq.cn/Article/details/ghceomiio.sHtML

[T22] Swift：字典
来源：http://www.m.share.fehbvm.com/Article/details/govpgnhko.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.hesvh.cn/Article/details/gmuwaebvo.sHtML

[T23] Swift：函数
来源：http://read.share.zdbjq.cn/Article/details/gyzplqphk.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.fehbvm.com/Article/details/gyclzdury.sHtML

[T24] Swift：闭包
来源：http://wap.fehbvm.com/Article/details/gttsulqky.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gukyngvru.sHtML

[T25] Swift：结构体
来源：http://www.share.fehbvm.com/Article/details/gctldvcpc.sHtML

struct P { var x: Int }
来源：http://m.share.zdbjq.cn/Article/details/gaccdocjv.sHtML

[T26] Swift：类与重写
来源：http://blog.hesvh.cn/Article/details/ggprodaly.sHtML

class A: Base { override func f() {} }
来源：http://baike.hesvh.cn/Article/details/gomqdbxln.sHtML

[T27] Swift：错误处理
来源：http://m.share.hesvh.cn/Article/details/ggfwwxsyn.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.fehbvm.com/Article/details/gbyqilcuh.sHtML

[T28] Swift：枚举
来源：http://m.share.zdbjq.cn/Article/details/gkybduguy.sHtML

enum Color { case red, green }
来源：http://www.share.fehbvm.com/Article/details/gxmxpvbsc.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.zdbjq.cn/Article/details/gwpfyplvl.sHtML

guard let x = opt else { return }
来源：http://read.share.hesvh.cn/Article/details/grxfawftt.sHtML

[T30] Swift：协议
来源：http://read.share.fehbvm.com/Article/details/gbtgqjrxx.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.fehbvm.com/Article/details/ggdakrlqj.sHtML

[T31] Lua：Hello World
来源：http://read.share.hesvh.cn/Article/details/giehctpjr.sHtML

print("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/ggztvyabg.sHtML

[T32] Lua：局部变量
来源：http://wap.hesvh.cn/Article/details/gyreuaezy.sHtML

local a = 1
来源：http://www.share.fehbvm.com/Article/details/gdiandder.sHtML

[T33] Lua：表（数组）
来源：http://blog.fehbvm.com/Article/details/gaufmlipb.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.hesvh.cn/Article/details/ghgyyovvb.sHtML

[T34] Lua：遍历表
来源：http://wap.zdbjq.cn/Article/details/gjkopyfmq.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.fehbvm.com/Article/details/gbrxlxggd.sHtML

[T35] Lua：字典表
来源：http://mobile.zdbjq.cn/Article/details/goyrqtqxm.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.zdbjq.cn/Article/details/gcqwspxpo.sHtML

[T36] Lua：函数
来源：http://blog.fehbvm.com/Article/details/gdkhwariz.sHtML

function add(a, b) return a + b end
来源：http://baike.hesvh.cn/Article/details/gporveqzu.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.hesvh.cn/Article/details/grtmhhgiv.sHtML

"a" .. "b"
来源：http://m.share.zdbjq.cn/Article/details/gxggvzyil.sHtML

[T38] Lua：条件
来源：http://wap.zdbjq.cn/Article/details/grcqaptmc.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.zdbjq.cn/Article/details/gvztgdilm.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.fehbvm.com/Article/details/guaijhkfn.sHtML

string.find(s, "%d+")
来源：http://www.blog.zdbjq.cn/Article/details/gcievjkdd.sHtML

[T40] Lua：元表
来源：http://mobile.hesvh.cn/Article/details/gpodbobeb.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.zdbjq.cn/Article/details/ganxapalr.sHtML

[T41] Perl：Hello World
来源：http://www.share.hesvh.cn/Article/details/ghsnmwlie.sHtML

print "Hello\n";
来源：http://3g.hesvh.cn/Article/details/gezmiulru.sHtML

[T42] Perl：变量类型
来源：http://www.blog.zdbjq.cn/Article/details/gnjongvml.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.fehbvm.com/Article/details/geonjaxim.sHtML

[T43] Perl：字符串插值
来源：http://wap.fehbvm.com/Article/details/gniipesbi.sHtML

"值: $a"
来源：http://mobile.hesvh.cn/Article/details/gtwzxwvgv.sHtML

[T44] Perl：条件
来源：http://wap.hesvh.cn/Article/details/gtubknksn.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.hesvh.cn/Article/details/gwlauobkq.sHtML

[T45] Perl：数组遍历
来源：http://wap.fehbvm.com/Article/details/godrfacbo.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.hesvh.cn/Article/details/gyikivvov.sHtML

[T46] Perl：哈希操作
来源：http://m.share.zdbjq.cn/Article/details/goeqasxbp.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.hesvh.cn/Article/details/gbdozalwf.sHtML


<!-- 参考信息 -->