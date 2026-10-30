代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://read.share.zdbjq.cn/Article/details/gnsqokmah.sHtML

[R50] awk 求和
来源：http://3g.hesvh.cn/Article/details/guwevfkzl.sHtML

awk '{s += $2} END {print s}' a.txt
来源：http://3g.zdbjq.cn/Article/details/gnuhzcogn.sHtML

[R51] 排序去重取前几
来源：http://www.share.hesvh.cn/Article/details/gtcfdmxhx.sHtML

sort a.txt | uniq -c | sort -rn | head
来源：http://3g.fehbvm.com/Article/details/gjyicutxj.sHtML

[R52] 统计行数
来源：http://www.m.share.hesvh.cn/Article/details/ghrtqafhc.sHtML

wc -l a.txt
来源：http://baike.zdbjq.cn/Article/details/gdsbbzjhg.sHtML

[R53] 查看文件头与实时尾
来源：http://3g.fehbvm.com/Article/details/gpymtiyeo.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mobile.hesvh.cn/Article/details/geyioxovv.sHtML

[R54] 比较两个文件
来源：http://m.share.fehbvm.com/Article/details/gjhzwyxfx.sHtML

diff a.txt b.txt
来源：http://blog.hesvh.cn/Article/details/gevjptgsh.sHtML

[R55] 压缩与解压
来源：http://mobile.fehbvm.com/Article/details/guzooqrfx.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.zdbjq.cn/Article/details/gvndgfcsz.sHtML

[R56] 远程拷贝
来源：http://mobile.zdbjq.cn/Article/details/ghtriowsl.sHtML

scp file user@host:/path/
来源：http://blog.zdbjq.cn/Article/details/gbhhgxgas.sHtML

[R57] 远程执行命令
来源：http://www.m.share.hesvh.cn/Article/details/gbidjuviv.sHtML

ssh user@host 'uptime'
来源：http://read.share.fehbvm.com/Article/details/godqrynpa.sHtML

[R58] 下载文件
来源：http://www.share.hesvh.cn/Article/details/ghmcassxx.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.zdbjq.cn/Article/details/glupwixre.sHtML

[R59] 发 POST JSON
来源：http://www.share.zdbjq.cn/Article/details/gdcitrjgn.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fehbvm.com/Article/details/grljpspjz.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.zdbjq.cn/Article/details/gcaaxrare.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.hesvh.cn/Article/details/gexajmskn.sHtML

[R61] 磁盘占用
来源：http://blog.zdbjq.cn/Article/details/gklsoxbak.sHtML

df -h;  du -sh *
来源：http://3g.fehbvm.com/Article/details/ghbdwjziw.sHtML

[R62] 找最占空间的文件
来源：http://baike.hesvh.cn/Article/details/gmrsxgmok.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.hesvh.cn/Article/details/gcwnwyozm.sHtML

[R63] 内存与进程
来源：http://read.share.hesvh.cn/Article/details/guplpzshe.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.zdbjq.cn/Article/details/gwbwneitt.sHtML

[R64] 结束进程
来源：http://3g.fehbvm.com/Article/details/ghtflzykj.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fehbvm.com/Article/details/gcsqxaqzd.sHtML

[R65] 查看端口占用
来源：http://read.share.hesvh.cn/Article/details/gnctaidzy.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://blog.zdbjq.cn/Article/details/gyokgbapw.sHtML

[R66] 定时任务
来源：http://read.share.fehbvm.com/Article/details/gexfymwaf.sHtML

crontab -e;  crontab -l
来源：http://www.blog.zdbjq.cn/Article/details/ggirufmhh.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fehbvm.com/Article/details/gsqwktxul.sHtML

openssl rand -hex 16
来源：http://www.m.share.fehbvm.com/Article/details/gcitvpnyu.sHtML

[R68] 计算文件校验值
来源：http://blog.fehbvm.com/Article/details/glxgvqnzo.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fehbvm.com/Article/details/gacppjspe.sHtML

