代发 wailian999

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.hesvh.cn/Article/details/glnqixjlx.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.zdbjq.cn/Article/details/geygillkb.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://baike.hesvh.cn/Article/details/ggxzxqxbx.sHtML

[R61] 磁盘占用
来源：http://www.share.fehbvm.com/Article/details/gxwuahduh.sHtML

df -h;  du -sh *
来源：http://www.blog.fehbvm.com/Article/details/gundwvqlr.sHtML

[R62] 找最占空间的文件
来源：http://www.share.hesvh.cn/Article/details/gxxkkynuy.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.hesvh.cn/Article/details/gowzbqmss.sHtML

[R63] 内存与进程
来源：http://read.share.fehbvm.com/Article/details/ggfxhwsay.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.zdbjq.cn/Article/details/gysjhpvjx.sHtML

[R64] 结束进程
来源：http://read.share.hesvh.cn/Article/details/gglwzneke.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fehbvm.com/Article/details/gejithjmv.sHtML

[R65] 查看端口占用
来源：http://blog.hesvh.cn/Article/details/gtfbnmmrt.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.fehbvm.com/Article/details/gpuosalkm.sHtML

[R66] 定时任务
来源：http://www.share.zdbjq.cn/Article/details/ghnayvvmt.sHtML

crontab -e;  crontab -l
来源：http://blog.hesvh.cn/Article/details/gsyvmwrhu.sHtML

[R67] 生成随机十六进制串
来源：http://3g.hesvh.cn/Article/details/gjnwaeocq.sHtML

openssl rand -hex 16
来源：http://baike.hesvh.cn/Article/details/gffmyuljs.sHtML

[R68] 计算文件校验值
来源：http://blog.fehbvm.com/Article/details/gvkfhjwci.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.share.zdbjq.cn/Article/details/gxkeqotks.sHtML

[R69] 生成随机密码
来源：http://mobile.zdbjq.cn/Article/details/guxqnxvtq.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fehbvm.com/Article/details/gyqephlwm.sHtML

[R70] 时间戳与互转
来源：http://read.share.zdbjq.cn/Article/details/gpxxultgs.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fehbvm.com/Article/details/grpfijcmg.sHtML

[R71] 日期格式化
来源：http://m.share.hesvh.cn/Article/details/gmehfihkz.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.zdbjq.cn/Article/details/guhgyowyv.sHtML

[R72] 等待端口就绪
来源：http://3g.hesvh.cn/Article/details/gcykggcda.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fehbvm.com/Article/details/gmthibtlw.sHtML

[R73] 分割大日志
来源：http://mobile.fehbvm.com/Article/details/groemtado.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fehbvm.com/Article/details/garogifyg.sHtML

[R74] 批量重命名
来源：http://read.share.fehbvm.com/Article/details/gslwwhytf.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.fehbvm.com/Article/details/gcgxseiqg.sHtML

[R75] 导出环境变量
来源：http://wap.zdbjq.cn/Article/details/ghevfxyky.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.hesvh.cn/Article/details/gjtfcgayr.sHtML

[R76] 使用临时文件
来源：http://www.blog.hesvh.cn/Article/details/ggwicmylh.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fehbvm.com/Article/details/guzxkvatv.sHtML

[R77] 读取用户输入
来源：http://baike.fehbvm.com/Article/details/gsbnnndez.sHtML

read -rp "请输入: " ans
来源：http://baike.zdbjq.cn/Article/details/gbrpcuqea.sHtML

[R78] 交互式菜单
来源：http://www.blog.fehbvm.com/Article/details/gpsqfonbu.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.hesvh.cn/Article/details/gpzwfnzgj.sHtML

[R79] 解析命令行选项
来源：http://3g.fehbvm.com/Article/details/grhrgsmum.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.hesvh.cn/Article/details/gdessgbhw.sHtML

