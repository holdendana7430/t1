代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.share.hesvh.cn/Article/details/gydmsdiuv.sHtML

[R54] 比较两个文件
来源：http://mobile.hesvh.cn/Article/details/grnvbiwul.sHtML

diff a.txt b.txt
来源：http://m.share.hesvh.cn/Article/details/gogvwyhkb.sHtML

[R55] 压缩与解压
来源：http://read.share.fehbvm.com/Article/details/gxqyfoiow.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://baike.zdbjq.cn/Article/details/gwosfmylk.sHtML

[R56] 远程拷贝
来源：http://www.share.zdbjq.cn/Article/details/gnlkuvidn.sHtML

scp file user@host:/path/
来源：http://www.blog.fehbvm.com/Article/details/gkfezjmpr.sHtML

[R57] 远程执行命令
来源：http://www.share.fehbvm.com/Article/details/getztmlza.sHtML

ssh user@host 'uptime'
来源：http://www.share.zdbjq.cn/Article/details/gvyffcqot.sHtML

[R58] 下载文件
来源：http://baike.zdbjq.cn/Article/details/gnyudepxt.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.hesvh.cn/Article/details/greianixl.sHtML

[R59] 发 POST JSON
来源：http://m.share.fehbvm.com/Article/details/geqlptdvq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.zdbjq.cn/Article/details/giclfikxa.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.hesvh.cn/Article/details/gfjvyfgdi.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fehbvm.com/Article/details/gmyqeblan.sHtML

[R61] 磁盘占用
来源：http://wap.hesvh.cn/Article/details/gsafjupwu.sHtML

df -h;  du -sh *
来源：http://blog.zdbjq.cn/Article/details/gyimielys.sHtML

[R62] 找最占空间的文件
来源：http://www.share.zdbjq.cn/Article/details/gwlidipam.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fehbvm.com/Article/details/ghyyrmsae.sHtML

[R63] 内存与进程
来源：http://mobile.zdbjq.cn/Article/details/giiazbbcm.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.hesvh.cn/Article/details/gcqninqdw.sHtML

[R64] 结束进程
来源：http://wap.fehbvm.com/Article/details/gvgsfcvty.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.hesvh.cn/Article/details/grtxhfdip.sHtML

[R65] 查看端口占用
来源：http://www.share.fehbvm.com/Article/details/gxyihgagb.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://3g.hesvh.cn/Article/details/gewdzwqjy.sHtML

[R66] 定时任务
来源：http://www.m.share.hesvh.cn/Article/details/ghxxionud.sHtML

crontab -e;  crontab -l
来源：http://baike.zdbjq.cn/Article/details/gfgaqsohf.sHtML

[R67] 生成随机十六进制串
来源：http://blog.hesvh.cn/Article/details/gaypwzxzy.sHtML

openssl rand -hex 16
来源：http://www.share.hesvh.cn/Article/details/gdxsspxnb.sHtML

[R68] 计算文件校验值
来源：http://m.share.zdbjq.cn/Article/details/gvfbylvhi.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://read.share.hesvh.cn/Article/details/gbwocdqnm.sHtML

[R69] 生成随机密码
来源：http://mobile.zdbjq.cn/Article/details/gzuiyvzpc.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.zdbjq.cn/Article/details/gtpnkuazd.sHtML

[R70] 时间戳与互转
来源：http://blog.zdbjq.cn/Article/details/gbzsavgze.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fehbvm.com/Article/details/gplhrtuxb.sHtML

[R71] 日期格式化
来源：http://www.share.hesvh.cn/Article/details/gxlqdtcuv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://wap.fehbvm.com/Article/details/gvsygvmtd.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fehbvm.com/Article/details/gmzhsyccw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.blog.fehbvm.com/Article/details/gbktxnzgn.sHtML

[R73] 分割大日志
来源：http://mobile.zdbjq.cn/Article/details/giuvksjhv.sHtML

split -l 1000 big.log part_
来源：http://wap.hesvh.cn/Article/details/guwcnhovu.sHtML