[R69] 生成随机密码
来源：http://mobile.fehbvm.com/Article/details/gvlxoefow.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.zdbjq.cn/Article/details/glvbdxdty.sHtML

[R70] 时间戳与互转
来源：http://baike.zdbjq.cn/Article/details/ggsvylovt.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.hesvh.cn/Article/details/gxivpbfub.sHtML

[R71] 日期格式化
来源：http://blog.zdbjq.cn/Article/details/gsbqxntwi.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.hesvh.cn/Article/details/gbbencrex.sHtML

[R72] 等待端口就绪
来源：http://read.share.zdbjq.cn/Article/details/gtdpgoyei.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.zdbjq.cn/Article/details/gfidzamic.sHtML

[R73] 分割大日志
来源：http://m.share.hesvh.cn/Article/details/gvxucgxzp.sHtML

split -l 1000 big.log part_
来源：http://baike.zdbjq.cn/Article/details/gradwdmhj.sHtML

[R74] 批量重命名
来源：http://baike.zdbjq.cn/Article/details/gpfkstwhv.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.zdbjq.cn/Article/details/gopufjrgz.sHtML

[R75] 导出环境变量
来源：http://wap.zdbjq.cn/Article/details/guskqpkqk.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.hesvh.cn/Article/details/ggxplrvbo.sHtML

[R76] 使用临时文件
来源：http://www.m.share.fehbvm.com/Article/details/gjhwlohgu.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/gzkytowyx.sHtML

[R77] 读取用户输入
来源：http://read.share.zdbjq.cn/Article/details/gcgjqhrjj.sHtML

read -rp "请输入: " ans
来源：http://www.share.hesvh.cn/Article/details/guqlzqhpk.sHtML

[R78] 交互式菜单
来源：http://3g.fehbvm.com/Article/details/goxueyank.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.zdbjq.cn/Article/details/gxkpwoxpq.sHtML

[R79] 解析命令行选项
来源：http://read.share.hesvh.cn/Article/details/gaytujmsv.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.zdbjq.cn/Article/details/gcmehosyc.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.hesvh.cn/Article/details/gfjunsdzl.sHtML

time ./run.sh
来源：http://www.m.share.hesvh.cn/Article/details/gsxstkruf.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/grihlxteg.sHtML

S. C / C++ 专题
来源：http://www.blog.fehbvm.com/Article/details/gihtvntxc.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/gdpfsvevh.sHtML

[S01] C：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/glldkdvyu.sHtML

#include <stdio.h>
来源：http://blog.hesvh.cn/Article/details/gevmrlnyc.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://read.share.fehbvm.com/Article/details/gvsryobzh.sHtML

[S02] C：变量与格式化输出
来源：http://blog.hesvh.cn/Article/details/gltvhpyah.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.hesvh.cn/Article/details/guvkfclpu.sHtML

[S03] C：读入整数
来源：http://3g.zdbjq.cn/Article/details/gtebyxfeo.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fehbvm.com/Article/details/gwcrrgjdc.sHtML

[S04] C：字符串复制
来源：http://www.m.share.zdbjq.cn/Article/details/gsrdnnjjc.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.hesvh.cn/Article/details/gcpaodqye.sHtML

[S05] C：字符串长度
来源：http://read.share.fehbvm.com/Article/details/gonnaaneg.sHtML

strlen(s)
来源：http://blog.zdbjq.cn/Article/details/gtumnudov.sHtML

[S06] C：字符串比较
来源：http://m.share.fehbvm.com/Article/details/gomlvfpms.sHtML

strcmp(a, b) == 0
来源：http://baike.zdbjq.cn/Article/details/gcbbgcysm.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.zdbjq.cn/Article/details/gnddhptxu.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.zdbjq.cn/Article/details/gqynzrgpj.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fehbvm.com/Article/details/gmmurqebo.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.hesvh.cn/Article/details/globgnkdu.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.hesvh.cn/Article/details/gankwwaws.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.hesvh.cn/Article/details/gkskafeez.sHtML