[R80] 查看脚本执行耗时
来源：http://read.share.zdbjq.cn/Article/details/gdqmjxaza.sHtML

time ./run.sh
来源：http://mobile.fehbvm.com/Article/details/gdppyanuc.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gljtfmpzx.sHtML

S. C / C++ 专题
来源：http://blog.zdbjq.cn/Article/details/gzpurnpif.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gyjihxasb.sHtML

[S01] C：Hello World
来源：http://read.share.fehbvm.com/Article/details/gecrwxxml.sHtML

#include <stdio.h>
来源：http://baike.zdbjq.cn/Article/details/gylvasknb.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fehbvm.com/Article/details/gdhptylah.sHtML

[S02] C：变量与格式化输出
来源：http://mobile.zdbjq.cn/Article/details/gazjrefpi.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fehbvm.com/Article/details/gesocxams.sHtML

[S03] C：读入整数
来源：http://mobile.hesvh.cn/Article/details/gmyvccvce.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.hesvh.cn/Article/details/gcacztbsp.sHtML

[S04] C：字符串复制
来源：http://read.share.hesvh.cn/Article/details/gvhrfajpg.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fehbvm.com/Article/details/gkyttpwpa.sHtML

[S05] C：字符串长度
来源：http://mobile.hesvh.cn/Article/details/gvsikruzm.sHtML

strlen(s)
来源：http://wap.zdbjq.cn/Article/details/gvnsvjefy.sHtML

[S06] C：字符串比较
来源：http://m.share.hesvh.cn/Article/details/gujohwsbj.sHtML

strcmp(a, b) == 0
来源：http://mobile.zdbjq.cn/Article/details/gaoeebnuv.sHtML

[S07] C：数组遍历求和
来源：http://mobile.hesvh.cn/Article/details/gawryikee.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.hesvh.cn/Article/details/gltfvjssb.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.hesvh.cn/Article/details/guwfwlmzy.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.zdbjq.cn/Article/details/gmaeupely.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.zdbjq.cn/Article/details/gnjsfohpk.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.hesvh.cn/Article/details/gtjksukcl.sHtML

[S10] C：指针与解引用
来源：http://www.blog.hesvh.cn/Article/details/gvzekraoe.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.zdbjq.cn/Article/details/gttuwkdkq.sHtML

[S11] C：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gxmgmpbkl.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.hesvh.cn/Article/details/gmvridoto.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fehbvm.com/Article/details/gwxzkzsaz.sHtML

fclose(f);
来源：http://wap.zdbjq.cn/Article/details/grtnzxawm.sHtML

[S12] C：写文件
来源：http://www.blog.zdbjq.cn/Article/details/ggewaayab.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.hesvh.cn/Article/details/gdkkfkboa.sHtML

[S13] C：宏定义
来源：http://blog.fehbvm.com/Article/details/ggmxjdjwr.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.hesvh.cn/Article/details/gzpvkezyl.sHtML

[S14] C：枚举
来源：http://3g.zdbjq.cn/Article/details/gwjkteryx.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.zdbjq.cn/Article/details/gcspdaody.sHtML

[S15] C：类型转换
来源：http://3g.hesvh.cn/Article/details/gqrikcsdq.sHtML

(double) a / b
来源：http://read.share.hesvh.cn/Article/details/gxpwzlhxr.sHtML

[S16] C：位操作置位
来源：http://www.share.zdbjq.cn/Article/details/gdgdfbehz.sHtML

x |= (1 << 3);
来源：http://3g.fehbvm.com/Article/details/gwarouraj.sHtML

[S17] C：安全拼接字符串
来源：http://3g.hesvh.cn/Article/details/gxkepkeah.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://blog.zdbjq.cn/Article/details/ggfqstxhs.sHtML

[S18] C：命令行参数
来源：http://mobile.zdbjq.cn/Article/details/gbdftvuuj.sHtML

int main(int argc, char **argv)
来源：http://read.share.fehbvm.com/Article/details/gmaxjjdql.sHtML

