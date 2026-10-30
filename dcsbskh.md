代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.m.share.zdbjq.cn/Article/details/gqpmkoagg.sHtML

[R50] awk 求和
来源：http://www.m.share.fehbvm.com/Article/details/gnwdnfijk.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.m.share.zdbjq.cn/Article/details/ghrriebam.sHtML

[R51] 排序去重取前几
来源：http://mobile.hesvh.cn/Article/details/grzpnerdr.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.fehbvm.com/Article/details/gqbotznqq.sHtML

[R52] 统计行数
来源：http://www.m.share.fehbvm.com/Article/details/ghvdfwuih.sHtML

wc -l a.txt
来源：http://m.share.zdbjq.cn/Article/details/gwzcxvzvp.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.fehbvm.com/Article/details/gzffhxuvi.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.zdbjq.cn/Article/details/ggwnhfkfu.sHtML

[R54] 比较两个文件
来源：http://www.share.fehbvm.com/Article/details/garzwhxxj.sHtML

diff a.txt b.txt
来源：http://blog.zdbjq.cn/Article/details/ghpkaxsjm.sHtML

[R55] 压缩与解压
来源：http://m.share.zdbjq.cn/Article/details/gkrpxsftw.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fehbvm.com/Article/details/gygzgdadd.sHtML

[R56] 远程拷贝
来源：http://www.m.share.zdbjq.cn/Article/details/gllvzterm.sHtML

scp file user@host:/path/
来源：http://wap.hesvh.cn/Article/details/gpxmlrfsc.sHtML

[R57] 远程执行命令
来源：http://blog.zdbjq.cn/Article/details/gbhwfetip.sHtML

ssh user@host 'uptime'
来源：http://www.share.hesvh.cn/Article/details/ggayshxdt.sHtML

[R58] 下载文件
来源：http://read.share.hesvh.cn/Article/details/ggcksehsj.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mobile.fehbvm.com/Article/details/girbhxqnb.sHtML

[R59] 发 POST JSON
来源：http://read.share.hesvh.cn/Article/details/gzekditfd.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fehbvm.com/Article/details/ggbfxqouc.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.fehbvm.com/Article/details/gnxjuiipl.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.hesvh.cn/Article/details/gpmuphlir.sHtML

[R61] 磁盘占用
来源：http://www.m.share.hesvh.cn/Article/details/gdqgpejra.sHtML

df -h;  du -sh *
来源：http://www.m.share.fehbvm.com/Article/details/gcfrzkiiv.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.zdbjq.cn/Article/details/gxomjccpj.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.hesvh.cn/Article/details/gqqfbdonn.sHtML

[R63] 内存与进程
来源：http://baike.zdbjq.cn/Article/details/gqcpthqyx.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.fehbvm.com/Article/details/gfxvobhjv.sHtML

[R64] 结束进程
来源：http://www.blog.hesvh.cn/Article/details/gxbqfagyl.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.hesvh.cn/Article/details/gatjwsiaq.sHtML

[R65] 查看端口占用
来源：http://m.share.hesvh.cn/Article/details/gxdlkbbbn.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.fehbvm.com/Article/details/gzkwmumuc.sHtML

[R66] 定时任务
来源：http://www.blog.hesvh.cn/Article/details/gduaosjnz.sHtML

crontab -e;  crontab -l
来源：http://wap.hesvh.cn/Article/details/ggctenxkc.sHtML

[R67] 生成随机十六进制串
来源：http://wap.zdbjq.cn/Article/details/gnawcoxxk.sHtML

openssl rand -hex 16
来源：http://www.m.share.zdbjq.cn/Article/details/goeyxeovx.sHtML

[R68] 计算文件校验值
来源：http://m.share.hesvh.cn/Article/details/gutowdqve.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.hesvh.cn/Article/details/gxyntopca.sHtML

[R69] 生成随机密码
来源：http://www.share.zdbjq.cn/Article/details/gvpfhpfgl.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.hesvh.cn/Article/details/gibatytog.sHtML

