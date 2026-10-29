代发 wailian999

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://3g.fehbvm.com/Article/details/gilenryqv.sHtML

[R56] 远程拷贝
来源：http://wap.fehbvm.com/Article/details/gsuwvnuch.sHtML

scp file user@host:/path/
来源：http://baike.zdbjq.cn/Article/details/giadwxcvc.sHtML

[R57] 远程执行命令
来源：http://blog.hesvh.cn/Article/details/gxtjvuekm.sHtML

ssh user@host 'uptime'
来源：http://www.m.share.zdbjq.cn/Article/details/goahwogpp.sHtML

[R58] 下载文件
来源：http://www.share.hesvh.cn/Article/details/gbcdgqftx.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://3g.hesvh.cn/Article/details/ggbtyxzhf.sHtML

[R59] 发 POST JSON
来源：http://wap.hesvh.cn/Article/details/gjuclmnml.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://m.share.zdbjq.cn/Article/details/gvlbinmtq.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.m.share.zdbjq.cn/Article/details/gjhmruevr.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.m.share.zdbjq.cn/Article/details/gauhrujuq.sHtML

[R61] 磁盘占用
来源：http://www.blog.zdbjq.cn/Article/details/gyqddvxvd.sHtML

df -h;  du -sh *
来源：http://www.share.hesvh.cn/Article/details/gozigwrhu.sHtML

[R62] 找最占空间的文件
来源：http://wap.fehbvm.com/Article/details/gxaahdejw.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.hesvh.cn/Article/details/gloveudrq.sHtML

[R63] 内存与进程
来源：http://www.m.share.hesvh.cn/Article/details/gvuewtfga.sHtML

free -h;  ps aux | grep nginx
来源：http://blog.fehbvm.com/Article/details/ghfnckkpr.sHtML

[R64] 结束进程
来源：http://m.share.fehbvm.com/Article/details/gnbkdbjoc.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.zdbjq.cn/Article/details/gvuuyjlhm.sHtML

[R65] 查看端口占用
来源：http://mobile.hesvh.cn/Article/details/gdjbiyvba.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.share.zdbjq.cn/Article/details/gcncqyuze.sHtML

[R66] 定时任务
来源：http://wap.fehbvm.com/Article/details/ghevxqyqi.sHtML

crontab -e;  crontab -l
来源：http://blog.hesvh.cn/Article/details/ggbiqtykw.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.zdbjq.cn/Article/details/gsltasdnx.sHtML

openssl rand -hex 16
来源：http://wap.fehbvm.com/Article/details/gdhhjlolz.sHtML

[R68] 计算文件校验值
来源：http://3g.hesvh.cn/Article/details/gjctwwako.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://3g.fehbvm.com/Article/details/gbakzqlvs.sHtML

[R69] 生成随机密码
来源：http://m.share.hesvh.cn/Article/details/ggilxzhoy.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.zdbjq.cn/Article/details/ghxrvncbo.sHtML

[R70] 时间戳与互转
来源：http://blog.zdbjq.cn/Article/details/gogsvomvb.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fehbvm.com/Article/details/gtrpgpnsn.sHtML

[R71] 日期格式化
来源：http://www.share.fehbvm.com/Article/details/gcrbdidqm.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fehbvm.com/Article/details/gnqhhnncv.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fehbvm.com/Article/details/gnwamwcot.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.zdbjq.cn/Article/details/gjcfeupmt.sHtML

[R73] 分割大日志
来源：http://wap.fehbvm.com/Article/details/gzqqkvvvf.sHtML

split -l 1000 big.log part_
来源：http://www.share.fehbvm.com/Article/details/gadcasesk.sHtML

[R74] 批量重命名
来源：http://baike.zdbjq.cn/Article/details/gokyhqidu.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.hesvh.cn/Article/details/gnhbwgziu.sHtML

[R75] 导出环境变量
来源：http://www.m.share.fehbvm.com/Article/details/ghlnkhdnx.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.fehbvm.com/Article/details/gajaifrne.sHtML

[R76] 使用临时文件
来源：http://mobile.fehbvm.com/Article/details/gbjpvcrca.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.zdbjq.cn/Article/details/gnimnyopj.sHtML

