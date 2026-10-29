代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.fehbvm.com/Article/details/gbrgvwhis.sHtML

[R52] 统计行数
来源：http://blog.hesvh.cn/Article/details/gbjdwsbsn.sHtML

wc -l a.txt
来源：http://blog.hesvh.cn/Article/details/gwmtgvoyn.sHtML

[R53] 查看文件头与实时尾
来源：http://www.share.hesvh.cn/Article/details/gxirqjcjt.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.m.share.zdbjq.cn/Article/details/gclypnsmr.sHtML

[R54] 比较两个文件
来源：http://mobile.hesvh.cn/Article/details/gbbkpvjky.sHtML

diff a.txt b.txt
来源：http://www.blog.zdbjq.cn/Article/details/glavsolds.sHtML

[R55] 压缩与解压
来源：http://blog.hesvh.cn/Article/details/gsamoruef.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.zdbjq.cn/Article/details/glhczztfg.sHtML

[R56] 远程拷贝
来源：http://mobile.zdbjq.cn/Article/details/goomhwdls.sHtML

scp file user@host:/path/
来源：http://www.m.share.zdbjq.cn/Article/details/gvtwememl.sHtML

[R57] 远程执行命令
来源：http://mobile.zdbjq.cn/Article/details/grbjgipuw.sHtML

ssh user@host 'uptime'
来源：http://www.share.zdbjq.cn/Article/details/gbxvuwopt.sHtML

[R58] 下载文件
来源：http://blog.zdbjq.cn/Article/details/ganbzabgx.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://blog.zdbjq.cn/Article/details/gdrbyaixd.sHtML

[R59] 发 POST JSON
来源：http://www.share.hesvh.cn/Article/details/grbsleimh.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://baike.zdbjq.cn/Article/details/gdqcwxddj.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fehbvm.com/Article/details/gjzapsvry.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://blog.zdbjq.cn/Article/details/gqczzjisv.sHtML

[R61] 磁盘占用
来源：http://baike.zdbjq.cn/Article/details/gexaquysq.sHtML

df -h;  du -sh *
来源：http://3g.hesvh.cn/Article/details/gurjkgtgm.sHtML

[R62] 找最占空间的文件
来源：http://read.share.zdbjq.cn/Article/details/gomemfnhj.sHtML

du -ah . | sort -rh | head -10
来源：http://mobile.zdbjq.cn/Article/details/gvohhpkxj.sHtML

[R63] 内存与进程
来源：http://blog.hesvh.cn/Article/details/geqyhucaq.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.zdbjq.cn/Article/details/givouiaoy.sHtML

[R64] 结束进程
来源：http://blog.hesvh.cn/Article/details/gfyjliejc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.zdbjq.cn/Article/details/gwejbaiqq.sHtML

[R65] 查看端口占用
来源：http://blog.fehbvm.com/Article/details/gmbiumzuo.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://m.share.hesvh.cn/Article/details/guwqqitwk.sHtML

[R66] 定时任务
来源：http://read.share.fehbvm.com/Article/details/gbpjawqjx.sHtML

crontab -e;  crontab -l
来源：http://mobile.zdbjq.cn/Article/details/gceghtdjn.sHtML

[R67] 生成随机十六进制串
来源：http://3g.hesvh.cn/Article/details/ggjpbuahk.sHtML

openssl rand -hex 16
来源：http://m.share.zdbjq.cn/Article/details/geclanjsr.sHtML

[R68] 计算文件校验值
来源：http://3g.zdbjq.cn/Article/details/gsbazmdqb.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://wap.zdbjq.cn/Article/details/gjruovkpt.sHtML

[R69] 生成随机密码
来源：http://www.blog.zdbjq.cn/Article/details/gdgulwsxk.sHtML

head -c 16 /dev/urandom | base64
来源：http://baike.fehbvm.com/Article/details/gsriwyyhf.sHtML

[R70] 时间戳与互转
来源：http://3g.fehbvm.com/Article/details/gatxusmpc.sHtML

date +%s;  date -d @1700000000
来源：http://read.share.hesvh.cn/Article/details/gzilethsv.sHtML

