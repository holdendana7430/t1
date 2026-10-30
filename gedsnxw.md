代发 wailian999

ssh user@host 'uptime'
来源：http://www.m.share.hesvh.cn/Article/details/gfcgommck.sHtML

[R58] 下载文件
来源：http://3g.hesvh.cn/Article/details/gmzmqtgmp.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.hesvh.cn/Article/details/gfbxfuirj.sHtML

[R59] 发 POST JSON
来源：http://3g.zdbjq.cn/Article/details/gpqhkrayl.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.hesvh.cn/Article/details/gqijvvtwb.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.hesvh.cn/Article/details/gzgpmqmsc.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.fehbvm.com/Article/details/gsgaiakpq.sHtML

[R61] 磁盘占用
来源：http://www.m.share.fehbvm.com/Article/details/gemjrkqsj.sHtML

df -h;  du -sh *
来源：http://blog.fehbvm.com/Article/details/gnrjbwkyk.sHtML

[R62] 找最占空间的文件
来源：http://blog.zdbjq.cn/Article/details/gsprjssxu.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fehbvm.com/Article/details/gadoglvtp.sHtML

[R63] 内存与进程
来源：http://www.share.hesvh.cn/Article/details/glopgoveh.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.hesvh.cn/Article/details/gpbfevrji.sHtML

[R64] 结束进程
来源：http://wap.hesvh.cn/Article/details/gpsrbghkp.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.hesvh.cn/Article/details/gohovzntw.sHtML

[R65] 查看端口占用
来源：http://www.share.hesvh.cn/Article/details/gckynklge.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.zdbjq.cn/Article/details/gjahuexem.sHtML

[R66] 定时任务
来源：http://read.share.hesvh.cn/Article/details/gesfziumr.sHtML

crontab -e;  crontab -l
来源：http://read.share.zdbjq.cn/Article/details/gaceceoea.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fehbvm.com/Article/details/ghynhnkyj.sHtML

openssl rand -hex 16
来源：http://wap.fehbvm.com/Article/details/gyvwzccxu.sHtML

[R68] 计算文件校验值
来源：http://wap.hesvh.cn/Article/details/gtzrmggtf.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://m.share.zdbjq.cn/Article/details/gcurrxwni.sHtML

[R69] 生成随机密码
来源：http://www.m.share.zdbjq.cn/Article/details/gtcrtolxv.sHtML

head -c 16 /dev/urandom | base64
来源：http://m.share.fehbvm.com/Article/details/grhqazhwa.sHtML

[R70] 时间戳与互转
来源：http://www.blog.hesvh.cn/Article/details/gjxwpkqnn.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fehbvm.com/Article/details/ggwlkfdpg.sHtML

[R71] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/gcttyiyxp.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://blog.zdbjq.cn/Article/details/gkgqlggmx.sHtML

[R72] 等待端口就绪
来源：http://www.share.hesvh.cn/Article/details/gkslglcdw.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://m.share.hesvh.cn/Article/details/gduhhkeqv.sHtML

[R73] 分割大日志
来源：http://baike.zdbjq.cn/Article/details/gphlbyvpz.sHtML

split -l 1000 big.log part_
来源：http://3g.fehbvm.com/Article/details/giabhwsas.sHtML

[R74] 批量重命名
来源：http://www.blog.zdbjq.cn/Article/details/grpzhnckk.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.zdbjq.cn/Article/details/guzlzinev.sHtML

[R75] 导出环境变量
来源：http://www.blog.hesvh.cn/Article/details/gbegtrvxe.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.fehbvm.com/Article/details/ggvllwtch.sHtML

[R76] 使用临时文件
来源：http://wap.zdbjq.cn/Article/details/gjmrvtwdj.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.hesvh.cn/Article/details/gdevootwe.sHtML

[R77] 读取用户输入
来源：http://m.share.fehbvm.com/Article/details/grorzqlqv.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.hesvh.cn/Article/details/gvlxlqzdd.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fehbvm.com/Article/details/gqndttnje.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.fehbvm.com/Article/details/ghfrxazox.sHtML

