代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：http://www.52xcode.cn/Article/details/gt2ovadajci.html

[R48] awk 取指定列
来源：http://www.52xcode.cn/Article/details/gt2zgpruskf.html

awk '{print $1, $3}' a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2boxhmrms.html

[R49] awk 带条件
来源：http://www.ydjk.org.cn/Article/details/gt2lrmdeuyl.html

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://www.ydjk.org.cn/Article/details/gt2rftbpisa.html

[R50] awk 求和
来源：http://www.52xcode.cn/Article/details/gt2tjalfxnk.html

awk '{s += $2} END {print s}' a.txt
来源：http://www.52xcode.cn/Article/details/gt2zqiwzjlj.html

[R51] 排序去重取前几
来源：http://www.ydjk.org.cn/Article/details/gt2yqjnrbfw.html

sort a.txt | uniq -c | sort -rn | head
来源：http://www.ydjk.org.cn/Article/details/gt2lmdphrul.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2zoqiwqjf.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2pijutdiw.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2akgdrohv.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2kbcdwdrk.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2jdquztyd.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2jthctgpm.html

[R55] 压缩与解压
来源：http://www.ydjk.org.cn/Article/details/gt2cicytqnc.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2mzwxttgg.html

[R56] 远程拷贝
来源：http://www.52xcode.cn/Article/details/gt2lxuanvcb.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2kvjoipsu.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2ipsglzwt.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2kvkuaziq.html

[R58] 下载文件
来源：http://www.ydjk.org.cn/Article/details/gt2wnyqzany.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2rysrjqce.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2wrqhoinl.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2intaearq.html

[R60] 只看 HTTP 状态码
来源：http://www.ydjk.org.cn/Article/details/gt2zooqguvb.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2ecyvfqcz.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2aedqskxs.html

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2lbyomaoz.html

[R62] 找最占空间的文件
来源：http://www.ydjk.org.cn/Article/details/gt2xcjytdfv.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2xxbliqmx.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt2aelkpkwf.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2lpzcyrbl.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2dibiiixi.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2zwxgtljp.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2gornctxh.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2aqqoruwk.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2hvubxtvj.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2zcwusdcf.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2xabtoltm.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2nyyausgz.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2sorupznx.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2kjsmofdq.html

[R69] 生成随机密码
来源：http://www.52xcode.cn/Article/details/gt2vtpfjicp.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2pyywhvyt.html

[R70] 时间戳与互转
来源：http://www.ydjk.org.cn/Article/details/gt2bvyqxxbb.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2uinnepti.html

[R71] 日期格式化
来源：http://www.ydjk.org.cn/Article/details/gt2myfzxqaz.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt2nsoewxgj.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2rrummhpp.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2bdpoqecg.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2dxytlvgl.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2vslvfclb.html

[R74] 批量重命名
来源：http://www.52xcode.cn/Article/details/gt2snlwyesf.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2tslesvsl.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2pcgviobw.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt2sjefrpqu.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt2rotuytbf.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2grbtrhyt.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2zuqttaex.html

read -rp "请输入: " ans
来源：http://www.ydjk.org.cn/Article/details/gt2smxmbcpf.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2viuindif.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2jmwmlilu.html

[R79] 解析命令行选项
来源：http://www.ydjk.org.cn/Article/details/gt2kuepkwcu.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2ivcvsiac.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2fzzdkwdk.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2jdhhbkgo.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2vzgdgwmu.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2jbztxaud.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2chkdrvzy.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2btllqaqu.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2clvaitno.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2avvvczph.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2nlcincof.html

int a = 10; printf("%d\n", a);
来源：http://www.ydjk.org.cn/Article/details/gt2rmqxtzba.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2vtajbjdh.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2xquzykue.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt2deehcibv.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2pbohpwrr.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2gvlbxtrj.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt2metmclgh.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2bcrityno.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2fkqethvz.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2iaffrlpe.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2tkqquqyq.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2wltbymvw.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2lwswlxfj.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2pinoxrtg.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2tfukpozl.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2izpdunne.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2abxuqcia.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2arsepcld.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt2akaftgud.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2xxpmhhgb.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2pwwxgimc.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2ekevanbf.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2yszzalag.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2jrwxoyze.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2opwjqogx.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2mejsenzn.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt2cpykhmez.html

[S15] C：类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2efdheado.html

(double) a / b
来源：http://www.52xcode.cn/Article/details/gt2ynlvlltq.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2jaalzepc.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2zagvvtnh.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2lcpimmzy.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt2hvogsnpm.html

[S18] C：命令行参数
来源：http://www.ydjk.org.cn/Article/details/gt2ugmxljtq.html

int main(int argc, char **argv)
来源：http://www.ydjk.org.cn/Article/details/gt2xsqgbwuj.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2xxeenswv.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2tqorrcrp.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2fsyevlnc.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2xwiubfly.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2kdhvplff.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2nphesrwi.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2ebrdmizv.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt2hsweqxxu.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt2tmkmbfiw.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2ncunkidd.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2tvqghxjs.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt2wlubnftv.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2tvokncud.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2irnbilzm.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2bmqhwvml.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2abzkqmpd.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2lpzckhsn.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2kjqhbudt.html

[S28] C：静态变量
来源：http://www.ydjk.org.cn/Article/details/gt2cvaooypt.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2oyismeen.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2jhddriaa.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2xfrfcusk.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2rpwrrlcu.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt2kbjngaol.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2oyrmdcka.html

