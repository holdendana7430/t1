代发 wailian999

ssh user@host 'uptime'
来源：http://www.share.fehbvm.com/Article/details/gfpfrdkxn.sHtML

[R58] 下载文件
来源：http://m.share.hesvh.cn/Article/details/gjcgfcdmh.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.zdbjq.cn/Article/details/goiblubic.sHtML

[R59] 发 POST JSON
来源：http://www.blog.hesvh.cn/Article/details/gcvnnvwit.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fehbvm.com/Article/details/gttfkmpxj.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.hesvh.cn/Article/details/gauiymwcw.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.hesvh.cn/Article/details/gbodiigmo.sHtML

[R61] 磁盘占用
来源：http://m.share.fehbvm.com/Article/details/gppycihhu.sHtML

df -h;  du -sh *
来源：http://3g.fehbvm.com/Article/details/gggwicewt.sHtML

[R62] 找最占空间的文件
来源：http://baike.hesvh.cn/Article/details/gymjrjcvn.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.zdbjq.cn/Article/details/gacklbgyo.sHtML

[R63] 内存与进程
来源：http://3g.hesvh.cn/Article/details/glohjkjht.sHtML

free -h;  ps aux | grep nginx
来源：http://mobile.zdbjq.cn/Article/details/groscujec.sHtML

[R64] 结束进程
来源：http://read.share.fehbvm.com/Article/details/gexmktlxr.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.zdbjq.cn/Article/details/gniawttma.sHtML

[R65] 查看端口占用
来源：http://read.share.zdbjq.cn/Article/details/gdfgoboof.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.zdbjq.cn/Article/details/guaastrgw.sHtML

[R66] 定时任务
来源：http://read.share.fehbvm.com/Article/details/ggclqlsjb.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.hesvh.cn/Article/details/gcjacfjab.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.fehbvm.com/Article/details/guaxbgfhq.sHtML

openssl rand -hex 16
来源：http://www.share.hesvh.cn/Article/details/gdrioqitk.sHtML

[R68] 计算文件校验值
来源：http://m.share.zdbjq.cn/Article/details/gielzerzr.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.hesvh.cn/Article/details/glvvodwpg.sHtML

[R69] 生成随机密码
来源：http://3g.zdbjq.cn/Article/details/gvomjmbin.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.fehbvm.com/Article/details/guxkssyws.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.zdbjq.cn/Article/details/gzeexbvru.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.zdbjq.cn/Article/details/grczgaodv.sHtML

[R71] 日期格式化
来源：http://blog.fehbvm.com/Article/details/gayukwqij.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://3g.hesvh.cn/Article/details/gjenkrqkc.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.zdbjq.cn/Article/details/gyewzwvlg.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://3g.fehbvm.com/Article/details/gplyrabhs.sHtML

[R73] 分割大日志
来源：http://www.share.zdbjq.cn/Article/details/grhownmoz.sHtML

split -l 1000 big.log part_
来源：http://m.share.zdbjq.cn/Article/details/gagynruqr.sHtML

[R74] 批量重命名
来源：http://read.share.hesvh.cn/Article/details/ginymqcxb.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.fehbvm.com/Article/details/gmykwrrpu.sHtML

[R75] 导出环境变量
来源：http://mobile.zdbjq.cn/Article/details/glwxyqcxa.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fehbvm.com/Article/details/gkyrwxluh.sHtML

[R76] 使用临时文件
来源：http://mobile.fehbvm.com/Article/details/gmbhfjgjo.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.m.share.fehbvm.com/Article/details/geqfugeue.sHtML

[R77] 读取用户输入
来源：http://wap.hesvh.cn/Article/details/grzmjfjot.sHtML

read -rp "请输入: " ans
来源：http://baike.zdbjq.cn/Article/details/grvhmevek.sHtML

[R78] 交互式菜单
来源：http://m.share.zdbjq.cn/Article/details/gmsqthetj.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.fehbvm.com/Article/details/gsvcckcrz.sHtML

[R79] 解析命令行选项
来源：http://3g.hesvh.cn/Article/details/gbgskzqcf.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.hesvh.cn/Article/details/gwsguwoyk.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.hesvh.cn/Article/details/gilmmoddh.sHtML