[R74] 批量重命名
来源：http://www.m.share.zdbjq.cn/Article/details/gmvojhfzi.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.zdbjq.cn/Article/details/gdgymkjpu.sHtML

[R75] 导出环境变量
来源：http://m.share.zdbjq.cn/Article/details/gmbuvdfyh.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.zdbjq.cn/Article/details/gbqocinhu.sHtML

[R76] 使用临时文件
来源：http://www.m.share.hesvh.cn/Article/details/gwuzffajx.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.share.fehbvm.com/Article/details/gxpzlyfhe.sHtML

[R77] 读取用户输入
来源：http://www.share.zdbjq.cn/Article/details/gxsesvwfi.sHtML

read -rp "请输入: " ans
来源：http://blog.hesvh.cn/Article/details/giknbnpxg.sHtML

[R78] 交互式菜单
来源：http://mobile.zdbjq.cn/Article/details/grlynrofx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.hesvh.cn/Article/details/geamxjnts.sHtML

[R79] 解析命令行选项
来源：http://wap.fehbvm.com/Article/details/gvraxkfuh.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.hesvh.cn/Article/details/gbzkjczai.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.hesvh.cn/Article/details/glavrtiaj.sHtML

time ./run.sh
来源：http://mobile.hesvh.cn/Article/details/gmimaoqvl.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gkfauoxgp.sHtML

S. C / C++ 专题
来源：http://blog.zdbjq.cn/Article/details/ggiccxrhm.sHtML

================================================================================
来源：http://m.share.hesvh.cn/Article/details/ghburatmc.sHtML

[S01] C：Hello World
来源：http://wap.fehbvm.com/Article/details/gzwnhzral.sHtML

#include <stdio.h>
来源：http://www.blog.fehbvm.com/Article/details/gimlninsn.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.hesvh.cn/Article/details/grcrolkix.sHtML

[S02] C：变量与格式化输出
来源：http://wap.zdbjq.cn/Article/details/gpwivraqp.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.hesvh.cn/Article/details/gviwgixcu.sHtML

[S03] C：读入整数
来源：http://blog.zdbjq.cn/Article/details/gyguisfst.sHtML

int x; scanf("%d", &x);
来源：http://blog.hesvh.cn/Article/details/gxwjqtmfz.sHtML

[S04] C：字符串复制
来源：http://wap.hesvh.cn/Article/details/gougnedoo.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fehbvm.com/Article/details/grbhybczj.sHtML

[S05] C：字符串长度
来源：http://read.share.fehbvm.com/Article/details/gmfarzjie.sHtML

strlen(s)
来源：http://3g.zdbjq.cn/Article/details/gmqqpsvgs.sHtML

[S06] C：字符串比较
来源：http://3g.hesvh.cn/Article/details/gjxqsdyhl.sHtML

strcmp(a, b) == 0
来源：http://blog.fehbvm.com/Article/details/gqdiqikdc.sHtML

[S07] C：数组遍历求和
来源：http://mobile.zdbjq.cn/Article/details/gvhvlqwyp.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.hesvh.cn/Article/details/gocongwgg.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.fehbvm.com/Article/details/gnrlekimb.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.fehbvm.com/Article/details/grzgjluaw.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fehbvm.com/Article/details/gsmrhdgys.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.zdbjq.cn/Article/details/ggenpfhkk.sHtML

[S10] C：指针与解引用
来源：http://3g.hesvh.cn/Article/details/gombwgrst.sHtML

int *p = &a;  *p = 5;
来源：http://blog.fehbvm.com/Article/details/gwhxzuupn.sHtML

[S11] C：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/ghutsvflh.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.zdbjq.cn/Article/details/gizzfesyk.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.zdbjq.cn/Article/details/ghkzcrbhi.sHtML

fclose(f);
来源：http://baike.zdbjq.cn/Article/details/gitowvvqt.sHtML

[S12] C：写文件
来源：http://blog.hesvh.cn/Article/details/gqhtmjwvb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.zdbjq.cn/Article/details/gzrezclao.sHtML

