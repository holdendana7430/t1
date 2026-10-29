代发 wailian999

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fehbvm.com/Article/details/geuvsppwz.sHtML

[R56] 远程拷贝
来源：http://www.blog.zdbjq.cn/Article/details/ghomhurgy.sHtML

scp file user@host:/path/
来源：http://read.share.hesvh.cn/Article/details/gkczxucrm.sHtML

[R57] 远程执行命令
来源：http://3g.hesvh.cn/Article/details/gvtditadu.sHtML

ssh user@host 'uptime'
来源：http://3g.hesvh.cn/Article/details/ggjzgjabn.sHtML

[R58] 下载文件
来源：http://www.share.zdbjq.cn/Article/details/gllmhoksn.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.hesvh.cn/Article/details/gtmyjjxef.sHtML

[R59] 发 POST JSON
来源：http://mobile.hesvh.cn/Article/details/guvfmfhsg.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.hesvh.cn/Article/details/gsbpxegbq.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.hesvh.cn/Article/details/gwvzgvrwv.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.hesvh.cn/Article/details/gtmtbyizu.sHtML

[R61] 磁盘占用
来源：http://baike.zdbjq.cn/Article/details/gslnoangx.sHtML

df -h;  du -sh *
来源：http://www.share.zdbjq.cn/Article/details/gwdrfjfhf.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fehbvm.com/Article/details/gilgqihev.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.zdbjq.cn/Article/details/glxltaesi.sHtML

[R63] 内存与进程
来源：http://mobile.fehbvm.com/Article/details/gpzgxsteq.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.zdbjq.cn/Article/details/gdhloulcc.sHtML

[R64] 结束进程
来源：http://blog.zdbjq.cn/Article/details/gyquzehzs.sHtML

kill -9 $(pgrep -f app.py)
来源：http://m.share.hesvh.cn/Article/details/gvhbksjsm.sHtML

[R65] 查看端口占用
来源：http://www.share.fehbvm.com/Article/details/gzlryymcr.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.hesvh.cn/Article/details/gldepxgwt.sHtML

[R66] 定时任务
来源：http://blog.fehbvm.com/Article/details/gtnanxjan.sHtML

crontab -e;  crontab -l
来源：http://www.share.zdbjq.cn/Article/details/ghucyogyc.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.hesvh.cn/Article/details/gtqcwlfma.sHtML

openssl rand -hex 16
来源：http://www.share.zdbjq.cn/Article/details/gyehwpfwb.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.fehbvm.com/Article/details/gpexwfuof.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.hesvh.cn/Article/details/giqmbtzlu.sHtML

[R69] 生成随机密码
来源：http://m.share.zdbjq.cn/Article/details/grrptgteb.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fehbvm.com/Article/details/gioipthmy.sHtML

[R70] 时间戳与互转
来源：http://mobile.zdbjq.cn/Article/details/geejzfbhq.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fehbvm.com/Article/details/gwzdvecpx.sHtML

[R71] 日期格式化
来源：http://mobile.zdbjq.cn/Article/details/ggmuzgqok.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.share.hesvh.cn/Article/details/ggwxgpxid.sHtML

[R72] 等待端口就绪
来源：http://mobile.fehbvm.com/Article/details/gjdwwuddl.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://baike.zdbjq.cn/Article/details/gewklctiy.sHtML

[R73] 分割大日志
来源：http://www.m.share.hesvh.cn/Article/details/gisqhfkrp.sHtML

split -l 1000 big.log part_
来源：http://mobile.zdbjq.cn/Article/details/gadwaqlnv.sHtML

[R74] 批量重命名
来源：http://read.share.fehbvm.com/Article/details/gkkqzxncr.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.zdbjq.cn/Article/details/gvisyjwoe.sHtML

[R75] 导出环境变量
来源：http://m.share.fehbvm.com/Article/details/gvtigvlil.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.hesvh.cn/Article/details/gqxbumcax.sHtML

