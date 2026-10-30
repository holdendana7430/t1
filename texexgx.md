代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://www.blog.hesvh.cn/Article/details/gnkmiedgb.sHtML

[R52] 统计行数
来源：http://blog.hesvh.cn/Article/details/gxxoyvdnu.sHtML

wc -l a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gycxotwwr.sHtML

[R53] 查看文件头与实时尾
来源：http://www.m.share.hesvh.cn/Article/details/gvayneewy.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://read.share.hesvh.cn/Article/details/gcavfflih.sHtML

[R54] 比较两个文件
来源：http://www.blog.zdbjq.cn/Article/details/gsbktqpjf.sHtML

diff a.txt b.txt
来源：http://www.blog.zdbjq.cn/Article/details/gyumqiiil.sHtML

[R55] 压缩与解压
来源：http://wap.hesvh.cn/Article/details/gwzlwjtsb.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.hesvh.cn/Article/details/grrjbfxfa.sHtML

[R56] 远程拷贝
来源：http://baike.zdbjq.cn/Article/details/gjjmsidnk.sHtML

scp file user@host:/path/
来源：http://baike.zdbjq.cn/Article/details/gciadqddl.sHtML

[R57] 远程执行命令
来源：http://baike.zdbjq.cn/Article/details/gsoppcliv.sHtML

ssh user@host 'uptime'
来源：http://www.share.zdbjq.cn/Article/details/gyssjyvjx.sHtML

[R58] 下载文件
来源：http://baike.zdbjq.cn/Article/details/gfltawfxh.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.hesvh.cn/Article/details/grdinxcuq.sHtML

[R59] 发 POST JSON
来源：http://blog.hesvh.cn/Article/details/gioqozdcc.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.zdbjq.cn/Article/details/gtbyzqcya.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.hesvh.cn/Article/details/gjziofhtu.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://wap.fehbvm.com/Article/details/gpufmdqfk.sHtML

[R61] 磁盘占用
来源：http://baike.zdbjq.cn/Article/details/gqcmyftxh.sHtML

df -h;  du -sh *
来源：http://3g.zdbjq.cn/Article/details/gcucuifyb.sHtML

[R62] 找最占空间的文件
来源：http://mobile.fehbvm.com/Article/details/grasmyoem.sHtML

du -ah . | sort -rh | head -10
来源：http://read.share.zdbjq.cn/Article/details/grnvoevvu.sHtML

[R63] 内存与进程
来源：http://wap.hesvh.cn/Article/details/grqpufoss.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.hesvh.cn/Article/details/gnwaaryjp.sHtML

[R64] 结束进程
来源：http://read.share.hesvh.cn/Article/details/grmrfdaed.sHtML

kill -9 $(pgrep -f app.py)
来源：http://blog.zdbjq.cn/Article/details/gcnpkusyk.sHtML

[R65] 查看端口占用
来源：http://blog.hesvh.cn/Article/details/godsmzwjd.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mobile.zdbjq.cn/Article/details/gmngejqwv.sHtML

[R66] 定时任务
来源：http://baike.hesvh.cn/Article/details/gogtsjrhw.sHtML

crontab -e;  crontab -l
来源：http://mobile.fehbvm.com/Article/details/ghzbygokv.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fehbvm.com/Article/details/gbjtdsuza.sHtML

openssl rand -hex 16
来源：http://wap.fehbvm.com/Article/details/gzjuwdbgd.sHtML

[R68] 计算文件校验值
来源：http://baike.fehbvm.com/Article/details/gdwejlzcq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.fehbvm.com/Article/details/gtnaidqmv.sHtML

[R69] 生成随机密码
来源：http://wap.zdbjq.cn/Article/details/grejsuazo.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fehbvm.com/Article/details/gxrqvxnhp.sHtML

[R70] 时间戳与互转
来源：http://baike.zdbjq.cn/Article/details/gsbyuhvoh.sHtML

date +%s;  date -d @1700000000
来源：http://blog.hesvh.cn/Article/details/gylsgrozf.sHtML