[S13] C：宏定义
来源：http://m.share.zdbjq.cn/Article/details/gvthwxbdd.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://baike.fehbvm.com/Article/details/gbedeabbx.sHtML

[S14] C：枚举
来源：http://read.share.hesvh.cn/Article/details/grfiqlqaw.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.hesvh.cn/Article/details/gseywxebs.sHtML

[S15] C：类型转换
来源：http://m.share.zdbjq.cn/Article/details/goavjwhkd.sHtML

(double) a / b
来源：http://www.share.hesvh.cn/Article/details/gobiechrd.sHtML

[S16] C：位操作置位
来源：http://baike.fehbvm.com/Article/details/gsdpdfdlv.sHtML

x |= (1 << 3);
来源：http://blog.zdbjq.cn/Article/details/gnhwlstwf.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gofkvnwgi.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.m.share.hesvh.cn/Article/details/gisuefytd.sHtML

[S18] C：命令行参数
来源：http://www.blog.zdbjq.cn/Article/details/gqikwqrba.sHtML

int main(int argc, char **argv)
来源：http://3g.fehbvm.com/Article/details/gfsavgpyt.sHtML

[S19] C：快速排序
来源：http://www.blog.hesvh.cn/Article/details/gfaeofzlr.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.fehbvm.com/Article/details/gfovszkty.sHtML

[S20] C：二分查找
来源：http://blog.hesvh.cn/Article/details/gzuszroyr.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.zdbjq.cn/Article/details/gwfepjptg.sHtML

[S21] C：字符类别判断
来源：http://m.share.zdbjq.cn/Article/details/gqiljvjcp.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.zdbjq.cn/Article/details/gwtwdaflh.sHtML

[S22] C：字符串转数字
来源：http://mobile.fehbvm.com/Article/details/gokmbbxhn.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.hesvh.cn/Article/details/gyrdoloob.sHtML

[S23] C：随机数
来源：http://baike.zdbjq.cn/Article/details/goatblxlg.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.zdbjq.cn/Article/details/gqqunrdpg.sHtML

[S24] C：获取本地时间
来源：http://wap.fehbvm.com/Article/details/gbcpnkjeh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://read.share.fehbvm.com/Article/details/gwwumkrrq.sHtML

[S25] C：内存拷贝
来源：http://www.share.fehbvm.com/Article/details/ghfbhgyxl.sHtML

memcpy(dst, src, n);
来源：http://m.share.fehbvm.com/Article/details/gpdebtjdh.sHtML

[S26] C：内存清零
来源：http://wap.hesvh.cn/Article/details/gxvkquiet.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.fehbvm.com/Article/details/gkgktrfxy.sHtML

[S27] C：定义常量
来源：http://3g.zdbjq.cn/Article/details/gbetddqcz.sHtML

const double PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gaqdwgmej.sHtML

[S28] C：静态变量
来源：http://mobile.zdbjq.cn/Article/details/gxoqtocpy.sHtML

static int counter = 0;
来源：http://mobile.fehbvm.com/Article/details/ghxahieuh.sHtML

[S29] C：变参函数
来源：http://blog.fehbvm.com/Article/details/gzmblooyp.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.hesvh.cn/Article/details/ggocewffh.sHtML

[S30] C：头文件保护
来源：http://3g.hesvh.cn/Article/details/gmcuvnocn.sHtML

#ifndef X_H
来源：http://read.share.fehbvm.com/Article/details/getpshxrl.sHtML

#define X_H
来源：http://www.blog.hesvh.cn/Article/details/gxfyiyahh.sHtML

#endif
来源：http://baike.fehbvm.com/Article/details/gopyntupi.sHtML

[S31] C++：Hello World
来源：http://3g.fehbvm.com/Article/details/gusbyamdc.sHtML

#include <iostream>
来源：http://3g.zdbjq.cn/Article/details/gwjsahjcc.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.zdbjq.cn/Article/details/gejzpmzls.sHtML