[R76] 使用临时文件
来源：http://www.blog.fehbvm.com/Article/details/gjjcpfilz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/gnjhzvght.sHtML

[R77] 读取用户输入
来源：http://read.share.zdbjq.cn/Article/details/gfttlyeiu.sHtML

read -rp "请输入: " ans
来源：http://www.share.fehbvm.com/Article/details/gmhbesklz.sHtML

[R78] 交互式菜单
来源：http://3g.hesvh.cn/Article/details/gsurvheap.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://blog.zdbjq.cn/Article/details/gxqlfjtox.sHtML

[R79] 解析命令行选项
来源：http://wap.hesvh.cn/Article/details/gdkkgwpww.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.hesvh.cn/Article/details/gvzaaenia.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.zdbjq.cn/Article/details/gcownybwe.sHtML

time ./run.sh
来源：http://baike.fehbvm.com/Article/details/gvdewuwsb.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gjvolgwzl.sHtML

S. C / C++ 专题
来源：http://www.blog.zdbjq.cn/Article/details/gioktxipc.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gyfbgtrbt.sHtML

[S01] C：Hello World
来源：http://3g.zdbjq.cn/Article/details/gfkkhiovi.sHtML

#include <stdio.h>
来源：http://baike.zdbjq.cn/Article/details/gkorgrbyf.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.zdbjq.cn/Article/details/gwywcolyt.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fehbvm.com/Article/details/gmhhqccgl.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.zdbjq.cn/Article/details/guioknfdc.sHtML

[S03] C：读入整数
来源：http://3g.fehbvm.com/Article/details/gnmgpovtx.sHtML

int x; scanf("%d", &x);
来源：http://mobile.zdbjq.cn/Article/details/gphjvaqny.sHtML

[S04] C：字符串复制
来源：http://mobile.fehbvm.com/Article/details/ggocjvwtq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.hesvh.cn/Article/details/gbzakhqqx.sHtML

[S05] C：字符串长度
来源：http://3g.hesvh.cn/Article/details/gikmeglci.sHtML

strlen(s)
来源：http://mobile.zdbjq.cn/Article/details/gkpsmekqp.sHtML

[S06] C：字符串比较
来源：http://3g.hesvh.cn/Article/details/gugdavlcj.sHtML

strcmp(a, b) == 0
来源：http://read.share.hesvh.cn/Article/details/ggtismwst.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fehbvm.com/Article/details/gpquzseqf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fehbvm.com/Article/details/gogfmxcfn.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.hesvh.cn/Article/details/gxdjtgjcl.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.zdbjq.cn/Article/details/grihqqszp.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.hesvh.cn/Article/details/gsdoazrmr.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.hesvh.cn/Article/details/gxemervud.sHtML

[S10] C：指针与解引用
来源：http://mobile.zdbjq.cn/Article/details/gsyqmrxmg.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.zdbjq.cn/Article/details/gywuupald.sHtML

[S11] C：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gpgigeeru.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.hesvh.cn/Article/details/gssieeujg.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.zdbjq.cn/Article/details/ghmawznas.sHtML

fclose(f);
来源：http://blog.hesvh.cn/Article/details/giapnzdii.sHtML

[S12] C：写文件
来源：http://m.share.fehbvm.com/Article/details/gdcirkaeo.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.hesvh.cn/Article/details/gikbozpru.sHtML

[S13] C：宏定义
来源：http://read.share.fehbvm.com/Article/details/gtzcbtaml.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.fehbvm.com/Article/details/gqswiwrxs.sHtML

[S14] C：枚举
来源：http://mobile.fehbvm.com/Article/details/gocjwhnvr.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.zdbjq.cn/Article/details/ggkltbyre.sHtML

[S15] C：类型转换
来源：http://read.share.zdbjq.cn/Article/details/gkclfkxqc.sHtML

