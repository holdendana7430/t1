代发 wailian999

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghalercsx.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.share.fanxiaobao.xyz/Article/details/gwsdxkfph.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fanxiaobao.xyz/Article/details/grpasenkb.sHtML

[R61] 磁盘占用
来源：http://www.share.fanxiaobao.xyz/Article/details/gkhzqxbla.sHtML

df -h;  du -sh *
来源：http://baike.fanxiaobao.xyz/Article/details/gkijtvpmm.sHtML

[R62] 找最占空间的文件
来源：http://3g.fanxiaobao.xyz/Article/details/giqcbgslr.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gazrlvowg.sHtML

[R63] 内存与进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcbyfauhj.sHtML

free -h;  ps aux | grep nginx
来源：http://www.share.fanxiaobao.xyz/Article/details/gnxwbuvhf.sHtML

[R64] 结束进程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkbnbyzrg.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.fanxiaobao.xyz/Article/details/gjusdycgl.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcxcslerk.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://read.share.fanxiaobao.xyz/Article/details/gkppltgpo.sHtML

[R66] 定时任务
来源：http://wap.fanxiaobao.xyz/Article/details/gbdolxphl.sHtML

crontab -e;  crontab -l
来源：http://wap.fanxiaobao.xyz/Article/details/gleqaihhc.sHtML

[R67] 生成随机十六进制串
来源：http://baike.fanxiaobao.xyz/Article/details/grdwtubnk.sHtML

openssl rand -hex 16
来源：http://m.share.fanxiaobao.xyz/Article/details/gkdpsymdv.sHtML

[R68] 计算文件校验值
来源：http://read.share.fanxiaobao.xyz/Article/details/gqsvqyhsj.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://mobile.fanxiaobao.xyz/Article/details/gbrxqzzid.sHtML

[R69] 生成随机密码
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtillhjed.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwrnmgmfc.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsfsksrcu.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fanxiaobao.xyz/Article/details/gxasbvckd.sHtML

[R71] 日期格式化
来源：http://3g.fanxiaobao.xyz/Article/details/ghtxaeozs.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjjqmiahq.sHtML

[R72] 等待端口就绪
来源：http://blog.fanxiaobao.xyz/Article/details/gzsommqxl.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gskjrqsvg.sHtML

[R73] 分割大日志
来源：http://mobile.fanxiaobao.xyz/Article/details/geykfufno.sHtML

split -l 1000 big.log part_
来源：http://m.share.fanxiaobao.xyz/Article/details/geelrsaoj.sHtML

[R74] 批量重命名
来源：http://www.share.fanxiaobao.xyz/Article/details/gfvjasnck.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gignwolke.sHtML

[R75] 导出环境变量
来源：http://baike.fanxiaobao.xyz/Article/details/guywyhcdk.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://wap.fanxiaobao.xyz/Article/details/gpkfocidv.sHtML

[R76] 使用临时文件
来源：http://www.share.fanxiaobao.xyz/Article/details/grzcwoeuq.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fanxiaobao.xyz/Article/details/gnktzgegl.sHtML

[R77] 读取用户输入
来源：http://baike.fanxiaobao.xyz/Article/details/gfxgktahc.sHtML

read -rp "请输入: " ans
来源：http://mobile.fanxiaobao.xyz/Article/details/giepeodbu.sHtML

[R78] 交互式菜单
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsmxxauga.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gjhfjztou.sHtML

[R79] 解析命令行选项
来源：http://baike.fanxiaobao.xyz/Article/details/gnsnkmabs.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fanxiaobao.xyz/Article/details/gdraqjiqc.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.fanxiaobao.xyz/Article/details/gogieekdp.sHtML

time ./run.sh
来源：http://blog.fanxiaobao.xyz/Article/details/giommfafw.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gwrvtfkxt.sHtML

S. C / C++ 专题
来源：http://3g.fanxiaobao.xyz/Article/details/gwfklbizm.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gchilyxfp.sHtML

[S01] C：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gblfaiscx.sHtML