[R79] 解析命令行选项
来源：http://read.share.zdbjq.cn/Article/details/ggzllrljg.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.zdbjq.cn/Article/details/gtxdcdlzp.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.hesvh.cn/Article/details/gexvyvpmr.sHtML

time ./run.sh
来源：http://www.blog.zdbjq.cn/Article/details/gkdlckzbx.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gubmovqhf.sHtML

S. C / C++ 专题
来源：http://3g.hesvh.cn/Article/details/gdgbainee.sHtML

================================================================================
来源：http://3g.hesvh.cn/Article/details/gufagprlr.sHtML

[S01] C：Hello World
来源：http://baike.hesvh.cn/Article/details/gfvabuwcg.sHtML

#include <stdio.h>
来源：http://baike.zdbjq.cn/Article/details/gytbkwald.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.fehbvm.com/Article/details/gmlbeivxl.sHtML

[S02] C：变量与格式化输出
来源：http://blog.hesvh.cn/Article/details/gilbbbgbl.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fehbvm.com/Article/details/gdqfximii.sHtML

[S03] C：读入整数
来源：http://www.m.share.hesvh.cn/Article/details/gsokmyxut.sHtML

int x; scanf("%d", &x);
来源：http://blog.fehbvm.com/Article/details/gjbgykdad.sHtML

[S04] C：字符串复制
来源：http://wap.zdbjq.cn/Article/details/gfkycknrx.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.share.zdbjq.cn/Article/details/gusjezztb.sHtML

[S05] C：字符串长度
来源：http://mobile.zdbjq.cn/Article/details/gsqlryyhp.sHtML

strlen(s)
来源：http://mobile.fehbvm.com/Article/details/gfeicbkdv.sHtML

[S06] C：字符串比较
来源：http://baike.fehbvm.com/Article/details/gtiypnxzz.sHtML

strcmp(a, b) == 0
来源：http://wap.fehbvm.com/Article/details/ghlcstwus.sHtML

[S07] C：数组遍历求和
来源：http://baike.fehbvm.com/Article/details/gypvucbwx.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.hesvh.cn/Article/details/gjhhurynn.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.hesvh.cn/Article/details/gkjujhwpn.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.zdbjq.cn/Article/details/gdqrkanko.sHtML

[S09] C：结构体定义与初始化
来源：http://blog.fehbvm.com/Article/details/gvcnuhzdl.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.hesvh.cn/Article/details/gzknzkxyu.sHtML

[S10] C：指针与解引用
来源：http://www.share.zdbjq.cn/Article/details/gtchnzxqw.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.zdbjq.cn/Article/details/grykobtmy.sHtML

[S11] C：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/grhihcfpm.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.blog.zdbjq.cn/Article/details/glulwwzhk.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fehbvm.com/Article/details/givuktguw.sHtML

fclose(f);
来源：http://baike.zdbjq.cn/Article/details/gdkudtalw.sHtML

[S12] C：写文件
来源：http://m.share.fehbvm.com/Article/details/gebqjlngo.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.zdbjq.cn/Article/details/gusywxxoz.sHtML

[S13] C：宏定义
来源：http://blog.zdbjq.cn/Article/details/girfpkpep.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.hesvh.cn/Article/details/gjvnofusf.sHtML

[S14] C：枚举
来源：http://mobile.zdbjq.cn/Article/details/gigribhof.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.hesvh.cn/Article/details/gfadxkhcv.sHtML

[S15] C：类型转换
来源：http://www.share.zdbjq.cn/Article/details/gbgjzchfm.sHtML

(double) a / b
来源：http://3g.zdbjq.cn/Article/details/gjrdroyjl.sHtML

[S16] C：位操作置位
来源：http://wap.fehbvm.com/Article/details/gdbjmneha.sHtML

x |= (1 << 3);
来源：http://m.share.hesvh.cn/Article/details/ggxnejmhr.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.hesvh.cn/Article/details/gzexediqw.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.zdbjq.cn/Article/details/goaemsomk.sHtML