[S19] C：快速排序
来源：http://www.blog.hesvh.cn/Article/details/gfvzglgei.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.hesvh.cn/Article/details/ggojoryxi.sHtML

[S20] C：二分查找
来源：http://m.share.zdbjq.cn/Article/details/grtlsgpfh.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.blog.hesvh.cn/Article/details/guszannqh.sHtML

[S21] C：字符类别判断
来源：http://blog.zdbjq.cn/Article/details/gquvodpbc.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.fehbvm.com/Article/details/gsbgbukma.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fehbvm.com/Article/details/gintryufv.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.fehbvm.com/Article/details/gsbnuhkkt.sHtML

[S23] C：随机数
来源：http://wap.hesvh.cn/Article/details/gunpsqnkv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.zdbjq.cn/Article/details/gqxhrnihp.sHtML

[S24] C：获取本地时间
来源：http://3g.zdbjq.cn/Article/details/gyoltyklb.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fehbvm.com/Article/details/gpngolipv.sHtML

[S25] C：内存拷贝
来源：http://www.share.zdbjq.cn/Article/details/gxodmpsmy.sHtML

memcpy(dst, src, n);
来源：http://3g.hesvh.cn/Article/details/gwzxemdqm.sHtML

[S26] C：内存清零
来源：http://www.share.fehbvm.com/Article/details/gqcjkzrbr.sHtML

memset(a, 0, sizeof a);
来源：http://blog.hesvh.cn/Article/details/ggeqpnpcu.sHtML

[S27] C：定义常量
来源：http://www.share.fehbvm.com/Article/details/girlukskc.sHtML

const double PI = 3.14159;
来源：http://www.share.hesvh.cn/Article/details/gpakowxyr.sHtML

[S28] C：静态变量
来源：http://www.blog.zdbjq.cn/Article/details/gyuucsyxt.sHtML

static int counter = 0;
来源：http://www.blog.zdbjq.cn/Article/details/goturtfgr.sHtML

[S29] C：变参函数
来源：http://blog.zdbjq.cn/Article/details/gfwmdveqy.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.zdbjq.cn/Article/details/gkxndtqhp.sHtML

[S30] C：头文件保护
来源：http://baike.fehbvm.com/Article/details/gwjsgrsft.sHtML

#ifndef X_H
来源：http://www.share.hesvh.cn/Article/details/gwqirvwvr.sHtML

#define X_H
来源：http://www.m.share.zdbjq.cn/Article/details/gljelizhu.sHtML

#endif
来源：http://baike.hesvh.cn/Article/details/gtqbfvave.sHtML

[S31] C++：Hello World
来源：http://wap.hesvh.cn/Article/details/gsmqpbbar.sHtML

#include <iostream>
来源：http://blog.fehbvm.com/Article/details/gteiruhtv.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.fehbvm.com/Article/details/gtxndmdyx.sHtML

[S32] C++：字符串
来源：http://blog.zdbjq.cn/Article/details/gjyyxxuwt.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.hesvh.cn/Article/details/gveczgcrz.sHtML

[S33] C++：vector 增删
来源：http://mobile.zdbjq.cn/Article/details/gzfwqzlbr.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fehbvm.com/Article/details/gdxsrstkc.sHtML

[S34] C++：遍历 vector
来源：http://www.blog.fehbvm.com/Article/details/gvkbrgchd.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fehbvm.com/Article/details/ggzhbwtuz.sHtML

[S35] C++：map
来源：http://baike.hesvh.cn/Article/details/gejdwxpev.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gzvnaqjts.sHtML

[S36] C++：unordered_map
来源：http://read.share.hesvh.cn/Article/details/gedjwbqqu.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.hesvh.cn/Article/details/gksurvbig.sHtML

[S37] C++：set
来源：http://www.blog.zdbjq.cn/Article/details/gwoicfpxg.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fehbvm.com/Article/details/gyuzcsziv.sHtML

