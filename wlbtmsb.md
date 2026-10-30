代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wap.hesvh.cn/Article/details/goamsykxu.sHtML

[R54] 比较两个文件
来源：http://mobile.zdbjq.cn/Article/details/gcwmqyyfh.sHtML

diff a.txt b.txt
来源：http://m.share.hesvh.cn/Article/details/gqryaojma.sHtML

[R55] 压缩与解压
来源：http://3g.zdbjq.cn/Article/details/gaywssqah.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://www.m.share.zdbjq.cn/Article/details/gkpqwwyhp.sHtML

[R56] 远程拷贝
来源：http://blog.fehbvm.com/Article/details/gnyayvond.sHtML

scp file user@host:/path/
来源：http://m.share.hesvh.cn/Article/details/gejzwezgx.sHtML

[R57] 远程执行命令
来源：http://wap.fehbvm.com/Article/details/gabthgjbw.sHtML

ssh user@host 'uptime'
来源：http://www.blog.fehbvm.com/Article/details/gdgexasmz.sHtML

[R58] 下载文件
来源：http://baike.fehbvm.com/Article/details/gkgnpnlcs.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://m.share.zdbjq.cn/Article/details/gaxygqdqz.sHtML

[R59] 发 POST JSON
来源：http://baike.zdbjq.cn/Article/details/gwymmqnra.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.fehbvm.com/Article/details/gawgfifqv.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.fehbvm.com/Article/details/gcnngjbiy.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://read.share.zdbjq.cn/Article/details/gnxpqevww.sHtML

[R61] 磁盘占用
来源：http://3g.zdbjq.cn/Article/details/ggwlauxcp.sHtML

df -h;  du -sh *
来源：http://www.m.share.hesvh.cn/Article/details/gazplklnf.sHtML

[R62] 找最占空间的文件
来源：http://3g.zdbjq.cn/Article/details/gplppezrg.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.hesvh.cn/Article/details/gfkilsxnu.sHtML

[R63] 内存与进程
来源：http://mobile.hesvh.cn/Article/details/gwogtfvyu.sHtML

free -h;  ps aux | grep nginx
来源：http://baike.zdbjq.cn/Article/details/gsxtfexjh.sHtML

[R64] 结束进程
来源：http://www.m.share.zdbjq.cn/Article/details/ggthqplfk.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.m.share.zdbjq.cn/Article/details/gcswwybom.sHtML

[R65] 查看端口占用
来源：http://www.share.fehbvm.com/Article/details/gyoowpbtj.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.zdbjq.cn/Article/details/ggetdgnuk.sHtML

[R66] 定时任务
来源：http://blog.fehbvm.com/Article/details/gavhgwrlk.sHtML

crontab -e;  crontab -l
来源：http://www.share.hesvh.cn/Article/details/gsrjmytpe.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.zdbjq.cn/Article/details/gpxhcllsu.sHtML

openssl rand -hex 16
来源：http://blog.fehbvm.com/Article/details/gjsymeqln.sHtML

[R68] 计算文件校验值
来源：http://mobile.fehbvm.com/Article/details/gbsqzotzd.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.zdbjq.cn/Article/details/gwpmuyyxd.sHtML

[R69] 生成随机密码
来源：http://wap.fehbvm.com/Article/details/glkifkhce.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.m.share.fehbvm.com/Article/details/ghpixdrsu.sHtML

[R70] 时间戳与互转
来源：http://www.share.zdbjq.cn/Article/details/galdoguno.sHtML

date +%s;  date -d @1700000000
来源：http://m.share.zdbjq.cn/Article/details/gabtdqcsp.sHtML

[R71] 日期格式化
来源：http://www.m.share.hesvh.cn/Article/details/gbwgsymsf.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.hesvh.cn/Article/details/gnouotawq.sHtML

[R72] 等待端口就绪
来源：http://m.share.fehbvm.com/Article/details/ghyuevujp.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.share.hesvh.cn/Article/details/gpcljcelq.sHtML

[R73] 分割大日志
来源：http://m.share.zdbjq.cn/Article/details/gzdeyiweu.sHtML

