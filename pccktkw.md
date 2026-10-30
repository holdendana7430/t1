代发 wailian999

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://m.share.hesvh.cn/Article/details/goxkedemq.sHtML

[R56] 远程拷贝
来源：http://blog.hesvh.cn/Article/details/grzgdmuwn.sHtML

scp file user@host:/path/
来源：http://read.share.hesvh.cn/Article/details/glefkqcbn.sHtML

[R57] 远程执行命令
来源：http://mobile.fehbvm.com/Article/details/gzszizrgp.sHtML

ssh user@host 'uptime'
来源：http://read.share.fehbvm.com/Article/details/gqeabjrft.sHtML

[R58] 下载文件
来源：http://www.share.hesvh.cn/Article/details/gypxsoooh.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.zdbjq.cn/Article/details/gljnfdono.sHtML

[R59] 发 POST JSON
来源：http://www.share.zdbjq.cn/Article/details/gthrjwejq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.zdbjq.cn/Article/details/grhajelmv.sHtML

[R60] 只看 HTTP 状态码
来源：http://mobile.zdbjq.cn/Article/details/gedvdjfzj.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.hesvh.cn/Article/details/gmzpgppsk.sHtML

[R61] 磁盘占用
来源：http://baike.zdbjq.cn/Article/details/gghrugiwd.sHtML

df -h;  du -sh *
来源：http://m.share.zdbjq.cn/Article/details/gqicnzhax.sHtML

[R62] 找最占空间的文件
来源：http://baike.fehbvm.com/Article/details/gjotffsas.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.fehbvm.com/Article/details/ghxnidrlc.sHtML

[R63] 内存与进程
来源：http://www.blog.hesvh.cn/Article/details/grkmyyfdg.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fehbvm.com/Article/details/gdickxayk.sHtML

[R64] 结束进程
来源：http://wap.zdbjq.cn/Article/details/gblfxxpny.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fehbvm.com/Article/details/gziyusehw.sHtML

[R65] 查看端口占用
来源：http://wap.zdbjq.cn/Article/details/gaalrrevq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.zdbjq.cn/Article/details/grmxtrsma.sHtML

[R66] 定时任务
来源：http://www.blog.zdbjq.cn/Article/details/guqsjqgrt.sHtML

crontab -e;  crontab -l
来源：http://3g.fehbvm.com/Article/details/gauykmwtl.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.zdbjq.cn/Article/details/gnewekjcu.sHtML

openssl rand -hex 16
来源：http://read.share.hesvh.cn/Article/details/gapmaqpcg.sHtML

[R68] 计算文件校验值
来源：http://www.blog.fehbvm.com/Article/details/golhdjbrl.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.hesvh.cn/Article/details/gwotpmgui.sHtML

[R69] 生成随机密码
来源：http://mobile.hesvh.cn/Article/details/gurseicit.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.zdbjq.cn/Article/details/gtvatttba.sHtML

[R70] 时间戳与互转
来源：http://m.share.zdbjq.cn/Article/details/gpfofhhqu.sHtML

date +%s;  date -d @1700000000
来源：http://www.m.share.hesvh.cn/Article/details/gfusltdfs.sHtML

[R71] 日期格式化
来源：http://read.share.fehbvm.com/Article/details/ggltvcqqf.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.hesvh.cn/Article/details/gzlezfwak.sHtML

[R72] 等待端口就绪
来源：http://wap.hesvh.cn/Article/details/gnluqrybk.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fehbvm.com/Article/details/gshhsupzt.sHtML

[R73] 分割大日志
来源：http://3g.fehbvm.com/Article/details/gsbjsuamn.sHtML

split -l 1000 big.log part_
来源：http://www.blog.hesvh.cn/Article/details/gpjcmbguc.sHtML

[R74] 批量重命名
来源：http://mobile.hesvh.cn/Article/details/gztkqatxb.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.hesvh.cn/Article/details/guzrbvnaa.sHtML

