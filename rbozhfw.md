代发 wailian999

ssh user@host 'uptime'
来源：http://mobile.zdbjq.cn/Article/details/gqiakmhgp.sHtML

[R58] 下载文件
来源：http://read.share.zdbjq.cn/Article/details/gueoarhtc.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.hesvh.cn/Article/details/gedjnfvos.sHtML

[R59] 发 POST JSON
来源：http://www.blog.hesvh.cn/Article/details/gzaieqhqy.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fehbvm.com/Article/details/gzeyrslnj.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.hesvh.cn/Article/details/gzxepssys.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.hesvh.cn/Article/details/gnisdhqrz.sHtML

[R61] 磁盘占用
来源：http://www.share.zdbjq.cn/Article/details/gvoufgkkd.sHtML

df -h;  du -sh *
来源：http://www.blog.zdbjq.cn/Article/details/gnpdwbico.sHtML

[R62] 找最占空间的文件
来源：http://wap.fehbvm.com/Article/details/ggfwcmdxe.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.zdbjq.cn/Article/details/geehydpmg.sHtML

[R63] 内存与进程
来源：http://www.blog.hesvh.cn/Article/details/grbuaguyg.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fehbvm.com/Article/details/gibupeitq.sHtML

[R64] 结束进程
来源：http://baike.zdbjq.cn/Article/details/gddiyiojf.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.zdbjq.cn/Article/details/grsgbcbnj.sHtML

[R65] 查看端口占用
来源：http://blog.fehbvm.com/Article/details/gffqcqepo.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.hesvh.cn/Article/details/gocextjyg.sHtML

[R66] 定时任务
来源：http://read.share.hesvh.cn/Article/details/gwbksxfxb.sHtML

crontab -e;  crontab -l
来源：http://read.share.hesvh.cn/Article/details/gtszfsyjo.sHtML

[R67] 生成随机十六进制串
来源：http://wap.fehbvm.com/Article/details/ghjiewdim.sHtML

openssl rand -hex 16
来源：http://m.share.hesvh.cn/Article/details/gzvzvggcz.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fehbvm.com/Article/details/ghmknaont.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.hesvh.cn/Article/details/gzwzmfivx.sHtML

[R69] 生成随机密码
来源：http://mobile.fehbvm.com/Article/details/giycodhbn.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fehbvm.com/Article/details/gjgfxxkcq.sHtML

[R70] 时间戳与互转
来源：http://mobile.zdbjq.cn/Article/details/ghezznxhq.sHtML

date +%s;  date -d @1700000000
来源：http://3g.zdbjq.cn/Article/details/gzpamakdy.sHtML

[R71] 日期格式化
来源：http://blog.hesvh.cn/Article/details/gzpwnekyd.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.hesvh.cn/Article/details/gpfzsniwc.sHtML

[R72] 等待端口就绪
来源：http://read.share.zdbjq.cn/Article/details/gmiriyqfl.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.zdbjq.cn/Article/details/grnwerdqo.sHtML

[R73] 分割大日志
来源：http://www.share.zdbjq.cn/Article/details/gnewszrcz.sHtML

split -l 1000 big.log part_
来源：http://wap.hesvh.cn/Article/details/gzzhqfdka.sHtML

[R74] 批量重命名
来源：http://blog.zdbjq.cn/Article/details/gmieezsgw.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.zdbjq.cn/Article/details/gclzpvhpm.sHtML

[R75] 导出环境变量
来源：http://wap.hesvh.cn/Article/details/gmjcuvrrm.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fehbvm.com/Article/details/gvdqaykuc.sHtML

[R76] 使用临时文件
来源：http://baike.zdbjq.cn/Article/details/gqioqdpue.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.fehbvm.com/Article/details/gpbdxguaz.sHtML

[R77] 读取用户输入
来源：http://3g.zdbjq.cn/Article/details/gwenkzdqi.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.hesvh.cn/Article/details/goxunvrqe.sHtML

