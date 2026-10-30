代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：http://wap.fehbvm.com/Article/details/grkbtlivl.sHtML

[R48] awk 取指定列
来源：http://www.share.fehbvm.com/Article/details/ggbrlorol.sHtML

awk '{print $1, $3}' a.txt
来源：http://3g.hesvh.cn/Article/details/gqlqttnvu.sHtML

[R49] awk 带条件
来源：http://blog.zdbjq.cn/Article/details/gnrgxlpid.sHtML

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://mobile.hesvh.cn/Article/details/gcmdtmxrx.sHtML

[R50] awk 求和
来源：http://www.share.fehbvm.com/Article/details/glxlandgl.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://www.blog.zdbjq.cn/Article/details/gkpjfvnme.sHtML

[R51] 排序去重取前几
来源：http://m.share.fehbvm.com/Article/details/giurcpska.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.hesvh.cn/Article/details/gkoszamdi.sHtML

[R52] 统计行数
来源：http://mobile.fehbvm.com/Article/details/gsnciejac.sHtML

wc -l a.txt
来源：http://read.share.hesvh.cn/Article/details/gcqfdlrww.sHtML

[R53] 查看文件头与实时尾
来源：http://read.share.zdbjq.cn/Article/details/gvgvnbveu.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.hesvh.cn/Article/details/ggbvxjpcg.sHtML

[R54] 比较两个文件
来源：http://wap.zdbjq.cn/Article/details/gmkzzhhqa.sHtML

diff a.txt b.txt
来源：http://m.share.fehbvm.com/Article/details/gqqtbqsxz.sHtML

[R55] 压缩与解压
来源：http://www.share.zdbjq.cn/Article/details/gkirepjdc.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.zdbjq.cn/Article/details/gmtqrugiu.sHtML

[R56] 远程拷贝
来源：http://3g.hesvh.cn/Article/details/gwjabqmhk.sHtML

scp file user@host:/path/
来源：http://www.blog.fehbvm.com/Article/details/gzherudqq.sHtML

[R57] 远程执行命令
来源：http://www.share.zdbjq.cn/Article/details/ggqfpfvzu.sHtML

ssh user@host 'uptime'
来源：http://wap.fehbvm.com/Article/details/gniwhultz.sHtML

[R58] 下载文件
来源：http://read.share.hesvh.cn/Article/details/gjwgnqtow.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.zdbjq.cn/Article/details/gmswqqzph.sHtML

[R59] 发 POST JSON
来源：http://m.share.hesvh.cn/Article/details/gityqheiq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.hesvh.cn/Article/details/gaoqqocvi.sHtML

[R60] 只看 HTTP 状态码
来源：http://m.share.hesvh.cn/Article/details/gdhokmmkl.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fehbvm.com/Article/details/gpqejpxxp.sHtML

[R61] 磁盘占用
来源：http://wap.zdbjq.cn/Article/details/gcysdrewg.sHtML

df -h;  du -sh *
来源：http://www.share.zdbjq.cn/Article/details/gtfkplcmz.sHtML

[R62] 找最占空间的文件
来源：http://www.m.share.hesvh.cn/Article/details/ghelthmzl.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.fehbvm.com/Article/details/gpcajrshr.sHtML

[R63] 内存与进程
来源：http://read.share.fehbvm.com/Article/details/gsynbutqm.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.hesvh.cn/Article/details/gjuwbgcnt.sHtML

[R64] 结束进程
来源：http://wap.fehbvm.com/Article/details/grglecata.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.hesvh.cn/Article/details/gfkneceny.sHtML

[R65] 查看端口占用
来源：http://www.blog.zdbjq.cn/Article/details/gyfymoppx.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.zdbjq.cn/Article/details/gzxrrmlif.sHtML

[R66] 定时任务
来源：http://mobile.hesvh.cn/Article/details/gorrxomyk.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.zdbjq.cn/Article/details/getllcbkh.sHtML