[R71] 日期格式化
来源：http://m.share.hesvh.cn/Article/details/gnisryyow.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fehbvm.com/Article/details/glnttleep.sHtML

[R72] 等待端口就绪
来源：http://mobile.hesvh.cn/Article/details/gahgkxpdj.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.hesvh.cn/Article/details/gybsjpury.sHtML

[R73] 分割大日志
来源：http://m.share.zdbjq.cn/Article/details/gfzvtqyli.sHtML

split -l 1000 big.log part_
来源：http://baike.fehbvm.com/Article/details/gvezfqerh.sHtML

[R74] 批量重命名
来源：http://3g.hesvh.cn/Article/details/gfvbrvtus.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.share.hesvh.cn/Article/details/gvbblaycu.sHtML

[R75] 导出环境变量
来源：http://mobile.fehbvm.com/Article/details/gxmcetavh.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fehbvm.com/Article/details/gvcintnhg.sHtML

[R76] 使用临时文件
来源：http://3g.hesvh.cn/Article/details/gwfzikjsv.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/gmfgaswst.sHtML

[R77] 读取用户输入
来源：http://baike.fehbvm.com/Article/details/gbljluhvr.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fehbvm.com/Article/details/gqzvtzfia.sHtML

[R78] 交互式菜单
来源：http://www.m.share.zdbjq.cn/Article/details/gdwmgnciw.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.hesvh.cn/Article/details/gtwjjtwsx.sHtML

[R79] 解析命令行选项
来源：http://m.share.zdbjq.cn/Article/details/gwcboxvxa.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fehbvm.com/Article/details/gwnliiaxu.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.zdbjq.cn/Article/details/gxmbgfhqn.sHtML

time ./run.sh
来源：http://www.blog.zdbjq.cn/Article/details/gakylkqfi.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gyamqapxo.sHtML

S. C / C++ 专题
来源：http://read.share.hesvh.cn/Article/details/ggvosdcwg.sHtML

================================================================================
来源：http://blog.zdbjq.cn/Article/details/gbsqrxskm.sHtML

[S01] C：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gtgeohzeq.sHtML

#include <stdio.h>
来源：http://3g.zdbjq.cn/Article/details/ghuordaho.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.zdbjq.cn/Article/details/giectktmz.sHtML

[S02] C：变量与格式化输出
来源：http://blog.hesvh.cn/Article/details/gcrrfdkuz.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.hesvh.cn/Article/details/gtjnsyvsq.sHtML

[S03] C：读入整数
来源：http://blog.fehbvm.com/Article/details/gfgjdmcdn.sHtML

int x; scanf("%d", &x);
来源：http://wap.hesvh.cn/Article/details/gaeuoeauh.sHtML

[S04] C：字符串复制
来源：http://read.share.hesvh.cn/Article/details/gdzqnmttp.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fehbvm.com/Article/details/gvpleepjp.sHtML

[S05] C：字符串长度
来源：http://www.blog.zdbjq.cn/Article/details/gatdnzzck.sHtML

strlen(s)
来源：http://www.m.share.hesvh.cn/Article/details/ghykpfkni.sHtML

[S06] C：字符串比较
来源：http://3g.hesvh.cn/Article/details/gumbabtaa.sHtML

strcmp(a, b) == 0
来源：http://3g.hesvh.cn/Article/details/gryvnvolw.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fehbvm.com/Article/details/gelyseknc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.zdbjq.cn/Article/details/gfjsltjwv.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.hesvh.cn/Article/details/gkavkolkr.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://m.share.hesvh.cn/Article/details/gtmkklzdo.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fehbvm.com/Article/details/gfsiidmcy.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.hesvh.cn/Article/details/gudbcqnny.sHtML

[S10] C：指针与解引用
来源：http://mobile.zdbjq.cn/Article/details/gkyizerih.sHtML

int *p = &a;  *p = 5;
来源：http://blog.hesvh.cn/Article/details/gpjbyorfx.sHtML