[S32] C++：字符串
来源：http://blog.hesvh.cn/Article/details/griemcbto.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fehbvm.com/Article/details/gchhiibsw.sHtML

[S33] C++：vector 增删
来源：http://blog.zdbjq.cn/Article/details/gpsxycdgk.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.zdbjq.cn/Article/details/gpvlpxhke.sHtML

[S34] C++：遍历 vector
来源：http://m.share.hesvh.cn/Article/details/gefeykitq.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.hesvh.cn/Article/details/gpzglmjys.sHtML

[S35] C++：map
来源：http://3g.fehbvm.com/Article/details/gcqepoycd.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fehbvm.com/Article/details/gbmosanej.sHtML

[S36] C++：unordered_map
来源：http://wap.fehbvm.com/Article/details/giyjwtvwr.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.hesvh.cn/Article/details/gznbbgbwx.sHtML

[S37] C++：set
来源：http://blog.hesvh.cn/Article/details/ganpqsthk.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.hesvh.cn/Article/details/gsjxnhtkf.sHtML

[S38] C++：排序
来源：http://baike.zdbjq.cn/Article/details/gqswxtrha.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.zdbjq.cn/Article/details/gyriqhrwi.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fehbvm.com/Article/details/gpghqdcqg.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.zdbjq.cn/Article/details/gwblkgeym.sHtML

[S40] C++：查找元素
来源：http://mobile.fehbvm.com/Article/details/gmcribnzz.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://blog.fehbvm.com/Article/details/gazzxnhgu.sHtML

[S41] C++：类与构造函数
来源：http://3g.zdbjq.cn/Article/details/gxqfulfcj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wap.fehbvm.com/Article/details/gbwdqkiou.sHtML

[S42] C++：继承与虚函数
来源：http://wap.zdbjq.cn/Article/details/grccbckov.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.zdbjq.cn/Article/details/ghivvpotv.sHtML

[S43] C++：智能指针
来源：http://baike.fehbvm.com/Article/details/gsdludkdp.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.share.zdbjq.cn/Article/details/gaqbdvarl.sHtML

[S44] C++：引用传参
来源：http://blog.zdbjq.cn/Article/details/gmbvskqyd.sHtML

void inc(int &x) { ++x; }
来源：http://baike.hesvh.cn/Article/details/ghtcfdani.sHtML

[S45] C++：lambda
来源：http://www.blog.hesvh.cn/Article/details/gvdsnzdis.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.zdbjq.cn/Article/details/gjcirvfhr.sHtML

[S46] C++：函数模板
来源：http://blog.zdbjq.cn/Article/details/gevlzmexn.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.hesvh.cn/Article/details/gishsuelp.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.hesvh.cn/Article/details/gjprhocsv.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.hesvh.cn/Article/details/geeuzynbi.sHtML

[S48] C++：逐行读文件
来源：http://3g.zdbjq.cn/Article/details/gzqfrzgwd.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.zdbjq.cn/Article/details/gaswbuvul.sHtML

while (std::getline(in, line)) { }
来源：http://wap.zdbjq.cn/Article/details/gkhqmgnsb.sHtML

[S49] C++：写文件
来源：http://m.share.hesvh.cn/Article/details/gownifwmo.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.hesvh.cn/Article/details/gcsyzrnrx.sHtML

[S50] C++：格式化数字
来源：http://m.share.hesvh.cn/Article/details/gkxsnwamr.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gtravlumu.sHtML

[S51] C++：显式类型转换
来源：http://3g.zdbjq.cn/Article/details/gobbwbucp.sHtML

static_cast<double>(a) / b
来源：http://baike.hesvh.cn/Article/details/gvzdywkyh.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fehbvm.com/Article/details/grxyurqme.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fehbvm.com/Article/details/gfdorbzhg.sHtML

[S53] C++：移动语义
来源：http://read.share.zdbjq.cn/Article/details/gyvcqdcor.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.hesvh.cn/Article/details/gmwcspkek.sHtML