[R67] 生成随机十六进制串
来源：http://wap.zdbjq.cn/Article/details/gtvrxovmy.sHtML

openssl rand -hex 16
来源：http://mobile.hesvh.cn/Article/details/gchqpebbc.sHtML

[R68] 计算文件校验值
来源：http://wap.fehbvm.com/Article/details/grbhtxlzb.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.zdbjq.cn/Article/details/grauizudf.sHtML

[R69] 生成随机密码
来源：http://baike.zdbjq.cn/Article/details/grqyciagg.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.zdbjq.cn/Article/details/guctouzzx.sHtML

[R70] 时间戳与互转
来源：http://wap.hesvh.cn/Article/details/gboswdedf.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.zdbjq.cn/Article/details/gwbtfolqt.sHtML

[R71] 日期格式化
来源：http://mobile.zdbjq.cn/Article/details/gwpadkxeo.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fehbvm.com/Article/details/gvwolipnk.sHtML

[R72] 等待端口就绪
来源：http://mobile.fehbvm.com/Article/details/gwxoceujg.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.hesvh.cn/Article/details/gmbxzzlcr.sHtML

[R73] 分割大日志
来源：http://m.share.fehbvm.com/Article/details/gnciszzel.sHtML

split -l 1000 big.log part_
来源：http://read.share.hesvh.cn/Article/details/gowhmvypl.sHtML

[R74] 批量重命名
来源：http://wap.fehbvm.com/Article/details/gogknuqdl.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.zdbjq.cn/Article/details/gjlcgshlo.sHtML

[R75] 导出环境变量
来源：http://baike.fehbvm.com/Article/details/ghfsqbjud.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.zdbjq.cn/Article/details/goxbitwqg.sHtML

[R76] 使用临时文件
来源：http://mobile.hesvh.cn/Article/details/guqvwlimp.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://baike.zdbjq.cn/Article/details/gfpqrulih.sHtML

[R77] 读取用户输入
来源：http://www.share.zdbjq.cn/Article/details/gdhyclamq.sHtML

read -rp "请输入: " ans
来源：http://baike.hesvh.cn/Article/details/gjkrpfobq.sHtML

[R78] 交互式菜单
来源：http://mobile.zdbjq.cn/Article/details/gjyqebzrx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fehbvm.com/Article/details/ganzexixr.sHtML

[R79] 解析命令行选项
来源：http://read.share.hesvh.cn/Article/details/geenjyxvj.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fehbvm.com/Article/details/gaopxewbn.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.hesvh.cn/Article/details/gqrhxkrht.sHtML

time ./run.sh
来源：http://wap.hesvh.cn/Article/details/gpkhoedld.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gpobrlpza.sHtML

S. C / C++ 专题
来源：http://m.share.zdbjq.cn/Article/details/gbocerhrd.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gqkqkayxt.sHtML

[S01] C：Hello World
来源：http://baike.hesvh.cn/Article/details/gjlezxcce.sHtML

#include <stdio.h>
来源：http://blog.hesvh.cn/Article/details/ghyhzugwt.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.fehbvm.com/Article/details/ghkprljiy.sHtML

[S02] C：变量与格式化输出
来源：http://blog.zdbjq.cn/Article/details/gcwfggktl.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.zdbjq.cn/Article/details/gvxjigbqx.sHtML

[S03] C：读入整数
来源：http://www.blog.zdbjq.cn/Article/details/gkqrtkrui.sHtML

int x; scanf("%d", &x);
来源：http://3g.zdbjq.cn/Article/details/gdvyptngx.sHtML

[S04] C：字符串复制
来源：http://blog.zdbjq.cn/Article/details/gyreslqkf.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.zdbjq.cn/Article/details/gpvkhxpnf.sHtML

[S05] C：字符串长度
来源：http://read.share.hesvh.cn/Article/details/gdniyshkf.sHtML