split -l 1000 big.log part_
来源：http://wap.hesvh.cn/Article/details/giclatpoi.sHtML

[R74] 批量重命名
来源：http://www.m.share.zdbjq.cn/Article/details/gzszyrcas.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://3g.zdbjq.cn/Article/details/gypnednjv.sHtML

[R75] 导出环境变量
来源：http://baike.fehbvm.com/Article/details/ghuklsigb.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.zdbjq.cn/Article/details/goqsvpjuc.sHtML

[R76] 使用临时文件
来源：http://m.share.fehbvm.com/Article/details/gyufoycvt.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.zdbjq.cn/Article/details/gdxlgfmio.sHtML

[R77] 读取用户输入
来源：http://blog.fehbvm.com/Article/details/gzafzcupj.sHtML

read -rp "请输入: " ans
来源：http://m.share.fehbvm.com/Article/details/gpzlgaqgf.sHtML

[R78] 交互式菜单
来源：http://blog.hesvh.cn/Article/details/glvwsmzjg.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.blog.hesvh.cn/Article/details/glfzxllbx.sHtML

[R79] 解析命令行选项
来源：http://www.blog.hesvh.cn/Article/details/gcopsnnmk.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://blog.fehbvm.com/Article/details/gqqcjnnqn.sHtML

[R80] 查看脚本执行耗时
来源：http://baike.fehbvm.com/Article/details/ghjlzocgx.sHtML

time ./run.sh
来源：http://wap.zdbjq.cn/Article/details/ggpxgoqzh.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/gtpvydqvg.sHtML

S. C / C++ 专题
来源：http://blog.fehbvm.com/Article/details/gwftcalqu.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gfiixsbfa.sHtML

[S01] C：Hello World
来源：http://3g.hesvh.cn/Article/details/gtttsiqck.sHtML

#include <stdio.h>
来源：http://blog.hesvh.cn/Article/details/ggyxayvrh.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.zdbjq.cn/Article/details/gprpcsqkh.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.hesvh.cn/Article/details/gplnnffxv.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fehbvm.com/Article/details/gzwswkvtm.sHtML

[S03] C：读入整数
来源：http://www.share.fehbvm.com/Article/details/gcgsqbaiv.sHtML

int x; scanf("%d", &x);
来源：http://www.share.hesvh.cn/Article/details/gckdwaujj.sHtML

[S04] C：字符串复制
来源：http://baike.fehbvm.com/Article/details/gizjdxnmp.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://read.share.hesvh.cn/Article/details/gzsmojepw.sHtML

[S05] C：字符串长度
来源：http://3g.zdbjq.cn/Article/details/gxwizgvov.sHtML

strlen(s)
来源：http://3g.zdbjq.cn/Article/details/gycpjsheg.sHtML

[S06] C：字符串比较
来源：http://www.m.share.zdbjq.cn/Article/details/gakmdixlf.sHtML

strcmp(a, b) == 0
来源：http://www.blog.hesvh.cn/Article/details/ggqsvpbuv.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.fehbvm.com/Article/details/gsiqncnzm.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.m.share.hesvh.cn/Article/details/guytfzmtv.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.zdbjq.cn/Article/details/gpilipqdu.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wap.fehbvm.com/Article/details/gfzfeuqup.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.hesvh.cn/Article/details/gmqhvdkfq.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.zdbjq.cn/Article/details/gpfgwzlkx.sHtML

[S10] C：指针与解引用
来源：http://www.m.share.fehbvm.com/Article/details/govgapyut.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.hesvh.cn/Article/details/grelhdzzf.sHtML

[S11] C：逐行读文件
来源：http://www.m.share.zdbjq.cn/Article/details/gpkmhspmd.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.hesvh.cn/Article/details/gjykyimen.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.zdbjq.cn/Article/details/gqkrkfgpi.sHtML

fclose(f);
来源：http://blog.hesvh.cn/Article/details/grsddouwj.sHtML

[S12] C：写文件
来源：http://www.share.hesvh.cn/Article/details/guulnolui.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.fehbvm.com/Article/details/gmnbskbtm.sHtML