[S11] C：逐行读文件
来源：http://www.share.hesvh.cn/Article/details/gkkdgkkzk.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fehbvm.com/Article/details/gqhddizqe.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fehbvm.com/Article/details/gsnmtyvwr.sHtML

fclose(f);
来源：http://3g.hesvh.cn/Article/details/giahxmqaz.sHtML

[S12] C：写文件
来源：http://baike.fehbvm.com/Article/details/gpcfclycw.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fehbvm.com/Article/details/godurrsyg.sHtML

[S13] C：宏定义
来源：http://baike.zdbjq.cn/Article/details/gyfsgqwkw.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.hesvh.cn/Article/details/gojiypstx.sHtML

[S14] C：枚举
来源：http://read.share.fehbvm.com/Article/details/ghznqpehj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.blog.fehbvm.com/Article/details/gpsfzpecf.sHtML

[S15] C：类型转换
来源：http://www.blog.zdbjq.cn/Article/details/gnisnhynb.sHtML

(double) a / b
来源：http://www.share.zdbjq.cn/Article/details/gawvsflrk.sHtML

[S16] C：位操作置位
来源：http://read.share.zdbjq.cn/Article/details/gxejbxadr.sHtML

x |= (1 << 3);
来源：http://mobile.hesvh.cn/Article/details/ghcqjaidr.sHtML

[S17] C：安全拼接字符串
来源：http://3g.hesvh.cn/Article/details/gmatfqhiv.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://3g.zdbjq.cn/Article/details/geuoetfda.sHtML

[S18] C：命令行参数
来源：http://www.share.fehbvm.com/Article/details/gmhsesltu.sHtML

int main(int argc, char **argv)
来源：http://read.share.fehbvm.com/Article/details/gbtfvncti.sHtML

[S19] C：快速排序
来源：http://wap.hesvh.cn/Article/details/glomxewra.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://blog.hesvh.cn/Article/details/gmjogtinm.sHtML

[S20] C：二分查找
来源：http://read.share.hesvh.cn/Article/details/guricpwpe.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.zdbjq.cn/Article/details/gyqigrboj.sHtML

[S21] C：字符类别判断
来源：http://3g.hesvh.cn/Article/details/gkfjmvkrz.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fehbvm.com/Article/details/gavbmcncq.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fehbvm.com/Article/details/gavvbnwsu.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fehbvm.com/Article/details/gnvwenstt.sHtML

[S23] C：随机数
来源：http://www.m.share.hesvh.cn/Article/details/gxyczwctt.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.hesvh.cn/Article/details/gauxfgksd.sHtML

[S24] C：获取本地时间
来源：http://mobile.fehbvm.com/Article/details/gfhfmugqg.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://3g.zdbjq.cn/Article/details/gyeuogeyo.sHtML

[S25] C：内存拷贝
来源：http://m.share.fehbvm.com/Article/details/ggjsplmzj.sHtML

memcpy(dst, src, n);
来源：http://www.share.zdbjq.cn/Article/details/ggyhajxbi.sHtML

[S26] C：内存清零
来源：http://3g.fehbvm.com/Article/details/gqyljfowh.sHtML

memset(a, 0, sizeof a);
来源：http://www.share.zdbjq.cn/Article/details/giddinlji.sHtML

[S27] C：定义常量
来源：http://mobile.zdbjq.cn/Article/details/ghshhphtf.sHtML

const double PI = 3.14159;
来源：http://wap.hesvh.cn/Article/details/giikddrzz.sHtML

[S28] C：静态变量
来源：http://www.m.share.fehbvm.com/Article/details/gbpaktgvq.sHtML

static int counter = 0;
来源：http://3g.zdbjq.cn/Article/details/gjerigybf.sHtML

[S29] C：变参函数
来源：http://mobile.fehbvm.com/Article/details/gnzdokysa.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fehbvm.com/Article/details/giujoshxg.sHtML

[S30] C：头文件保护
来源：http://mobile.zdbjq.cn/Article/details/gisubllgs.sHtML

#ifndef X_H
来源：http://m.share.zdbjq.cn/Article/details/golzfabfs.sHtML