[R75] 导出环境变量
来源：http://wap.hesvh.cn/Article/details/gnogijrsr.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.hesvh.cn/Article/details/geamlppye.sHtML

[R76] 使用临时文件
来源：http://wap.hesvh.cn/Article/details/gveeuznms.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fehbvm.com/Article/details/galjcvlnn.sHtML

[R77] 读取用户输入
来源：http://mobile.fehbvm.com/Article/details/gygjlflsn.sHtML

read -rp "请输入: " ans
来源：http://blog.fehbvm.com/Article/details/goozgvaep.sHtML

[R78] 交互式菜单
来源：http://wap.fehbvm.com/Article/details/gsfikwzlz.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fehbvm.com/Article/details/gltcscenf.sHtML

[R79] 解析命令行选项
来源：http://www.blog.zdbjq.cn/Article/details/gfuboxhox.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.zdbjq.cn/Article/details/gxecxugav.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fehbvm.com/Article/details/gbqepzvdv.sHtML

time ./run.sh
来源：http://www.share.hesvh.cn/Article/details/gavthddcb.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gbywqtsqv.sHtML

S. C / C++ 专题
来源：http://read.share.fehbvm.com/Article/details/gwrfbvklc.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gtyaheuqx.sHtML

[S01] C：Hello World
来源：http://baike.hesvh.cn/Article/details/gosxmjtqx.sHtML

#include <stdio.h>
来源：http://mobile.hesvh.cn/Article/details/gzbknfaoe.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://mobile.zdbjq.cn/Article/details/gacadkbep.sHtML

[S02] C：变量与格式化输出
来源：http://baike.zdbjq.cn/Article/details/gchsviset.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.zdbjq.cn/Article/details/gsppiprqu.sHtML

[S03] C：读入整数
来源：http://read.share.fehbvm.com/Article/details/gtwqmdbkz.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fehbvm.com/Article/details/glxbyhyie.sHtML

[S04] C：字符串复制
来源：http://baike.hesvh.cn/Article/details/gddemdkkj.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://mobile.fehbvm.com/Article/details/gsmiswmpm.sHtML

[S05] C：字符串长度
来源：http://mobile.hesvh.cn/Article/details/gctdgojaz.sHtML

strlen(s)
来源：http://m.share.hesvh.cn/Article/details/gjkenlmfy.sHtML

[S06] C：字符串比较
来源：http://3g.hesvh.cn/Article/details/gfrfbkcvs.sHtML

strcmp(a, b) == 0
来源：http://3g.fehbvm.com/Article/details/grkfenqca.sHtML

[S07] C：数组遍历求和
来源：http://3g.zdbjq.cn/Article/details/gjisgpeke.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.fehbvm.com/Article/details/gidvzyacv.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.zdbjq.cn/Article/details/gurqrxluf.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.hesvh.cn/Article/details/gbpjpqfxm.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.hesvh.cn/Article/details/gpnmdgzti.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.share.fehbvm.com/Article/details/gnehmrtcs.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fehbvm.com/Article/details/goqwqtafx.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.zdbjq.cn/Article/details/gbqkjltch.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gumzbtrbp.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.fehbvm.com/Article/details/gydcwzapa.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://baike.fehbvm.com/Article/details/gxncajxgc.sHtML

fclose(f);
来源：http://read.share.zdbjq.cn/Article/details/giacrkszr.sHtML

[S12] C：写文件
来源：http://3g.hesvh.cn/Article/details/gxjxsvqmj.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fehbvm.com/Article/details/gxrwwmcvw.sHtML

[S13] C：宏定义
来源：http://wap.fehbvm.com/Article/details/gwyexzxvz.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://m.share.fehbvm.com/Article/details/gpfvokrdk.sHtML

[S14] C：枚举
来源：http://www.m.share.hesvh.cn/Article/details/gdovltneg.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://blog.fehbvm.com/Article/details/gsdihfkfx.sHtML

[S15] C：类型转换
来源：http://baike.zdbjq.cn/Article/details/gxmirivhd.sHtML