[S10] C：指针与解引用
来源：http://blog.fehbvm.com/Article/details/gppguvken.sHtML

int *p = &a;  *p = 5;
来源：http://baike.fehbvm.com/Article/details/gstovrloj.sHtML

[S11] C：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gsrpbdypz.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.zdbjq.cn/Article/details/gcqxnqmfe.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://m.share.fehbvm.com/Article/details/gzaawersm.sHtML

fclose(f);
来源：http://mobile.fehbvm.com/Article/details/gexqyzekn.sHtML

[S12] C：写文件
来源：http://www.m.share.zdbjq.cn/Article/details/gqqnystxn.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.hesvh.cn/Article/details/gmlrgrxvo.sHtML

[S13] C：宏定义
来源：http://mobile.hesvh.cn/Article/details/gknzewnri.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://3g.hesvh.cn/Article/details/gffkzpgup.sHtML

[S14] C：枚举
来源：http://baike.hesvh.cn/Article/details/gveelgsyb.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.fehbvm.com/Article/details/gasjjzmpf.sHtML

[S15] C：类型转换
来源：http://baike.hesvh.cn/Article/details/gwgwstlmn.sHtML

(double) a / b
来源：http://read.share.hesvh.cn/Article/details/gwfnkkgys.sHtML

[S16] C：位操作置位
来源：http://mobile.zdbjq.cn/Article/details/gjgskyjmz.sHtML

x |= (1 << 3);
来源：http://wap.zdbjq.cn/Article/details/gxivdiexa.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.zdbjq.cn/Article/details/gdztfpljz.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.zdbjq.cn/Article/details/gpshdtxov.sHtML

[S18] C：命令行参数
来源：http://www.share.fehbvm.com/Article/details/gjylgkfyq.sHtML

int main(int argc, char **argv)
来源：http://www.blog.hesvh.cn/Article/details/gbefbjejj.sHtML

[S19] C：快速排序
来源：http://www.blog.fehbvm.com/Article/details/ggcbdrctx.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/gwnppvryt.sHtML

[S20] C：二分查找
来源：http://3g.zdbjq.cn/Article/details/gixikbfjp.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/gdfjexdnc.sHtML

[S21] C：字符类别判断
来源：http://m.share.fehbvm.com/Article/details/gerzigeik.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.zdbjq.cn/Article/details/gcwvrgjtg.sHtML

[S22] C：字符串转数字
来源：http://www.share.hesvh.cn/Article/details/gnvdoaxvm.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.zdbjq.cn/Article/details/gvioslayb.sHtML

[S23] C：随机数
来源：http://baike.fehbvm.com/Article/details/gkbglgqrq.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.hesvh.cn/Article/details/ghxmyyahe.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.hesvh.cn/Article/details/gqrfgpnah.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.zdbjq.cn/Article/details/glwdxrgwz.sHtML

[S25] C：内存拷贝
来源：http://www.share.fehbvm.com/Article/details/gbthksglt.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.hesvh.cn/Article/details/grfuvmyxt.sHtML

[S26] C：内存清零
来源：http://3g.zdbjq.cn/Article/details/gtihjjonp.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.zdbjq.cn/Article/details/gyfgbosae.sHtML

[S27] C：定义常量
来源：http://3g.fehbvm.com/Article/details/gzardrnpt.sHtML

const double PI = 3.14159;
来源：http://baike.zdbjq.cn/Article/details/gknirwmij.sHtML

[S28] C：静态变量
来源：http://www.blog.fehbvm.com/Article/details/gsnrrlqoo.sHtML

static int counter = 0;
来源：http://blog.fehbvm.com/Article/details/gjvzcxogq.sHtML