#define X_H
来源：http://www.m.share.hesvh.cn/Article/details/gqghpyxhw.sHtML

#endif
来源：http://blog.fehbvm.com/Article/details/gdprcheab.sHtML

[S31] C++：Hello World
来源：http://wap.hesvh.cn/Article/details/gfcuoufgn.sHtML

#include <iostream>
来源：http://m.share.zdbjq.cn/Article/details/gjeeazlhh.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.hesvh.cn/Article/details/gbbhsvofo.sHtML

[S32] C++：字符串
来源：http://m.share.fehbvm.com/Article/details/gaufkuwnd.sHtML

std::string s = "hi";  s += "!";
来源：http://read.share.hesvh.cn/Article/details/gcngjtqie.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.zdbjq.cn/Article/details/ghawsbuwy.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.fehbvm.com/Article/details/gcreemeiy.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.zdbjq.cn/Article/details/gbbibscbc.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.hesvh.cn/Article/details/ggawuguhk.sHtML

[S35] C++：map
来源：http://m.share.zdbjq.cn/Article/details/gddkpcpuf.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mobile.zdbjq.cn/Article/details/gxtimfave.sHtML

[S36] C++：unordered_map
来源：http://read.share.hesvh.cn/Article/details/ggyfvyrqe.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.zdbjq.cn/Article/details/gvidbapdt.sHtML

[S37] C++：set
来源：http://mobile.hesvh.cn/Article/details/gyytgtwhp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.zdbjq.cn/Article/details/gflcwenzc.sHtML

[S38] C++：排序
来源：http://baike.hesvh.cn/Article/details/gpqrxrbjk.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.zdbjq.cn/Article/details/gzatjhqgb.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.fehbvm.com/Article/details/grzyruorg.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.fehbvm.com/Article/details/gftyxellk.sHtML

[S40] C++：查找元素
来源：http://www.blog.hesvh.cn/Article/details/gwkpprdfo.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.hesvh.cn/Article/details/gokkjthrb.sHtML

[S41] C++：类与构造函数
来源：http://m.share.hesvh.cn/Article/details/gcyexcocg.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.zdbjq.cn/Article/details/gcbzbsuye.sHtML

[S42] C++：继承与虚函数
来源：http://3g.zdbjq.cn/Article/details/gajprauen.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.zdbjq.cn/Article/details/grtkmjaxp.sHtML

[S43] C++：智能指针
来源：http://www.m.share.hesvh.cn/Article/details/ghhaymusa.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fehbvm.com/Article/details/ghfzawudb.sHtML

[S44] C++：引用传参
来源：http://wap.fehbvm.com/Article/details/ghzmsekne.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fehbvm.com/Article/details/gcersbvra.sHtML

[S45] C++：lambda
来源：http://3g.hesvh.cn/Article/details/ggrqtajky.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.fehbvm.com/Article/details/gfgcepixm.sHtML

[S46] C++：函数模板
来源：http://m.share.zdbjq.cn/Article/details/gjxaghjdt.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.zdbjq.cn/Article/details/ggdhqobqv.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.hesvh.cn/Article/details/gzgmfytof.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fehbvm.com/Article/details/gpssitwek.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/gneoxcmde.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.hesvh.cn/Article/details/guesufpct.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fehbvm.com/Article/details/gdotvrujq.sHtML

[S49] C++：写文件
来源：http://3g.fehbvm.com/Article/details/gfhrqhuxm.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.fehbvm.com/Article/details/gyiyijjof.sHtML

[S50] C++：格式化数字
来源：http://read.share.fehbvm.com/Article/details/gigdqqxnk.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gulykzxpa.sHtML

[S51] C++：显式类型转换
来源：http://www.blog.hesvh.cn/Article/details/gyjnxkxpi.sHtML

static_cast<double>(a) / b
来源：http://www.share.zdbjq.cn/Article/details/gqjgiaslt.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.zdbjq.cn/Article/details/gfuqgsuht.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fehbvm.com/Article/details/gvnoatvvr.sHtML