[S38] C++：排序
来源：http://m.share.fehbvm.com/Article/details/gwbzayvpu.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fehbvm.com/Article/details/gbianaplv.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.hesvh.cn/Article/details/gpiryoxuh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.fehbvm.com/Article/details/gpfeevrhf.sHtML

[S40] C++：查找元素
来源：http://www.blog.zdbjq.cn/Article/details/gkmnnywix.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fehbvm.com/Article/details/gcoiskmln.sHtML

[S41] C++：类与构造函数
来源：http://baike.zdbjq.cn/Article/details/gpacoghtv.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.hesvh.cn/Article/details/gydlhieae.sHtML

[S42] C++：继承与虚函数
来源：http://wap.zdbjq.cn/Article/details/grppdhiwm.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fehbvm.com/Article/details/gqylsttuz.sHtML

[S43] C++：智能指针
来源：http://blog.fehbvm.com/Article/details/gdffohplr.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.zdbjq.cn/Article/details/gratxmzbq.sHtML

[S44] C++：引用传参
来源：http://3g.fehbvm.com/Article/details/gjetncurk.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fehbvm.com/Article/details/ghqgroccm.sHtML

[S45] C++：lambda
来源：http://www.m.share.zdbjq.cn/Article/details/gbsrkcymu.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.fehbvm.com/Article/details/gkzzleorr.sHtML

[S46] C++：函数模板
来源：http://baike.zdbjq.cn/Article/details/gtioeopbd.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.hesvh.cn/Article/details/gpcvmhfah.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.zdbjq.cn/Article/details/gcwrwmujx.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fehbvm.com/Article/details/gsxbhpuei.sHtML

[S48] C++：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gmnugpbkj.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.zdbjq.cn/Article/details/grlqtrdjm.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.hesvh.cn/Article/details/gsfyqzivg.sHtML

[S49] C++：写文件
来源：http://read.share.hesvh.cn/Article/details/gnzogzkcp.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.hesvh.cn/Article/details/gbyqjqgjs.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fehbvm.com/Article/details/gtkefwvku.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fehbvm.com/Article/details/gnrtsglub.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.fehbvm.com/Article/details/gfmiggogk.sHtML

static_cast<double>(a) / b
来源：http://baike.zdbjq.cn/Article/details/gpxtechwn.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.zdbjq.cn/Article/details/gxtysxhdf.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fehbvm.com/Article/details/gndyrgfaz.sHtML

[S53] C++：移动语义
来源：http://www.blog.zdbjq.cn/Article/details/gsrrafncu.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.fehbvm.com/Article/details/gtqojhijs.sHtML

[S54] C++：异常处理
来源：http://mobile.zdbjq.cn/Article/details/gifrwldcm.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.hesvh.cn/Article/details/gweqefuos.sHtML

[S55] C++：结构化绑定
来源：http://baike.fehbvm.com/Article/details/gdhxtuchs.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fehbvm.com/Article/details/grmhmqyxb.sHtML

[S56] C++：optional
来源：http://read.share.hesvh.cn/Article/details/gfdnxgdms.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fehbvm.com/Article/details/gmknvjnmq.sHtML

[S57] C++：编译期常量
来源：http://www.blog.zdbjq.cn/Article/details/gnvljccxa.sHtML

constexpr int N = 10;
来源：http://baike.zdbjq.cn/Article/details/gaatccsgg.sHtML

[S58] C++：命名空间
来源：http://m.share.fehbvm.com/Article/details/gfabxsjbn.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fehbvm.com/Article/details/gefzceruo.sHtML

[S59] C++：静态断言
来源：http://3g.hesvh.cn/Article/details/gpfssglfi.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.fehbvm.com/Article/details/gjehfjrmn.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fehbvm.com/Article/details/gogshmtcx.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.fehbvm.com/Article/details/gxwpoynir.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/guvzpnthg.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fehbvm.com/Article/details/gmmkrjqxd.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gisrpoftj.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.fehbvm.com/Article/details/gcwsgvsoh.sHtML

