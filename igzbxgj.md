代发 wailian999

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://read.share.fanxiaobao.xyz/Article/details/gvrjhvhfz.sHtML

[R56] 远程拷贝
来源：http://read.share.fanxiaobao.xyz/Article/details/ggzilqkar.sHtML

scp file user@host:/path/
来源：http://wap.fanxiaobao.xyz/Article/details/gofwlmoke.sHtML

[R57] 远程执行命令
来源：http://m.share.fanxiaobao.xyz/Article/details/genvjugds.sHtML

ssh user@host 'uptime'
来源：http://m.share.fanxiaobao.xyz/Article/details/gqfjilufe.sHtML

[R58] 下载文件
来源：http://baike.fanxiaobao.xyz/Article/details/gbbujznlz.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfrfkauzm.sHtML

[R59] 发 POST JSON
来源：http://read.share.fanxiaobao.xyz/Article/details/gxbjnetnj.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpdcosipv.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gqtfwwqfu.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggqmiarpf.sHtML

[R61] 磁盘占用
来源：http://www.blog.fanxiaobao.xyz/Article/details/gywbzcvbl.sHtML

df -h;  du -sh *
来源：http://read.share.fanxiaobao.xyz/Article/details/gmvusxmox.sHtML

[R62] 找最占空间的文件
来源：http://3g.fanxiaobao.xyz/Article/details/gluyjmrqr.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fanxiaobao.xyz/Article/details/gjluoysci.sHtML

[R63] 内存与进程
来源：http://mobile.fanxiaobao.xyz/Article/details/gzzguqxix.sHtML

free -h;  ps aux | grep nginx
来源：http://wap.fanxiaobao.xyz/Article/details/gkfhagmxz.sHtML

[R64] 结束进程
来源：http://m.share.fanxiaobao.xyz/Article/details/gaydcvagy.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqtmtxsmz.sHtML

[R65] 查看端口占用
来源：http://wap.fanxiaobao.xyz/Article/details/gevsfrwrz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fanxiaobao.xyz/Article/details/gesccvtjc.sHtML

[R66] 定时任务
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcxxwexoh.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/gugmwcngl.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fanxiaobao.xyz/Article/details/ggpbvaheb.sHtML

openssl rand -hex 16
来源：http://m.share.fanxiaobao.xyz/Article/details/gxxoaplgv.sHtML

[R68] 计算文件校验值
来源：http://baike.fanxiaobao.xyz/Article/details/gzarponsb.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.blog.fanxiaobao.xyz/Article/details/grvshcoei.sHtML

[R69] 生成随机密码
来源：http://m.share.fanxiaobao.xyz/Article/details/gkibjfgoz.sHtML

head -c 16 /dev/urandom | base64
来源：http://3g.fanxiaobao.xyz/Article/details/glqoyszpf.sHtML

[R70] 时间戳与互转
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsposhqnx.sHtML

date +%s;  date -d @1700000000
来源：http://3g.fanxiaobao.xyz/Article/details/gfoahgujr.sHtML

[R71] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gunvbstvj.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpdxuvzzs.sHtML

[R72] 等待端口就绪
来源：http://wap.fanxiaobao.xyz/Article/details/gdkqyczzd.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.fanxiaobao.xyz/Article/details/gnnftjpkz.sHtML

[R73] 分割大日志
来源：http://blog.fanxiaobao.xyz/Article/details/gyjknkhzq.sHtML

split -l 1000 big.log part_
来源：http://baike.fanxiaobao.xyz/Article/details/gimrcyicz.sHtML

[R74] 批量重命名
来源：http://m.share.fanxiaobao.xyz/Article/details/gmgcdbczw.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://m.share.fanxiaobao.xyz/Article/details/gclgylpqc.sHtML

[R75] 导出环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gdbicfogc.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fanxiaobao.xyz/Article/details/ghwptuwcn.sHtML

[R76] 使用临时文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/grwiusqdk.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.blog.fanxiaobao.xyz/Article/details/gnasshleb.sHtML