[S53] C++：移动语义
来源：http://www.share.hesvh.cn/Article/details/gdhdqzlzs.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fehbvm.com/Article/details/gpjvibkqc.sHtML

[S54] C++：异常处理
来源：http://blog.hesvh.cn/Article/details/gxbeyzrxj.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gilguqgpy.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.zdbjq.cn/Article/details/gmvseqjgq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.zdbjq.cn/Article/details/gsxlfdobq.sHtML

[S56] C++：optional
来源：http://read.share.hesvh.cn/Article/details/gbezfhwmh.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fehbvm.com/Article/details/gufkkpxxb.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fehbvm.com/Article/details/ganfrxtas.sHtML

constexpr int N = 10;
来源：http://wap.hesvh.cn/Article/details/gmuziksib.sHtML

[S58] C++：命名空间
来源：http://www.blog.fehbvm.com/Article/details/gqwlmicfj.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.hesvh.cn/Article/details/gmvxqtjzo.sHtML

[S59] C++：静态断言
来源：http://m.share.zdbjq.cn/Article/details/griwsoppp.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.zdbjq.cn/Article/details/gikqpkosy.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.zdbjq.cn/Article/details/guiorpndr.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.zdbjq.cn/Article/details/gamybrusp.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gjaensjgg.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.zdbjq.cn/Article/details/gglnairxr.sHtML

================================================================================
来源：http://wap.fehbvm.com/Article/details/gxcygrqob.sHtML

[T01] Kotlin：Hello World
来源：http://wap.hesvh.cn/Article/details/gdxerabtj.sHtML

println("Hello")
来源：http://wap.zdbjq.cn/Article/details/gwrrejbgy.sHtML

[T02] Kotlin：变量
来源：http://m.share.zdbjq.cn/Article/details/ghbqplytq.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.fehbvm.com/Article/details/gmalqtfna.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fehbvm.com/Article/details/gblsbqvxj.sHtML

"值: $b"
来源：http://m.share.hesvh.cn/Article/details/gflpjwahf.sHtML

[T04] Kotlin：空安全
来源：http://3g.fehbvm.com/Article/details/gkwbvgcyb.sHtML

val n: String? = null;  n?.length
来源：http://www.blog.fehbvm.com/Article/details/ggptynzun.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.zdbjq.cn/Article/details/gnbjbhvtj.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.hesvh.cn/Article/details/gjjkdoccj.sHtML

[T06] Kotlin：集合映射
来源：http://mobile.fehbvm.com/Article/details/gpbjfxtie.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.m.share.zdbjq.cn/Article/details/gmhjxhcgd.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.hesvh.cn/Article/details/gqhnqtcap.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.zdbjq.cn/Article/details/gvkffxmbw.sHtML

[T08] Kotlin：数据类
来源：http://wap.zdbjq.cn/Article/details/gtewvqvvm.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.zdbjq.cn/Article/details/gsamzdlof.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fehbvm.com/Article/details/gxinukoia.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.zdbjq.cn/Article/details/gcqzekpvu.sHtML

[T10] Kotlin：默认参数
来源：http://wap.zdbjq.cn/Article/details/gxywnlglu.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fehbvm.com/Article/details/gvooqhneu.sHtML

[T11] Kotlin：协程
来源：http://baike.fehbvm.com/Article/details/gngpuyjmm.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fehbvm.com/Article/details/gvammzpkk.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.zdbjq.cn/Article/details/gmilzbvuj.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.hesvh.cn/Article/details/gwcpccpmb.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.zdbjq.cn/Article/details/gslkufwop.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.hesvh.cn/Article/details/gkdcrjulk.sHtML

[T14] Kotlin：循环
来源：http://blog.fehbvm.com/Article/details/gktomprhe.sHtML

for (i in 1..10) println(i)
来源：http://baike.fehbvm.com/Article/details/gzeqtnhed.sHtML

[T15] Kotlin：接口
来源：http://3g.fehbvm.com/Article/details/gbheepupv.sHtML

