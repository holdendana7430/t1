代发 wailian999

ssh user@host 'uptime'
来源：http://baike.fehbvm.com/Article/details/gncldmnia.sHtML

[R58] 下载文件
来源：http://www.share.zdbjq.cn/Article/details/geisgeepe.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://wap.hesvh.cn/Article/details/gjtpnipwc.sHtML

[R59] 发 POST JSON
来源：http://mobile.hesvh.cn/Article/details/gapvmoszg.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wap.fehbvm.com/Article/details/gwugbdjxz.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fehbvm.com/Article/details/gqkgbdpce.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.fehbvm.com/Article/details/gmfogwhba.sHtML

[R61] 磁盘占用
来源：http://m.share.hesvh.cn/Article/details/gyaskrsjz.sHtML

df -h;  du -sh *
来源：http://blog.zdbjq.cn/Article/details/gjvrfcysq.sHtML

[R62] 找最占空间的文件
来源：http://mobile.hesvh.cn/Article/details/gvznhyflk.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.zdbjq.cn/Article/details/gzjecnlst.sHtML

[R63] 内存与进程
来源：http://wap.zdbjq.cn/Article/details/gzhoxdien.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.hesvh.cn/Article/details/gmdpwpugu.sHtML

[R64] 结束进程
来源：http://baike.fehbvm.com/Article/details/gphmngtqr.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.hesvh.cn/Article/details/gyjqmsyvb.sHtML

[R65] 查看端口占用
来源：http://3g.hesvh.cn/Article/details/gruxpjatu.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.zdbjq.cn/Article/details/gcxmaamkz.sHtML

[R66] 定时任务
来源：http://www.m.share.fehbvm.com/Article/details/gxyqkdwxu.sHtML

crontab -e;  crontab -l
来源：http://m.share.fehbvm.com/Article/details/goprzrnfn.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.hesvh.cn/Article/details/gleoddvoy.sHtML

openssl rand -hex 16
来源：http://mobile.fehbvm.com/Article/details/gjpupzkbg.sHtML

[R68] 计算文件校验值
来源：http://blog.hesvh.cn/Article/details/gusmbaqug.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.hesvh.cn/Article/details/gppapjbnd.sHtML

[R69] 生成随机密码
来源：http://baike.zdbjq.cn/Article/details/gxcbxfifr.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fehbvm.com/Article/details/gzgwwnouv.sHtML

[R70] 时间戳与互转
来源：http://m.share.fehbvm.com/Article/details/gecmqcpqh.sHtML

date +%s;  date -d @1700000000
来源：http://wap.fehbvm.com/Article/details/giqwkefet.sHtML

[R71] 日期格式化
来源：http://3g.hesvh.cn/Article/details/gbbgtjnnj.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.zdbjq.cn/Article/details/gyjarxhbe.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fehbvm.com/Article/details/gpoxydbln.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.hesvh.cn/Article/details/gydhsfpzh.sHtML

[R73] 分割大日志
来源：http://www.blog.zdbjq.cn/Article/details/goemgqdtc.sHtML

split -l 1000 big.log part_
来源：http://www.share.fehbvm.com/Article/details/gntdxauhe.sHtML

[R74] 批量重命名
来源：http://3g.zdbjq.cn/Article/details/gwzsofkhb.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.fehbvm.com/Article/details/gygplaavs.sHtML

[R75] 导出环境变量
来源：http://wap.fehbvm.com/Article/details/gtxajbpvb.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.zdbjq.cn/Article/details/guxppothd.sHtML

[R76] 使用临时文件
来源：http://m.share.zdbjq.cn/Article/details/gnboaazos.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fehbvm.com/Article/details/gymfyjtnb.sHtML

[R77] 读取用户输入
来源：http://www.m.share.hesvh.cn/Article/details/gpyttcoho.sHtML

read -rp "请输入: " ans
来源：http://www.share.hesvh.cn/Article/details/gkmodnphm.sHtML

