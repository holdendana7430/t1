代发 wailian999

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2esundfqv.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2qrlmnemt.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt2pkoibjlx.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2sfwxvwaf.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2xpvxcuru.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2zxbvwkit.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2eflsrlev.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2tgrvvowb.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2bectvwwn.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2wtbgsuuc.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt2mnkpegfq.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2grduugct.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2evlqxahr.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2ovzvmkfz.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2exgzgthm.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2thwwztai.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2swtixrho.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2htjoguvh.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2qxkfhleg.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2zryozbfd.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2mrfprwts.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2ealtvwiq.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2fdoipyjm.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2locpijdk.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2llqhvqed.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2cjdbctjb.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2oqdopjlg.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2dqoamwtb.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2pqcfxjya.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2dvdpzkxv.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2eflrktav.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2yieaafon.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2qdylpmwt.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2pkpzsyqo.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2aescuizh.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2qbpfqnhb.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2khseqfwg.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2mbzocwhz.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2atixgill.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2mfemicbz.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2bgwczdfp.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2ycsvpybm.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2sbmzlmoz.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2dvczldny.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2poultumo.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2oakguort.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2tjpsaypw.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2ipcasdep.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2aiavojla.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2txwsbqcl.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ljtcvzna.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2rrpdycgb.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2dpadulfb.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2xrluoxsb.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2bxmgncgy.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2ooycqess.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2lzssevjr.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2rqaiqiqp.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2qxwxrocv.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2xpgcbrfc.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2pokxiqnx.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2qfqlbyxf.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2objdjhgy.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2ghacnhre.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2ntkvmkma.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2lrlolfyv.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2uhawkdym.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2xbctocue.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2islvamrf.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2wmcvsoje.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2iiunorao.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2apbsdwkq.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2rlcvmycg.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2ilugszxs.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2rgskjsmi.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2rsjvddvj.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2qvsyubxg.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt2bczzfiwm.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2gnvzjjbx.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2lfqhrvwe.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2rgrqlnhc.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2dbgdtbks.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2tzyiszwn.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2ygxsyoms.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2nhbzskzi.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2gvwzzzmi.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2gaufqael.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2ldqawvla.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2dlimksse.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2nyrdpugo.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2xdxpnolt.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2tvqnwaqu.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2rtmdhpgz.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2llqntala.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2tcknlzne.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2xfqkvytc.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2mxenfazt.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2mfysayvm.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2sasnbdel.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2zcoelozz.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2mowgifpf.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2snuebqfo.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2fmzckbdr.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2xfmmgkze.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2xqiykavs.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2lilwyjbk.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2asyezfkz.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2tdbwckjg.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2zzgeypmb.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt2dddvqpkn.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2cfkblhjp.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2hbnbkbrr.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2hmbxzruv.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2lugoxhkl.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2wkcdncdu.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2hpaoumij.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2wajdtdcv.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2kogxtnpl.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2tipofylq.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2zafgohwj.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2ldbzlaix.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2nniwzviy.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2vuuwgwbq.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2cuajsxmn.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2whqmbnuz.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ywurcylx.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2lmhvmttq.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2fnbfhlru.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2tbtkpyxl.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2miktlrez.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2jbsmjbed.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2hgiauymo.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2pnseqdhe.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2xcnmzrsc.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2xtisolpu.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2nwequjvj.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2gbqymngj.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2bjycdgkd.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2hxbwxdil.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2akucrgxi.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2pcjoyfbu.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2formzckz.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2klkuipli.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2sgrkllbd.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2eyjaemdi.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2nkbrwaqd.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2pkmjccmk.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2hgbywgyk.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qdokuqqt.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2kgnzkdle.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2zsmshedd.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2pmcoydbu.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2nzdiloyi.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2lbwwtvgb.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2csjxbhmr.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2urmkoztm.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2uqmzysdz.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt2znntgilq.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2ehkqqkxc.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2qbfoowtr.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2ygtwrpwt.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2qobxxkzl.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2vzztpasx.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2jtvimeth.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2ywsfrega.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2iyrtvlmd.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2wghpongq.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2ipsratli.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2gslulhmb.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2iqhrpstj.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2knczagsc.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2vnkhypuj.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2miyvlwpg.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2pqvahqsv.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2cthzmnms.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2ztwyakht.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2emkplgdk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2xhwbocux.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2wjzuqepj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2arzwrzen.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2jzanyrsb.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2xwgqyper.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2oeabkhpq.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2nxyxpwxw.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2xkrdmcbq.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2gdidzjio.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2lcxuizzc.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2jrlerobm.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2shldfjul.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2fnnbkgqo.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2esxemjvn.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2qgeosqjv.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2vubqatsq.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2vozomnhw.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2dertflum.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2enxznusx.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2kyqfdizs.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2hgfoasou.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2esoboexm.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2hvglbcpv.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2liuubdhy.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2rsiprbnp.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2ulrujlkk.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2rdbdtdwz.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2lgvbghok.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2oblsuygt.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2nmfflzzq.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2rskujoox.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2dadehoov.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2bnijhigz.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2vgaphjhd.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2eznsidti.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2xwjqthln.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2vygcstsg.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2odxinmlc.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2jgjeosuc.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2jhfbpobv.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2tjfmnyps.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2cnqjcuym.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2ifrzqzga.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2mczkhjbj.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2zvgttvia.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2qhxmqplt.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2jahcxrhk.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2sctfmzpn.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2ibjuseep.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2hnloiyyu.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2neazndwz.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2phgveceb.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2niynhgsb.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2nupzfove.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2ycpuuedq.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2anqvzjsp.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2atjyfczj.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2cmtpchda.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2ajahjcwi.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2ndrismte.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2wtqmrrjb.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2cizflvqz.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2rrqlhxdu.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2xcsblfia.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2aapsuhxs.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2ivrlwfpm.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2woobgptr.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2edbusaec.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2ccnmyrys.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2pvuqxskj.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2biqsdohz.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2swffzvha.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2duxfytga.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt2cmknnwxl.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2tsfuprmd.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2ukzlezvq.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2zyagfdiu.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2udyuckvh.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2xmmxqvmk.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2gmqxofqh.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2ujwmpdvd.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2ptithfjt.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2rhivnbqe.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2qjjgmalu.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2hqzkywet.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt2utgrsrzr.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2qpnkosgf.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2vbajseca.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2kwlawkos.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2jzehfqwy.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2jafpagdh.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2qqktkdkd.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2tpixkfgz.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2petfimen.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2dujhtpkb.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2buejddty.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2qumldpuj.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2dnpadefp.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2hdmxoghu.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2gqsxoppi.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2jopgtlrl.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2nnewjhza.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2zmzkrlxd.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2exjcwjmt.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2bldhgylh.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ddpdkamp.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2vfngthuz.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2odmtzhwm.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2dlhkcrpw.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2razbfqzm.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2loqbjbmu.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2ercciphc.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2sumwceck.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt2kqmsbenm.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2hnrtemag.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2ijxeewqp.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2jhpfmwph.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2ipfjzxjq.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2ieusqwlq.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2zqvkymcg.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2hvucpyrt.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2jvuonppj.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2piqzffvg.html


<!-- 参考信息 -->