[R77] 读取用户输入
来源：http://3g.fehbvm.com/Article/details/gpbmfxkxt.sHtML

read -rp "请输入: " ans
来源：http://blog.hesvh.cn/Article/details/grfwsokgw.sHtML

[R78] 交互式菜单
来源：http://blog.hesvh.cn/Article/details/gtpzotrwu.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.share.hesvh.cn/Article/details/geaowvbsd.sHtML

[R79] 解析命令行选项
来源：http://3g.zdbjq.cn/Article/details/gccuggxly.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://m.share.hesvh.cn/Article/details/gtfxuzira.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.zdbjq.cn/Article/details/gosfsqcni.sHtML

time ./run.sh
来源：http://baike.fehbvm.com/Article/details/gsvuignkk.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gvgyktbmu.sHtML

S. C / C++ 专题
来源：http://blog.fehbvm.com/Article/details/gpposwxbs.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/goprutsqt.sHtML

[S01] C：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gbfymgdae.sHtML

#include <stdio.h>
来源：http://www.blog.zdbjq.cn/Article/details/gdhdwkopz.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.zdbjq.cn/Article/details/gwrtrqpdr.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.zdbjq.cn/Article/details/gqwprrfzs.sHtML

int a = 10; printf("%d\n", a);
来源：http://m.share.fehbvm.com/Article/details/gjdfkinbh.sHtML

[S03] C：读入整数
来源：http://www.m.share.zdbjq.cn/Article/details/gzurkqirs.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.zdbjq.cn/Article/details/ghgeuotej.sHtML

[S04] C：字符串复制
来源：http://read.share.hesvh.cn/Article/details/gnlelbxvv.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.zdbjq.cn/Article/details/gmqjgsbis.sHtML

[S05] C：字符串长度
来源：http://read.share.fehbvm.com/Article/details/gxqbyrxkq.sHtML

strlen(s)
来源：http://www.share.zdbjq.cn/Article/details/gyjfffgbl.sHtML

[S06] C：字符串比较
来源：http://blog.zdbjq.cn/Article/details/giximwpmj.sHtML

strcmp(a, b) == 0
来源：http://mobile.fehbvm.com/Article/details/ghccslskw.sHtML

[S07] C：数组遍历求和
来源：http://wap.hesvh.cn/Article/details/gzmymcves.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://read.share.fehbvm.com/Article/details/gbtltkjqm.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.fehbvm.com/Article/details/gqbbnsiao.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://3g.fehbvm.com/Article/details/giqthaplb.sHtML

[S09] C：结构体定义与初始化
来源：http://read.share.fehbvm.com/Article/details/gnshcpwbs.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://read.share.zdbjq.cn/Article/details/gawfpvqqu.sHtML

[S10] C：指针与解引用
来源：http://blog.fehbvm.com/Article/details/gsbjtgzgd.sHtML

int *p = &a;  *p = 5;
来源：http://blog.zdbjq.cn/Article/details/gacqchytr.sHtML

[S11] C：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/govronjnp.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.zdbjq.cn/Article/details/ghatbuqbp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.hesvh.cn/Article/details/gesmmguny.sHtML

fclose(f);
来源：http://baike.zdbjq.cn/Article/details/gmlfqcjwc.sHtML

[S12] C：写文件
来源：http://read.share.hesvh.cn/Article/details/gefvsqyjv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://mobile.zdbjq.cn/Article/details/ganfneqlb.sHtML

[S13] C：宏定义
来源：http://3g.hesvh.cn/Article/details/glxqyulek.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.hesvh.cn/Article/details/gxkzngymc.sHtML

[S14] C：枚举
来源：http://read.share.fehbvm.com/Article/details/goeuhhzpj.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.zdbjq.cn/Article/details/gbjyotmsb.sHtML

[S15] C：类型转换
来源：http://www.share.fehbvm.com/Article/details/gmftbfwph.sHtML

(double) a / b
来源：http://www.share.zdbjq.cn/Article/details/gysmqvjrj.sHtML

[S16] C：位操作置位
来源：http://wap.fehbvm.com/Article/details/ggpffoucp.sHtML