[R78] 交互式菜单
来源：http://www.share.zdbjq.cn/Article/details/gvbhtcwzi.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fehbvm.com/Article/details/govmrsowb.sHtML

[R79] 解析命令行选项
来源：http://baike.zdbjq.cn/Article/details/gozrllmgu.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mobile.fehbvm.com/Article/details/gkfaunxbp.sHtML

[R80] 查看脚本执行耗时
来源：http://mobile.hesvh.cn/Article/details/gdnygorrr.sHtML

time ./run.sh
来源：http://3g.fehbvm.com/Article/details/gwfkashsw.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gkfbeqqfd.sHtML

S. C / C++ 专题
来源：http://m.share.hesvh.cn/Article/details/gwhwdjztl.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gyvbvspea.sHtML

[S01] C：Hello World
来源：http://m.share.hesvh.cn/Article/details/gwevyctpa.sHtML

#include <stdio.h>
来源：http://blog.hesvh.cn/Article/details/gbyepyzcs.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fehbvm.com/Article/details/gdwunntwl.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fehbvm.com/Article/details/gudckhahk.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.hesvh.cn/Article/details/gttlnxnrz.sHtML

[S03] C：读入整数
来源：http://mobile.hesvh.cn/Article/details/gjwnxxiap.sHtML

int x; scanf("%d", &x);
来源：http://3g.zdbjq.cn/Article/details/guvyufffs.sHtML

[S04] C：字符串复制
来源：http://wap.hesvh.cn/Article/details/gcwlkktvy.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.hesvh.cn/Article/details/gzdzwksrx.sHtML

[S05] C：字符串长度
来源：http://www.m.share.zdbjq.cn/Article/details/ghgtthlql.sHtML

strlen(s)
来源：http://read.share.zdbjq.cn/Article/details/gepsvqzmw.sHtML

[S06] C：字符串比较
来源：http://www.blog.zdbjq.cn/Article/details/gvspxmleq.sHtML

strcmp(a, b) == 0
来源：http://m.share.hesvh.cn/Article/details/gzowvrlrx.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fehbvm.com/Article/details/gtpwpiehg.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.hesvh.cn/Article/details/gzuylpaap.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.hesvh.cn/Article/details/gchlnhwkh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fehbvm.com/Article/details/gefiyhqwc.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.hesvh.cn/Article/details/gextmqsqf.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fehbvm.com/Article/details/glwdepzao.sHtML

[S10] C：指针与解引用
来源：http://wap.zdbjq.cn/Article/details/gxtglfllu.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fehbvm.com/Article/details/grskchhpx.sHtML

[S11] C：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gafsdsauv.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.hesvh.cn/Article/details/ggqokshry.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.fehbvm.com/Article/details/gxagzckkm.sHtML

fclose(f);
来源：http://www.share.hesvh.cn/Article/details/gbbgvunot.sHtML

[S12] C：写文件
来源：http://baike.zdbjq.cn/Article/details/gxdmwiybw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.hesvh.cn/Article/details/grmvleooc.sHtML

[S13] C：宏定义
来源：http://3g.hesvh.cn/Article/details/gucdzwvse.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.zdbjq.cn/Article/details/gktxxtixz.sHtML

[S14] C：枚举
来源：http://wap.fehbvm.com/Article/details/gnwoyyzcm.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fehbvm.com/Article/details/gpgcvbwqg.sHtML

[S15] C：类型转换
来源：http://3g.hesvh.cn/Article/details/gesrljdqn.sHtML

(double) a / b
来源：http://wap.zdbjq.cn/Article/details/geotpwkjr.sHtML

[S16] C：位操作置位
来源：http://blog.zdbjq.cn/Article/details/guletwoqy.sHtML

x |= (1 << 3);
来源：http://www.blog.fehbvm.com/Article/details/gcozbsjwc.sHtML

