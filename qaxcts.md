代发 wailian999

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2kyvzzfus.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2qhtgowbl.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2hpirlmsv.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2dmbyadrp.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2koadigqz.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2gyrsupet.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2agwxkqcr.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2fjhlktro.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2wzpuxleg.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2ebrqygwz.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2pcbhcgzo.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2htmgnigs.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2yhqamtme.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2jloaamyt.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2abjjckpk.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2lffzrtwy.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2ngeyscro.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2owojoqyz.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2vtbfippg.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2eerenlok.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2yezhcbmb.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2fqrdfbzs.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2xjpofjkv.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2mfmrgkdo.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2evnmvezy.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2scsaovxo.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2ffyruesi.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2hxehwgpq.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2tobhpewu.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2qnhgwcmg.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2zgfhwqnd.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2jinchytq.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2ksxrqpjb.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2ceoqoaec.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2ltcgpmxv.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2sbhqlizg.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2vmedknqg.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2fbcryydc.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2ogvbbglb.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2xxtydmjy.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2hifysket.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2faqxcpuw.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2ycgriadk.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2qhdrmgdd.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2ludmksry.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2cqixlmpc.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2xccobkqo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2mfyeeuga.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2dhjmiegx.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2qzcnrsyk.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2kxeleaic.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2ylkjfroq.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2viyagbsd.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2bnuminze.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2jdcqtndz.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2jyvxfdir.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2esclgkdk.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2jptxhoxo.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2flsusvrg.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2aufugnom.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2faikxfqi.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2rmhumrwu.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2vvdvzhbz.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2pnhjrelf.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2qltruqjb.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2vjplasiu.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2giiztpdp.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2vnprlkfn.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2gydkaemf.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2zxogwyuc.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2hastxzdm.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2hqtpnuzy.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2udhzouxt.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2imtsxtmp.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2mjrjjmiv.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2ylakngdc.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2cyqzefsn.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2ebazriax.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2rrxszycg.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2eimkpspg.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2xuerutfy.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2ifcmufdd.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2hvzmxfta.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2fkkyjvly.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2heuupeox.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2flikmdzv.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2ybdmhkep.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2djestlbu.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2lwtjwvci.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2ftwqmcll.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2jgqcfeju.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2wwrxeoed.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2nvlcwkvn.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2ersuvxmn.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2kilchfsa.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2hgjjuzxf.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2dawctipi.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2jyryokzb.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2nvvjzpsg.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2ehdipdcv.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2nnrssjmw.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2qlenwukl.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2jqccjpyb.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2ilvnmmiq.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt2pzuucblm.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2ruoyfoui.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2rtduqywz.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2zolklsak.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2ajpnzvra.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2gueiokdg.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2gyylqmhc.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2yxftnkeb.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2hzczhkrh.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2zvlwcrbp.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2prjewkki.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2motssymc.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2zzvuawjj.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2pbjsyqko.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2xhaknhxb.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2rlqwzzym.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2lkuotmtr.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2pamnbxsh.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2pagtebkg.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2sznzwnla.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2uzibrlvu.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ajizqlcf.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2pppyaspl.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2bqopdscl.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2njpgaprv.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2znsoxskm.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2ozrskcow.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2cwmtdyxr.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2lwckghni.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2edxqkmtq.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2laiwfmmq.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2zivitpoa.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2fnsrcztq.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2pufbdwht.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2uxqkxluo.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2vswkpccv.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2ldltdeox.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2ingcotts.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2ayiovtlk.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2chgtqdzj.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2mnekbmsp.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2kvpylpqh.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2axhgvlgc.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2brnejywo.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2esxcabjj.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2hxktrnoc.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2wftsmpru.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2wkwhlzhj.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2avlmpjru.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2izvxnnlp.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2okofdqkx.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2gqjmobio.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2cxfkkpuh.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2geeqvwqo.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2ovikkmga.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2ipwstnnh.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2tmqmmauy.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2rvbhpusx.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2utnuqorf.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2jiodfopj.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2zrwxbrzm.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2eyvixlrh.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2oebbbrlx.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2tuljoosx.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2hiagmnvc.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2ccrhrxck.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2jbisbpjr.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2ygdbdpdc.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2jyftsxlg.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2suuiuqrj.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2cuaydqha.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2jbwyrkkh.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2tjbrctro.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2oqvylude.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2neuzahmt.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wwskpskp.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jfuxysvr.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2bxyxlwem.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2vnrdwkkm.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2lzwtqhwf.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt2iyazdhta.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2kehvkgay.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2pmckujdu.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2rjfmhrih.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2ydnyuike.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2hfranyaz.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2bskufjuv.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2karwsrqm.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2ibooinyq.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2ovndmfrc.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2ojzmxedo.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2qkzdtnbf.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2hbqrzqqj.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2cixkyfup.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2ftbbcqoz.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2gdjammbj.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2qhuvwjxx.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2hyvmpbxx.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2rzbijycn.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2lxoblxqv.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2rtclyvsv.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2tlsrpyfb.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2ythqsgrd.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2chmdukhw.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2syyvzvjf.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2lvstsuwq.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ukbvwtey.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2oiacmwvb.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2dvsqiiiq.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2chxvdbbt.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2sumfzevc.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2atncuxth.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2jkyuvyfj.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2kiqswmld.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2blrvmwug.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2dwxnesrr.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2poaiwhzl.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2vcbntunb.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2jcrfjjhu.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2japqxfsh.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2qddqhnvl.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2cwrxbsyn.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2kkpkxqwr.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2ghpcgzxy.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2jinavyzv.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2elyngzmy.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2pqethwcp.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2cetdgdeq.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2cnkhdrbx.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2uppaxtlc.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2yyfmruvn.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2qgewquev.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2blbxpcpb.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2oaxnkqra.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2ezgkjcnm.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2dvlxryft.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jfkghwbd.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2spemblrf.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2wdcthuto.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2xpukaxsd.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2kgpgvxyf.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2pwttamra.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2pnniyytc.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2iwxjiolu.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2idvvgsrw.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2isakyquj.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2cflmvcsm.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2bceqxudb.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2pwygkqid.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2mtqodhur.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2rfqvmqti.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2rljlfsxn.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2phkszetv.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2nycouagh.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2fyqrgboa.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2mjlksleb.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2sboyihqm.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2hhtablnb.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2zofpbksg.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2sknyemtf.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2cuuldgze.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2piykchfz.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2wekgesbb.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt2lbbmprtm.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2hhdojyts.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2yesfuick.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2dykqjwtu.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2suqpgqzt.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2qlwooriw.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2binqbtwv.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2adeliiig.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2guirevay.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2vxgyxsmn.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ozksxsjs.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2hcnuxtty.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2rkdsaesa.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2jpndlefg.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2gcfevisb.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2wvbfjcuz.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2isssoptw.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2xgvutcmn.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2rrqivpaa.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2ocpqpqfj.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2sjsihwie.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2veseggmu.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2yuhngwdz.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2ltthimpk.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2jnodkuuu.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2pvuplrzv.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ipopyohg.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2jnouyjcj.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2wakiwthc.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2csgtcizp.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2xguzieoo.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2abmokzct.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2neeguezr.html


<!-- 参考信息 -->