println("Hello")
来源：http://3g.fehbvm.com/Article/details/gwklmdxgj.sHtML

[T02] Kotlin：变量
来源：http://baike.zdbjq.cn/Article/details/gvoysirnw.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.zdbjq.cn/Article/details/gooznkqvk.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.hesvh.cn/Article/details/grdaikmij.sHtML

"值: $b"
来源：http://www.m.share.hesvh.cn/Article/details/gwysitcuw.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.zdbjq.cn/Article/details/gcalzmbvw.sHtML

val n: String? = null;  n?.length
来源：http://3g.zdbjq.cn/Article/details/gkpssgmqq.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.hesvh.cn/Article/details/gppilchqq.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.zdbjq.cn/Article/details/gfatarzxz.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.fehbvm.com/Article/details/gnkacqiai.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.hesvh.cn/Article/details/glunkmgzt.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.zdbjq.cn/Article/details/gwhnkheyu.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fehbvm.com/Article/details/gphwjmgaz.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fehbvm.com/Article/details/gzzefsjpt.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.zdbjq.cn/Article/details/gjtxsjrdp.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.zdbjq.cn/Article/details/gbjpirijq.sHtML

fun String.exclaim() = this + "!"
来源：http://3g.hesvh.cn/Article/details/gmzpdhebb.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fehbvm.com/Article/details/gxpgtafih.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fehbvm.com/Article/details/gupcumryb.sHtML

[T11] Kotlin：协程
来源：http://m.share.hesvh.cn/Article/details/gmhngeyhg.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.zdbjq.cn/Article/details/gspvjpjvk.sHtML

[T12] Kotlin：解构声明
来源：http://blog.fehbvm.com/Article/details/gafhkyjsj.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gkzfgyuku.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.zdbjq.cn/Article/details/gihppomld.sHtML

val m = mapOf("a" to 1)
来源：http://baike.hesvh.cn/Article/details/ggvcthjve.sHtML

[T14] Kotlin：循环
来源：http://m.share.zdbjq.cn/Article/details/ghxqfexge.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fehbvm.com/Article/details/gvhyiwyrj.sHtML

[T15] Kotlin：接口
来源：http://baike.zdbjq.cn/Article/details/gylnxzfny.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.hesvh.cn/Article/details/gmgddrqwy.sHtML

[T16] Swift：Hello World
来源：http://m.share.zdbjq.cn/Article/details/ghozhvhzb.sHtML

print("Hello")
来源：http://read.share.hesvh.cn/Article/details/gcrlydqup.sHtML

[T17] Swift：变量与常量
来源：http://read.share.fehbvm.com/Article/details/gtugsnmcz.sHtML

var a = 1;  let b = 2
来源：http://wap.fehbvm.com/Article/details/ggasmgyot.sHtML

[T18] Swift：字符串插值
来源：http://mobile.fehbvm.com/Article/details/geikdlozj.sHtML

"值: \(b)"
来源：http://www.m.share.hesvh.cn/Article/details/gsuqilsfm.sHtML

[T19] Swift：可选绑定
来源：http://m.share.hesvh.cn/Article/details/grgdjmmcp.sHtML

if let n = opt { print(n) }
来源：http://www.share.zdbjq.cn/Article/details/gfkguouzt.sHtML

[T20] Swift：数组操作
来源：http://m.share.hesvh.cn/Article/details/gzlbzhtyu.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.hesvh.cn/Article/details/gqejanssu.sHtML

[T21] Swift：遍历
来源：http://wap.fehbvm.com/Article/details/gwhhleusm.sHtML

for x in a { print(x) }
来源：http://blog.fehbvm.com/Article/details/glbliklwy.sHtML