[S17] C：安全拼接字符串
来源：http://baike.zdbjq.cn/Article/details/giwexdrwz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.zdbjq.cn/Article/details/gwjevsoeq.sHtML

[S18] C：命令行参数
来源：http://read.share.fehbvm.com/Article/details/gbqhdenvc.sHtML

int main(int argc, char **argv)
来源：http://read.share.hesvh.cn/Article/details/ghgdsfcie.sHtML

[S19] C：快速排序
来源：http://www.m.share.fehbvm.com/Article/details/gvonmdluk.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.zdbjq.cn/Article/details/gmmpudygt.sHtML

[S20] C：二分查找
来源：http://wap.zdbjq.cn/Article/details/grajpzero.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fehbvm.com/Article/details/gejdqjjgy.sHtML

[S21] C：字符类别判断
来源：http://baike.fehbvm.com/Article/details/gqyrplxxy.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.zdbjq.cn/Article/details/gjpexqpen.sHtML

[S22] C：字符串转数字
来源：http://mobile.zdbjq.cn/Article/details/gzmxnawbn.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://m.share.zdbjq.cn/Article/details/gvuevkjor.sHtML

[S23] C：随机数
来源：http://baike.zdbjq.cn/Article/details/gygnicvuh.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.hesvh.cn/Article/details/gaodkybuq.sHtML

[S24] C：获取本地时间
来源：http://read.share.fehbvm.com/Article/details/ghxhadbvh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fehbvm.com/Article/details/gbkjzkbbi.sHtML

[S25] C：内存拷贝
来源：http://m.share.fehbvm.com/Article/details/gaililojl.sHtML

memcpy(dst, src, n);
来源：http://www.blog.hesvh.cn/Article/details/gpyjwgwgq.sHtML

[S26] C：内存清零
来源：http://blog.hesvh.cn/Article/details/guavrvgnj.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.zdbjq.cn/Article/details/gjaevurkz.sHtML

[S27] C：定义常量
来源：http://www.blog.fehbvm.com/Article/details/gylitfchu.sHtML

const double PI = 3.14159;
来源：http://blog.hesvh.cn/Article/details/gtqpkffox.sHtML

[S28] C：静态变量
来源：http://www.share.hesvh.cn/Article/details/gcrlyuper.sHtML

static int counter = 0;
来源：http://m.share.zdbjq.cn/Article/details/guwxzyvfy.sHtML

[S29] C：变参函数
来源：http://mobile.fehbvm.com/Article/details/gxaehpsfk.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.hesvh.cn/Article/details/gorvizwmh.sHtML

[S30] C：头文件保护
来源：http://blog.fehbvm.com/Article/details/gedwrpkhm.sHtML

#ifndef X_H
来源：http://mobile.hesvh.cn/Article/details/glsmzxxkn.sHtML

#define X_H
来源：http://mobile.hesvh.cn/Article/details/gtdkamsix.sHtML

#endif
来源：http://blog.zdbjq.cn/Article/details/gccggowev.sHtML

[S31] C++：Hello World
来源：http://wap.zdbjq.cn/Article/details/gegmojjva.sHtML

#include <iostream>
来源：http://www.share.zdbjq.cn/Article/details/gstbbgnwg.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.hesvh.cn/Article/details/gvosrbaze.sHtML

[S32] C++：字符串
来源：http://baike.zdbjq.cn/Article/details/gitwcqahk.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.hesvh.cn/Article/details/grgexowza.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.fehbvm.com/Article/details/gjiflcfez.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.zdbjq.cn/Article/details/ghpknwikp.sHtML

[S34] C++：遍历 vector
来源：http://baike.hesvh.cn/Article/details/gsbdzfrdf.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fehbvm.com/Article/details/gaxieuwgx.sHtML

[S35] C++：map
来源：http://mobile.fehbvm.com/Article/details/gwztymwbg.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.zdbjq.cn/Article/details/gpqycfwcp.sHtML