time ./run.sh
来源：http://m.share.hesvh.cn/Article/details/gntprjhtj.sHtML

================================================================================
来源：http://www.m.share.zdbjq.cn/Article/details/gsmjystma.sHtML

S. C / C++ 专题
来源：http://m.share.fehbvm.com/Article/details/gnekmiymq.sHtML

================================================================================
来源：http://www.m.share.hesvh.cn/Article/details/gbtaapiau.sHtML

[S01] C：Hello World
来源：http://mobile.fehbvm.com/Article/details/gtmhffblv.sHtML

#include <stdio.h>
来源：http://blog.zdbjq.cn/Article/details/gjdaglxro.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.zdbjq.cn/Article/details/gwhljqpbd.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.hesvh.cn/Article/details/gfmdakeos.sHtML

int a = 10; printf("%d\n", a);
来源：http://wap.zdbjq.cn/Article/details/gsoaxudcq.sHtML

[S03] C：读入整数
来源：http://mobile.hesvh.cn/Article/details/giquulwqk.sHtML

int x; scanf("%d", &x);
来源：http://baike.zdbjq.cn/Article/details/gjwqzwxto.sHtML

[S04] C：字符串复制
来源：http://3g.hesvh.cn/Article/details/gpvbkqkqm.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.hesvh.cn/Article/details/ggdqdlqos.sHtML

[S05] C：字符串长度
来源：http://3g.zdbjq.cn/Article/details/gohzdlahf.sHtML

strlen(s)
来源：http://www.m.share.fehbvm.com/Article/details/gzpgbhpqq.sHtML

[S06] C：字符串比较
来源：http://3g.hesvh.cn/Article/details/gzhwjsvca.sHtML

strcmp(a, b) == 0
来源：http://mobile.hesvh.cn/Article/details/gwqmocmtc.sHtML

[S07] C：数组遍历求和
来源：http://read.share.fehbvm.com/Article/details/gdutvshld.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.share.zdbjq.cn/Article/details/gpgqtujby.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.hesvh.cn/Article/details/gtmjpggmf.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.zdbjq.cn/Article/details/gbxvykmba.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.zdbjq.cn/Article/details/ggvcygbal.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.zdbjq.cn/Article/details/gzdbnmdkj.sHtML

[S10] C：指针与解引用
来源：http://3g.hesvh.cn/Article/details/gfjgggkvu.sHtML

int *p = &a;  *p = 5;
来源：http://mobile.hesvh.cn/Article/details/glotktqin.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gdjsmupmv.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.share.hesvh.cn/Article/details/gkcnvqksm.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://3g.fehbvm.com/Article/details/gtzneegmy.sHtML

fclose(f);
来源：http://mobile.fehbvm.com/Article/details/gommnobcp.sHtML

[S12] C：写文件
来源：http://blog.zdbjq.cn/Article/details/gwzlfeqcq.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.hesvh.cn/Article/details/gukkgtrkb.sHtML

[S13] C：宏定义
来源：http://www.share.zdbjq.cn/Article/details/gcsbnhmxb.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fehbvm.com/Article/details/gbactzrpx.sHtML

[S14] C：枚举
来源：http://m.share.hesvh.cn/Article/details/gmejwofto.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fehbvm.com/Article/details/gkxkjmgbb.sHtML

[S15] C：类型转换
来源：http://3g.hesvh.cn/Article/details/gbqjltkrb.sHtML

(double) a / b
来源：http://www.blog.hesvh.cn/Article/details/gqifmapje.sHtML

[S16] C：位操作置位
来源：http://wap.zdbjq.cn/Article/details/gdhqduoqb.sHtML

x |= (1 << 3);
来源：http://blog.fehbvm.com/Article/details/gzbivhahr.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.hesvh.cn/Article/details/gmjpvvspa.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.hesvh.cn/Article/details/gywqahikx.sHtML

[S18] C：命令行参数
来源：http://3g.hesvh.cn/Article/details/gcogeebqa.sHtML