(double) a / b
来源：http://read.share.fehbvm.com/Article/details/gaqotjpgf.sHtML

[S16] C：位操作置位
来源：http://www.share.zdbjq.cn/Article/details/gvdhcggng.sHtML

x |= (1 << 3);
来源：http://wap.zdbjq.cn/Article/details/ggiiffeox.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/grlieysld.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.hesvh.cn/Article/details/gbwblhkoc.sHtML

[S18] C：命令行参数
来源：http://www.m.share.zdbjq.cn/Article/details/gsbbhilso.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fehbvm.com/Article/details/gjetjqdff.sHtML

[S19] C：快速排序
来源：http://www.m.share.zdbjq.cn/Article/details/guilbbdib.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.hesvh.cn/Article/details/gppivdfvs.sHtML

[S20] C：二分查找
来源：http://3g.zdbjq.cn/Article/details/gyoypbkjm.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/gjeissbqs.sHtML

[S21] C：字符类别判断
来源：http://m.share.zdbjq.cn/Article/details/ghctxwmov.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.m.share.zdbjq.cn/Article/details/gyfdclbeg.sHtML

[S22] C：字符串转数字
来源：http://read.share.hesvh.cn/Article/details/gxrhlxsxj.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.hesvh.cn/Article/details/gbtfwkxyg.sHtML

[S23] C：随机数
来源：http://read.share.fehbvm.com/Article/details/gxfmtjtrc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.hesvh.cn/Article/details/gxxqjfjxv.sHtML

[S24] C：获取本地时间
来源：http://www.share.zdbjq.cn/Article/details/gjvpqlrce.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fehbvm.com/Article/details/ggordplzn.sHtML

[S25] C：内存拷贝
来源：http://m.share.fehbvm.com/Article/details/gtmqyanko.sHtML

memcpy(dst, src, n);
来源：http://blog.zdbjq.cn/Article/details/gxekdqmbp.sHtML

[S26] C：内存清零
来源：http://www.m.share.fehbvm.com/Article/details/geddtodqt.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fehbvm.com/Article/details/gtdulhmba.sHtML

[S27] C：定义常量
来源：http://www.share.zdbjq.cn/Article/details/gqcywslim.sHtML

const double PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/guhvquhdd.sHtML

[S28] C：静态变量
来源：http://mobile.zdbjq.cn/Article/details/gjvfjkstn.sHtML

static int counter = 0;
来源：http://baike.fehbvm.com/Article/details/gdujxamya.sHtML

[S29] C：变参函数
来源：http://baike.fehbvm.com/Article/details/gmfrddiov.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.fehbvm.com/Article/details/gloapczld.sHtML

[S30] C：头文件保护
来源：http://read.share.fehbvm.com/Article/details/ghcflaenp.sHtML

#ifndef X_H
来源：http://read.share.zdbjq.cn/Article/details/gyigvjvtt.sHtML

#define X_H
来源：http://mobile.zdbjq.cn/Article/details/guwhjtvex.sHtML

#endif
来源：http://baike.fehbvm.com/Article/details/gnnfstuar.sHtML

[S31] C++：Hello World
来源：http://mobile.hesvh.cn/Article/details/gqgvtehtt.sHtML

#include <iostream>
来源：http://read.share.hesvh.cn/Article/details/gscjiukcy.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fehbvm.com/Article/details/gelcwemlz.sHtML

[S32] C++：字符串
来源：http://blog.hesvh.cn/Article/details/gtstrieoy.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.hesvh.cn/Article/details/gnxccytlv.sHtML

[S33] C++：vector 增删
来源：http://mobile.hesvh.cn/Article/details/gixfpfqtk.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.hesvh.cn/Article/details/gphuqeigf.sHtML

[S34] C++：遍历 vector
来源：http://m.share.zdbjq.cn/Article/details/ggwkhhzme.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.hesvh.cn/Article/details/grnoqccca.sHtML

