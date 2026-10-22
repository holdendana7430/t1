代发 wailian999

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2wvxyduje.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2lgrzcbwc.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2xbffopvr.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2fpiaoiff.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2gytmvdci.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2pquxmsap.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2acwgrykz.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2dhbcfwxq.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2tfjckkke.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2rifkzinr.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2wvqkqnmk.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2kmhwnsse.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2ayervxzm.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2glwxbgqk.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2pfzvgire.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2ywuusond.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2cosnjgwj.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2djlflrws.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2bxeluakd.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2zvcdwfro.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2dqkwndil.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2brlqpcev.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2sustgvco.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2awmoqgpo.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2yyxpbkwn.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2agicfnzq.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2dkslcrgc.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2ienyxldy.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2qrdxeaix.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2qhfdcrox.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2lavyntyn.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2tzemydfr.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2hcasndgf.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2hzirxkvm.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2hpltgsjn.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2juwpvsli.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2nzyukles.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2tnkftojp.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2dvzkknmx.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2mwhzzpxc.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2qejaaomb.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2lcftiitv.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2ygqzepud.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cekgowps.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2fzpvtgxm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fqthacvx.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2vuvxcdxh.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2bottuslw.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2afwsablp.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2ichhdmxl.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2dpctmutm.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2oekfsqrw.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2qfrduuwg.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2nzwtnrvz.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2vzuglwov.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2nfkxlice.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2iylldpqe.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2eczmzzrk.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2bjrzjrhz.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2nlpurcyb.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2fodlyxyq.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2vqtfayry.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2stffjnar.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2tmtnwkvf.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2exypvyym.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2kzmmxsnx.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2nijbroxp.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2jjogywid.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2synffpqc.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2exfklxzs.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2khvwylfk.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2tstqbjnp.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2uucyctsf.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2xmfzfrbw.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2hfztacid.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2oktyroed.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2uzjxkfvu.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2zzrmuvna.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2nypzbuhi.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2ddzqbbwg.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2yohutzzc.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2atyhmhgy.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2lzsnbung.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2rhovgjcy.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2smyydvmt.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2oemtieqn.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2sgqauutl.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2blhkbcox.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2kdpufroi.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2hlcnqsiv.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2jdciuzui.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2jmwbmjfm.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2uaetmgor.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2hwlrlylm.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2ulzubvgk.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2blrpmpem.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2rhljmycu.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2aekhkipb.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2prhenayt.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2lbqfddnn.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2axrxrfub.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2anhuuull.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2wpzrhdfg.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2fslriknp.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2wybuptnq.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2amyejgrj.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2tpifhonz.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2cebypbnk.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2rtzchlrj.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2lwqdqchw.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2hsjvhhnn.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ivjppslk.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2jxncezwa.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2edeaknje.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2gsaxzltp.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2umpulzuq.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2zsuivuyv.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2obdbbjkm.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2dxfxlyfi.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2iyxoqxsv.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2gorizhvn.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2jjnfdzws.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2yzohvyxr.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2qtotuskf.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2ycuxzopl.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2rehstjji.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2ufzaixsx.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2ssmvwtze.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2eforilhz.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2oioepipr.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2pknbzuzl.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2aazrcsec.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2nxguzrva.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2ryuqcwvf.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2eulnvfan.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2vymylrpy.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt2iiwgzcau.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2fdbrjcjt.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2gtpzpjcn.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2xkmnhfxp.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2ccbabqcv.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2abypfqzx.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2toyfebrk.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2qmttakaw.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2dhhoomer.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2dtvowwyj.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2hgwvqabl.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2fermmrnv.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2ulcpxciy.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2ssrybjpw.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2wwquxlem.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2zrvqgjxv.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2kbntccrw.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2ysbaxsmx.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2gjjdsrfn.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2dqnniyiz.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2nkkjkodw.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2sqdbluyr.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2vyhlivpt.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2wbgimnbt.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2aomzmenh.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2pmrhldib.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2fplbjvgd.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2afzoqvuo.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2surbxvvd.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2wsjvgvaw.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2mmmgigpp.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2eopckxun.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2sqgnxelj.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2yqerrgzv.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2ynfiixxw.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2nfnmyvww.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2ddoxmkwd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ugfkblmh.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2aljslzyn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cbizoksq.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2mbyjdybf.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2vjhyqthb.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2hkdagywt.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2kvpkqavb.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2gwovicfc.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2stekuwiv.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2tphophsb.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2mwbcngkp.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2mnkzgcfe.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2aocghoop.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2jleabxya.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2pmhneapg.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2odyyaczj.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2swcvcqfd.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2tqxhzinu.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2yfglhuvn.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2emekjrup.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2rjcakamw.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2kutouerh.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2acdylaav.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2bybymkdb.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2alstjpdo.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2pzkuxstd.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2nhxjykvs.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2nmnmmidn.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2lpwfgrbu.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2wymcnbsf.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2irzzfeqf.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2wpqxypgd.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2xgjenahs.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ynzqmiuf.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2tsamabyh.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2jsgzygov.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2iganzltq.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2vuqljbye.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2ivcncqoe.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2yfxhdvys.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2qmuqxgjx.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2cvjfzbul.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2pevtbxtc.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2velilyel.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2inaxinds.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2vgqhndzt.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2zhpudmph.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2nsqazapj.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2zxgzttul.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2kdvsybwj.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2nhluqxgx.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2vgluuien.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2anxjqzve.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2jooqmmwn.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2xcvqoqkc.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2yrdobexg.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2dmfaouhp.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2uextrels.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2etvsdade.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2cudfznpc.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2yknzfxcc.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2hmoiprtw.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2fifvpqns.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2pzcqmfal.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2btutgavl.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2ccdbxyye.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2yavtrfxc.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2ktuclsvt.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2lbdynvjy.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2sctnxftl.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2ojesiqxk.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2bwpyfrbk.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2hvhdffcz.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2qntncdej.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2riawuogf.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2ynehqhcz.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2lvmusdpt.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2lkqcnqhg.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2xepdsbrt.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ljxjcoos.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2utwdoopv.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2avjskkrq.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2qfcwzobv.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2zgbavoxc.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2mgzuhrup.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2iziebdwl.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2xgyfbatn.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2byfsotxa.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2xnrsfsak.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2mdgqdyku.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ycynsxyx.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2nyfhmlgf.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2kkfigchr.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2foxrptqn.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2gopcinnu.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2tqkymrnu.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2vjjgiflz.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2jmqqjexs.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2nwaqichc.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2fmfppvxf.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2lvjwklet.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2zgeqwitx.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2whgbdkgu.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2jqetnkfs.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2kykhyngh.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ahgakdrj.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2eoadtnru.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2abdgfdyc.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ogfrpbbp.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2xkwksgcf.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2nzolyntk.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2dhxzdfwv.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2jzfgtekj.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2xserbbpn.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2qbcpgrjz.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2oajvyrxf.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2hwjcrhwd.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2bcqvalkl.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2sgjwxxhz.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2tfyyaher.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2monznyct.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2pvkriyrt.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2biregten.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.ydjk.org.cn/Article/details/gt2ooonxuee.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2rvmavnhi.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2cfebmaij.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qyotammg.html


<!-- 参考信息 -->