[R77] 读取用户输入
来源：http://3g.fanxiaobao.xyz/Article/details/gjohmxssg.sHtML

read -rp "请输入: " ans
来源：http://blog.fanxiaobao.xyz/Article/details/gdgpsfoqv.sHtML

[R78] 交互式菜单
来源：http://www.share.fanxiaobao.xyz/Article/details/gsqwcyebo.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fanxiaobao.xyz/Article/details/gyacjezpm.sHtML

[R79] 解析命令行选项
来源：http://baike.fanxiaobao.xyz/Article/details/giulufozn.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdatbwxzc.sHtML

[R80] 查看脚本执行耗时
来源：http://blog.fanxiaobao.xyz/Article/details/ghvzfrcww.sHtML

time ./run.sh
来源：http://www.blog.fanxiaobao.xyz/Article/details/gsbdhggqp.sHtML

================================================================================
来源：http://3g.fanxiaobao.xyz/Article/details/gjbdrbcmu.sHtML

S. C / C++ 专题
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjjadyfog.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gwezjpzsb.sHtML

[S01] C：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/ggwezvkkz.sHtML

#include <stdio.h>
来源：http://m.share.fanxiaobao.xyz/Article/details/gxzfjruil.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.fanxiaobao.xyz/Article/details/gfxurntwa.sHtML

[S02] C：变量与格式化输出
来源：http://m.share.fanxiaobao.xyz/Article/details/gbrihxwak.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fanxiaobao.xyz/Article/details/guhcfeugq.sHtML

[S03] C：读入整数
来源：http://m.share.fanxiaobao.xyz/Article/details/gmsvtgaea.sHtML

int x; scanf("%d", &x);
来源：http://read.share.fanxiaobao.xyz/Article/details/gitbgmyrk.sHtML

[S04] C：字符串复制
来源：http://blog.fanxiaobao.xyz/Article/details/gadcusgbg.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fanxiaobao.xyz/Article/details/geitaqhwb.sHtML

[S05] C：字符串长度
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbejcmdhq.sHtML

strlen(s)
来源：http://baike.fanxiaobao.xyz/Article/details/ggkljxdew.sHtML

[S06] C：字符串比较
来源：http://read.share.fanxiaobao.xyz/Article/details/gzfwtwcbk.sHtML

strcmp(a, b) == 0
来源：http://3g.fanxiaobao.xyz/Article/details/gdexmjsst.sHtML

[S07] C：数组遍历求和
来源：http://baike.fanxiaobao.xyz/Article/details/gffvlkijf.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fanxiaobao.xyz/Article/details/gbccqagya.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcdbjzqxo.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fanxiaobao.xyz/Article/details/gkfkqruel.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.fanxiaobao.xyz/Article/details/gmyqzrkqa.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.fanxiaobao.xyz/Article/details/gtqfdzhlg.sHtML

[S10] C：指针与解引用
来源：http://www.share.fanxiaobao.xyz/Article/details/gjyhddfge.sHtML

int *p = &a;  *p = 5;
来源：http://wap.fanxiaobao.xyz/Article/details/gatqajkzj.sHtML

[S11] C：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gdtfwdlec.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://read.share.fanxiaobao.xyz/Article/details/groouqtxp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcbuzueio.sHtML

fclose(f);
来源：http://www.share.fanxiaobao.xyz/Article/details/gqtolfbiw.sHtML

[S12] C：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gxbaiyvgx.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/grxfsazns.sHtML

[S13] C：宏定义
来源：http://blog.fanxiaobao.xyz/Article/details/gvfsgmgkm.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.fanxiaobao.xyz/Article/details/gubvyngot.sHtML

[S14] C：枚举
来源：http://wap.fanxiaobao.xyz/Article/details/gbxsfbazq.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://read.share.fanxiaobao.xyz/Article/details/gcxalzlhb.sHtML

[S15] C：类型转换
来源：http://mobile.fanxiaobao.xyz/Article/details/gfjsnbcgf.sHtML