[S35] C++：map
来源：http://www.blog.hesvh.cn/Article/details/gcvqtdtih.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gjbtkkqwb.sHtML

[S36] C++：unordered_map
来源：http://www.blog.zdbjq.cn/Article/details/gbkkgavmh.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.zdbjq.cn/Article/details/gfltbohfi.sHtML

[S37] C++：set
来源：http://www.m.share.hesvh.cn/Article/details/gmnnkweud.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.zdbjq.cn/Article/details/gxegqdcmo.sHtML

[S38] C++：排序
来源：http://m.share.fehbvm.com/Article/details/gttvadalr.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.zdbjq.cn/Article/details/gdiqcmbke.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.hesvh.cn/Article/details/gwsclcnoy.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.zdbjq.cn/Article/details/gzsygnuic.sHtML

[S40] C++：查找元素
来源：http://3g.fehbvm.com/Article/details/giiuqqwon.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.zdbjq.cn/Article/details/gcjgzhyxp.sHtML

[S41] C++：类与构造函数
来源：http://blog.zdbjq.cn/Article/details/ghlypqfrv.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fehbvm.com/Article/details/gwrssdlih.sHtML

[S42] C++：继承与虚函数
来源：http://baike.zdbjq.cn/Article/details/gzrlbsxvx.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.zdbjq.cn/Article/details/grbhtjdmu.sHtML

[S43] C++：智能指针
来源：http://www.blog.fehbvm.com/Article/details/gnekcckcp.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.zdbjq.cn/Article/details/gijtnrmoh.sHtML

[S44] C++：引用传参
来源：http://www.m.share.hesvh.cn/Article/details/gxyugqpqa.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fehbvm.com/Article/details/gjnsguspj.sHtML

[S45] C++：lambda
来源：http://www.m.share.hesvh.cn/Article/details/gnwblrvde.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.zdbjq.cn/Article/details/gnkaxkmhr.sHtML

[S46] C++：函数模板
来源：http://www.blog.fehbvm.com/Article/details/gnfctvcde.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.zdbjq.cn/Article/details/ghbfwgwvj.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.hesvh.cn/Article/details/gyanyhkdk.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.zdbjq.cn/Article/details/gspfltrzf.sHtML

[S48] C++：逐行读文件
来源：http://www.share.fehbvm.com/Article/details/giqmrqtno.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://m.share.fehbvm.com/Article/details/ggujuqmoe.sHtML

while (std::getline(in, line)) { }
来源：http://3g.hesvh.cn/Article/details/glpqvaqem.sHtML

[S49] C++：写文件
来源：http://3g.zdbjq.cn/Article/details/gyybseepz.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.fehbvm.com/Article/details/gwukthdbx.sHtML

[S50] C++：格式化数字
来源：http://mobile.zdbjq.cn/Article/details/gltukuuke.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gbdzibgxq.sHtML

[S51] C++：显式类型转换
来源：http://www.share.hesvh.cn/Article/details/glpxolcwf.sHtML

static_cast<double>(a) / b
来源：http://www.share.hesvh.cn/Article/details/gaayhijmq.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.zdbjq.cn/Article/details/gpqogqnat.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.hesvh.cn/Article/details/grrbhsvom.sHtML

[S53] C++：移动语义
来源：http://read.share.zdbjq.cn/Article/details/goazyfgwk.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fehbvm.com/Article/details/gvaflsaku.sHtML

[S54] C++：异常处理
来源：http://baike.zdbjq.cn/Article/details/gkyjfeijp.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.hesvh.cn/Article/details/gqovoxssx.sHtML

[S55] C++：结构化绑定
来源：http://blog.fehbvm.com/Article/details/glwmblwqh.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.share.zdbjq.cn/Article/details/goahznmkc.sHtML

[S56] C++：optional
来源：http://blog.fehbvm.com/Article/details/geizzrehv.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://m.share.zdbjq.cn/Article/details/glohcvzuu.sHtML

[S57] C++：编译期常量
来源：http://mobile.hesvh.cn/Article/details/gvxddidat.sHtML

