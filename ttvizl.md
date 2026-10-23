代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt3utbojidp.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt3oqinptgh.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3tplmybpv.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt3xhkmpocp.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt3dlvckrmc.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt3lcefzxsm.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt3titpmcpw.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt3kvhcavmj.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt3zyqdmrkc.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt3yjcmwlwh.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt3gchuxplu.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt3njkvpqto.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt3ypkwqtla.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt3rfjbevok.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.ydjk.org.cn/Article/details/gt3keqpqhzz.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt3ibxgmooc.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt3wfazbjro.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt3gxatxvqk.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt3qbfjxfsd.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt3zptwjwig.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3lqmcuezy.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3badegcxf.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3jvogdgwd.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt3aszdkksu.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt3rcgsvwvq.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt3janenztu.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt3foistbos.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3xmeqhsol.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3whpfiegn.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt3vdkzdgtx.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3ldxvedjo.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3dgnhxgjn.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt3eamolyiv.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3rwumiosg.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.52xcode.cn/Article/details/gt3jauplzag.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt3yobznkoi.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt3iewmxkio.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3hpbrmivj.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt3vvcnqlgl.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3sjmnpdmj.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3vuanzkzz.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt3cjatxgzu.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt3youwktxp.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3aqhnuvga.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3pghsktuw.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3wjftofcm.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3gsyjpduy.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt3aivcpppv.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3dijcakyp.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3njssoapy.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.52xcode.cn/Article/details/gt3myellyom.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt3mzvlgoln.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt3priaqhzc.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3kzueuzkz.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3kueuejid.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3hbwsdeuq.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3mrjyvqku.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3rcwlfogx.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt3ptjffxbj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bnvssrzb.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3bagmnage.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3mndjveou.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3xymtksna.html

#include <stdio.h>
来源：http://www.52xcode.cn/Article/details/gt3wcdqzxym.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3pbpdgdau.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3ervhuqoi.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt3rthqrsjg.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt3fugjapoe.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt3jelktbxp.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt3wcbvauyj.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3fviewpca.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3pepxvlxl.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt3ckosxesz.html

[S06] C：字符串比较
来源：http://www.ydjk.org.cn/Article/details/gt3dkwulvnz.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3awotahxe.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt3ppgvduqf.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.52xcode.cn/Article/details/gt3kzvffggx.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt3ylzmacdz.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt3rcnlrmtv.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt3lvsqxcqg.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3xmcqfiqf.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3kzcataeb.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3tmbhneft.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3jqktknns.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3ejfvyudf.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3vehhadry.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3jcdgmwjq.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt3jtzhmhzb.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3wvpzfpyi.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3cwhclsph.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3hiqkxfgf.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt3wpkmfmyo.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt3twnfzjtk.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3tpblxewd.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt3ivdloysi.html

[S16] C：位操作置位
来源：http://www.ydjk.org.cn/Article/details/gt3ojilymlb.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt3afyqplas.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3tcdcztsg.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3jnkbfgsq.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt3nnstuprc.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3sudiiixj.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt3kwuymjgm.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3yuuktibc.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3wpydcfih.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3hfntmjfz.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3dimpslfe.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3yrczxceu.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt3gbwwdotl.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3ualagcje.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3cxpoilgd.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt3hsmlyliy.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt3fxirwvlm.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3wwbtnknl.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3amjybydh.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt3wiubfkqa.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3itgnwfad.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt3rchhlgjk.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3jnlmeoxr.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ipjadflv.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3rsfnmtdt.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt3scnnjmqj.html

[S29] C：变参函数
来源：http://www.ydjk.org.cn/Article/details/gt3scvynpmh.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3syrdhstu.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt3fdvsuood.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt3tvgrtfgz.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt3xxbnzyeh.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3obswhfsj.html

[S31] C++：Hello World
来源：http://www.52xcode.cn/Article/details/gt3qoedgbwo.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3kvqjzvar.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt3scjgvmpo.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt3eaujyrun.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3sxaqfxrk.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt3ogopufyv.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt3nnkxklwo.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3lstopxxd.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3zjmsyqku.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3ywhyuvbq.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3ttvjkelc.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3zkepeusg.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3okuqvcgu.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt3lqyvywcs.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.ydjk.org.cn/Article/details/gt3oovhblso.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt3qaaijuty.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3xvtjvvvh.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt3indfdagz.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt3xsewlmwk.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3imexefwr.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3pdzmojvu.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3pnrsfvtn.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3vrywoaax.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt3jxydohoj.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt3kyoqxabo.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3hzuzukfr.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt3xkzpfwue.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3jupirvyp.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt3jzofhqrt.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3bqbdmgfl.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt3fdmdcceb.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3uwmhbogh.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt3vwiybjcd.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt3jpoasdsw.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt3vgkyjpaz.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3knhpegch.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt3nttjpkwf.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3hjqajfgv.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3lnapstqu.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt3lputzvtd.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt3tmjwubvg.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3ucsbjxvn.html