[S29] C：变参函数
来源：http://mobile.fehbvm.com/Article/details/gvdrbjmkg.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.hesvh.cn/Article/details/gbuczxiqm.sHtML

[S30] C：头文件保护
来源：http://baike.hesvh.cn/Article/details/gagyjtqat.sHtML

#ifndef X_H
来源：http://wap.fehbvm.com/Article/details/gttjifnyh.sHtML

#define X_H
来源：http://baike.fehbvm.com/Article/details/grrahpvyt.sHtML

#endif
来源：http://m.share.fehbvm.com/Article/details/gbxypizby.sHtML

[S31] C++：Hello World
来源：http://3g.hesvh.cn/Article/details/gmzhwngrg.sHtML

#include <iostream>
来源：http://3g.hesvh.cn/Article/details/gdwpgnxfg.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://read.share.zdbjq.cn/Article/details/grcsfycrc.sHtML

[S32] C++：字符串
来源：http://www.blog.zdbjq.cn/Article/details/gwdfpuqkf.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.hesvh.cn/Article/details/ggglxhqnt.sHtML

[S33] C++：vector 增删
来源：http://www.share.fehbvm.com/Article/details/gtipmtidj.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fehbvm.com/Article/details/gwytyyicd.sHtML

[S34] C++：遍历 vector
来源：http://wap.zdbjq.cn/Article/details/gxcdwuveu.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.zdbjq.cn/Article/details/gspiegslb.sHtML

[S35] C++：map
来源：http://3g.zdbjq.cn/Article/details/genzyydhr.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.hesvh.cn/Article/details/gruwcyjhq.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.hesvh.cn/Article/details/ggdpaxuap.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/ghhpruzff.sHtML

[S37] C++：set
来源：http://3g.hesvh.cn/Article/details/gfltxyssi.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fehbvm.com/Article/details/goefrnthk.sHtML

[S38] C++：排序
来源：http://blog.zdbjq.cn/Article/details/gqbcmhpfr.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fehbvm.com/Article/details/gsllpavoc.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fehbvm.com/Article/details/gykkeehxq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fehbvm.com/Article/details/gkjfazvto.sHtML

[S40] C++：查找元素
来源：http://read.share.zdbjq.cn/Article/details/gyeqhmgdc.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://m.share.hesvh.cn/Article/details/gsypesxie.sHtML

[S41] C++：类与构造函数
来源：http://blog.zdbjq.cn/Article/details/gzgmaxpgh.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.zdbjq.cn/Article/details/gjazknhfk.sHtML

[S42] C++：继承与虚函数
来源：http://3g.hesvh.cn/Article/details/gdfcisfkw.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.zdbjq.cn/Article/details/gdysfgvnr.sHtML

[S43] C++：智能指针
来源：http://m.share.zdbjq.cn/Article/details/gabldkpls.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.hesvh.cn/Article/details/gtdekkrht.sHtML

[S44] C++：引用传参
来源：http://baike.zdbjq.cn/Article/details/gtsfygurm.sHtML

void inc(int &x) { ++x; }
来源：http://mobile.hesvh.cn/Article/details/gdzeadgyp.sHtML

[S45] C++：lambda
来源：http://baike.fehbvm.com/Article/details/gtxssfkzo.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.fehbvm.com/Article/details/gtwkoeajh.sHtML

[S46] C++：函数模板
来源：http://baike.zdbjq.cn/Article/details/grnhotvru.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.fehbvm.com/Article/details/gqdqmhtkn.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.hesvh.cn/Article/details/gifqvdiou.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.hesvh.cn/Article/details/grjrwcoyt.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gkoqcmhvi.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.zdbjq.cn/Article/details/gcnufcmss.sHtML

while (std::getline(in, line)) { }
来源：http://blog.zdbjq.cn/Article/details/ggnoacbry.sHtML