#include <stdio.h>
来源：http://www.share.fanxiaobao.xyz/Article/details/gyzttfpsr.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fanxiaobao.xyz/Article/details/guodtccox.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsncjthvd.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.fanxiaobao.xyz/Article/details/gbvrykoxi.sHtML

[S03] C：读入整数
来源：http://baike.fanxiaobao.xyz/Article/details/gdkmqwogv.sHtML

int x; scanf("%d", &x);
来源：http://mobile.fanxiaobao.xyz/Article/details/glfwpflzy.sHtML

[S04] C：字符串复制
来源：http://m.share.fanxiaobao.xyz/Article/details/gozpypvqp.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fanxiaobao.xyz/Article/details/gzgbindac.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnihzdzec.sHtML

strlen(s)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvoyzqchy.sHtML

[S06] C：字符串比较
来源：http://3g.fanxiaobao.xyz/Article/details/gjhzzuzwd.sHtML

strcmp(a, b) == 0
来源：http://wap.fanxiaobao.xyz/Article/details/geinfjmor.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fanxiaobao.xyz/Article/details/gnliejhyr.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://blog.fanxiaobao.xyz/Article/details/grcorhupi.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.fanxiaobao.xyz/Article/details/gxwoxynky.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fanxiaobao.xyz/Article/details/gmylzlmvk.sHtML

[S09] C：结构体定义与初始化
来源：http://mobile.fanxiaobao.xyz/Article/details/gmwptptwr.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://wap.fanxiaobao.xyz/Article/details/gxktzikjk.sHtML

[S10] C：指针与解引用
来源：http://www.share.fanxiaobao.xyz/Article/details/gjmynwjty.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/grcsnswgg.sHtML

[S11] C：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/grxavofqy.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fanxiaobao.xyz/Article/details/gsgqfyuuh.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxnacneab.sHtML

fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gkciedigy.sHtML

[S12] C：写文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gtffcrxbf.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.fanxiaobao.xyz/Article/details/gpifxqfwo.sHtML

[S13] C：宏定义
来源：http://blog.fanxiaobao.xyz/Article/details/glztodnhk.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fanxiaobao.xyz/Article/details/ggrqqkuwb.sHtML

[S14] C：枚举
来源：http://mobile.fanxiaobao.xyz/Article/details/gqvqoomet.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fanxiaobao.xyz/Article/details/gtdxawxma.sHtML

[S15] C：类型转换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvjnvgaqy.sHtML

(double) a / b
来源：http://3g.fanxiaobao.xyz/Article/details/gxktwhldv.sHtML

[S16] C：位操作置位
来源：http://3g.fanxiaobao.xyz/Article/details/goologyov.sHtML