(double) a / b
来源：http://www.m.share.fehbvm.com/Article/details/ghlmsifgh.sHtML

[S16] C：位操作置位
来源：http://www.m.share.zdbjq.cn/Article/details/grrppjitq.sHtML

x |= (1 << 3);
来源：http://blog.fehbvm.com/Article/details/gtcvlrnjo.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gzxsasezc.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.zdbjq.cn/Article/details/ghuzlltht.sHtML

[S18] C：命令行参数
来源：http://baike.hesvh.cn/Article/details/gdwdrwakj.sHtML

int main(int argc, char **argv)
来源：http://www.share.hesvh.cn/Article/details/gchnhrldb.sHtML

[S19] C：快速排序
来源：http://wap.zdbjq.cn/Article/details/gdwjvtuji.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.share.zdbjq.cn/Article/details/glesxmnft.sHtML

[S20] C：二分查找
来源：http://read.share.fehbvm.com/Article/details/gdgcmjsri.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/gjoobecag.sHtML

[S21] C：字符类别判断
来源：http://blog.fehbvm.com/Article/details/gbdbgfvpb.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wap.zdbjq.cn/Article/details/gylvgwxtz.sHtML

[S22] C：字符串转数字
来源：http://wap.fehbvm.com/Article/details/gnrtuffoi.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.zdbjq.cn/Article/details/gonnkoerm.sHtML

[S23] C：随机数
来源：http://m.share.fehbvm.com/Article/details/gngybbmqx.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.hesvh.cn/Article/details/gsdzapkwe.sHtML

[S24] C：获取本地时间
来源：http://blog.hesvh.cn/Article/details/gifeuplte.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.fehbvm.com/Article/details/gfzygutpa.sHtML

[S25] C：内存拷贝
来源：http://m.share.hesvh.cn/Article/details/gumzpvmuo.sHtML

memcpy(dst, src, n);
来源：http://3g.fehbvm.com/Article/details/gjuifjhuf.sHtML

[S26] C：内存清零
来源：http://baike.fehbvm.com/Article/details/ghxnzwscu.sHtML

memset(a, 0, sizeof a);
来源：http://blog.hesvh.cn/Article/details/gjplcggom.sHtML

[S27] C：定义常量
来源：http://3g.fehbvm.com/Article/details/gwzxdlemk.sHtML

const double PI = 3.14159;
来源：http://m.share.zdbjq.cn/Article/details/gocxwktpb.sHtML

[S28] C：静态变量
来源：http://blog.hesvh.cn/Article/details/gopfsoysi.sHtML

static int counter = 0;
来源：http://baike.hesvh.cn/Article/details/goeskrylc.sHtML

[S29] C：变参函数
来源：http://www.blog.hesvh.cn/Article/details/gvojyvyvr.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.hesvh.cn/Article/details/gwypyacqc.sHtML

[S30] C：头文件保护
来源：http://mobile.fehbvm.com/Article/details/golrwazca.sHtML

#ifndef X_H
来源：http://read.share.fehbvm.com/Article/details/gdumhapcr.sHtML

#define X_H
来源：http://baike.fehbvm.com/Article/details/gmrypnkav.sHtML

#endif
来源：http://m.share.hesvh.cn/Article/details/gzijgcltf.sHtML

[S31] C++：Hello World
来源：http://www.share.hesvh.cn/Article/details/gbsbgmjch.sHtML

#include <iostream>
来源：http://3g.fehbvm.com/Article/details/gzxsonazk.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.zdbjq.cn/Article/details/gablejykl.sHtML

[S32] C++：字符串
来源：http://read.share.hesvh.cn/Article/details/gnrcvhvuc.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fehbvm.com/Article/details/gozaebyfs.sHtML

[S33] C++：vector 增删
来源：http://www.blog.hesvh.cn/Article/details/gbzxfieso.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.zdbjq.cn/Article/details/gpxcsdvyh.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fehbvm.com/Article/details/gxwjvbzho.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fehbvm.com/Article/details/gsbhgtwjl.sHtML

