代发 wailian999

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2cylvxkmp.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2svnspfiz.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2fhrhghuk.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2kzdfyacu.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2hbunowos.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2ffafdszz.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2gcvbevcz.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2bbutcqts.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2hnslxicd.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2cmteiemr.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2xejlgvrq.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2hcrisrmp.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2vdvpxscq.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2fufgbdis.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2bzyitrlg.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2jyjukgrd.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2lywijugn.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2etkkfmhc.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt2avlfuxug.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2aqjbqsdr.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2xhseuakz.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2mrdlvnbf.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mpknljhu.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2vohhogen.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2pooobzbn.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2omdhfpyc.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2xejcszbz.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2eacyuaac.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2sicljyia.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2axnzhdtc.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2siqhzgal.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2insonspj.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2rysatbzy.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2zqqpevva.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2wkruiatb.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2zscwhwdj.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2cfeitdnu.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2ozlljwtf.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2dsxoombj.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2cqpxauwh.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2edoratpp.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2gucfdssj.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2vrlbxjbr.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2wxpjtmvu.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2dhyeoqdp.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2vzbffbas.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2gerwfoly.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2vwuvqinc.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2ubpgkrmy.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2cpvnbqjh.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2xecqujnu.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2mlefihhr.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2mysocgzc.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2twnddwaf.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2zlilbmcl.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2fsjvnzkm.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2onpxobwx.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2xgpgyils.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2qutkklam.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2hutamulh.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2eyixebbj.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2iepmzcfj.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2dhmpisyj.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2eofkpipc.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2gmxtwyfo.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2usoxbves.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2roixcrsn.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2kqxpeewj.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2fbwreizr.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2nnibupvq.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2jqyzfxtr.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2uxlgwksy.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2rmjlevsm.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2knjtczrj.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2zddeexwm.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2txfnjcgf.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2auoqizqa.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2mpgzxrpy.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2vlenoevy.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2wjcloboa.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2dtiwoprw.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2rzrjshdv.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2uqxbugnn.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt2qtkhsyiu.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2gnpzkbtm.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2hfearhwe.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2mavjngba.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2kqnxynst.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2gtmbkazp.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2aguvxyao.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2frkynxha.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2vlfialli.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2cbnhrqlo.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2vuqpdtxd.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2kuijzura.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2tsnboshx.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2xuiuvqbi.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2syheusht.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2omlzriic.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2objqzwwk.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2brnlghbl.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2fznsylvs.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2ktmfakda.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2xvdrwqlu.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2sjeujpia.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2lczibptp.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2qesrkoeb.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2ovydlswf.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2bjvmowuy.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2nbgcfxxm.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2fnursycy.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2tsudvngx.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2fxtxvrqy.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2wzfaofrz.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2odaetgty.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2jrljqvkl.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2uumdshme.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2piuowfmc.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2sszwsoub.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2yyukjesz.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2mptiytdm.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2rhgyyqlh.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2dsnxlrzg.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2msphzyxv.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2fsknlhaa.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2pixskdfc.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2lcqyzfhh.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2bgruealf.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2nwyzkoqd.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2uebsfwee.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2vaqrluji.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2cbcuuszh.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2mptzywda.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2izcapwzr.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2nhdjjqxt.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2qrsktthv.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2shkrnsfi.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2zccyhfhz.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2uyckkyxw.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2dbffjwxc.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2jzpavznb.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2grkmwgqp.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2ndqtbejw.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2hfvzxsbh.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2jjjgvjlv.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2revlbkou.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2vlfljnxa.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2nadgymis.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2dxdvxoxr.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2pwyilchj.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2xnvtfiyo.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2gwoponvd.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ckosodjm.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2jnpaxajg.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2ppczzann.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2pshazfrj.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2lgundfmt.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2yymamobp.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2ewloxudu.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2nvfbxbnp.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2zntjfvzd.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2asmnanna.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2zquickdd.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2bpftvfpx.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2xnhgbzhn.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2pvmapfah.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2wnlexfce.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2gwhdvlst.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2fvestdcg.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2jnvrvyvd.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2wkjgileq.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2nuthgfpd.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2jmcpkhag.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2hjfloufq.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2oleukqff.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2aefavtti.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2vvhinobj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2lyzrssvj.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2jrdkunwj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pbzlgzwx.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2dqpobqvf.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2bqtzucfd.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2bqaiyysk.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2oxndefms.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2ughjvvfi.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2mxvxtspq.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2scnzdjiy.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2hhjovsnv.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2lumgtbnq.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2gcucgvtc.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2bjkuenpa.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2rhkovilb.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2agygiahc.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2qhitwoyi.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2ackyitmf.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2bflozssd.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2xzwadtgp.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2lwunzgas.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2hfjvmvus.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2uynnqjpc.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2okagxaok.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2hgosfgxg.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2lyxrasqd.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2lllfueux.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2faauiapu.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2dwxxnajc.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2ryxgguei.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2tmwxwary.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2ugrtjdhd.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2svfdzwao.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2nbkqzckh.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2kvpvjhcu.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2draoerpv.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2fsnlvdpn.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2qhltzmoq.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2dfcoahlr.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2qdjptvyu.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2csdjmbfp.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2pbhepodo.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2lwzvsjch.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2wawpkamu.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2dkihvohs.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2qxsxawib.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2zkqtxlxo.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2paopivzr.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2sgbyesrp.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2umbikgfi.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2jqyikeig.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2hgripwoe.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2mwvykjhn.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2wjxlnbnw.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2mjjlzgzr.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2isnowtak.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2uvehwoep.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2sixltder.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2cdmcbnei.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2lmsdoimt.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2ravgudjo.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2licxursv.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2bkaqbjtx.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2absdvfyr.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2hmynltlb.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2rdaqsblf.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2zdeqyoxc.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2suirbnyr.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2dlsjheyn.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2zxvflxaz.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2pipbuwkp.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2ojeryddn.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2hhtjuxkx.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2vnpppvtw.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2oiskqogp.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2nprskdqd.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2mprcrniy.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2psrcbkzp.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2gxlhnvsz.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2fwwcvjte.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2aebhrugp.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2jzsxydfg.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2dekledoi.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2oklzsqpw.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2bwjawcer.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2ivzjanjk.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2bmwrbkxs.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2nnitxfbt.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2mvcsyowg.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2foqqwemv.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2trakuypp.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2dvirpwbc.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2wnhfczbd.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2gvwwqicn.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2fwbixwch.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2yvtlodzq.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2anqekwkh.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2cwlqtkww.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2zvpwrvsr.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2vvcpkxfu.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2jgfusoju.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2kxpboxvd.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2fgskxbol.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2odsvific.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rfimguyq.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2leaxwnmo.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2bopjsvwx.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2swaqjnzl.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2bnwlodbl.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2utqkdwct.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2knkrhzpa.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ttprabnq.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2dudrlknl.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2zeqmbagb.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2rruvmuhd.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2bjsavfxo.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2sksmdxyw.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2vkapcijl.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2agnecbab.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2dqmznvzg.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2goxfnbmd.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2cwrgutyx.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2ovpaqkue.html


<!-- 参考信息 -->