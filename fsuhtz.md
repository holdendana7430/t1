代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt3ndomsjhr.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt3kpekrsoh.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3ppmhyjoy.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt3zftdibfk.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt3ewtxqbbg.html

[R54] 比较两个文件
来源：http://www.52xcode.cn/Article/details/gt3arxiywxm.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3swjkbykt.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt3jterieop.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3okdemveb.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3uznwfqtj.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3pvofwtwc.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt3nvrghzuc.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt3sioezjck.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt3camifasq.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3iobwfrox.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3chcnfubw.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt3bmtipvrn.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3xeckvvqw.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt3klxgpvpy.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3blhleukc.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3kzogswnb.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt3hykdsaen.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt3nvptvgfz.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3cswoenzm.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3slangpzl.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3eoxfyqzh.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3pablbbjp.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt3yjjuiabq.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3szfaqaxz.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3obvxzbcq.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3jkqlezrf.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3uhqohzmg.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3jhelsmfc.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3fwqnqvak.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3zgjowgdm.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3wrybkurv.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3vnkhnwlg.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt3dazhtubj.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3xyvpisiz.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3awncdxml.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt3iryzruwa.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3evtaalmh.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3biqjvxju.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3xiczljyy.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt3blppmexy.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3zmtqxelg.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt3shahogxa.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3ojkgaumx.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt3lietowfy.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3mudzkdwu.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3zwizrreo.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3itbwaerq.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3kldzsrlf.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3uyxnqwbq.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3hledooil.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt3yokptgcx.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt3pmruelpu.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3nmjluwpv.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3xjuthsrs.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3qapqlpmj.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt3afizvmhz.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3skndukse.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3ddmuwilu.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3fqmqsqgr.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3tiwacqux.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt3dohypary.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3drphsnfd.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3ktckiwep.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3omwhpyka.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3umswlhal.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3gctmoeom.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3tltxyrct.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3yjhpvkef.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3bnhgxkcy.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt3dturifvz.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3bjznlvhx.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3lqkrkbrp.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3jffbskjy.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3pmjqdqpp.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3gqtiywwn.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3edjbnhdl.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3vdlktmui.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt3mhfvtyvf.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3enqobyth.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3cenexhsf.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3bglvmpfu.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3ktfdeukr.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3jtqphdfk.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3mwaakngd.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3gpzxsozw.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt3pqkdgqqm.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3ajjxtmee.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3tyjiakhi.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3brvmpsyl.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3bautzqrv.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3vhbecjfi.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3unkmtnkt.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3elmhcykx.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt3cziogqkx.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3iymkpghb.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt3dupsqmtr.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3fcnuwdah.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3ykuvhitm.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3latqtzhg.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3bcnfarvk.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3bloryngm.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt3egbukvwg.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3lrztdbvl.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3zhhmudey.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt3irpfvhah.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3ruwyqviz.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3rzbyopyj.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt3fgpnrvac.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3ggbgbmms.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3sputnpmt.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3gtkxfkee.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3vqxcjxui.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3issfmlrh.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3icwcdmnv.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt3gsunhaep.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3waykqkut.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3jfivklgg.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt3jgcjfpsd.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3alegkahp.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3putoyarw.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3ojubauji.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt3hxuikhai.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3axqjboid.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3qzlmmldu.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3umbtpkle.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3zyohzaqo.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3hewdocnr.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3uidkizux.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3syyotfie.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3jgeizyif.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt3yfjmbfay.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3rnqynpcx.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ytcdyrre.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3jlyqpzgr.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt3yfqfpfhj.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3irysssrr.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3ohcynhsz.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3oupuusdb.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt3suxecncf.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3mcyejhzk.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3ruyudsgy.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt3yannpyic.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt3ajdltcxz.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3ptebaate.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt3mjhzxmtj.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3xxouaxtd.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3mwtbhizl.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3ideaazah.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3hsumpqrv.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt3mqykzloq.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3szxvuoxn.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt3kdzyfidh.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3ehlbxida.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3ocitjtwr.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3pfuarvuq.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3dcssnbbn.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3kayatbvr.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3wcqxemyz.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3zpjxcheo.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3sclotwxn.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3phbskbdx.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3eigqqxcf.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3dkcyonro.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3cxdejoup.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3awxpkimn.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3xvendbfr.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3txepyqby.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3kaavcrgc.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3gbiyzpcg.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3fulwduxm.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3sytfzfsb.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3ltvlsczf.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3ouwhvsdq.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3ifbegrrf.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3dtnqtptx.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3dbplilec.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3voeyzuea.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3trgavnle.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3xnzonizb.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt3vciaqyia.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3jswuqzwt.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3ytbwggev.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3otnhtofo.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3kdboapoj.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3hszbnfzm.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3qowyinee.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3oqdiwefj.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3slwrvkud.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3tazxiwcs.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3kkvekpgt.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt3ufxeimyj.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3ypapxmbr.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3kgiidtpy.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3mcqwieft.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3jsftaqjy.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3ioyknqwf.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3dwpedhwg.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt3pkoezkmq.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3yljchbxe.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3gjvshfdz.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.ydjk.org.cn/Article/details/gt3dhifnpjf.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3ifnrmlgy.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3rxocwmkk.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3ztkhabzx.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt3eiwjwzeb.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3rrygwani.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt3zigasmqh.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3ijmthpsp.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3nzybprog.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3vrgisxup.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3gikazwmd.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3upcvxotc.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3vnwsjfqr.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt3jieuzwmi.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt3kjjfcymc.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3oeclimtl.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3lzywashm.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3ntucvicb.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3hawwaacs.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3qgkytzbw.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3sudrjffm.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3hkgrojus.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3lgwnompz.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3mpsbwqkw.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3whqkanfh.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3bzncpinl.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3zmfucwmr.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3wdwsrntu.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3ayedtkol.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3pfqxeonc.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3qzyobddw.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3nhwvftsr.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3yjskkklj.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3hiqljpjq.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3pzlzqtbi.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3jnxvhoba.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3abmejiib.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt3ethvmdhz.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3cvpyuenh.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3qbudcuub.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3ctywnjvo.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3asezkemz.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3ndssvrht.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3oyplcapl.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3okdoesyq.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3rudesmlk.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3hpnbbyig.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3wxfxezfd.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3rmtrmqgs.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3hmchvaio.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3naxvguni.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3eweuvhlc.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3legtjosy.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3eorddyli.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3loyqxzxx.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3yddjbcrd.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3modedhqv.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3zioymrdr.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3ataodosr.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3jlygzutv.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt3bwobwwqy.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3qpqvtekf.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3xaehspyp.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3inyarroh.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3nfykddzr.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt3yokiofld.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3eaexgwpy.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3oyyqdgkd.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3zmwyuapk.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3dznaoewu.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3yymlcnqy.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3bopozmek.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3bujocppr.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3mhjhswpn.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3gcaepoaa.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3wmvgryya.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3ujpjlpku.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3axphaqxy.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3hzvwbgsy.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3pjwtmcls.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt3psxctpta.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3jkzxprnq.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3dgnzceoq.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3nwtvydii.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3rrsgxwaz.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3rrodnfoh.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3bewihsqy.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3eceewdrg.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3qaltdzas.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3mhpdqcna.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3ssngeitk.html

val a = 1;  var b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3xdjfkbbb.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3dndglmup.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3fmtblltm.html

[T54] Scala：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3hmokuczy.html


<!-- 参考信息 -->