[S18] C：命令行参数
来源：http://www.share.zdbjq.cn/Article/details/gkijeinak.sHtML

int main(int argc, char **argv)
来源：http://m.share.zdbjq.cn/Article/details/gkbjxnpfb.sHtML

[S19] C：快速排序
来源：http://www.m.share.fehbvm.com/Article/details/gzpednsmn.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fehbvm.com/Article/details/glnybqkak.sHtML

[S20] C：二分查找
来源：http://wap.zdbjq.cn/Article/details/gpfnqjnsb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.hesvh.cn/Article/details/gplwwctfh.sHtML

[S21] C：字符类别判断
来源：http://blog.zdbjq.cn/Article/details/gkvugvnyj.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fehbvm.com/Article/details/ghdtukzko.sHtML

[S22] C：字符串转数字
来源：http://baike.fehbvm.com/Article/details/gpwyacsty.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.zdbjq.cn/Article/details/gjvkaiifq.sHtML

[S23] C：随机数
来源：http://read.share.hesvh.cn/Article/details/gdhxgpzlp.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.fehbvm.com/Article/details/gnzqeclty.sHtML

[S24] C：获取本地时间
来源：http://blog.zdbjq.cn/Article/details/gtcxulbid.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.hesvh.cn/Article/details/gyftcrwoy.sHtML

[S25] C：内存拷贝
来源：http://www.share.fehbvm.com/Article/details/gtjnwpeic.sHtML

memcpy(dst, src, n);
来源：http://mobile.fehbvm.com/Article/details/gvmjgothj.sHtML

[S26] C：内存清零
来源：http://read.share.zdbjq.cn/Article/details/ganaovibx.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.fehbvm.com/Article/details/ghmivuzti.sHtML

[S27] C：定义常量
来源：http://baike.hesvh.cn/Article/details/gampkyzvm.sHtML

const double PI = 3.14159;
来源：http://mobile.zdbjq.cn/Article/details/gfwprsylj.sHtML

[S28] C：静态变量
来源：http://mobile.fehbvm.com/Article/details/gletsozet.sHtML

static int counter = 0;
来源：http://blog.zdbjq.cn/Article/details/gzxhyqfqd.sHtML

[S29] C：变参函数
来源：http://3g.hesvh.cn/Article/details/gnqhysjvl.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.hesvh.cn/Article/details/gvmerodip.sHtML

[S30] C：头文件保护
来源：http://read.share.zdbjq.cn/Article/details/gcgiwaktd.sHtML

#ifndef X_H
来源：http://www.share.hesvh.cn/Article/details/gwxmcpcde.sHtML

#define X_H
来源：http://www.m.share.fehbvm.com/Article/details/gfdffpjdv.sHtML

#endif
来源：http://www.share.fehbvm.com/Article/details/gjwefkzwa.sHtML

[S31] C++：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gbcjrqdxy.sHtML

#include <iostream>
来源：http://www.blog.hesvh.cn/Article/details/gfangvmss.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.hesvh.cn/Article/details/givkitfoa.sHtML

[S32] C++：字符串
来源：http://3g.hesvh.cn/Article/details/grqqgmxpb.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fehbvm.com/Article/details/givnwevsn.sHtML

[S33] C++：vector 增删
来源：http://baike.fehbvm.com/Article/details/genzuulql.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fehbvm.com/Article/details/gzeoyprqj.sHtML

[S34] C++：遍历 vector
来源：http://wap.fehbvm.com/Article/details/gynyvsqgw.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.hesvh.cn/Article/details/gfhxqvdqv.sHtML

[S35] C++：map
来源：http://wap.zdbjq.cn/Article/details/gxplelswd.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gudfllzpz.sHtML

[S36] C++：unordered_map
来源：http://blog.zdbjq.cn/Article/details/gqguxqltf.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.blog.zdbjq.cn/Article/details/gaptutlcm.sHtML

[S37] C++：set
来源：http://wap.hesvh.cn/Article/details/gamhjyurp.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fehbvm.com/Article/details/guaedfyas.sHtML

