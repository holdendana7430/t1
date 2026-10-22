代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2fsojkair.html

[R52] 统计行数
来源：http://www.ydjk.org.cn/Article/details/gt2fgjpljsp.html

wc -l a.txt
来源：http://www.52xcode.cn/Article/details/gt2yblvppcg.html

[R53] 查看文件头与实时尾
来源：http://www.52xcode.cn/Article/details/gt2bmbbiyjz.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.52xcode.cn/Article/details/gt2woahqlta.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2yumxpstr.html

diff a.txt b.txt
来源：http://www.ydjk.org.cn/Article/details/gt2mbxgcwcb.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2knqffvzb.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2exqstmpr.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2nhargzpq.html

scp file user@host:/path/
来源：http://www.52xcode.cn/Article/details/gt2gzyfmjvy.html

[R57] 远程执行命令
来源：http://www.ydjk.org.cn/Article/details/gt2ilgazeay.html

ssh user@host 'uptime'
来源：http://www.52xcode.cn/Article/details/gt2ndakdcdu.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2gaivtojt.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2ooztaoxj.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2nuftftgl.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.52xcode.cn/Article/details/gt2bzxvliju.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2zybjnrop.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.52xcode.cn/Article/details/gt2bmipirhx.html

[R61] 磁盘占用
来源：http://www.52xcode.cn/Article/details/gt2kcxwaguf.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2ulpffapi.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2zwjfylwh.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2ntphtyhm.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2kllmgwog.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2ghaozdfh.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2sgskqbji.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2jgxmplxs.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2bksowqsp.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2nwhasfxv.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2gvedrpxa.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2mnacpxqu.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt2pjjzcoof.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2bqusmncr.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2eogdbwth.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2ggzwarpr.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2khraabcm.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2wkuulzno.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2vhwzvrlw.html

date +%s;  date -d @1700000000
来源：http://www.52xcode.cn/Article/details/gt2fykhyvea.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2idpllmnh.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2jakrmdpt.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2bevyhyyc.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2tyonxsce.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt2mcryarjy.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2lfmbpfrw.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2rxfgjhdo.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2ntwdbela.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt2jlvffvif.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2qkbcvtrk.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2pknngqdx.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2vggpsoje.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2kbvohhnf.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2sipvjkac.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2jiqxiyez.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2ztrlslkl.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2hsqzgdrn.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2ffhwcghq.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2iqtrnlwp.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2mmpoblts.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2klyxzsee.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2dsjbxyyc.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2etaexrod.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2futyzszg.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2hucrjbey.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2nwuqmblu.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2edkyujag.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2irfaobly.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt2sgwovcai.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt2ysgxchzf.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2idrvwvun.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2dawazewh.html

[S05] C：字符串长度
来源：http://www.52xcode.cn/Article/details/gt2csuunukh.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2zgeyaukc.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2zdlukyda.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2ycuvrjqt.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2gwheeoqi.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2gxsnpyqk.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2hbtutnqj.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2gqozcqwi.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2fukxcvxj.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2twkvlwat.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2plfjvtkv.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2vodapukq.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2eptjmtun.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2mcckvlrf.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.52xcode.cn/Article/details/gt2xlwptsxx.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2mjeqzvoc.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2dutndnue.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2wczfbicy.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2fblnkosi.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.ydjk.org.cn/Article/details/gt2nfithnly.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2rndyarzl.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2mempmemw.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2jdqmnhej.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2ntbejjkk.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2jcmfprpm.html

x |= (1 << 3);
来源：http://www.52xcode.cn/Article/details/gt2getazomj.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2mxioqjaw.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2yvsvxkap.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2mvpyrxos.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2xfxceutv.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2mmbbwscg.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2vyjldbcq.html

[S20] C：二分查找
来源：http://www.52xcode.cn/Article/details/gt2ngvfkqfu.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2xrcmiupx.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt2kucrnswe.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2vsipwved.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2lfbelsjr.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2bgdwzaue.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2lznqrryq.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2sdgeuumm.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2gbcgaidk.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2pvcqktnq.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2fpshctik.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2eoyagmjf.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2ibccgarf.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2kpzjoeuv.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2pvhjlkmn.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2omujeytv.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2mmylueqh.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2gpbduiaq.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2numakfcs.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt2lotohlwb.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2uzboooca.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2hapacwpf.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2mfvoxyyb.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2dphfyfrh.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2zsxfrdqv.html

