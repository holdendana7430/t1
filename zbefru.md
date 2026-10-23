代发 wailian999

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.ydjk.org.cn/Article/details/gt3qindeynb.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3ksicdbny.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3bemsfgbg.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3ggfuitct.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3ndpgvvaz.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3vsloeoyy.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3fafxplvn.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ljzjalsc.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3ocqsphku.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3avoegurm.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3mgrarzcp.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3ywqzxiyv.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3xjwwvflt.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3vojtxqen.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3wdorevdk.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3sfedryjm.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3cerkftle.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3cvtnqbjk.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3tizqpxtv.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3ibwjrorq.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3fnuvglqb.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3farsoxcy.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3qgbmruwe.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3miuvqzui.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3xxhzwjkq.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3okirmypg.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3djaceigd.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3acgrpsyi.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3qhxnkufs.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3zeovnanb.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3srjktxem.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3fgwmmqfb.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3aspsmnbj.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3rzakoxyo.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3iiflrcvh.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3wxjifphm.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3izeddwws.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3frbbgxgh.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ecnpwkct.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3rqgrytdh.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3mdylrhud.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3ojtodvmk.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3spcobttd.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3skchsmig.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3blcjnjwy.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3jgzzewvd.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3igqsujvt.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3ofucdpsf.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3svmfdwzq.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3jehasngr.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3nuzkejuf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bcnswqri.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3cmnlaybi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3szgvrjkt.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3dntfydky.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3vaclrsmm.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3eaixdthc.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3cnankcuo.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3brwkufeh.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3ilzmfwlk.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3hxgxnxky.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3asxtkbtc.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3xloewmhu.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3bhphxuti.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3tbirmcof.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3wtezxoxi.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3pcuohgcs.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3quzisjxr.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3suhcwumz.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3eavpqzoe.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3fqtfnwqv.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3kwfrtczh.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3nmhcjsza.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3tdaurtwc.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3kmvissjc.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3eryjxnrv.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3lciyoane.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3jmzhpqxv.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3jrtzexuh.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3vcbktqhh.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3mwuqhkdb.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3iaaneyfa.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3eoudohpj.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3seiutjdb.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3afivhewt.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3qwhggmye.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3dvflzjgl.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3ynhteewt.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3gxwnpnvr.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ekqyavkg.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3npdiviug.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3fkvhbivn.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3rkmnzphq.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3rhpbjpsp.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3cvpkjkoy.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3unjqnvpu.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3bdlrtawn.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3iugbjihc.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3yoqvtwuc.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3rbfjbtrb.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3xtdrezai.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3rjqayndc.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3ianwmjfo.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3gwevrmnb.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3thiteasv.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3mkaylbfr.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3lmwfvqkj.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3mtxdqusv.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3ktefmayl.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3jtvyemtr.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3ukjigxry.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3grjyfmwo.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3zmtgnera.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3wotpzerc.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3valuoeht.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3qoerozcj.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3jgldmwvz.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3ashvuagy.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3hyzgtgnb.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ynllfmvs.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3pmpkwmpr.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3xujwlpni.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3myfvqcyx.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3vyizmosz.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3mjedgpur.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3kzefigdk.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3avexzexn.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3ugrtgnnc.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3uvkrthuk.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3dzbehyyr.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3acgntfob.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3ndexobdt.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3rmgbdapn.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3dhxwyoxm.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3vtbgnwgh.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3sbjahmhp.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3tgnwyedf.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3yedcckgn.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3hrcgowwo.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3kncwljkl.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3scvsvaxi.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3jgtnaexo.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3fhqrxvwa.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3rmcwyflh.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3qcmybxfn.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3pidaksol.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3oavoussa.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3stejfoey.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3dimhlksr.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3tnblfoje.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3elbttcab.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3ccvorxfn.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3mhyjbnrp.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3yhnutcvr.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3migbwwby.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3jptrcjtq.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3fceqckuy.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3ykipcyli.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3povooxhe.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3jmrbkhcz.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3tcztwvre.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3dttsmyso.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3bapbkvos.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3obqtpvev.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3mhaipyze.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3oqwccpyx.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3yxqekktr.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3rjszctri.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3upgtsini.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3zurhxgmc.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3ctifsbns.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3ozbyzlks.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3iikhyuui.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3aowxjdmd.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3tpkaebta.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3wfrsfmjq.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3qkisiyox.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3iwczifqz.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3fgnxdacp.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3rrnphbso.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3awavfxij.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hcdmteic.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3fhuhsnyq.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3hfdfjxce.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3pifigrzt.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3uylwptfl.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3qihdenjo.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3ipqupiao.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3ocopsjcd.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3ovsocjqv.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3pgzjyewt.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3bcqpwbdp.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3itjmkbub.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3dafvsdis.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3ixgvsbkt.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3yawilxgj.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3fwwchgep.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3fqrvrabb.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3sbxqaypf.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3wjbjnjkh.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3fflnjtai.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3hcopdkpv.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3tifnmaqf.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3tbnrzrwc.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3mjkhbvgl.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3iatsexzt.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3vxhhicxn.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3vevnynim.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3keplwapy.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3egcjbfea.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3umnrsrbk.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3pcmhslnl.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3rnqpmlvc.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3xmybjvcc.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3srfdopka.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3mjobugym.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3zltmbeiu.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3vokncurl.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3hvcxwyiv.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3foghpnia.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3gevxjoot.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3sqkmaxfl.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3ayqeaour.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3nrwhgysq.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3jgeunwjc.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3wnhwxjkr.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3qajzhwez.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3xgoooqhr.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3exixjezq.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3fazmvrnq.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3ryyfaoil.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ounqjvfp.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3txvgvdqo.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3guaxmldv.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3qzqxuiyj.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3cgwudeht.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3dstrfzvq.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3sovpuyrm.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3vgjatldq.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3gffvvqgm.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3xqoewjql.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3gwopwtso.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3yqfqqxds.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3fyiffnvg.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3zoixxrkf.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3tkhbiqpe.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3jlvcffsw.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3vnmmrjlb.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3afvidxhv.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3bcriwide.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3bsntitga.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3jedmsewc.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3bafvncqp.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3ztfufavf.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3xnpihjls.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3dyntenpo.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3wpuzznwz.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3zopssmbl.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3xfaklpqv.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3snptzmbt.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3xnqytlst.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3xldtpsrd.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3saqnjqbc.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3fahuwupx.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3dcwtizty.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3abbnsyde.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3vzdeovqz.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3aevpviwv.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ymdyoifs.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3zmacynjq.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3wzwksnco.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3bomesxeg.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3mgvfsjzn.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3prwmbpse.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3sqpymtmm.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kyhgvila.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3bqskhwvs.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3uakzojcc.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3ttnnaolf.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3ooajspux.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3zibwwsxd.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3pnbtroxn.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3rgrqpuir.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3nbynwbhg.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3dbdfjwkt.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3tyccxnut.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3aoilicqb.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3uadoroog.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3kqvatqyd.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3jrraoddy.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3jcrzldje.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3dwgwuixz.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3loxoqqtd.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3nsmoaedp.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3brjypwvw.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3mdlhmyix.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3xjnngtoo.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3bnvmfrpc.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3nrbykpnn.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3wvzccpyz.html


<!-- 参考信息 -->