constexpr int N = 10;
来源：http://www.blog.fehbvm.com/Article/details/gprcopbpi.sHtML

[S58] C++：命名空间
来源：http://www.m.share.hesvh.cn/Article/details/gntzsthgb.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.zdbjq.cn/Article/details/gnaissryh.sHtML

[S59] C++：静态断言
来源：http://blog.fehbvm.com/Article/details/gjushtalz.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.hesvh.cn/Article/details/grydovixq.sHtML

[S60] C++：遍历并删除元素
来源：http://read.share.hesvh.cn/Article/details/gagkuzeri.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.zdbjq.cn/Article/details/gsbzsjlqv.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/giiftexmf.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.zdbjq.cn/Article/details/gmgwcqhph.sHtML

================================================================================
来源：http://read.share.fehbvm.com/Article/details/gpdqhnoiq.sHtML

[T01] Kotlin：Hello World
来源：http://wap.zdbjq.cn/Article/details/gtqanrdxa.sHtML

println("Hello")
来源：http://blog.hesvh.cn/Article/details/gljmpkdsc.sHtML

[T02] Kotlin：变量
来源：http://baike.hesvh.cn/Article/details/gyqeezhgp.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://m.share.fehbvm.com/Article/details/gxlrsvdur.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.hesvh.cn/Article/details/gmxcpnggx.sHtML

"值: $b"
来源：http://mobile.hesvh.cn/Article/details/gtzrsamtv.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fehbvm.com/Article/details/gbbvfpdjv.sHtML

val n: String? = null;  n?.length
来源：http://baike.hesvh.cn/Article/details/gxinghxkr.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.zdbjq.cn/Article/details/gekktzwki.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.zdbjq.cn/Article/details/gakydqghu.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fehbvm.com/Article/details/gmovhmcuc.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://m.share.zdbjq.cn/Article/details/gfyhyxybj.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.hesvh.cn/Article/details/gfkervvnv.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.zdbjq.cn/Article/details/gqwxyragz.sHtML

[T08] Kotlin：数据类
来源：http://www.share.hesvh.cn/Article/details/glodghewz.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.fehbvm.com/Article/details/gjfckcnvi.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.zdbjq.cn/Article/details/gjficzhpt.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fehbvm.com/Article/details/godegikzc.sHtML

[T10] Kotlin：默认参数
来源：http://baike.zdbjq.cn/Article/details/gkuqquhjx.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.hesvh.cn/Article/details/gjpbchijr.sHtML

[T11] Kotlin：协程
来源：http://read.share.hesvh.cn/Article/details/glzyaetds.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.zdbjq.cn/Article/details/gsfzvtydn.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.hesvh.cn/Article/details/gpvulyhxv.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.zdbjq.cn/Article/details/gkrzvhgjs.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.hesvh.cn/Article/details/gdjhwkufr.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.zdbjq.cn/Article/details/gudstdmjn.sHtML

[T14] Kotlin：循环
来源：http://blog.fehbvm.com/Article/details/gvionycyb.sHtML

for (i in 1..10) println(i)
来源：http://baike.fehbvm.com/Article/details/gtdqkrlzm.sHtML

[T15] Kotlin：接口
来源：http://wap.zdbjq.cn/Article/details/getqaxizg.sHtML

interface Shape { fun area(): Double }
来源：http://wap.fehbvm.com/Article/details/ggqugntks.sHtML

[T16] Swift：Hello World
来源：http://www.share.hesvh.cn/Article/details/gtpeorhmy.sHtML

print("Hello")
来源：http://mobile.hesvh.cn/Article/details/gfpcesjtm.sHtML

[T17] Swift：变量与常量
来源：http://read.share.zdbjq.cn/Article/details/gatipnzwo.sHtML

var a = 1;  let b = 2
来源：http://baike.fehbvm.com/Article/details/gupsdjldz.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gpegzsvte.sHtML

