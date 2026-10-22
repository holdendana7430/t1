代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://www.52xcode.cn/Article/details/gt2zjihnwbs.html

[R52] 统计行数
来源：http://www.52xcode.cn/Article/details/gt2jzrbywmy.html

wc -l a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2caeijkqg.html

[R53] 查看文件头与实时尾
来源：http://www.ydjk.org.cn/Article/details/gt2bddnptrj.html

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.ydjk.org.cn/Article/details/gt2olwzmenl.html

[R54] 比较两个文件
来源：http://www.ydjk.org.cn/Article/details/gt2vsmtyttd.html

diff a.txt b.txt
来源：http://www.52xcode.cn/Article/details/gt2huhgrwum.html

[R55] 压缩与解压
来源：http://www.52xcode.cn/Article/details/gt2wqvjxhuy.html

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.52xcode.cn/Article/details/gt2orkcrsjj.html

[R56] 远程拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2fukimhmq.html

scp file user@host:/path/
来源：http://www.ydjk.org.cn/Article/details/gt2gpgjqycr.html

[R57] 远程执行命令
来源：http://www.52xcode.cn/Article/details/gt2wcvamsyx.html

ssh user@host 'uptime'
来源：http://www.ydjk.org.cn/Article/details/gt2lbmpaxza.html

[R58] 下载文件
来源：http://www.52xcode.cn/Article/details/gt2xwlelgsj.html

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.52xcode.cn/Article/details/gt2xaikkkzq.html

[R59] 发 POST JSON
来源：http://www.ydjk.org.cn/Article/details/gt2qvywbafa.html

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.ydjk.org.cn/Article/details/gt2mrzplety.html

[R60] 只看 HTTP 状态码
来源：http://www.52xcode.cn/Article/details/gt2kgsabyxa.html

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.ydjk.org.cn/Article/details/gt2tswarawx.html

[R61] 磁盘占用
来源：http://www.ydjk.org.cn/Article/details/gt2asdkydys.html

df -h;  du -sh *
来源：http://www.52xcode.cn/Article/details/gt2hilmnfpk.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2nrjulcxz.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2hexxzdul.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2vflsbfyt.html

free -h;  ps aux | grep nginx
来源：http://www.ydjk.org.cn/Article/details/gt2snmmuuem.html

[R64] 结束进程
来源：http://www.ydjk.org.cn/Article/details/gt2maobsfnh.html

kill -9 $(pgrep -f app.py)
来源：http://www.ydjk.org.cn/Article/details/gt2uqrwohep.html

[R65] 查看端口占用
来源：http://www.ydjk.org.cn/Article/details/gt2tsyrsten.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt2osizscdt.html

[R66] 定时任务
来源：http://www.52xcode.cn/Article/details/gt2dungsloe.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2asijimcu.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2qfodpllw.html

openssl rand -hex 16
来源：http://www.52xcode.cn/Article/details/gt2cygyghqs.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2ygutxykg.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2flaxcmxs.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2stkojhrs.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt2ciebhbgf.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2ucbxkwcw.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2ercqhyhv.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2nlmwcqnj.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2synnlxmj.html

[R72] 等待端口就绪
来源：http://www.ydjk.org.cn/Article/details/gt2fytdwjkz.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt2ekzauhfw.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2ajekvtlp.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt2umihvryl.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2chwyajfe.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt2uxclwawq.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2xnlqnxhd.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2uyypeokq.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2fgbwitlr.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2zzsblycp.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt2gkcgcvgk.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2fgfnxvsa.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt2svwmvouh.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.52xcode.cn/Article/details/gt2fxutrzhi.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2egnfxbti.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt2zbgllbfb.html

[R80] 查看脚本执行耗时
来源：http://www.52xcode.cn/Article/details/gt2dcopxpgk.html

time ./run.sh
来源：http://www.ydjk.org.cn/Article/details/gt2keevmmsh.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2zgncjmjd.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt2vyyhxskk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2wanxtzvw.html

[S01] C：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2uzbaeltv.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2tmjlgwss.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt2znelkjjo.html

[S02] C：变量与格式化输出
来源：http://www.52xcode.cn/Article/details/gt2nzdqdgql.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2aztaoulu.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2rlpspwwn.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2oecusxbo.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2cxgpehpm.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.ydjk.org.cn/Article/details/gt2hglsmtwq.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2jprfwolk.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2dtdyjgch.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2flzlugsr.html