[R71] 日期格式化
来源：http://wap.zdbjq.cn/Article/details/gcgtoafas.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.hesvh.cn/Article/details/grgcatwuq.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.fehbvm.com/Article/details/gaenxdohe.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.fehbvm.com/Article/details/gnlqrcqfc.sHtML

[R73] 分割大日志
来源：http://www.blog.hesvh.cn/Article/details/gbcahltio.sHtML

split -l 1000 big.log part_
来源：http://wap.zdbjq.cn/Article/details/gspmvdbwi.sHtML

[R74] 批量重命名
来源：http://3g.fehbvm.com/Article/details/gnkofefev.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://blog.hesvh.cn/Article/details/ggslwgpkg.sHtML

[R75] 导出环境变量
来源：http://mobile.zdbjq.cn/Article/details/gujpjdxxj.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.m.share.zdbjq.cn/Article/details/gbumewbvo.sHtML

[R76] 使用临时文件
来源：http://3g.hesvh.cn/Article/details/gkpagkvji.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/guihccfql.sHtML

[R77] 读取用户输入
来源：http://mobile.hesvh.cn/Article/details/gihvqvdrb.sHtML

read -rp "请输入: " ans
来源：http://blog.zdbjq.cn/Article/details/goptrgsfy.sHtML

[R78] 交互式菜单
来源：http://www.share.hesvh.cn/Article/details/gbmhxwjby.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://baike.hesvh.cn/Article/details/gapmsqbdu.sHtML

[R79] 解析命令行选项
来源：http://www.blog.hesvh.cn/Article/details/gamcxlclh.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.zdbjq.cn/Article/details/gtpzxzoxj.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.zdbjq.cn/Article/details/gqgxiipug.sHtML

time ./run.sh
来源：http://read.share.hesvh.cn/Article/details/gygfhgsun.sHtML

================================================================================
来源：http://wap.hesvh.cn/Article/details/gfrohucqk.sHtML

S. C / C++ 专题
来源：http://read.share.hesvh.cn/Article/details/gklxmdasy.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gvblqrafb.sHtML

[S01] C：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gshsnlvks.sHtML

#include <stdio.h>
来源：http://m.share.hesvh.cn/Article/details/gswepijeh.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fehbvm.com/Article/details/glpywyqsi.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.hesvh.cn/Article/details/gcyjgbyky.sHtML

int a = 10; printf("%d\n", a);
来源：http://baike.fehbvm.com/Article/details/gdwughgcb.sHtML

[S03] C：读入整数
来源：http://read.share.hesvh.cn/Article/details/gfsmelssj.sHtML

int x; scanf("%d", &x);
来源：http://blog.zdbjq.cn/Article/details/gajatrngn.sHtML

[S04] C：字符串复制
来源：http://m.share.fehbvm.com/Article/details/gmhcfqbnf.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.zdbjq.cn/Article/details/gqcbimlrn.sHtML

[S05] C：字符串长度
来源：http://3g.zdbjq.cn/Article/details/gmjogbfdr.sHtML

strlen(s)
来源：http://baike.fehbvm.com/Article/details/gmozhfkss.sHtML

[S06] C：字符串比较
来源：http://mobile.zdbjq.cn/Article/details/gfftczjzj.sHtML

strcmp(a, b) == 0
来源：http://blog.fehbvm.com/Article/details/gtxpohvzd.sHtML

[S07] C：数组遍历求和
来源：http://m.share.fehbvm.com/Article/details/gmvqoycad.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.hesvh.cn/Article/details/gyhbvxqte.sHtML

[S08] C：动态内存分配与释放
来源：http://baike.zdbjq.cn/Article/details/gezilbrca.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://blog.hesvh.cn/Article/details/gexokwwhl.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.hesvh.cn/Article/details/gsgfwilyq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://baike.zdbjq.cn/Article/details/gxmcpcvto.sHtML

[S10] C：指针与解引用
来源：http://blog.hesvh.cn/Article/details/ghnnkiglc.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.zdbjq.cn/Article/details/gymrjnykf.sHtML

[S11] C：逐行读文件
来源：http://m.share.hesvh.cn/Article/details/ghdunnuqb.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fehbvm.com/Article/details/gidzstlxb.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.zdbjq.cn/Article/details/ggydaeuab.sHtML