(double) a / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glbkatdlf.sHtML

[S16] C：位操作置位
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gespbeyxw.sHtML

x |= (1 << 3);
来源：http://3g.fanxiaobao.xyz/Article/details/gofbijran.sHtML

[S17] C：安全拼接字符串
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpyahzaww.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wap.fanxiaobao.xyz/Article/details/gtkgzriqm.sHtML

[S18] C：命令行参数
来源：http://blog.fanxiaobao.xyz/Article/details/ghnxmergu.sHtML

int main(int argc, char **argv)
来源：http://wap.fanxiaobao.xyz/Article/details/ghtbuccno.sHtML

[S19] C：快速排序
来源：http://baike.fanxiaobao.xyz/Article/details/gpubiaaji.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fanxiaobao.xyz/Article/details/gvjswjxew.sHtML

[S20] C：二分查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gbtepkhdz.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.fanxiaobao.xyz/Article/details/gbumicitb.sHtML

[S21] C：字符类别判断
来源：http://3g.fanxiaobao.xyz/Article/details/gkntycyla.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fanxiaobao.xyz/Article/details/gcpplsssu.sHtML

[S22] C：字符串转数字
来源：http://www.m.share.fanxiaobao.xyz/Article/details/giafvycjz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://wap.fanxiaobao.xyz/Article/details/ghlphpvvb.sHtML

[S23] C：随机数
来源：http://mobile.fanxiaobao.xyz/Article/details/glewfkzrm.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fanxiaobao.xyz/Article/details/gqsfmfhni.sHtML

[S24] C：获取本地时间
来源：http://baike.fanxiaobao.xyz/Article/details/gsayxnyrt.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mobile.fanxiaobao.xyz/Article/details/gxcyiwuca.sHtML

[S25] C：内存拷贝
来源：http://blog.fanxiaobao.xyz/Article/details/gkgtspjlh.sHtML

memcpy(dst, src, n);
来源：http://blog.fanxiaobao.xyz/Article/details/gmajbkzbk.sHtML

[S26] C：内存清零
来源：http://mobile.fanxiaobao.xyz/Article/details/gttmslxtt.sHtML

memset(a, 0, sizeof a);
来源：http://3g.fanxiaobao.xyz/Article/details/gnfnmleyk.sHtML

[S27] C：定义常量
来源：http://mobile.fanxiaobao.xyz/Article/details/gjssnexqo.sHtML

const double PI = 3.14159;
来源：http://3g.fanxiaobao.xyz/Article/details/gyqcccorj.sHtML

[S28] C：静态变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjyurzlii.sHtML

static int counter = 0;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gozdshbgt.sHtML

[S29] C：变参函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gcsjcmeoo.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://3g.fanxiaobao.xyz/Article/details/glwgmhwqf.sHtML

[S30] C：头文件保护
来源：http://www.share.fanxiaobao.xyz/Article/details/gxgijkpvg.sHtML

#ifndef X_H
来源：http://blog.fanxiaobao.xyz/Article/details/gsocurtzb.sHtML

#define X_H
来源：http://read.share.fanxiaobao.xyz/Article/details/gcsisnbns.sHtML

#endif
来源：http://baike.fanxiaobao.xyz/Article/details/gstmprlmx.sHtML

[S31] C++：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gglbmfukv.sHtML

#include <iostream>
来源：http://wap.fanxiaobao.xyz/Article/details/gxsyyixxk.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbrgdtffi.sHtML

[S32] C++：字符串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtxmtgyus.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.fanxiaobao.xyz/Article/details/gkjrnsbdk.sHtML

[S33] C++：vector 增删
来源：http://mobile.fanxiaobao.xyz/Article/details/gzrdwkbyl.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fanxiaobao.xyz/Article/details/gmyirkyba.sHtML

[S34] C++：遍历 vector
来源：http://baike.fanxiaobao.xyz/Article/details/gkihjyupp.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwwlvogqs.sHtML

[S35] C++：map
来源：http://mobile.fanxiaobao.xyz/Article/details/gexgdmwgd.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/ghpqplqts.sHtML