interface Shape { fun area(): Double }
来源：http://blog.hesvh.cn/Article/details/gxlamospj.sHtML

[T16] Swift：Hello World
来源：http://wap.zdbjq.cn/Article/details/gcdwiaajb.sHtML

print("Hello")
来源：http://read.share.zdbjq.cn/Article/details/giluymjzy.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.hesvh.cn/Article/details/gjdtulkhi.sHtML

var a = 1;  let b = 2
来源：http://mobile.zdbjq.cn/Article/details/gvpidxoqs.sHtML

[T18] Swift：字符串插值
来源：http://blog.hesvh.cn/Article/details/giputojyy.sHtML

"值: \(b)"
来源：http://blog.hesvh.cn/Article/details/gujujngjx.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.zdbjq.cn/Article/details/glxuraqyq.sHtML

if let n = opt { print(n) }
来源：http://www.blog.zdbjq.cn/Article/details/gjwortmzm.sHtML

[T20] Swift：数组操作
来源：http://www.share.hesvh.cn/Article/details/gfgessbsl.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.fehbvm.com/Article/details/gkackwoat.sHtML

[T21] Swift：遍历
来源：http://www.blog.zdbjq.cn/Article/details/gemffjgxz.sHtML

for x in a { print(x) }
来源：http://mobile.hesvh.cn/Article/details/gthzauhvb.sHtML

[T22] Swift：字典
来源：http://blog.zdbjq.cn/Article/details/gzvrgzyvb.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.zdbjq.cn/Article/details/gzqlhzmjt.sHtML

[T23] Swift：函数
来源：http://mobile.zdbjq.cn/Article/details/gywpbhoru.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.hesvh.cn/Article/details/gxacpxger.sHtML

[T24] Swift：闭包
来源：http://read.share.zdbjq.cn/Article/details/guqaqswsz.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.hesvh.cn/Article/details/ghfbsbtig.sHtML

[T25] Swift：结构体
来源：http://mobile.hesvh.cn/Article/details/gunzzjqxg.sHtML

struct P { var x: Int }
来源：http://blog.zdbjq.cn/Article/details/gotfdvscu.sHtML

[T26] Swift：类与重写
来源：http://www.blog.zdbjq.cn/Article/details/gdxsobkzw.sHtML

class A: Base { override func f() {} }
来源：http://blog.fehbvm.com/Article/details/gzfvnwcle.sHtML

[T27] Swift：错误处理
来源：http://www.share.fehbvm.com/Article/details/gesnrkwtr.sHtML

do { try f() } catch { print(error) }
来源：http://baike.fehbvm.com/Article/details/gvcchiguk.sHtML

[T28] Swift：枚举
来源：http://mobile.zdbjq.cn/Article/details/glmzpgxpb.sHtML

enum Color { case red, green }
来源：http://www.blog.zdbjq.cn/Article/details/gqonytqgm.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.fehbvm.com/Article/details/gxgyaoapn.sHtML

guard let x = opt else { return }
来源：http://blog.fehbvm.com/Article/details/gvvywvpgy.sHtML

[T30] Swift：协议
来源：http://wap.zdbjq.cn/Article/details/gydoorskd.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.hesvh.cn/Article/details/gpumwwcyu.sHtML

[T31] Lua：Hello World
来源：http://www.share.fehbvm.com/Article/details/gyfcnflee.sHtML

print("Hello")
来源：http://www.blog.hesvh.cn/Article/details/gwdmabbsw.sHtML

[T32] Lua：局部变量
来源：http://m.share.zdbjq.cn/Article/details/grvwkkbgg.sHtML

local a = 1
来源：http://www.m.share.zdbjq.cn/Article/details/gdreiboxj.sHtML

[T33] Lua：表（数组）
来源：http://3g.hesvh.cn/Article/details/gvfiwpvkq.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.hesvh.cn/Article/details/gnsoqizud.sHtML

[T34] Lua：遍历表
来源：http://m.share.hesvh.cn/Article/details/gdtlhodra.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.zdbjq.cn/Article/details/ghuubotkt.sHtML

