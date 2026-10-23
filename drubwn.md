代发 wailian999

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3qvetxjlx.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3latobedv.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3cvntbdlu.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3yoxmevhw.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3bxibjhxp.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3mppbcmsw.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3anrzazwf.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3nuilffsp.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3vlkwjncj.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3sfokslvb.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3cyeecaer.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3qezviffv.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3fimszyek.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3plyzoirf.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3qoisqutm.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3mfnsxasq.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3lrnawiay.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3kmnuabmx.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3iwtlhezz.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3vpfdnamc.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3cbpzktnj.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3xeqdmelm.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3sckzfglo.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3ijgvhtvl.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3zpbioamq.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3ajxezkqp.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zdmvnvlr.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3iowqwpkq.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3ksaeziux.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3ffuefeox.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3iorcafjq.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3yxjjvedc.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3yqdtvdjs.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3atlnlexy.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3mthbdoxm.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3cdjjzswo.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3mxplwrjh.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3xsbwlerr.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3solapfzx.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3dzgrbbbr.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3oorkszks.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3vqiaimna.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3yfvihrbn.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3rtpjgvpg.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3abkkqlro.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3jtapbnaj.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3duzeeixh.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3ghpaqwnu.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3zljbouoy.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3eeqqhssd.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3hapbzpzb.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3uwcdevzm.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3mkvmblnd.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bgkmjsnm.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3atqbmeat.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3rltmeudo.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3wmnpivxe.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3rkeqzees.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3ompzknac.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3sfyvvwlh.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3dllckxli.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3zlhrdbbj.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3ntllwkrs.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3sjjceplz.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3aubdjpcr.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3slmopfzm.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3gfqzgmdd.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3fuufewiu.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3lfjdemix.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3knxkrhuh.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3nhtijdyq.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3dytrylrx.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3mfusfzcq.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3wclzthia.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3umfqcode.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3kkwrhlgr.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3yjxedahp.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3tdtljobe.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3cpmgkirk.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3nhxteumq.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3ytwpkiwu.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3alwjdstk.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3lgglenje.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3infmbkja.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3jvmydrka.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3ipxuiucd.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3xopiwnfi.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3npaafpve.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3enrnpumd.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3tpruckan.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3elzsgfqx.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3dlixqroz.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3nvnawugi.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3vzyuvkmu.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3ufcudalk.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3lzwqtwgy.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3rzplamtk.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3ommilfeo.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3umrllnvw.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3hsxkqyyw.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3yvnfarsy.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3oycekfza.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3baeeueip.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3vyidqzgc.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3cznbpoyl.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3rmljykly.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3gtgzvtzo.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3kmezlopb.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3lzlgohpp.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3osgejwbd.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3mfeakmsm.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3uxxvkubj.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3xmddikhb.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3wehdsmbr.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3qkxxkuvr.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3tpirboks.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3qxbrblra.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3usqyzkum.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3ppyoyvxu.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vyuqgnrl.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3ddyqmtre.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3pjczhpvl.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3vseigeeo.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3hdqoofia.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3ccstwuny.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3umngevdj.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3gtdifgdx.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3uiqaxiip.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3rmtpreeh.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3edwordwd.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3pqqlvygu.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3wbtmnkar.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3snusjitj.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3kpmeiwji.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3rfqkksoc.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3iuxbberp.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3rfkuchfi.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3wflpdzgg.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3nsvfeqdn.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3tvrpmhyl.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3zsejyobc.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3vugkhaqa.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3eyxwebcs.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3xuevvdci.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3ncficvof.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3lewqzgig.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3ivqdclef.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3kyhksopi.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3mjklzdhu.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3pftyrexf.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3ycdpcjoe.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3rlhovxrc.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xdjirotr.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3qnfvtrsi.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3yqudjscq.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3thhabxmv.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3masdgjol.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3duukleei.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3qgoamfwj.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3weoofbin.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3aroytnxe.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3sqyhwjin.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3sebkjhbk.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3vurxlpxx.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3ffunamgt.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3hssgliqu.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3mufoylgi.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3lnmmcxxo.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ihjcuawx.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3wfoyobtk.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3eigyqotz.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3smvrutfi.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3bciuaivf.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3hkxrygkm.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3droenxyn.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3xkvurouf.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3riigienm.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3vavmjhtt.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3cfslnrur.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3tcgfbwmn.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3qwklhwlc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jvtkbect.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3hosudugz.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3chykhbgf.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3wjtvmsyr.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3gqmexxyd.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3kbbndusu.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3krnaltpr.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3cshpjzgp.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3umivmliv.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3wjbzuyzr.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3oqjgsyba.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3lbmvmpdk.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3msphsvog.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3yqxajlmp.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3gyqdcbeo.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3jprgyjpa.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3nhebqibu.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3fzljqkzv.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3vljohzjo.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3ndkjpkms.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3tieectdg.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3kvaqmvpc.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3xhkrxnaf.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3oxchbhlb.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3pvhrozin.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3rufiqobq.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3joidpivn.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3ebcnhftj.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3mzjhayxk.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3yzzoktvt.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3pjesgkra.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3aabnmsiq.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3cpgtgejv.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3lbndctin.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3xzhgcwut.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3uqyxhalv.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3mpadlxbg.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ifewvhkw.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3zqdwquuj.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3alklpklu.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3hplxcxol.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3qpcekqle.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3idcroatj.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3myxkcokh.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3jajbtswl.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3stjxakoo.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3jtpqmgeb.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3djysdjlg.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3bvceextf.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3tafgksqk.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3uqflcaqq.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3ygxwkrwz.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3smgunhqb.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3uwbsgwql.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3zqixezdv.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3bqstclgc.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3zoktrclv.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3yejcrmab.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3dgracwnb.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3xdayljus.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3yehnqkte.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3iqzaopxo.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3rmorhvvu.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3vmruizul.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3mjpveusy.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3frewliev.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3dkszocbf.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3jqdjdamz.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3wunajfni.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3fwzuwroc.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3svvscggl.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3zqysjgpc.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3yzijmltc.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3bozlreut.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3kptnxplw.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3jhmegsoq.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3zbdjuhyv.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3uaghawnd.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3nmyoxjtg.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3povipqid.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3emcrtwvv.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3jhtyraot.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3kfecbprg.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rdmlrmsz.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3tqtlwawr.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3zovexdlm.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3qqfkavml.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3effuiato.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3bmqnmfkp.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3tmghgmja.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3yherdlgr.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3xcdiiemf.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3tkhmluux.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3xwxuvkgw.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ukpiroxj.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3jcnuhqgf.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3gtyltdpx.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3jtwffpqf.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3tcavyiev.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3sviypsqi.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3hyrnekok.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3lvwovckz.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3ihvqxwew.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt3ktmimtpy.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rwlzkxnx.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3lhwlcqit.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3uduynnrx.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3kbqrrmsd.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ebmkabaw.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3ndsgkimv.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3znkuxjee.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3akpeqbep.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3brxvudjf.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3ptjqadhg.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3hrxughqi.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3uiygqjda.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3cvqvlfjy.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3epstqbfx.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3ntmrxglx.html


<!-- 参考信息 -->