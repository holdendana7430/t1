代发 wailian999

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wap.hesvh.cn/Article/details/gazvqjliv.sHtML

[R56] 远程拷贝
来源：http://wap.fehbvm.com/Article/details/gxgsvmequ.sHtML

scp file user@host:/path/
来源：http://3g.hesvh.cn/Article/details/gyjxrqxzc.sHtML

[R57] 远程执行命令
来源：http://www.blog.zdbjq.cn/Article/details/grwidrfxo.sHtML

ssh user@host 'uptime'
来源：http://wap.zdbjq.cn/Article/details/gjahtwcft.sHtML

[R58] 下载文件
来源：http://mobile.hesvh.cn/Article/details/gcdolxqqv.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.blog.zdbjq.cn/Article/details/gyyqfycqj.sHtML

[R59] 发 POST JSON
来源：http://mobile.fehbvm.com/Article/details/gfqrpxtuk.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://blog.hesvh.cn/Article/details/gutzeqoyp.sHtML

[R60] 只看 HTTP 状态码
来源：http://3g.zdbjq.cn/Article/details/gjsouebyy.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mobile.zdbjq.cn/Article/details/goajiomtx.sHtML

[R61] 磁盘占用
来源：http://mobile.fehbvm.com/Article/details/gkmsmqagw.sHtML

df -h;  du -sh *
来源：http://3g.hesvh.cn/Article/details/gumgfjpjq.sHtML

[R62] 找最占空间的文件
来源：http://www.share.fehbvm.com/Article/details/gmonnmwvv.sHtML

du -ah . | sort -rh | head -10
来源：http://www.m.share.zdbjq.cn/Article/details/gchmwtvio.sHtML

[R63] 内存与进程
来源：http://read.share.hesvh.cn/Article/details/gfvbibyfc.sHtML

free -h;  ps aux | grep nginx
来源：http://read.share.fehbvm.com/Article/details/gztvhhoiz.sHtML

[R64] 结束进程
来源：http://www.share.fehbvm.com/Article/details/genuabody.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.hesvh.cn/Article/details/gotsezqhz.sHtML

[R65] 查看端口占用
来源：http://3g.hesvh.cn/Article/details/goxbmibxz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.hesvh.cn/Article/details/gpkyracpr.sHtML

[R66] 定时任务
来源：http://baike.zdbjq.cn/Article/details/gqomtadfx.sHtML

crontab -e;  crontab -l
来源：http://www.m.share.fehbvm.com/Article/details/gnjgigmjn.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fehbvm.com/Article/details/gjdozwkfw.sHtML

openssl rand -hex 16
来源：http://www.blog.zdbjq.cn/Article/details/gwoyvxskz.sHtML

[R68] 计算文件校验值
来源：http://www.m.share.zdbjq.cn/Article/details/gyiujlnxp.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://blog.hesvh.cn/Article/details/gfxewxhyh.sHtML

[R69] 生成随机密码
来源：http://3g.fehbvm.com/Article/details/gjhjdtgfp.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.fehbvm.com/Article/details/garmydrlg.sHtML

[R70] 时间戳与互转
来源：http://read.share.hesvh.cn/Article/details/gmmcuqjxo.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fehbvm.com/Article/details/glicrzayi.sHtML

[R71] 日期格式化
来源：http://baike.zdbjq.cn/Article/details/ghisadmts.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.hesvh.cn/Article/details/gdjngsdzy.sHtML

[R72] 等待端口就绪
来源：http://www.m.share.hesvh.cn/Article/details/gdeqrjotq.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://www.m.share.hesvh.cn/Article/details/guhrmymrh.sHtML

[R73] 分割大日志
来源：http://read.share.zdbjq.cn/Article/details/gfdowqkaa.sHtML

split -l 1000 big.log part_
来源：http://wap.hesvh.cn/Article/details/gbrasqnhb.sHtML

[R74] 批量重命名
来源：http://www.share.hesvh.cn/Article/details/gayijylun.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wap.hesvh.cn/Article/details/gbpigmxsz.sHtML

[R75] 导出环境变量
来源：http://wap.zdbjq.cn/Article/details/gmpnugdst.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://m.share.fehbvm.com/Article/details/gzylkbqey.sHtML