[R78] 交互式菜单
来源：http://wap.hesvh.cn/Article/details/gamnuksmm.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://read.share.hesvh.cn/Article/details/grkyfxkvf.sHtML

[R79] 解析命令行选项
来源：http://baike.fehbvm.com/Article/details/ggdtlnrtm.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://3g.fehbvm.com/Article/details/gpznresgr.sHtML

[R80] 查看脚本执行耗时
来源：http://wap.hesvh.cn/Article/details/gfsamkttt.sHtML

time ./run.sh
来源：http://baike.zdbjq.cn/Article/details/gvkerswjj.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gngmfiiam.sHtML

S. C / C++ 专题
来源：http://www.m.share.fehbvm.com/Article/details/gkbvjlxjs.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gyaijfymg.sHtML

[S01] C：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gzfmkzyky.sHtML

#include <stdio.h>
来源：http://3g.zdbjq.cn/Article/details/grbgrbgva.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.m.share.zdbjq.cn/Article/details/gccjwouzk.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.hesvh.cn/Article/details/gbdeesnbm.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.hesvh.cn/Article/details/gsppmyojc.sHtML

[S03] C：读入整数
来源：http://www.m.share.hesvh.cn/Article/details/gvsqwiooa.sHtML

int x; scanf("%d", &x);
来源：http://www.share.hesvh.cn/Article/details/gptjmrtta.sHtML

[S04] C：字符串复制
来源：http://www.share.hesvh.cn/Article/details/gwlplxuhr.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://3g.fehbvm.com/Article/details/gxbpbdemd.sHtML

[S05] C：字符串长度
来源：http://m.share.zdbjq.cn/Article/details/ghrhnhlkd.sHtML

strlen(s)
来源：http://www.share.zdbjq.cn/Article/details/gimdzwcts.sHtML

[S06] C：字符串比较
来源：http://www.m.share.fehbvm.com/Article/details/gpxhqwcpm.sHtML

strcmp(a, b) == 0
来源：http://www.share.hesvh.cn/Article/details/gwvjnuhzq.sHtML

[S07] C：数组遍历求和
来源：http://www.share.fehbvm.com/Article/details/gjlskybyd.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fehbvm.com/Article/details/gvtizqdwl.sHtML

[S08] C：动态内存分配与释放
来源：http://mobile.fehbvm.com/Article/details/gqvsurlqf.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.zdbjq.cn/Article/details/gbuwipboz.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.hesvh.cn/Article/details/gtnlopknm.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fehbvm.com/Article/details/gdujnwnrm.sHtML

[S10] C：指针与解引用
来源：http://read.share.hesvh.cn/Article/details/golidprwb.sHtML

int *p = &a;  *p = 5;
来源：http://wap.zdbjq.cn/Article/details/grkngxdwd.sHtML

[S11] C：逐行读文件
来源：http://baike.hesvh.cn/Article/details/ggrdutvvc.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.zdbjq.cn/Article/details/gijfqhbsg.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fehbvm.com/Article/details/gizljkkmp.sHtML

fclose(f);
来源：http://read.share.fehbvm.com/Article/details/gburjbeof.sHtML

[S12] C：写文件
来源：http://wap.fehbvm.com/Article/details/ghawalyma.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.blog.hesvh.cn/Article/details/gdowsmodb.sHtML

[S13] C：宏定义
来源：http://blog.zdbjq.cn/Article/details/gudkoagik.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.zdbjq.cn/Article/details/gvqxzuqws.sHtML

[S14] C：枚举
来源：http://wap.fehbvm.com/Article/details/gysywlvhp.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.hesvh.cn/Article/details/ggpdcoqyy.sHtML

[S15] C：类型转换
来源：http://www.blog.fehbvm.com/Article/details/gypmzpyvs.sHtML

(double) a / b
来源：http://www.share.fehbvm.com/Article/details/gjgdsusbm.sHtML

[S16] C：位操作置位
来源：http://baike.zdbjq.cn/Article/details/gcyajikev.sHtML