[S49] C++：写文件
来源：http://www.m.share.hesvh.cn/Article/details/gsvcjnpsu.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fehbvm.com/Article/details/gkncbndvq.sHtML

[S50] C++：格式化数字
来源：http://baike.hesvh.cn/Article/details/gwzyvpirc.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gixtzarac.sHtML

[S51] C++：显式类型转换
来源：http://blog.fehbvm.com/Article/details/gvivntwat.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.zdbjq.cn/Article/details/gzgnsoqfk.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.zdbjq.cn/Article/details/gzuemrlkt.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.zdbjq.cn/Article/details/gwguvoaby.sHtML

[S53] C++：移动语义
来源：http://www.blog.fehbvm.com/Article/details/gyzkpyxvj.sHtML

std::vector<int> w = std::move(v);
来源：http://www.share.fehbvm.com/Article/details/gbgzdrrmu.sHtML

[S54] C++：异常处理
来源：http://m.share.hesvh.cn/Article/details/gubtbtdta.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.hesvh.cn/Article/details/gmgkgunqf.sHtML

[S55] C++：结构化绑定
来源：http://mobile.fehbvm.com/Article/details/gfmuolbnk.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://read.share.fehbvm.com/Article/details/geylgbbpc.sHtML

[S56] C++：optional
来源：http://read.share.zdbjq.cn/Article/details/gdvgjzfrz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fehbvm.com/Article/details/ggzhqqlge.sHtML

[S57] C++：编译期常量
来源：http://baike.hesvh.cn/Article/details/giwxhttsx.sHtML

constexpr int N = 10;
来源：http://mobile.hesvh.cn/Article/details/goqgxysyv.sHtML

[S58] C++：命名空间
来源：http://wap.zdbjq.cn/Article/details/ggdumaxyl.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.zdbjq.cn/Article/details/gpgdouoqe.sHtML

[S59] C++：静态断言
来源：http://blog.hesvh.cn/Article/details/gmlfwnohd.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.zdbjq.cn/Article/details/gmnljqkdb.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.hesvh.cn/Article/details/gxfhgsmca.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.zdbjq.cn/Article/details/gekrepjrg.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gqnkhxpgh.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fehbvm.com/Article/details/gwyoljgrm.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/gicbsokll.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fehbvm.com/Article/details/glvazwhtg.sHtML

println("Hello")
来源：http://mobile.zdbjq.cn/Article/details/gyvmardon.sHtML

[T02] Kotlin：变量
来源：http://mobile.hesvh.cn/Article/details/goyrxkmgo.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.zdbjq.cn/Article/details/gnqypusiy.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.fehbvm.com/Article/details/gueiyzaen.sHtML

"值: $b"
来源：http://read.share.zdbjq.cn/Article/details/guwcnagdt.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.hesvh.cn/Article/details/guakfhsjm.sHtML

val n: String? = null;  n?.length
来源：http://wap.zdbjq.cn/Article/details/gedcdmtgv.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fehbvm.com/Article/details/gmusliaav.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.hesvh.cn/Article/details/gtbtanfgs.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.hesvh.cn/Article/details/gtvqlallf.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.hesvh.cn/Article/details/gulifqhfv.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.zdbjq.cn/Article/details/gcajkxhum.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://mobile.fehbvm.com/Article/details/gmnisxzzj.sHtML

[T08] Kotlin：数据类
来源：http://mobile.zdbjq.cn/Article/details/gztgnbcfe.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.hesvh.cn/Article/details/gmujoozgn.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.hesvh.cn/Article/details/gmibkthog.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.fehbvm.com/Article/details/gmiojeuji.sHtML

[T10] Kotlin：默认参数
来源：http://3g.zdbjq.cn/Article/details/gtedecutc.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.fehbvm.com/Article/details/geyrfseuw.sHtML