strcmp(a, b) == 0
来源：http://www.ydjk.org.cn/Article/details/gt2ymfmvvmx.html

[S07] C：数组遍历求和
来源：http://www.ydjk.org.cn/Article/details/gt2coahqspd.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2sciaacyl.html

[S08] C：动态内存分配与释放
来源：http://www.52xcode.cn/Article/details/gt2quymqgkv.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.52xcode.cn/Article/details/gt2tqmqnfon.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt2shyxzjuu.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.ydjk.org.cn/Article/details/gt2brhkbari.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2snsapyta.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt2thhgjszb.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2vlylhvsw.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2rgcbsjie.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2hmvxvsdg.html

fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2tkoyzzkg.html

[S12] C：写文件
来源：http://www.52xcode.cn/Article/details/gt2lqacnlwg.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2ujoxpvfz.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2laaejsba.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2rtftbytw.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2ivaukiem.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2krjwevpy.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2ikddztzw.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2iqkivfdl.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2lknwqbur.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2ftyadzej.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt2oagijwsb.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2lmuzropo.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2raqsiqwc.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2hpttohfw.html

[S19] C：快速排序
来源：http://www.52xcode.cn/Article/details/gt2kynxerdr.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2eagjsvts.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2yqssasdt.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2yzsanwgb.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2ioljnqcm.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt2mkqpsdvk.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt2zegmhxjt.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2hhxpocev.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2slcbvige.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.52xcode.cn/Article/details/gt2yhruhhiv.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2qlaelmiv.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2qdliqwnp.html

[S25] C：内存拷贝
来源：http://www.52xcode.cn/Article/details/gt2odcekhpd.html

memcpy(dst, src, n);
来源：http://www.52xcode.cn/Article/details/gt2vdumjzab.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt2xlncyasm.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2burgjvfk.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt2forrfozj.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2azeszrqx.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2vkexydmx.html

static int counter = 0;
来源：http://www.52xcode.cn/Article/details/gt2ikybmpru.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2axtkwamv.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2lzirpiab.html

[S30] C：头文件保护
来源：http://www.52xcode.cn/Article/details/gt2yrbhopmd.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2prkhccsj.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt2qlniaxir.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2gizepudg.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2pypatnei.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2pvbwuutc.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt2ndjcaduo.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2zebftvaj.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt2vxlocokk.html

[S33] C++：vector 增删
来源：http://www.ydjk.org.cn/Article/details/gt2ppufcktd.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt2eujqwgff.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2xdxdcwtf.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2ldbznohh.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2lozjgnkz.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2czcfitsj.html

[S36] C++：unordered_map
来源：http://www.52xcode.cn/Article/details/gt2qrvvvfiv.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.52xcode.cn/Article/details/gt2jkoxlmfs.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt2xvbbvrwg.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2ldafvaqr.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt2ulqwjjbr.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2gcemamlb.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt2gtzltixu.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2hkxcpwgf.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2kbtmlexz.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.ydjk.org.cn/Article/details/gt2gtcmidzh.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2xpsgcggz.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2ziwebkta.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2aiascchr.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt2kitgfbep.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2czxrtrfk.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2dslhivbd.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt2ewlxyfxr.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt2fykrffzq.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2ybvhljjq.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt2fgdpwdzq.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2ugoaeykl.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.52xcode.cn/Article/details/gt2lohewrsl.html

[S47] C++：结构化绑定遍历
来源：http://www.52xcode.cn/Article/details/gt2myjvizko.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.52xcode.cn/Article/details/gt2ewtnkqqm.html

[S48] C++：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2mmjmubwl.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2agosewhm.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2rjrkzehx.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2czzhupug.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt2lrjlfdob.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt2srdaitbu.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2ecopryyn.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2pangqmrv.html

static_cast<double>(a) / b
来源：http://www.ydjk.org.cn/Article/details/gt2hcfnlzvs.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2ldvsocjj.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2entvvpsg.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt2iikekgzw.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2sgnleuod.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2tarqkree.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt2ozbapcqq.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt2ttczvxin.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2kucruudf.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt2ozixbgzv.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt2dauoteus.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2unqptpwt.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt2smpecouq.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2aqyyrhej.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt2uslabogg.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2dobaxojh.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt2piuxhfbz.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2agytlmtt.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt2acdnrbzm.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2azwzktae.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.52xcode.cn/Article/details/gt2fqmwldmd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2yldnblca.html