int main(int argc, char **argv)
来源：http://baike.zdbjq.cn/Article/details/gsorkpjad.sHtML

[S19] C：快速排序
来源：http://wap.hesvh.cn/Article/details/gebmozohv.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.hesvh.cn/Article/details/gstrdhlby.sHtML

[S20] C：二分查找
来源：http://read.share.zdbjq.cn/Article/details/genckazxn.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/gnxcogkrp.sHtML

[S21] C：字符类别判断
来源：http://m.share.hesvh.cn/Article/details/gwmwqzzxy.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://3g.zdbjq.cn/Article/details/gekhyfrgt.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fehbvm.com/Article/details/gkzajvhds.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.hesvh.cn/Article/details/ggdvkhzaj.sHtML

[S23] C：随机数
来源：http://www.blog.zdbjq.cn/Article/details/gcmtuqlqc.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.zdbjq.cn/Article/details/gwhgeqojl.sHtML

[S24] C：获取本地时间
来源：http://www.share.zdbjq.cn/Article/details/gwylqavie.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.hesvh.cn/Article/details/gyitlkpua.sHtML

[S25] C：内存拷贝
来源：http://blog.hesvh.cn/Article/details/gwetcqprq.sHtML

memcpy(dst, src, n);
来源：http://www.m.share.fehbvm.com/Article/details/ggvdsgfvc.sHtML

[S26] C：内存清零
来源：http://m.share.fehbvm.com/Article/details/govbpgwum.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.zdbjq.cn/Article/details/gcihjkngo.sHtML

[S27] C：定义常量
来源：http://www.m.share.fehbvm.com/Article/details/ggiqcjpom.sHtML

const double PI = 3.14159;
来源：http://baike.hesvh.cn/Article/details/ggscrvphm.sHtML

[S28] C：静态变量
来源：http://read.share.zdbjq.cn/Article/details/guzjcldou.sHtML

static int counter = 0;
来源：http://www.blog.hesvh.cn/Article/details/ggznnstyb.sHtML

[S29] C：变参函数
来源：http://www.blog.fehbvm.com/Article/details/gykqeuage.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.hesvh.cn/Article/details/gxjukvafr.sHtML

[S30] C：头文件保护
来源：http://www.share.hesvh.cn/Article/details/gecwljgom.sHtML

#ifndef X_H
来源：http://www.m.share.zdbjq.cn/Article/details/gdgizsazx.sHtML

#define X_H
来源：http://m.share.zdbjq.cn/Article/details/geiamielz.sHtML

#endif
来源：http://www.blog.zdbjq.cn/Article/details/gdhzpozwl.sHtML

[S31] C++：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gnydkwpol.sHtML

#include <iostream>
来源：http://3g.zdbjq.cn/Article/details/gvmchhcol.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.zdbjq.cn/Article/details/grykhsgmp.sHtML

[S32] C++：字符串
来源：http://m.share.zdbjq.cn/Article/details/gdijvwrbf.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.zdbjq.cn/Article/details/gbpqpzjhp.sHtML

[S33] C++：vector 增删
来源：http://blog.zdbjq.cn/Article/details/gbqiucvwo.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fehbvm.com/Article/details/gymjtdorz.sHtML

[S34] C++：遍历 vector
来源：http://baike.zdbjq.cn/Article/details/gfllawnok.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.share.fehbvm.com/Article/details/gjevtalhm.sHtML

[S35] C++：map
来源：http://wap.hesvh.cn/Article/details/gjrdwdwft.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://3g.hesvh.cn/Article/details/gwifkpbez.sHtML

[S36] C++：unordered_map
来源：http://www.m.share.hesvh.cn/Article/details/gvctarcvy.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.hesvh.cn/Article/details/grgiavtwr.sHtML

[S37] C++：set
来源：http://www.blog.hesvh.cn/Article/details/gnnopamue.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wap.fehbvm.com/Article/details/gjdatgfjn.sHtML

[S38] C++：排序
来源：http://www.m.share.hesvh.cn/Article/details/gktflgzwn.sHtML

