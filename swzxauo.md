代发 wailian999

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.fanxiaobao.xyz/Article/details/gctouhdrd.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gjvmiyyro.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.fanxiaobao.xyz/Article/details/gkpkgrylu.sHtML

[R61] 磁盘占用
来源：http://read.share.fanxiaobao.xyz/Article/details/geelxxyrj.sHtML

df -h;  du -sh *
来源：http://www.share.fanxiaobao.xyz/Article/details/gpwekvdzx.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fanxiaobao.xyz/Article/details/giupofzbh.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fanxiaobao.xyz/Article/details/gfzelfeha.sHtML

[R63] 内存与进程
来源：http://baike.fanxiaobao.xyz/Article/details/gpufdjysl.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fanxiaobao.xyz/Article/details/grioaiptc.sHtML

[R64] 结束进程
来源：http://read.share.fanxiaobao.xyz/Article/details/gtvlldjcp.sHtML

kill -9 $(pgrep -f app.py)
来源：http://read.share.fanxiaobao.xyz/Article/details/gyfeczial.sHtML

[R65] 查看端口占用
来源：http://3g.fanxiaobao.xyz/Article/details/ghscmxsct.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.fanxiaobao.xyz/Article/details/gwgorrueo.sHtML

[R66] 定时任务
来源：http://blog.fanxiaobao.xyz/Article/details/gatywauyq.sHtML

crontab -e;  crontab -l
来源：http://mobile.fanxiaobao.xyz/Article/details/gxllocujl.sHtML

[R67] 生成随机十六进制串
来源：http://blog.fanxiaobao.xyz/Article/details/gzlsawdmm.sHtML

openssl rand -hex 16
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gocctuzzq.sHtML

[R68] 计算文件校验值
来源：http://www.share.fanxiaobao.xyz/Article/details/gajnecsvq.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.fanxiaobao.xyz/Article/details/gouulcofp.sHtML

[R69] 生成随机密码
来源：http://blog.fanxiaobao.xyz/Article/details/grjkymbfs.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fanxiaobao.xyz/Article/details/gfjgsxitf.sHtML

[R70] 时间戳与互转
来源：http://mobile.fanxiaobao.xyz/Article/details/gvmxxjumf.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.fanxiaobao.xyz/Article/details/gqqggvuan.sHtML

[R71] 日期格式化
来源：http://m.share.fanxiaobao.xyz/Article/details/gecufbqwh.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.fanxiaobao.xyz/Article/details/gaemrqghc.sHtML

[R72] 等待端口就绪
来源：http://3g.fanxiaobao.xyz/Article/details/gpwdapinu.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gghidspvy.sHtML

[R73] 分割大日志
来源：http://read.share.fanxiaobao.xyz/Article/details/gogfnyina.sHtML

split -l 1000 big.log part_
来源：http://wap.fanxiaobao.xyz/Article/details/gghdjextt.sHtML

[R74] 批量重命名
来源：http://baike.fanxiaobao.xyz/Article/details/ggonzffdm.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gmuryyzvh.sHtML

[R75] 导出环境变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gibqngmbj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpukpgaqx.sHtML

[R76] 使用临时文件
来源：http://mobile.fanxiaobao.xyz/Article/details/gzbjgayao.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fanxiaobao.xyz/Article/details/gaotxfqte.sHtML

[R77] 读取用户输入
来源：http://baike.fanxiaobao.xyz/Article/details/gvkuwqwkk.sHtML

read -rp "请输入: " ans
来源：http://baike.fanxiaobao.xyz/Article/details/glvkmbzcy.sHtML

[R78] 交互式菜单
来源：http://blog.fanxiaobao.xyz/Article/details/greuybmkt.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.fanxiaobao.xyz/Article/details/gaasyrehd.sHtML

[R79] 解析命令行选项
来源：http://www.share.fanxiaobao.xyz/Article/details/gbhucrwdi.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.fanxiaobao.xyz/Article/details/gxpykrzdu.sHtML

[R80] 查看脚本执行耗时
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggdbyyhnc.sHtML

time ./run.sh
来源：http://www.blog.fanxiaobao.xyz/Article/details/gozlcbjfq.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/ghqsokawt.sHtML