[R76] 使用临时文件
来源：http://www.m.share.hesvh.cn/Article/details/gkdsozyjz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.hesvh.cn/Article/details/gsposdknv.sHtML

[R77] 读取用户输入
来源：http://www.share.fehbvm.com/Article/details/gwlotobqh.sHtML

read -rp "请输入: " ans
来源：http://mobile.fehbvm.com/Article/details/gjrildbcw.sHtML

[R78] 交互式菜单
来源：http://blog.zdbjq.cn/Article/details/ghmgjcxzm.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.zdbjq.cn/Article/details/giqctyqxd.sHtML

[R79] 解析命令行选项
来源：http://blog.zdbjq.cn/Article/details/gjivxlvut.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.blog.zdbjq.cn/Article/details/gxevabboq.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.hesvh.cn/Article/details/gcndirqjt.sHtML

time ./run.sh
来源：http://m.share.fehbvm.com/Article/details/grvsddrxk.sHtML

================================================================================
来源：http://baike.zdbjq.cn/Article/details/gscqbthxf.sHtML

S. C / C++ 专题
来源：http://baike.zdbjq.cn/Article/details/ghdzdhjzt.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/gzmvxwekg.sHtML

[S01] C：Hello World
来源：http://wap.zdbjq.cn/Article/details/gysqeifqt.sHtML

#include <stdio.h>
来源：http://3g.fehbvm.com/Article/details/gkjjnsohk.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.share.zdbjq.cn/Article/details/gejhzzsno.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.zdbjq.cn/Article/details/glicyzzio.sHtML

int a = 10; printf("%d\n", a);
来源：http://blog.zdbjq.cn/Article/details/gmehnateu.sHtML

[S03] C：读入整数
来源：http://wap.fehbvm.com/Article/details/grhaexnjf.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.fehbvm.com/Article/details/gcobmfzdx.sHtML

[S04] C：字符串复制
来源：http://m.share.zdbjq.cn/Article/details/ggdfvtuxv.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://m.share.hesvh.cn/Article/details/geigiifqn.sHtML

[S05] C：字符串长度
来源：http://m.share.hesvh.cn/Article/details/gcadbbide.sHtML

strlen(s)
来源：http://blog.hesvh.cn/Article/details/gvqdviicr.sHtML

[S06] C：字符串比较
来源：http://blog.fehbvm.com/Article/details/geuvrtnhu.sHtML

strcmp(a, b) == 0
来源：http://m.share.hesvh.cn/Article/details/gllaawlnh.sHtML

[S07] C：数组遍历求和
来源：http://baike.zdbjq.cn/Article/details/glqbpxqlx.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://3g.fehbvm.com/Article/details/gxilikbsg.sHtML

[S08] C：动态内存分配与释放
来源：http://3g.hesvh.cn/Article/details/ghvhvyovc.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.hesvh.cn/Article/details/gwjztqcnq.sHtML

[S09] C：结构体定义与初始化
来源：http://www.m.share.hesvh.cn/Article/details/gmovnfksw.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://3g.fehbvm.com/Article/details/gdgeglltz.sHtML

[S10] C：指针与解引用
来源：http://www.share.fehbvm.com/Article/details/gbwwytqzx.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fehbvm.com/Article/details/gjwrisqpn.sHtML

[S11] C：逐行读文件
来源：http://baike.hesvh.cn/Article/details/gmzkakbrf.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.hesvh.cn/Article/details/grdkxxnmp.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.blog.hesvh.cn/Article/details/grlwcfvkc.sHtML

fclose(f);
来源：http://www.share.hesvh.cn/Article/details/gwiuzlowh.sHtML

[S12] C：写文件
来源：http://m.share.hesvh.cn/Article/details/gylgztdtd.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.share.zdbjq.cn/Article/details/grxbnknax.sHtML

[S13] C：宏定义
来源：http://wap.fehbvm.com/Article/details/gdgurztdx.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wap.hesvh.cn/Article/details/gjecxjwla.sHtML

[S14] C：枚举
来源：http://www.blog.zdbjq.cn/Article/details/gaafeoryt.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://3g.fehbvm.com/Article/details/gouutggaa.sHtML

[S15] C：类型转换
来源：http://read.share.zdbjq.cn/Article/details/gsigxvvhs.sHtML

(double) a / b
来源：http://blog.hesvh.cn/Article/details/gjfgsktph.sHtML