x |= (1 << 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/ggafndpez.sHtML

[S17] C：安全拼接字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gbjhajeii.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fanxiaobao.xyz/Article/details/gojhnpvsx.sHtML

[S18] C：命令行参数
来源：http://blog.fanxiaobao.xyz/Article/details/gtkkxjaeb.sHtML

int main(int argc, char **argv)
来源：http://wap.fanxiaobao.xyz/Article/details/gmexbozrj.sHtML

[S19] C：快速排序
来源：http://wap.fanxiaobao.xyz/Article/details/gehohjcgw.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvqeuwuqy.sHtML

[S20] C：二分查找
来源：http://3g.fanxiaobao.xyz/Article/details/goeaahemv.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvpzkcvpp.sHtML

[S21] C：字符类别判断
来源：http://m.share.fanxiaobao.xyz/Article/details/gnmuttyeu.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.fanxiaobao.xyz/Article/details/guinsfqes.sHtML

[S22] C：字符串转数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gwimfdxsr.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fanxiaobao.xyz/Article/details/glwugbfky.sHtML

[S23] C：随机数
来源：http://wap.fanxiaobao.xyz/Article/details/gssiixwxl.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fanxiaobao.xyz/Article/details/gdmmtaxcn.sHtML

[S24] C：获取本地时间
来源：http://baike.fanxiaobao.xyz/Article/details/gmckoehxs.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wap.fanxiaobao.xyz/Article/details/gmkurrubu.sHtML

[S25] C：内存拷贝
来源：http://baike.fanxiaobao.xyz/Article/details/gfrhrjsik.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gexqicmsd.sHtML

[S26] C：内存清零
来源：http://m.share.fanxiaobao.xyz/Article/details/gshqbhbdj.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fanxiaobao.xyz/Article/details/gtlrxvljd.sHtML

[S27] C：定义常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwlxvrisv.sHtML

const double PI = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gjvnwnljn.sHtML

[S28] C：静态变量
来源：http://read.share.fanxiaobao.xyz/Article/details/giakmgjsj.sHtML

static int counter = 0;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtplytzro.sHtML

[S29] C：变参函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gesnrrnoo.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://blog.fanxiaobao.xyz/Article/details/gdginspns.sHtML

[S30] C：头文件保护
来源：http://blog.fanxiaobao.xyz/Article/details/gfmnuyfib.sHtML

#ifndef X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gzicqprvb.sHtML

#define X_H
来源：http://m.share.fanxiaobao.xyz/Article/details/glfgbeaaz.sHtML

#endif
来源：http://www.share.fanxiaobao.xyz/Article/details/gmfxmhjxk.sHtML

[S31] C++：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gsfhgicsq.sHtML

#include <iostream>
来源：http://blog.fanxiaobao.xyz/Article/details/gvdobyltq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fanxiaobao.xyz/Article/details/gwkrwxwsd.sHtML

[S32] C++：字符串
来源：http://m.share.fanxiaobao.xyz/Article/details/gnmwsenoj.sHtML

std::string s = "hi";  s += "!";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmgaeprjl.sHtML

[S33] C++：vector 增删
来源：http://read.share.fanxiaobao.xyz/Article/details/goarpfkpf.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqdpjylun.sHtML

[S34] C++：遍历 vector
来源：http://wap.fanxiaobao.xyz/Article/details/gtkvtxqmf.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gozkbpuaw.sHtML

[S35] C++：map
来源：http://www.blog.fanxiaobao.xyz/Article/details/godnnttnp.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fanxiaobao.xyz/Article/details/gltslumys.sHtML

[S36] C++：unordered_map
来源：http://m.share.fanxiaobao.xyz/Article/details/gwqfdcemo.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/glykziqyz.sHtML

[S37] C++：set
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqcpmliki.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gkxodkglq.sHtML

[S38] C++：排序
来源：http://blog.fanxiaobao.xyz/Article/details/gdhxhixva.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fanxiaobao.xyz/Article/details/gumxorwif.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fanxiaobao.xyz/Article/details/gczbssjfo.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvjpceddp.sHtML

[S40] C++：查找元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gadkzpnpc.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gcuxvajnt.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvjdlrvpb.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://3g.fanxiaobao.xyz/Article/details/gclihlkzv.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fanxiaobao.xyz/Article/details/gqnxwnqtx.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fanxiaobao.xyz/Article/details/gfbxuviwg.sHtML

[S43] C++：智能指针
来源：http://wap.fanxiaobao.xyz/Article/details/gpvpooqsa.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fanxiaobao.xyz/Article/details/gvedhlevj.sHtML

[S44] C++：引用传参
来源：http://mobile.fanxiaobao.xyz/Article/details/gnuonmuod.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvchiddsv.sHtML

[S45] C++：lambda
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggmqpiixj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fanxiaobao.xyz/Article/details/gemwwdaza.sHtML

[S46] C++：函数模板
来源：http://read.share.fanxiaobao.xyz/Article/details/gdysfrbnr.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gileqljsn.sHtML

[S47] C++：结构化绑定遍历
来源：http://3g.fanxiaobao.xyz/Article/details/ggbionbpm.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gmtcolmuw.sHtML

[S48] C++：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/gukfxbkwp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fanxiaobao.xyz/Article/details/groiyjnhn.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fanxiaobao.xyz/Article/details/gytcahlzz.sHtML

[S49] C++：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxqahpidq.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.blog.fanxiaobao.xyz/Article/details/govdvgzdz.sHtML

[S50] C++：格式化数字
来源：http://read.share.fanxiaobao.xyz/Article/details/ghwllkrbm.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fanxiaobao.xyz/Article/details/gptrayxih.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gaglhyutj.sHtML

static_cast<double>(a) / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ganuhsdwt.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fanxiaobao.xyz/Article/details/ghzcehlec.sHtML

int size() const noexcept { return n_; }
来源：http://3g.fanxiaobao.xyz/Article/details/gsyhxetvi.sHtML

[S53] C++：移动语义
来源：http://baike.fanxiaobao.xyz/Article/details/getrtqvfg.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gljqifylb.sHtML

[S54] C++：异常处理
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzsqzgiho.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gztvtoyji.sHtML

[S55] C++：结构化绑定
来源：http://wap.fanxiaobao.xyz/Article/details/gaysucavu.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giyxfzuxk.sHtML

[S56] C++：optional
来源：http://www.share.fanxiaobao.xyz/Article/details/gozaxsgzl.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fanxiaobao.xyz/Article/details/gipcfdakx.sHtML

[S57] C++：编译期常量
来源：http://mobile.fanxiaobao.xyz/Article/details/geeudlymi.sHtML

constexpr int N = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/ggojkphls.sHtML

[S58] C++：命名空间
来源：http://blog.fanxiaobao.xyz/Article/details/gcjgthomj.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fanxiaobao.xyz/Article/details/glfqvnaal.sHtML

[S59] C++：静态断言
来源：http://baike.fanxiaobao.xyz/Article/details/gwvthftas.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.fanxiaobao.xyz/Article/details/gdhqwfhgb.sHtML

[S60] C++：遍历并删除元素
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqsyfrimf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/gqudlkpan.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/ghjdygywg.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gihwjnksy.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gtlerzjnl.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggwqjmecv.sHtML

println("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/glstmswvv.sHtML

[T02] Kotlin：变量
来源：http://wap.fanxiaobao.xyz/Article/details/gmtuarisb.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gldppkexa.sHtML

[T03] Kotlin：字符串模板
来源：http://blog.fanxiaobao.xyz/Article/details/gdydpfpdj.sHtML

"值: $b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gwajjxnnp.sHtML

[T04] Kotlin：空安全
来源：http://mobile.fanxiaobao.xyz/Article/details/gnogbpftk.sHtML

val n: String? = null;  n?.length
来源：http://3g.fanxiaobao.xyz/Article/details/gubfxrsrq.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gsaugfits.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fanxiaobao.xyz/Article/details/gbjfmrqmy.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fanxiaobao.xyz/Article/details/gmxwksoji.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gqmrztljt.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gmlrtfdok.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/guigqetjs.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gelgiredg.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fanxiaobao.xyz/Article/details/gytvwcykb.sHtML

[T09] Kotlin：扩展函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmiurfexb.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ginncymnb.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gzhvzzisl.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.fanxiaobao.xyz/Article/details/gyjxfgplz.sHtML

[T11] Kotlin：协程
来源：http://wap.fanxiaobao.xyz/Article/details/ghayajxqm.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.share.fanxiaobao.xyz/Article/details/gkzyyvbue.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fanxiaobao.xyz/Article/details/gabpmxtdp.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.fanxiaobao.xyz/Article/details/gtsqjszrz.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.fanxiaobao.xyz/Article/details/goqmcgvff.sHtML

val m = mapOf("a" to 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gzpnfzutm.sHtML

[T14] Kotlin：循环
来源：http://baike.fanxiaobao.xyz/Article/details/gnzuxzyjm.sHtML

for (i in 1..10) println(i)
来源：http://blog.fanxiaobao.xyz/Article/details/gikpagijl.sHtML

[T15] Kotlin：接口
来源：http://blog.fanxiaobao.xyz/Article/details/gyfinspmf.sHtML

interface Shape { fun area(): Double }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzvynycxe.sHtML

[T16] Swift：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gwmfjpdep.sHtML

print("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gmhvpjldz.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gfsxgtqzj.sHtML

var a = 1;  let b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gxqcifhur.sHtML

[T18] Swift：字符串插值
来源：http://www.blog.fanxiaobao.xyz/Article/details/gesmlmfmf.sHtML

"值: \(b)"
来源：http://www.share.fanxiaobao.xyz/Article/details/gqxyaqgph.sHtML

[T19] Swift：可选绑定
来源：http://blog.fanxiaobao.xyz/Article/details/gpozxkjad.sHtML

if let n = opt { print(n) }
来源：http://www.share.fanxiaobao.xyz/Article/details/gxsbsujob.sHtML

[T20] Swift：数组操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gyhjoztoo.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://baike.fanxiaobao.xyz/Article/details/gzhufnvef.sHtML

[T21] Swift：遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvnluvsnn.sHtML

for x in a { print(x) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtdxsqaax.sHtML

[T22] Swift：字典
来源：http://www.share.fanxiaobao.xyz/Article/details/gjtfpefvx.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gnzrkujpg.sHtML

[T23] Swift：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gjayynwzm.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcwnyvqjm.sHtML

[T24] Swift：闭包
来源：http://m.share.fanxiaobao.xyz/Article/details/gztxtegwm.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.fanxiaobao.xyz/Article/details/gudxkazpg.sHtML

[T25] Swift：结构体
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbhbtdqit.sHtML

struct P { var x: Int }
来源：http://wap.fanxiaobao.xyz/Article/details/gzdkdzqee.sHtML

[T26] Swift：类与重写
来源：http://3g.fanxiaobao.xyz/Article/details/gjemzhpsr.sHtML

class A: Base { override func f() {} }
来源：http://3g.fanxiaobao.xyz/Article/details/gorbwkkjz.sHtML

[T27] Swift：错误处理
来源：http://m.share.fanxiaobao.xyz/Article/details/gbksbbdny.sHtML

do { try f() } catch { print(error) }
来源：http://mobile.fanxiaobao.xyz/Article/details/gryfhxvnb.sHtML

[T28] Swift：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggwcfnpit.sHtML

enum Color { case red, green }
来源：http://3g.fanxiaobao.xyz/Article/details/gbigoeubu.sHtML

[T29] Swift：guard 提前返回
来源：http://read.share.fanxiaobao.xyz/Article/details/gtwvojbfn.sHtML

guard let x = opt else { return }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gefrsoydn.sHtML

[T30] Swift：协议
来源：http://read.share.fanxiaobao.xyz/Article/details/gzzagpfyx.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.fanxiaobao.xyz/Article/details/gdyhrxqnd.sHtML

[T31] Lua：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/glxgwebom.sHtML

print("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/ggngmxsny.sHtML

[T32] Lua：局部变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gwmacvlug.sHtML

local a = 1
来源：http://www.share.fanxiaobao.xyz/Article/details/goxtzgoss.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcfupbmpr.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.fanxiaobao.xyz/Article/details/grwubkxoy.sHtML

[T34] Lua：遍历表
来源：http://read.share.fanxiaobao.xyz/Article/details/gpiewjusa.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.fanxiaobao.xyz/Article/details/gkwlxthqq.sHtML

[T35] Lua：字典表
来源：http://blog.fanxiaobao.xyz/Article/details/gkqbvbkzf.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/glvoikzyh.sHtML

[T36] Lua：函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gwcyutwoo.sHtML

function add(a, b) return a + b end
来源：http://wap.fanxiaobao.xyz/Article/details/gyykbduvc.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.fanxiaobao.xyz/Article/details/ghhjdxeqb.sHtML

"a" .. "b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gznbwgczn.sHtML

[T38] Lua：条件
来源：http://www.share.fanxiaobao.xyz/Article/details/gqgsifrbc.sHtML

if x > 0 then print("正") end
来源：http://www.share.fanxiaobao.xyz/Article/details/goxpwhijt.sHtML

[T39] Lua：模式匹配
来源：http://baike.fanxiaobao.xyz/Article/details/gsnpuzdoo.sHtML

string.find(s, "%d+")
来源：http://www.share.fanxiaobao.xyz/Article/details/gibgtjpzb.sHtML

[T40] Lua：元表
来源：http://wap.fanxiaobao.xyz/Article/details/gxcjggdhp.sHtML

setmetatable({}, { __index = base })
来源：http://mobile.fanxiaobao.xyz/Article/details/gnyjnkvcs.sHtML

[T41] Perl：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/glrigffmg.sHtML

print "Hello\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/gqjwwdwym.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfsqfhugj.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.fanxiaobao.xyz/Article/details/glbndxeqm.sHtML

[T43] Perl：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gsquslqax.sHtML

"值: $a"
来源：http://baike.fanxiaobao.xyz/Article/details/geitthwns.sHtML

[T44] Perl：条件
来源：http://3g.fanxiaobao.xyz/Article/details/gxxijenpu.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/glesbfode.sHtML

[T45] Perl：数组遍历
来源：http://3g.fanxiaobao.xyz/Article/details/grpqakmpv.sHtML

for my $x (@arr) { print $x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gltteqztu.sHtML

[T46] Perl：哈希操作
来源：http://www.share.fanxiaobao.xyz/Article/details/ggkaeyikn.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gimndqets.sHtML

[T47] Perl：正则捕获
来源：http://m.share.fanxiaobao.xyz/Article/details/gxeuveikh.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://3g.fanxiaobao.xyz/Article/details/glccnyrnb.sHtML

[T48] Perl：正则替换
来源：http://wap.fanxiaobao.xyz/Article/details/gxyrkzecu.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gftowfswj.sHtML

[T49] Perl：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/giexiphkj.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://blog.fanxiaobao.xyz/Article/details/gojdhpmvn.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpgvlxuyp.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.fanxiaobao.xyz/Article/details/ginhwvfgn.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggaquhdox.sHtML

[T51] Scala：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gfmhlustv.sHtML

println("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gwukaswkr.sHtML

[T52] Scala：变量
来源：http://3g.fanxiaobao.xyz/Article/details/goemnjnmr.sHtML

val a = 1;  var b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gazzbswhb.sHtML

[T53] Scala：字符串插值
来源：http://www.share.fanxiaobao.xyz/Article/details/gcjfgttft.sHtML

s"值: $b"
来源：http://blog.fanxiaobao.xyz/Article/details/gqgasnbqq.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwuyphwfh.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://read.share.fanxiaobao.xyz/Article/details/gpqucrudi.sHtML

[T55] Scala：集合过滤
来源：http://blog.fanxiaobao.xyz/Article/details/gmoijxnjx.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://baike.fanxiaobao.xyz/Article/details/gzzdvxahx.sHtML

[T56] Scala：样例类
来源：http://baike.fanxiaobao.xyz/Article/details/gtvbybrde.sHtML

case class User(name: String, age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/gwhkjcghz.sHtML

[T57] Scala：模式匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gwufmwqqn.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqtnpubln.sHtML

[T58] Scala：函数定义
来源：http://wap.fanxiaobao.xyz/Article/details/geafhtcpm.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://m.share.fanxiaobao.xyz/Article/details/gjxtfnlca.sHtML

[T59] Scala：循环
来源：http://read.share.fanxiaobao.xyz/Article/details/glrvgynwn.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/gcfailyam.sHtML

[T60] Scala：折叠
来源：http://blog.fanxiaobao.xyz/Article/details/gsivxoxrx.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wap.fanxiaobao.xyz/Article/details/gujkotjzd.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqlrjlgbt.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gtcpazamy.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gobxyjjdt.sHtML


<!-- 参考信息 -->