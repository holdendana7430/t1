代发 wailian999

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.fanxiaobao.xyz/Article/details/gzdltvvqx.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gnkffvnhv.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwuspovch.sHtML

[R61] 磁盘占用
来源：http://blog.fanxiaobao.xyz/Article/details/gthbflkxd.sHtML

df -h;  du -sh *
来源：http://3g.fanxiaobao.xyz/Article/details/gsmmxdkyw.sHtML

[R62] 找最占空间的文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gykkzovzy.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.fanxiaobao.xyz/Article/details/gzgvwvpbc.sHtML

[R63] 内存与进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gjhbhezwh.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fanxiaobao.xyz/Article/details/glxgglmpn.sHtML

[R64] 结束进程
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyazucgsw.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fanxiaobao.xyz/Article/details/gyhbkslft.sHtML

[R65] 查看端口占用
来源：http://3g.fanxiaobao.xyz/Article/details/gdsnoeecg.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.fanxiaobao.xyz/Article/details/gwbwulwgx.sHtML

[R66] 定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gjxdalcxg.sHtML

crontab -e;  crontab -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gepedjscm.sHtML

[R67] 生成随机十六进制串
来源：http://www.share.fanxiaobao.xyz/Article/details/gttzfchnf.sHtML

openssl rand -hex 16
来源：http://mobile.fanxiaobao.xyz/Article/details/gpcesjbqh.sHtML

[R68] 计算文件校验值
来源：http://baike.fanxiaobao.xyz/Article/details/gjtfbqsxp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.fanxiaobao.xyz/Article/details/gjpxbhswh.sHtML

[R69] 生成随机密码
来源：http://3g.fanxiaobao.xyz/Article/details/gyqfyvxff.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.share.fanxiaobao.xyz/Article/details/ggnvxbhxb.sHtML

[R70] 时间戳与互转
来源：http://baike.fanxiaobao.xyz/Article/details/ggluwavpp.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fanxiaobao.xyz/Article/details/gneuekczg.sHtML

[R71] 日期格式化
来源：http://blog.fanxiaobao.xyz/Article/details/gxzdnonjv.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtnctyclh.sHtML

[R72] 等待端口就绪
来源：http://read.share.fanxiaobao.xyz/Article/details/gfkszbmbg.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjnolycya.sHtML

[R73] 分割大日志
来源：http://3g.fanxiaobao.xyz/Article/details/gbmcsdlls.sHtML

split -l 1000 big.log part_
来源：http://read.share.fanxiaobao.xyz/Article/details/ghsxvvots.sHtML

[R74] 批量重命名
来源：http://3g.fanxiaobao.xyz/Article/details/ginajyrjm.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/grenvgyqf.sHtML

[R75] 导出环境变量
来源：http://blog.fanxiaobao.xyz/Article/details/glamzsaza.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fanxiaobao.xyz/Article/details/gyofjaxeh.sHtML

[R76] 使用临时文件
来源：http://mobile.fanxiaobao.xyz/Article/details/ghjptlnnz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gvyyulhut.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glpglylff.sHtML

read -rp "请输入: " ans
来源：http://blog.fanxiaobao.xyz/Article/details/gkvurphgt.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gktqjvmqx.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkykeljnk.sHtML

[R79] 解析命令行选项
来源：http://baike.fanxiaobao.xyz/Article/details/gwpjqgmkg.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fanxiaobao.xyz/Article/details/gmbflmnph.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjyzogqcz.sHtML

time ./run.sh
来源：http://3g.fanxiaobao.xyz/Article/details/gfoqqsgwr.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gdmhsqmyu.sHtML

S. C / C++ 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/gmjcefzmw.sHtML

================================================================================
来源：http://blog.fanxiaobao.xyz/Article/details/gzsmupdfu.sHtML

[S01] C：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gatgfehkk.sHtML

#include <stdio.h>
来源：http://blog.fanxiaobao.xyz/Article/details/gdsfgryii.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbakocnss.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fanxiaobao.xyz/Article/details/gakkzdinw.sHtML

int a = 10; printf("%d\n", a);
来源：http://3g.fanxiaobao.xyz/Article/details/gjpblunmh.sHtML

[S03] C：读入整数
来源：http://www.share.fanxiaobao.xyz/Article/details/gnddgumga.sHtML

int x; scanf("%d", &x);
来源：http://blog.fanxiaobao.xyz/Article/details/gvxbzxunu.sHtML

[S04] C：字符串复制
来源：http://baike.fanxiaobao.xyz/Article/details/gnyxzawxt.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.fanxiaobao.xyz/Article/details/gklmroomx.sHtML