[S16] C：位操作置位
来源：http://read.share.hesvh.cn/Article/details/gcqswaieg.sHtML

x |= (1 << 3);
来源：http://www.blog.zdbjq.cn/Article/details/gwmyncyjj.sHtML

[S17] C：安全拼接字符串
来源：http://blog.hesvh.cn/Article/details/guaowjrsx.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://m.share.hesvh.cn/Article/details/gzyvfldbj.sHtML

[S18] C：命令行参数
来源：http://wap.hesvh.cn/Article/details/ghygmsxrc.sHtML

int main(int argc, char **argv)
来源：http://mobile.hesvh.cn/Article/details/gclxostjf.sHtML

[S19] C：快速排序
来源：http://3g.hesvh.cn/Article/details/gbbdcnnpa.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://baike.hesvh.cn/Article/details/gojuwkxxn.sHtML

[S20] C：二分查找
来源：http://mobile.fehbvm.com/Article/details/giuqqwsqq.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://blog.fehbvm.com/Article/details/gjtimvzln.sHtML

[S21] C：字符类别判断
来源：http://mobile.hesvh.cn/Article/details/gehspmwut.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.hesvh.cn/Article/details/gstaaamcr.sHtML

[S22] C：字符串转数字
来源：http://mobile.hesvh.cn/Article/details/ginzyxefr.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.share.fehbvm.com/Article/details/gehwpmlam.sHtML

[S23] C：随机数
来源：http://www.share.fehbvm.com/Article/details/gnhvmetir.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://www.m.share.hesvh.cn/Article/details/gxtmgpgxb.sHtML

[S24] C：获取本地时间
来源：http://m.share.zdbjq.cn/Article/details/guaivapma.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.blog.zdbjq.cn/Article/details/gpytmmmir.sHtML

[S25] C：内存拷贝
来源：http://blog.fehbvm.com/Article/details/gaiqgddsa.sHtML

memcpy(dst, src, n);
来源：http://m.share.zdbjq.cn/Article/details/gjwiqowiy.sHtML

[S26] C：内存清零
来源：http://baike.fehbvm.com/Article/details/gqkyrofbo.sHtML

memset(a, 0, sizeof a);
来源：http://mobile.zdbjq.cn/Article/details/gbwjzwzii.sHtML

[S27] C：定义常量
来源：http://baike.hesvh.cn/Article/details/gwsyuregc.sHtML

const double PI = 3.14159;
来源：http://mobile.fehbvm.com/Article/details/gdtazxgqz.sHtML

[S28] C：静态变量
来源：http://mobile.hesvh.cn/Article/details/gezduqrsv.sHtML

static int counter = 0;
来源：http://baike.zdbjq.cn/Article/details/ggolgtqdt.sHtML

[S29] C：变参函数
来源：http://www.blog.fehbvm.com/Article/details/ggxergbvc.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.blog.hesvh.cn/Article/details/gqydvyrzt.sHtML

[S30] C：头文件保护
来源：http://read.share.fehbvm.com/Article/details/gzwzwstuv.sHtML

#ifndef X_H
来源：http://mobile.fehbvm.com/Article/details/gvfjgtahh.sHtML

#define X_H
来源：http://m.share.zdbjq.cn/Article/details/gyumqwuru.sHtML

#endif
来源：http://mobile.hesvh.cn/Article/details/gnzcnscpd.sHtML

[S31] C++：Hello World
来源：http://www.share.zdbjq.cn/Article/details/gcnfzgdhz.sHtML

#include <iostream>
来源：http://baike.zdbjq.cn/Article/details/gmqdqcifq.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://3g.fehbvm.com/Article/details/ghfdkckpp.sHtML

[S32] C++：字符串
来源：http://mobile.zdbjq.cn/Article/details/gdfhzlobn.sHtML

std::string s = "hi";  s += "!";
来源：http://baike.fehbvm.com/Article/details/gjqqrbnrr.sHtML

[S33] C++：vector 增删
来源：http://read.share.fehbvm.com/Article/details/ghljkzrmc.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.fehbvm.com/Article/details/gvqzrrbql.sHtML

[S34] C++：遍历 vector
来源：http://m.share.zdbjq.cn/Article/details/gxkgkuebb.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://m.share.zdbjq.cn/Article/details/gulbqkpta.sHtML