strlen(s)
来源：http://blog.zdbjq.cn/Article/details/gkfshcpxk.sHtML

[S06] C：字符串比较
来源：http://www.m.share.zdbjq.cn/Article/details/gtxakjryj.sHtML

strcmp(a, b) == 0
来源：http://mobile.fehbvm.com/Article/details/gojcydpac.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.hesvh.cn/Article/details/gkqicybcb.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.hesvh.cn/Article/details/gshiqrubj.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fehbvm.com/Article/details/gwcvyskgm.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fehbvm.com/Article/details/gyfqhacwm.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.zdbjq.cn/Article/details/gwrwtnqlk.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.zdbjq.cn/Article/details/gdgttxdtg.sHtML

[S10] C：指针与解引用
来源：http://wap.hesvh.cn/Article/details/grcsufdzp.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.hesvh.cn/Article/details/gicmgfxws.sHtML

[S11] C：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gnzxiaudo.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fehbvm.com/Article/details/ggjrnifco.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.hesvh.cn/Article/details/glloaotxn.sHtML

fclose(f);
来源：http://www.blog.zdbjq.cn/Article/details/ghblyjfho.sHtML

[S12] C：写文件
来源：http://mobile.fehbvm.com/Article/details/gedegiozu.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.zdbjq.cn/Article/details/gtgbraken.sHtML

[S13] C：宏定义
来源：http://m.share.zdbjq.cn/Article/details/gtceptqhl.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fehbvm.com/Article/details/gcxcxwjar.sHtML

[S14] C：枚举
来源：http://3g.hesvh.cn/Article/details/gsawdespm.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.hesvh.cn/Article/details/gxaljfefa.sHtML

[S15] C：类型转换
来源：http://baike.fehbvm.com/Article/details/gufhinnop.sHtML

(double) a / b
来源：http://www.share.fehbvm.com/Article/details/gzyxkfmkt.sHtML

[S16] C：位操作置位
来源：http://read.share.zdbjq.cn/Article/details/ghvimbrik.sHtML

x |= (1 << 3);
来源：http://www.blog.hesvh.cn/Article/details/glipntvdz.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.hesvh.cn/Article/details/gjofhtyla.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.fehbvm.com/Article/details/gnksqveoe.sHtML

[S18] C：命令行参数
来源：http://m.share.fehbvm.com/Article/details/glavdqusu.sHtML

int main(int argc, char **argv)
来源：http://www.blog.zdbjq.cn/Article/details/glzaqrndk.sHtML

[S19] C：快速排序
来源：http://www.m.share.fehbvm.com/Article/details/grdnmwhkx.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/gxppxwmxs.sHtML

[S20] C：二分查找
来源：http://www.blog.hesvh.cn/Article/details/ghmblfjlp.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.zdbjq.cn/Article/details/gedanilha.sHtML

[S21] C：字符类别判断
来源：http://www.blog.zdbjq.cn/Article/details/gugjcupak.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fehbvm.com/Article/details/gcsoutfac.sHtML

[S22] C：字符串转数字
来源：http://baike.hesvh.cn/Article/details/gmwuaxfxu.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.hesvh.cn/Article/details/gsvngcpaj.sHtML

[S23] C：随机数
来源：http://baike.zdbjq.cn/Article/details/gopmowbgy.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.hesvh.cn/Article/details/gbitooezi.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.hesvh.cn/Article/details/gnbrrkste.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.hesvh.cn/Article/details/gmuqbonrb.sHtML

[S25] C：内存拷贝
来源：http://3g.fehbvm.com/Article/details/gxdjibyjl.sHtML

memcpy(dst, src, n);
来源：http://www.share.hesvh.cn/Article/details/grxewpwfw.sHtML

[S26] C：内存清零
来源：http://www.blog.hesvh.cn/Article/details/gzieeasjt.sHtML

memset(a, 0, sizeof a);
来源：http://3g.hesvh.cn/Article/details/glxdrqydh.sHtML