[S36] C++：unordered_map
来源：http://m.share.hesvh.cn/Article/details/gouzhyivi.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://3g.zdbjq.cn/Article/details/gyaxykbsf.sHtML

[S37] C++：set
来源：http://mobile.fehbvm.com/Article/details/grwhmwibm.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.zdbjq.cn/Article/details/gdybifztp.sHtML

[S38] C++：排序
来源：http://m.share.hesvh.cn/Article/details/gbdjzzvvo.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.zdbjq.cn/Article/details/gwidipjlq.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.zdbjq.cn/Article/details/gtjnwlxyh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.hesvh.cn/Article/details/gvqvothfp.sHtML

[S40] C++：查找元素
来源：http://wap.fehbvm.com/Article/details/grarkousr.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.fehbvm.com/Article/details/gnvsmiafh.sHtML

[S41] C++：类与构造函数
来源：http://www.m.share.hesvh.cn/Article/details/goerxwkdm.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fehbvm.com/Article/details/gxqbbdorb.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.zdbjq.cn/Article/details/gvsdxlirb.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.hesvh.cn/Article/details/gtyrqrccx.sHtML

[S43] C++：智能指针
来源：http://mobile.zdbjq.cn/Article/details/gdvwqizha.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fehbvm.com/Article/details/gtwsxkxpr.sHtML

[S44] C++：引用传参
来源：http://www.share.fehbvm.com/Article/details/gydcdjwnp.sHtML

void inc(int &x) { ++x; }
来源：http://baike.hesvh.cn/Article/details/gcvvksdee.sHtML

[S45] C++：lambda
来源：http://mobile.hesvh.cn/Article/details/gnrgonjyx.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.hesvh.cn/Article/details/gzactdegs.sHtML

[S46] C++：函数模板
来源：http://mobile.hesvh.cn/Article/details/gosgaomfn.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.zdbjq.cn/Article/details/gcmjaxifm.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.zdbjq.cn/Article/details/goehadzoc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.hesvh.cn/Article/details/gbnmoncpw.sHtML

[S48] C++：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gknqgoppr.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://3g.hesvh.cn/Article/details/gsmxkfryv.sHtML

while (std::getline(in, line)) { }
来源：http://baike.hesvh.cn/Article/details/gnspfwiil.sHtML

[S49] C++：写文件
来源：http://mobile.fehbvm.com/Article/details/gmywssoul.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.hesvh.cn/Article/details/glqbxrvhs.sHtML

[S50] C++：格式化数字
来源：http://mobile.zdbjq.cn/Article/details/gijfzvfvx.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wap.fehbvm.com/Article/details/gxxwcxwbe.sHtML

[S51] C++：显式类型转换
来源：http://www.share.hesvh.cn/Article/details/gwnlcpyzm.sHtML

static_cast<double>(a) / b
来源：http://m.share.hesvh.cn/Article/details/ggyocsygd.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.hesvh.cn/Article/details/gfhquxkqo.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.hesvh.cn/Article/details/gmxeqejcs.sHtML

[S53] C++：移动语义
来源：http://mobile.hesvh.cn/Article/details/gxsecrvlz.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.hesvh.cn/Article/details/gsbcnudrw.sHtML

[S54] C++：异常处理
来源：http://3g.zdbjq.cn/Article/details/gzvhxbwjk.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.hesvh.cn/Article/details/gjzfmuxts.sHtML

[S55] C++：结构化绑定
来源：http://blog.zdbjq.cn/Article/details/gnwrtjqvz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.hesvh.cn/Article/details/gbnpuqmiw.sHtML

[S56] C++：optional
来源：http://www.blog.fehbvm.com/Article/details/gxhxksaob.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.hesvh.cn/Article/details/guuerjmex.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fehbvm.com/Article/details/gggyixtsw.sHtML

constexpr int N = 10;
来源：http://read.share.zdbjq.cn/Article/details/gewnqfrdm.sHtML