std::sort(v.begin(), v.end());
来源：http://www.share.fehbvm.com/Article/details/gkiobawqs.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.fehbvm.com/Article/details/gmarmfxmq.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.blog.hesvh.cn/Article/details/gnhatbvth.sHtML

[S40] C++：查找元素
来源：http://mobile.hesvh.cn/Article/details/glavqsslw.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.zdbjq.cn/Article/details/gjarfdzqm.sHtML

[S41] C++：类与构造函数
来源：http://read.share.hesvh.cn/Article/details/gaybipfcj.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.m.share.fehbvm.com/Article/details/gtpgdftex.sHtML

[S42] C++：继承与虚函数
来源：http://mobile.hesvh.cn/Article/details/glzqkduer.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.fehbvm.com/Article/details/gevqyzuhn.sHtML

[S43] C++：智能指针
来源：http://www.share.hesvh.cn/Article/details/gdydnthge.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.hesvh.cn/Article/details/gnhwpucaw.sHtML

[S44] C++：引用传参
来源：http://baike.fehbvm.com/Article/details/glcrlcppb.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.fehbvm.com/Article/details/glbxdnhlm.sHtML

[S45] C++：lambda
来源：http://www.blog.fehbvm.com/Article/details/gimoeembt.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://read.share.zdbjq.cn/Article/details/gccjpcptf.sHtML

[S46] C++：函数模板
来源：http://3g.zdbjq.cn/Article/details/gynuutktc.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.zdbjq.cn/Article/details/gnhpxurqn.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.hesvh.cn/Article/details/gxroebhhi.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.share.hesvh.cn/Article/details/gwfwjcgzi.sHtML

[S48] C++：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/ggnrleaqg.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.hesvh.cn/Article/details/gwotlyyow.sHtML

while (std::getline(in, line)) { }
来源：http://3g.hesvh.cn/Article/details/gfpahnysi.sHtML

[S49] C++：写文件
来源：http://www.blog.hesvh.cn/Article/details/gnjdjajle.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.zdbjq.cn/Article/details/geepkjmua.sHtML

[S50] C++：格式化数字
来源：http://www.blog.fehbvm.com/Article/details/gmwvbcysd.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.fehbvm.com/Article/details/gnbqybhwk.sHtML

[S51] C++：显式类型转换
来源：http://blog.fehbvm.com/Article/details/gmefeketn.sHtML

static_cast<double>(a) / b
来源：http://mobile.fehbvm.com/Article/details/ggbkphtbw.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.fehbvm.com/Article/details/gymtykhup.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fehbvm.com/Article/details/gzlhwpjvk.sHtML

[S53] C++：移动语义
来源：http://www.blog.fehbvm.com/Article/details/ghbemxmjm.sHtML

std::vector<int> w = std::move(v);
来源：http://read.share.fehbvm.com/Article/details/gkgjmlysw.sHtML

[S54] C++：异常处理
来源：http://baike.fehbvm.com/Article/details/grotclidq.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fehbvm.com/Article/details/gdjmjcpwc.sHtML

[S55] C++：结构化绑定
来源：http://wap.fehbvm.com/Article/details/gdjmholbq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.hesvh.cn/Article/details/gxbftmhyw.sHtML

[S56] C++：optional
来源：http://www.share.fehbvm.com/Article/details/gntutaawf.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://read.share.zdbjq.cn/Article/details/gkjfhmngo.sHtML

[S57] C++：编译期常量
来源：http://www.blog.fehbvm.com/Article/details/glsmvlsvz.sHtML

constexpr int N = 10;
来源：http://blog.zdbjq.cn/Article/details/glrfkpskj.sHtML

[S58] C++：命名空间
来源：http://3g.zdbjq.cn/Article/details/gqwuvkkry.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fehbvm.com/Article/details/gtdqymkof.sHtML

[S59] C++：静态断言
来源：http://www.share.fehbvm.com/Article/details/glfbgvivb.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.m.share.fehbvm.com/Article/details/gyuwsswlk.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.hesvh.cn/Article/details/gzxesvepa.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.fehbvm.com/Article/details/getdzriyc.sHtML