fclose(f);
来源：http://baike.hesvh.cn/Article/details/goclaprny.sHtML

[S12] C：写文件
来源：http://blog.zdbjq.cn/Article/details/gbvseuclu.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://3g.fehbvm.com/Article/details/geglbyscj.sHtML

[S13] C：宏定义
来源：http://3g.zdbjq.cn/Article/details/gvbyvxgxd.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fehbvm.com/Article/details/glcsfpjwa.sHtML

[S14] C：枚举
来源：http://www.m.share.hesvh.cn/Article/details/gfygokris.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.m.share.hesvh.cn/Article/details/gixymgwmw.sHtML

[S15] C：类型转换
来源：http://www.blog.fehbvm.com/Article/details/ghrcwzjlu.sHtML

(double) a / b
来源：http://m.share.fehbvm.com/Article/details/gopuyhmef.sHtML

[S16] C：位操作置位
来源：http://www.share.zdbjq.cn/Article/details/gscdmvxbf.sHtML

x |= (1 << 3);
来源：http://wap.hesvh.cn/Article/details/ghggbqaor.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.hesvh.cn/Article/details/gphriqfoo.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.hesvh.cn/Article/details/gyuvgfyhe.sHtML

[S18] C：命令行参数
来源：http://3g.fehbvm.com/Article/details/gvcizjkbr.sHtML

int main(int argc, char **argv)
来源：http://wap.zdbjq.cn/Article/details/gqpbyhsss.sHtML

[S19] C：快速排序
来源：http://www.m.share.zdbjq.cn/Article/details/gapnxenit.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://m.share.fehbvm.com/Article/details/gaondojcj.sHtML

[S20] C：二分查找
来源：http://www.share.fehbvm.com/Article/details/gfvbkrgrb.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.fehbvm.com/Article/details/glszppomu.sHtML

[S21] C：字符类别判断
来源：http://blog.fehbvm.com/Article/details/gxylovysz.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://m.share.hesvh.cn/Article/details/gwobxxvya.sHtML

[S22] C：字符串转数字
来源：http://www.share.zdbjq.cn/Article/details/gyryzaxua.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fehbvm.com/Article/details/gvbtsiqab.sHtML

[S23] C：随机数
来源：http://m.share.zdbjq.cn/Article/details/gxnikznln.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://blog.hesvh.cn/Article/details/gnetfvvum.sHtML

[S24] C：获取本地时间
来源：http://baike.hesvh.cn/Article/details/gwvjkdatq.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.zdbjq.cn/Article/details/gkloolisl.sHtML

[S25] C：内存拷贝
来源：http://www.share.hesvh.cn/Article/details/goitkzfmb.sHtML

memcpy(dst, src, n);
来源：http://3g.zdbjq.cn/Article/details/gzoimzdty.sHtML

[S26] C：内存清零
来源：http://www.m.share.fehbvm.com/Article/details/gynqatuct.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.hesvh.cn/Article/details/geunglluw.sHtML

[S27] C：定义常量
来源：http://www.m.share.fehbvm.com/Article/details/grtnpeesb.sHtML

const double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gylqdihye.sHtML

[S28] C：静态变量
来源：http://m.share.zdbjq.cn/Article/details/giktwunpi.sHtML

static int counter = 0;
来源：http://www.blog.hesvh.cn/Article/details/grjiigwau.sHtML

[S29] C：变参函数
来源：http://read.share.fehbvm.com/Article/details/goxwanvbk.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.zdbjq.cn/Article/details/gsyajnuvo.sHtML

[S30] C：头文件保护
来源：http://www.share.hesvh.cn/Article/details/grnuuwtvc.sHtML

#ifndef X_H
来源：http://m.share.zdbjq.cn/Article/details/gokaqqtek.sHtML

#define X_H
来源：http://baike.fehbvm.com/Article/details/gawzehdrg.sHtML

#endif
来源：http://www.share.zdbjq.cn/Article/details/ganxsjouw.sHtML

[S31] C++：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gilwrxikc.sHtML