[S35] C++：map
来源：http://www.m.share.fehbvm.com/Article/details/guxcuzmeb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fehbvm.com/Article/details/graunlmiq.sHtML

[S36] C++：unordered_map
来源：http://3g.hesvh.cn/Article/details/ghygagzmi.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/gpjjkkqla.sHtML

[S37] C++：set
来源：http://www.m.share.hesvh.cn/Article/details/gaxgatyek.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.hesvh.cn/Article/details/gjmfiauqd.sHtML

[S38] C++：排序
来源：http://www.blog.hesvh.cn/Article/details/gnefyewmz.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fehbvm.com/Article/details/gxfrmsqsq.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fehbvm.com/Article/details/goidjlvbc.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fehbvm.com/Article/details/ghsxscwfy.sHtML

[S40] C++：查找元素
来源：http://www.blog.hesvh.cn/Article/details/gcvgpuygi.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.zdbjq.cn/Article/details/gtduveymn.sHtML

[S41] C++：类与构造函数
来源：http://read.share.zdbjq.cn/Article/details/gisumefqt.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.fehbvm.com/Article/details/ghyrzotoh.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.zdbjq.cn/Article/details/ghonubjkr.sHtML

class B : public Base { public: void f() override {} };
来源：http://3g.fehbvm.com/Article/details/gvamfhrry.sHtML

[S43] C++：智能指针
来源：http://blog.hesvh.cn/Article/details/gbndbcezh.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fehbvm.com/Article/details/gwdzqsric.sHtML

[S44] C++：引用传参
来源：http://3g.fehbvm.com/Article/details/glakrjfze.sHtML

void inc(int &x) { ++x; }
来源：http://blog.fehbvm.com/Article/details/gzfvrpzkm.sHtML

[S45] C++：lambda
来源：http://m.share.hesvh.cn/Article/details/gwztsjrcw.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fehbvm.com/Article/details/ghvqdrmko.sHtML

[S46] C++：函数模板
来源：http://3g.fehbvm.com/Article/details/gmaroxwfq.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fehbvm.com/Article/details/gpbcnqess.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.zdbjq.cn/Article/details/gxbdzaogc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fehbvm.com/Article/details/gwpjwsgpx.sHtML

[S48] C++：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gbyhowwor.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.hesvh.cn/Article/details/gbtmwqdmp.sHtML

while (std::getline(in, line)) { }
来源：http://blog.hesvh.cn/Article/details/gwljtcjfu.sHtML

[S49] C++：写文件
来源：http://3g.hesvh.cn/Article/details/gfifpdfge.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.hesvh.cn/Article/details/gojqxvxuj.sHtML

[S50] C++：格式化数字
来源：http://www.blog.fehbvm.com/Article/details/gemhcwkqb.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.m.share.fehbvm.com/Article/details/gfzdafcvr.sHtML

[S51] C++：显式类型转换
来源：http://3g.zdbjq.cn/Article/details/gxosrtvxr.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.zdbjq.cn/Article/details/gugspmjnu.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.zdbjq.cn/Article/details/gceekxhpu.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fehbvm.com/Article/details/gukrusdfl.sHtML

[S53] C++：移动语义
来源：http://read.share.hesvh.cn/Article/details/gqtnlyhyi.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.hesvh.cn/Article/details/gzgpaovrq.sHtML

[S54] C++：异常处理
来源：http://read.share.zdbjq.cn/Article/details/gvwyiknqe.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.hesvh.cn/Article/details/gedbdfbll.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.zdbjq.cn/Article/details/gnsrwhsxj.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.hesvh.cn/Article/details/gsgjnznwk.sHtML

[S56] C++：optional
来源：http://m.share.hesvh.cn/Article/details/gzwqulnps.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.hesvh.cn/Article/details/gfvqbbedu.sHtML