x |= (1 << 3);
来源：http://www.blog.hesvh.cn/Article/details/goiutrmbh.sHtML

[S17] C：安全拼接字符串
来源：http://m.share.fehbvm.com/Article/details/gfsnchfok.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://baike.hesvh.cn/Article/details/ggkzubodr.sHtML

[S18] C：命令行参数
来源：http://www.m.share.zdbjq.cn/Article/details/guqmwurno.sHtML

int main(int argc, char **argv)
来源：http://baike.zdbjq.cn/Article/details/gnfvkmlbh.sHtML

[S19] C：快速排序
来源：http://mobile.zdbjq.cn/Article/details/gyqdmbidl.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.blog.fehbvm.com/Article/details/gegxslzap.sHtML

[S20] C：二分查找
来源：http://baike.hesvh.cn/Article/details/gtitcipfj.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/gfgqpqktt.sHtML

[S21] C：字符类别判断
来源：http://www.share.hesvh.cn/Article/details/gomzxhtht.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.blog.zdbjq.cn/Article/details/guxhwhjys.sHtML

[S22] C：字符串转数字
来源：http://wap.fehbvm.com/Article/details/gkgrmyzmq.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://read.share.zdbjq.cn/Article/details/gbghsqhkm.sHtML

[S23] C：随机数
来源：http://blog.fehbvm.com/Article/details/gohzcvbnt.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.zdbjq.cn/Article/details/gfmabyvev.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fehbvm.com/Article/details/glycrdlxe.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.hesvh.cn/Article/details/gsyzguhqn.sHtML

[S25] C：内存拷贝
来源：http://www.blog.hesvh.cn/Article/details/ginkakeme.sHtML

memcpy(dst, src, n);
来源：http://mobile.hesvh.cn/Article/details/gdoecggfn.sHtML

[S26] C：内存清零
来源：http://mobile.fehbvm.com/Article/details/geujaxkhy.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fehbvm.com/Article/details/gaqoolgsa.sHtML

[S27] C：定义常量
来源：http://read.share.hesvh.cn/Article/details/gjoseosgz.sHtML

const double PI = 3.14159;
来源：http://www.blog.fehbvm.com/Article/details/gdhnrisdn.sHtML

[S28] C：静态变量
来源：http://www.blog.hesvh.cn/Article/details/gugtccafx.sHtML

static int counter = 0;
来源：http://3g.hesvh.cn/Article/details/gijbiqarn.sHtML

[S29] C：变参函数
来源：http://mobile.fehbvm.com/Article/details/gkzboxaal.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.hesvh.cn/Article/details/glxilflis.sHtML

[S30] C：头文件保护
来源：http://3g.hesvh.cn/Article/details/gxpnokaoy.sHtML

#ifndef X_H
来源：http://www.blog.zdbjq.cn/Article/details/gfoygfyeg.sHtML

#define X_H
来源：http://www.blog.zdbjq.cn/Article/details/gnsdbmukq.sHtML

#endif
来源：http://m.share.zdbjq.cn/Article/details/gwhqiosna.sHtML

[S31] C++：Hello World
来源：http://mobile.fehbvm.com/Article/details/gvsrbxvlv.sHtML

#include <iostream>
来源：http://www.share.fehbvm.com/Article/details/gcipyqaai.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://mobile.fehbvm.com/Article/details/gbxnntejk.sHtML

[S32] C++：字符串
来源：http://www.blog.fehbvm.com/Article/details/gvtjrxyzy.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.fehbvm.com/Article/details/ggvmboisp.sHtML

[S33] C++：vector 增删
来源：http://www.m.share.hesvh.cn/Article/details/gbownsszd.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.blog.fehbvm.com/Article/details/gmsjowtzx.sHtML

[S34] C++：遍历 vector
来源：http://m.share.zdbjq.cn/Article/details/ggpittgfj.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.zdbjq.cn/Article/details/gaihbdyjr.sHtML

[S35] C++：map
来源：http://www.share.fehbvm.com/Article/details/gxzzwqvsi.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.share.fehbvm.com/Article/details/gcxsekhkb.sHtML