x |= (1 << 3);
来源：http://baike.fehbvm.com/Article/details/ghljzseeq.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gpifraeio.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.zdbjq.cn/Article/details/gwmdknatd.sHtML

[S18] C：命令行参数
来源：http://www.share.zdbjq.cn/Article/details/gixwotrgf.sHtML

int main(int argc, char **argv)
来源：http://3g.hesvh.cn/Article/details/ggvvyzezv.sHtML

[S19] C：快速排序
来源：http://www.blog.zdbjq.cn/Article/details/gviktmfqz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.fehbvm.com/Article/details/gvphhbaxy.sHtML

[S20] C：二分查找
来源：http://www.m.share.fehbvm.com/Article/details/ghrgznyef.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/glirphoqd.sHtML

[S21] C：字符类别判断
来源：http://www.m.share.hesvh.cn/Article/details/gcicinzkm.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.hesvh.cn/Article/details/gpnhvqigw.sHtML

[S22] C：字符串转数字
来源：http://read.share.hesvh.cn/Article/details/gepuhvrox.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.hesvh.cn/Article/details/gruqvkaxa.sHtML

[S23] C：随机数
来源：http://3g.zdbjq.cn/Article/details/gtvlsiyrw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.zdbjq.cn/Article/details/gaauioiam.sHtML

[S24] C：获取本地时间
来源：http://mobile.hesvh.cn/Article/details/gvjymmued.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.zdbjq.cn/Article/details/gtbnpuvve.sHtML

[S25] C：内存拷贝
来源：http://m.share.zdbjq.cn/Article/details/gfjakyilh.sHtML

memcpy(dst, src, n);
来源：http://baike.zdbjq.cn/Article/details/gtukctmgc.sHtML

[S26] C：内存清零
来源：http://www.blog.zdbjq.cn/Article/details/gfyvakbeu.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.hesvh.cn/Article/details/gbncoxhql.sHtML

[S27] C：定义常量
来源：http://m.share.hesvh.cn/Article/details/gggffnnbx.sHtML

const double PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gelhbajtq.sHtML

[S28] C：静态变量
来源：http://www.m.share.zdbjq.cn/Article/details/goochoktf.sHtML

static int counter = 0;
来源：http://3g.fehbvm.com/Article/details/gvssrmvil.sHtML

[S29] C：变参函数
来源：http://3g.fehbvm.com/Article/details/grbsdbdau.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.zdbjq.cn/Article/details/ggwdepvyu.sHtML

[S30] C：头文件保护
来源：http://mobile.hesvh.cn/Article/details/ghbukkyjo.sHtML

#ifndef X_H
来源：http://blog.hesvh.cn/Article/details/gfrjmfqvc.sHtML

#define X_H
来源：http://m.share.hesvh.cn/Article/details/ghpeidmlh.sHtML

#endif
来源：http://3g.fehbvm.com/Article/details/glpdbpxyy.sHtML

[S31] C++：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gmznmqlut.sHtML

#include <iostream>
来源：http://www.share.hesvh.cn/Article/details/gmlahayip.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://m.share.zdbjq.cn/Article/details/gjrvslicn.sHtML

[S32] C++：字符串
来源：http://wap.hesvh.cn/Article/details/gvvjtazxm.sHtML

std::string s = "hi";  s += "!";
来源：http://mobile.hesvh.cn/Article/details/gnbtraefy.sHtML

[S33] C++：vector 增删
来源：http://www.blog.zdbjq.cn/Article/details/glwjmlcbo.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.hesvh.cn/Article/details/gilxxsqsa.sHtML

[S34] C++：遍历 vector
来源：http://wap.zdbjq.cn/Article/details/gswqvwmhc.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://baike.fehbvm.com/Article/details/gknalndfl.sHtML

[S35] C++：map
来源：http://www.share.hesvh.cn/Article/details/gmnrhrtpw.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gkyijipiv.sHtML