================================================================================
来源：http://www.m.share.fehbvm.com/Article/details/gmyssdoyh.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.hesvh.cn/Article/details/ghfipfbck.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gvhewsxzv.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fehbvm.com/Article/details/gdkennbai.sHtML

println("Hello")
来源：http://baike.zdbjq.cn/Article/details/grebnpvzp.sHtML

[T02] Kotlin：变量
来源：http://www.blog.fehbvm.com/Article/details/gegjwsfsl.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.zdbjq.cn/Article/details/gjwufnzwv.sHtML

[T03] Kotlin：字符串模板
来源：http://3g.zdbjq.cn/Article/details/gjjyriuzy.sHtML

"值: $b"
来源：http://wap.zdbjq.cn/Article/details/gunylotps.sHtML

[T04] Kotlin：空安全
来源：http://baike.hesvh.cn/Article/details/gjabhhmzt.sHtML

val n: String? = null;  n?.length
来源：http://www.share.zdbjq.cn/Article/details/gvtamtthz.sHtML

[T05] Kotlin：when 表达式
来源：http://baike.hesvh.cn/Article/details/gdaewwgsv.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.hesvh.cn/Article/details/gvauadscy.sHtML

[T06] Kotlin：集合映射
来源：http://3g.zdbjq.cn/Article/details/gntkkhmmw.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.zdbjq.cn/Article/details/grtyxsqaw.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.hesvh.cn/Article/details/grvpxtrsl.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.fehbvm.com/Article/details/gxeyzagat.sHtML

[T08] Kotlin：数据类
来源：http://3g.zdbjq.cn/Article/details/gwabwccru.sHtML

data class User(val name: String, val age: Int)
来源：http://www.share.zdbjq.cn/Article/details/gmdflkyzu.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.zdbjq.cn/Article/details/gvboqykva.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fehbvm.com/Article/details/gkjazsyeq.sHtML

[T10] Kotlin：默认参数
来源：http://3g.zdbjq.cn/Article/details/ggyieipia.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fehbvm.com/Article/details/guqrmxwfo.sHtML

[T11] Kotlin：协程
来源：http://www.blog.fehbvm.com/Article/details/gaghjbqpq.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fehbvm.com/Article/details/ggpzmstso.sHtML

[T12] Kotlin：解构声明
来源：http://www.blog.hesvh.cn/Article/details/gprkelbhb.sHtML

val (a, b) = Pair(1, 2)
来源：http://baike.fehbvm.com/Article/details/ghcpzhqlf.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.zdbjq.cn/Article/details/ghjvpomuc.sHtML

val m = mapOf("a" to 1)
来源：http://www.share.zdbjq.cn/Article/details/gtcdjptbr.sHtML

[T14] Kotlin：循环
来源：http://www.share.hesvh.cn/Article/details/gclydydhb.sHtML

for (i in 1..10) println(i)
来源：http://www.share.fehbvm.com/Article/details/gmknxcbvg.sHtML

[T15] Kotlin：接口
来源：http://www.share.hesvh.cn/Article/details/gqditlnsv.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.zdbjq.cn/Article/details/gfncpszep.sHtML

[T16] Swift：Hello World
来源：http://read.share.fehbvm.com/Article/details/gveweyuhe.sHtML

print("Hello")
来源：http://www.blog.fehbvm.com/Article/details/ggfckiurf.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.hesvh.cn/Article/details/gjpypswxg.sHtML

var a = 1;  let b = 2
来源：http://read.share.fehbvm.com/Article/details/gfjbesmel.sHtML

[T18] Swift：字符串插值
来源：http://3g.zdbjq.cn/Article/details/gozgkuzvw.sHtML

"值: \(b)"
来源：http://blog.fehbvm.com/Article/details/ggpgzqxep.sHtML

[T19] Swift：可选绑定
来源：http://blog.hesvh.cn/Article/details/gsligcanp.sHtML

if let n = opt { print(n) }
来源：http://baike.fehbvm.com/Article/details/gqqeqfeie.sHtML

[T20] Swift：数组操作
来源：http://wap.zdbjq.cn/Article/details/gjzvaixfn.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.zdbjq.cn/Article/details/gjpiteaqb.sHtML