#include <iostream>
来源：http://baike.zdbjq.cn/Article/details/gnkiwgzii.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.hesvh.cn/Article/details/gydgamxuh.sHtML

[S32] C++：字符串
来源：http://wap.fehbvm.com/Article/details/gtolmqmyq.sHtML

std::string s = "hi";  s += "!";
来源：http://3g.zdbjq.cn/Article/details/gtdsojfiy.sHtML

[S33] C++：vector 增删
来源：http://wap.zdbjq.cn/Article/details/giqldetsb.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://m.share.hesvh.cn/Article/details/gjhnxigca.sHtML

[S34] C++：遍历 vector
来源：http://m.share.hesvh.cn/Article/details/gucgjompt.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://mobile.fehbvm.com/Article/details/gknuvixcd.sHtML

[S35] C++：map
来源：http://www.share.fehbvm.com/Article/details/glbtbdsdl.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wap.fehbvm.com/Article/details/grtxeqcno.sHtML

[S36] C++：unordered_map
来源：http://wap.fehbvm.com/Article/details/gpnfotkyi.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.hesvh.cn/Article/details/gpazgsrtu.sHtML

[S37] C++：set
来源：http://www.share.zdbjq.cn/Article/details/gidyrcdlj.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://read.share.zdbjq.cn/Article/details/gkuobjwjv.sHtML

[S38] C++：排序
来源：http://baike.hesvh.cn/Article/details/gpziosnmh.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.zdbjq.cn/Article/details/gfirbblqc.sHtML

[S39] C++：自定义比较器排序
来源：http://baike.zdbjq.cn/Article/details/gxeritybc.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.share.fehbvm.com/Article/details/ggznmkyxu.sHtML

[S40] C++：查找元素
来源：http://read.share.zdbjq.cn/Article/details/gnqwhbrqh.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.hesvh.cn/Article/details/gmnqmqfho.sHtML

[S41] C++：类与构造函数
来源：http://m.share.hesvh.cn/Article/details/ggebnfmua.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.hesvh.cn/Article/details/gjzwcnloq.sHtML

[S42] C++：继承与虚函数
来源：http://www.blog.fehbvm.com/Article/details/gmooaavtw.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.fehbvm.com/Article/details/gpbhhplmj.sHtML

[S43] C++：智能指针
来源：http://wap.fehbvm.com/Article/details/guzkefevq.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.fehbvm.com/Article/details/grwieqnkx.sHtML

[S44] C++：引用传参
来源：http://baike.zdbjq.cn/Article/details/gowdnwzsx.sHtML

void inc(int &x) { ++x; }
来源：http://www.m.share.zdbjq.cn/Article/details/gpnsqhfgk.sHtML

[S45] C++：lambda
来源：http://3g.fehbvm.com/Article/details/gmvzumgjb.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.hesvh.cn/Article/details/ghnwltoeu.sHtML

[S46] C++：函数模板
来源：http://wap.hesvh.cn/Article/details/guhfdkigf.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mobile.zdbjq.cn/Article/details/gwzobahue.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.zdbjq.cn/Article/details/gqbemxdao.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.hesvh.cn/Article/details/gqrdfwqbx.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gdjmmqcrp.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://mobile.hesvh.cn/Article/details/girqgubia.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fehbvm.com/Article/details/ghoyvsknp.sHtML

[S49] C++：写文件
来源：http://m.share.zdbjq.cn/Article/details/gbechihsa.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.hesvh.cn/Article/details/gutyxloao.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.zdbjq.cn/Article/details/gxyvhhivl.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://3g.hesvh.cn/Article/details/gsqoumysh.sHtML

[S51] C++：显式类型转换
来源：http://mobile.zdbjq.cn/Article/details/gnpqvpqts.sHtML

static_cast<double>(a) / b
来源：http://www.share.fehbvm.com/Article/details/gkkthwsqf.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fehbvm.com/Article/details/gndbielsp.sHtML

int size() const noexcept { return n_; }
来源：http://wap.hesvh.cn/Article/details/gqsxwemfu.sHtML

[S53] C++：移动语义
来源：http://www.share.hesvh.cn/Article/details/ghmgfdzte.sHtML