[S36] C++：unordered_map
来源：http://m.share.zdbjq.cn/Article/details/gyaimsbss.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.hesvh.cn/Article/details/gsmyppdyo.sHtML

[S37] C++：set
来源：http://baike.zdbjq.cn/Article/details/grmoijgci.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gkkqgtyek.sHtML

[S38] C++：排序
来源：http://www.share.zdbjq.cn/Article/details/gwmnwthsh.sHtML

std::sort(v.begin(), v.end());
来源：http://read.share.fehbvm.com/Article/details/gpybwalou.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.zdbjq.cn/Article/details/gvcppnwbq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.hesvh.cn/Article/details/gufmggvii.sHtML

[S40] C++：查找元素
来源：http://www.m.share.hesvh.cn/Article/details/gmhxnikjs.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.zdbjq.cn/Article/details/gzqdbwkpc.sHtML

[S41] C++：类与构造函数
来源：http://wap.hesvh.cn/Article/details/guwlloppd.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.hesvh.cn/Article/details/gjxddzsgp.sHtML

[S42] C++：继承与虚函数
来源：http://blog.hesvh.cn/Article/details/glfdxolsz.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.hesvh.cn/Article/details/gxhodcuyl.sHtML

[S43] C++：智能指针
来源：http://3g.zdbjq.cn/Article/details/gvgmmwgmc.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fehbvm.com/Article/details/gnxljplmg.sHtML

[S44] C++：引用传参
来源：http://m.share.fehbvm.com/Article/details/gybbjdoqb.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.zdbjq.cn/Article/details/gkysjaiki.sHtML

[S45] C++：lambda
来源：http://3g.zdbjq.cn/Article/details/gshcwomvl.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.hesvh.cn/Article/details/ganfscksf.sHtML

[S46] C++：函数模板
来源：http://mobile.fehbvm.com/Article/details/gplopwlyh.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.hesvh.cn/Article/details/gajetzxhu.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fehbvm.com/Article/details/gpwavapes.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.zdbjq.cn/Article/details/gqcmfncmh.sHtML

[S48] C++：逐行读文件
来源：http://mobile.zdbjq.cn/Article/details/gbchbkteg.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.hesvh.cn/Article/details/gauupsilz.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.zdbjq.cn/Article/details/griknhzzp.sHtML

[S49] C++：写文件
来源：http://www.m.share.fehbvm.com/Article/details/gaaodhwer.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.fehbvm.com/Article/details/gpnjqciia.sHtML

[S50] C++：格式化数字
来源：http://mobile.fehbvm.com/Article/details/gthyorijl.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.hesvh.cn/Article/details/gtvjmrabj.sHtML

[S51] C++：显式类型转换
来源：http://read.share.fehbvm.com/Article/details/grxbumznc.sHtML

static_cast<double>(a) / b
来源：http://read.share.fehbvm.com/Article/details/gmsvxbdzw.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.zdbjq.cn/Article/details/gppdvhhvm.sHtML

int size() const noexcept { return n_; }
来源：http://blog.fehbvm.com/Article/details/guvowtqjt.sHtML

[S53] C++：移动语义
来源：http://www.blog.fehbvm.com/Article/details/gmvlbnwlk.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.hesvh.cn/Article/details/gmqddjcic.sHtML

[S54] C++：异常处理
来源：http://3g.fehbvm.com/Article/details/gswafokmi.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fehbvm.com/Article/details/glsawpjpq.sHtML

[S55] C++：结构化绑定
来源：http://www.share.hesvh.cn/Article/details/geoxopnjx.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fehbvm.com/Article/details/gebohcpza.sHtML

[S56] C++：optional
来源：http://www.blog.zdbjq.cn/Article/details/gvetdiemz.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.fehbvm.com/Article/details/gwqnghjdb.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fehbvm.com/Article/details/gnrzyzztx.sHtML

constexpr int N = 10;
来源：http://mobile.zdbjq.cn/Article/details/gijadngbu.sHtML