[S36] C++：unordered_map
来源：http://mobile.hesvh.cn/Article/details/gpnwizwvi.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.hesvh.cn/Article/details/gflgdwsnt.sHtML

[S37] C++：set
来源：http://www.share.fehbvm.com/Article/details/gsgorgbeg.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.fehbvm.com/Article/details/gqecgdfze.sHtML

[S38] C++：排序
来源：http://www.blog.fehbvm.com/Article/details/ggvguudbz.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.zdbjq.cn/Article/details/ghcabaxhy.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.fehbvm.com/Article/details/gtiwlcqat.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.fehbvm.com/Article/details/gracqwqwr.sHtML

[S40] C++：查找元素
来源：http://m.share.hesvh.cn/Article/details/grsomrhrf.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://3g.fehbvm.com/Article/details/gufipcdcq.sHtML

[S41] C++：类与构造函数
来源：http://m.share.zdbjq.cn/Article/details/guisfayfe.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.fehbvm.com/Article/details/gjovlorec.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.fehbvm.com/Article/details/gitcdcljn.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.zdbjq.cn/Article/details/gwytoimdp.sHtML

[S43] C++：智能指针
来源：http://wap.fehbvm.com/Article/details/gqgbdwfgs.sHtML

auto p = std::make_unique<int>(5);
来源：http://mobile.zdbjq.cn/Article/details/gufcdqsfh.sHtML

[S44] C++：引用传参
来源：http://3g.zdbjq.cn/Article/details/gnfboswgy.sHtML

void inc(int &x) { ++x; }
来源：http://m.share.zdbjq.cn/Article/details/gadyrfmsv.sHtML

[S45] C++：lambda
来源：http://www.m.share.hesvh.cn/Article/details/gwewtdvxt.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fehbvm.com/Article/details/gggsycgej.sHtML

[S46] C++：函数模板
来源：http://mobile.hesvh.cn/Article/details/gfumelurx.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://read.share.zdbjq.cn/Article/details/guvycdyxi.sHtML

[S47] C++：结构化绑定遍历
来源：http://baike.hesvh.cn/Article/details/gitjjgdrj.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.zdbjq.cn/Article/details/gbtkxwblk.sHtML

[S48] C++：逐行读文件
来源：http://m.share.zdbjq.cn/Article/details/ggkqfuimn.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.hesvh.cn/Article/details/gkbqltrav.sHtML

while (std::getline(in, line)) { }
来源：http://read.share.hesvh.cn/Article/details/ghxiyvkym.sHtML

[S49] C++：写文件
来源：http://m.share.fehbvm.com/Article/details/gsvketlnv.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.share.zdbjq.cn/Article/details/gmlmehqqx.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fehbvm.com/Article/details/glkqhxmqv.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gwgnnmfqf.sHtML

[S51] C++：显式类型转换
来源：http://mobile.zdbjq.cn/Article/details/gimrgyjwa.sHtML

static_cast<double>(a) / b
来源：http://3g.zdbjq.cn/Article/details/gnnbeyfso.sHtML

[S52] C++：const 与 noexcept
来源：http://mobile.zdbjq.cn/Article/details/golhkyvui.sHtML

int size() const noexcept { return n_; }
来源：http://baike.fehbvm.com/Article/details/gajzjriyy.sHtML

[S53] C++：移动语义
来源：http://baike.zdbjq.cn/Article/details/gjcoivwce.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.hesvh.cn/Article/details/guflmudav.sHtML

[S54] C++：异常处理
来源：http://wap.hesvh.cn/Article/details/gpsdytadx.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.blog.zdbjq.cn/Article/details/gghkyogrp.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.hesvh.cn/Article/details/ggkjcizqh.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fehbvm.com/Article/details/gzsbcxthi.sHtML

[S56] C++：optional
来源：http://blog.hesvh.cn/Article/details/gjthqzglf.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.hesvh.cn/Article/details/gsytyopbm.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.zdbjq.cn/Article/details/gqnybwhre.sHtML

constexpr int N = 10;
来源：http://baike.hesvh.cn/Article/details/gpfzuonrg.sHtML

[S58] C++：命名空间
来源：http://mobile.zdbjq.cn/Article/details/gifqjegfi.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.zdbjq.cn/Article/details/gkjgvaxvs.sHtML