[S27] C：定义常量
来源：http://m.share.zdbjq.cn/Article/details/gycbfktjk.sHtML

const double PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gkkrhjjuv.sHtML

[S28] C：静态变量
来源：http://www.m.share.fehbvm.com/Article/details/gffxemscc.sHtML

static int counter = 0;
来源：http://www.m.share.zdbjq.cn/Article/details/gznnharek.sHtML

[S29] C：变参函数
来源：http://baike.hesvh.cn/Article/details/gtvhvxwck.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.hesvh.cn/Article/details/geymziajj.sHtML

[S30] C：头文件保护
来源：http://3g.fehbvm.com/Article/details/gtqxcenvg.sHtML

#ifndef X_H
来源：http://m.share.hesvh.cn/Article/details/gthuebiai.sHtML

#define X_H
来源：http://mobile.fehbvm.com/Article/details/gyszibwoe.sHtML

#endif
来源：http://www.blog.fehbvm.com/Article/details/gkhsjsrzl.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gbzgismbk.sHtML

#include <iostream>
来源：http://blog.fehbvm.com/Article/details/gtwodsdzd.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.zdbjq.cn/Article/details/ghrojazub.sHtML

[S32] C++：字符串
来源：http://wap.zdbjq.cn/Article/details/gmrxygnpj.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.zdbjq.cn/Article/details/gayprymzy.sHtML

[S33] C++：vector 增删
来源：http://3g.hesvh.cn/Article/details/gxsslezff.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.share.zdbjq.cn/Article/details/gqejvepgr.sHtML

[S34] C++：遍历 vector
来源：http://m.share.zdbjq.cn/Article/details/gzrmpsmxc.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.zdbjq.cn/Article/details/gcvaggcks.sHtML

[S35] C++：map
来源：http://m.share.hesvh.cn/Article/details/gnjguittb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.hesvh.cn/Article/details/gzvkvrpta.sHtML

[S36] C++：unordered_map
来源：http://3g.fehbvm.com/Article/details/gvmyatkfb.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gggzwqfgx.sHtML

[S37] C++：set
来源：http://baike.zdbjq.cn/Article/details/gxlqkpznh.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.hesvh.cn/Article/details/gswdykchn.sHtML

[S38] C++：排序
来源：http://read.share.zdbjq.cn/Article/details/ggbqotclq.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fehbvm.com/Article/details/gdgfneojz.sHtML

[S39] C++：自定义比较器排序
来源：http://read.share.hesvh.cn/Article/details/gxzsimvik.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.hesvh.cn/Article/details/gofmnzmne.sHtML

[S40] C++：查找元素
来源：http://m.share.fehbvm.com/Article/details/gnllthhnv.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fehbvm.com/Article/details/gvaylrzja.sHtML

[S41] C++：类与构造函数
来源：http://baike.fehbvm.com/Article/details/gtiveqntp.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.zdbjq.cn/Article/details/gemknbrvb.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.hesvh.cn/Article/details/gvfovgjtm.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.zdbjq.cn/Article/details/gfxehoyhs.sHtML

[S43] C++：智能指针
来源：http://blog.hesvh.cn/Article/details/gjojotkun.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fehbvm.com/Article/details/gdcagpown.sHtML

[S44] C++：引用传参
来源：http://blog.hesvh.cn/Article/details/gmuezmyhl.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fehbvm.com/Article/details/ghjudqmxh.sHtML

[S45] C++：lambda
来源：http://3g.zdbjq.cn/Article/details/gcpnsfhuw.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fehbvm.com/Article/details/ginahhpjs.sHtML

[S46] C++：函数模板
来源：http://www.share.zdbjq.cn/Article/details/gvzkihfpm.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fehbvm.com/Article/details/gwykoaegq.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.hesvh.cn/Article/details/gzpnfkiwm.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://3g.zdbjq.cn/Article/details/gyrixhiaw.sHtML