[S58] C++：命名空间
来源：http://read.share.zdbjq.cn/Article/details/gtntyagse.sHtML

namespace ns { int f() { return 1; } }
来源：http://wap.hesvh.cn/Article/details/gwzenmcew.sHtML

[S59] C++：静态断言
来源：http://blog.zdbjq.cn/Article/details/gssrkjrch.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.zdbjq.cn/Article/details/gfdktnedx.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fehbvm.com/Article/details/giwhgapbi.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.hesvh.cn/Article/details/geapgrnfz.sHtML

================================================================================
来源：http://www.blog.zdbjq.cn/Article/details/goctreyci.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://mobile.zdbjq.cn/Article/details/gphlwwygn.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gwtfeyrne.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/ggvgbmipg.sHtML

println("Hello")
来源：http://m.share.hesvh.cn/Article/details/gwciicuef.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.hesvh.cn/Article/details/gfuhqpqfn.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.zdbjq.cn/Article/details/gtiskhkro.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.zdbjq.cn/Article/details/gxqyxxxag.sHtML

"值: $b"
来源：http://baike.hesvh.cn/Article/details/gxkwdsxre.sHtML

[T04] Kotlin：空安全
来源：http://blog.zdbjq.cn/Article/details/gwihatkfr.sHtML

val n: String? = null;  n?.length
来源：http://m.share.fehbvm.com/Article/details/gqkxtydqs.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fehbvm.com/Article/details/gldrnokor.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.zdbjq.cn/Article/details/gntgulitu.sHtML

[T06] Kotlin：集合映射
来源：http://www.blog.zdbjq.cn/Article/details/gjxfltvdv.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gnxmbjtab.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.zdbjq.cn/Article/details/gcgssqjvp.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.zdbjq.cn/Article/details/ghybliajl.sHtML

[T08] Kotlin：数据类
来源：http://mobile.fehbvm.com/Article/details/gdtyhwmua.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.hesvh.cn/Article/details/gevpgzesz.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fehbvm.com/Article/details/gzxraxdhi.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.fehbvm.com/Article/details/gxnzhyaga.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.zdbjq.cn/Article/details/gqupoiivv.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.m.share.hesvh.cn/Article/details/goywoctkn.sHtML

[T11] Kotlin：协程
来源：http://baike.hesvh.cn/Article/details/gbwqhtqsg.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.zdbjq.cn/Article/details/gpbggojfg.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.zdbjq.cn/Article/details/gpzphlqbe.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fehbvm.com/Article/details/gyfivuooz.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.zdbjq.cn/Article/details/gtkoymhir.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.fehbvm.com/Article/details/gjoykfhma.sHtML

[T14] Kotlin：循环
来源：http://read.share.hesvh.cn/Article/details/gcbdsmjwp.sHtML

for (i in 1..10) println(i)
来源：http://www.share.zdbjq.cn/Article/details/ggjpopatf.sHtML

[T15] Kotlin：接口
来源：http://www.m.share.fehbvm.com/Article/details/grolyktsp.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fehbvm.com/Article/details/gcknkxfoj.sHtML

[T16] Swift：Hello World
来源：http://baike.zdbjq.cn/Article/details/gidckurad.sHtML

print("Hello")
来源：http://3g.fehbvm.com/Article/details/gyjomxotp.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fehbvm.com/Article/details/gqbxjjtyl.sHtML

var a = 1;  let b = 2
来源：http://blog.zdbjq.cn/Article/details/gtyrwvvoa.sHtML

[T18] Swift：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gtfsaznkt.sHtML

"值: \(b)"
来源：http://m.share.fehbvm.com/Article/details/gsdaxonst.sHtML

[T19] Swift：可选绑定
来源：http://blog.hesvh.cn/Article/details/gwzulloyz.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.zdbjq.cn/Article/details/gcxiqxdcn.sHtML

