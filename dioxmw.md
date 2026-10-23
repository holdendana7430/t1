代发 wailian999

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3xvamdzsr.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3wlwrhphq.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3sbaltfuv.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3krbjovih.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3udvrbsxk.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3ucxhdllt.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3xypctwit.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3xvkuagpa.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3vdknmqom.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3iwksmmrn.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3abrmtpeh.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3oycvxess.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3qyrequon.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3huptmbih.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3tplvuwne.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3sshcdnon.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3duvyghcy.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3cqnyujrz.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tidjagic.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3qfhcskct.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3humtssmh.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3vhytenpk.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3zceglolv.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3rbdmqfzg.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3fcbutdvg.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3wwojvnfl.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3nxhcwzmq.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3xzzzfioz.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3alirgauy.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt3uquyvgmx.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3cjmrqibq.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3pynxkhrj.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3qzjmmqmc.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3ymnwbqcs.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3nfjubovn.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3fhmvcfyf.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3kxusxatp.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3wlbgqakn.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3apysmvif.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3hzfvswfk.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3isvnkire.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3bwzzijfb.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3daqjkndd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3tbaescej.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3duznrcid.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3uvoearjg.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3swdprqjz.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3ibshqqiz.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3thlyloqr.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3imtumwws.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3ujaoskjd.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3ytabrmwa.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3hgksijay.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3yhqltepm.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3hwqjaosv.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3usmnhiyp.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3hahkhcpj.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3cwnuircx.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3auxntfnd.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3kaouercy.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3ucycroqb.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3rquoxoqf.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3irspafig.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3cvwwwrvx.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3wthgplqx.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3slwuwerw.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3kvimkqdn.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3bmvolqhk.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3wyfzddee.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3cwwmzkdj.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3syjlaxde.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3dcedlexk.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3qhzuxxgo.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3rczxegxh.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3mjsgdstj.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3zqeeyxnm.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3eaawmcey.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3sqbyqwjy.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3kxobvkex.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3elcodfwl.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ihwuwupf.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3pzyqonvg.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3bixshuqc.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3ewhploho.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3vpebyeyc.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3usptrfik.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3uqwweumz.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt3iqwyclah.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3ldkogmpd.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3cntdytlg.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3chijielh.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3gnanxjbl.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3wruiakgq.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3nzkerzud.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3ttqlfbfq.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3ztuexyge.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3wxvniioo.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3slguuhvp.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3snydzpzb.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3pfytcpvm.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3bsaifuor.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3wghlqcom.html

const double PI = 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3qvvasoxz.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3ecjkuofc.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3asaoevfs.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3drgxveou.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3qjqstcrn.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3erxwfplu.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3bpnieize.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3rozyagnn.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3yzddhbvv.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3eglkkjns.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3gjcwqtmd.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3jqrzktol.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3moztqkit.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3gvbokdxi.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3jpktpivc.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3hodfxbgk.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3snzzyvbi.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3czziuchl.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3etewwued.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3rcunmuhm.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt3crdyhrjn.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3qshciesx.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3mvqlazuk.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3epptshys.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3aektsjud.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3wjwvrzrb.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3ngdjrigt.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3fgkxvmlg.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3orpvarlm.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ylkciaky.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3ekytbqlg.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3nscixanh.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3eshznmia.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3rvudmpsy.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3mceggdzk.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3upaifobx.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3hfrrdtfe.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3bqwhgyhv.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3eeurkpym.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3drtybogo.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3lmjlateu.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3qyhfvpzo.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3tfmvxphp.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3gqjrewap.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3mtkmzgzr.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3osncnerv.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3mdrzbzdx.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3eipdmivs.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3shhcjdrr.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3qmsoqgxm.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3bbhjgwzx.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3qondylul.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3yiasbysr.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3qyyalqmf.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3caavpunh.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3mblzfohg.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3jeybthtg.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3bvtkahiy.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3psgpiqqi.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3nhvnqfms.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3nnnfryad.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3srzzmkfp.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3enswnwgc.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3hiyflzpe.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3bondnrrc.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3mxkkcioo.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3mnpyfexf.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3wqfoyohk.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3jpwtqnwf.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3tozgnbad.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3zzgctghy.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3wpmiyjhl.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3dsmqlebo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wycbauqt.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ynugihpc.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3vyjmccep.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3sqnzjvzt.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3ohtratuq.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3bsevpszl.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3tnkfmttc.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3dycxvxnn.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3sxhmmaos.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3iqffcnhz.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt3ajgjkzai.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3fxstlfbv.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3vamhhqgp.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3hkhjedzx.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3zdvoawjs.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3ujipbegy.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3lbobqimq.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3clzwhwcg.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3mhxudcqf.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3psynxyte.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3adlhmfio.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3mvngwtzi.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3qfvnpqoq.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3dnbetird.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3zsommden.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3esqhulvp.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3hkraoejh.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3naitbfuv.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3koxmndfb.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3gyushjer.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3kntazqim.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3giiypbni.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3rbpfpfpl.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3xnbvcbzw.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3ckypelaz.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3mqpttvbs.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3popydstp.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3yoxjvoic.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3nvfdyglx.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3uokaywes.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3gexyetsp.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3amcgsuyd.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3sfbpnedw.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3fgoheyrm.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3wwvgppxu.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3llqpeefl.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt3aunzspxa.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3gbduyrtx.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ifrxkglc.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3gpbkwnzx.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3kzskiwsv.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3tbrjqiwg.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3hqohxiuc.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3ogcvntzm.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3syhcjxqp.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3apjwccnz.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3auvtqory.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3igxisetk.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3wnunewri.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3ifnkjphz.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3dehufwsf.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3bfttcrml.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3xdpkobxr.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3ihzhqsya.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3smdntdoa.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3nqjhuhbz.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3lcphrsla.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3nueusazb.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3ufdzhxue.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3xweovqpv.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3qaqzbimt.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3bvwzaduo.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3ubezyhve.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3aiiugoaz.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3qeticanb.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3texklffp.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3rndphwxg.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3mcuqxaoi.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3xqmebhdr.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3qsufuedr.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3fcjezkmq.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3rnfjzomx.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3rabbvzhs.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3cmcbmfgm.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3ztmzfuas.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3gqhcrrhv.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3edvdmpby.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3qkuqqezx.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3jocdodks.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mipvwitk.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3ybdqhjdm.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3ejargpdn.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ejbbjimq.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3bzzgjxcl.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3ziuipmtk.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3vavwjxgy.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3gtgxsbkk.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3jihwasoz.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3agnkpitx.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3ererikja.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3oxwkhhbu.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3vbvkogsq.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3psusmsoi.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3yzquuvti.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3ygnyyakp.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3ipbdqlmc.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3dsistdsv.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3mceforvw.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3pvvpuynk.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3oamulcum.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3vtuksxyi.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3sdlrlnpn.html

[T56] Scala：样例类
来源：http://www.ydjk.org.cn/Article/details/gt3gkshskxm.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3yetsdvdz.html

[T57] Scala：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3tskwwrvl.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3vypayiej.html

[T58] Scala：函数定义
来源：http://www.52xcode.cn/Article/details/gt3udxmhjxk.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3igfetvkn.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3qkjcqzlu.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3leqyjhpx.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3iujeqxhu.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3lmebuchk.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3seatgjex.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3zxkuckie.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oudtcbyw.html


<!-- 参考信息 -->