S. C / C++ 专题
来源：http://m.share.fanxiaobao.xyz/Article/details/gwarturxx.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmjwgyllh.sHtML

[S01] C：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gygraiipm.sHtML

#include <stdio.h>
来源：http://baike.fanxiaobao.xyz/Article/details/ghreeaesi.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fanxiaobao.xyz/Article/details/goebwqkvs.sHtML

[S02] C：变量与格式化输出
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gewhpodif.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/glfhqmsld.sHtML

[S03] C：读入整数
来源：http://www.share.fanxiaobao.xyz/Article/details/gryxnrtey.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fanxiaobao.xyz/Article/details/gixigcqao.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfqhbvzez.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.fanxiaobao.xyz/Article/details/guvfxsaln.sHtML

[S05] C：字符串长度
来源：http://m.share.fanxiaobao.xyz/Article/details/gfhouutoz.sHtML

strlen(s)
来源：http://3g.fanxiaobao.xyz/Article/details/gjjiexcsu.sHtML

[S06] C：字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gdfhzqstc.sHtML

strcmp(a, b) == 0
来源：http://m.share.fanxiaobao.xyz/Article/details/grfnyfraf.sHtML

[S07] C：数组遍历求和
来源：http://3g.fanxiaobao.xyz/Article/details/gvbcmwezc.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fanxiaobao.xyz/Article/details/geuccurzj.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.fanxiaobao.xyz/Article/details/gwniudokw.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.share.fanxiaobao.xyz/Article/details/gsjkygewg.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.fanxiaobao.xyz/Article/details/glisyxvye.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghkwpfkxu.sHtML

[S10] C：指针与解引用
来源：http://m.share.fanxiaobao.xyz/Article/details/glkuukkiq.sHtML

int *p = &a;  *p = 5;
来源：http://read.share.fanxiaobao.xyz/Article/details/ggmletixa.sHtML

[S11] C：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gdojtxequ.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://mobile.fanxiaobao.xyz/Article/details/gxwszmmbh.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fanxiaobao.xyz/Article/details/goanybbel.sHtML

fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gskuyiqzq.sHtML

[S12] C：写文件
来源：http://3g.fanxiaobao.xyz/Article/details/gwtzwfmzb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/gylfaslgo.sHtML

[S13] C：宏定义
来源：http://blog.fanxiaobao.xyz/Article/details/gwkpjyeuy.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fanxiaobao.xyz/Article/details/gfrklsqzk.sHtML

[S14] C：枚举
来源：http://blog.fanxiaobao.xyz/Article/details/gwffqjsrj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fanxiaobao.xyz/Article/details/gcigunxxw.sHtML

[S15] C：类型转换
来源：http://read.share.fanxiaobao.xyz/Article/details/gccxbatwo.sHtML

(double) a / b
来源：http://wap.fanxiaobao.xyz/Article/details/gejjlxcdo.sHtML

[S16] C：位操作置位
来源：http://wap.fanxiaobao.xyz/Article/details/gkoobciwh.sHtML

x |= (1 << 3);
来源：http://baike.fanxiaobao.xyz/Article/details/gregvujbt.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gldzbmzqp.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.fanxiaobao.xyz/Article/details/gnoyepjuz.sHtML

[S18] C：命令行参数
来源：http://www.share.fanxiaobao.xyz/Article/details/gjnrzpasf.sHtML

int main(int argc, char **argv)
来源：http://m.share.fanxiaobao.xyz/Article/details/giasazbsn.sHtML

[S19] C：快速排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzgzwuzxz.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/ghzbxtmtt.sHtML

[S20] C：二分查找
来源：http://mobile.fanxiaobao.xyz/Article/details/gmgtwlayk.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fanxiaobao.xyz/Article/details/gfmhctdtq.sHtML

[S21] C：字符类别判断
来源：http://m.share.fanxiaobao.xyz/Article/details/grrizyqyb.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fanxiaobao.xyz/Article/details/gnaidlkdt.sHtML

[S22] C：字符串转数字
来源：http://read.share.fanxiaobao.xyz/Article/details/gushlolku.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.fanxiaobao.xyz/Article/details/gthcczves.sHtML