[S13] C：宏定义
来源：http://www.m.share.fehbvm.com/Article/details/gwyuvfcqg.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.zdbjq.cn/Article/details/gjbokppqf.sHtML

[S14] C：枚举
来源：http://www.share.fehbvm.com/Article/details/glemjiekz.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fehbvm.com/Article/details/ggvafcdbs.sHtML

[S15] C：类型转换
来源：http://mobile.fehbvm.com/Article/details/gmdabzlgw.sHtML

(double) a / b
来源：http://3g.hesvh.cn/Article/details/gkalqgwpy.sHtML

[S16] C：位操作置位
来源：http://www.blog.zdbjq.cn/Article/details/gvyjzarcq.sHtML

x |= (1 << 3);
来源：http://wap.fehbvm.com/Article/details/gzcsyrsdl.sHtML

[S17] C：安全拼接字符串
来源：http://wap.fehbvm.com/Article/details/gpqoigwza.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.share.hesvh.cn/Article/details/ghqppxsfb.sHtML

[S18] C：命令行参数
来源：http://www.m.share.hesvh.cn/Article/details/gbkrzwdop.sHtML

int main(int argc, char **argv)
来源：http://mobile.fehbvm.com/Article/details/ghxmilxkn.sHtML

[S19] C：快速排序
来源：http://blog.hesvh.cn/Article/details/gsdzhocvk.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.zdbjq.cn/Article/details/gcjchskss.sHtML

[S20] C：二分查找
来源：http://www.m.share.zdbjq.cn/Article/details/gvfspuftd.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fehbvm.com/Article/details/gjhxmrrtf.sHtML

[S21] C：字符类别判断
来源：http://read.share.fehbvm.com/Article/details/gimsscitz.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.hesvh.cn/Article/details/gpnnjyfyq.sHtML

[S22] C：字符串转数字
来源：http://baike.hesvh.cn/Article/details/gbyrrsayu.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.fehbvm.com/Article/details/guldqbudk.sHtML

[S23] C：随机数
来源：http://www.m.share.hesvh.cn/Article/details/ghpcepczv.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.hesvh.cn/Article/details/gwcwsepjz.sHtML

[S24] C：获取本地时间
来源：http://www.share.fehbvm.com/Article/details/gogzlvhwo.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fehbvm.com/Article/details/gjqywmvyq.sHtML

[S25] C：内存拷贝
来源：http://read.share.zdbjq.cn/Article/details/gxjscflcz.sHtML

memcpy(dst, src, n);
来源：http://3g.hesvh.cn/Article/details/gmsrmvzck.sHtML

[S26] C：内存清零
来源：http://read.share.hesvh.cn/Article/details/gnieywror.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.hesvh.cn/Article/details/gaxzrixea.sHtML

[S27] C：定义常量
来源：http://blog.hesvh.cn/Article/details/gdgchirvc.sHtML

const double PI = 3.14159;
来源：http://wap.fehbvm.com/Article/details/gmnjvllve.sHtML

[S28] C：静态变量
来源：http://www.blog.fehbvm.com/Article/details/gckzjbdrr.sHtML

static int counter = 0;
来源：http://mobile.hesvh.cn/Article/details/glaheurfu.sHtML

[S29] C：变参函数
来源：http://wap.zdbjq.cn/Article/details/glmyherne.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.fehbvm.com/Article/details/guuczqorz.sHtML

[S30] C：头文件保护
来源：http://3g.hesvh.cn/Article/details/gukjqqjvt.sHtML

#ifndef X_H
来源：http://www.blog.zdbjq.cn/Article/details/geukcntpr.sHtML

#define X_H
来源：http://baike.hesvh.cn/Article/details/gcfntcoie.sHtML

#endif
来源：http://www.share.fehbvm.com/Article/details/gjtizoehn.sHtML

[S31] C++：Hello World
来源：http://3g.zdbjq.cn/Article/details/glfyhcsat.sHtML

#include <iostream>
来源：http://blog.hesvh.cn/Article/details/ghwzfkukc.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.fehbvm.com/Article/details/gheyhajrs.sHtML