[R70] 时间戳与互转
来源：http://www.blog.zdbjq.cn/Article/details/gxogooqur.sHtML

date +%s;  date -d @1700000000
来源：http://wap.hesvh.cn/Article/details/gxaadllll.sHtML

[R71] 日期格式化
来源：http://blog.hesvh.cn/Article/details/gtdcmevku.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://read.share.zdbjq.cn/Article/details/gnckutrkl.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.hesvh.cn/Article/details/gofsptklc.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://read.share.fehbvm.com/Article/details/gskrjxdsf.sHtML

[R73] 分割大日志
来源：http://m.share.hesvh.cn/Article/details/gsnrfugrc.sHtML

split -l 1000 big.log part_
来源：http://wap.hesvh.cn/Article/details/gpnutsivs.sHtML

[R74] 批量重命名
来源：http://read.share.zdbjq.cn/Article/details/gwqpjnqsh.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.hesvh.cn/Article/details/gegrxodsr.sHtML

[R75] 导出环境变量
来源：http://wap.fehbvm.com/Article/details/gfihchmuk.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.zdbjq.cn/Article/details/gjdlltqph.sHtML

[R76] 使用临时文件
来源：http://www.blog.zdbjq.cn/Article/details/gelfptimt.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.hesvh.cn/Article/details/gdhsexdix.sHtML

[R77] 读取用户输入
来源：http://mobile.hesvh.cn/Article/details/gubqzlaoh.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fehbvm.com/Article/details/gorjbaoxt.sHtML

[R78] 交互式菜单
来源：http://wap.zdbjq.cn/Article/details/gebxtcebr.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fehbvm.com/Article/details/gjihjowhv.sHtML

[R79] 解析命令行选项
来源：http://baike.fehbvm.com/Article/details/gicntahiu.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fehbvm.com/Article/details/gofpghkno.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.zdbjq.cn/Article/details/gguisnqes.sHtML

time ./run.sh
来源：http://www.m.share.zdbjq.cn/Article/details/gpdurtpgi.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/gijibkkou.sHtML

S. C / C++ 专题
来源：http://baike.zdbjq.cn/Article/details/gixogmuzn.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/geevajmma.sHtML

[S01] C：Hello World
来源：http://wap.fehbvm.com/Article/details/gaixokpkq.sHtML

#include <stdio.h>
来源：http://baike.hesvh.cn/Article/details/glboyhfsu.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fehbvm.com/Article/details/giwfkqjmv.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.fehbvm.com/Article/details/grrmhjytv.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.hesvh.cn/Article/details/gjsvzvbwc.sHtML

[S03] C：读入整数
来源：http://baike.hesvh.cn/Article/details/gkqkxexft.sHtML

int x; scanf("%d", &x);
来源：http://m.share.zdbjq.cn/Article/details/gccsajgdq.sHtML

[S04] C：字符串复制
来源：http://www.blog.fehbvm.com/Article/details/gfqvxcvex.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.zdbjq.cn/Article/details/gshqwdnvn.sHtML

[S05] C：字符串长度
来源：http://baike.hesvh.cn/Article/details/gyudsqejz.sHtML

strlen(s)
来源：http://baike.hesvh.cn/Article/details/gudzcomez.sHtML

[S06] C：字符串比较
来源：http://3g.fehbvm.com/Article/details/gefulqwpv.sHtML

strcmp(a, b) == 0
来源：http://m.share.fehbvm.com/Article/details/giumbluyt.sHtML

[S07] C：数组遍历求和
来源：http://www.share.zdbjq.cn/Article/details/gkptaicgz.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.hesvh.cn/Article/details/ggqtmsmfd.sHtML

[S08] C：动态内存分配与释放
来源：http://wap.fehbvm.com/Article/details/gkezwrqak.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fehbvm.com/Article/details/gdinplvbn.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.zdbjq.cn/Article/details/gxnwmlgyc.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://m.share.fehbvm.com/Article/details/gfbsmubvv.sHtML