#endif
来源：http://www.ydjk.org.cn/Article/details/gt2ecpvcgbp.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ibbmebxq.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2crsqiqgq.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2uegxfkic.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt2roszdsof.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2rnwjozdd.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2oukvnitf.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2opronnwe.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt2qefpurzj.html

for (auto &x : v) { std::cout << x; }
来源：http://www.52xcode.cn/Article/details/gt2fosolhee.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2bbdrthyv.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2vvpfoqvc.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2szrvhzoh.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ivzgcurn.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2acfprdod.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2oogdopfd.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2zzefsfgl.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2uogjdypj.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2bnzpgbtl.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.ydjk.org.cn/Article/details/gt2rsqhimar.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt2lnzdegmi.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2gyubmovt.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2uyfbzasn.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt2bswcaunq.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2kainiido.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2mzyubzmt.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2wtatxpei.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2yaedgufu.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2fykvrxmv.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2ixfdmwpk.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt2ognhmzdx.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2twmjtzvi.html

[S46] C++：函数模板
来源：http://www.52xcode.cn/Article/details/gt2xefhqght.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2vszjjatc.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2oejioznv.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2ybfoagfh.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2zmkpwtwv.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt2oqxxsgof.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2vuicjojh.html

[S49] C++：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2yyxcdttz.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2dvrvpmwh.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2ubgelgjv.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2caerxcri.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2vqchgikw.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2ivfpnoaz.html

[S52] C++：const 与 noexcept
来源：http://www.52xcode.cn/Article/details/gt2orzkhhjv.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2dnzjqvix.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2adrssblt.html

std::vector<int> w = std::move(v);
来源：http://www.52xcode.cn/Article/details/gt2cvvsgvmg.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2jibjlkvj.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2najluudx.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2zgvufuod.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2npkdqege.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2dmhuvhwh.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2lemwpwsm.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt2fgflcskc.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2qmwggmre.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2reaikryu.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2mmppsful.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2sqhksxua.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2gdxetvzt.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt2dvjgvzxf.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2ztkxblte.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2sffsjaxr.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2jvicvzbc.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2tsopzatl.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2kjvakazk.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2dusqvtvh.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2frdhstpo.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt2ihgcecvf.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2cyrugnjl.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2aydemoiv.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt2kjuizvzd.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt2jpcqotbh.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt2dvejjxry.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2lexixivr.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2ipdfuvos.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2ptmitaix.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2ubvawoux.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2eppqmgff.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2tbswmzyf.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2amljiixq.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2grwdgbgs.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2hjrquuzp.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2lpuldgqh.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt2wejajpvw.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2iqowuehy.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2rwslhvlq.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2upgzesoo.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2eyzzcamm.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2yurpimay.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt2dgjuuwkw.html

[T14] Kotlin：循环
来源：http://www.52xcode.cn/Article/details/gt2okaqsltz.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2rgvxcngp.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt2xaldbuzm.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2yajyotut.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2keqcklvo.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2drcwfbjj.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2glputzwb.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ucolppag.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2orytcbfp.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2aidhvssq.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2yysdxlsq.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt2sktaexwj.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2ycwnpvng.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2qfhzpekj.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2yrtscpby.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2tjgbokdh.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt2hqfdyaks.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2ikyutjqu.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2mlvvwcvv.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2rgrwlnhx.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2dyxpdsba.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2eebrulwi.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2tfceodoi.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt2llckcexv.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt2pekzvpvc.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2dfptguya.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2qhwhjgca.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2pintxhhr.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ezcuvuhi.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2gtsfdiwu.html

[T29] Swift：guard 提前返回
来源：http://www.52xcode.cn/Article/details/gt2qsvaakuw.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2jnruqwhj.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2ocruvjpg.html

protocol Shape { func area() -> Double }
来源：http://www.ydjk.org.cn/Article/details/gt2wmifcyzo.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2dyzofjpy.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2yzerixuy.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2xjuguggb.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2dueyofdw.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt2qzeaiydp.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.ydjk.org.cn/Article/details/gt2yxwjkoet.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2xgfwqtad.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2lfpajmhy.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2zkmhlckc.html

local d = { a = 1 };  d.b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ouoqijmk.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2kpiqdtxx.html

function add(a, b) return a + b end
来源：http://www.52xcode.cn/Article/details/gt2rjivacsk.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2xfxcuira.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2zcftmikl.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2cnbfjibm.html

if x > 0 then print("正") end
来源：http://www.ydjk.org.cn/Article/details/gt2utzkhkqi.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2lrovbyeu.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2zhcnlglf.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2rujjgqiw.html

setmetatable({}, { __index = base })
来源：http://www.52xcode.cn/Article/details/gt2qdfoowpa.html

[T41] Perl：Hello World
来源：http://www.52xcode.cn/Article/details/gt2sffcoycd.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt2mlcwjnhq.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2lkzuaabc.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2jhoabzmi.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2mwyofgal.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2mxvoktkh.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt2bshaiutw.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2gvpjutwf.html

[T45] Perl：数组遍历
来源：http://www.52xcode.cn/Article/details/gt2oxadgnfs.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2buvdbrch.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt2pybsiuvl.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2nkdnvfbj.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2usvzleel.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt2sbjwdnve.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt2hqhpmamr.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2nfqhnvye.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2kpzhciyi.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2spznkrsg.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2rheblojo.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.52xcode.cn/Article/details/gt2rksjcywf.html


<!-- 参考信息 -->