[S48] C++：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/ggdunstcw.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.hesvh.cn/Article/details/gtmouqxgg.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fehbvm.com/Article/details/ghonlybzk.sHtML

[S49] C++：写文件
来源：http://m.share.zdbjq.cn/Article/details/geyyljhhi.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fehbvm.com/Article/details/gufhtmwsx.sHtML

[S50] C++：格式化数字
来源：http://wap.hesvh.cn/Article/details/gobxciwts.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gkxphnwox.sHtML

[S51] C++：显式类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/gsumlnxod.sHtML

static_cast<double>(a) / b
来源：http://baike.hesvh.cn/Article/details/gpfcpcdux.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.zdbjq.cn/Article/details/ghoxbdzyr.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.hesvh.cn/Article/details/gayodjsdu.sHtML

[S53] C++：移动语义
来源：http://3g.fehbvm.com/Article/details/gvffbnili.sHtML

std::vector<int> w = std::move(v);
来源：http://3g.fehbvm.com/Article/details/ghwiqhbwi.sHtML

[S54] C++：异常处理
来源：http://www.share.fehbvm.com/Article/details/ghwfqfddl.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fehbvm.com/Article/details/gpoyevqvd.sHtML

[S55] C++：结构化绑定
来源：http://www.share.hesvh.cn/Article/details/gzxqqamtp.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.zdbjq.cn/Article/details/ghctatxhs.sHtML

[S56] C++：optional
来源：http://baike.fehbvm.com/Article/details/gdyshpfio.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fehbvm.com/Article/details/gspmnxstu.sHtML

[S57] C++：编译期常量
来源：http://read.share.hesvh.cn/Article/details/ggxniscom.sHtML

constexpr int N = 10;
来源：http://www.share.fehbvm.com/Article/details/grbejwnff.sHtML

[S58] C++：命名空间
来源：http://blog.hesvh.cn/Article/details/gwcthdxll.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fehbvm.com/Article/details/gpjwcvngt.sHtML

[S59] C++：静态断言
来源：http://www.m.share.zdbjq.cn/Article/details/gwbkfrbas.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.zdbjq.cn/Article/details/gshytntfi.sHtML

[S60] C++：遍历并删除元素
来源：http://m.share.hesvh.cn/Article/details/gpcvsuwny.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.zdbjq.cn/Article/details/gnudvrvbm.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gdomxkkry.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fehbvm.com/Article/details/gvxygoetp.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/ggaadjyvz.sHtML

[T01] Kotlin：Hello World
来源：http://m.share.hesvh.cn/Article/details/gqdpyweul.sHtML

println("Hello")
来源：http://wap.fehbvm.com/Article/details/gtgbjeklf.sHtML

[T02] Kotlin：变量
来源：http://mobile.hesvh.cn/Article/details/gtkgxoetx.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.zdbjq.cn/Article/details/gzqwyaahq.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fehbvm.com/Article/details/gqqhjanzd.sHtML

"值: $b"
来源：http://mobile.fehbvm.com/Article/details/ghplvnxxc.sHtML

[T04] Kotlin：空安全
来源：http://www.blog.hesvh.cn/Article/details/gecxykljd.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fehbvm.com/Article/details/gsyrzsqti.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.zdbjq.cn/Article/details/gehgmgjoo.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.hesvh.cn/Article/details/gkmclsdky.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.hesvh.cn/Article/details/gixstmrso.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.hesvh.cn/Article/details/gubheybnq.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.hesvh.cn/Article/details/gtjlkjexc.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.hesvh.cn/Article/details/ghhfxejgf.sHtML

[T08] Kotlin：数据类
来源：http://read.share.zdbjq.cn/Article/details/gotdowcfw.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.hesvh.cn/Article/details/gzqoquwlk.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.zdbjq.cn/Article/details/gorykgywc.sHtML

fun String.exclaim() = this + "!"
来源：http://wap.zdbjq.cn/Article/details/gimwlftcg.sHtML