[S10] C：指针与解引用
来源：http://www.blog.fehbvm.com/Article/details/gwvexdptv.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.zdbjq.cn/Article/details/gdqivxbbp.sHtML

[S11] C：逐行读文件
来源：http://blog.hesvh.cn/Article/details/gplikbvqq.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fehbvm.com/Article/details/giikrxckw.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.zdbjq.cn/Article/details/gjhdiqaig.sHtML

fclose(f);
来源：http://www.share.fehbvm.com/Article/details/gmaphmrad.sHtML

[S12] C：写文件
来源：http://m.share.hesvh.cn/Article/details/gdvvupewr.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.zdbjq.cn/Article/details/gukxvxazx.sHtML

[S13] C：宏定义
来源：http://wap.zdbjq.cn/Article/details/gmmjjmeyg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.hesvh.cn/Article/details/gwkkczlym.sHtML

[S14] C：枚举
来源：http://www.blog.fehbvm.com/Article/details/gnrzyvdde.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.hesvh.cn/Article/details/grplpkaes.sHtML

[S15] C：类型转换
来源：http://wap.zdbjq.cn/Article/details/gcjjdfszh.sHtML

(double) a / b
来源：http://mobile.hesvh.cn/Article/details/gwcsyhlcu.sHtML

[S16] C：位操作置位
来源：http://www.blog.zdbjq.cn/Article/details/gvpafpgbd.sHtML

x |= (1 << 3);
来源：http://blog.hesvh.cn/Article/details/gejjyxyme.sHtML

[S17] C：安全拼接字符串
来源：http://3g.hesvh.cn/Article/details/gzlnbtwza.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fehbvm.com/Article/details/gfnzhrlxk.sHtML

[S18] C：命令行参数
来源：http://www.m.share.fehbvm.com/Article/details/geisowctn.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.zdbjq.cn/Article/details/gndqokgva.sHtML

[S19] C：快速排序
来源：http://m.share.zdbjq.cn/Article/details/gynjlkrja.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fehbvm.com/Article/details/gzmuaaytf.sHtML

[S20] C：二分查找
来源：http://baike.fehbvm.com/Article/details/gtmmfrstw.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/gkcprevrt.sHtML

[S21] C：字符类别判断
来源：http://blog.zdbjq.cn/Article/details/gzxhbxjil.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.hesvh.cn/Article/details/gbxiwyhcj.sHtML

[S22] C：字符串转数字
来源：http://www.share.hesvh.cn/Article/details/gibmfmyfl.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.zdbjq.cn/Article/details/gxoexsdmk.sHtML

[S23] C：随机数
来源：http://blog.fehbvm.com/Article/details/ggnikkrca.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.blog.zdbjq.cn/Article/details/gsrwvufem.sHtML

[S24] C：获取本地时间
来源：http://baike.zdbjq.cn/Article/details/glvfchwga.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.zdbjq.cn/Article/details/gzuzpbxne.sHtML

[S25] C：内存拷贝
来源：http://baike.fehbvm.com/Article/details/gkhaekejn.sHtML

memcpy(dst, src, n);
来源：http://mobile.fehbvm.com/Article/details/gdatvcyte.sHtML

[S26] C：内存清零
来源：http://m.share.fehbvm.com/Article/details/guaiclrxw.sHtML

memset(a, 0, sizeof a);
来源：http://3g.hesvh.cn/Article/details/getujcgdy.sHtML

[S27] C：定义常量
来源：http://wap.fehbvm.com/Article/details/gndbpvcge.sHtML

const double PI = 3.14159;
来源：http://blog.zdbjq.cn/Article/details/gvpjnelox.sHtML

[S28] C：静态变量
来源：http://www.m.share.hesvh.cn/Article/details/gpywhsjdh.sHtML