std::vector<int> w = std::move(v);
来源：http://baike.fehbvm.com/Article/details/ghwoqhvbg.sHtML

[S54] C++：异常处理
来源：http://m.share.fehbvm.com/Article/details/gjasqzoyl.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.zdbjq.cn/Article/details/gysnpaiot.sHtML

[S55] C++：结构化绑定
来源：http://m.share.hesvh.cn/Article/details/gdrbzfueb.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.zdbjq.cn/Article/details/gomurtmkp.sHtML

[S56] C++：optional
来源：http://baike.hesvh.cn/Article/details/gzzwqjcfl.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fehbvm.com/Article/details/ghjhkmjdz.sHtML

[S57] C++：编译期常量
来源：http://3g.fehbvm.com/Article/details/gbpyjatdf.sHtML

constexpr int N = 10;
来源：http://baike.zdbjq.cn/Article/details/gfvuofeao.sHtML

[S58] C++：命名空间
来源：http://m.share.zdbjq.cn/Article/details/gqwqvgdno.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.hesvh.cn/Article/details/gogmpifuv.sHtML

[S59] C++：静态断言
来源：http://blog.zdbjq.cn/Article/details/gmsftzdlr.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://baike.zdbjq.cn/Article/details/gpgsbangc.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.hesvh.cn/Article/details/guzauopym.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.zdbjq.cn/Article/details/gvfspyvbt.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gmbzvztqk.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.fehbvm.com/Article/details/gquujmwhg.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gkrmlucex.sHtML

[T01] Kotlin：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gdenimxkg.sHtML

println("Hello")
来源：http://read.share.hesvh.cn/Article/details/gcwrhxfql.sHtML

[T02] Kotlin：变量
来源：http://www.blog.hesvh.cn/Article/details/gtfwvlcdi.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fehbvm.com/Article/details/gdpvieluu.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.hesvh.cn/Article/details/gvuugkzbi.sHtML

"值: $b"
来源：http://www.m.share.hesvh.cn/Article/details/gmcgjngth.sHtML

[T04] Kotlin：空安全
来源：http://m.share.fehbvm.com/Article/details/grrtbotol.sHtML

val n: String? = null;  n?.length
来源：http://read.share.zdbjq.cn/Article/details/guuiposlq.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.zdbjq.cn/Article/details/gjenqncif.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.m.share.hesvh.cn/Article/details/gmuvvaebc.sHtML

[T06] Kotlin：集合映射
来源：http://wap.fehbvm.com/Article/details/gggerigyo.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.zdbjq.cn/Article/details/gixfbgvff.sHtML

[T07] Kotlin：集合过滤
来源：http://read.share.hesvh.cn/Article/details/gfxnhmygb.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fehbvm.com/Article/details/glqahpxpm.sHtML

[T08] Kotlin：数据类
来源：http://blog.fehbvm.com/Article/details/gidzdywhd.sHtML

data class User(val name: String, val age: Int)
来源：http://baike.zdbjq.cn/Article/details/geniacuui.sHtML

[T09] Kotlin：扩展函数
来源：http://www.share.zdbjq.cn/Article/details/gpjqlsldf.sHtML

fun String.exclaim() = this + "!"
来源：http://blog.fehbvm.com/Article/details/gwudxkvcn.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.fehbvm.com/Article/details/gfxzndgde.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://www.share.hesvh.cn/Article/details/grougvzxa.sHtML

[T11] Kotlin：协程
来源：http://www.blog.hesvh.cn/Article/details/geniqcisn.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.fehbvm.com/Article/details/gqvafjzys.sHtML

[T12] Kotlin：解构声明
来源：http://wap.zdbjq.cn/Article/details/gwxcjypke.sHtML

val (a, b) = Pair(1, 2)
来源：http://mobile.fehbvm.com/Article/details/gjzqwchgw.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.fehbvm.com/Article/details/gsrvhgggt.sHtML

val m = mapOf("a" to 1)
来源：http://baike.fehbvm.com/Article/details/gskugjddp.sHtML

[T14] Kotlin：循环
来源：http://wap.hesvh.cn/Article/details/gwzorlsir.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.zdbjq.cn/Article/details/gxwrulahp.sHtML