[S58] C++：命名空间
来源：http://mobile.hesvh.cn/Article/details/goyvrigiz.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.zdbjq.cn/Article/details/gjfypjeha.sHtML

[S59] C++：静态断言
来源：http://3g.fehbvm.com/Article/details/gxthbndie.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.hesvh.cn/Article/details/ggmtmoayr.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.zdbjq.cn/Article/details/gxfmzwzui.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fehbvm.com/Article/details/ggwaxrunk.sHtML

================================================================================
来源：http://www.blog.fehbvm.com/Article/details/greoxtvlw.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fehbvm.com/Article/details/gnseatmrx.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gcpwogsqn.sHtML

[T01] Kotlin：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gbhgmfprh.sHtML

println("Hello")
来源：http://3g.zdbjq.cn/Article/details/gfjcfvpcv.sHtML

[T02] Kotlin：变量
来源：http://3g.zdbjq.cn/Article/details/gvmwlcghq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.zdbjq.cn/Article/details/gycszwvjv.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fehbvm.com/Article/details/gfielwmeu.sHtML

"值: $b"
来源：http://www.m.share.fehbvm.com/Article/details/ggxlzmcgi.sHtML

[T04] Kotlin：空安全
来源：http://read.share.zdbjq.cn/Article/details/gnjpxlicr.sHtML

val n: String? = null;  n?.length
来源：http://mobile.hesvh.cn/Article/details/gkljhddfr.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fehbvm.com/Article/details/gohovnxcz.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.hesvh.cn/Article/details/gufkurruo.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.hesvh.cn/Article/details/gvyfaokce.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fehbvm.com/Article/details/gdkxlqgxm.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.zdbjq.cn/Article/details/gixrodciv.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.zdbjq.cn/Article/details/gpocqrown.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fehbvm.com/Article/details/gxywshvlf.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.fehbvm.com/Article/details/guvovqqbc.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fehbvm.com/Article/details/grlewdstz.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.zdbjq.cn/Article/details/gzscwymem.sHtML

[T10] Kotlin：默认参数
来源：http://baike.hesvh.cn/Article/details/gmfyrlswh.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fehbvm.com/Article/details/gahocczjf.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.hesvh.cn/Article/details/gzexxmbft.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.hesvh.cn/Article/details/gsypahoop.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fehbvm.com/Article/details/gfaeeswgb.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.zdbjq.cn/Article/details/gfrymglzb.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.fehbvm.com/Article/details/glacmwfcz.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.zdbjq.cn/Article/details/glivdudqo.sHtML

[T14] Kotlin：循环
来源：http://read.share.hesvh.cn/Article/details/gdewdhhcj.sHtML

for (i in 1..10) println(i)
来源：http://3g.fehbvm.com/Article/details/gtxmbjiio.sHtML

[T15] Kotlin：接口
来源：http://m.share.zdbjq.cn/Article/details/gkoopxfoy.sHtML

interface Shape { fun area(): Double }
来源：http://wap.fehbvm.com/Article/details/gstizqztv.sHtML

[T16] Swift：Hello World
来源：http://mobile.fehbvm.com/Article/details/gcxabkvnl.sHtML

print("Hello")
来源：http://wap.fehbvm.com/Article/details/gcdpyuifj.sHtML

[T17] Swift：变量与常量
来源：http://3g.fehbvm.com/Article/details/gkfbwueju.sHtML

var a = 1;  let b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gwgqwdplt.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fehbvm.com/Article/details/gfsspqykn.sHtML

"值: \(b)"
来源：http://m.share.hesvh.cn/Article/details/gybfefgis.sHtML

[T19] Swift：可选绑定
来源：http://wap.fehbvm.com/Article/details/gwjjlwcbk.sHtML

if let n = opt { print(n) }
来源：http://read.share.zdbjq.cn/Article/details/gdqrtxxht.sHtML

