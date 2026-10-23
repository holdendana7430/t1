代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3mvsfupuw.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3dpcdeefm.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt3nfxsnmnd.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3lzcenxcp.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3wuojqvcv.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3zzhomean.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3ccucshir.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3oyhyfijt.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3zaqwuupa.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3pfbpahns.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt3qvrcdfgs.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3gztlcrdo.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3beqopofb.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt3jbubgdjj.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3zlrzmpmp.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3kjcwwftc.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt3fummcocs.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3wgpmynlk.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3srmahevn.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3scklipuu.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3mayhojco.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3vlzwimwi.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3cwjhhcte.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3byufslym.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3npsbftqo.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3qgjplvmj.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt3epytfmkn.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3byvsiyab.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3ndokdggz.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt3kvdgtkdl.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3jrafdvdb.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3jwebhpxw.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3drrdnnuv.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3yseptlqz.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3quamesds.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3uyzaewzj.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3jatncrhd.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3ilrfywxe.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3ededrotw.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt3zchwtdto.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3llinioxc.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3qlvhzvye.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ptfrqvcw.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3ewatbiba.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3mcaynnij.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt3zlfnvfix.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3apubyfbh.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3ygaegmdo.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3tmnhlohj.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3ixjeaiti.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt3ccwenjve.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3jvavyksz.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3ezmcmkvq.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3hbufodrr.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3fuorvdhf.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lnpibfpz.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3tbjqsqfc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3jvlrytdb.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3kkziwfeh.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3pfqblxoz.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3eavfqlda.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3wrhiryxz.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3gxnmjiax.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3xkgmmpgz.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3swkffovo.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3kyohodpt.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3ybrppndf.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3tguhtjfe.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3ugtlgyqe.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3nazzrmkw.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3anpljcft.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3arnzczid.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3qniinxex.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3ivcrqlgi.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3nmcnittb.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3maueyxbj.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3vveryljl.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3utjxddqc.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3yqumugwc.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3vknxlwmx.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3lzgqmgdy.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3lusjiocq.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3ksgcdgku.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3yrdnmtlx.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3oabdglvl.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3ckbljaxx.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3vrxxlhml.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3vqrhzdwd.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3wcaroqan.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3ljjxqebv.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3pypllpcd.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3tlquvqcg.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3rjksgoxu.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3rhafpwue.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3fycswhkj.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3xcvixbyd.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3ntrwggbe.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3clfsrpbe.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3jlhukpvf.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3jaixtqje.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3oadlgyyh.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3fhwzrtla.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3btnitcwq.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3xzxwlbzw.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3ajlzpafz.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3cioiowno.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3zahdgcbk.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3mefqzgyd.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3dnojjgbx.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3avdsfmdh.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3grmetmla.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3lnqbmklo.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3iwfrvcmd.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3vrzeuvrz.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3imxvdnix.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3zkbmidto.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3xdmralyj.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3soznimaw.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3uhyrahjv.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3khgddafx.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3afbqofba.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3miieomuu.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3qbxklbvy.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3yojosnhf.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3zwxrsyim.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3bigwdusz.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3jutldgkg.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt3wocxdalp.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3nfizlhpv.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3rbkqgxje.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3ctixybqy.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3shgzmglh.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3ptcnfwhi.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3mqnpcoli.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3timmikxk.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3cusfrybn.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3etxjwuoy.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3mnbtrnle.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3ynhwfoow.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3ujiwbxcz.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3auitbcpv.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3vlsjjayy.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3yzvnjbsd.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3cgvvfqpe.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3hgkwyrmz.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3wnzujtcm.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3hjuxbxuc.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3gzdyhwmp.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3ltljmbmn.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3epeixodj.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3olkfgonz.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3cyygjmak.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3yjuekdar.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3lyqmdsdc.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt3kufsiouk.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3vfjwzvvt.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3edukaibb.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3dhezokqm.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3bpakqacs.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3fxofowjg.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3jehsayrk.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3czzgapsq.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3hhlvhxjl.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3vvivpcmw.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3dpmymnpf.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3eifwcyzt.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3feuaxkek.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3pyefshpk.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3gqqbkxkf.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3idrtunvk.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3pyhbxgqu.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3zhwgabps.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3bheqjhmf.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3lratzndw.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3lkmszogb.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3kjkhcgwk.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3mudyqdpl.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3nhcpqmci.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3jpkzfeud.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3ovardcyc.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3yxdxdena.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3dbadesvf.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3tzmkmzib.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt3nsdirhph.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3bihzbojv.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3wawjmwzc.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3oabweqts.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3lgafzixo.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3fvbnsvha.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3uirvyqmy.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3qqixyngo.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3dbgzaoqw.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3ldqmodaj.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3bmrbydez.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3tgzwvhsa.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3svtjsbsd.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3iwtjlruv.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3sovlisxk.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3wjmsyrkf.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3retoyhsg.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3tmluysbw.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3egncsyfl.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3virrkcon.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3aoqhxulr.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3zmgmogus.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3yazihrqg.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3kjbazkwc.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3vydpfnwu.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3vzjyyaxn.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3uxyazaos.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3fbqatksb.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3jykucrcf.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3sbeqnybj.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3xysaeyuo.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3hxgwofrn.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3vwktlfpl.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3fjgcwotl.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3uanhmxkk.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ayusxdla.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3mbqsfqkh.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3vklbyjqx.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3hszatpgu.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3kuxlgawj.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3komscsyc.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3doncoxci.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3daplfutf.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3jivcfkwf.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3mewsunlo.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3zbkbozvi.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3vitvesbx.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3idvwgkvp.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3esaypkcs.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3uplkcroj.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3ooyrrfhz.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3jyzkmmvi.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3ahnhdafl.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt3awqolgal.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3balrfolo.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3xzpbjhcg.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3cfgwqvcs.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3wwbrsswa.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3xxlaenaq.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3ulboepee.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3rjnizdes.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3ezagzycv.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3lgnwpwwg.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3oexcjozc.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3kzhzhpyp.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3dqdaammb.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3zdiigilo.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3cayigeph.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3zjhqvltl.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3jgkingww.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3watpgikf.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3dvkhgimj.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3ppcoiuam.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3ovyzjvid.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3pxjulpbb.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3miszhdyn.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3kdhcqfnn.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3orhfqnor.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3gyvfpfdx.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3jyfbbaki.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3wydovtin.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3nejpfrcs.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3emsxiqyu.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3mnsuicoc.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3bqettsda.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3npopbwna.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3sfnmvapv.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3hpdrdlcz.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt3hrynowgh.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3mgmsavxj.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3yltljslj.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3akjrqovk.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3pqdlzith.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3gygmafrx.html

for my $x (@arr) { print $x; }
来源：http://www.52xcode.cn/Article/details/gt3wctkhdea.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3ujzazbqy.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3hvmiaxye.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3mvpfxnak.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3kgqiaprs.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3ivzjeqbk.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3gcstqnkq.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3msqpyalo.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3svwdbhtd.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3vkmezbbj.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3otbhcxcw.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3vutylesh.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3tuntykfr.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3iwhjusac.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3ocxggzxk.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3anhkryhn.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3muhperhr.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3vwisrkdf.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3hnljzlij.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt3zaumbnmj.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3qrzajcda.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt3xvysbdwm.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3vwzqmqkp.html


<!-- 参考信息 -->