[S32] C++：字符串
来源：http://mobile.zdbjq.cn/Article/details/gblugbazf.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.hesvh.cn/Article/details/gfadkxpkq.sHtML

[S33] C++：vector 增删
来源：http://baike.hesvh.cn/Article/details/grexslbky.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.zdbjq.cn/Article/details/gixrnsnsi.sHtML

[S34] C++：遍历 vector
来源：http://3g.zdbjq.cn/Article/details/gzcqlguqp.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fehbvm.com/Article/details/gtypvrbkl.sHtML

[S35] C++：map
来源：http://www.m.share.fehbvm.com/Article/details/gofbwfkns.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fehbvm.com/Article/details/gpbusnref.sHtML

[S36] C++：unordered_map
来源：http://mobile.fehbvm.com/Article/details/gjwskavdw.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wap.hesvh.cn/Article/details/gsvkxhqlp.sHtML

[S37] C++：set
来源：http://m.share.fehbvm.com/Article/details/gqzyjovgl.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://blog.fehbvm.com/Article/details/gfixjnplp.sHtML

[S38] C++：排序
来源：http://blog.hesvh.cn/Article/details/giturcfaw.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.hesvh.cn/Article/details/gqsfxpixp.sHtML

[S39] C++：自定义比较器排序
来源：http://www.m.share.hesvh.cn/Article/details/gnoggcntf.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fehbvm.com/Article/details/goicuxihp.sHtML

[S40] C++：查找元素
来源：http://read.share.hesvh.cn/Article/details/gqgllxhhf.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://baike.fehbvm.com/Article/details/gqeckcxno.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.zdbjq.cn/Article/details/gmutjmljy.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.hesvh.cn/Article/details/gwzroazgd.sHtML

[S42] C++：继承与虚函数
来源：http://wap.hesvh.cn/Article/details/gfufqebon.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.share.zdbjq.cn/Article/details/gchqbuntt.sHtML

[S43] C++：智能指针
来源：http://www.blog.zdbjq.cn/Article/details/gwvyjcsiy.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.blog.zdbjq.cn/Article/details/gknfjwaem.sHtML

[S44] C++：引用传参
来源：http://baike.zdbjq.cn/Article/details/gxfhkbddw.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fehbvm.com/Article/details/gqnlderqp.sHtML

[S45] C++：lambda
来源：http://m.share.hesvh.cn/Article/details/gbxiwrsxc.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fehbvm.com/Article/details/gswkyewvd.sHtML

[S46] C++：函数模板
来源：http://m.share.zdbjq.cn/Article/details/gdmdkjpej.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.blog.hesvh.cn/Article/details/gtejdcqbr.sHtML

[S47] C++：结构化绑定遍历
来源：http://blog.fehbvm.com/Article/details/gmyzsevpo.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.zdbjq.cn/Article/details/gadmtzziw.sHtML

[S48] C++：逐行读文件
来源：http://m.share.fehbvm.com/Article/details/gyqljeizu.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.m.share.zdbjq.cn/Article/details/gctddavjq.sHtML

while (std::getline(in, line)) { }
来源：http://baike.fehbvm.com/Article/details/grlddmxnv.sHtML

[S49] C++：写文件
来源：http://www.m.share.fehbvm.com/Article/details/gmufytzkb.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.hesvh.cn/Article/details/gfaythejf.sHtML

[S50] C++：格式化数字
来源：http://m.share.zdbjq.cn/Article/details/ghhkclkoo.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://m.share.hesvh.cn/Article/details/gdbslwjac.sHtML

[S51] C++：显式类型转换
来源：http://3g.hesvh.cn/Article/details/gskhpdncj.sHtML

static_cast<double>(a) / b
来源：http://mobile.zdbjq.cn/Article/details/gpfcnfbjw.sHtML

[S52] C++：const 与 noexcept
来源：http://www.share.zdbjq.cn/Article/details/gcapuodzu.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fehbvm.com/Article/details/geltmtduu.sHtML

[S53] C++：移动语义
来源：http://wap.fehbvm.com/Article/details/gdagitqic.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.zdbjq.cn/Article/details/giccqixru.sHtML