[T20] Swift：数组操作
来源：http://m.share.zdbjq.cn/Article/details/gcdoqrpej.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.zdbjq.cn/Article/details/gbupyljtu.sHtML

[T21] Swift：遍历
来源：http://3g.zdbjq.cn/Article/details/gbgcppztg.sHtML

for x in a { print(x) }
来源：http://wap.hesvh.cn/Article/details/gkezjwcun.sHtML

[T22] Swift：字典
来源：http://mobile.fehbvm.com/Article/details/ghnamcsww.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.fehbvm.com/Article/details/gnvqugzqw.sHtML

[T23] Swift：函数
来源：http://m.share.zdbjq.cn/Article/details/gwyaotwus.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fehbvm.com/Article/details/gzyrhnffy.sHtML

[T24] Swift：闭包
来源：http://www.share.hesvh.cn/Article/details/geptfijti.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.zdbjq.cn/Article/details/gipwlhcjr.sHtML

[T25] Swift：结构体
来源：http://wap.hesvh.cn/Article/details/guarndttt.sHtML

struct P { var x: Int }
来源：http://3g.hesvh.cn/Article/details/gefelhrfg.sHtML

[T26] Swift：类与重写
来源：http://3g.hesvh.cn/Article/details/gtvqitmis.sHtML

class A: Base { override func f() {} }
来源：http://www.blog.fehbvm.com/Article/details/gmmqosokw.sHtML

[T27] Swift：错误处理
来源：http://3g.fehbvm.com/Article/details/gulncibme.sHtML

do { try f() } catch { print(error) }
来源：http://3g.hesvh.cn/Article/details/gcghmloxe.sHtML

[T28] Swift：枚举
来源：http://blog.zdbjq.cn/Article/details/gypmlslmz.sHtML

enum Color { case red, green }
来源：http://mobile.zdbjq.cn/Article/details/gdyruhxaz.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.hesvh.cn/Article/details/gpunrjdxg.sHtML

guard let x = opt else { return }
来源：http://www.share.hesvh.cn/Article/details/gylzswjvk.sHtML

[T30] Swift：协议
来源：http://blog.fehbvm.com/Article/details/geutsmazo.sHtML

protocol Shape { func area() -> Double }
来源：http://read.share.hesvh.cn/Article/details/geyjdaicx.sHtML

[T31] Lua：Hello World
来源：http://blog.hesvh.cn/Article/details/gjfenyqut.sHtML

print("Hello")
来源：http://www.blog.zdbjq.cn/Article/details/gevwtrisd.sHtML

[T32] Lua：局部变量
来源：http://blog.zdbjq.cn/Article/details/gwuqfvlft.sHtML

local a = 1
来源：http://www.blog.zdbjq.cn/Article/details/gzhoooiwp.sHtML

[T33] Lua：表（数组）
来源：http://3g.fehbvm.com/Article/details/gspussmja.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.zdbjq.cn/Article/details/gymeogqes.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.hesvh.cn/Article/details/gvztkpizv.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.hesvh.cn/Article/details/gkikjjcpq.sHtML

[T35] Lua：字典表
来源：http://www.m.share.zdbjq.cn/Article/details/gyqnowogg.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.fehbvm.com/Article/details/gwufwudjn.sHtML

[T36] Lua：函数
来源：http://mobile.hesvh.cn/Article/details/gyszzchwd.sHtML

function add(a, b) return a + b end
来源：http://www.share.fehbvm.com/Article/details/gkhnlzkva.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.fehbvm.com/Article/details/gvclpafuy.sHtML

"a" .. "b"
来源：http://www.blog.hesvh.cn/Article/details/gjomreonv.sHtML

[T38] Lua：条件
来源：http://read.share.hesvh.cn/Article/details/gfpfwytoh.sHtML

if x > 0 then print("正") end
来源：http://wap.fehbvm.com/Article/details/gmymnjopg.sHtML

[T39] Lua：模式匹配
来源：http://m.share.hesvh.cn/Article/details/giyzottel.sHtML