"值: \(b)"
来源：http://mobile.hesvh.cn/Article/details/guayfuyej.sHtML

[T19] Swift：可选绑定
来源：http://3g.zdbjq.cn/Article/details/gyuixdxgz.sHtML

if let n = opt { print(n) }
来源：http://wap.zdbjq.cn/Article/details/gnqoajqxy.sHtML

[T20] Swift：数组操作
来源：http://www.m.share.fehbvm.com/Article/details/gznslbkza.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.hesvh.cn/Article/details/glqoavvep.sHtML

[T21] Swift：遍历
来源：http://wap.zdbjq.cn/Article/details/gguopwvbb.sHtML

for x in a { print(x) }
来源：http://wap.fehbvm.com/Article/details/giwwwukkc.sHtML

[T22] Swift：字典
来源：http://blog.zdbjq.cn/Article/details/gfvgzstom.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gnktqqgcn.sHtML

[T23] Swift：函数
来源：http://www.m.share.hesvh.cn/Article/details/gupibqaue.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.zdbjq.cn/Article/details/gibevsvvf.sHtML

[T24] Swift：闭包
来源：http://blog.zdbjq.cn/Article/details/gdkifvgxw.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.hesvh.cn/Article/details/gmliorkgb.sHtML

[T25] Swift：结构体
来源：http://www.share.fehbvm.com/Article/details/gspilztff.sHtML

struct P { var x: Int }
来源：http://baike.hesvh.cn/Article/details/gcewohqcv.sHtML

[T26] Swift：类与重写
来源：http://read.share.fehbvm.com/Article/details/grcepnham.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.hesvh.cn/Article/details/gtwrztdlk.sHtML

[T27] Swift：错误处理
来源：http://baike.fehbvm.com/Article/details/guqkofool.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.zdbjq.cn/Article/details/gcirdoxne.sHtML

[T28] Swift：枚举
来源：http://wap.hesvh.cn/Article/details/gajaklkgz.sHtML

enum Color { case red, green }
来源：http://baike.fehbvm.com/Article/details/gidqcnnqg.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.zdbjq.cn/Article/details/grnvspqiv.sHtML

guard let x = opt else { return }
来源：http://wap.hesvh.cn/Article/details/gyqvdefvo.sHtML

[T30] Swift：协议
来源：http://wap.hesvh.cn/Article/details/ggspedrwj.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.hesvh.cn/Article/details/gptvldjcv.sHtML

[T31] Lua：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gjimxxccw.sHtML

print("Hello")
来源：http://wap.fehbvm.com/Article/details/gsbjthpwg.sHtML

[T32] Lua：局部变量
来源：http://read.share.fehbvm.com/Article/details/gfyuwxuho.sHtML

local a = 1
来源：http://wap.fehbvm.com/Article/details/gnqfpdpzw.sHtML

[T33] Lua：表（数组）
来源：http://baike.fehbvm.com/Article/details/gjschomjm.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.hesvh.cn/Article/details/giwxnsdok.sHtML

[T34] Lua：遍历表
来源：http://3g.hesvh.cn/Article/details/gdfpnzeog.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.hesvh.cn/Article/details/glyawuxyr.sHtML

[T35] Lua：字典表
来源：http://blog.fehbvm.com/Article/details/gidrhefth.sHtML

local d = { a = 1 };  d.b = 2
来源：http://m.share.hesvh.cn/Article/details/gcemejqij.sHtML

[T36] Lua：函数
来源：http://read.share.fehbvm.com/Article/details/gxfebrktp.sHtML

function add(a, b) return a + b end
来源：http://blog.fehbvm.com/Article/details/gkpvddpfb.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.zdbjq.cn/Article/details/gjlqdmpan.sHtML

"a" .. "b"
来源：http://www.m.share.zdbjq.cn/Article/details/gdxdgszfv.sHtML

[T38] Lua：条件
来源：http://www.m.share.zdbjq.cn/Article/details/gipqvdmmp.sHtML