[S23] C：随机数
来源：http://3g.fanxiaobao.xyz/Article/details/gyrzvamgb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://read.share.fanxiaobao.xyz/Article/details/gwliawplm.sHtML

[S24] C：获取本地时间
来源：http://www.blog.fanxiaobao.xyz/Article/details/gawthxwtl.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fanxiaobao.xyz/Article/details/gmdeelpoo.sHtML

[S25] C：内存拷贝
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grzrretaa.sHtML

memcpy(dst, src, n);
来源：http://wap.fanxiaobao.xyz/Article/details/grkixymbe.sHtML

[S26] C：内存清零
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gewidodwm.sHtML

memset(a, 0, sizeof a);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzmofnhxc.sHtML

[S27] C：定义常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gjvtcxjoe.sHtML

const double PI = 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gmkuwowtl.sHtML

[S28] C：静态变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gytlpcxip.sHtML

static int counter = 0;
来源：http://3g.fanxiaobao.xyz/Article/details/gdbltyuvt.sHtML

[S29] C：变参函数
来源：http://baike.fanxiaobao.xyz/Article/details/gpagkdkrs.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.fanxiaobao.xyz/Article/details/gfpelgpkv.sHtML

[S30] C：头文件保护
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gufdvcgap.sHtML

#ifndef X_H
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqnrsbrdm.sHtML

#define X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gpksmyykp.sHtML

#endif
来源：http://blog.fanxiaobao.xyz/Article/details/ghccpieis.sHtML

[S31] C++：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gaqdxbrfh.sHtML

#include <iostream>
来源：http://wap.fanxiaobao.xyz/Article/details/giigmblpj.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gnrngqwuv.sHtML

[S32] C++：字符串
来源：http://3g.fanxiaobao.xyz/Article/details/garhxpogh.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fanxiaobao.xyz/Article/details/gnuhemcir.sHtML

[S33] C++：vector 增删
来源：http://mobile.fanxiaobao.xyz/Article/details/ggcjzixjo.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://blog.fanxiaobao.xyz/Article/details/gynmohksx.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guponlnkf.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gtjlihhav.sHtML

[S35] C++：map
来源：http://www.share.fanxiaobao.xyz/Article/details/gnqjhugqn.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fanxiaobao.xyz/Article/details/gwouvspot.sHtML

[S36] C++：unordered_map
来源：http://www.share.fanxiaobao.xyz/Article/details/getocxurf.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.fanxiaobao.xyz/Article/details/gsinctfbh.sHtML

[S37] C++：set
来源：http://mobile.fanxiaobao.xyz/Article/details/gcvrjukbm.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/giactqkjh.sHtML

[S38] C++：排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gzfzmcbud.sHtML

std::sort(v.begin(), v.end());
来源：http://blog.fanxiaobao.xyz/Article/details/gaitgwhkj.sHtML

[S39] C++：自定义比较器排序
来源：http://3g.fanxiaobao.xyz/Article/details/gmtypqtyc.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wap.fanxiaobao.xyz/Article/details/gefntrtzf.sHtML

[S40] C++：查找元素
来源：http://www.blog.fanxiaobao.xyz/Article/details/guefuvhdh.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjsztgcqo.sHtML

[S41] C++：类与构造函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gwhutggxz.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gzjatueyu.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fanxiaobao.xyz/Article/details/gefafywiq.sHtML

class B : public Base { public: void f() override {} };
来源：http://blog.fanxiaobao.xyz/Article/details/gxkclhncn.sHtML

[S43] C++：智能指针
来源：http://www.share.fanxiaobao.xyz/Article/details/glfaujizr.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.fanxiaobao.xyz/Article/details/grwspzyrr.sHtML

[S44] C++：引用传参
来源：http://read.share.fanxiaobao.xyz/Article/details/gxomohajn.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gelgyveei.sHtML

[S45] C++：lambda
来源：http://www.blog.fanxiaobao.xyz/Article/details/gisurzhtj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://3g.fanxiaobao.xyz/Article/details/giuamwruk.sHtML

[S46] C++：函数模板
来源：http://m.share.fanxiaobao.xyz/Article/details/gnfukggna.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gazvwihdw.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.fanxiaobao.xyz/Article/details/gnvxtkutp.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gafucsrcr.sHtML