[T10] Kotlin：默认参数
来源：http://3g.zdbjq.cn/Article/details/gsltefxal.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.hesvh.cn/Article/details/gkhbhvxtr.sHtML

[T11] Kotlin：协程
来源：http://m.share.fehbvm.com/Article/details/gpflsffkd.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.hesvh.cn/Article/details/gwjkuboec.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fehbvm.com/Article/details/gsmhfuedl.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/ggkjbytqk.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.fehbvm.com/Article/details/gksfqgsjf.sHtML

val m = mapOf("a" to 1)
来源：http://read.share.hesvh.cn/Article/details/gatvwyvon.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.zdbjq.cn/Article/details/gpjtivtux.sHtML

for (i in 1..10) println(i)
来源：http://m.share.zdbjq.cn/Article/details/gpwedpwcg.sHtML

[T15] Kotlin：接口
来源：http://www.blog.hesvh.cn/Article/details/gsqfwjqgn.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.hesvh.cn/Article/details/glsbciujg.sHtML

[T16] Swift：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gudnakbar.sHtML

print("Hello")
来源：http://www.blog.hesvh.cn/Article/details/glgjpuubk.sHtML

[T17] Swift：变量与常量
来源：http://blog.zdbjq.cn/Article/details/ggxjnlvdl.sHtML

var a = 1;  let b = 2
来源：http://www.share.fehbvm.com/Article/details/gtpbaznyg.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gjktoxxkb.sHtML

"值: \(b)"
来源：http://www.blog.fehbvm.com/Article/details/gzhzvbeoh.sHtML

[T19] Swift：可选绑定
来源：http://wap.hesvh.cn/Article/details/gfrjxaemt.sHtML

if let n = opt { print(n) }
来源：http://blog.zdbjq.cn/Article/details/gionyqnka.sHtML

[T20] Swift：数组操作
来源：http://read.share.hesvh.cn/Article/details/gzelrvijz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://read.share.zdbjq.cn/Article/details/gsdcasykv.sHtML

[T21] Swift：遍历
来源：http://www.m.share.hesvh.cn/Article/details/grtsubckp.sHtML

for x in a { print(x) }
来源：http://baike.fehbvm.com/Article/details/gsxxvhqbv.sHtML

[T22] Swift：字典
来源：http://blog.hesvh.cn/Article/details/gjbhhmpbl.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.hesvh.cn/Article/details/guynnecec.sHtML

[T23] Swift：函数
来源：http://wap.fehbvm.com/Article/details/gsxremcxj.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.zdbjq.cn/Article/details/gqbgxkofw.sHtML

[T24] Swift：闭包
来源：http://3g.fehbvm.com/Article/details/guukmchyw.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fehbvm.com/Article/details/gdmfpphhp.sHtML

[T25] Swift：结构体
来源：http://wap.hesvh.cn/Article/details/getiyvfxh.sHtML

struct P { var x: Int }
来源：http://www.blog.fehbvm.com/Article/details/gyrdvqiaw.sHtML

[T26] Swift：类与重写
来源：http://baike.zdbjq.cn/Article/details/gipbxtrzl.sHtML

class A: Base { override func f() {} }
来源：http://wap.zdbjq.cn/Article/details/gyvzeitmq.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fehbvm.com/Article/details/gxadbwuvm.sHtML

do { try f() } catch { print(error) }
来源：http://m.share.hesvh.cn/Article/details/gapfmjlns.sHtML

[T28] Swift：枚举
来源：http://baike.fehbvm.com/Article/details/gbwwdqrts.sHtML

enum Color { case red, green }
来源：http://wap.fehbvm.com/Article/details/gzuhwpwek.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.fehbvm.com/Article/details/grikkenas.sHtML

guard let x = opt else { return }
来源：http://wap.zdbjq.cn/Article/details/gyafoyxyf.sHtML