[S59] C++：静态断言
来源：http://3g.fehbvm.com/Article/details/gynjzzkym.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.zdbjq.cn/Article/details/goyfavenb.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.hesvh.cn/Article/details/gcudjeaie.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.zdbjq.cn/Article/details/gvguriaaj.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gwpvvdmao.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://3g.fehbvm.com/Article/details/gaiuywkex.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/ghbvjqyuy.sHtML

[T01] Kotlin：Hello World
来源：http://blog.zdbjq.cn/Article/details/gtswmbsfi.sHtML

println("Hello")
来源：http://blog.hesvh.cn/Article/details/givbykgnc.sHtML

[T02] Kotlin：变量
来源：http://www.share.hesvh.cn/Article/details/gkwaekbfm.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.fehbvm.com/Article/details/gocehpukv.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.zdbjq.cn/Article/details/gkipidfwz.sHtML

"值: $b"
来源：http://blog.zdbjq.cn/Article/details/gpmixhxsj.sHtML

[T04] Kotlin：空安全
来源：http://www.share.zdbjq.cn/Article/details/gtrflmtfz.sHtML

val n: String? = null;  n?.length
来源：http://www.share.zdbjq.cn/Article/details/gkgntqplj.sHtML

[T05] Kotlin：when 表达式
来源：http://www.blog.zdbjq.cn/Article/details/grdswvldh.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://baike.hesvh.cn/Article/details/gtixyedxu.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.hesvh.cn/Article/details/grzkmyumv.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.fehbvm.com/Article/details/gnbxikkbi.sHtML

[T07] Kotlin：集合过滤
来源：http://www.blog.hesvh.cn/Article/details/glfvexesw.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fehbvm.com/Article/details/givmbyevp.sHtML

[T08] Kotlin：数据类
来源：http://wap.hesvh.cn/Article/details/geojhncwu.sHtML

data class User(val name: String, val age: Int)
来源：http://read.share.hesvh.cn/Article/details/gkfbswhya.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.hesvh.cn/Article/details/gfilesoxy.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.fehbvm.com/Article/details/gbhxwcnsm.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fehbvm.com/Article/details/gxakrnzwa.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.zdbjq.cn/Article/details/gusvcajha.sHtML

[T11] Kotlin：协程
来源：http://blog.hesvh.cn/Article/details/gtlrecaws.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://blog.zdbjq.cn/Article/details/gjlpjsoqk.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fehbvm.com/Article/details/gmqieotiv.sHtML

val (a, b) = Pair(1, 2)
来源：http://wap.fehbvm.com/Article/details/gvexygicw.sHtML

[T13] Kotlin：只读 Map
来源：http://read.share.zdbjq.cn/Article/details/gegfdiyva.sHtML

val m = mapOf("a" to 1)
来源：http://www.blog.hesvh.cn/Article/details/gxoreocpx.sHtML

[T14] Kotlin：循环
来源：http://read.share.fehbvm.com/Article/details/gbjbdhmjc.sHtML

for (i in 1..10) println(i)
来源：http://read.share.fehbvm.com/Article/details/gofzxzqqy.sHtML

[T15] Kotlin：接口
来源：http://blog.zdbjq.cn/Article/details/gluflzfkw.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.hesvh.cn/Article/details/gcenmbhnd.sHtML

[T16] Swift：Hello World
来源：http://www.blog.fehbvm.com/Article/details/gufgcljzp.sHtML