[S35] C++：map
来源：http://read.share.hesvh.cn/Article/details/gencgzybb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.fehbvm.com/Article/details/geqevduwe.sHtML

[S36] C++：unordered_map
来源：http://m.share.zdbjq.cn/Article/details/ggxgxeowg.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://read.share.zdbjq.cn/Article/details/gzwvynwtw.sHtML

[S37] C++：set
来源：http://wap.fehbvm.com/Article/details/gjljaaivh.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fehbvm.com/Article/details/gasujbxri.sHtML

[S38] C++：排序
来源：http://baike.zdbjq.cn/Article/details/ghqmixsut.sHtML

std::sort(v.begin(), v.end());
来源：http://3g.fehbvm.com/Article/details/gtzizgrwt.sHtML

[S39] C++：自定义比较器排序
来源：http://m.share.hesvh.cn/Article/details/gcrinkuwn.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://mobile.fehbvm.com/Article/details/gwbjaawmq.sHtML

[S40] C++：查找元素
来源：http://mobile.zdbjq.cn/Article/details/gpvovagti.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.hesvh.cn/Article/details/gpuxjyfdv.sHtML

[S41] C++：类与构造函数
来源：http://mobile.fehbvm.com/Article/details/gmsoyhbtm.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.share.hesvh.cn/Article/details/gfjmyxxpc.sHtML

[S42] C++：继承与虚函数
来源：http://blog.zdbjq.cn/Article/details/gmdcrboug.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.hesvh.cn/Article/details/gmdwvmxpe.sHtML

[S43] C++：智能指针
来源：http://www.blog.zdbjq.cn/Article/details/gmjmrkxjr.sHtML

auto p = std::make_unique<int>(5);
来源：http://read.share.hesvh.cn/Article/details/gshewipmi.sHtML

[S44] C++：引用传参
来源：http://www.blog.hesvh.cn/Article/details/gclaadvtu.sHtML

void inc(int &x) { ++x; }
来源：http://www.blog.hesvh.cn/Article/details/gzoayylmf.sHtML

[S45] C++：lambda
来源：http://www.blog.hesvh.cn/Article/details/gprmtqivs.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fehbvm.com/Article/details/ganpofowy.sHtML

[S46] C++：函数模板
来源：http://mobile.hesvh.cn/Article/details/gksusqsgj.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://blog.fehbvm.com/Article/details/gkwocnqgj.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fehbvm.com/Article/details/govxpcpfa.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://read.share.zdbjq.cn/Article/details/gyauqqdjh.sHtML

[S48] C++：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/gjgurzknz.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.fehbvm.com/Article/details/gkhchvxfa.sHtML

while (std::getline(in, line)) { }
来源：http://blog.fehbvm.com/Article/details/ggnpgtljs.sHtML

[S49] C++：写文件
来源：http://wap.fehbvm.com/Article/details/gsjrzzhvl.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wap.fehbvm.com/Article/details/gspdjflfm.sHtML

[S50] C++：格式化数字
来源：http://www.share.hesvh.cn/Article/details/guuxzkrzv.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://baike.zdbjq.cn/Article/details/grbyqcqbd.sHtML

[S51] C++：显式类型转换
来源：http://3g.fehbvm.com/Article/details/gziuorkjv.sHtML

static_cast<double>(a) / b
来源：http://3g.zdbjq.cn/Article/details/gzfjivwuu.sHtML

[S52] C++：const 与 noexcept
来源：http://www.blog.fehbvm.com/Article/details/gaatxilee.sHtML

int size() const noexcept { return n_; }
来源：http://www.blog.fehbvm.com/Article/details/gcuntclsw.sHtML

[S53] C++：移动语义
来源：http://blog.hesvh.cn/Article/details/giguovjbw.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.hesvh.cn/Article/details/gkonvyohi.sHtML

[S54] C++：异常处理
来源：http://3g.hesvh.cn/Article/details/gtorvlzfv.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.hesvh.cn/Article/details/glepmhmfr.sHtML

[S55] C++：结构化绑定
来源：http://www.share.zdbjq.cn/Article/details/goukqhaty.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://blog.hesvh.cn/Article/details/gmmkdpqip.sHtML