[S05] C：字符串长度
来源：http://3g.fanxiaobao.xyz/Article/details/ghwzyxmjx.sHtML

strlen(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gglrzkoat.sHtML

[S06] C：字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gyjvqalui.sHtML

strcmp(a, b) == 0
来源：http://read.share.fanxiaobao.xyz/Article/details/gpdocfimb.sHtML

[S07] C：数组遍历求和
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxhnmiblb.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.fanxiaobao.xyz/Article/details/gjmlzqurf.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fanxiaobao.xyz/Article/details/gwjdtatyb.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gosgvrwpy.sHtML

[S09] C：结构体定义与初始化
来源：http://m.share.fanxiaobao.xyz/Article/details/ghajdzopm.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.fanxiaobao.xyz/Article/details/gldjotcok.sHtML

[S10] C：指针与解引用
来源：http://wap.fanxiaobao.xyz/Article/details/gnjxrblsn.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqcumdyzd.sHtML

[S11] C：逐行读文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gswmojtdo.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://blog.fanxiaobao.xyz/Article/details/gmpbfhqhq.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gugdgkhjl.sHtML

fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gikppugre.sHtML

[S12] C：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/giqmuufgh.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnsetsqqz.sHtML

[S13] C：宏定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gosrzswsu.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.fanxiaobao.xyz/Article/details/gftyisyrf.sHtML

[S14] C：枚举
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gufdypdce.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fanxiaobao.xyz/Article/details/gxcoxwfcf.sHtML

[S15] C：类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gwadwmnng.sHtML

(double) a / b
来源：http://3g.fanxiaobao.xyz/Article/details/giidbkkaq.sHtML

[S16] C：位操作置位
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfhqxbocl.sHtML

x |= (1 << 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gwmvsrnyi.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gijwazddi.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gknemdzkg.sHtML

[S18] C：命令行参数
来源：http://blog.fanxiaobao.xyz/Article/details/glzfaofmy.sHtML

int main(int argc, char **argv)
来源：http://blog.fanxiaobao.xyz/Article/details/galfmgcpw.sHtML

[S19] C：快速排序
来源：http://m.share.fanxiaobao.xyz/Article/details/glhziystw.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsmdzfxzh.sHtML

[S20] C：二分查找
来源：http://read.share.fanxiaobao.xyz/Article/details/gpbbnlfeu.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gzuswmxoy.sHtML

[S21] C：字符类别判断
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwajejjb.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://baike.fanxiaobao.xyz/Article/details/gnrcuerpc.sHtML

[S22] C：字符串转数字
来源：http://blog.fanxiaobao.xyz/Article/details/gqhtkntqz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwcjuulbr.sHtML

[S23] C：随机数
来源：http://blog.fanxiaobao.xyz/Article/details/gnetsnkne.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://3g.fanxiaobao.xyz/Article/details/gyxmqqtkv.sHtML

[S24] C：获取本地时间
来源：http://3g.fanxiaobao.xyz/Article/details/gylsyrnke.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.fanxiaobao.xyz/Article/details/gcfgjhboz.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjfmlvwsa.sHtML

memcpy(dst, src, n);
来源：http://wap.fanxiaobao.xyz/Article/details/gjtsyxmer.sHtML

[S26] C：内存清零
来源：http://blog.fanxiaobao.xyz/Article/details/gqhqpjsfq.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gyoyrdglr.sHtML

[S27] C：定义常量
来源：http://3g.fanxiaobao.xyz/Article/details/gcejzzziq.sHtML

const double PI = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gsuuvddlp.sHtML

[S28] C：静态变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfpabpqoo.sHtML

static int counter = 0;
来源：http://m.share.fanxiaobao.xyz/Article/details/garkoojvu.sHtML

[S29] C：变参函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsqmksjhr.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.fanxiaobao.xyz/Article/details/grmvpjcic.sHtML

[S30] C：头文件保护
来源：http://read.share.fanxiaobao.xyz/Article/details/gbvqfiebg.sHtML

#ifndef X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gyhyjkgwj.sHtML

#define X_H
来源：http://baike.fanxiaobao.xyz/Article/details/gjmyhisln.sHtML

#endif
来源：http://blog.fanxiaobao.xyz/Article/details/gpvfqurax.sHtML

[S31] C++：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqzuxyfcd.sHtML

#include <iostream>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwlbalzxf.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glrujlvcw.sHtML

[S32] C++：字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gulmezjad.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fanxiaobao.xyz/Article/details/ggwphgskh.sHtML

[S33] C++：vector 增删
来源：http://mobile.fanxiaobao.xyz/Article/details/gefparasg.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gbqyhowzt.sHtML

[S34] C++：遍历 vector
来源：http://baike.fanxiaobao.xyz/Article/details/gckgmjssh.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfjhvvqbr.sHtML

[S35] C++：map
来源：http://mobile.fanxiaobao.xyz/Article/details/ghskixvda.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.fanxiaobao.xyz/Article/details/gktzghxcz.sHtML

[S36] C++：unordered_map
来源：http://mobile.fanxiaobao.xyz/Article/details/gdzplzptb.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghbcfinpg.sHtML

[S37] C++：set
来源：http://wap.fanxiaobao.xyz/Article/details/gzcfawwey.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fanxiaobao.xyz/Article/details/gdelfzrxp.sHtML

[S38] C++：排序
来源：http://blog.fanxiaobao.xyz/Article/details/ghsebsiyy.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/gyaentlzb.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqosijflc.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://blog.fanxiaobao.xyz/Article/details/ghgrhxkum.sHtML

[S40] C++：查找元素
来源：http://blog.fanxiaobao.xyz/Article/details/gyglnukft.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbknylojc.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaxsfdyrx.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gdsgazczl.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfjllolij.sHtML

class B : public Base { public: void f() override {} };
来源：http://m.share.fanxiaobao.xyz/Article/details/gdxhhgbwd.sHtML

[S43] C++：智能指针
来源：http://3g.fanxiaobao.xyz/Article/details/gvqrfbekz.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.fanxiaobao.xyz/Article/details/gyarzjhig.sHtML

[S44] C++：引用传参
来源：http://baike.fanxiaobao.xyz/Article/details/gqjpnonal.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fanxiaobao.xyz/Article/details/glnsezxeu.sHtML

[S45] C++：lambda
来源：http://blog.fanxiaobao.xyz/Article/details/gnhdkhfsy.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://mobile.fanxiaobao.xyz/Article/details/glhrtwxiw.sHtML

[S46] C++：函数模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gvenvvfxx.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gbbjomrbw.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.fanxiaobao.xyz/Article/details/gidtgvper.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.fanxiaobao.xyz/Article/details/goxvuespj.sHtML

[S48] C++：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gcxfncatz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fanxiaobao.xyz/Article/details/gbinwkfpf.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfoewooqb.sHtML

[S49] C++：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gmjxonjvv.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mobile.fanxiaobao.xyz/Article/details/geiwtyxvw.sHtML

[S50] C++：格式化数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gheqyqkjt.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fanxiaobao.xyz/Article/details/gshubuwvf.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gzbbflclt.sHtML

static_cast<double>(a) / b
来源：http://www.share.fanxiaobao.xyz/Article/details/ggwitswrz.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.fanxiaobao.xyz/Article/details/gmomnvltg.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gnymmnoba.sHtML

[S53] C++：移动语义
来源：http://baike.fanxiaobao.xyz/Article/details/gyvkjfnie.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fanxiaobao.xyz/Article/details/gvfaowxxo.sHtML

[S54] C++：异常处理
来源：http://mobile.fanxiaobao.xyz/Article/details/gdctimsfi.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsctvfryl.sHtML

[S55] C++：结构化绑定
来源：http://read.share.fanxiaobao.xyz/Article/details/gvfemxpab.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fanxiaobao.xyz/Article/details/gxshfbycs.sHtML

[S56] C++：optional
来源：http://mobile.fanxiaobao.xyz/Article/details/gqwezbpzj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fanxiaobao.xyz/Article/details/gvklwrxla.sHtML

[S57] C++：编译期常量
来源：http://read.share.fanxiaobao.xyz/Article/details/gyyicttxj.sHtML

constexpr int N = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gqndjmotw.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghjndqexz.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fanxiaobao.xyz/Article/details/geogbjoug.sHtML

[S59] C++：静态断言
来源：http://3g.fanxiaobao.xyz/Article/details/gbhswdkbs.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://read.share.fanxiaobao.xyz/Article/details/gsorpgcpp.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.fanxiaobao.xyz/Article/details/grgaaippl.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mobile.fanxiaobao.xyz/Article/details/gahzurrcf.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/ghapsdzhy.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fanxiaobao.xyz/Article/details/grecxjdwx.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gphlplsrw.sHtML

[T01] Kotlin：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gywqwyfgc.sHtML

println("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gpasymntr.sHtML

[T02] Kotlin：变量
来源：http://blog.fanxiaobao.xyz/Article/details/grkdacikr.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fanxiaobao.xyz/Article/details/gmfzohxov.sHtML

[T03] Kotlin：字符串模板
来源：http://wap.fanxiaobao.xyz/Article/details/gmctsrink.sHtML

"值: $b"
来源：http://mobile.fanxiaobao.xyz/Article/details/gcujiawcm.sHtML

[T04] Kotlin：空安全
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdhjbeejx.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fanxiaobao.xyz/Article/details/gkgoodrlm.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/geilkkryt.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.share.fanxiaobao.xyz/Article/details/gvlbgcrey.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.fanxiaobao.xyz/Article/details/gjivgrqaw.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gjxlltzma.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsstjpvyd.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://3g.fanxiaobao.xyz/Article/details/gjvmotbcu.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fanxiaobao.xyz/Article/details/gqqpatvyy.sHtML

data class User(val name: String, val age: Int)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtwbnushj.sHtML

[T09] Kotlin：扩展函数
来源：http://read.share.fanxiaobao.xyz/Article/details/glhbezxgs.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.fanxiaobao.xyz/Article/details/gyxcmjbzp.sHtML

[T10] Kotlin：默认参数
来源：http://wap.fanxiaobao.xyz/Article/details/gzdcuzxha.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.fanxiaobao.xyz/Article/details/gizexslht.sHtML

[T11] Kotlin：协程
来源：http://blog.fanxiaobao.xyz/Article/details/gdukxdszq.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.fanxiaobao.xyz/Article/details/gbpnpybbg.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.fanxiaobao.xyz/Article/details/gzcrwqpfq.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gghajpstb.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gucbbujaj.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gaysboqxo.sHtML

[T14] Kotlin：循环
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjhxrlpku.sHtML

for (i in 1..10) println(i)
来源：http://wap.fanxiaobao.xyz/Article/details/gnwhtvbvt.sHtML

[T15] Kotlin：接口
来源：http://3g.fanxiaobao.xyz/Article/details/gyrnuwoyj.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/grwrumeco.sHtML

[T16] Swift：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gekvvjwfg.sHtML

print("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzivenuoj.sHtML

[T17] Swift：变量与常量
来源：http://www.share.fanxiaobao.xyz/Article/details/gkonkntze.sHtML

var a = 1;  let b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gclssguao.sHtML

[T18] Swift：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gfaxyxfrn.sHtML

"值: \(b)"
来源：http://wap.fanxiaobao.xyz/Article/details/gavnvxjco.sHtML

[T19] Swift：可选绑定
来源：http://3g.fanxiaobao.xyz/Article/details/ghjcmohdu.sHtML

if let n = opt { print(n) }
来源：http://blog.fanxiaobao.xyz/Article/details/gkcokkzdt.sHtML

[T20] Swift：数组操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gmqpaojvk.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.fanxiaobao.xyz/Article/details/guorufqyf.sHtML

[T21] Swift：遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwyzvrfeq.sHtML

for x in a { print(x) }
来源：http://baike.fanxiaobao.xyz/Article/details/gbnqkiphh.sHtML

[T22] Swift：字典
来源：http://www.share.fanxiaobao.xyz/Article/details/gwalktrrp.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gikldrqnv.sHtML

[T23] Swift：函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxsebjkij.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdufgjgrs.sHtML

[T24] Swift：闭包
来源：http://m.share.fanxiaobao.xyz/Article/details/gvjlademk.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gssflibnq.sHtML

[T25] Swift：结构体
来源：http://baike.fanxiaobao.xyz/Article/details/gebhbagqk.sHtML

struct P { var x: Int }
来源：http://www.share.fanxiaobao.xyz/Article/details/gcgrlvmti.sHtML

[T26] Swift：类与重写
来源：http://www.share.fanxiaobao.xyz/Article/details/gdoxrqjaa.sHtML

class A: Base { override func f() {} }
来源：http://wap.fanxiaobao.xyz/Article/details/grixivmly.sHtML

[T27] Swift：错误处理
来源：http://baike.fanxiaobao.xyz/Article/details/gmizxqhso.sHtML

do { try f() } catch { print(error) }
来源：http://wap.fanxiaobao.xyz/Article/details/gtcpglgjc.sHtML

[T28] Swift：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gtutrmzyj.sHtML

enum Color { case red, green }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfphqpozs.sHtML

[T29] Swift：guard 提前返回
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnhrxuhar.sHtML

guard let x = opt else { return }
来源：http://wap.fanxiaobao.xyz/Article/details/gbxegixsz.sHtML

[T30] Swift：协议
来源：http://3g.fanxiaobao.xyz/Article/details/glphmzadv.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fanxiaobao.xyz/Article/details/geayknvxb.sHtML

[T31] Lua：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gabbrbktz.sHtML

print("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwusytlr.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghihauleu.sHtML

local a = 1
来源：http://3g.fanxiaobao.xyz/Article/details/gjspdpdkt.sHtML

[T33] Lua：表（数组）
来源：http://blog.fanxiaobao.xyz/Article/details/gnxovdhfi.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.fanxiaobao.xyz/Article/details/gnmcdpqmq.sHtML

[T34] Lua：遍历表
来源：http://www.blog.fanxiaobao.xyz/Article/details/grrwbxjpd.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://3g.fanxiaobao.xyz/Article/details/gtklulunq.sHtML

[T35] Lua：字典表
来源：http://wap.fanxiaobao.xyz/Article/details/ggslsoxym.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gxnjwguyk.sHtML

[T36] Lua：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/goahkptzq.sHtML

function add(a, b) return a + b end
来源：http://wap.fanxiaobao.xyz/Article/details/geqrkvyot.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.fanxiaobao.xyz/Article/details/gadfquubc.sHtML

"a" .. "b"
来源：http://m.share.fanxiaobao.xyz/Article/details/ghmppepqc.sHtML

[T38] Lua：条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gtqpcuzuc.sHtML

if x > 0 then print("正") end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyagzxrsj.sHtML

[T39] Lua：模式匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/ggrqvmqqx.sHtML

string.find(s, "%d+")
来源：http://m.share.fanxiaobao.xyz/Article/details/gjqxzjtli.sHtML

[T40] Lua：元表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpsmyrcgk.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghmpckjyi.sHtML

[T41] Perl：Hello World
来源：http://wap.fanxiaobao.xyz/Article/details/gbjeqihas.sHtML

print "Hello\n";
来源：http://baike.fanxiaobao.xyz/Article/details/gitnmwstq.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxiaxxbkz.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.fanxiaobao.xyz/Article/details/gvwtmgmgp.sHtML

[T43] Perl：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gobiiaxiq.sHtML

"值: $a"
来源：http://www.share.fanxiaobao.xyz/Article/details/gpmcgtbpu.sHtML

[T44] Perl：条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/grfwikpto.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glvurhghk.sHtML

[T45] Perl：数组遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gerblytcn.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gspsscjwx.sHtML

[T46] Perl：哈希操作
来源：http://m.share.fanxiaobao.xyz/Article/details/gaqnxdsbx.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggmxqyujb.sHtML

[T47] Perl：正则捕获
来源：http://mobile.fanxiaobao.xyz/Article/details/gjxlvyzhn.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gbwgvaesh.sHtML

[T48] Perl：正则替换
来源：http://blog.fanxiaobao.xyz/Article/details/gcdsgyvsc.sHtML

$s =~ s/old/new/g;
来源：http://baike.fanxiaobao.xyz/Article/details/gspuzreif.sHtML

[T49] Perl：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gkjociyyc.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gojujcfnt.sHtML

[T50] Perl：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gbcsxhvmf.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.fanxiaobao.xyz/Article/details/gmhqkexku.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://wap.fanxiaobao.xyz/Article/details/gpepgxtjw.sHtML

[T51] Scala：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gwxgxbixw.sHtML

println("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gehxyxnal.sHtML

[T52] Scala：变量
来源：http://m.share.fanxiaobao.xyz/Article/details/glqbzbdao.sHtML

val a = 1;  var b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gyogibeip.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzuxjzvjy.sHtML

s"值: $b"
来源：http://blog.fanxiaobao.xyz/Article/details/gidzdveva.sHtML

[T54] Scala：集合映射
来源：http://m.share.fanxiaobao.xyz/Article/details/gyxhotggj.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.fanxiaobao.xyz/Article/details/gszyjvgbe.sHtML

[T55] Scala：集合过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqjfauvtu.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gnldhvcjs.sHtML

[T56] Scala：样例类
来源：http://baike.fanxiaobao.xyz/Article/details/gaabyerch.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtvprtauy.sHtML

[T57] Scala：模式匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gagltppwz.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjzvznayc.sHtML

[T58] Scala：函数定义
来源：http://read.share.fanxiaobao.xyz/Article/details/grhsuslxd.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.fanxiaobao.xyz/Article/details/gfjfoktll.sHtML

[T59] Scala：循环
来源：http://blog.fanxiaobao.xyz/Article/details/ghbcnphit.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/glrojecpn.sHtML

[T60] Scala：折叠
来源：http://mobile.fanxiaobao.xyz/Article/details/gqxyswkyx.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcnajsypr.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gbpyirbaz.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wap.fanxiaobao.xyz/Article/details/gnpcyklff.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvzypannj.sHtML


<!-- 参考信息 -->