[T11] Kotlin：协程
来源：http://mobile.zdbjq.cn/Article/details/guzzlqozc.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.zdbjq.cn/Article/details/gvtfkohxv.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.zdbjq.cn/Article/details/gyzccabob.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.hesvh.cn/Article/details/gsuqfmmvi.sHtML

[T13] Kotlin：只读 Map
来源：http://mobile.zdbjq.cn/Article/details/gnyyvwvzi.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.fehbvm.com/Article/details/ghekezieo.sHtML

[T14] Kotlin：循环
来源：http://read.share.fehbvm.com/Article/details/gtendexqt.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.zdbjq.cn/Article/details/ghhysmhig.sHtML

[T15] Kotlin：接口
来源：http://3g.hesvh.cn/Article/details/giswcsbwf.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.zdbjq.cn/Article/details/gzfojikzx.sHtML

[T16] Swift：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gvnrtocwz.sHtML

print("Hello")
来源：http://read.share.fehbvm.com/Article/details/gbjeacglz.sHtML

[T17] Swift：变量与常量
来源：http://3g.hesvh.cn/Article/details/glwafpxna.sHtML

var a = 1;  let b = 2
来源：http://3g.hesvh.cn/Article/details/ghkpfkdpg.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gsbmbmbqv.sHtML

"值: \(b)"
来源：http://baike.fehbvm.com/Article/details/gtallhywn.sHtML

[T19] Swift：可选绑定
来源：http://read.share.zdbjq.cn/Article/details/ggyztychf.sHtML

if let n = opt { print(n) }
来源：http://mobile.hesvh.cn/Article/details/ggldzdyvn.sHtML

[T20] Swift：数组操作
来源：http://www.blog.hesvh.cn/Article/details/givqwbovv.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.zdbjq.cn/Article/details/gvyfxqfsi.sHtML

[T21] Swift：遍历
来源：http://www.m.share.zdbjq.cn/Article/details/gmgixkjmj.sHtML

for x in a { print(x) }
来源：http://www.share.fehbvm.com/Article/details/ggvvdlpql.sHtML

[T22] Swift：字典
来源：http://www.blog.fehbvm.com/Article/details/gowgvwrkb.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.hesvh.cn/Article/details/ggwsxgmow.sHtML

[T23] Swift：函数
来源：http://read.share.fehbvm.com/Article/details/gjfvylwae.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fehbvm.com/Article/details/gkmhhrsup.sHtML

[T24] Swift：闭包
来源：http://www.blog.hesvh.cn/Article/details/gwhhzphff.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.hesvh.cn/Article/details/gxthxbhzm.sHtML

[T25] Swift：结构体
来源：http://blog.fehbvm.com/Article/details/gtmebxnrp.sHtML

struct P { var x: Int }
来源：http://www.share.fehbvm.com/Article/details/glzjgumbf.sHtML

[T26] Swift：类与重写
来源：http://baike.zdbjq.cn/Article/details/ghqvkdzor.sHtML

class A: Base { override func f() {} }
来源：http://mobile.zdbjq.cn/Article/details/gxjiczpix.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fehbvm.com/Article/details/gvavhmyzq.sHtML

do { try f() } catch { print(error) }
来源：http://wap.fehbvm.com/Article/details/gqbehoxrq.sHtML

[T28] Swift：枚举
来源：http://www.share.zdbjq.cn/Article/details/gtdgglcpd.sHtML

enum Color { case red, green }
来源：http://www.share.zdbjq.cn/Article/details/gydedwpgq.sHtML

[T29] Swift：guard 提前返回
来源：http://wap.fehbvm.com/Article/details/gcwdyawzs.sHtML

guard let x = opt else { return }
来源：http://www.share.hesvh.cn/Article/details/gczmklosg.sHtML

[T30] Swift：协议
来源：http://www.m.share.fehbvm.com/Article/details/gdwmwqcpl.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.zdbjq.cn/Article/details/gyljvdjfh.sHtML