[T15] Kotlin：接口
来源：http://mobile.zdbjq.cn/Article/details/gduzzmqvw.sHtML

interface Shape { fun area(): Double }
来源：http://baike.zdbjq.cn/Article/details/gbvoleqpj.sHtML

[T16] Swift：Hello World
来源：http://wap.fehbvm.com/Article/details/gwqqkxodw.sHtML

print("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/gtgsttohz.sHtML

[T17] Swift：变量与常量
来源：http://mobile.fehbvm.com/Article/details/gobbfxnyx.sHtML

var a = 1;  let b = 2
来源：http://m.share.zdbjq.cn/Article/details/gcrznsbbv.sHtML

[T18] Swift：字符串插值
来源：http://m.share.zdbjq.cn/Article/details/gacoasmai.sHtML

"值: \(b)"
来源：http://baike.zdbjq.cn/Article/details/gaakckian.sHtML

[T19] Swift：可选绑定
来源：http://read.share.zdbjq.cn/Article/details/gbpdupewm.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.fehbvm.com/Article/details/gsmqrnzqe.sHtML

[T20] Swift：数组操作
来源：http://www.blog.zdbjq.cn/Article/details/gbbrnzhjd.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.fehbvm.com/Article/details/gvlrvhtij.sHtML

[T21] Swift：遍历
来源：http://m.share.hesvh.cn/Article/details/gipwkwjzt.sHtML

for x in a { print(x) }
来源：http://3g.fehbvm.com/Article/details/gvbyheqjr.sHtML

[T22] Swift：字典
来源：http://read.share.hesvh.cn/Article/details/gevsadtzc.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.zdbjq.cn/Article/details/gfxabytnv.sHtML

[T23] Swift：函数
来源：http://www.share.hesvh.cn/Article/details/ggtevhpro.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.hesvh.cn/Article/details/gdfvbxhyg.sHtML

[T24] Swift：闭包
来源：http://read.share.hesvh.cn/Article/details/gesgyzxzi.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.fehbvm.com/Article/details/gqjvyvyyo.sHtML

[T25] Swift：结构体
来源：http://read.share.fehbvm.com/Article/details/gzawkkpgv.sHtML

struct P { var x: Int }
来源：http://wap.hesvh.cn/Article/details/gcynzkyua.sHtML

[T26] Swift：类与重写
来源：http://read.share.fehbvm.com/Article/details/geanstjht.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.fehbvm.com/Article/details/glrqkcmtj.sHtML

[T27] Swift：错误处理
来源：http://www.share.fehbvm.com/Article/details/gzowztbpv.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.zdbjq.cn/Article/details/gtiezvwzh.sHtML

[T28] Swift：枚举
来源：http://m.share.fehbvm.com/Article/details/gcbjxsqzi.sHtML

enum Color { case red, green }
来源：http://baike.zdbjq.cn/Article/details/ggmvcsibs.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.zdbjq.cn/Article/details/gshqvaqzj.sHtML

guard let x = opt else { return }
来源：http://3g.hesvh.cn/Article/details/geikrdmsw.sHtML

[T30] Swift：协议
来源：http://m.share.hesvh.cn/Article/details/gyuagevty.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.hesvh.cn/Article/details/gabpifezg.sHtML

[T31] Lua：Hello World
来源：http://www.blog.zdbjq.cn/Article/details/gzrchcqjm.sHtML

print("Hello")
来源：http://wap.fehbvm.com/Article/details/grglpomlw.sHtML

[T32] Lua：局部变量
来源：http://mobile.fehbvm.com/Article/details/gzyoxcybx.sHtML

local a = 1
来源：http://blog.zdbjq.cn/Article/details/gkjpdxjet.sHtML

[T33] Lua：表（数组）
来源：http://3g.hesvh.cn/Article/details/gmsvxjdos.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.fehbvm.com/Article/details/gyytaijsm.sHtML

[T34] Lua：遍历表
来源：http://wap.zdbjq.cn/Article/details/grmuuuxlg.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://blog.hesvh.cn/Article/details/gwkhjbjfd.sHtML

[T35] Lua：字典表
来源：http://3g.zdbjq.cn/Article/details/gdsslezcv.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.hesvh.cn/Article/details/guvbiqtqv.sHtML

[T36] Lua：函数
来源：http://www.blog.fehbvm.com/Article/details/gonycgzcm.sHtML

function add(a, b) return a + b end
来源：http://m.share.zdbjq.cn/Article/details/gyuowlzfp.sHtML

[T37] Lua：字符串拼接
来源：http://mobile.hesvh.cn/Article/details/glbmjwluq.sHtML

"a" .. "b"
来源：http://wap.fehbvm.com/Article/details/gopbrridf.sHtML

[T38] Lua：条件
来源：http://baike.fehbvm.com/Article/details/guojnjvql.sHtML

if x > 0 then print("正") end
来源：http://www.share.zdbjq.cn/Article/details/gtvigymjc.sHtML

[T39] Lua：模式匹配
来源：http://wap.fehbvm.com/Article/details/gdcavhetc.sHtML

string.find(s, "%d+")
来源：http://www.blog.zdbjq.cn/Article/details/gnzvmszwd.sHtML

[T40] Lua：元表
来源：http://mobile.hesvh.cn/Article/details/gknxdinlh.sHtML

setmetatable({}, { __index = base })
来源：http://www.m.share.fehbvm.com/Article/details/gtpwfwzwv.sHtML

[T41] Perl：Hello World
来源：http://baike.hesvh.cn/Article/details/gdvhlfktj.sHtML

print "Hello\n";
来源：http://m.share.zdbjq.cn/Article/details/gwzvlibkv.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.fehbvm.com/Article/details/gyrnylwpq.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.zdbjq.cn/Article/details/gqlioauku.sHtML

[T43] Perl：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gezsmynzo.sHtML

"值: $a"
来源：http://blog.hesvh.cn/Article/details/gewrmudmf.sHtML

[T44] Perl：条件
来源：http://mobile.hesvh.cn/Article/details/ghvuxnsis.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.hesvh.cn/Article/details/ghthxpvrt.sHtML

[T45] Perl：数组遍历
来源：http://3g.fehbvm.com/Article/details/gaeyvizaj.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.zdbjq.cn/Article/details/ghkbfhhfn.sHtML

[T46] Perl：哈希操作
来源：http://mobile.hesvh.cn/Article/details/gafrlunie.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.zdbjq.cn/Article/details/gcqntvaqs.sHtML

[T47] Perl：正则捕获
来源：http://www.m.share.zdbjq.cn/Article/details/gkokblifv.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.fehbvm.com/Article/details/gnwmacazu.sHtML

[T48] Perl：正则替换
来源：http://mobile.fehbvm.com/Article/details/gqcwzucgf.sHtML

$s =~ s/old/new/g;
来源：http://mobile.hesvh.cn/Article/details/gorzyccla.sHtML

[T49] Perl：函数
来源：http://mobile.hesvh.cn/Article/details/ggyukpsce.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.fehbvm.com/Article/details/gqzluegbk.sHtML

[T50] Perl：逐行读文件
来源：http://mobile.hesvh.cn/Article/details/gaqckbpjh.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.hesvh.cn/Article/details/gouisneys.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://baike.fehbvm.com/Article/details/gyldrdbrd.sHtML

[T51] Scala：Hello World
来源：http://mobile.hesvh.cn/Article/details/gnmsbrqfx.sHtML

println("Hello")
来源：http://www.m.share.fehbvm.com/Article/details/ggjrhjcjt.sHtML

[T52] Scala：变量
来源：http://blog.fehbvm.com/Article/details/gwopgzjdq.sHtML

val a = 1;  var b = 2
来源：http://baike.zdbjq.cn/Article/details/gkladwxha.sHtML

[T53] Scala：字符串插值
来源：http://blog.hesvh.cn/Article/details/ggpqpchmk.sHtML

s"值: $b"
来源：http://mobile.fehbvm.com/Article/details/gpiiydnfg.sHtML

[T54] Scala：集合映射
来源：http://www.share.zdbjq.cn/Article/details/gcgtgzafs.sHtML


<!-- 参考信息 -->