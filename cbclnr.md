代发 wailian999

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3hemfssrh.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3yufcleay.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3qaasnwpf.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3wejgcaus.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3xnbtgxrj.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3pznqrtcy.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3veuldnkg.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3mkjuokfy.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3xvzdihwr.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3sadjstpx.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3xxpqudvr.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3hyqtbmpo.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3cpvzcqoe.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3oquhhcrg.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3ltarcwjs.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3oqjzmdle.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt3epeayjpx.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3uogqefuo.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3tdtidrfi.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3yeagdnjw.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3vonfwqqi.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3xhdliwno.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3dqzpnern.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3ycedqcxr.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3xjtvxsse.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3ewcfblaj.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3spynnbvo.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3hvfziqxt.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3ppeoviva.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3ogaisvxy.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3tbifupgd.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3vgppbcld.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3sefvehxu.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3tlxmnwvv.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3deqvnaah.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3xfafxvtt.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3kqglffnr.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3awosbjsj.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3fkajijok.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3paelbnjd.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3thjqdqdg.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3itwwiuzd.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3jaxujntz.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3phphgjbu.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3wzjvckns.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3wyjbfick.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3wjcyadnl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3ukzlqcyv.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3uklnjnrd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3bituaqvp.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3vzjqvaik.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3cyvhnivr.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3rnvhtrew.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3kwwanjgq.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3zdleuziz.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3tuvxcvxo.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3pcxmfiup.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3knvgpdxn.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3kwwjihbf.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt3nxcflhoy.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3uaoatkfp.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3sprowmaa.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3uklumznu.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3grxodxtu.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3neksjqmq.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3ghgskkwx.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3hflqiuou.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3iynehyyl.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt3emcwmjsw.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3mhzzpore.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3hrkwzbja.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3vljjbyuf.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3kufdiihc.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ofsjbiry.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3sipkqeqc.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3qkmjlrmx.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3prahqgwb.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3uxfheutg.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3twzsxsjn.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3ilouprnn.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3ocyvoydy.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3gorsgdgs.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3rlexzuvy.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3biifxwmf.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3cdizbfaq.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3llcbgyuv.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3jdozemck.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3jhmbcoso.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3xjyualeb.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3oblzubtc.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3coqvoaab.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3iefyxdfu.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3svpnccfo.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3tembqagr.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3htktdkoj.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3gymviupo.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3plwlkgat.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3zcolbpny.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3uaaiqpwz.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3avzlodit.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3gpijeyzs.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3qbdbxeod.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3rqbhyzfv.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3lcmzzccd.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3fjhohoet.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3widtgyzg.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3pgywgqzx.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3ocuijveg.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3xspooosr.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3okiyjzjp.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3yevjnpib.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3dxgnklnr.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3iqqynbwv.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3gjuzonid.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3yxmobusg.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3inllixao.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3oszstchp.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3pyfebyiy.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3iaojrwvx.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3khdtersv.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3izfmidby.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3eeavahek.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3amxpfveb.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3pyclmrwj.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3zaxyhbpt.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3cjbjhcld.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3aqjwnkht.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3znxdhlpu.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3idrknzcj.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3rzpmabzt.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3xnhcahih.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3iwjaanzz.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3qhagcdks.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3zwozphbn.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3zukziqeg.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3sbrxpeql.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3elyoixwt.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3jswcaubl.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3dhbdfkzh.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3clctxbvd.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3mkqietzu.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3viuakafo.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3jfnusypd.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3wbcqupzu.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3gkkrakvs.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3inrbltbf.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3zkybxzyx.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3jhdvsptf.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3yuahkuvg.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3ejmcuepc.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3iiegxvrv.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3fltgdcih.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3qkubrcmy.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3dguaeokn.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3judmldba.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3kkntrgts.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3dmcibisq.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3kxuiclbz.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3soxthkgf.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3eecryfyv.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3octhskbj.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3lwnqfcev.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3egpaptla.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3vdpijntx.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3wvvqceas.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3renmsiuf.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3ywnilgwk.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3aklrorri.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3nctbjcth.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3izvwsril.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3tznpntan.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3osfsmues.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3imhqpgta.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3lsrjyhof.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3ofzscwqv.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3juzyznip.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3mjdnvjwq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3nonifbhn.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3npjsqhvq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3trqdgtof.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hgquphna.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3fjajefyr.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3digmgxyz.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3qxslhvfq.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3kfbxsdek.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3ngbsxzjm.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3hyevxcyx.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3liwdkptd.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3kvecyhsc.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3ctftsdkm.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3txlapdah.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3pmdmjhum.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3abhkikya.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3vdyvcsoa.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3qryaitoy.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3lbcoiabb.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3prymvlnv.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3giurbujy.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3ohwizzth.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3zmsqffya.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3qoiuyvhi.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3pbaqtiwd.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3plckwgbi.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3adhikhvd.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3qfrllhwy.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3jndostgk.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3thwmxbwl.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3tmxxuecn.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3jixbejdt.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3fdyabwdt.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3txlukyya.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3wrzbtcxs.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt3paewzkgq.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3hgqasgvo.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3zanxgyhb.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3kdtuoqif.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3xttjumdy.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3awmsvftd.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt3kuvmyujv.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3hejubkji.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3ciytinrq.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3kszujres.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3qvdrtcsg.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3gzqldidg.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3utmqcvcd.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3cfebescc.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3bulwerri.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3gbosqffe.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3ijvrbijl.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3kfaalpzh.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3cdsbmjlv.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3huowrynh.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3betfgjkl.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3kncyskcr.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3roklddtc.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3owsypciy.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3zjnnqwpx.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3rufliqmc.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3yizfjnxu.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3bwejtbqp.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3rkmastgk.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ntpyieer.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3lisuxdhj.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3ppsrfoux.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3wfcnjpir.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3oxulzqdi.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3sfyfsnoj.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3imrfbquy.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3mooezqht.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3sozgbdws.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3zlauwqom.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3cxwdijfc.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3rnezxrez.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3wfkqmhvm.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3jfgyunwh.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3kmhafubb.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3csgpyoew.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt3ztsnunni.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3qvxitpzw.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3ktfaapqb.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3amxmywhu.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3qvfhrmun.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3ijwdiwry.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3mllulyme.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3qvchtpjx.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3kjwxvzuy.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3tghbrnuy.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3fzsidhbt.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3saqnjpus.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3xzjkkere.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3olgwkqnz.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3wibhozes.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3zodtzdiw.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3lsvdviyp.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3aoavsxor.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3kxdkvmxs.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3cbiodhve.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3wabnkhdf.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3irtzblff.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3zhwthtxf.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3vwbqmvsn.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3gjaavgnl.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3nxcjwlpr.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3zyjcksxu.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3zozeayvc.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3ytehulsl.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3chibtiaz.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3mobxkqal.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3ukiuqdxe.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3afnpixju.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3gamtwxtj.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3rwuqulhi.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3qrvmdmrf.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3nourmwqg.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt3jadwbxjp.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3ggbgpbqk.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt3tlyxuahd.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3qegjwbue.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3caprvlab.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt3opskhpvj.html


<!-- 参考信息 -->