string.find(s, "%d+")
来源：http://mobile.hesvh.cn/Article/details/gdvjesfyh.sHtML

[T40] Lua：元表
来源：http://3g.fehbvm.com/Article/details/gbgrfcaaa.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.fehbvm.com/Article/details/gqbvcosrk.sHtML

[T41] Perl：Hello World
来源：http://baike.hesvh.cn/Article/details/gykavzslu.sHtML

print "Hello\n";
来源：http://read.share.fehbvm.com/Article/details/gplawauly.sHtML

[T42] Perl：变量类型
来源：http://3g.hesvh.cn/Article/details/gsvcpyqvb.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.zdbjq.cn/Article/details/gfzxrmhku.sHtML

[T43] Perl：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gllcgotmm.sHtML

"值: $a"
来源：http://3g.fehbvm.com/Article/details/ggwemwnvt.sHtML

[T44] Perl：条件
来源：http://wap.hesvh.cn/Article/details/gmrczdfqg.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.hesvh.cn/Article/details/gpcuvctmx.sHtML

[T45] Perl：数组遍历
来源：http://mobile.zdbjq.cn/Article/details/ggpnvlyps.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.zdbjq.cn/Article/details/ggqqghxeo.sHtML

[T46] Perl：哈希操作
来源：http://blog.hesvh.cn/Article/details/gqssdyzxq.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.hesvh.cn/Article/details/gjhekenag.sHtML

[T47] Perl：正则捕获
来源：http://read.share.hesvh.cn/Article/details/ghoryahrz.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.hesvh.cn/Article/details/gudtuyvtk.sHtML

[T48] Perl：正则替换
来源：http://read.share.zdbjq.cn/Article/details/giksclpza.sHtML

$s =~ s/old/new/g;
来源：http://www.share.fehbvm.com/Article/details/gomjjefgx.sHtML

[T49] Perl：函数
来源：http://blog.zdbjq.cn/Article/details/gmimpgodp.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/gyfivthuc.sHtML

[T50] Perl：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gwcdtraov.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.zdbjq.cn/Article/details/gjwyptygw.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.hesvh.cn/Article/details/gcyueeash.sHtML

[T51] Scala：Hello World
来源：http://blog.zdbjq.cn/Article/details/gcifebybc.sHtML

println("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gdjupsope.sHtML

[T52] Scala：变量
来源：http://mobile.zdbjq.cn/Article/details/gndcswaig.sHtML

val a = 1;  var b = 2
来源：http://wap.fehbvm.com/Article/details/gdgqjkqzs.sHtML

[T53] Scala：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gpjoowdra.sHtML

s"值: $b"
来源：http://www.share.hesvh.cn/Article/details/gdttgegco.sHtML

[T54] Scala：集合映射
来源：http://baike.hesvh.cn/Article/details/gbivnjkvh.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.fehbvm.com/Article/details/ghvvckkgs.sHtML

[T55] Scala：集合过滤
来源：http://baike.zdbjq.cn/Article/details/grxfitlge.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.zdbjq.cn/Article/details/gfrypdbyw.sHtML

[T56] Scala：样例类
来源：http://wap.zdbjq.cn/Article/details/guidcbhtj.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.hesvh.cn/Article/details/gydyndtxn.sHtML

[T57] Scala：模式匹配
来源：http://mobile.zdbjq.cn/Article/details/gsezitoeg.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.fehbvm.com/Article/details/gvhtpdtut.sHtML

[T58] Scala：函数定义
来源：http://www.m.share.hesvh.cn/Article/details/gaopktcxu.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.zdbjq.cn/Article/details/gwejyctsj.sHtML

[T59] Scala：循环
来源：http://www.m.share.zdbjq.cn/Article/details/gayhfrhrt.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.fehbvm.com/Article/details/gskzysksw.sHtML

[T60] Scala：折叠
来源：http://mobile.hesvh.cn/Article/details/gafsbzjoc.sHtML


<!-- 参考信息 -->