[S54] C++：异常处理
来源：http://m.share.fehbvm.com/Article/details/gggwtqteo.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://blog.fehbvm.com/Article/details/gbkaarluc.sHtML

[S55] C++：结构化绑定
来源：http://blog.fehbvm.com/Article/details/gxgbpfqup.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.hesvh.cn/Article/details/gogumzyij.sHtML

[S56] C++：optional
来源：http://m.share.fehbvm.com/Article/details/gbdytobwo.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.hesvh.cn/Article/details/gluhbgtxe.sHtML

[S57] C++：编译期常量
来源：http://read.share.hesvh.cn/Article/details/gpwgjlklo.sHtML

constexpr int N = 10;
来源：http://read.share.fehbvm.com/Article/details/gxptzqjbi.sHtML

[S58] C++：命名空间
来源：http://blog.fehbvm.com/Article/details/gtsttroxz.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.zdbjq.cn/Article/details/gtsynaxvy.sHtML

[S59] C++：静态断言
来源：http://www.blog.zdbjq.cn/Article/details/gxztxtoxz.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.hesvh.cn/Article/details/gcwvcdhrk.sHtML

[S60] C++：遍历并删除元素
来源：http://www.share.hesvh.cn/Article/details/gltipavag.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.share.fehbvm.com/Article/details/goqdudvjy.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/glotmteia.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.zdbjq.cn/Article/details/gqstfaeuh.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/ggyubgdxe.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fehbvm.com/Article/details/gxuacwpew.sHtML

println("Hello")
来源：http://mobile.zdbjq.cn/Article/details/ggmzircal.sHtML

[T02] Kotlin：变量
来源：http://wap.hesvh.cn/Article/details/glzczdsbm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.hesvh.cn/Article/details/gutxzgeho.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fehbvm.com/Article/details/geqrovocv.sHtML

"值: $b"
来源：http://www.m.share.fehbvm.com/Article/details/gresqgggc.sHtML

[T04] Kotlin：空安全
来源：http://3g.hesvh.cn/Article/details/gadrrijzm.sHtML

val n: String? = null;  n?.length
来源：http://read.share.fehbvm.com/Article/details/gacnmzrts.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.hesvh.cn/Article/details/gnauihsim.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.fehbvm.com/Article/details/gpeaaatvc.sHtML

[T06] Kotlin：集合映射
来源：http://www.share.zdbjq.cn/Article/details/gdynjimiv.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.hesvh.cn/Article/details/gjkhltpqa.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.hesvh.cn/Article/details/gypuijlji.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.zdbjq.cn/Article/details/gcdkiofdy.sHtML

[T08] Kotlin：数据类
来源：http://www.share.zdbjq.cn/Article/details/gognefuiu.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fehbvm.com/Article/details/geeptowbf.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fehbvm.com/Article/details/gnbzwgtqc.sHtML

fun String.exclaim() = this + "!"
来源：http://m.share.hesvh.cn/Article/details/gtotavkon.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.zdbjq.cn/Article/details/gcdedharm.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.zdbjq.cn/Article/details/gzczuaauh.sHtML

[T11] Kotlin：协程
来源：http://blog.hesvh.cn/Article/details/gjdkqpqyq.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://baike.zdbjq.cn/Article/details/gfrxaezul.sHtML

[T12] Kotlin：解构声明
来源：http://read.share.zdbjq.cn/Article/details/gxgdbngbe.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.zdbjq.cn/Article/details/gfpirvkwo.sHtML

[T13] Kotlin：只读 Map
来源：http://baike.hesvh.cn/Article/details/gdnldccyc.sHtML

val m = mapOf("a" to 1)
来源：http://3g.zdbjq.cn/Article/details/gfoizcfcp.sHtML

[T14] Kotlin：循环
来源：http://read.share.zdbjq.cn/Article/details/gdprwzdsr.sHtML

for (i in 1..10) println(i)
来源：http://www.share.hesvh.cn/Article/details/gosaeprxu.sHtML

[T15] Kotlin：接口
来源：http://www.blog.zdbjq.cn/Article/details/gwmbjhmxe.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fehbvm.com/Article/details/gdyxliltf.sHtML