[S38] C++：排序
来源：http://m.share.fehbvm.com/Article/details/gzrvooirb.sHtML

std::sort(v.begin(), v.end());
来源：http://mobile.hesvh.cn/Article/details/gkdekccfk.sHtML

[S39] C++：自定义比较器排序
来源：http://mobile.hesvh.cn/Article/details/glamqfkfv.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.hesvh.cn/Article/details/gdwdoeajo.sHtML

[S40] C++：查找元素
来源：http://read.share.hesvh.cn/Article/details/gajlljucq.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.hesvh.cn/Article/details/ghkrvrmxz.sHtML

[S41] C++：类与构造函数
来源：http://baike.hesvh.cn/Article/details/gnibxfjbt.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://m.share.zdbjq.cn/Article/details/gfpgdkxve.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.zdbjq.cn/Article/details/gryosatvd.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.zdbjq.cn/Article/details/gdzejwmwa.sHtML

[S43] C++：智能指针
来源：http://www.m.share.hesvh.cn/Article/details/gjyhfajaq.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.zdbjq.cn/Article/details/gregrtpqw.sHtML

[S44] C++：引用传参
来源：http://read.share.fehbvm.com/Article/details/guruerrvz.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fehbvm.com/Article/details/gsprvwwif.sHtML

[S45] C++：lambda
来源：http://www.blog.hesvh.cn/Article/details/gnfgxzjqj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://baike.zdbjq.cn/Article/details/gaacuadvk.sHtML

[S46] C++：函数模板
来源：http://wap.zdbjq.cn/Article/details/gjwdtwxjj.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtxmsvrcm.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.zdbjq.cn/Article/details/gyypyuplc.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://blog.fehbvm.com/Article/details/gkgrlskym.sHtML

[S48] C++：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gachbsemy.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.share.fehbvm.com/Article/details/gdqunfetq.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.hesvh.cn/Article/details/gztyhryhk.sHtML

[S49] C++：写文件
来源：http://read.share.fehbvm.com/Article/details/gpljisrjt.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.zdbjq.cn/Article/details/gwlrnkzbs.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fehbvm.com/Article/details/gzuznrobf.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.fehbvm.com/Article/details/gflicvlue.sHtML

[S51] C++：显式类型转换
来源：http://www.share.zdbjq.cn/Article/details/gjckpnifz.sHtML

static_cast<double>(a) / b
来源：http://3g.hesvh.cn/Article/details/gkewuxiyk.sHtML

[S52] C++：const 与 noexcept
来源：http://m.share.hesvh.cn/Article/details/glurbdtkg.sHtML

int size() const noexcept { return n_; }
来源：http://blog.fehbvm.com/Article/details/gscscdyfw.sHtML

[S53] C++：移动语义
来源：http://m.share.zdbjq.cn/Article/details/gttenoafc.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.hesvh.cn/Article/details/gxzhedhvr.sHtML

[S54] C++：异常处理
来源：http://baike.zdbjq.cn/Article/details/gpznedpdb.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://m.share.fehbvm.com/Article/details/gbwyuuhev.sHtML

[S55] C++：结构化绑定
来源：http://www.share.fehbvm.com/Article/details/gbrmqbqtt.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://3g.hesvh.cn/Article/details/gkjmkeeli.sHtML

[S56] C++：optional
来源：http://m.share.zdbjq.cn/Article/details/gbfyohjkt.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fehbvm.com/Article/details/gsmnicpnm.sHtML

[S57] C++：编译期常量
来源：http://m.share.zdbjq.cn/Article/details/gyfggrsjo.sHtML

constexpr int N = 10;
来源：http://www.blog.fehbvm.com/Article/details/gwxgwtkrb.sHtML

[S58] C++：命名空间
来源：http://read.share.zdbjq.cn/Article/details/gxhggtkhm.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.m.share.fehbvm.com/Article/details/gmifybozu.sHtML