[S57] C++：编译期常量
来源：http://baike.hesvh.cn/Article/details/glorwwvlg.sHtML

constexpr int N = 10;
来源：http://read.share.fehbvm.com/Article/details/gnvzzxxwf.sHtML

[S58] C++：命名空间
来源：http://blog.hesvh.cn/Article/details/gosayehaw.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.zdbjq.cn/Article/details/gbwpyotdk.sHtML

[S59] C++：静态断言
来源：http://3g.hesvh.cn/Article/details/gadaxxeot.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://m.share.zdbjq.cn/Article/details/gjghuznpf.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.hesvh.cn/Article/details/ggsdckxmi.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://m.share.zdbjq.cn/Article/details/gqornlrnx.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gjdushnnt.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.zdbjq.cn/Article/details/grhzrfjix.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/gwcdrgbxq.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gxhsdvjfp.sHtML

println("Hello")
来源：http://3g.hesvh.cn/Article/details/gllggtenn.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fehbvm.com/Article/details/gehcxlfsi.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://read.share.hesvh.cn/Article/details/gopqnpmtz.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.fehbvm.com/Article/details/ggnqdjgqb.sHtML

"值: $b"
来源：http://3g.zdbjq.cn/Article/details/gfniebfja.sHtML

[T04] Kotlin：空安全
来源：http://www.share.hesvh.cn/Article/details/grexetiez.sHtML

val n: String? = null;  n?.length
来源：http://blog.zdbjq.cn/Article/details/gffedxubu.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.hesvh.cn/Article/details/gchbmzrqs.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.fehbvm.com/Article/details/gempnwhhc.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fehbvm.com/Article/details/gpfsngnkq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.zdbjq.cn/Article/details/guhllvnuu.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.hesvh.cn/Article/details/gzlrprvkg.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.zdbjq.cn/Article/details/gygfzksgc.sHtML

[T08] Kotlin：数据类
来源：http://3g.zdbjq.cn/Article/details/gcdkkcyds.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.hesvh.cn/Article/details/goftlfypi.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.hesvh.cn/Article/details/gsktkgxnx.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fehbvm.com/Article/details/gvbmhyosm.sHtML

[T10] Kotlin：默认参数
来源：http://baike.fehbvm.com/Article/details/gypgnnrsb.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.zdbjq.cn/Article/details/gximjnizr.sHtML

[T11] Kotlin：协程
来源：http://read.share.hesvh.cn/Article/details/gmzbrqeam.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.zdbjq.cn/Article/details/gedihrohw.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.zdbjq.cn/Article/details/glhuywona.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.zdbjq.cn/Article/details/guunptexs.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.hesvh.cn/Article/details/gislazrqx.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fehbvm.com/Article/details/grtzicdyd.sHtML

[T14] Kotlin：循环
来源：http://wap.zdbjq.cn/Article/details/gureefsjx.sHtML

for (i in 1..10) println(i)
来源：http://m.share.hesvh.cn/Article/details/gvozoolfb.sHtML

[T15] Kotlin：接口
来源：http://www.blog.fehbvm.com/Article/details/gapwhdwcg.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.zdbjq.cn/Article/details/gtbmtbnbk.sHtML

[T16] Swift：Hello World
来源：http://read.share.hesvh.cn/Article/details/gufqswixc.sHtML