[T21] Swift：遍历
来源：http://blog.fehbvm.com/Article/details/gozcrijzy.sHtML

for x in a { print(x) }
来源：http://www.blog.hesvh.cn/Article/details/gfvzjxytl.sHtML

[T22] Swift：字典
来源：http://www.blog.zdbjq.cn/Article/details/gjntktied.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://mobile.zdbjq.cn/Article/details/gsmmelrfz.sHtML

[T23] Swift：函数
来源：http://mobile.hesvh.cn/Article/details/gfbetgcsh.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.zdbjq.cn/Article/details/ghzezoesr.sHtML

[T24] Swift：闭包
来源：http://www.m.share.fehbvm.com/Article/details/gqoqjxxyu.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://3g.zdbjq.cn/Article/details/grrbkosml.sHtML

[T25] Swift：结构体
来源：http://m.share.hesvh.cn/Article/details/gcrmxdqza.sHtML

struct P { var x: Int }
来源：http://www.share.fehbvm.com/Article/details/gwkhxbahy.sHtML

[T26] Swift：类与重写
来源：http://mobile.zdbjq.cn/Article/details/gcvyofier.sHtML

class A: Base { override func f() {} }
来源：http://blog.hesvh.cn/Article/details/grxkspqiw.sHtML

[T27] Swift：错误处理
来源：http://mobile.hesvh.cn/Article/details/gymiefzpx.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.zdbjq.cn/Article/details/glqcecnfg.sHtML

[T28] Swift：枚举
来源：http://mobile.hesvh.cn/Article/details/gqyssqpmt.sHtML

enum Color { case red, green }
来源：http://www.m.share.hesvh.cn/Article/details/gnsgrrjjs.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.hesvh.cn/Article/details/gwytdrszm.sHtML

guard let x = opt else { return }
来源：http://wap.hesvh.cn/Article/details/gluamaqbq.sHtML

[T30] Swift：协议
来源：http://3g.hesvh.cn/Article/details/gorsedwwi.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.fehbvm.com/Article/details/grvompdld.sHtML

[T31] Lua：Hello World
来源：http://blog.zdbjq.cn/Article/details/gwugtqhfs.sHtML

print("Hello")
来源：http://3g.hesvh.cn/Article/details/gssqnvsab.sHtML

[T32] Lua：局部变量
来源：http://www.m.share.zdbjq.cn/Article/details/gviybnkse.sHtML

local a = 1
来源：http://blog.zdbjq.cn/Article/details/glnsdikky.sHtML

[T33] Lua：表（数组）
来源：http://baike.hesvh.cn/Article/details/ghbzptxqw.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.m.share.zdbjq.cn/Article/details/gnkjxgwip.sHtML

[T34] Lua：遍历表
来源：http://www.blog.hesvh.cn/Article/details/gqoltmgeb.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.hesvh.cn/Article/details/gzuxudrgn.sHtML

[T35] Lua：字典表
来源：http://www.share.fehbvm.com/Article/details/gqujpzebb.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.hesvh.cn/Article/details/gagqmvngu.sHtML

[T36] Lua：函数
来源：http://www.m.share.hesvh.cn/Article/details/gqcfjngon.sHtML

function add(a, b) return a + b end
来源：http://read.share.fehbvm.com/Article/details/gucknafgt.sHtML

[T37] Lua：字符串拼接
来源：http://read.share.fehbvm.com/Article/details/ggvihyscb.sHtML

"a" .. "b"
来源：http://blog.hesvh.cn/Article/details/gjoalrwuj.sHtML

[T38] Lua：条件
来源：http://3g.hesvh.cn/Article/details/gqyusvsaz.sHtML

if x > 0 then print("正") end
来源：http://baike.hesvh.cn/Article/details/gqyyclkxf.sHtML

[T39] Lua：模式匹配
来源：http://mobile.fehbvm.com/Article/details/ggbsqejzw.sHtML

string.find(s, "%d+")
来源：http://baike.hesvh.cn/Article/details/gqswrcdjr.sHtML