[S59] C++：静态断言
来源：http://3g.zdbjq.cn/Article/details/ghvyebvah.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wap.hesvh.cn/Article/details/gpvkytfaf.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.zdbjq.cn/Article/details/gdkuxhjoi.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://baike.zdbjq.cn/Article/details/gnpoiuicp.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/giczhcfkp.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.fehbvm.com/Article/details/gijnffzjy.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gqqqriqxq.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.hesvh.cn/Article/details/gbbxigmiw.sHtML

println("Hello")
来源：http://m.share.fehbvm.com/Article/details/gtlvfuxgr.sHtML

[T02] Kotlin：变量
来源：http://baike.hesvh.cn/Article/details/gdeselxry.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.zdbjq.cn/Article/details/gxeubjpmw.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.fehbvm.com/Article/details/gsolzadex.sHtML

"值: $b"
来源：http://read.share.fehbvm.com/Article/details/ghvmxojkp.sHtML

[T04] Kotlin：空安全
来源：http://baike.fehbvm.com/Article/details/gisgicyhq.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fehbvm.com/Article/details/gdyuxicsf.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fehbvm.com/Article/details/gvqdyrbfr.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.zdbjq.cn/Article/details/giozxmnbs.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fehbvm.com/Article/details/gurkfmkdu.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.share.fehbvm.com/Article/details/gbkyoohjl.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.fehbvm.com/Article/details/gebnnezam.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fehbvm.com/Article/details/gydmvtnuc.sHtML

[T08] Kotlin：数据类
来源：http://www.share.fehbvm.com/Article/details/gncqpwfin.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.hesvh.cn/Article/details/gzxgubtkp.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.hesvh.cn/Article/details/gcbrkooqg.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fehbvm.com/Article/details/gyhthvjay.sHtML

[T10] Kotlin：默认参数
来源：http://www.blog.hesvh.cn/Article/details/glmylvncp.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fehbvm.com/Article/details/glhlnucix.sHtML

[T11] Kotlin：协程
来源：http://baike.fehbvm.com/Article/details/gmxgyigfs.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.fehbvm.com/Article/details/gxpauaqwg.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.hesvh.cn/Article/details/gulientuh.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.hesvh.cn/Article/details/gtctnetiw.sHtML

[T13] Kotlin：只读 Map
来源：http://blog.zdbjq.cn/Article/details/gsemvvhfj.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.hesvh.cn/Article/details/gmhnrfpiy.sHtML

[T14] Kotlin：循环
来源：http://www.share.hesvh.cn/Article/details/gicsqrina.sHtML

for (i in 1..10) println(i)
来源：http://wap.hesvh.cn/Article/details/gvxjckoer.sHtML

[T15] Kotlin：接口
来源：http://3g.zdbjq.cn/Article/details/gabghoxyu.sHtML

interface Shape { fun area(): Double }
来源：http://wap.fehbvm.com/Article/details/ggfrmryou.sHtML

[T16] Swift：Hello World
来源：http://blog.hesvh.cn/Article/details/gmoaghswu.sHtML

print("Hello")
来源：http://www.share.hesvh.cn/Article/details/gzfvmtgve.sHtML

[T17] Swift：变量与常量
来源：http://wap.hesvh.cn/Article/details/genkumtqu.sHtML

var a = 1;  let b = 2
来源：http://www.share.fehbvm.com/Article/details/gjklotmyk.sHtML

[T18] Swift：字符串插值
来源：http://read.share.fehbvm.com/Article/details/gleelxkdb.sHtML

"值: \(b)"
来源：http://blog.hesvh.cn/Article/details/gapvrwxni.sHtML

[T19] Swift：可选绑定
来源：http://m.share.fehbvm.com/Article/details/gxbomlloq.sHtML

if let n = opt { print(n) }
来源：http://read.share.zdbjq.cn/Article/details/gofejjcqy.sHtML

[T20] Swift：数组操作
来源：http://wap.fehbvm.com/Article/details/gqbrpmkih.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.hesvh.cn/Article/details/gbmovfnic.sHtML

[T21] Swift：遍历
来源：http://www.share.fehbvm.com/Article/details/ggzunpjeq.sHtML

for x in a { print(x) }
来源：http://read.share.zdbjq.cn/Article/details/giinhbjot.sHtML