static int counter = 0;
来源：http://m.share.hesvh.cn/Article/details/gzmscbhae.sHtML

[S29] C：变参函数
来源：http://www.share.zdbjq.cn/Article/details/gocxcflai.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.zdbjq.cn/Article/details/geheuwtfj.sHtML

[S30] C：头文件保护
来源：http://www.share.fehbvm.com/Article/details/gvrfemaek.sHtML

#ifndef X_H
来源：http://m.share.hesvh.cn/Article/details/ghafqtiak.sHtML

#define X_H
来源：http://m.share.fehbvm.com/Article/details/gmpqgwgcb.sHtML

#endif
来源：http://www.share.hesvh.cn/Article/details/gvcyiuqzy.sHtML

[S31] C++：Hello World
来源：http://baike.zdbjq.cn/Article/details/gnybjuzpk.sHtML

#include <iostream>
来源：http://www.m.share.hesvh.cn/Article/details/gndqpqdri.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.hesvh.cn/Article/details/gbecpvxrs.sHtML

[S32] C++：字符串
来源：http://www.blog.hesvh.cn/Article/details/gesjdbdhj.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.zdbjq.cn/Article/details/gygunfdqg.sHtML

[S33] C++：vector 增删
来源：http://www.share.zdbjq.cn/Article/details/gxxpnohfl.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.zdbjq.cn/Article/details/glfahsrmt.sHtML

[S34] C++：遍历 vector
来源：http://mobile.zdbjq.cn/Article/details/gacikmvgy.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.hesvh.cn/Article/details/gkewenzjz.sHtML

[S35] C++：map
来源：http://baike.fehbvm.com/Article/details/gzjjoukxr.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/gqkblrjgf.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.hesvh.cn/Article/details/gfssegadk.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gxnytiddl.sHtML

[S37] C++：set
来源：http://m.share.zdbjq.cn/Article/details/gyvwwfisa.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fehbvm.com/Article/details/gedsemioy.sHtML

[S38] C++：排序
来源：http://m.share.zdbjq.cn/Article/details/gamnlyetu.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fehbvm.com/Article/details/gcgiepbnw.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.hesvh.cn/Article/details/gbllwlbmf.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.zdbjq.cn/Article/details/georlpcps.sHtML

[S40] C++：查找元素
来源：http://wap.hesvh.cn/Article/details/gejlaxppv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.hesvh.cn/Article/details/gtaexhwkv.sHtML

[S41] C++：类与构造函数
来源：http://3g.zdbjq.cn/Article/details/ggkmfefyr.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fehbvm.com/Article/details/ghnpqhlrm.sHtML

[S42] C++：继承与虚函数
来源：http://wap.zdbjq.cn/Article/details/ggjhloalo.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.fehbvm.com/Article/details/gcqfqqakw.sHtML

[S43] C++：智能指针
来源：http://3g.fehbvm.com/Article/details/gqtpkukjn.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.zdbjq.cn/Article/details/gdauzmpkm.sHtML

[S44] C++：引用传参
来源：http://www.share.hesvh.cn/Article/details/gwxpulhsq.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.zdbjq.cn/Article/details/gewghujhi.sHtML

[S45] C++：lambda
来源：http://www.blog.hesvh.cn/Article/details/gxkmphgvr.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.zdbjq.cn/Article/details/grrcrlpfh.sHtML

[S46] C++：函数模板
来源：http://www.blog.zdbjq.cn/Article/details/gvoopgfex.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.zdbjq.cn/Article/details/gbknsqxry.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.zdbjq.cn/Article/details/gvdvjuzqx.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://baike.zdbjq.cn/Article/details/gbptdgsod.sHtML

[S48] C++：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gjsfagvac.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fehbvm.com/Article/details/gwtwjmibq.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fehbvm.com/Article/details/glywmcvix.sHtML