[T16] Swift：Hello World
来源：http://mobile.zdbjq.cn/Article/details/gbdpmcosx.sHtML

print("Hello")
来源：http://www.m.share.zdbjq.cn/Article/details/gozarloks.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.zdbjq.cn/Article/details/gxxibxcud.sHtML

var a = 1;  let b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gywkymass.sHtML

[T18] Swift：字符串插值
来源：http://www.share.zdbjq.cn/Article/details/gznpawdrk.sHtML

"值: \(b)"
来源：http://mobile.hesvh.cn/Article/details/gomabykho.sHtML

[T19] Swift：可选绑定
来源：http://m.share.zdbjq.cn/Article/details/glykecymj.sHtML

if let n = opt { print(n) }
来源：http://wap.fehbvm.com/Article/details/gxrelkwux.sHtML

[T20] Swift：数组操作
来源：http://wap.hesvh.cn/Article/details/gwyvheiyu.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://wap.hesvh.cn/Article/details/gfomrvsuz.sHtML

[T21] Swift：遍历
来源：http://3g.hesvh.cn/Article/details/gmyezgltl.sHtML

for x in a { print(x) }
来源：http://baike.zdbjq.cn/Article/details/gsbpwrnlk.sHtML

[T22] Swift：字典
来源：http://baike.fehbvm.com/Article/details/gxilqpgzs.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.zdbjq.cn/Article/details/gqrqznqdv.sHtML

[T23] Swift：函数
来源：http://read.share.hesvh.cn/Article/details/gowuakhgx.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.zdbjq.cn/Article/details/gvuygcpqj.sHtML

[T24] Swift：闭包
来源：http://read.share.fehbvm.com/Article/details/gparxtntz.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gcwfqayet.sHtML

[T25] Swift：结构体
来源：http://blog.hesvh.cn/Article/details/gqtzrjamn.sHtML

struct P { var x: Int }
来源：http://m.share.fehbvm.com/Article/details/gpdgnvtmf.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.zdbjq.cn/Article/details/gtmklnxod.sHtML

class A: Base { override func f() {} }
来源：http://read.share.zdbjq.cn/Article/details/gpnxpedxo.sHtML

[T27] Swift：错误处理
来源：http://www.m.share.fehbvm.com/Article/details/guwyvhzoi.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.zdbjq.cn/Article/details/gbfiucrrr.sHtML

[T28] Swift：枚举
来源：http://www.share.zdbjq.cn/Article/details/gwnywxemg.sHtML

enum Color { case red, green }
来源：http://www.m.share.hesvh.cn/Article/details/gzveqaosk.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.zdbjq.cn/Article/details/gtobbmdvr.sHtML

guard let x = opt else { return }
来源：http://wap.zdbjq.cn/Article/details/ghtdjnqcg.sHtML

[T30] Swift：协议
来源：http://read.share.fehbvm.com/Article/details/ggoqrqsit.sHtML

protocol Shape { func area() -> Double }
来源：http://mobile.zdbjq.cn/Article/details/gkirvekhy.sHtML

[T31] Lua：Hello World
来源：http://3g.fehbvm.com/Article/details/gkdzytqud.sHtML

print("Hello")
来源：http://www.blog.fehbvm.com/Article/details/ggtgjmsik.sHtML

[T32] Lua：局部变量
来源：http://baike.zdbjq.cn/Article/details/ghhbvpxnz.sHtML

local a = 1
来源：http://wap.zdbjq.cn/Article/details/gmxbvxlcl.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fehbvm.com/Article/details/ghsohbdaw.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://m.share.fehbvm.com/Article/details/gupfltdgv.sHtML

[T34] Lua：遍历表
来源：http://read.share.fehbvm.com/Article/details/gfkiokcjg.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://m.share.fehbvm.com/Article/details/gdxbseulw.sHtML

[T35] Lua：字典表
来源：http://www.blog.fehbvm.com/Article/details/gjntjiixr.sHtML

local d = { a = 1 };  d.b = 2
来源：http://baike.zdbjq.cn/Article/details/gguvjsfhw.sHtML