[S54] C++：异常处理
来源：http://baike.hesvh.cn/Article/details/gakhypzau.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fehbvm.com/Article/details/ghkicaneq.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.zdbjq.cn/Article/details/gbzocilqe.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.zdbjq.cn/Article/details/gvmedjwdm.sHtML

[S56] C++：optional
来源：http://www.m.share.fehbvm.com/Article/details/gnzzvdxav.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.hesvh.cn/Article/details/gzstfwjsd.sHtML

[S57] C++：编译期常量
来源：http://mobile.fehbvm.com/Article/details/gaufbxcxx.sHtML

constexpr int N = 10;
来源：http://www.blog.hesvh.cn/Article/details/gvaieumov.sHtML

[S58] C++：命名空间
来源：http://mobile.zdbjq.cn/Article/details/gcnqwcduy.sHtML

namespace ns { int f() { return 1; } }
来源：http://blog.fehbvm.com/Article/details/gxoreohzl.sHtML

[S59] C++：静态断言
来源：http://m.share.fehbvm.com/Article/details/ghcxcrejd.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.zdbjq.cn/Article/details/gjvlycffw.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.hesvh.cn/Article/details/gnakqvndz.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.zdbjq.cn/Article/details/gkexdcgxb.sHtML

================================================================================
来源：http://mobile.hesvh.cn/Article/details/gvtxjhzxz.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wap.fehbvm.com/Article/details/gxvcsrncl.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gjjsbqaru.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fehbvm.com/Article/details/gihjsbfjy.sHtML

println("Hello")
来源：http://mobile.fehbvm.com/Article/details/gimenuvvm.sHtML

[T02] Kotlin：变量
来源：http://www.share.hesvh.cn/Article/details/gfnystyfs.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fehbvm.com/Article/details/gfxudvssy.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.hesvh.cn/Article/details/gzgzzlzrh.sHtML

"值: $b"
来源：http://wap.zdbjq.cn/Article/details/gvqzpzspv.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fehbvm.com/Article/details/gwjehyuqm.sHtML

val n: String? = null;  n?.length
来源：http://mobile.hesvh.cn/Article/details/gvwspiove.sHtML

[T05] Kotlin：when 表达式
来源：http://3g.hesvh.cn/Article/details/gntwafnbx.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.hesvh.cn/Article/details/gmsfxfayo.sHtML

[T06] Kotlin：集合映射
来源：http://3g.zdbjq.cn/Article/details/gnwezigfv.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://baike.fehbvm.com/Article/details/ghetuxofo.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.zdbjq.cn/Article/details/ghoucbuzp.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.hesvh.cn/Article/details/grloclrqu.sHtML

[T08] Kotlin：数据类
来源：http://m.share.hesvh.cn/Article/details/gjxcetrkd.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.hesvh.cn/Article/details/grpdhwufk.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.hesvh.cn/Article/details/gmdhdrkil.sHtML

fun String.exclaim() = this + "!"
来源：http://read.share.fehbvm.com/Article/details/gqqgmdfxk.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.zdbjq.cn/Article/details/gjausiuis.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://baike.hesvh.cn/Article/details/geqyprejl.sHtML

[T11] Kotlin：协程
来源：http://baike.hesvh.cn/Article/details/glttozpba.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.zdbjq.cn/Article/details/gpcqyugij.sHtML

[T12] Kotlin：解构声明
来源：http://blog.hesvh.cn/Article/details/gscxqagyr.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.hesvh.cn/Article/details/gcmhicqfa.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.zdbjq.cn/Article/details/gogshhsqm.sHtML

val m = mapOf("a" to 1)
来源：http://blog.fehbvm.com/Article/details/gvsxuqooi.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fehbvm.com/Article/details/gvoacqiyv.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fehbvm.com/Article/details/gpwlzjene.sHtML

[T15] Kotlin：接口
来源：http://m.share.zdbjq.cn/Article/details/gxjkiglsr.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.zdbjq.cn/Article/details/gnsmavpyg.sHtML

[T16] Swift：Hello World
来源：http://blog.fehbvm.com/Article/details/gpdroeanh.sHtML