[T22] Swift：字典
来源：http://3g.hesvh.cn/Article/details/ggoewnmje.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://blog.zdbjq.cn/Article/details/givhhyoks.sHtML

[T23] Swift：函数
来源：http://www.m.share.zdbjq.cn/Article/details/gmygfhygw.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.fehbvm.com/Article/details/gmpuksjcp.sHtML

[T24] Swift：闭包
来源：http://wap.fehbvm.com/Article/details/gsrtscvqf.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gpuhkhgux.sHtML

[T25] Swift：结构体
来源：http://www.m.share.fehbvm.com/Article/details/gmabassca.sHtML

struct P { var x: Int }
来源：http://baike.fehbvm.com/Article/details/gpvqgydyn.sHtML

[T26] Swift：类与重写
来源：http://read.share.hesvh.cn/Article/details/gmdwpiaou.sHtML

class A: Base { override func f() {} }
来源：http://blog.fehbvm.com/Article/details/gvzpqpgsq.sHtML

[T27] Swift：错误处理
来源：http://www.share.hesvh.cn/Article/details/gvhizgrfp.sHtML

do { try f() } catch { print(error) }
来源：http://www.share.fehbvm.com/Article/details/gytxrzbda.sHtML

[T28] Swift：枚举
来源：http://www.share.fehbvm.com/Article/details/ggwgxitys.sHtML

enum Color { case red, green }
来源：http://mobile.zdbjq.cn/Article/details/gfvnpcaen.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.zdbjq.cn/Article/details/gqctdznrv.sHtML

guard let x = opt else { return }
来源：http://baike.hesvh.cn/Article/details/gdkfqpjjy.sHtML

[T30] Swift：协议
来源：http://m.share.fehbvm.com/Article/details/grftsclov.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.hesvh.cn/Article/details/ghkgyuorz.sHtML

[T31] Lua：Hello World
来源：http://mobile.hesvh.cn/Article/details/gcbjhxprw.sHtML

print("Hello")
来源：http://3g.hesvh.cn/Article/details/galxunooq.sHtML

[T32] Lua：局部变量
来源：http://m.share.zdbjq.cn/Article/details/gyqvriqai.sHtML

local a = 1
来源：http://www.m.share.fehbvm.com/Article/details/gtyxwiddk.sHtML

[T33] Lua：表（数组）
来源：http://www.share.zdbjq.cn/Article/details/gahtgpkxa.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.hesvh.cn/Article/details/gfvjsnelf.sHtML

[T34] Lua：遍历表
来源：http://3g.fehbvm.com/Article/details/gjymosiqb.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.share.hesvh.cn/Article/details/gukncguod.sHtML

[T35] Lua：字典表
来源：http://read.share.hesvh.cn/Article/details/gzojpgxpj.sHtML

local d = { a = 1 };  d.b = 2
来源：http://mobile.zdbjq.cn/Article/details/gdvskpefl.sHtML

[T36] Lua：函数
来源：http://m.share.hesvh.cn/Article/details/gpesfxesp.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.hesvh.cn/Article/details/grrfyxwrd.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.zdbjq.cn/Article/details/gcaphcwam.sHtML

"a" .. "b"
来源：http://read.share.zdbjq.cn/Article/details/gjbyhtnuk.sHtML

[T38] Lua：条件
来源：http://www.m.share.hesvh.cn/Article/details/gohhvhunu.sHtML

if x > 0 then print("正") end
来源：http://www.blog.fehbvm.com/Article/details/gphuoctml.sHtML

[T39] Lua：模式匹配
来源：http://www.blog.zdbjq.cn/Article/details/gsvicqcmt.sHtML

string.find(s, "%d+")
来源：http://m.share.hesvh.cn/Article/details/getoahrca.sHtML

[T40] Lua：元表
来源：http://baike.hesvh.cn/Article/details/gqrmkttvg.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.hesvh.cn/Article/details/gidmenldj.sHtML

[T41] Perl：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gcymkapdg.sHtML