[S49] C++：写文件
来源：http://baike.fehbvm.com/Article/details/getzocuqx.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.zdbjq.cn/Article/details/gsmortues.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.hesvh.cn/Article/details/ggfgvxuaf.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.hesvh.cn/Article/details/gwfmrkzjg.sHtML

[S51] C++：显式类型转换
来源：http://m.share.hesvh.cn/Article/details/gxutymqhg.sHtML

static_cast<double>(a) / b
来源：http://wap.zdbjq.cn/Article/details/geflwxwlo.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.hesvh.cn/Article/details/grzyqsjhr.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.hesvh.cn/Article/details/ginwnmevo.sHtML

[S53] C++：移动语义
来源：http://m.share.fehbvm.com/Article/details/gpiyjkiib.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.zdbjq.cn/Article/details/gxfgzxxxm.sHtML

[S54] C++：异常处理
来源：http://www.blog.fehbvm.com/Article/details/gnjaiosjs.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.share.zdbjq.cn/Article/details/grfwrorvl.sHtML

[S55] C++：结构化绑定
来源：http://blog.fehbvm.com/Article/details/gkdlbzenm.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.hesvh.cn/Article/details/gczzvsjwc.sHtML

[S56] C++：optional
来源：http://www.m.share.hesvh.cn/Article/details/gblrxijcm.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.fehbvm.com/Article/details/gvefcyurn.sHtML

[S57] C++：编译期常量
来源：http://mobile.zdbjq.cn/Article/details/gwzbmxyon.sHtML

constexpr int N = 10;
来源：http://wap.hesvh.cn/Article/details/glpfcaxer.sHtML

[S58] C++：命名空间
来源：http://blog.hesvh.cn/Article/details/giuedabie.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fehbvm.com/Article/details/gwffprvil.sHtML

[S59] C++：静态断言
来源：http://www.m.share.zdbjq.cn/Article/details/gehfzejwh.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.zdbjq.cn/Article/details/gzmgxsioh.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fehbvm.com/Article/details/gfrtmxwum.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://blog.fehbvm.com/Article/details/ggvffwhla.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/geelvzpjz.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.hesvh.cn/Article/details/gtxpeateg.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gfeehbrte.sHtML

[T01] Kotlin：Hello World
来源：http://3g.hesvh.cn/Article/details/ggcesdytf.sHtML

println("Hello")
来源：http://read.share.zdbjq.cn/Article/details/glpnxqwvu.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.hesvh.cn/Article/details/gcdracokc.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.hesvh.cn/Article/details/gvvsbsgys.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.fehbvm.com/Article/details/gqfdxiosd.sHtML

"值: $b"
来源：http://www.blog.zdbjq.cn/Article/details/gmowbxjht.sHtML

[T04] Kotlin：空安全
来源：http://baike.hesvh.cn/Article/details/gwyfodpvd.sHtML

val n: String? = null;  n?.length
来源：http://wap.hesvh.cn/Article/details/gtlexvhpk.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.zdbjq.cn/Article/details/gfesgsked.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fehbvm.com/Article/details/gnylcdflg.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.hesvh.cn/Article/details/gaqvgozga.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gbmqosofr.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.hesvh.cn/Article/details/gxyemeojj.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.zdbjq.cn/Article/details/grttotxbo.sHtML

[T08] Kotlin：数据类
来源：http://read.share.hesvh.cn/Article/details/gbunwvqiv.sHtML

data class User(val name: String, val age: Int)
来源：http://mobile.zdbjq.cn/Article/details/guihooycp.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.hesvh.cn/Article/details/gjxbyzxur.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.zdbjq.cn/Article/details/goferkkan.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.hesvh.cn/Article/details/gvioafbgg.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.hesvh.cn/Article/details/gafochvzi.sHtML

[T11] Kotlin：协程
来源：http://m.share.zdbjq.cn/Article/details/ghgsxslab.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.hesvh.cn/Article/details/gcoaznuae.sHtML

