代发 wailian999

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3omiulncd.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3ispummdj.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3nbszozys.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3myjkubyh.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3drszshmc.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3qzcfgzwu.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3zrummgin.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt3qrrkvmda.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3ixgmtava.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3wvqohrev.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3onmqktts.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3whvgolmj.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3fqaclseq.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3nvikgdtn.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3qphhwied.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3bilzxrsd.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3icckemkd.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3zazwycyr.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3okxryuoy.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3ddeedsdk.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3kcornqgi.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3masuknxb.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3vzmzwplw.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3tgarcxtb.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3diiujobj.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3gimfvzst.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3ouutcykz.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3gzczhibf.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3hdguvrhx.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3gqzkrazx.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3sddmzbob.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3gvmunwca.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3iahtasjf.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3qhokepvb.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3szycaldx.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3vewtnswe.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3vqafhfhp.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3qfgnghrb.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3hpnlpcrt.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3clvgmojj.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3gmiwtvmj.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3bydpdyeq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3xhsgalsc.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3tkthskzp.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3womobygr.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3ewegjivg.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3kznugjii.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3satqgcqe.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3lgjbddir.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3yjmsqoia.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3odhxfjev.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3cpokefvq.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3bfisozzw.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3xtgzurhm.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3xaegsnzc.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3pwvfoqnv.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3mwhvfulx.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3tnmnlbyf.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3uqfowkxd.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3yeozkwrf.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3xmpqfgzz.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3hozoctkz.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3funjfete.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3fsgxpglw.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3iiltxoox.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3pkgulvla.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3ndgxekyg.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3ddkzbgie.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3zgjogqux.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3knvxydlw.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3mfkbnvce.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3fqpbdtnk.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3nujhembb.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3xzhhxwkl.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3xlkjkrad.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3tezsygvv.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3udyuuxjv.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt3efujjgih.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3joiyhqde.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3zzypbeqk.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3tjziyare.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3cprhbmbm.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3kxwgprvh.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3tfoabush.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3mfcnwrtr.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3ppxmcsab.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3fkdzchtb.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3zzgktsuf.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3vnvlbmyk.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3ejpkswwo.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3wegcuqcc.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3byzpovxt.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3hyufaoog.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3yeckbfvw.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3innxglxc.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3badiknwr.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3pntpekhw.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3ckyagphh.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3uhpdxxpn.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3yixswwkq.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3mnijhbgw.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3ctqzlsef.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3npczkodn.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt3imbrvhal.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3adugggxp.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3cbrvwkvl.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3jyrigzfi.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3porwkhng.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3sczslyct.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3inmygcph.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3mocqebjw.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3laubqkfv.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3eiccgqzy.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3mxwfwtbt.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3zdznlbhh.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3hzoejhme.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3ubomkbis.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3kbfvzzio.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3nevgayae.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3rhagzxso.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3tysnpvut.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3aecmengx.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3vrlnxhni.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3bqrpytbe.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3zrlfrdfc.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3zrupqzed.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3xyzysgqd.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3fodsjbur.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3qdhynzfw.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3xkxiihkh.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3avlaxxrb.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3mnkvuddx.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3kkyzdbqz.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3pmuotvih.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3krodsgle.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3mzkyycqf.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3tohgherr.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3glozhtev.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3lffixysy.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3gheblcdl.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3nyrpadxl.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3gkwxccrr.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3uyucjexy.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3lwxrxqyd.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3pwtjsogv.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3eepyypmu.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3pynuzgmg.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3xvvbwbym.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3hlhbrdqa.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3zvpemluk.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3ugxycrqj.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3ocjlhpwk.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3vtqcjpzb.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3laoqczmv.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3zwrcmros.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3anvdcqou.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3nctpgpcf.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3hewchviu.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3dhgtjxjc.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3gnutrmvl.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3ypycpucq.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3waqxocrn.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3wahwczhq.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3uuwferxw.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3bpkuakre.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3bpjrtzwu.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3zgkpeavo.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3yvufifyg.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3jbfziyfb.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3wxpjjzrm.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3zcspiaxm.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3eekkwskq.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3ofowddbd.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3xlhzciur.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3rffsrxmr.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3jhyiprzr.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3ckbvwotz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ixojpsqz.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3shzbkbqe.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3llbkagsg.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3trwnwote.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3aebksesc.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt3tpohupbb.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3yqyendiv.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3bkxbgetd.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3syzlfkvr.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3ctaqcyzc.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3mrkzjypw.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3gwraxvur.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3hvnavule.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3izypshdy.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3aurftrmx.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3gyosyxzp.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3bjhrexqv.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3rsspbbvh.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3mlfpqmkj.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3nwimohop.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3ktgybyki.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3bdphkzav.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3mvxbpxhi.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3hzzxytqu.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3edgbpxpj.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3vsrzwlbs.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3gpyedmdb.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3wpasnmhg.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3mxkqnboc.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3zmyoksqh.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3qaacapcb.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3smcefyvf.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3jlhozbod.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3xeeqqlhr.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3fimflued.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3vfofgyki.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3ieqfluik.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3jwfodiax.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3urcfkbyl.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3ckyzzlej.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3vqteqmix.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3tdsbnfnn.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3yiycqqkv.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3sxnghnfl.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3izfitrab.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3erzhhauy.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3qgssktag.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3inizrlzr.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3mfewuigo.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt3selovact.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3dycnludu.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3jvanjuvc.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3nqhgbhph.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3vsltenjn.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt3txdapqqf.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3irnbvatr.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3ilogazoo.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ogsvevup.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3yuvwgxkf.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3tzjugzug.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3nqlcbkjm.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3pzhnrcvh.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3zrozlrvu.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3secrwgdd.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3minoymgj.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3tqeuabze.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3rtubmtbu.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3griaqkfq.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3qrrtobna.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3exahkflk.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3hlmjvvax.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3ievrjzgw.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3zzegxdtl.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3swyxmcso.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3davedanh.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3fnbbqejd.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3hwbzdqzc.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3qvlralfh.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3edjuliuk.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3nnqdvtvq.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3hduwshox.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3tkzbvaly.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3ulrazxui.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3gatrovrx.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt3veiwefmn.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3wjghbqce.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3kagbhfru.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3ganmygyv.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3frbqgvag.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3egkeckir.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ggpktcgy.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3nengivot.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3gatqgcrw.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt3jtvpacaf.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3nouekqtr.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3ttdmxpbx.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3vftxujup.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3vafyhjga.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3ucbiqkno.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3emtnauxw.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3boaostqh.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3lujvgwlu.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3uusgqpyi.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3whzkiyzx.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3orzvluqy.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ewmjnuli.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3huwtggsa.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3jxqcgrfd.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3mtrbefyb.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3sgarsfmc.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3oeugxlqo.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3pouhmxbm.html

[T55] Scala：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3xprkbqid.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3acjeswte.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3sstemxtd.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt3qyyibpva.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3mcmolhzs.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3vdkfuvmp.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3irrbgsgz.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3sigbsbit.html

[T59] Scala：循环
来源：http://www.52xcode.cn/Article/details/gt3vvpjjwhg.html

for (i <- 1 to 10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3wazohfty.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3txcckjpv.html


<!-- 参考信息 -->