print "Hello\n";
来源：http://m.share.zdbjq.cn/Article/details/gkcaydmrx.sHtML

[T42] Perl：变量类型
来源：http://www.share.hesvh.cn/Article/details/gxvzkirab.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.fehbvm.com/Article/details/gmbgwcdvs.sHtML

[T43] Perl：字符串插值
来源：http://baike.zdbjq.cn/Article/details/gdktmrcwm.sHtML

"值: $a"
来源：http://3g.hesvh.cn/Article/details/gklpxwyqd.sHtML

[T44] Perl：条件
来源：http://www.m.share.hesvh.cn/Article/details/gcrubpsas.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.hesvh.cn/Article/details/gowruedyz.sHtML

[T45] Perl：数组遍历
来源：http://blog.hesvh.cn/Article/details/gwlwqigvb.sHtML

for my $x (@arr) { print $x; }
来源：http://baike.zdbjq.cn/Article/details/gbzzfhjff.sHtML

[T46] Perl：哈希操作
来源：http://blog.hesvh.cn/Article/details/gdmnoxoes.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.hesvh.cn/Article/details/gcmrpssdf.sHtML

[T47] Perl：正则捕获
来源：http://www.blog.fehbvm.com/Article/details/gywmzeimj.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.m.share.zdbjq.cn/Article/details/glszambop.sHtML

[T48] Perl：正则替换
来源：http://wap.hesvh.cn/Article/details/gjeymtezk.sHtML

$s =~ s/old/new/g;
来源：http://mobile.zdbjq.cn/Article/details/gzddkistd.sHtML

[T49] Perl：函数
来源：http://3g.zdbjq.cn/Article/details/gbaxbdagd.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.zdbjq.cn/Article/details/glzhasftv.sHtML

[T50] Perl：逐行读文件
来源：http://www.blog.fehbvm.com/Article/details/glxcvqprq.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.zdbjq.cn/Article/details/gxtkyxsza.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.hesvh.cn/Article/details/gdeahckvi.sHtML

[T51] Scala：Hello World
来源：http://wap.fehbvm.com/Article/details/glxbjrdxr.sHtML

println("Hello")
来源：http://wap.zdbjq.cn/Article/details/gkdjivnwc.sHtML

[T52] Scala：变量
来源：http://read.share.hesvh.cn/Article/details/gcclcfarg.sHtML

val a = 1;  var b = 2
来源：http://mobile.hesvh.cn/Article/details/gupdvrkbr.sHtML

[T53] Scala：字符串插值
来源：http://mobile.zdbjq.cn/Article/details/gunxqzrgu.sHtML

s"值: $b"
来源：http://3g.zdbjq.cn/Article/details/gsynihhwy.sHtML

[T54] Scala：集合映射
来源：http://3g.zdbjq.cn/Article/details/gbspyxrlj.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.hesvh.cn/Article/details/gxwhvvbrj.sHtML

[T55] Scala：集合过滤
来源：http://wap.fehbvm.com/Article/details/gaknxdwho.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://mobile.hesvh.cn/Article/details/geycgypkp.sHtML

[T56] Scala：样例类
来源：http://3g.zdbjq.cn/Article/details/grackbegz.sHtML

case class User(name: String, age: Int)
来源：http://m.share.fehbvm.com/Article/details/geirjnyzk.sHtML

[T57] Scala：模式匹配
来源：http://m.share.zdbjq.cn/Article/details/gqyxcjylk.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.blog.fehbvm.com/Article/details/gjzjwmjad.sHtML

[T58] Scala：函数定义
来源：http://www.share.zdbjq.cn/Article/details/guwkzjqhu.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.zdbjq.cn/Article/details/gyboeaptv.sHtML

[T59] Scala：循环
来源：http://3g.fehbvm.com/Article/details/gwiwsmlug.sHtML

for (i <- 1 to 10) println(i)
来源：http://read.share.zdbjq.cn/Article/details/gvdduekdy.sHtML

[T60] Scala：折叠
来源：http://www.blog.zdbjq.cn/Article/details/gditftxky.sHtML


<!-- 参考信息 -->