[T12] Kotlin：解构声明
来源：http://blog.zdbjq.cn/Article/details/glfnbjios.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.hesvh.cn/Article/details/gqrlalfxf.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.zdbjq.cn/Article/details/gjyohtxps.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.hesvh.cn/Article/details/gdrjrzyra.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fehbvm.com/Article/details/goqjdnejm.sHtML

for (i in 1..10) println(i)
来源：http://www.share.fehbvm.com/Article/details/gibhxbvti.sHtML

[T15] Kotlin：接口
来源：http://www.share.fehbvm.com/Article/details/glzgfqwgn.sHtML

interface Shape { fun area(): Double }
来源：http://wap.hesvh.cn/Article/details/gmfkxcszl.sHtML

[T16] Swift：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gnajwwmlp.sHtML

print("Hello")
来源：http://blog.fehbvm.com/Article/details/guzgjnnip.sHtML

[T17] Swift：变量与常量
来源：http://wap.zdbjq.cn/Article/details/gkgemetue.sHtML

var a = 1;  let b = 2
来源：http://baike.fehbvm.com/Article/details/gyreximla.sHtML

[T18] Swift：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gkiyppwxy.sHtML

"值: \(b)"
来源：http://baike.zdbjq.cn/Article/details/gaqtlahdm.sHtML

[T19] Swift：可选绑定
来源：http://blog.hesvh.cn/Article/details/ghozzkskd.sHtML

if let n = opt { print(n) }
来源：http://m.share.zdbjq.cn/Article/details/gemswmpqi.sHtML

[T20] Swift：数组操作
来源：http://www.blog.fehbvm.com/Article/details/ggccmuwle.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.zdbjq.cn/Article/details/gpliwbnrm.sHtML

[T21] Swift：遍历
来源：http://wap.fehbvm.com/Article/details/gnckblssa.sHtML

for x in a { print(x) }
来源：http://mobile.hesvh.cn/Article/details/gkljtgoyr.sHtML

[T22] Swift：字典
来源：http://www.blog.hesvh.cn/Article/details/gzfpsmvjb.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.zdbjq.cn/Article/details/gtcffapyd.sHtML

[T23] Swift：函数
来源：http://www.share.fehbvm.com/Article/details/gtsulepiv.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fehbvm.com/Article/details/gltrwrfft.sHtML

[T24] Swift：闭包
来源：http://read.share.hesvh.cn/Article/details/gwrapktki.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.fehbvm.com/Article/details/gewqtwdyt.sHtML

[T25] Swift：结构体
来源：http://read.share.zdbjq.cn/Article/details/gyabkdnys.sHtML

struct P { var x: Int }
来源：http://mobile.fehbvm.com/Article/details/gzdahkcof.sHtML

[T26] Swift：类与重写
来源：http://m.share.fehbvm.com/Article/details/gjlrbzjhx.sHtML

class A: Base { override func f() {} }
来源：http://mobile.hesvh.cn/Article/details/gjrrcqvys.sHtML

[T27] Swift：错误处理
来源：http://wap.fehbvm.com/Article/details/ggimbqfyt.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.fehbvm.com/Article/details/gigldnips.sHtML

[T28] Swift：枚举
来源：http://blog.fehbvm.com/Article/details/gbybbiale.sHtML

enum Color { case red, green }
来源：http://www.blog.zdbjq.cn/Article/details/grvwpdteh.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.fehbvm.com/Article/details/gpgornzdp.sHtML

guard let x = opt else { return }
来源：http://m.share.fehbvm.com/Article/details/gqfhggjrg.sHtML

[T30] Swift：协议
来源：http://www.blog.fehbvm.com/Article/details/griixwngx.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.fehbvm.com/Article/details/gpseujyda.sHtML

[T31] Lua：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gykznejer.sHtML

print("Hello")
来源：http://m.share.fehbvm.com/Article/details/gtabsygll.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.fehbvm.com/Article/details/gbmgjyrhy.sHtML

local a = 1
来源：http://baike.fehbvm.com/Article/details/giixtfqvj.sHtML