[S48] C++：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gwtotlrwn.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.fanxiaobao.xyz/Article/details/geupecgan.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gvbxcbsrg.sHtML

[S49] C++：写文件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gieafjuop.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gduoxrilc.sHtML

[S50] C++：格式化数字
来源：http://read.share.fanxiaobao.xyz/Article/details/ggvkdbjoo.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gxlxmrayw.sHtML

[S51] C++：显式类型转换
来源：http://3g.fanxiaobao.xyz/Article/details/gfpptsjrk.sHtML

static_cast<double>(a) / b
来源：http://baike.fanxiaobao.xyz/Article/details/gyqvupreg.sHtML

[S52] C++：const 与 noexcept
来源：http://wap.fanxiaobao.xyz/Article/details/ggxbftorg.sHtML

int size() const noexcept { return n_; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gtxhjvcqv.sHtML

[S53] C++：移动语义
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghwiwalgf.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.fanxiaobao.xyz/Article/details/giboneiuc.sHtML

[S54] C++：异常处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gqbhstqnt.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://3g.fanxiaobao.xyz/Article/details/gzofywgtj.sHtML

[S55] C++：结构化绑定
来源：http://3g.fanxiaobao.xyz/Article/details/gyagitajy.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://m.share.fanxiaobao.xyz/Article/details/grzrwcoai.sHtML

[S56] C++：optional
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdrrllelj.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjzyudpmg.sHtML

[S57] C++：编译期常量
来源：http://baike.fanxiaobao.xyz/Article/details/gccesjxuo.sHtML

constexpr int N = 10;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmehmswvn.sHtML

[S58] C++：命名空间
来源：http://wap.fanxiaobao.xyz/Article/details/gfnmwnwam.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdatxrhpi.sHtML

[S59] C++：静态断言
来源：http://m.share.fanxiaobao.xyz/Article/details/goemousyh.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fanxiaobao.xyz/Article/details/gegbrcthp.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fanxiaobao.xyz/Article/details/gnvhdijcf.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fanxiaobao.xyz/Article/details/gdzmusgot.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggxqjooxj.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fanxiaobao.xyz/Article/details/gdycfptve.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gtbryyzic.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzzesfnal.sHtML

println("Hello")
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpajgzbvo.sHtML

[T02] Kotlin：变量
来源：http://m.share.fanxiaobao.xyz/Article/details/gwutqgtnk.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fanxiaobao.xyz/Article/details/gwhezmohz.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.fanxiaobao.xyz/Article/details/gncfrwcbd.sHtML

"值: $b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gnsrtoylh.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fanxiaobao.xyz/Article/details/gytscoxdl.sHtML

val n: String? = null;  n?.length
来源：http://mobile.fanxiaobao.xyz/Article/details/gjwsiukmu.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.fanxiaobao.xyz/Article/details/guradfjlg.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghqnkhxwo.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fanxiaobao.xyz/Article/details/gutoktbwe.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://3g.fanxiaobao.xyz/Article/details/gucruuolw.sHtML

[T07] Kotlin：集合过滤
来源：http://wap.fanxiaobao.xyz/Article/details/gsjpammmc.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fanxiaobao.xyz/Article/details/gsdahketr.sHtML

[T08] Kotlin：数据类
来源：http://wap.fanxiaobao.xyz/Article/details/gepqrhoko.sHtML

data class User(val name: String, val age: Int)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdqxglaue.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gprwuvebi.sHtML

fun String.exclaim() = this + "!"
来源：http://www.share.fanxiaobao.xyz/Article/details/glliygqby.sHtML

[T10] Kotlin：默认参数
来源：http://www.share.fanxiaobao.xyz/Article/details/guqbjirgl.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fanxiaobao.xyz/Article/details/gqxbnlegd.sHtML

[T11] Kotlin：协程
来源：http://mobile.fanxiaobao.xyz/Article/details/gvoeqsjwx.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.fanxiaobao.xyz/Article/details/gklgexhxb.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.fanxiaobao.xyz/Article/details/grscksriy.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmrkdesum.sHtML

[T13] Kotlin：只读 Map
来源：http://wap.fanxiaobao.xyz/Article/details/ghgbrvehv.sHtML

val m = mapOf("a" to 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/geyozcylt.sHtML

[T14] Kotlin：循环
来源：http://blog.fanxiaobao.xyz/Article/details/gfhpdfsmt.sHtML

for (i in 1..10) println(i)
来源：http://www.share.fanxiaobao.xyz/Article/details/gjxjcmyhj.sHtML

[T15] Kotlin：接口
来源：http://3g.fanxiaobao.xyz/Article/details/gynjjoclp.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gaxwtpdgo.sHtML

[T16] Swift：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gdejxekuh.sHtML

print("Hello")
来源：http://3g.fanxiaobao.xyz/Article/details/gyuxxgqpf.sHtML

[T17] Swift：变量与常量
来源：http://baike.fanxiaobao.xyz/Article/details/gvaumfxze.sHtML

var a = 1;  let b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/giajkxitp.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/guatbhcpb.sHtML

"值: \(b)"
来源：http://blog.fanxiaobao.xyz/Article/details/gsqjkjsic.sHtML

[T19] Swift：可选绑定
来源：http://www.share.fanxiaobao.xyz/Article/details/gueevadhx.sHtML

if let n = opt { print(n) }
来源：http://baike.fanxiaobao.xyz/Article/details/gzlrkgzgr.sHtML

[T20] Swift：数组操作
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyjpwvgdb.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqqmeacgq.sHtML

[T21] Swift：遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gpxwmgien.sHtML

for x in a { print(x) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gcwyazqwa.sHtML

[T22] Swift：字典
来源：http://3g.fanxiaobao.xyz/Article/details/gbxnkvong.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.fanxiaobao.xyz/Article/details/gipcptgdz.sHtML

[T23] Swift：函数
来源：http://baike.fanxiaobao.xyz/Article/details/gaarjnwup.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtodrzssl.sHtML

[T24] Swift：闭包
来源：http://read.share.fanxiaobao.xyz/Article/details/gialjophw.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyeuynxgj.sHtML

[T25] Swift：结构体
来源：http://mobile.fanxiaobao.xyz/Article/details/geequthcv.sHtML

struct P { var x: Int }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqgpzfyew.sHtML

[T26] Swift：类与重写
来源：http://www.share.fanxiaobao.xyz/Article/details/gmupyiqik.sHtML

class A: Base { override func f() {} }
来源：http://www.share.fanxiaobao.xyz/Article/details/gqsyuzkjy.sHtML

[T27] Swift：错误处理
来源：http://read.share.fanxiaobao.xyz/Article/details/gezozxxsf.sHtML

do { try f() } catch { print(error) }
来源：http://wap.fanxiaobao.xyz/Article/details/gmyoefhnm.sHtML

[T28] Swift：枚举
来源：http://read.share.fanxiaobao.xyz/Article/details/ghozscike.sHtML

enum Color { case red, green }
来源：http://www.share.fanxiaobao.xyz/Article/details/grojsnmtd.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvrxqpehz.sHtML

guard let x = opt else { return }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gofqadnbd.sHtML

[T30] Swift：协议
来源：http://blog.fanxiaobao.xyz/Article/details/glmgqqsly.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.fanxiaobao.xyz/Article/details/gynamfcqg.sHtML

[T31] Lua：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/glwtntlsq.sHtML

print("Hello")
来源：http://m.share.fanxiaobao.xyz/Article/details/gogzhqros.sHtML

[T32] Lua：局部变量
来源：http://3g.fanxiaobao.xyz/Article/details/gxhthndyw.sHtML

local a = 1
来源：http://blog.fanxiaobao.xyz/Article/details/grtvtvamj.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fanxiaobao.xyz/Article/details/givhjcsfc.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.fanxiaobao.xyz/Article/details/gkwyhgprq.sHtML

[T34] Lua：遍历表
来源：http://www.share.fanxiaobao.xyz/Article/details/gbkfawmwv.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.fanxiaobao.xyz/Article/details/gwayyhdhw.sHtML

[T35] Lua：字典表
来源：http://www.share.fanxiaobao.xyz/Article/details/gtjmfdvlr.sHtML

local d = { a = 1 };  d.b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/grtrtxgvb.sHtML

[T36] Lua：函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gbbqtcpxg.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwqkrkxcg.sHtML

[T37] Lua：字符串拼接
来源：http://wap.fanxiaobao.xyz/Article/details/gjzonfuaa.sHtML

"a" .. "b"
来源：http://m.share.fanxiaobao.xyz/Article/details/ggvowdqjc.sHtML

[T38] Lua：条件
来源：http://baike.fanxiaobao.xyz/Article/details/glytcrfzo.sHtML

if x > 0 then print("正") end
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjjmzapas.sHtML

[T39] Lua：模式匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gpqmmsetj.sHtML

string.find(s, "%d+")
来源：http://read.share.fanxiaobao.xyz/Article/details/gomohbmlq.sHtML

[T40] Lua：元表
来源：http://m.share.fanxiaobao.xyz/Article/details/gaqiqkskd.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.fanxiaobao.xyz/Article/details/gagelqkts.sHtML

[T41] Perl：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gagunrwss.sHtML

print "Hello\n";
来源：http://m.share.fanxiaobao.xyz/Article/details/gazqizqsu.sHtML

[T42] Perl：变量类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gkxffqvjb.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.fanxiaobao.xyz/Article/details/gozmxttrt.sHtML

[T43] Perl：字符串插值
来源：http://read.share.fanxiaobao.xyz/Article/details/gqirwlcnf.sHtML

"值: $a"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gomgccojt.sHtML

[T44] Perl：条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsiipffyg.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gialjadtb.sHtML

[T45] Perl：数组遍历
来源：http://wap.fanxiaobao.xyz/Article/details/gpmelvkca.sHtML

for my $x (@arr) { print $x; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gvdlwvamh.sHtML

[T46] Perl：哈希操作
来源：http://3g.fanxiaobao.xyz/Article/details/gveyemfdg.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gsjezapdx.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxknkzvsv.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gvpygeqrv.sHtML

[T48] Perl：正则替换
来源：http://3g.fanxiaobao.xyz/Article/details/gbdjkhwwm.sHtML

$s =~ s/old/new/g;
来源：http://mobile.fanxiaobao.xyz/Article/details/gyuhqmidw.sHtML

[T49] Perl：函数
来源：http://blog.fanxiaobao.xyz/Article/details/grzasignh.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.fanxiaobao.xyz/Article/details/ghbebbxha.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/goxhhmubr.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.fanxiaobao.xyz/Article/details/gunvoywek.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gdawfmdvq.sHtML

[T51] Scala：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/glbgibszz.sHtML

println("Hello")
来源：http://baike.fanxiaobao.xyz/Article/details/glauaitfd.sHtML

[T52] Scala：变量
来源：http://mobile.fanxiaobao.xyz/Article/details/gmjiywdhf.sHtML

val a = 1;  var b = 2
来源：http://3g.fanxiaobao.xyz/Article/details/gmrucrljv.sHtML

[T53] Scala：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gfjfggqqb.sHtML

s"值: $b"
来源：http://read.share.fanxiaobao.xyz/Article/details/gwlmrtqxs.sHtML

[T54] Scala：集合映射
来源：http://mobile.fanxiaobao.xyz/Article/details/ggldyswib.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gjavneoxj.sHtML

[T55] Scala：集合过滤
来源：http://wap.fanxiaobao.xyz/Article/details/ggfgjlyyd.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.fanxiaobao.xyz/Article/details/gbyzhqzma.sHtML

[T56] Scala：样例类
来源：http://baike.fanxiaobao.xyz/Article/details/gbkshculb.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsnyxmxpr.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyqpfxloo.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.fanxiaobao.xyz/Article/details/ggjanumvu.sHtML

[T58] Scala：函数定义
来源：http://baike.fanxiaobao.xyz/Article/details/gqeylkzhc.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://baike.fanxiaobao.xyz/Article/details/glxllsumb.sHtML

[T59] Scala：循环
来源：http://www.share.fanxiaobao.xyz/Article/details/gcnjtubiu.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.fanxiaobao.xyz/Article/details/gisqcbfaj.sHtML

[T60] Scala：折叠
来源：http://mobile.fanxiaobao.xyz/Article/details/gnsmdiugn.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqtlymofe.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gsiyoyelq.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.fanxiaobao.xyz/Article/details/ghsbdnitf.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/guddkcrkh.sHtML


<!-- 参考信息 -->