[T22] Swift：字典
来源：http://3g.hesvh.cn/Article/details/gikarcumf.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.zdbjq.cn/Article/details/gbwcajgek.sHtML

[T23] Swift：函数
来源：http://baike.zdbjq.cn/Article/details/gtxypxhdn.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.zdbjq.cn/Article/details/gsuxqundn.sHtML

[T24] Swift：闭包
来源：http://blog.zdbjq.cn/Article/details/gdzqsdgpp.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gbybcktlu.sHtML

[T25] Swift：结构体
来源：http://3g.hesvh.cn/Article/details/gpdiyswiy.sHtML

struct P { var x: Int }
来源：http://www.share.fehbvm.com/Article/details/gcfwovjcc.sHtML

[T26] Swift：类与重写
来源：http://read.share.zdbjq.cn/Article/details/ghqwignqa.sHtML

class A: Base { override func f() {} }
来源：http://www.share.fehbvm.com/Article/details/gcindzwwx.sHtML

[T27] Swift：错误处理
来源：http://baike.fehbvm.com/Article/details/ganbrkmyo.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.zdbjq.cn/Article/details/ggvpnizys.sHtML

[T28] Swift：枚举
来源：http://read.share.hesvh.cn/Article/details/ghtemoehx.sHtML

enum Color { case red, green }
来源：http://blog.fehbvm.com/Article/details/gnplimvnk.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.zdbjq.cn/Article/details/gqozgiwsr.sHtML

guard let x = opt else { return }
来源：http://3g.hesvh.cn/Article/details/gzhrpqwtk.sHtML

[T30] Swift：协议
来源：http://www.m.share.zdbjq.cn/Article/details/gousvbonn.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.fehbvm.com/Article/details/grywttihl.sHtML

[T31] Lua：Hello World
来源：http://blog.fehbvm.com/Article/details/gdzmncbvm.sHtML

print("Hello")
来源：http://www.share.zdbjq.cn/Article/details/grcjgneah.sHtML

[T32] Lua：局部变量
来源：http://read.share.fehbvm.com/Article/details/ghpnqdyvp.sHtML

local a = 1
来源：http://www.share.zdbjq.cn/Article/details/gupxlcmwc.sHtML

[T33] Lua：表（数组）
来源：http://www.share.zdbjq.cn/Article/details/gzyquxcyr.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://blog.hesvh.cn/Article/details/gnvzpqksn.sHtML

[T34] Lua：遍历表
来源：http://baike.zdbjq.cn/Article/details/gxffdjtpk.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.zdbjq.cn/Article/details/gkknokqjy.sHtML

[T35] Lua：字典表
来源：http://www.blog.fehbvm.com/Article/details/gqwaxrlbn.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gqxjvvtru.sHtML

[T36] Lua：函数
来源：http://mobile.fehbvm.com/Article/details/gjjwbgzcv.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.hesvh.cn/Article/details/gszksprut.sHtML

[T37] Lua：字符串拼接
来源：http://wap.fehbvm.com/Article/details/gtlggfkfv.sHtML

"a" .. "b"
来源：http://m.share.zdbjq.cn/Article/details/gfwtweaao.sHtML

[T38] Lua：条件
来源：http://www.m.share.fehbvm.com/Article/details/gpnatmcqs.sHtML

if x > 0 then print("正") end
来源：http://www.blog.zdbjq.cn/Article/details/gwfwgridq.sHtML

[T39] Lua：模式匹配
来源：http://blog.zdbjq.cn/Article/details/gnsadeozw.sHtML

string.find(s, "%d+")
来源：http://www.m.share.zdbjq.cn/Article/details/gmwbycmzq.sHtML

[T40] Lua：元表
来源：http://read.share.fehbvm.com/Article/details/gxdrlrexn.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.hesvh.cn/Article/details/gapgnfgmr.sHtML

[T41] Perl：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gndvssqeu.sHtML