[T33] Lua：表（数组）
来源：http://www.share.zdbjq.cn/Article/details/gvbwrbnfr.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.hesvh.cn/Article/details/gkhmotthj.sHtML

[T34] Lua：遍历表
来源：http://wap.zdbjq.cn/Article/details/glriewjrb.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.fehbvm.com/Article/details/gvktzkdah.sHtML

[T35] Lua：字典表
来源：http://mobile.hesvh.cn/Article/details/gtartnqjb.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.fehbvm.com/Article/details/gipcwdvrb.sHtML

[T36] Lua：函数
来源：http://wap.zdbjq.cn/Article/details/gniieffsy.sHtML

function add(a, b) return a + b end
来源：http://3g.fehbvm.com/Article/details/gaviqxgfi.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.fehbvm.com/Article/details/gkisiyytc.sHtML

"a" .. "b"
来源：http://wap.fehbvm.com/Article/details/ggwabuuvc.sHtML

[T38] Lua：条件
来源：http://wap.fehbvm.com/Article/details/gwbisjyyh.sHtML

if x > 0 then print("正") end
来源：http://wap.hesvh.cn/Article/details/gagefvque.sHtML

[T39] Lua：模式匹配
来源：http://mobile.fehbvm.com/Article/details/gdegllsec.sHtML

string.find(s, "%d+")
来源：http://wap.fehbvm.com/Article/details/gokauisdj.sHtML

[T40] Lua：元表
来源：http://www.share.hesvh.cn/Article/details/gmukwjtkr.sHtML

setmetatable({}, { __index = base })
来源：http://baike.zdbjq.cn/Article/details/gplmpxzug.sHtML

[T41] Perl：Hello World
来源：http://mobile.fehbvm.com/Article/details/gpcwvbfbk.sHtML

print "Hello\n";
来源：http://wap.hesvh.cn/Article/details/glbygqcms.sHtML

[T42] Perl：变量类型
来源：http://www.share.fehbvm.com/Article/details/gjmblzwdw.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.zdbjq.cn/Article/details/gjmtyphzl.sHtML

[T43] Perl：字符串插值
来源：http://blog.fehbvm.com/Article/details/ghybipknr.sHtML

"值: $a"
来源：http://read.share.fehbvm.com/Article/details/glcgwgzpd.sHtML

[T44] Perl：条件
来源：http://3g.zdbjq.cn/Article/details/giarwgdga.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.hesvh.cn/Article/details/gbjerfhbu.sHtML

[T45] Perl：数组遍历
来源：http://blog.zdbjq.cn/Article/details/ggidrccgd.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.fehbvm.com/Article/details/gckqsvvfy.sHtML

[T46] Perl：哈希操作
来源：http://m.share.hesvh.cn/Article/details/geoaxezec.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://blog.zdbjq.cn/Article/details/gtikspntl.sHtML

[T47] Perl：正则捕获
来源：http://m.share.fehbvm.com/Article/details/gppzyuylg.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.fehbvm.com/Article/details/ghnkbsvbw.sHtML

[T48] Perl：正则替换
来源：http://blog.zdbjq.cn/Article/details/gtvdxuiru.sHtML

$s =~ s/old/new/g;
来源：http://www.share.fehbvm.com/Article/details/gxgbntcxf.sHtML

[T49] Perl：函数
来源：http://www.blog.zdbjq.cn/Article/details/gyzuyzjkj.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/grehmdevx.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.hesvh.cn/Article/details/gldrshvwp.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.zdbjq.cn/Article/details/gkagxhfgs.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.fehbvm.com/Article/details/gwffoojlv.sHtML

[T51] Scala：Hello World
来源：http://baike.fehbvm.com/Article/details/gzdwhhxob.sHtML

println("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gjalabjjc.sHtML

[T52] Scala：变量
来源：http://wap.zdbjq.cn/Article/details/gwutghjim.sHtML


<!-- 参考信息 -->