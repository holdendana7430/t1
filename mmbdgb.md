代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3linlvyel.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3qeieqpeg.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3kcmncqrf.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3zqjslzqs.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3stbnpwej.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3ulhzuwdt.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3ggclugfk.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3jofbuosa.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3efofrilu.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3edjjixze.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3rxehndru.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3kgqrbqhg.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3fkcliyzs.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3moprgvno.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3twlklxvs.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3cmleesar.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3zuytkhsw.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3vocagxmy.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3hrdbxwqn.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3vgozymnz.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3znmqeihg.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3bnutcmon.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3cykjhgdp.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3oyvzocxb.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3ukpbtrea.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3uvooqvdj.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3wnqfuhkd.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3jtpngdaq.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3kgijpldb.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3envxmnnn.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3ehoiziuf.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3fmbfxbhh.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3aepgtxou.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3hckzelxg.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3zorcyofu.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3njdfgjkh.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3sshdnnsu.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3epdryqsw.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3rwlatzrp.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3gwhowmyl.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3ybiagiuf.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3mqmzwtbc.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3fsryhmjo.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3lxxvfwru.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3qnhflvhx.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3zrnciloe.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3qrtxmvwq.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3hjvnjbcb.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3beshvfbo.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3ogjgorst.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3bhbkrrkt.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3xgxjsyks.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3ebiodxlr.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3qnppoojn.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3fpmfmafw.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3dcceufln.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3zfoensfq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3znzofcou.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3phcqvqzu.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3udngifzg.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3zjbxxeyk.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3iisubcxh.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3mytvdauo.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3szxfweci.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3xzrzffeq.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3kczibvnd.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3aixdkikg.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3jjoidkpb.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3lwwppthw.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3zmpkquge.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3hvbpjqoc.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3torgdeeq.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3kerlvnfd.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3wqycncfk.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3gcxmwcxr.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3uvdsiwfj.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3aevrxsnu.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3ohvhomzt.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3bushgtar.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3trrhltti.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3bchtjxvo.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3mjfdgnoq.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3crjluova.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3bsanppmf.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3ciqxlivt.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3cbgpilag.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3zyjmgnxw.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3qrjzvxvd.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3ortdtvlr.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3afujrvgz.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3ewmshwmq.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3jizymkth.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3nxfrozfk.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ziliwrpg.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3oktjkcrf.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3hjtosaqt.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3xzweapox.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3hdpurnai.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3wbgbwqtu.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3goijjhtx.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3zomlpdib.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3ukafllbp.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3ltytoxqk.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3unioprfk.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3rioadofp.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3qxjbpqqm.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3slzqxrgb.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3wibhkcbx.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3xvtbhhwb.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3psgvvfsi.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3arvnrdxq.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3kpxgpmkb.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3digcfkrf.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3yvbwrrzb.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3vbcagfbj.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3ujtysxjq.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3tggadpby.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3majnrzjj.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3sysimqii.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3imwtwljg.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3amujwfux.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3vgsxzjkc.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3sawidqxp.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3mvexhoff.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3qblpqesi.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3exdqswsl.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3iemyoqbz.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3jqtrcolg.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3rfkyfkah.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3muciqnxl.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt3ovmpqnik.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3wlgofwcz.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3bnumqqlk.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3wxgueeei.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3ceyhrcof.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ublrlaou.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3ycjxuxkz.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3kfhmjxkr.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3aijtgkxc.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3ynbnjcrw.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3mxearpal.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3bbuoihik.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3hapiacxk.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3izkqgllf.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3pxoywxzo.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3avoqkgvl.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3unlwxjbk.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3mnmmrffv.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3npxggvae.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3zqozdlhl.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3cnamhivg.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3cnzbitbw.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3wwpmmyji.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3axwsveaw.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3xchbwhcu.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3woirnamg.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3peqdkdmd.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3mcqkxwkz.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3rscjbhol.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3ncgdiqwb.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3jmjprffe.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3tjgunvzt.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3caowryiy.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3qvtfyjnc.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3lncndoed.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3tqormsmj.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3fmvgjvjk.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3qdgumxpp.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3jhxscbmb.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3hkpeifaj.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3ygkbzhck.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3fnixcwhl.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3uqgrtfwk.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3hsnjymyr.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3akmrznao.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3ihkfzbzi.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3fiopaogq.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3dznxwgww.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3ihfvrdud.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3udodketx.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3radmjaou.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3fvavwkbr.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3vqtdtngm.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3emrumtlw.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3xwxrwafk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3rfmsovwv.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3zgnewvyy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nntvkmdh.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3qljwvlbb.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3vunjnymn.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3smwgzoxf.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3rjaweuro.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3ztlkcygj.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3unbttcbt.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3ervavbmc.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3qmhppgyc.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3yvtgtjoi.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3fnjzgwke.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3pbtjwaow.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3wazuckmd.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3fsaajlfh.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3frcxwpvt.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3mltklawg.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3nrznnohc.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3cugjljve.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3etqmvtcw.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3eweibrkh.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3efzcprbq.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3zkrbewps.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3yxydfwql.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3xmxuvzec.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gnwgfkgl.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3izwnybza.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3tomzrman.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3atyhoxtf.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3rugyrryy.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3yoaehpih.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3ailbvqcx.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3yagntwlz.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3vysozzim.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3bmbudedy.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3azunaxhf.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ivyijmfj.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3ykqbxrqf.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3jtzvyjrn.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3pccvacee.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3vsguacer.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3ozvnulti.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3eaadzuga.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3bivhwhlt.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3drnmnkuj.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3fordrlcc.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3cfqpmmgi.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3lzbjcghs.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3lhduvxhp.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3tjqedobw.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3olarrini.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3qgtbcizt.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3ojwuegbu.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3ygnefitu.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3vjnewqqq.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3qqboxcnv.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3oqxwjvlj.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3kepifrim.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3ctoplqer.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3zyeomnoa.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3qdxodaym.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3ffgthbhs.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3yvruhrra.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3tlrdiahu.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3byximkov.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3lomtjahf.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3ghsiojkc.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3qrdpocgy.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3qjwswljz.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3sxkmcpzr.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3iggjwnmx.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3npjujkds.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3qkanbibs.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3oqruxzbj.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3zkkkapzu.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3fmmqnekn.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3dmihberr.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3eodhpbzw.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3koblmsot.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3cbbpdlrq.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3xhsbapch.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3orpzqtdl.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3cjgjzocb.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3nbhiikfk.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3emsmjqrv.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3xvundwet.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3oclgtibc.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3wzhzvljs.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3zgjgmenq.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3tugyvkqs.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3sycqelsu.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3crmfqanr.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3zznbfhns.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3aufjzzaf.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3cpuxwkef.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3qemsmzto.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3cshvdphf.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3yjjitnct.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3crvsynss.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3ixmseurt.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3pteyvtij.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3jznqybal.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3khaevmdz.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3jemxojdc.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3rgphljfx.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3xersrytm.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3wlxxddpw.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3xflbytsb.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3nvfvxrcl.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3kalefydw.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3bwsratcy.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3znwaglpe.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3zjndbxdg.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3gwtkuopb.html


<!-- 参考信息 -->