[T20] Swift：数组操作
来源：http://www.share.zdbjq.cn/Article/details/gfdovtnfo.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.zdbjq.cn/Article/details/gnwcbyykn.sHtML

[T21] Swift：遍历
来源：http://www.m.share.fehbvm.com/Article/details/glvdrblcq.sHtML

for x in a { print(x) }
来源：http://baike.hesvh.cn/Article/details/gdlpwqlws.sHtML

[T22] Swift：字典
来源：http://blog.zdbjq.cn/Article/details/ghvpbzfia.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.hesvh.cn/Article/details/gijnttiov.sHtML

[T23] Swift：函数
来源：http://www.m.share.zdbjq.cn/Article/details/glogpsjay.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fehbvm.com/Article/details/gjdhaporf.sHtML

[T24] Swift：闭包
来源：http://www.blog.hesvh.cn/Article/details/glbgzmejn.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.hesvh.cn/Article/details/gymjxaykx.sHtML

[T25] Swift：结构体
来源：http://read.share.fehbvm.com/Article/details/gdcdiplbm.sHtML

struct P { var x: Int }
来源：http://www.blog.zdbjq.cn/Article/details/gzvznsdfv.sHtML

[T26] Swift：类与重写
来源：http://www.share.fehbvm.com/Article/details/gqoieqhap.sHtML

class A: Base { override func f() {} }
来源：http://baike.fehbvm.com/Article/details/gndzcydcf.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.hesvh.cn/Article/details/gnozprbtu.sHtML

do { try f() } catch { print(error) }
来源：http://wap.fehbvm.com/Article/details/gfrkdcpai.sHtML

[T28] Swift：枚举
来源：http://mobile.zdbjq.cn/Article/details/gwidaieim.sHtML

enum Color { case red, green }
来源：http://wap.hesvh.cn/Article/details/gkkzbvtuz.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.hesvh.cn/Article/details/gdhptmcqg.sHtML

guard let x = opt else { return }
来源：http://baike.fehbvm.com/Article/details/gdjacasfn.sHtML

[T30] Swift：协议
来源：http://mobile.fehbvm.com/Article/details/gnwbphakn.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.zdbjq.cn/Article/details/gvgckwxjz.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gcqeuzzbq.sHtML