print("Hello")
来源：http://wap.zdbjq.cn/Article/details/gliggnuxf.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fehbvm.com/Article/details/gxqozhtsy.sHtML

var a = 1;  let b = 2
来源：http://m.share.fehbvm.com/Article/details/gnutzqbxb.sHtML

[T18] Swift：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gjttfmytk.sHtML

"值: \(b)"
来源：http://read.share.hesvh.cn/Article/details/gmwcnulyl.sHtML

[T19] Swift：可选绑定
来源：http://www.share.fehbvm.com/Article/details/gqkolrqfz.sHtML

if let n = opt { print(n) }
来源：http://mobile.hesvh.cn/Article/details/gbjbbjpye.sHtML

[T20] Swift：数组操作
来源：http://3g.hesvh.cn/Article/details/gnudqqtpo.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.hesvh.cn/Article/details/gzxkmqsco.sHtML

[T21] Swift：遍历
来源：http://www.m.share.hesvh.cn/Article/details/ggdmqmrhx.sHtML

for x in a { print(x) }
来源：http://3g.hesvh.cn/Article/details/gbtblldbp.sHtML

[T22] Swift：字典
来源：http://www.share.zdbjq.cn/Article/details/gcihdwork.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.zdbjq.cn/Article/details/gijdrhnix.sHtML

[T23] Swift：函数
来源：http://blog.fehbvm.com/Article/details/gdncgxrbi.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.hesvh.cn/Article/details/gbbdkvsze.sHtML

[T24] Swift：闭包
来源：http://m.share.zdbjq.cn/Article/details/grzpmzxzy.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fehbvm.com/Article/details/gjhmupxrs.sHtML

[T25] Swift：结构体
来源：http://www.blog.hesvh.cn/Article/details/gneorzcfp.sHtML

struct P { var x: Int }
来源：http://m.share.fehbvm.com/Article/details/gmrsrewmw.sHtML

[T26] Swift：类与重写
来源：http://baike.fehbvm.com/Article/details/gavxuirgc.sHtML

class A: Base { override func f() {} }
来源：http://wap.hesvh.cn/Article/details/gpzjwrtme.sHtML

[T27] Swift：错误处理
来源：http://baike.zdbjq.cn/Article/details/grvhxucve.sHtML

do { try f() } catch { print(error) }
来源：http://blog.fehbvm.com/Article/details/golczqvpt.sHtML

[T28] Swift：枚举
来源：http://www.share.zdbjq.cn/Article/details/gkwttwcrs.sHtML

enum Color { case red, green }
来源：http://blog.hesvh.cn/Article/details/ghtsspycy.sHtML

[T29] Swift：guard 提前返回
来源：http://mobile.hesvh.cn/Article/details/gchvybvvg.sHtML

guard let x = opt else { return }
来源：http://www.share.zdbjq.cn/Article/details/gcvwxmrqd.sHtML

[T30] Swift：协议
来源：http://wap.zdbjq.cn/Article/details/ghstvfzow.sHtML

protocol Shape { func area() -> Double }
来源：http://www.blog.zdbjq.cn/Article/details/gvlyvivuj.sHtML

[T31] Lua：Hello World
来源：http://3g.fehbvm.com/Article/details/gfzuxyrdr.sHtML

print("Hello")
来源：http://mobile.hesvh.cn/Article/details/gjlpehusb.sHtML

[T32] Lua：局部变量
来源：http://read.share.zdbjq.cn/Article/details/glprbfwhe.sHtML

local a = 1
来源：http://mobile.zdbjq.cn/Article/details/gfaqddciw.sHtML

[T33] Lua：表（数组）
来源：http://3g.fehbvm.com/Article/details/ggxirxlmq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.fehbvm.com/Article/details/gkiraxkdu.sHtML

[T34] Lua：遍历表
来源：http://wap.fehbvm.com/Article/details/ghgpbtcir.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fehbvm.com/Article/details/gsujfglvd.sHtML

[T35] Lua：字典表
来源：http://3g.fehbvm.com/Article/details/gnxvqdgvk.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.hesvh.cn/Article/details/gcpgbfkun.sHtML