#include <iostream>
来源：http://www.ydjk.org.cn/Article/details/gt2aitpbndh.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ldwljsdb.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2furtzqys.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2ushshrao.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2xhlgfjrn.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2ztwtcbaj.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2waxbnseu.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2rmcnnywx.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt2ggrbwdjq.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2jjetvytp.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2pbuemryk.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2vebsckvf.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2ljmgbymb.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2gnkzpxjc.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2utquraaw.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2jrzkdmzw.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2pybiroyn.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2jpjmtzxr.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2cnyuzpmm.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2gotmnixh.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2tsfhwnud.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2wtffmsqk.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt2dhazvuwa.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2cjvyirdg.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2htgnsdmj.html

auto p = std::make_unique<int>(5);
来源：http://www.ydjk.org.cn/Article/details/gt2gqlgzvtv.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2cfhcacuj.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2vlbjsoms.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2gfrfimsx.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2nudkcvud.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2kultizcc.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2acndcied.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2txvgljrd.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2wshkhxln.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2hecncbcy.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2rynzvtae.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt2dshloemb.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2xrkdnpud.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2lioapbxy.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2wifiqhhu.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt2ttknqtkh.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2yzwwuvbc.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2xywkgxwi.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2suddgeez.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2izuvbnty.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2zcimytve.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2iulrdifi.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt2owxvzvdu.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2aqkcjcvj.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2azhejqnn.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt2bodbatcv.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2vpiqrfzk.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2azlnrnoz.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2jcgmrggh.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2kzxhbqby.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt2kbajwnda.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2euzulmla.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2oilvlypp.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2gzgwkfxi.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2tqaqutkm.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2pkxgwjgc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2gavlyyyh.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2zkdbgghq.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2amrlayjf.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2hvgsgujz.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2xihdhlfl.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2lufftsmp.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2baevbath.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2tdqdugxn.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2bsmlujuk.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2xsqefvoy.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2zavxehjw.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2gowgaahd.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2qkjldjeq.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2bnlfblup.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2wqltawqx.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2wyagwemy.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2xcmddajs.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt2orballkn.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2iyveumol.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2dsvirkac.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2jccetqnb.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2ivpueflk.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2ytimytzg.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2dcbuqinr.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2juqubswn.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2jyosuqso.html

val (a, b) = Pair(1, 2)
来源：http://www.ydjk.org.cn/Article/details/gt2vfklrfnt.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2ksjvmohq.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2brapnito.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2aipkznto.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2cnchabur.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2jbbahhkb.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2alnzslhz.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ycjaikkr.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2zmkisgyd.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt2fvftaktv.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2jrbfbhio.html

[T18] Swift：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2sucykblm.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2sgbfdxcm.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2sbizbwjo.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2azfxouaa.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2spdhzbtl.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2hgkrdint.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2hwigzjtt.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2jaedmzfe.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2iyyvuxfn.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt2rhrwvfqg.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt2cgonzpeu.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2ekruowvm.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2ugtmrpje.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2jurdhbag.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2exdtobkl.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2cfqgfsjl.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2jvgdzmrn.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2yzpyzmwq.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt2dhkqzeba.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2fsyxzamj.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2narcypdy.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt2fndrhcun.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2pgwfhyuz.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2usxvkyju.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2ncewydzk.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2kcztttrb.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2zsiakqdq.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2alefcmhw.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2uoruzcao.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2gnhudfrc.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2nzcuxivf.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2zbzcgbmc.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2ajlczaex.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2lnrskazh.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt2cevctlul.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ulrgqxdp.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2svqcwdpv.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2ycwyrcda.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2jcvlveld.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2buhvsnsf.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt2gnvfvvjv.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2rpfzvgge.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2vpwyvaan.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2ayclkecp.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt2ibfnkirw.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2kwtjwhvu.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2cgvfvsdq.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2mhuheilw.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2mgtezluh.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2ocizeasf.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2hfcxvodl.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2iscgywuw.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2bpbjorlb.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2qmslkcfn.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2zwjkaxzf.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2ytytqzrw.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2ketnkdcv.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt2vgpcngmb.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt2xzqzcilo.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2gnxrmtdw.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2rdzruuno.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2kmzmemvv.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2xktgzpcl.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2ovzdbxun.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2xumgswfv.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2jfayggex.html

while (my $line = <$fh>) { print $line; }
来源：http://www.52xcode.cn/Article/details/gt2wqbhjpqa.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2hmzuxgbi.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2ckfbcucx.html

[T52] Scala：变量
来源：http://www.ydjk.org.cn/Article/details/gt2aruncjcd.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2wcyusmub.html

[T53] Scala：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2rphumeee.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2ocqgocyv.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2vlnbwyul.html


<!-- 参考信息 -->