[T01] Kotlin：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ybhjwgnx.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2nsodoodi.html

[T02] Kotlin：变量
来源：http://www.52xcode.cn/Article/details/gt2ubcxyjhu.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2qrxemadb.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2yxxfyaue.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2jhwyofyd.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2wouhirrt.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2pyyitmds.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2vczaptww.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt2lfcqcfpm.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt2phdqyxea.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt2zqzzphhj.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2yswnwowg.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2vpvtranj.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2qfngedrs.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2ijnvawmn.html

[T09] Kotlin：扩展函数
来源：http://www.52xcode.cn/Article/details/gt2dzmxteop.html

fun String.exclaim() = this + "!"
来源：http://www.52xcode.cn/Article/details/gt2wrytczye.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt2hdmmzphe.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2dzzkujfz.html

[T11] Kotlin：协程
来源：http://www.ydjk.org.cn/Article/details/gt2cunemwzd.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.ydjk.org.cn/Article/details/gt2zwdpavvi.html

[T12] Kotlin：解构声明
来源：http://www.52xcode.cn/Article/details/gt2ivhvpbjn.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2luseoabq.html

[T13] Kotlin：只读 Map
来源：http://www.ydjk.org.cn/Article/details/gt2jhsaucoc.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2cepsoxba.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2aspnfmfk.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2whbfgqsx.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2zhqipaqk.html

interface Shape { fun area(): Double }
来源：http://www.52xcode.cn/Article/details/gt2nznhcvnq.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2ojuyivak.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2ggmjajjs.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2frexhoqi.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2uoualsxm.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2trighixn.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt2exqnpzcf.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt2ixpmwtwq.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2cazsicmb.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt2sfxgvkof.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.ydjk.org.cn/Article/details/gt2ywjivkte.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt2rgsidjzv.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt2ydghuejl.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2wboxkmcy.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2nnxhrfku.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2sbzzwgra.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.ydjk.org.cn/Article/details/gt2gvnnthau.html

[T24] Swift：闭包
来源：http://www.ydjk.org.cn/Article/details/gt2ueqsmomc.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2vhwpzdwt.html

[T25] Swift：结构体
来源：http://www.52xcode.cn/Article/details/gt2zomgzymc.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2cuujuqnq.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2syfceeeh.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt2axgqdyfx.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2gzgtnmvb.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt2uaqxnbpi.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt2hiuzvydd.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2svbhhpmd.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2wghblwru.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt2zbbgxrfs.html

[T30] Swift：协议
来源：http://www.ydjk.org.cn/Article/details/gt2yxwdtvjz.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2mnruwcon.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2rqfbiqkn.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2kikipauc.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt2nihrcbpm.html

local a = 1
来源：http://www.ydjk.org.cn/Article/details/gt2lpdintmc.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2rqcitowh.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2rwakgfhc.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt2xczxmefi.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2tdfusacr.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2usvxkati.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2diqtjtyb.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2wpagezpy.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2adjgvzxx.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt2wuagcscy.html

"a" .. "b"
来源：http://www.52xcode.cn/Article/details/gt2mtuvtupl.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2qjgnrfrg.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2ozeofkjv.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2xlmywmph.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2vyboxvyl.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2qalqmydz.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2ysryiymb.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2gsyrlfsd.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2akhbaqir.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2ekstptbt.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt2jtlytpxp.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2rqknancp.html

"值: $a"
来源：http://www.ydjk.org.cn/Article/details/gt2kfixtkzt.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2hrgkxflm.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2otawvyai.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2flhorsod.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2aeujiafh.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2qoqrxtoe.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2bvejoqpp.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2hanjtuzw.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2gsqmasac.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2wiiajyzi.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt2aiwendtc.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2qcuoupmm.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.ydjk.org.cn/Article/details/gt2lobtdggh.html

[T50] Perl：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2fpbjejxi.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2pdgfkyza.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2lrwlcfvz.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt2bytmnirk.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2cuhbdcbp.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2fonprftm.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2upeibezg.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2calcoyah.html

s"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt2noqlrnqq.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2uhxdbrsf.html


<!-- 参考信息 -->