[S51] C++：显式类型转换
来源：http://www.52xcode.cn/Article/details/gt3uesgszyv.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt3ipgrctof.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt3acoexhih.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt3dnroufnn.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt3cmhmhisu.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3olxibags.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3jelnecic.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt3riwgxqau.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt3rjjhpbrj.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt3cngvficx.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt3svwfwnyq.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3jlxjoybk.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt3whebceev.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt3ttbvujms.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt3xhzpuovp.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3xoyaglhv.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt3sxvkdshk.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3ffmnosmg.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3tedxxmaz.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt3tumyxjpl.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3iyjyubtr.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt3dutqlakp.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3yxzhylsv.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3sdjadibz.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt3qyfeofgx.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3nbtpjgyy.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3cnfeonzw.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3royoutrk.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3yijpbwpq.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt3oehefdxc.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt3nbsgojhw.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3yciexnpg.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3eytwhdpa.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3rhjoqefv.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3btotxxje.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3dbvqauze.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3gbqbahia.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3fkuodzzr.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3gdbqcxou.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt3nysmdgji.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3adopxoei.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt3qzpjswxu.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3fskvuuxz.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt3xsjvuzyg.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt3srdguzqt.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt3nsiuhsmn.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3nbxmvvvf.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt3npbvjisd.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt3pahthcxu.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3sgnygrog.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3wbulrpil.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt3xznkszun.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt3lqolvoza.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3xrunzuoz.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3ukmevwxd.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3dfiszvxu.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt3jmqquoow.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3uxvdnlme.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt3vhvmifjw.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt3ejjyroam.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt3mmgsishn.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3pbohvgem.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3epbyswxm.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt3suhbfaiw.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt3kscgfbeg.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt3wcfupbhu.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt3rundiwts.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt3garcxfct.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3tjqiriwf.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3utvkgfvt.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt3mqwddnsw.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3xaicqled.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt3wdusmwhe.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3aanrfket.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3ajdiydfj.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt3ggibydvo.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3fkbdpumy.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3ogbosqis.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt3jptdxjaq.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt3kfkjekzq.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt3qudhxavb.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt3pwgcjlai.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt3arpokmjh.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt3poqkexcp.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3pfbpcdee.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt3ovlwyhdx.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3taaemiwd.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt3bebgopex.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3bljvwocm.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt3datjhdnv.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.ydjk.org.cn/Article/details/gt3mpvyzxgc.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3vthdzemf.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3hxnnhoqu.html

[T36] Lua：函数
来源：http://www.ydjk.org.cn/Article/details/gt3pumknhsa.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt3opashxlw.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt3woebbfmc.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3kquiheiy.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt3oiqbccdl.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt3hokpbkot.html

[T39] Lua：模式匹配
来源：http://www.52xcode.cn/Article/details/gt3cdlppvam.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3buxopdko.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3majohsfb.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt3zcabbobx.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt3wmtvlshu.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3tmozzxbf.html

[T42] Perl：变量类型
来源：http://www.ydjk.org.cn/Article/details/gt3bdaqcnwv.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3cydaxcyq.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3diljcpcy.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt3ipvykxtx.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt3tyvvldtc.html

if ($a > 0) { print "正"; }
来源：http://www.ydjk.org.cn/Article/details/gt3eipafbyi.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt3qvnzdqrd.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3alxotjur.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3mlprmgud.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt3ntbdwjuv.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt3wqnkjsbh.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3wskgeanf.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3kkncjijx.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt3neqqwknk.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3ouvcsagf.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt3lvohbhii.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3veyemlfq.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3wkwydhqk.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3mkyzyeti.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3kckxdyvd.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3uuemnyjv.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt3wlqtodhm.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3knnoiowx.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3kksgmsbh.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3tlaskfwc.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3ggdygmvv.html


<!-- 参考信息 -->