[T35] Lua：字典表
来源：http://www.m.share.fehbvm.com/Article/details/gvgxfoced.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.blog.fehbvm.com/Article/details/glyjghmpk.sHtML

[T36] Lua：函数
来源：http://read.share.fehbvm.com/Article/details/gspdymckp.sHtML

function add(a, b) return a + b end
来源：http://mobile.zdbjq.cn/Article/details/gbapclcxa.sHtML

[T37] Lua：字符串拼接
来源：http://wap.hesvh.cn/Article/details/gfuldjfot.sHtML

"a" .. "b"
来源：http://read.share.zdbjq.cn/Article/details/gpjnwqamx.sHtML

[T38] Lua：条件
来源：http://baike.fehbvm.com/Article/details/goaybsure.sHtML

if x > 0 then print("正") end
来源：http://blog.zdbjq.cn/Article/details/gsioaxahl.sHtML

[T39] Lua：模式匹配
来源：http://www.share.hesvh.cn/Article/details/gwpyxqrok.sHtML

string.find(s, "%d+")
来源：http://read.share.zdbjq.cn/Article/details/gnsebdmhu.sHtML

[T40] Lua：元表
来源：http://baike.zdbjq.cn/Article/details/gmopkqiuj.sHtML

setmetatable({}, { __index = base })
来源：http://baike.hesvh.cn/Article/details/gleukpcsd.sHtML

[T41] Perl：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gtxayzard.sHtML

print "Hello\n";
来源：http://wap.fehbvm.com/Article/details/guqeefcoi.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.hesvh.cn/Article/details/gfblyuayc.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://baike.zdbjq.cn/Article/details/gyyjlmfzu.sHtML

[T43] Perl：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gwrktsybj.sHtML

"值: $a"
来源：http://baike.fehbvm.com/Article/details/gvhsmyttm.sHtML

[T44] Perl：条件
来源：http://3g.hesvh.cn/Article/details/gycaekqit.sHtML

if ($a > 0) { print "正"; }
来源：http://3g.zdbjq.cn/Article/details/gmdspvfib.sHtML

[T45] Perl：数组遍历
来源：http://baike.zdbjq.cn/Article/details/gqaxjhzeb.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.fehbvm.com/Article/details/gvrhhkaic.sHtML

[T46] Perl：哈希操作
来源：http://blog.zdbjq.cn/Article/details/gpviafowc.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.hesvh.cn/Article/details/ghwghffqb.sHtML

[T47] Perl：正则捕获
来源：http://baike.fehbvm.com/Article/details/gwbecgdag.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.fehbvm.com/Article/details/gljngufld.sHtML

[T48] Perl：正则替换
来源：http://www.blog.hesvh.cn/Article/details/gjinfybfs.sHtML

$s =~ s/old/new/g;
来源：http://blog.zdbjq.cn/Article/details/gesnkilsf.sHtML

[T49] Perl：函数
来源：http://read.share.fehbvm.com/Article/details/gfkyacwjk.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.fehbvm.com/Article/details/goiaazldm.sHtML

[T50] Perl：逐行读文件
来源：http://www.share.zdbjq.cn/Article/details/gjuzxmoho.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.zdbjq.cn/Article/details/gsylarndi.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.fehbvm.com/Article/details/gbjnxvpwy.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gazbxzdbw.sHtML

println("Hello")
来源：http://m.share.hesvh.cn/Article/details/gsvzqwfjm.sHtML

[T52] Scala：变量
来源：http://wap.fehbvm.com/Article/details/gujdvtvvm.sHtML

val a = 1;  var b = 2
来源：http://read.share.hesvh.cn/Article/details/gktzzjgpq.sHtML

[T53] Scala：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gqtbapfdl.sHtML

s"值: $b"
来源：http://mobile.hesvh.cn/Article/details/gjhnhdehl.sHtML

[T54] Scala：集合映射
来源：http://blog.fehbvm.com/Article/details/gpnrfhuui.sHtML


<!-- 参考信息 -->