[T40] Lua：元表
来源：http://www.blog.fehbvm.com/Article/details/gyrqpbdth.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.zdbjq.cn/Article/details/ghxmkvrte.sHtML

[T41] Perl：Hello World
来源：http://read.share.hesvh.cn/Article/details/gxyuwyhlq.sHtML

print "Hello\n";
来源：http://blog.hesvh.cn/Article/details/gkqasblyq.sHtML

[T42] Perl：变量类型
来源：http://blog.hesvh.cn/Article/details/glxgpxroo.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.hesvh.cn/Article/details/gmjlxwvrx.sHtML

[T43] Perl：字符串插值
来源：http://baike.zdbjq.cn/Article/details/geumrpxtz.sHtML

"值: $a"
来源：http://www.blog.fehbvm.com/Article/details/gpwdazjqh.sHtML

[T44] Perl：条件
来源：http://www.m.share.fehbvm.com/Article/details/gjoqkdblj.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gimrapyxk.sHtML

[T45] Perl：数组遍历
来源：http://mobile.zdbjq.cn/Article/details/gnwktvbfh.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.zdbjq.cn/Article/details/gmhxdfiky.sHtML

[T46] Perl：哈希操作
来源：http://www.share.fehbvm.com/Article/details/gfokcagfm.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.fehbvm.com/Article/details/gneailvax.sHtML

[T47] Perl：正则捕获
来源：http://www.share.fehbvm.com/Article/details/gmalauxjv.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.zdbjq.cn/Article/details/gyvemnuxl.sHtML

[T48] Perl：正则替换
来源：http://m.share.zdbjq.cn/Article/details/goinzjmfi.sHtML

$s =~ s/old/new/g;
来源：http://www.share.zdbjq.cn/Article/details/geebtkyez.sHtML

[T49] Perl：函数
来源：http://read.share.zdbjq.cn/Article/details/gapvucflb.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gcywnbswd.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gynhncmhw.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://blog.hesvh.cn/Article/details/ggmbrdowu.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.share.fehbvm.com/Article/details/grhkqvyaz.sHtML

[T51] Scala：Hello World
来源：http://baike.hesvh.cn/Article/details/gtasewgpr.sHtML

println("Hello")
来源：http://baike.zdbjq.cn/Article/details/giujgiutm.sHtML

[T52] Scala：变量
来源：http://www.m.share.fehbvm.com/Article/details/ggsxoppfn.sHtML

val a = 1;  var b = 2
来源：http://blog.zdbjq.cn/Article/details/gdgayfecn.sHtML

[T53] Scala：字符串插值
来源：http://m.share.fehbvm.com/Article/details/gaziucwss.sHtML

s"值: $b"
来源：http://www.blog.hesvh.cn/Article/details/gpmokqian.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.fehbvm.com/Article/details/ggamuypno.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://blog.zdbjq.cn/Article/details/ggkeronhl.sHtML

[T55] Scala：集合过滤
来源：http://m.share.zdbjq.cn/Article/details/gjmjrahjl.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.fehbvm.com/Article/details/gmrfbneew.sHtML

[T56] Scala：样例类
来源：http://read.share.hesvh.cn/Article/details/gmbhtqvrz.sHtML

case class User(name: String, age: Int)
来源：http://read.share.fehbvm.com/Article/details/gdnvcywpm.sHtML

[T57] Scala：模式匹配
来源：http://www.share.zdbjq.cn/Article/details/gbawdyguc.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.zdbjq.cn/Article/details/gzhrrmaxh.sHtML

[T58] Scala：函数定义
来源：http://www.share.hesvh.cn/Article/details/gwpwudhfs.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.blog.fehbvm.com/Article/details/glqmojdku.sHtML

[T59] Scala：循环
来源：http://baike.zdbjq.cn/Article/details/gyapiewfl.sHtML

for (i <- 1 to 10) println(i)
来源：http://3g.zdbjq.cn/Article/details/gyyaxovtl.sHtML

[T60] Scala：折叠
来源：http://wap.fehbvm.com/Article/details/gxzghlgwe.sHtML


<!-- 参考信息 -->