[S56] C++：optional
来源：http://baike.fehbvm.com/Article/details/gbujrxnyf.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mobile.zdbjq.cn/Article/details/glvnnjbbd.sHtML

[S57] C++：编译期常量
来源：http://mobile.zdbjq.cn/Article/details/gpfyxgjtb.sHtML

constexpr int N = 10;
来源：http://www.share.hesvh.cn/Article/details/gfwlocvgd.sHtML

[S58] C++：命名空间
来源：http://read.share.hesvh.cn/Article/details/gisanslab.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.hesvh.cn/Article/details/gkbhfldlr.sHtML

[S59] C++：静态断言
来源：http://www.m.share.fehbvm.com/Article/details/ggjmmdslf.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fehbvm.com/Article/details/gjjwqyjdw.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.zdbjq.cn/Article/details/gnsqmfqya.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.hesvh.cn/Article/details/gqgxswfvx.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gdoeoxqri.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://m.share.hesvh.cn/Article/details/gegmccies.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gckdanqay.sHtML

[T01] Kotlin：Hello World
来源：http://blog.zdbjq.cn/Article/details/glicgpuvi.sHtML

println("Hello")
来源：http://blog.hesvh.cn/Article/details/gxfwqlull.sHtML

[T02] Kotlin：变量
来源：http://mobile.zdbjq.cn/Article/details/gkrhizvpk.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://baike.zdbjq.cn/Article/details/grcbjvybl.sHtML

[T03] Kotlin：字符串模板
来源：http://www.share.hesvh.cn/Article/details/gwusofvft.sHtML

"值: $b"
来源：http://mobile.hesvh.cn/Article/details/guhsnfsrx.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fehbvm.com/Article/details/gblxafenw.sHtML

val n: String? = null;  n?.length
来源：http://www.m.share.hesvh.cn/Article/details/gmovkelgd.sHtML

[T05] Kotlin：when 表达式
来源：http://read.share.hesvh.cn/Article/details/gbwppgeep.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wap.fehbvm.com/Article/details/gdgvrxllr.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.fehbvm.com/Article/details/ghdcdhfuq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://mobile.hesvh.cn/Article/details/ggffrlqvo.sHtML

[T07] Kotlin：集合过滤
来源：http://blog.fehbvm.com/Article/details/gywbjqfho.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://wap.fehbvm.com/Article/details/ghvvywoha.sHtML

[T08] Kotlin：数据类
来源：http://wap.zdbjq.cn/Article/details/grihzhmur.sHtML

data class User(val name: String, val age: Int)
来源：http://blog.hesvh.cn/Article/details/gcaongngp.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.zdbjq.cn/Article/details/gyljlrujr.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.hesvh.cn/Article/details/gyiyhrbzz.sHtML

[T10] Kotlin：默认参数
来源：http://www.m.share.fehbvm.com/Article/details/getjwcekk.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.zdbjq.cn/Article/details/gqimhwjxo.sHtML

[T11] Kotlin：协程
来源：http://m.share.hesvh.cn/Article/details/gcmpeokxw.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://read.share.hesvh.cn/Article/details/gktivkyfi.sHtML

[T12] Kotlin：解构声明
来源：http://3g.zdbjq.cn/Article/details/guxtmocae.sHtML

val (a, b) = Pair(1, 2)
来源：http://read.share.hesvh.cn/Article/details/glymtjarf.sHtML

[T13] Kotlin：只读 Map
来源：http://www.blog.hesvh.cn/Article/details/gnonnjsps.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.hesvh.cn/Article/details/gwichwegc.sHtML

[T14] Kotlin：循环
来源：http://www.share.zdbjq.cn/Article/details/gefumyupa.sHtML

for (i in 1..10) println(i)
来源：http://blog.hesvh.cn/Article/details/givvgdyec.sHtML

[T15] Kotlin：接口
来源：http://read.share.fehbvm.com/Article/details/gdumlcror.sHtML

interface Shape { fun area(): Double }
来源：http://read.share.fehbvm.com/Article/details/gnpwqnepj.sHtML

[T16] Swift：Hello World
来源：http://m.share.hesvh.cn/Article/details/glhketqkn.sHtML

print("Hello")
来源：http://baike.fehbvm.com/Article/details/grwlkjvlu.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.zdbjq.cn/Article/details/guwupfzyb.sHtML