print "Hello\n";
来源：http://www.share.fehbvm.com/Article/details/gfajseiyl.sHtML

[T42] Perl：变量类型
来源：http://m.share.fehbvm.com/Article/details/gbfmrqzba.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.zdbjq.cn/Article/details/giyfibbli.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gyqzfpzfb.sHtML

"值: $a"
来源：http://www.blog.hesvh.cn/Article/details/ggphwjxfi.sHtML

[T44] Perl：条件
来源：http://m.share.zdbjq.cn/Article/details/gsdyiomcr.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.zdbjq.cn/Article/details/gecbeikyl.sHtML

[T45] Perl：数组遍历
来源：http://blog.fehbvm.com/Article/details/gcxgzgcpv.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.hesvh.cn/Article/details/gwfhrvxhq.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.hesvh.cn/Article/details/gegjbyefg.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.fehbvm.com/Article/details/gubyilhks.sHtML

[T47] Perl：正则捕获
来源：http://3g.zdbjq.cn/Article/details/gnnljjmmq.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.hesvh.cn/Article/details/gvljbhavn.sHtML

[T48] Perl：正则替换
来源：http://wap.zdbjq.cn/Article/details/gjgckwmno.sHtML

$s =~ s/old/new/g;
来源：http://www.share.hesvh.cn/Article/details/glganscik.sHtML

[T49] Perl：函数
来源：http://blog.fehbvm.com/Article/details/gntwxrhwr.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gtvszcema.sHtML

[T50] Perl：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gyhzfddus.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.fehbvm.com/Article/details/gzpbempeq.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.fehbvm.com/Article/details/gbvroajlh.sHtML

[T51] Scala：Hello World
来源：http://blog.fehbvm.com/Article/details/ghkcsknqu.sHtML

println("Hello")
来源：http://3g.hesvh.cn/Article/details/gyamzzykg.sHtML

[T52] Scala：变量
来源：http://www.m.share.zdbjq.cn/Article/details/gacunmkal.sHtML

val a = 1;  var b = 2
来源：http://baike.hesvh.cn/Article/details/gyprbcdjm.sHtML

[T53] Scala：字符串插值
来源：http://www.blog.hesvh.cn/Article/details/getonqsay.sHtML

s"值: $b"
来源：http://blog.fehbvm.com/Article/details/gyujqaygb.sHtML

[T54] Scala：集合映射
来源：http://wap.hesvh.cn/Article/details/glzbglzgt.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.hesvh.cn/Article/details/gaxuypwlu.sHtML

[T55] Scala：集合过滤
来源：http://3g.fehbvm.com/Article/details/gxouazmrr.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.hesvh.cn/Article/details/gmxqpfsnr.sHtML

[T56] Scala：样例类
来源：http://baike.fehbvm.com/Article/details/ghcmmxfmc.sHtML

case class User(name: String, age: Int)
来源：http://m.share.hesvh.cn/Article/details/gylabbbih.sHtML

[T57] Scala：模式匹配
来源：http://3g.hesvh.cn/Article/details/gmiiunzmu.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://m.share.zdbjq.cn/Article/details/ggccqhhxw.sHtML

[T58] Scala：函数定义
来源：http://www.share.hesvh.cn/Article/details/gtrmqjhbq.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.fehbvm.com/Article/details/glqqftghp.sHtML

[T59] Scala：循环
来源：http://wap.hesvh.cn/Article/details/gidaemfxr.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fehbvm.com/Article/details/gknvydqkr.sHtML

[T60] Scala：折叠
来源：http://baike.zdbjq.cn/Article/details/ghmdcmkxy.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://blog.fehbvm.com/Article/details/grqmzujvm.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gwxxsrosl.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.zdbjq.cn/Article/details/gfjqjlqml.sHtML

================================================================================
来源：http://m.share.zdbjq.cn/Article/details/goyujnvww.sHtML


<!-- 参考信息 -->