print("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gmorfsccw.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.hesvh.cn/Article/details/giczampxj.sHtML

local a = 1
来源：http://read.share.hesvh.cn/Article/details/gslnmtyus.sHtML

[T33] Lua：表（数组）
来源：http://3g.fehbvm.com/Article/details/gjmnlcfur.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.fehbvm.com/Article/details/goaunvidk.sHtML

[T34] Lua：遍历表
来源：http://m.share.hesvh.cn/Article/details/gldgeafgy.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://read.share.zdbjq.cn/Article/details/ghccfrwgg.sHtML

[T35] Lua：字典表
来源：http://wap.fehbvm.com/Article/details/gskroelfr.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fehbvm.com/Article/details/gkvydekqs.sHtML

[T36] Lua：函数
来源：http://m.share.zdbjq.cn/Article/details/gfarirukc.sHtML

function add(a, b) return a + b end
来源：http://www.blog.hesvh.cn/Article/details/gmzffrcuq.sHtML

[T37] Lua：字符串拼接
来源：http://blog.hesvh.cn/Article/details/gnblzqbel.sHtML

"a" .. "b"
来源：http://3g.fehbvm.com/Article/details/gteoilogi.sHtML

[T38] Lua：条件
来源：http://baike.zdbjq.cn/Article/details/gaqwpmjiv.sHtML

if x > 0 then print("正") end
来源：http://www.blog.zdbjq.cn/Article/details/gdshdvusx.sHtML

[T39] Lua：模式匹配
来源：http://read.share.fehbvm.com/Article/details/gzzrgxqht.sHtML

string.find(s, "%d+")
来源：http://www.m.share.fehbvm.com/Article/details/goizdeywa.sHtML

[T40] Lua：元表
来源：http://3g.zdbjq.cn/Article/details/ggofxmbpf.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.fehbvm.com/Article/details/gryxpqrrq.sHtML

[T41] Perl：Hello World
来源：http://m.share.hesvh.cn/Article/details/gxmvkmxce.sHtML

print "Hello\n";
来源：http://www.blog.zdbjq.cn/Article/details/gdxxasfbn.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.fehbvm.com/Article/details/gdwzjeoyh.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.hesvh.cn/Article/details/gfzfapiyb.sHtML

[T43] Perl：字符串插值
来源：http://baike.fehbvm.com/Article/details/gzpnwlzlc.sHtML

"值: $a"
来源：http://www.m.share.zdbjq.cn/Article/details/gvukbqllu.sHtML

[T44] Perl：条件
来源：http://baike.hesvh.cn/Article/details/gjojzhzwg.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.hesvh.cn/Article/details/gmzaixnux.sHtML

[T45] Perl：数组遍历
来源：http://mobile.zdbjq.cn/Article/details/gqixjfowa.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.hesvh.cn/Article/details/gtyobjjlp.sHtML

[T46] Perl：哈希操作
来源：http://www.blog.hesvh.cn/Article/details/gowrqgvcc.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.zdbjq.cn/Article/details/gzfrrplwq.sHtML

[T47] Perl：正则捕获
来源：http://mobile.fehbvm.com/Article/details/gafrbyqwn.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.zdbjq.cn/Article/details/gdazdupmn.sHtML

[T48] Perl：正则替换
来源：http://www.blog.hesvh.cn/Article/details/gpjhigebm.sHtML

$s =~ s/old/new/g;
来源：http://m.share.hesvh.cn/Article/details/gobnmoykl.sHtML

[T49] Perl：函数
来源：http://www.share.hesvh.cn/Article/details/gjulseehs.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/gaqhlspbt.sHtML

[T50] Perl：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gudhfhfbs.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.zdbjq.cn/Article/details/gpjhymerc.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.fehbvm.com/Article/details/gvpjpobpp.sHtML

[T51] Scala：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gchswkojp.sHtML

println("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gynwhflgg.sHtML

[T52] Scala：变量
来源：http://blog.fehbvm.com/Article/details/gvyiaxfaq.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gowshjszp.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gzitignpt.sHtML

s"值: $b"
来源：http://www.m.share.hesvh.cn/Article/details/gqvaxppaa.sHtML

[T54] Scala：集合映射
来源：http://3g.fehbvm.com/Article/details/gyyjpppwb.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.hesvh.cn/Article/details/gstusnsvq.sHtML

[T55] Scala：集合过滤
来源：http://mobile.fehbvm.com/Article/details/gobfgxfnr.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.fehbvm.com/Article/details/gyvqxaxcz.sHtML

[T56] Scala：样例类
来源：http://www.share.zdbjq.cn/Article/details/gzeitqhah.sHtML

case class User(name: String, age: Int)
来源：http://m.share.hesvh.cn/Article/details/gvpqgnccg.sHtML

[T57] Scala：模式匹配
来源：http://mobile.zdbjq.cn/Article/details/guxjaccuf.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.hesvh.cn/Article/details/gyqvmmutv.sHtML

[T58] Scala：函数定义
来源：http://read.share.zdbjq.cn/Article/details/gfemttyub.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://read.share.fehbvm.com/Article/details/gbqqlnufg.sHtML

[T59] Scala：循环
来源：http://www.m.share.fehbvm.com/Article/details/gvtliarur.sHtML

for (i <- 1 to 10) println(i)
来源：http://baike.fehbvm.com/Article/details/gyrlkoijx.sHtML

[T60] Scala：折叠
来源：http://m.share.zdbjq.cn/Article/details/gndmgfibp.sHtML


<!-- 参考信息 -->