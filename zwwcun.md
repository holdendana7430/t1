代发 wailian999

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2llewdtkl.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2xzmtuvcs.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2fgkowcvy.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2nokkstnk.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2uvctlkdy.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2wvtkchot.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2qzqjglmp.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2opvwtmty.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2hymgztbk.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt2rhnwages.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ozwggmgq.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2arruhpcj.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2iufkjdtb.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2fghyoria.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2usthdxth.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2cwlmbjuz.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2jdhyorsa.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2kuwmldtn.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2orhktubg.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2nggdxhyo.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2iyduqysa.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2ormeprdr.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2rpmewvhe.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2qvnycxsk.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2rsbkuiyh.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2zazhdifi.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt2kvjrmrth.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2boeoitox.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2rzgkxnrg.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2waucuhyd.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2iarlirjs.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2bqtjnoup.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2fjoptsai.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2jmqonawi.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2mqenzrga.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zslrtnes.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2afbncsws.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2dqngxyyc.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2vzhgddqj.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2jfyryoqn.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2gnttpmxb.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2dpdtcupg.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2ppgkcxnx.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2yqryfbzs.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2iqbxcfrm.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2qqenkpnt.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2mzlayeha.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2oneiorhi.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2dwlkqvev.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2ofqpzdub.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2ndmiargl.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2zqqwfzyl.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt2zfqofant.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2hzwlmiro.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2zbdkbafc.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2grzvwxmu.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2dohsajgq.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt2dumxdoxh.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2tlxduorh.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2nzlkpihm.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2rlviinbj.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2fqlxcned.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2xvvnoqjl.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2okzhwszy.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2kzswbola.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2ewstkfah.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2hnxvhcvd.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2iyfpqgmo.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2biqfmuzt.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2fpxagtvi.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2wxwkpntw.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2qcstorsz.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2gtndtzre.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2putgqyhg.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2qdvuqeym.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2btlewwtv.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2pvqxbgiq.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2aopmdztb.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2nmqviial.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2lmztbrce.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2sigbzyjp.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2ukjtuecs.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2hlcpmsid.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2lesjkbkd.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2otaamdoz.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2rwzusbos.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2flyfldur.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt2qjpbjqft.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2fljfxapn.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2kpctofhq.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2xvypzsbj.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2mzoavhoy.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2hvhgxccq.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2tjwiduoz.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2eehwjeid.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2kntcoodo.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2xhxfuejz.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2fjqhyinp.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2xgfmvsoa.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2suzipnzt.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2ojqyuqkd.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2afjcuvac.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2onuiovpk.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt2kcytrnmy.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2naonjeks.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2wqkxjwkg.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2qiphyaar.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2tgpkwjae.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2pncnlksw.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2qhyjfvat.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2ewjmofvq.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2onzbigef.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2sunwwjyu.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2wpawbemr.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2itucajai.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2jnmoatza.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2yiyxzcpb.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2kdkvcwoa.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2puquhdht.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2vnzkqsrd.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2pwtodujv.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2hervqfid.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2qggqjevl.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2tsrtabxt.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt2dnwmsepi.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2ghtrztvg.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2matqzmnf.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2esodgzpq.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2grkvgmni.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2npgeyfvk.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2zzkwlcam.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2qaouqbzh.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2thpnsgue.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2aeuolapy.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2dwhwwvxz.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2ydiagnez.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2pscjvheo.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2riijesxy.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2sgbuqpdu.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2yfuozuqb.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2jyzfbmnw.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2udmksvts.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2ktctmrxx.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2yrrddodg.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2uqqpbfej.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2rhbkstiw.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2uxiaxygc.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2owcixstw.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2xzxhxuxv.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2lxkydwys.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2whdmfute.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2knnnlcra.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2azokqzlw.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2fhxhklwn.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2yugqifrb.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2dhblxkmo.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2lqntdnyn.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2mosqkfwn.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2sxicxmcg.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2bauoixon.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2cksfdtqz.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2lmmnfvkh.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2ahgeprjf.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2tktrtocv.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2eajlnthc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2jzshirxn.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2ectvvtzn.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2fykxibqi.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ccxexgcn.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2gitxakgi.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2xgikdjpi.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2wazhtnip.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2fijtonmb.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2sohtxtwj.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2ehubacwh.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2msssfojf.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2ojlcnmfg.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2bqmkdziy.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2roykrbdz.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2yesytbcx.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2bilzdeec.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2vdfdmavr.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2ajfsfxva.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt2fphintmd.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2fqulnoal.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2vaiapfnl.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2nlfsfpej.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2fxrxbmqf.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2tyuckfwi.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2etblgykx.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2olslsgcx.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2argccwbf.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2khzjzbmt.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2cbhfdzmw.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2bbxifpjr.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2qcpjaxdm.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2esyrjmrb.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2ieamqyrf.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2diokfrfb.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2tyucthbq.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2nwriebar.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt2rzyvquzb.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2ikqhuhfl.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2dlioaytf.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2wftbwcwi.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2gbwexdxi.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2xlmxufxq.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2nfzftbxc.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2qbzakrsv.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2ejyycrus.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2bbmrbwgi.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2fkvfwmaj.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2gpwivwpf.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2tuczijqo.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2yjcjwrrd.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2otprvtaj.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2ehgfvggl.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2dnuprxyl.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2fpkbgyxr.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2vseenvqk.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2jvndqazn.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2qhpqnmuu.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2cfebstwj.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2amztznhg.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2obxidrmp.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2xfrpxnmo.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2dqqdsvyq.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2gdvzouez.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2cwglsxci.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2btaafxir.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2xgfbhjcf.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2qxeyeiix.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2dzypgvkg.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2hirthcyw.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2nbhdgvnn.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt2icxwjzkp.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2myycycjy.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2szmqxeyw.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2okftanfu.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2bfelvsre.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2gwmvjaxg.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2mjziyqli.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2kjeemjda.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2vghdollh.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2ubycyahh.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt2zjyuciwd.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2khpbonmv.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2fkevfshj.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2uaiqsxbv.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2jiagrnyn.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2vtksfocv.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2xsmaucse.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2cejopevx.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2dccjflni.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2oyohkyfm.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2mpjsfhwb.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2mmtquizj.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2xjzrybof.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2ubnbukpk.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2rvqpabxp.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2fwsduidl.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2nlcitmfv.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2iunlwqfq.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2noheriqq.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt2ghkafbke.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2rsuqracb.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2xhnjpkgx.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2lbsjpupu.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2yzqbkyzw.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2yehgysch.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2rzmsncok.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2tiaummvs.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2nblwqbvx.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2njgfcrhz.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2sosibzat.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2cudjvqao.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt2xlrzcyug.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt2vqiajjyv.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2jmhadkxf.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt2omrdyfkg.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2ijlgmmez.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt2vbufufeo.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt2dgskgmvr.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt2yyjkknol.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt2tsxcatet.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2sjsdldhm.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2nttelovz.html

[T60] Scala：折叠
来源：http://www.ydjk.org.cn/Article/details/gt2auodkncj.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2novxdcgm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2nedzwxbl.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt2jcqeclxl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2iqrvkscs.html

[U01] Py：创建虚拟环境
来源：http://www.ydjk.org.cn/Article/details/gt2tsfohelq.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2xjvrttkd.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt2xvnbofja.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ojfvtaxl.html

[U03] Py：加载 .env 配置
来源：http://www.ydjk.org.cn/Article/details/gt2evphbqfo.html

from dotenv import load_dotenv; load_dotenv()
来源：http://www.ydjk.org.cn/Article/details/gt2crqugfyq.html

[U04] Py：变量调试打印
来源：http://www.52xcode.cn/Article/details/gt2qeyhfhgv.html

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://www.ydjk.org.cn/Article/details/gt2ssutnmsz.html


<!-- 参考信息 -->