[S36] C++：unordered_map
来源：http://blog.fanxiaobao.xyz/Article/details/gaywmtsam.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gdbogzwym.sHtML

[S37] C++：set
来源：http://3g.fanxiaobao.xyz/Article/details/gcrrwyzhg.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.fanxiaobao.xyz/Article/details/gfolichgt.sHtML

[S38] C++：排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gckwwdktg.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaciuubfs.sHtML

[S39] C++：自定义比较器排序
来源：http://www.share.fanxiaobao.xyz/Article/details/ghijpnacj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gecjouibu.sHtML

[S40] C++：查找元素
来源：http://m.share.fanxiaobao.xyz/Article/details/gvsfilglx.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gyzcijzlv.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gamlouhjl.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://read.share.fanxiaobao.xyz/Article/details/gvkjqdawa.sHtML

[S42] C++：继承与虚函数
来源：http://baike.fanxiaobao.xyz/Article/details/gyigvhdtj.sHtML

class B : public Base { public: void f() override {} };
来源：http://read.share.fanxiaobao.xyz/Article/details/gvsxgahbj.sHtML

[S43] C++：智能指针
来源：http://baike.fanxiaobao.xyz/Article/details/ghfdcjooi.sHtML

auto p = std::make_unique<int>(5);
来源：http://m.share.fanxiaobao.xyz/Article/details/gkatsghmt.sHtML

[S44] C++：引用传参
来源：http://baike.fanxiaobao.xyz/Article/details/gpynudgmv.sHtML

void inc(int &x) { ++x; }
来源：http://baike.fanxiaobao.xyz/Article/details/gmkgenenu.sHtML

[S45] C++：lambda
来源：http://mobile.fanxiaobao.xyz/Article/details/gcujqxluv.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fanxiaobao.xyz/Article/details/grqqoprhu.sHtML

[S46] C++：函数模板
来源：http://baike.fanxiaobao.xyz/Article/details/gyubyvnfk.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gjihrsbwo.sHtML

[S47] C++：结构化绑定遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gfmxmfedk.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.fanxiaobao.xyz/Article/details/getoieire.sHtML

[S48] C++：逐行读文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxpgzcjfy.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fanxiaobao.xyz/Article/details/gedztiueo.sHtML

while (std::getline(in, line)) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gmynnvjji.sHtML

[S49] C++：写文件
来源：http://blog.fanxiaobao.xyz/Article/details/gdhodconc.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fanxiaobao.xyz/Article/details/givgvxste.sHtML

[S50] C++：格式化数字
来源：http://mobile.fanxiaobao.xyz/Article/details/gyukzdwhl.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gostzhbrl.sHtML

[S51] C++：显式类型转换
来源：http://m.share.fanxiaobao.xyz/Article/details/gzpufsnoe.sHtML

static_cast<double>(a) / b
来源：http://read.share.fanxiaobao.xyz/Article/details/gkuzzeyzr.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.fanxiaobao.xyz/Article/details/gknijslsf.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gizlripqv.sHtML

[S53] C++：移动语义
来源：http://3g.fanxiaobao.xyz/Article/details/gbpceybsl.sHtML

std::vector<int> w = std::move(v);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqzcgrwbo.sHtML

[S54] C++：异常处理
来源：http://wap.fanxiaobao.xyz/Article/details/glrlupnfq.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzpyfhejx.sHtML

[S55] C++：结构化绑定
来源：http://www.blog.fanxiaobao.xyz/Article/details/glrwybinl.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghdrwpxlf.sHtML

[S56] C++：optional
来源：http://baike.fanxiaobao.xyz/Article/details/gracsotuq.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdknnlakx.sHtML

[S57] C++：编译期常量
来源：http://blog.fanxiaobao.xyz/Article/details/goahuhpmr.sHtML

constexpr int N = 10;
来源：http://3g.fanxiaobao.xyz/Article/details/gyeeeajjf.sHtML

