代发 wailian999

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2trthkzde.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2snyoaxsg.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2wnquzvam.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt2lbafpwkn.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2fgfgkspn.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2bkiyfmlb.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2auwurzhq.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2kqcmsswl.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2wvwbgcxe.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2immnqqyk.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2heridnyr.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2noypqcfz.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2unteqedl.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2dsreoqpu.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2dxelgheb.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2bonnskwd.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2gpscbtsd.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2vwxakchz.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2lqrefhhu.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2hgweckja.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2dcsvcgvj.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2rleuztpl.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt2pgimfrbf.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2arjovnco.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2wbsmrnyb.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2acwljjcv.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2cxwxnrkg.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2gpdqljob.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2sfiqgqfh.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2ufmbgkdi.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2fwmhqkev.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2urrlfily.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2elremlmg.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2uqlqdlao.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2isglhxdf.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2vinazycq.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2tldsweyi.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2odwxnfpb.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2jspfswno.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2hgxqsjkb.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2ucmruqvg.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2gqsbryzp.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2ffmsmmll.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2uzcrziws.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2vnzlvaem.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2anuyybde.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2jgztrywc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2djqwjdvb.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2rmskhsmv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ejcmqbme.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2nayobmyb.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt2zrkxmbhs.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2weunwgxq.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2llnmpspa.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2yfifnkvm.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2ksajmsjm.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2mtaxyqhd.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2mxjljsol.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2ccgfolmi.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2zcueibbr.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2scwgaihq.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt2selcljdh.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2wdwxovtd.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2mfkiqkfn.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2cwyqtnji.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2oxacerjv.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2uyxrpkcs.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2hedqrkpv.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2gudhckbt.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2rxffrrmk.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2ryqoilfd.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ofcvjukt.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2zajtkynk.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2bnsfhxeu.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2owsmbbil.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2weayszjk.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2etipupqj.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2xrffqevg.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2tzixvrvt.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2arntjgsw.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2yrzhokru.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2jrdrlhca.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2zhcymxrx.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2jyarxdxs.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zumifpkx.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wsimzqxx.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2jnwqzuwl.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2slcfihej.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2jakkktop.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2mjpuvzst.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2nioriudu.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2shbdcben.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2pnpqzuwm.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2inagsqkk.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2dwscdqun.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2dvwsdbhu.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2onxlnkmh.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2cctxyuzu.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2ibqllpqo.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2vodqhewh.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2dkjhomti.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2jogjbnmf.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2bjcguopm.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2vyievlna.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2qdaojnqs.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2prygaklr.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2lzjwlvkt.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2eaammlqu.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2uzioixoc.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2jvnkxpsf.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2ltznpyxv.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2jikrovuc.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2iqioztya.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2bggqfiny.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2fhsvachv.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2lygmexcb.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2yrnbsdif.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2xrgpamsw.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2wlzphxjr.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2lztdffjn.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2fikrhwpn.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2uxssvkgl.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2haekqiqi.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2swwtltnd.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2pmrkdjyi.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2yaljcxxc.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2ywvompxs.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2yacfgczh.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2apawccbk.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt2qnctpqhy.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2qrdsbeiy.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2wvrawmcf.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2elexwqtp.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2gehndehy.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2xrtrcenx.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2gxvounqb.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2sawpkbmq.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2lxiddoeq.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2ecwsnjwm.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2qmmxgnna.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2jkgltqbq.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2alihvqjf.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2egvixhfi.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2tttooyqg.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2eaqoouaw.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2mqfvnqdy.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2pacpvoxq.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2zbcsoxon.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2zikquxdq.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2htttdrix.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2fyvkeveu.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2pxryhmod.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ttslmgyq.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2ecmkhjkj.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2dfkvqtfy.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2pleojdje.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2gpdgihhj.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2bpgvpvbk.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2jtdipgdu.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2yjkytpfn.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2qaxvtabf.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2nmlzysvv.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2gyfowmtz.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2ybnkcvbs.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2hgeokzag.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2jyklymoa.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2ewjyucmb.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2zxmkngbj.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2behovhsm.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2flruigpd.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2lgitcbad.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2hyythvck.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2qvlpxmxx.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt2pecovcpp.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2txdhpdbp.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2plkxxazi.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2fyzwjoak.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2erelxjlk.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2htjyeewi.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2wqgacevi.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2aaxmerzw.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2nyareluf.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2uuyqobwr.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2adevezdn.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2juxellxu.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2aycmztot.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2gdeiyysi.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2snybeuuy.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2pmsmompl.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2jqgktoxa.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2rwwxfzwh.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ddefrhej.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2mmdlxwco.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt2niahrswi.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2zxagjllw.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2zzminbhf.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2aqgjevrj.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2dkdddzsq.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2llgdbsmj.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2vqpflwxe.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2qngnbszu.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2tdhoxyvd.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2smtnsqrp.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2obyzuenn.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2lzvwpmbk.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2ykjcolei.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2oydubukx.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2kwvielqs.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2wzvoqign.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2guehwtvt.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ygehqlte.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ukgampgl.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2ycjhckku.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ifhmqvwb.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2jbqiambd.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2rnpmcred.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2mqzemzah.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2hfctwsuh.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2sbvelcon.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2xtxbvyxz.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2rcforjfp.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2bhtneuue.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2ofiqlnnu.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ffcknppa.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2gnifdvmq.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2cchojbpl.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2hsjaobtx.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2znywxqqg.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2dklenqhs.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2zmakltpk.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2ejjkwwan.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2yxxzphim.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2tnzssyem.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2kqxkfqym.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2yclprwpd.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2aniycxop.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2tgxwoids.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2crjwmdcb.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2yolbryls.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2ygkdrtsg.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2rqbflugj.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2yktlglbl.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2uatvqmtt.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2oepopodo.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2ubdzcyrg.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2oqlikmis.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2dejlhnst.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2upvgewrp.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2zjnxgzwg.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2dqquybds.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2gbqzirby.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2qbksoanb.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2tidizsie.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2vzjddhpe.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2ucgwjujn.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2ieaemrkd.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2snndovqv.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2kmwcxxod.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2yeithdcd.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2trcisryj.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2zcsscael.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2oyvgrrno.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2ylfotusy.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2vquojfbb.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ovalqwca.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2yoywyimi.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2wipezzje.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2blopsamr.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xpwifubj.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt2wkatlrnb.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2pzkzmncn.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2hrojpjrr.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2dveczzzh.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2fmhvlwpp.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2lpfhzvzv.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2dstywope.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2lwknlqil.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2onikwucz.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2xrktntta.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2rlkkrywg.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2eogojnqr.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2fbqubhym.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2kugptjzj.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2hgggciir.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2eduxblic.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2skdwzfil.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2ncmyfnsd.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2lgurgwiu.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2uvhpaudy.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2xotsgfih.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2azyuloax.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2milsdilm.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2ufmlykot.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2xmrjjexj.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2zmrrheyx.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2tchfjdyv.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2hdrzqgbs.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt2obyakhnk.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2fgeawjyv.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2aredqztl.html


<!-- 参考信息 -->