[T36] Lua：函数
来源：http://m.share.fehbvm.com/Article/details/gjmytvtyz.sHtML

function add(a, b) return a + b end
来源：http://3g.zdbjq.cn/Article/details/gxbduupqs.sHtML

[T37] Lua：字符串拼接
来源：http://blog.hesvh.cn/Article/details/gcrggvqjh.sHtML

"a" .. "b"
来源：http://www.share.hesvh.cn/Article/details/gfhapbnen.sHtML

[T38] Lua：条件
来源：http://m.share.zdbjq.cn/Article/details/grybxhzgs.sHtML

if x > 0 then print("正") end
来源：http://www.blog.fehbvm.com/Article/details/gpedakdkz.sHtML

[T39] Lua：模式匹配
来源：http://www.m.share.zdbjq.cn/Article/details/guxubhibn.sHtML

string.find(s, "%d+")
来源：http://read.share.zdbjq.cn/Article/details/gjqhzfuus.sHtML

[T40] Lua：元表
来源：http://mobile.zdbjq.cn/Article/details/gebdmtnve.sHtML

setmetatable({}, { __index = base })
来源：http://baike.fehbvm.com/Article/details/gvcpnijpe.sHtML

[T41] Perl：Hello World
来源：http://baike.hesvh.cn/Article/details/gkbxhorcx.sHtML

print "Hello\n";
来源：http://blog.fehbvm.com/Article/details/geakixijr.sHtML

[T42] Perl：变量类型
来源：http://mobile.fehbvm.com/Article/details/geebxbcob.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.hesvh.cn/Article/details/gjpgvrfuk.sHtML

[T43] Perl：字符串插值
来源：http://blog.zdbjq.cn/Article/details/gswumpssf.sHtML

"值: $a"
来源：http://baike.zdbjq.cn/Article/details/grmatchon.sHtML

[T44] Perl：条件
来源：http://www.blog.fehbvm.com/Article/details/goqulvsks.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.fehbvm.com/Article/details/gmtogsnsw.sHtML

[T45] Perl：数组遍历
来源：http://read.share.zdbjq.cn/Article/details/gkqbzgkzb.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.hesvh.cn/Article/details/gcgihnzyw.sHtML

[T46] Perl：哈希操作
来源：http://m.share.zdbjq.cn/Article/details/gspcagjrm.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://baike.hesvh.cn/Article/details/gxpfetxww.sHtML

[T47] Perl：正则捕获
来源：http://blog.fehbvm.com/Article/details/gyqymxvpx.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.fehbvm.com/Article/details/gnskafhil.sHtML

[T48] Perl：正则替换
来源：http://baike.zdbjq.cn/Article/details/gqidevohv.sHtML

$s =~ s/old/new/g;
来源：http://blog.hesvh.cn/Article/details/gvxguxtdk.sHtML

[T49] Perl：函数
来源：http://www.share.fehbvm.com/Article/details/ghduumjzz.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mobile.hesvh.cn/Article/details/gqmebdckt.sHtML

[T50] Perl：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gwxkfagfh.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.fehbvm.com/Article/details/gezkgcmvw.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.zdbjq.cn/Article/details/gsheoewlj.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gqifcpnag.sHtML

println("Hello")
来源：http://baike.fehbvm.com/Article/details/guqlrcdtx.sHtML

[T52] Scala：变量
来源：http://blog.fehbvm.com/Article/details/gdtgkhdld.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.fehbvm.com/Article/details/gdnafycpj.sHtML

[T53] Scala：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gcrigqyzu.sHtML

s"值: $b"
来源：http://wap.zdbjq.cn/Article/details/gdmivsfcq.sHtML

[T54] Scala：集合映射
来源：http://blog.fehbvm.com/Article/details/gibabvzpq.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.fehbvm.com/Article/details/gsetslubs.sHtML

[T55] Scala：集合过滤
来源：http://wap.hesvh.cn/Article/details/gromxxrbv.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.hesvh.cn/Article/details/gypsuflqa.sHtML

[T56] Scala：样例类
来源：http://www.share.zdbjq.cn/Article/details/gjofgwgil.sHtML


<!-- 参考信息 -->