if x > 0 then print("正") end
来源：http://www.share.fehbvm.com/Article/details/gwbfhuyei.sHtML

[T39] Lua：模式匹配
来源：http://www.share.zdbjq.cn/Article/details/gwwqiurhb.sHtML

string.find(s, "%d+")
来源：http://read.share.hesvh.cn/Article/details/gvynzlici.sHtML

[T40] Lua：元表
来源：http://www.share.fehbvm.com/Article/details/gayrxiuqn.sHtML

setmetatable({}, { __index = base })
来源：http://wap.zdbjq.cn/Article/details/gqmkvmnnx.sHtML

[T41] Perl：Hello World
来源：http://read.share.hesvh.cn/Article/details/gtgtvjvrc.sHtML

print "Hello\n";
来源：http://3g.zdbjq.cn/Article/details/gblbvxtkr.sHtML

[T42] Perl：变量类型
来源：http://baike.hesvh.cn/Article/details/gjdtlevfd.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.fehbvm.com/Article/details/gzspfvxiq.sHtML

[T43] Perl：字符串插值
来源：http://read.share.zdbjq.cn/Article/details/gowtyxljv.sHtML

"值: $a"
来源：http://3g.zdbjq.cn/Article/details/giwtwvxqy.sHtML

[T44] Perl：条件
来源：http://3g.hesvh.cn/Article/details/gsrukdrpf.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.zdbjq.cn/Article/details/gxjmqunsg.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.hesvh.cn/Article/details/gmqjpociu.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.fehbvm.com/Article/details/gebwrjwjb.sHtML

[T46] Perl：哈希操作
来源：http://mobile.fehbvm.com/Article/details/grusyoslb.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.hesvh.cn/Article/details/gvxftwzox.sHtML

[T47] Perl：正则捕获
来源：http://read.share.hesvh.cn/Article/details/ghnqgabuv.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.hesvh.cn/Article/details/gzqfcdzmr.sHtML

[T48] Perl：正则替换
来源：http://wap.zdbjq.cn/Article/details/gwjrzvttw.sHtML

$s =~ s/old/new/g;
来源：http://wap.zdbjq.cn/Article/details/gqmciovjb.sHtML

[T49] Perl：函数
来源：http://mobile.zdbjq.cn/Article/details/gyrpxplfh.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://3g.hesvh.cn/Article/details/gjhykltkf.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/grfgvndwm.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.m.share.fehbvm.com/Article/details/gnskiygyb.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://blog.zdbjq.cn/Article/details/gzpaxzljw.sHtML

[T51] Scala：Hello World
来源：http://www.share.fehbvm.com/Article/details/ghlmfgyqb.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/gubxwydzq.sHtML

[T52] Scala：变量
来源：http://3g.hesvh.cn/Article/details/gjnfuscvq.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gcxxdxuzk.sHtML

[T53] Scala：字符串插值
来源：http://3g.fehbvm.com/Article/details/gfigfxsoo.sHtML

s"值: $b"
来源：http://wap.fehbvm.com/Article/details/goqkstdge.sHtML

[T54] Scala：集合映射
来源：http://www.blog.hesvh.cn/Article/details/gacbdbzeh.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.fehbvm.com/Article/details/gfshhgwpb.sHtML

[T55] Scala：集合过滤
来源：http://wap.zdbjq.cn/Article/details/gkfbtgulk.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.fehbvm.com/Article/details/guxzmjmnz.sHtML

[T56] Scala：样例类
来源：http://www.m.share.zdbjq.cn/Article/details/gnhjqzjqm.sHtML

case class User(name: String, age: Int)
来源：http://3g.zdbjq.cn/Article/details/gmnojexrw.sHtML

[T57] Scala：模式匹配
来源：http://www.m.share.hesvh.cn/Article/details/gcogljcsb.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.hesvh.cn/Article/details/gpjhzsbwm.sHtML

[T58] Scala：函数定义
来源：http://m.share.zdbjq.cn/Article/details/gvgualkpp.sHtML


<!-- 参考信息 -->