print("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gykanxeki.sHtML

[T17] Swift：变量与常量
来源：http://m.share.zdbjq.cn/Article/details/gzkpjfcwd.sHtML

var a = 1;  let b = 2
来源：http://www.blog.zdbjq.cn/Article/details/gpifbxggk.sHtML

[T18] Swift：字符串插值
来源：http://3g.hesvh.cn/Article/details/giixrtums.sHtML

"值: \(b)"
来源：http://wap.fehbvm.com/Article/details/gvlxqxcyr.sHtML

[T19] Swift：可选绑定
来源：http://3g.fehbvm.com/Article/details/gbdrhmjfd.sHtML

if let n = opt { print(n) }
来源：http://m.share.fehbvm.com/Article/details/gzgktzahy.sHtML

[T20] Swift：数组操作
来源：http://mobile.zdbjq.cn/Article/details/gshcdsqvb.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.zdbjq.cn/Article/details/gyuetrkcr.sHtML

[T21] Swift：遍历
来源：http://mobile.hesvh.cn/Article/details/gmddlpncl.sHtML

for x in a { print(x) }
来源：http://baike.hesvh.cn/Article/details/gsgetwcil.sHtML

[T22] Swift：字典
来源：http://mobile.hesvh.cn/Article/details/gzjolxtel.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://3g.fehbvm.com/Article/details/gqrxolmbl.sHtML

[T23] Swift：函数
来源：http://mobile.zdbjq.cn/Article/details/gdzbjeyaf.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.zdbjq.cn/Article/details/gjulegnid.sHtML

[T24] Swift：闭包
来源：http://www.share.fehbvm.com/Article/details/gdnzkgnce.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.zdbjq.cn/Article/details/gnpbqiofk.sHtML

[T25] Swift：结构体
来源：http://read.share.fehbvm.com/Article/details/grkkruviv.sHtML

struct P { var x: Int }
来源：http://read.share.zdbjq.cn/Article/details/gdafmrbso.sHtML

[T26] Swift：类与重写
来源：http://read.share.zdbjq.cn/Article/details/gwpeaqpza.sHtML

class A: Base { override func f() {} }
来源：http://mobile.fehbvm.com/Article/details/gdfamiilv.sHtML

[T27] Swift：错误处理
来源：http://3g.fehbvm.com/Article/details/gxulwglip.sHtML

do { try f() } catch { print(error) }
来源：http://wap.fehbvm.com/Article/details/gwpvttdyv.sHtML

[T28] Swift：枚举
来源：http://read.share.hesvh.cn/Article/details/geexkobdz.sHtML

enum Color { case red, green }
来源：http://blog.fehbvm.com/Article/details/grnjgdwpx.sHtML

[T29] Swift：guard 提前返回
来源：http://baike.hesvh.cn/Article/details/gppknvdlx.sHtML

guard let x = opt else { return }
来源：http://read.share.zdbjq.cn/Article/details/gknwefbqj.sHtML

[T30] Swift：协议
来源：http://blog.hesvh.cn/Article/details/gnrobfagt.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.zdbjq.cn/Article/details/gfejaoxhj.sHtML

[T31] Lua：Hello World
来源：http://blog.hesvh.cn/Article/details/gkiawjefz.sHtML

print("Hello")
来源：http://www.share.zdbjq.cn/Article/details/ghrzanybw.sHtML

[T32] Lua：局部变量
来源：http://blog.fehbvm.com/Article/details/gdopyexaq.sHtML

local a = 1
来源：http://m.share.fehbvm.com/Article/details/gfeqnqowo.sHtML

[T33] Lua：表（数组）
来源：http://3g.zdbjq.cn/Article/details/gwmtqhegv.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://baike.zdbjq.cn/Article/details/gorpcgaaw.sHtML

[T34] Lua：遍历表
来源：http://www.share.hesvh.cn/Article/details/ghrkxlqtg.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.hesvh.cn/Article/details/getocaqgn.sHtML

[T35] Lua：字典表
来源：http://mobile.hesvh.cn/Article/details/gvyiqwhab.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.hesvh.cn/Article/details/grfhgpcsz.sHtML

[T36] Lua：函数
来源：http://www.blog.zdbjq.cn/Article/details/gdkbaorpd.sHtML

function add(a, b) return a + b end
来源：http://read.share.fehbvm.com/Article/details/gceiefyaz.sHtML

[T37] Lua：字符串拼接
来源：http://wap.fehbvm.com/Article/details/gewvjfnmr.sHtML

"a" .. "b"
来源：http://m.share.fehbvm.com/Article/details/gdswjnilc.sHtML

[T38] Lua：条件
来源：http://m.share.hesvh.cn/Article/details/googtckgz.sHtML

if x > 0 then print("正") end
来源：http://read.share.hesvh.cn/Article/details/ghrwykqba.sHtML

[T39] Lua：模式匹配
来源：http://m.share.zdbjq.cn/Article/details/gantylepq.sHtML

string.find(s, "%d+")
来源：http://blog.fehbvm.com/Article/details/ggoavqujm.sHtML

[T40] Lua：元表
来源：http://www.m.share.hesvh.cn/Article/details/grunfkvgz.sHtML

setmetatable({}, { __index = base })
来源：http://blog.hesvh.cn/Article/details/gpekhyuvp.sHtML

[T41] Perl：Hello World
来源：http://blog.zdbjq.cn/Article/details/gttgapyvy.sHtML

print "Hello\n";
来源：http://www.m.share.zdbjq.cn/Article/details/gkhmjqtkm.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.zdbjq.cn/Article/details/gbdmqojev.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.zdbjq.cn/Article/details/ghdeqweil.sHtML

[T43] Perl：字符串插值
来源：http://wap.fehbvm.com/Article/details/gefkrohzs.sHtML

"值: $a"
来源：http://read.share.zdbjq.cn/Article/details/ghkkbkwls.sHtML

[T44] Perl：条件
来源：http://wap.hesvh.cn/Article/details/gfghzhknq.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.fehbvm.com/Article/details/gwbvzjocn.sHtML

[T45] Perl：数组遍历
来源：http://blog.zdbjq.cn/Article/details/gqhogwmtn.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.zdbjq.cn/Article/details/glkuybqhg.sHtML

[T46] Perl：哈希操作
来源：http://read.share.zdbjq.cn/Article/details/gjjrprcbb.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.blog.hesvh.cn/Article/details/gmczmlcek.sHtML

[T47] Perl：正则捕获
来源：http://3g.fehbvm.com/Article/details/gxkcnijfv.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.share.hesvh.cn/Article/details/gpmzdijzy.sHtML

[T48] Perl：正则替换
来源：http://mobile.hesvh.cn/Article/details/gmvkaetax.sHtML

$s =~ s/old/new/g;
来源：http://mobile.fehbvm.com/Article/details/gmqzpdbyn.sHtML

[T49] Perl：函数
来源：http://3g.zdbjq.cn/Article/details/guzdfynkt.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/grmgoxhjp.sHtML

[T50] Perl：逐行读文件
来源：http://www.m.share.fehbvm.com/Article/details/gzkqotaxf.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://read.share.fehbvm.com/Article/details/gjhqbkcxy.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.fehbvm.com/Article/details/gjbxuvcfr.sHtML

[T51] Scala：Hello World
来源：http://www.m.share.hesvh.cn/Article/details/gqhydgoyp.sHtML

println("Hello")
来源：http://m.share.zdbjq.cn/Article/details/grdyzhfpk.sHtML

[T52] Scala：变量
来源：http://read.share.hesvh.cn/Article/details/gqbaisbzw.sHtML

val a = 1;  var b = 2
来源：http://wap.hesvh.cn/Article/details/ghobhmyhy.sHtML

[T53] Scala：字符串插值
来源：http://mobile.fehbvm.com/Article/details/giqdwcfuf.sHtML

s"值: $b"
来源：http://www.blog.zdbjq.cn/Article/details/gyyqggego.sHtML

[T54] Scala：集合映射
来源：http://m.share.fehbvm.com/Article/details/gaacmzvyi.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://wap.hesvh.cn/Article/details/gwrmxxqtn.sHtML

[T55] Scala：集合过滤
来源：http://wap.hesvh.cn/Article/details/giobyipvt.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://read.share.hesvh.cn/Article/details/gzyylbpko.sHtML

[T56] Scala：样例类
来源：http://mobile.hesvh.cn/Article/details/guceklhkm.sHtML

case class User(name: String, age: Int)
来源：http://baike.hesvh.cn/Article/details/gmzfmqter.sHtML

[T57] Scala：模式匹配
来源：http://www.share.hesvh.cn/Article/details/gjysgvlog.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.zdbjq.cn/Article/details/gbgmwibie.sHtML

[T58] Scala：函数定义
来源：http://3g.zdbjq.cn/Article/details/gcnriuoeu.sHtML


<!-- 参考信息 -->