[T30] Swift：协议
来源：http://mobile.zdbjq.cn/Article/details/gougyodts.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.fehbvm.com/Article/details/gjbfapmvg.sHtML

[T31] Lua：Hello World
来源：http://blog.hesvh.cn/Article/details/gedqwihvt.sHtML

print("Hello")
来源：http://3g.fehbvm.com/Article/details/guwpumbdn.sHtML

[T32] Lua：局部变量
来源：http://wap.zdbjq.cn/Article/details/gntnbwwgt.sHtML

local a = 1
来源：http://baike.zdbjq.cn/Article/details/gxsdvidfq.sHtML

[T33] Lua：表（数组）
来源：http://baike.zdbjq.cn/Article/details/gdysgewvq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.fehbvm.com/Article/details/gxkqhmldv.sHtML

[T34] Lua：遍历表
来源：http://www.share.fehbvm.com/Article/details/gkxzdlezl.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.zdbjq.cn/Article/details/gowysihvz.sHtML

[T35] Lua：字典表
来源：http://www.share.hesvh.cn/Article/details/gipfkwlzt.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.hesvh.cn/Article/details/gwmeqtslp.sHtML

[T36] Lua：函数
来源：http://blog.hesvh.cn/Article/details/gevlrsbvk.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.zdbjq.cn/Article/details/gzisyeloa.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.hesvh.cn/Article/details/gmigkqvtz.sHtML

"a" .. "b"
来源：http://read.share.hesvh.cn/Article/details/gamvkljfy.sHtML

[T38] Lua：条件
来源：http://mobile.fehbvm.com/Article/details/gvexcsrnc.sHtML

if x > 0 then print("正") end
来源：http://www.share.zdbjq.cn/Article/details/gofdsljws.sHtML

[T39] Lua：模式匹配
来源：http://3g.zdbjq.cn/Article/details/gjnuuqjiw.sHtML

string.find(s, "%d+")
来源：http://www.share.hesvh.cn/Article/details/gifpedoxp.sHtML

[T40] Lua：元表
来源：http://blog.fehbvm.com/Article/details/gercblinq.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.hesvh.cn/Article/details/gjemsuwjn.sHtML

[T41] Perl：Hello World
来源：http://blog.fehbvm.com/Article/details/gcypgghid.sHtML

print "Hello\n";
来源：http://www.m.share.fehbvm.com/Article/details/gmqiqtopd.sHtML

[T42] Perl：变量类型
来源：http://blog.hesvh.cn/Article/details/gffppqtyx.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.blog.zdbjq.cn/Article/details/gnrjiznmq.sHtML

[T43] Perl：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gknzxuwae.sHtML

"值: $a"
来源：http://read.share.hesvh.cn/Article/details/gmbtfcbbz.sHtML

[T44] Perl：条件
来源：http://mobile.fehbvm.com/Article/details/gnjxoiizt.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.fehbvm.com/Article/details/gudvncodm.sHtML

[T45] Perl：数组遍历
来源：http://3g.hesvh.cn/Article/details/gvzcsyupf.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.hesvh.cn/Article/details/gjlueskzq.sHtML

[T46] Perl：哈希操作
来源：http://baike.fehbvm.com/Article/details/gcxshviiu.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.fehbvm.com/Article/details/gjinhamwv.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.hesvh.cn/Article/details/gjlhsjcxg.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.zdbjq.cn/Article/details/gyvzchbpp.sHtML

[T48] Perl：正则替换
来源：http://read.share.hesvh.cn/Article/details/gdenwpqsn.sHtML

$s =~ s/old/new/g;
来源：http://m.share.fehbvm.com/Article/details/gtjgxscwn.sHtML

[T49] Perl：函数
来源：http://3g.fehbvm.com/Article/details/gislppcmh.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.fehbvm.com/Article/details/giezwturk.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/gqmlpzcrd.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.fehbvm.com/Article/details/gkuvntzam.sHtML


<!-- 参考信息 -->