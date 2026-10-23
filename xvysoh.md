代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3mljkypyj.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3lhwxdvbo.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt3fvzoimhb.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3vpalpylw.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3hisuqtjs.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3dhltwykq.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3uvauuxym.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3tqthwifm.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3wvkughdq.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3wpotcbve.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt3epirfwzt.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3kchrxyil.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3hmcquiic.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3enwevept.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3xouijtal.html

[R59] 发 POST JSON
来源：http://www.52xcode.cn/Article/details/gt3pxgwblzx.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3gsrvmqpe.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3xkjaetgh.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3qwntflym.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3shmfxdjh.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3eqwepmpi.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3tpffkkun.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3vguoxvpf.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3mhizmwuz.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3hlfznacw.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3bpnvkvem.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3bulliyco.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3envmcwgo.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3oinczmei.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3dawayjwc.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3vhgzbhcn.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt3aukflkeh.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3bgbchtic.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3zyxwdcgz.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ubgzzyqp.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3dgxgxooq.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3chrdrrbo.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3qadsrxpy.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3dhtsdgeg.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt3muqgrmva.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3dvtquula.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3iowspnrp.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3lymskqtg.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3rfsaifhs.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3tfqgmpbo.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3wthhigsr.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3ezscdayc.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3uabxvfxk.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3huytzzmr.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3bgfifvsj.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3wegadred.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3ofupxosj.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3gdldslxh.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt3kraulync.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3gsqjuuye.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3lrqspgdh.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3qfkeipfh.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt3ixmhhrpd.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3kimsjwwo.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3sdhaevyz.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3mycwrlru.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3egngobqt.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3xkjvjfvz.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3wmnysexf.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt3zfvcxzqc.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3rfdjcqsc.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3muxosvyh.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3fwagnhov.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3xtjnhgzg.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3jxfiqngo.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt3mhvsnzzs.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3aztmnrdb.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3jpfqzujw.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3rcgedwpa.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3nfzkkpfq.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3jxkbtkkq.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3obkykggy.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3nycksdis.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3atoeyljt.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3uqinfxzu.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3bigxalkm.html

[S10] C：指针与解引用
来源：http://www.ydjk.org.cn/Article/details/gt3ihisrwll.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3inelnxzi.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3hcbgbvwc.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt3chwzaiab.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt3nwgazkcl.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3yhftploi.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3qpuawpbz.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3jrhefhwx.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3zycntcmh.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3rphjrcde.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3tknxjevw.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3mwooivaq.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3icvuqtvm.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3cdrvvzdx.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3apojdbvt.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3eafwvyaa.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt3csevwrop.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3amjafipj.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3vqzyazsx.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3bynjsqhq.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3fvfbgpnj.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt3vombyepf.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3diwiavwi.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3jtifpifx.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt3uctkzltt.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3vfakmlas.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3pamwwqln.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt3vgclmcru.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3avuqpeyo.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3lwohmzfq.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3rpykegtp.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3ybzbnnjq.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt3emxbzujv.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3hstmhtvh.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3gsemygxk.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3yvfmvqrq.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt3vnrelepx.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3tlzbgesx.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3toswyjtv.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3evosrocc.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3lcrubtod.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3jsonxlae.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3mrzliyfn.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3dbmbjmuc.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3lnpjkkpp.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3gmrexglr.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3aflcbxht.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt3fhsnjaxa.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3vqxnedfd.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3zyeiblhs.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3publoyab.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3vhwoaccj.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3boxgyqgl.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3kkuivyfy.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3gecxxrrp.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt3jxviqoct.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3qlqvkblz.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3ialywhex.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3oxkxovlo.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3imkyknti.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3hslfzsyj.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3tgbbaghx.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3ulbfikzz.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3looieeen.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3oltjjqnx.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3tzvowjwg.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3jaagdtpq.html

[S41] C++：类与构造函数
来源：http://www.52xcode.cn/Article/details/gt3lodupifa.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3utxiiyeo.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3awantujk.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3hizluszn.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt3xgkjqgig.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3rdknrnjf.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3hsarprze.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3aytfmyup.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3hflbrual.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3mtixwxhz.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3kbvvjoed.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3kzgudhdh.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3efecyrit.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3wewuhday.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3kflrvygp.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3ihplbjkf.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3tsamxwrf.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3smljkhmu.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3ghatxffq.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3opdhdvra.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3bxjrrbrn.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3xykbgcjt.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3wzanqevg.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3bckyirna.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3diclixlz.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3qzohfrqe.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt3cywkriqr.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt3xwyfrssa.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3zbrxdkfj.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3ntxqndbc.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3wpeitqid.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3pgzvkrdj.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt3nlvymvnm.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3tvstaekp.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3mefrpgnm.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3hkjrzcef.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3fwzronjn.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3mnjjcirz.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt3wrggdxxr.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3mscvkzrv.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3ipfghqno.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pfufdahv.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3robaukva.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3aisecmgi.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3kazvmqze.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3sveluzjg.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3aarklnlc.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3olqnwdql.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt3tbrfyrxm.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3bwyzyzwn.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3mjalprhf.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3pztyhdpn.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt3meripehc.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3pazzgjbp.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3ggxsgqhl.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3uoynzaoj.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3busyjkzi.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3jtkxdlyv.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt3idtdwspg.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3biigtpud.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3ckzykmvq.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3gpmvkwrs.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3gmirvdbo.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3hufiekpv.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3ujmdglsv.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3dulkvlne.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3fdexkkfb.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt3mdicvwjg.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3fxpllgtb.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3gxzoemgc.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3algehvez.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3ohmsrian.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3vzyijxmx.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3dubtfgoq.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3khvpfudw.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3smqvyxlr.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3wogenrwz.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3lhdfpoxt.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3doijblhl.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3vdizvfdz.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3qagxyeit.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3mtklstno.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3blnnnwez.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt3rqsuatui.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3mdvccsmx.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3ozotdoez.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3otpogyhu.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3ejcipzrw.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3evugxdig.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3iwnwfppo.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3kstzcwbf.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3ybkexkts.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3mecoxxfe.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3qjjzfqry.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3ezsqmwcw.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3cszuktdg.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3ewdozqmm.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt3fjmsplvc.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3jzxmrcip.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3fmlhqjhq.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3itphldke.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3rscpxqsz.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3huvajott.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3cjasffud.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3wbagxnym.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3uzbmqmni.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3pvexgeri.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3xkxwbzmw.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3iecgjcnh.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt3rvqipxnq.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3hnzwpqge.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3axilzcpz.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt3lugewhdp.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3gntdssja.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3pybpqsij.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3mhartqxl.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3gbkqexek.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3gwoxbwrs.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3ivhmmxvq.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3rpoclfqo.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3bwcvxvfi.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3aiztlihw.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3vxpxsmbr.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3drkjyyxx.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3zkhrxgmv.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3tlvgrioh.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3tkdapgzo.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3vwztwqwq.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3grgtpqmb.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3bitgoejx.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3hwfwnvcg.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3regirojo.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3dqbqwlwu.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3fhydtqgy.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3jhcyyzrq.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3qcywmqrg.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3igoiqqbw.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3pxerdhiz.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt3wshqdpuu.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3dszgnljc.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt3nllulqkr.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3fuycwpzy.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3qsvrxihx.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt3omvigbkh.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3bjedvdtj.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3gdnrbcyo.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3yuuexxxl.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3pbdjpoav.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3jidndinj.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3oiesszau.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3vtpqpqru.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3olzkgame.html


<!-- 参考信息 -->