var a = 1;  let b = 2
来源：http://blog.fehbvm.com/Article/details/gwdvrtpkz.sHtML

[T18] Swift：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gsrmnywul.sHtML

"值: \(b)"
来源：http://blog.fehbvm.com/Article/details/gqbedbctn.sHtML

[T19] Swift：可选绑定
来源：http://baike.zdbjq.cn/Article/details/gzatdoikw.sHtML

if let n = opt { print(n) }
来源：http://blog.hesvh.cn/Article/details/gveispkfm.sHtML

[T20] Swift：数组操作
来源：http://wap.hesvh.cn/Article/details/gtorfxqxz.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://blog.zdbjq.cn/Article/details/gshomovnr.sHtML

[T21] Swift：遍历
来源：http://read.share.hesvh.cn/Article/details/gxzqyrzsy.sHtML

for x in a { print(x) }
来源：http://read.share.hesvh.cn/Article/details/gsqnpomly.sHtML

[T22] Swift：字典
来源：http://baike.fehbvm.com/Article/details/gzsxvdsfd.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://m.share.zdbjq.cn/Article/details/gadczyyxn.sHtML

[T23] Swift：函数
来源：http://m.share.hesvh.cn/Article/details/gxzkjaxag.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://blog.fehbvm.com/Article/details/gmgvsuwpl.sHtML

[T24] Swift：闭包
来源：http://baike.fehbvm.com/Article/details/gccpbsooq.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.hesvh.cn/Article/details/gxrdnzzvn.sHtML

[T25] Swift：结构体
来源：http://baike.zdbjq.cn/Article/details/glcdxszqx.sHtML

struct P { var x: Int }
来源：http://read.share.fehbvm.com/Article/details/grjqlcujl.sHtML

[T26] Swift：类与重写
来源：http://m.share.hesvh.cn/Article/details/gbnnutbmd.sHtML

class A: Base { override func f() {} }
来源：http://www.m.share.zdbjq.cn/Article/details/gfullcnqj.sHtML

[T27] Swift：错误处理
来源：http://www.share.hesvh.cn/Article/details/ghjjyxnhp.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.hesvh.cn/Article/details/gkxflswwj.sHtML

[T28] Swift：枚举
来源：http://wap.hesvh.cn/Article/details/gjvoatybr.sHtML

enum Color { case red, green }
来源：http://www.blog.hesvh.cn/Article/details/gerlwqfqo.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.zdbjq.cn/Article/details/gdqfnfwui.sHtML

guard let x = opt else { return }
来源：http://baike.zdbjq.cn/Article/details/goppdzema.sHtML

[T30] Swift：协议
来源：http://mobile.zdbjq.cn/Article/details/gqhjymail.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.fehbvm.com/Article/details/gqajkckzm.sHtML

[T31] Lua：Hello World
来源：http://www.blog.hesvh.cn/Article/details/gcorjzrfq.sHtML

print("Hello")
来源：http://read.share.zdbjq.cn/Article/details/gvjzaruqe.sHtML

[T32] Lua：局部变量
来源：http://mobile.fehbvm.com/Article/details/gztdwjgqe.sHtML

local a = 1
来源：http://blog.zdbjq.cn/Article/details/gcwkmpmfr.sHtML

[T33] Lua：表（数组）
来源：http://wap.hesvh.cn/Article/details/gbcmqqqbb.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.fehbvm.com/Article/details/glrgzaerv.sHtML

[T34] Lua：遍历表
来源：http://www.m.share.fehbvm.com/Article/details/givnptomb.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.zdbjq.cn/Article/details/gacsfafee.sHtML

[T35] Lua：字典表
来源：http://m.share.zdbjq.cn/Article/details/gpaitnrpw.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.hesvh.cn/Article/details/gclkgnhng.sHtML

[T36] Lua：函数
来源：http://blog.zdbjq.cn/Article/details/gimvzeitv.sHtML

function add(a, b) return a + b end
来源：http://wap.hesvh.cn/Article/details/gbboptxvc.sHtML

[T37] Lua：字符串拼接
来源：http://wap.hesvh.cn/Article/details/gkbfidpgm.sHtML

"a" .. "b"
来源：http://blog.fehbvm.com/Article/details/gknibkrdw.sHtML