[T31] Lua：Hello World
来源：http://3g.zdbjq.cn/Article/details/gmkorgble.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/grthmhugd.sHtML

[T32] Lua：局部变量
来源：http://wap.zdbjq.cn/Article/details/gptavzxeh.sHtML

local a = 1
来源：http://www.share.hesvh.cn/Article/details/gehpjieze.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.zdbjq.cn/Article/details/gpruatcir.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.hesvh.cn/Article/details/gpdantarj.sHtML

[T34] Lua：遍历表
来源：http://www.blog.zdbjq.cn/Article/details/gfrpyqkuh.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.hesvh.cn/Article/details/gnwashxhh.sHtML

[T35] Lua：字典表
来源：http://www.m.share.hesvh.cn/Article/details/gdvumparb.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.hesvh.cn/Article/details/ghsinoghk.sHtML

[T36] Lua：函数
来源：http://blog.zdbjq.cn/Article/details/gjisodtul.sHtML

function add(a, b) return a + b end
来源：http://wap.hesvh.cn/Article/details/gcwdojkxa.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.hesvh.cn/Article/details/gcsoqprca.sHtML

"a" .. "b"
来源：http://mobile.hesvh.cn/Article/details/gykozzhbo.sHtML

[T38] Lua：条件
来源：http://www.share.hesvh.cn/Article/details/gohhtatrw.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.fehbvm.com/Article/details/gjqmuvcfn.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.hesvh.cn/Article/details/gyqkqfxpw.sHtML

string.find(s, "%d+")
来源：http://wap.hesvh.cn/Article/details/gtnqrqicf.sHtML

[T40] Lua：元表
来源：http://blog.zdbjq.cn/Article/details/gtyxdnawc.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.zdbjq.cn/Article/details/giqsglgol.sHtML

[T41] Perl：Hello World
来源：http://wap.hesvh.cn/Article/details/ghfqwdfyg.sHtML

print "Hello\n";
来源：http://read.share.fehbvm.com/Article/details/ghjcjafam.sHtML

[T42] Perl：变量类型
来源：http://mobile.hesvh.cn/Article/details/gnebsagju.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mobile.hesvh.cn/Article/details/guvysmqsm.sHtML

[T43] Perl：字符串插值
来源：http://read.share.fehbvm.com/Article/details/ghhkrqmvz.sHtML

"值: $a"
来源：http://m.share.hesvh.cn/Article/details/gikiswpih.sHtML

[T44] Perl：条件
来源：http://www.m.share.fehbvm.com/Article/details/guwhpqkjs.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.zdbjq.cn/Article/details/grikjhdfz.sHtML

[T45] Perl：数组遍历
来源：http://www.share.fehbvm.com/Article/details/gtieujxxf.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.hesvh.cn/Article/details/giclmmopf.sHtML

[T46] Perl：哈希操作
来源：http://mobile.fehbvm.com/Article/details/giatehgqz.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.zdbjq.cn/Article/details/ggzlpbfcf.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.hesvh.cn/Article/details/gucgdrnmv.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.zdbjq.cn/Article/details/glmvfzgnw.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.fehbvm.com/Article/details/gxvmsgfrw.sHtML

$s =~ s/old/new/g;
来源：http://read.share.hesvh.cn/Article/details/gzqqaxflw.sHtML

[T49] Perl：函数
来源：http://m.share.zdbjq.cn/Article/details/gvlwrzzcq.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.zdbjq.cn/Article/details/gofibtgqf.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/ghptsggye.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.fehbvm.com/Article/details/gxkqtqbpn.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.fehbvm.com/Article/details/gxdavwkaq.sHtML

[T51] Scala：Hello World
来源：http://blog.zdbjq.cn/Article/details/gkndaimec.sHtML

println("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/ghlagnxdd.sHtML

[T52] Scala：变量
来源：http://mobile.hesvh.cn/Article/details/goeekqzer.sHtML


<!-- 参考信息 -->