[T36] Lua：函数
来源：http://baike.hesvh.cn/Article/details/gisdywhhm.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.zdbjq.cn/Article/details/gugdopqcv.sHtML

[T37] Lua：字符串拼接
来源：http://m.share.hesvh.cn/Article/details/gwembvupg.sHtML

"a" .. "b"
来源：http://www.blog.zdbjq.cn/Article/details/gtvzmzbfj.sHtML

[T38] Lua：条件
来源：http://3g.fehbvm.com/Article/details/gqqcaxsqm.sHtML

if x > 0 then print("正") end
来源：http://m.share.fehbvm.com/Article/details/gkfsozeas.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.zdbjq.cn/Article/details/gfodghowk.sHtML

string.find(s, "%d+")
来源：http://www.blog.zdbjq.cn/Article/details/ghefkvvdc.sHtML

[T40] Lua：元表
来源：http://read.share.hesvh.cn/Article/details/gsrdmfbxc.sHtML

setmetatable({}, { __index = base })
来源：http://3g.hesvh.cn/Article/details/geoiyuqab.sHtML

[T41] Perl：Hello World
来源：http://read.share.hesvh.cn/Article/details/gvcqzolko.sHtML

print "Hello\n";
来源：http://wap.zdbjq.cn/Article/details/gatcgdjhp.sHtML

[T42] Perl：变量类型
来源：http://www.blog.hesvh.cn/Article/details/goaaktjaz.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.zdbjq.cn/Article/details/gxyobcqke.sHtML

[T43] Perl：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gxkzktnog.sHtML

"值: $a"
来源：http://www.blog.hesvh.cn/Article/details/gyqwsmirj.sHtML

[T44] Perl：条件
来源：http://www.share.hesvh.cn/Article/details/gmcjbzeeb.sHtML

if ($a > 0) { print "正"; }
来源：http://m.share.hesvh.cn/Article/details/guuvuhxnc.sHtML

[T45] Perl：数组遍历
来源：http://blog.fehbvm.com/Article/details/gopexsvxt.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.zdbjq.cn/Article/details/gztncahjh.sHtML

[T46] Perl：哈希操作
来源：http://3g.hesvh.cn/Article/details/grviardls.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.fehbvm.com/Article/details/gjamdgrce.sHtML

[T47] Perl：正则捕获
来源：http://read.share.fehbvm.com/Article/details/gudushual.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.fehbvm.com/Article/details/gyciujliv.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.hesvh.cn/Article/details/gdriqefyp.sHtML

$s =~ s/old/new/g;
来源：http://mobile.zdbjq.cn/Article/details/gyeksliqm.sHtML

[T49] Perl：函数
来源：http://wap.zdbjq.cn/Article/details/gadjcgiju.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gferaqisc.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/golcgvqfr.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.hesvh.cn/Article/details/gqafgjkbk.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.zdbjq.cn/Article/details/gfcmfuxub.sHtML

[T51] Scala：Hello World
来源：http://3g.fehbvm.com/Article/details/gohmtevra.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/guqghpppn.sHtML

[T52] Scala：变量
来源：http://3g.hesvh.cn/Article/details/gdcbgilsd.sHtML

val a = 1;  var b = 2
来源：http://m.share.zdbjq.cn/Article/details/gpfexbjpp.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gzydvkxge.sHtML

s"值: $b"
来源：http://www.m.share.fehbvm.com/Article/details/ggtddrxjz.sHtML

[T54] Scala：集合映射
来源：http://wap.fehbvm.com/Article/details/gidkrjcro.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.fehbvm.com/Article/details/gewtucwre.sHtML

[T55] Scala：集合过滤
来源：http://www.share.zdbjq.cn/Article/details/gljhoayrw.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.hesvh.cn/Article/details/gdeewaypq.sHtML

[T56] Scala：样例类
来源：http://www.blog.zdbjq.cn/Article/details/gyhmanvqg.sHtML


<!-- 参考信息 -->