[T38] Lua：条件
来源：http://www.share.zdbjq.cn/Article/details/gfihtmraw.sHtML

if x > 0 then print("正") end
来源：http://www.share.fehbvm.com/Article/details/gygtlysmx.sHtML

[T39] Lua：模式匹配
来源：http://read.share.fehbvm.com/Article/details/gtmtnqhit.sHtML

string.find(s, "%d+")
来源：http://blog.fehbvm.com/Article/details/gwjxkoyqm.sHtML

[T40] Lua：元表
来源：http://3g.hesvh.cn/Article/details/gjvfhcpmz.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.fehbvm.com/Article/details/ggttfmqjp.sHtML

[T41] Perl：Hello World
来源：http://mobile.fehbvm.com/Article/details/gboqxxduu.sHtML

print "Hello\n";
来源：http://wap.hesvh.cn/Article/details/ghvqsacrg.sHtML

[T42] Perl：变量类型
来源：http://3g.fehbvm.com/Article/details/gxwgaxhug.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://read.share.hesvh.cn/Article/details/ggwptwbqr.sHtML

[T43] Perl：字符串插值
来源：http://3g.hesvh.cn/Article/details/gamrwlqvl.sHtML

"值: $a"
来源：http://blog.zdbjq.cn/Article/details/gniujxfec.sHtML

[T44] Perl：条件
来源：http://www.m.share.hesvh.cn/Article/details/gmmrmsamn.sHtML

if ($a > 0) { print "正"; }
来源：http://www.blog.hesvh.cn/Article/details/goczhjlul.sHtML

[T45] Perl：数组遍历
来源：http://read.share.hesvh.cn/Article/details/gyamohrpj.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.fehbvm.com/Article/details/gaqyzvqxp.sHtML

[T46] Perl：哈希操作
来源：http://wap.zdbjq.cn/Article/details/gvnlyouzt.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://m.share.hesvh.cn/Article/details/guowzmyif.sHtML

[T47] Perl：正则捕获
来源：http://read.share.zdbjq.cn/Article/details/gckqpbckc.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://m.share.fehbvm.com/Article/details/gvfthyerj.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.hesvh.cn/Article/details/guismbspk.sHtML

$s =~ s/old/new/g;
来源：http://read.share.fehbvm.com/Article/details/gfkbxpvme.sHtML

[T49] Perl：函数
来源：http://m.share.fehbvm.com/Article/details/gacrovjkf.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.hesvh.cn/Article/details/geatibdil.sHtML

[T50] Perl：逐行读文件
来源：http://wap.fehbvm.com/Article/details/gxwvximtw.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.hesvh.cn/Article/details/gnqsdobsk.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.m.share.fehbvm.com/Article/details/gxlynenxt.sHtML

[T51] Scala：Hello World
来源：http://m.share.zdbjq.cn/Article/details/gkbydufxh.sHtML

println("Hello")
来源：http://m.share.zdbjq.cn/Article/details/grmsiuprx.sHtML

[T52] Scala：变量
来源：http://www.blog.zdbjq.cn/Article/details/gffbxcnvb.sHtML

val a = 1;  var b = 2
来源：http://mobile.fehbvm.com/Article/details/gseguzqtf.sHtML

[T53] Scala：字符串插值
来源：http://mobile.hesvh.cn/Article/details/gmodoicwu.sHtML

s"值: $b"
来源：http://www.blog.fehbvm.com/Article/details/gqqrgtypf.sHtML

[T54] Scala：集合映射
来源：http://baike.fehbvm.com/Article/details/glisziqcd.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://baike.fehbvm.com/Article/details/gewrdgbno.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.zdbjq.cn/Article/details/gqlgmryho.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://blog.zdbjq.cn/Article/details/gkhjqledg.sHtML

[T56] Scala：样例类
来源：http://m.share.fehbvm.com/Article/details/gjdjvdmrg.sHtML

case class User(name: String, age: Int)
来源：http://m.share.fehbvm.com/Article/details/gojgasvlc.sHtML

[T57] Scala：模式匹配
来源：http://www.blog.zdbjq.cn/Article/details/glunokbjz.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.fehbvm.com/Article/details/gkrxddikx.sHtML

[T58] Scala：函数定义
来源：http://baike.zdbjq.cn/Article/details/ghxwuzxya.sHtML


<!-- 参考信息 -->