[S58] C++：命名空间
来源：http://3g.fanxiaobao.xyz/Article/details/gzqvebvga.sHtML

namespace ns { int f() { return 1; } }
来源：http://mobile.fanxiaobao.xyz/Article/details/grrtjxaad.sHtML

[S59] C++：静态断言
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxhykkvii.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://3g.fanxiaobao.xyz/Article/details/gtfbnqfkg.sHtML

[S60] C++：遍历并删除元素
来源：http://wap.fanxiaobao.xyz/Article/details/gfviboboj.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbmrshhtj.sHtML

================================================================================
来源：http://m.share.fanxiaobao.xyz/Article/details/gdhipniib.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fanxiaobao.xyz/Article/details/giusryvca.sHtML

================================================================================
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjcecuscj.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gnsfubfgt.sHtML

println("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gpbzkyopz.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gkxhmdtxl.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.share.fanxiaobao.xyz/Article/details/gmivhrzhi.sHtML

[T03] Kotlin：字符串模板
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gziiggabh.sHtML

"值: $b"
来源：http://3g.fanxiaobao.xyz/Article/details/gzqcawdgk.sHtML

[T04] Kotlin：空安全
来源：http://3g.fanxiaobao.xyz/Article/details/gbhbqblxz.sHtML

val n: String? = null;  n?.length
来源：http://3g.fanxiaobao.xyz/Article/details/gvlfjimik.sHtML

[T05] Kotlin：when 表达式
来源：http://wap.fanxiaobao.xyz/Article/details/guxnuljbr.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.fanxiaobao.xyz/Article/details/gfuronrpd.sHtML

[T06] Kotlin：集合映射
来源：http://www.m.share.fanxiaobao.xyz/Article/details/glurvkzzc.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gxahovcae.sHtML

[T07] Kotlin：集合过滤
来源：http://mobile.fanxiaobao.xyz/Article/details/gsggbztrp.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://m.share.fanxiaobao.xyz/Article/details/ggiwivywk.sHtML

[T08] Kotlin：数据类
来源：http://3g.fanxiaobao.xyz/Article/details/gitzfxray.sHtML

data class User(val name: String, val age: Int)
来源：http://m.share.fanxiaobao.xyz/Article/details/gtmcubjep.sHtML

[T09] Kotlin：扩展函数
来源：http://3g.fanxiaobao.xyz/Article/details/gixqmyqty.sHtML

fun String.exclaim() = this + "!"
来源：http://baike.fanxiaobao.xyz/Article/details/gqvdpycql.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gvqruxhag.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.fanxiaobao.xyz/Article/details/gvnjbyqts.sHtML

[T11] Kotlin：协程
来源：http://baike.fanxiaobao.xyz/Article/details/gsxckdwbp.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gdchfzigo.sHtML

[T12] Kotlin：解构声明
来源：http://mobile.fanxiaobao.xyz/Article/details/guczvaypu.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfhfmruyd.sHtML

[T13] Kotlin：只读 Map
来源：http://m.share.fanxiaobao.xyz/Article/details/gmltxdcpq.sHtML

val m = mapOf("a" to 1)
来源：http://blog.fanxiaobao.xyz/Article/details/gtdggdaoo.sHtML

[T14] Kotlin：循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gtvoysnza.sHtML

for (i in 1..10) println(i)
来源：http://wap.fanxiaobao.xyz/Article/details/gvbftlprb.sHtML

[T15] Kotlin：接口
来源：http://baike.fanxiaobao.xyz/Article/details/gxoxxnewm.sHtML

interface Shape { fun area(): Double }
来源：http://mobile.fanxiaobao.xyz/Article/details/gdqpisgdz.sHtML

[T16] Swift：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcmswfzja.sHtML

print("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjzbtgbhk.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gucvkifmb.sHtML

var a = 1;  let b = 2
来源：http://mobile.fanxiaobao.xyz/Article/details/gwerqyzmi.sHtML

[T18] Swift：字符串插值
来源：http://m.share.fanxiaobao.xyz/Article/details/gmqgqfywt.sHtML

"值: \(b)"
来源：http://baike.fanxiaobao.xyz/Article/details/gmjzldhwb.sHtML

[T19] Swift：可选绑定
来源：http://blog.fanxiaobao.xyz/Article/details/gqsxaxytp.sHtML

if let n = opt { print(n) }
来源：http://baike.fanxiaobao.xyz/Article/details/gxuxhbyie.sHtML

[T20] Swift：数组操作
来源：http://blog.fanxiaobao.xyz/Article/details/gvzbfhdud.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.fanxiaobao.xyz/Article/details/gryhfcukw.sHtML

[T21] Swift：遍历
来源：http://m.share.fanxiaobao.xyz/Article/details/gszchmdnr.sHtML

for x in a { print(x) }
来源：http://m.share.fanxiaobao.xyz/Article/details/gktqcywrf.sHtML

[T22] Swift：字典
来源：http://www.m.share.fanxiaobao.xyz/Article/details/grzqzsfqv.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvvqjmuwz.sHtML

[T23] Swift：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gwkbipytu.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.fanxiaobao.xyz/Article/details/giyflaanw.sHtML

[T24] Swift：闭包
来源：http://wap.fanxiaobao.xyz/Article/details/gprcotvlr.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://wap.fanxiaobao.xyz/Article/details/gdsoqujtq.sHtML

[T25] Swift：结构体
来源：http://blog.fanxiaobao.xyz/Article/details/gzpjeupdb.sHtML

struct P { var x: Int }
来源：http://wap.fanxiaobao.xyz/Article/details/gvpbegqyt.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsfdpankr.sHtML

class A: Base { override func f() {} }
来源：http://3g.fanxiaobao.xyz/Article/details/gfgfoaksj.sHtML

[T27] Swift：错误处理
来源：http://blog.fanxiaobao.xyz/Article/details/gaesanehr.sHtML

do { try f() } catch { print(error) }
来源：http://blog.fanxiaobao.xyz/Article/details/gjehxvlvp.sHtML

[T28] Swift：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/grdjrxlci.sHtML

enum Color { case red, green }
来源：http://3g.fanxiaobao.xyz/Article/details/gzqrhcumw.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdaxpajmf.sHtML

guard let x = opt else { return }
来源：http://blog.fanxiaobao.xyz/Article/details/gjqfzzhzf.sHtML

[T30] Swift：协议
来源：http://wap.fanxiaobao.xyz/Article/details/gefabnomv.sHtML

protocol Shape { func area() -> Double }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gldwsxrhw.sHtML

[T31] Lua：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gqlovviaf.sHtML

print("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzbpksewn.sHtML

[T32] Lua：局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gqpxuvynd.sHtML

local a = 1
来源：http://read.share.fanxiaobao.xyz/Article/details/gaxryywkw.sHtML

[T33] Lua：表（数组）
来源：http://read.share.fanxiaobao.xyz/Article/details/gocjagfbs.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.fanxiaobao.xyz/Article/details/gyefykppf.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gducptqdp.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://mobile.fanxiaobao.xyz/Article/details/ghdxhwwxq.sHtML

[T35] Lua：字典表
来源：http://blog.fanxiaobao.xyz/Article/details/gpdokjgcw.sHtML

local d = { a = 1 };  d.b = 2
来源：http://wap.fanxiaobao.xyz/Article/details/gohzkwkxi.sHtML

[T36] Lua：函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gwnbefoma.sHtML

function add(a, b) return a + b end
来源：http://www.share.fanxiaobao.xyz/Article/details/gutuzwech.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.fanxiaobao.xyz/Article/details/gstvtrmjo.sHtML

"a" .. "b"
来源：http://blog.fanxiaobao.xyz/Article/details/gpanmebfa.sHtML

[T38] Lua：条件
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtcgkecpp.sHtML

if x > 0 then print("正") end
来源：http://wap.fanxiaobao.xyz/Article/details/getynrxlb.sHtML

[T39] Lua：模式匹配
来源：http://m.share.fanxiaobao.xyz/Article/details/gptdjxfvm.sHtML

string.find(s, "%d+")
来源：http://m.share.fanxiaobao.xyz/Article/details/gaggkgftg.sHtML

[T40] Lua：元表
来源：http://baike.fanxiaobao.xyz/Article/details/gogsuvvlc.sHtML

setmetatable({}, { __index = base })
来源：http://wap.fanxiaobao.xyz/Article/details/gomnujvsg.sHtML

[T41] Perl：Hello World
来源：http://blog.fanxiaobao.xyz/Article/details/gtkpqzebl.sHtML

print "Hello\n";
来源：http://mobile.fanxiaobao.xyz/Article/details/gvzbkupdn.sHtML

[T42] Perl：变量类型
来源：http://mobile.fanxiaobao.xyz/Article/details/gyfmtzgcf.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wap.fanxiaobao.xyz/Article/details/getowvtna.sHtML

[T43] Perl：字符串插值
来源：http://wap.fanxiaobao.xyz/Article/details/gvstjeimw.sHtML

"值: $a"
来源：http://baike.fanxiaobao.xyz/Article/details/gnmpzjxnv.sHtML

[T44] Perl：条件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyhpynjvt.sHtML

if ($a > 0) { print "正"; }
来源：http://wap.fanxiaobao.xyz/Article/details/gbpygqdmv.sHtML

[T45] Perl：数组遍历
来源：http://wap.fanxiaobao.xyz/Article/details/guauzvffq.sHtML

for my $x (@arr) { print $x; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gynydwqxf.sHtML

[T46] Perl：哈希操作
来源：http://mobile.fanxiaobao.xyz/Article/details/gjezvgjfd.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://3g.fanxiaobao.xyz/Article/details/gtkkpmsbd.sHtML

[T47] Perl：正则捕获
来源：http://www.share.fanxiaobao.xyz/Article/details/gdeznkngo.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.fanxiaobao.xyz/Article/details/goubiwzxw.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbyxnofmj.sHtML

$s =~ s/old/new/g;
来源：http://blog.fanxiaobao.xyz/Article/details/gywjpmbly.sHtML

[T49] Perl：函数
来源：http://3g.fanxiaobao.xyz/Article/details/gxqnoajce.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://baike.fanxiaobao.xyz/Article/details/gpyatflcq.sHtML

[T50] Perl：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/goeixanej.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://wap.fanxiaobao.xyz/Article/details/guuxoicot.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gajryhoqo.sHtML

[T51] Scala：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/gehhvlutp.sHtML

println("Hello")
来源：http://blog.fanxiaobao.xyz/Article/details/gdnmfhqrd.sHtML

[T52] Scala：变量
来源：http://blog.fanxiaobao.xyz/Article/details/gmzvbskdc.sHtML

val a = 1;  var b = 2
来源：http://blog.fanxiaobao.xyz/Article/details/gkhszupwl.sHtML

[T53] Scala：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/gyelntayd.sHtML

s"值: $b"
来源：http://m.share.fanxiaobao.xyz/Article/details/gppctymxc.sHtML

[T54] Scala：集合映射
来源：http://mobile.fanxiaobao.xyz/Article/details/gxtxucoif.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gbmnojibl.sHtML

[T55] Scala：集合过滤
来源：http://read.share.fanxiaobao.xyz/Article/details/gjdqclflr.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.fanxiaobao.xyz/Article/details/gwyuvxfgp.sHtML

[T56] Scala：样例类
来源：http://m.share.fanxiaobao.xyz/Article/details/gjnoeyjzl.sHtML

case class User(name: String, age: Int)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gqngguqoq.sHtML

[T57] Scala：模式匹配
来源：http://3g.fanxiaobao.xyz/Article/details/gjcyicvqr.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://blog.fanxiaobao.xyz/Article/details/geidnyxrf.sHtML

[T58] Scala：函数定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gaaqceduw.sHtML


<!-- 参考信息 -->