print("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gybypmsgv.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.hesvh.cn/Article/details/gnhjqdgdn.sHtML

var a = 1;  let b = 2
来源：http://mobile.hesvh.cn/Article/details/gmgzvdmaa.sHtML

[T18] Swift：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gggxbhoiy.sHtML

"值: \(b)"
来源：http://baike.hesvh.cn/Article/details/glntckxpt.sHtML

[T19] Swift：可选绑定
来源：http://wap.hesvh.cn/Article/details/gdpnchysi.sHtML

if let n = opt { print(n) }
来源：http://m.share.zdbjq.cn/Article/details/gplhgiwuz.sHtML

[T20] Swift：数组操作
来源：http://mobile.zdbjq.cn/Article/details/giewvxnlj.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.hesvh.cn/Article/details/gocujpxaz.sHtML

[T21] Swift：遍历
来源：http://www.m.share.fehbvm.com/Article/details/gthmkodey.sHtML

for x in a { print(x) }
来源：http://3g.zdbjq.cn/Article/details/gcixlxfan.sHtML

[T22] Swift：字典
来源：http://wap.hesvh.cn/Article/details/gfqwuittq.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.hesvh.cn/Article/details/gbtbgisyb.sHtML

[T23] Swift：函数
来源：http://wap.zdbjq.cn/Article/details/ggupqsqrf.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://baike.fehbvm.com/Article/details/graighdwo.sHtML

[T24] Swift：闭包
来源：http://blog.fehbvm.com/Article/details/gslfqzfqs.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.zdbjq.cn/Article/details/gbgofxnje.sHtML

[T25] Swift：结构体
来源：http://mobile.zdbjq.cn/Article/details/glufersqe.sHtML

struct P { var x: Int }
来源：http://www.m.share.zdbjq.cn/Article/details/gcwoudjen.sHtML

[T26] Swift：类与重写
来源：http://wap.hesvh.cn/Article/details/gvuglbdmw.sHtML

class A: Base { override func f() {} }
来源：http://read.share.fehbvm.com/Article/details/goumlpnew.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.zdbjq.cn/Article/details/geyhfqxtp.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.fehbvm.com/Article/details/gtxcanqsv.sHtML

[T28] Swift：枚举
来源：http://3g.hesvh.cn/Article/details/ghaoimzsx.sHtML

enum Color { case red, green }
来源：http://mobile.fehbvm.com/Article/details/gxlxekdnp.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.zdbjq.cn/Article/details/gobkskkqz.sHtML

guard let x = opt else { return }
来源：http://www.share.zdbjq.cn/Article/details/gndhtdszt.sHtML

[T30] Swift：协议
来源：http://www.share.hesvh.cn/Article/details/guapcyooh.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.fehbvm.com/Article/details/gewqpgbqs.sHtML

[T31] Lua：Hello World
来源：http://blog.zdbjq.cn/Article/details/grfstbugd.sHtML

print("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gxwzdtfqj.sHtML

[T32] Lua：局部变量
来源：http://blog.fehbvm.com/Article/details/gcmteyifh.sHtML

local a = 1
来源：http://read.share.fehbvm.com/Article/details/gkggzocrz.sHtML

[T33] Lua：表（数组）
来源：http://read.share.hesvh.cn/Article/details/gcqyzhlhm.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.hesvh.cn/Article/details/gyhkivpky.sHtML

[T34] Lua：遍历表
来源：http://wap.hesvh.cn/Article/details/giufmzjbd.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.hesvh.cn/Article/details/gcspomlfg.sHtML

[T35] Lua：字典表
来源：http://3g.fehbvm.com/Article/details/gytfyyrcl.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.hesvh.cn/Article/details/gzdyvrcdu.sHtML

[T36] Lua：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gacwunbnl.sHtML

function add(a, b) return a + b end
来源：http://www.share.fehbvm.com/Article/details/gugyrhoio.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.zdbjq.cn/Article/details/gkifmedxm.sHtML

"a" .. "b"
来源：http://www.m.share.zdbjq.cn/Article/details/gzqlmgvjb.sHtML

[T38] Lua：条件
来源：http://mobile.hesvh.cn/Article/details/gofogbsyp.sHtML

if x > 0 then print("正") end
来源：http://mobile.fehbvm.com/Article/details/gudtfdlsw.sHtML

[T39] Lua：模式匹配
来源：http://wap.zdbjq.cn/Article/details/gyhlzmycw.sHtML

string.find(s, "%d+")
来源：http://blog.zdbjq.cn/Article/details/gciaxxkku.sHtML

[T40] Lua：元表
来源：http://www.m.share.hesvh.cn/Article/details/goudeqkvf.sHtML

setmetatable({}, { __index = base })
来源：http://3g.hesvh.cn/Article/details/gzfguyudm.sHtML

[T41] Perl：Hello World
来源：http://m.share.fehbvm.com/Article/details/grdhbpkmq.sHtML

print "Hello\n";
来源：http://m.share.zdbjq.cn/Article/details/gnnyhhccz.sHtML

[T42] Perl：变量类型
来源：http://read.share.fehbvm.com/Article/details/gsbslzxzv.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.zdbjq.cn/Article/details/gxyuhhqwq.sHtML

[T43] Perl：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gkzounkpw.sHtML

"值: $a"
来源：http://baike.hesvh.cn/Article/details/gtnndcmvj.sHtML

[T44] Perl：条件
来源：http://www.blog.fehbvm.com/Article/details/gezzkvlsw.sHtML

if ($a > 0) { print "正"; }
来源：http://baike.zdbjq.cn/Article/details/gcdphkqsc.sHtML

[T45] Perl：数组遍历
来源：http://baike.hesvh.cn/Article/details/gbinzxmbw.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.hesvh.cn/Article/details/gfvtujsdq.sHtML

[T46] Perl：哈希操作
来源：http://www.share.zdbjq.cn/Article/details/ghoukwgup.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.fehbvm.com/Article/details/gbzkuqurf.sHtML

[T47] Perl：正则捕获
来源：http://blog.hesvh.cn/Article/details/gtthjgwlt.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.fehbvm.com/Article/details/ghuglnfxi.sHtML

[T48] Perl：正则替换
来源：http://3g.fehbvm.com/Article/details/guashsifl.sHtML

$s =~ s/old/new/g;
来源：http://m.share.hesvh.cn/Article/details/gtfvmslum.sHtML

[T49] Perl：函数
来源：http://blog.hesvh.cn/Article/details/gxmgpdxus.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.hesvh.cn/Article/details/gwuburvcu.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/giqvkkoad.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.hesvh.cn/Article/details/gqtxnvisa.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.zdbjq.cn/Article/details/ghmirgubk.sHtML

[T51] Scala：Hello World
来源：http://m.share.fehbvm.com/Article/details/gyesiwrme.sHtML

println("Hello")
来源：http://m.share.zdbjq.cn/Article/details/gtuvpjlgj.sHtML

[T52] Scala：变量
来源：http://wap.hesvh.cn/Article/details/griulhmgd.sHtML

val a = 1;  var b = 2
来源：http://3g.zdbjq.cn/Article/details/gixmuqjwe.sHtML

[T53] Scala：字符串插值
来源：http://www.share.fehbvm.com/Article/details/gbkfyqcfy.sHtML

s"值: $b"
来源：http://3g.fehbvm.com/Article/details/gvchwtbdw.sHtML

[T54] Scala：集合映射
来源：http://www.share.fehbvm.com/Article/details/gqtsnhmva.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.blog.hesvh.cn/Article/details/gawuocwwm.sHtML

[T55] Scala：集合过滤
来源：http://wap.zdbjq.cn/Article/details/gkbgehstz.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gtggbveqz.sHtML

[T56] Scala：样例类
来源：http://wap.zdbjq.cn/Article/details/gjazhuakc.sHtML

case class User(name: String, age: Int)
来源：http://3g.fehbvm.com/Article/details/ggpiuherh.sHtML

[T57] Scala：模式匹配
来源：http://mobile.hesvh.cn/Article/details/gpxielggc.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://wap.zdbjq.cn/Article/details/gpwlqbpuy.sHtML

[T58] Scala：函数定义
来源：http://baike.hesvh.cn/Article/details/gjavdzfxp.sHtML


<!-- 参考信息 -->