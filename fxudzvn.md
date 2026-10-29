代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://wap.hesvh.cn/Article/details/gvutnsxek.sHtML

[R52] 统计行数
来源：http://m.share.zdbjq.cn/Article/details/gtwueyzdo.sHtML

wc -l a.txt
来源：http://www.m.share.hesvh.cn/Article/details/gayifagnt.sHtML

[R53] 查看文件头与实时尾
来源：http://mobile.hesvh.cn/Article/details/gejldzmec.sHtML

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://www.blog.fehbvm.com/Article/details/ggfwuftqe.sHtML

[R54] 比较两个文件
来源：http://mobile.fehbvm.com/Article/details/glursgehm.sHtML

diff a.txt b.txt
来源：http://3g.hesvh.cn/Article/details/gmtphzpnv.sHtML

[R55] 压缩与解压
来源：http://blog.zdbjq.cn/Article/details/gtneyfmze.sHtML

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mobile.fehbvm.com/Article/details/gqlaesvwp.sHtML

[R56] 远程拷贝
来源：http://m.share.fehbvm.com/Article/details/gnyhklyox.sHtML

scp file user@host:/path/
来源：http://m.share.hesvh.cn/Article/details/guoczikkj.sHtML

[R57] 远程执行命令
来源：http://baike.fehbvm.com/Article/details/gcfclmdnm.sHtML

ssh user@host 'uptime'
来源：http://baike.zdbjq.cn/Article/details/gwektvigp.sHtML

[R58] 下载文件
来源：http://blog.hesvh.cn/Article/details/gyplpqhfl.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://baike.hesvh.cn/Article/details/gtvjqujfz.sHtML

[R59] 发 POST JSON
来源：http://www.m.share.fehbvm.com/Article/details/gvujzileq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://www.share.fehbvm.com/Article/details/gutdoufca.sHtML

[R60] 只看 HTTP 状态码
来源：http://read.share.hesvh.cn/Article/details/gwqfxslop.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://3g.hesvh.cn/Article/details/gvwahigoo.sHtML

[R61] 磁盘占用
来源：http://read.share.fehbvm.com/Article/details/gtyshqnpn.sHtML

df -h;  du -sh *
来源：http://www.share.hesvh.cn/Article/details/gdjahkxux.sHtML

[R62] 找最占空间的文件
来源：http://3g.zdbjq.cn/Article/details/goyriirvr.sHtML

du -ah . | sort -rh | head -10
来源：http://blog.hesvh.cn/Article/details/gkmhqgxjh.sHtML

[R63] 内存与进程
来源：http://mobile.hesvh.cn/Article/details/gwkclfdam.sHtML

free -h;  ps aux | grep nginx
来源：http://www.m.share.fehbvm.com/Article/details/gmhqhkyyf.sHtML

[R64] 结束进程
来源：http://mobile.zdbjq.cn/Article/details/grrswttml.sHtML

kill -9 $(pgrep -f app.py)
来源：http://3g.hesvh.cn/Article/details/gtgfzdjfh.sHtML

[R65] 查看端口占用
来源：http://www.m.share.fehbvm.com/Article/details/gpqirpsdq.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://baike.zdbjq.cn/Article/details/gbbtmyuop.sHtML

[R66] 定时任务
来源：http://baike.zdbjq.cn/Article/details/grmnsydhr.sHtML

crontab -e;  crontab -l
来源：http://m.share.fehbvm.com/Article/details/ghcmqspue.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.zdbjq.cn/Article/details/gpydvxefh.sHtML

openssl rand -hex 16
来源：http://baike.hesvh.cn/Article/details/ghumyoxug.sHtML

[R68] 计算文件校验值
来源：http://mobile.zdbjq.cn/Article/details/gtxklvdfh.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gyygjlaff.sHtML

[R69] 生成随机密码
来源：http://3g.fehbvm.com/Article/details/gowjynzqf.sHtML

head -c 16 /dev/urandom | base64
来源：http://www.blog.hesvh.cn/Article/details/gibfmqhtq.sHtML

[R70] 时间戳与互转
来源：http://baike.hesvh.cn/Article/details/gnpgcepdz.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fehbvm.com/Article/details/gsecmjjbz.sHtML

[R71] 日期格式化
来源：http://mobile.fehbvm.com/Article/details/gsyambxpr.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://mobile.fehbvm.com/Article/details/ggqyzlqkd.sHtML

[R72] 等待端口就绪
来源：http://m.share.hesvh.cn/Article/details/gocowvekb.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://wap.zdbjq.cn/Article/details/gdkmmsfzx.sHtML

[R73] 分割大日志
来源：http://www.m.share.zdbjq.cn/Article/details/gvbwiabes.sHtML

split -l 1000 big.log part_
来源：http://www.share.zdbjq.cn/Article/details/gojabpbxv.sHtML

[R74] 批量重命名
来源：http://mobile.fehbvm.com/Article/details/gtembnwzq.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.m.share.fehbvm.com/Article/details/gaytzusoa.sHtML

[R75] 导出环境变量
来源：http://m.share.hesvh.cn/Article/details/gcclhcsjm.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://baike.hesvh.cn/Article/details/gzpatjtom.sHtML

[R76] 使用临时文件
来源：http://www.share.zdbjq.cn/Article/details/gtrdqdgtk.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mobile.fehbvm.com/Article/details/grmskruzg.sHtML

[R77] 读取用户输入
来源：http://www.m.share.fehbvm.com/Article/details/gkrpueqzh.sHtML

read -rp "请输入: " ans
来源：http://www.blog.fehbvm.com/Article/details/ggyftvfcy.sHtML

[R78] 交互式菜单
来源：http://mobile.fehbvm.com/Article/details/gitbmtoyd.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://www.m.share.fehbvm.com/Article/details/gybepsuud.sHtML

[R79] 解析命令行选项
来源：http://3g.zdbjq.cn/Article/details/ghltpvlms.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://baike.fehbvm.com/Article/details/gqhyddmjo.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.hesvh.cn/Article/details/gclramwbt.sHtML

time ./run.sh
来源：http://blog.fehbvm.com/Article/details/gfvdnocys.sHtML

================================================================================
来源：http://www.share.fehbvm.com/Article/details/geizjxqos.sHtML

S. C / C++ 专题
来源：http://wap.zdbjq.cn/Article/details/gopbokddd.sHtML

================================================================================
来源：http://mobile.zdbjq.cn/Article/details/gzdbmfney.sHtML

[S01] C：Hello World
来源：http://www.m.share.fehbvm.com/Article/details/gxmyaihbb.sHtML

#include <stdio.h>
来源：http://www.blog.zdbjq.cn/Article/details/gmxvbbxge.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://baike.zdbjq.cn/Article/details/gfjoqnlsa.sHtML

[S02] C：变量与格式化输出
来源：http://www.blog.hesvh.cn/Article/details/gxirwwpsa.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.blog.fehbvm.com/Article/details/gjemoslcj.sHtML

[S03] C：读入整数
来源：http://mobile.fehbvm.com/Article/details/gxthtpvhp.sHtML

int x; scanf("%d", &x);
来源：http://www.blog.zdbjq.cn/Article/details/gxpzlshfg.sHtML

[S04] C：字符串复制
来源：http://blog.fehbvm.com/Article/details/gpuqpcqtc.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://baike.zdbjq.cn/Article/details/gaqptgwyv.sHtML

[S05] C：字符串长度
来源：http://mobile.hesvh.cn/Article/details/gshxmbete.sHtML

strlen(s)
来源：http://baike.zdbjq.cn/Article/details/gauvcmlgb.sHtML

[S06] C：字符串比较
来源：http://www.share.hesvh.cn/Article/details/gnedjnbys.sHtML

strcmp(a, b) == 0
来源：http://m.share.zdbjq.cn/Article/details/gccixoisf.sHtML

[S07] C：数组遍历求和
来源：http://www.m.share.hesvh.cn/Article/details/gjkbcmxij.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.blog.fehbvm.com/Article/details/ggpvivbhc.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.zdbjq.cn/Article/details/gvbamigbi.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.fehbvm.com/Article/details/giegwqskm.sHtML

[S09] C：结构体定义与初始化
来源：http://www.share.zdbjq.cn/Article/details/gxnevbkuc.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fehbvm.com/Article/details/gawrdvpsf.sHtML

[S10] C：指针与解引用
来源：http://3g.zdbjq.cn/Article/details/gcffvydzj.sHtML

int *p = &a;  *p = 5;
来源：http://m.share.fehbvm.com/Article/details/glgholkgr.sHtML

[S11] C：逐行读文件
来源：http://baike.zdbjq.cn/Article/details/gjckmjdcn.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://www.m.share.fehbvm.com/Article/details/gsstrdjex.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://mobile.fehbvm.com/Article/details/gccaemuxl.sHtML

fclose(f);
来源：http://mobile.zdbjq.cn/Article/details/gfvfqiywk.sHtML

[S12] C：写文件
来源：http://blog.hesvh.cn/Article/details/gjbxikpmv.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.m.share.fehbvm.com/Article/details/ghyjfxmab.sHtML

[S13] C：宏定义
来源：http://www.m.share.zdbjq.cn/Article/details/gpkjzynxm.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.blog.hesvh.cn/Article/details/gxexhwixq.sHtML

[S14] C：枚举
来源：http://m.share.hesvh.cn/Article/details/gnznhbues.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://baike.fehbvm.com/Article/details/ghtbccsxf.sHtML

[S15] C：类型转换
来源：http://blog.zdbjq.cn/Article/details/gtxkxmvzt.sHtML

(double) a / b
来源：http://www.m.share.zdbjq.cn/Article/details/gmgifeixy.sHtML

[S16] C：位操作置位
来源：http://read.share.fehbvm.com/Article/details/gwbxduqnf.sHtML

x |= (1 << 3);
来源：http://mobile.zdbjq.cn/Article/details/gownwyiii.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.fehbvm.com/Article/details/gtntpeylu.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fehbvm.com/Article/details/gpxohexut.sHtML

[S18] C：命令行参数
来源：http://baike.fehbvm.com/Article/details/gptchyepd.sHtML

int main(int argc, char **argv)
来源：http://www.share.zdbjq.cn/Article/details/gnejzdzip.sHtML

[S19] C：快速排序
来源：http://www.blog.zdbjq.cn/Article/details/gmrwzzovg.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://read.share.hesvh.cn/Article/details/gvhaoglwh.sHtML

[S20] C：二分查找
来源：http://mobile.hesvh.cn/Article/details/ghqikcwoz.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://3g.hesvh.cn/Article/details/gqfplafvn.sHtML

[S21] C：字符类别判断
来源：http://blog.fehbvm.com/Article/details/ggevqdpya.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://blog.fehbvm.com/Article/details/gduyqybhp.sHtML

[S22] C：字符串转数字
来源：http://www.blog.hesvh.cn/Article/details/gwuqeevbn.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://3g.zdbjq.cn/Article/details/gbvgqchrm.sHtML

[S23] C：随机数
来源：http://mobile.fehbvm.com/Article/details/gufklgmfw.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://wap.hesvh.cn/Article/details/gekduuxox.sHtML

[S24] C：获取本地时间
来源：http://www.m.share.fehbvm.com/Article/details/gybmoxdvv.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://m.share.zdbjq.cn/Article/details/gonnsxfif.sHtML

[S25] C：内存拷贝
来源：http://mobile.hesvh.cn/Article/details/guxmxrbgi.sHtML

memcpy(dst, src, n);
来源：http://read.share.zdbjq.cn/Article/details/gwsmfjfvo.sHtML

[S26] C：内存清零
来源：http://mobile.hesvh.cn/Article/details/gjlhqbcxt.sHtML

memset(a, 0, sizeof a);
来源：http://wap.zdbjq.cn/Article/details/ghnzcnbjj.sHtML

[S27] C：定义常量
来源：http://www.m.share.zdbjq.cn/Article/details/grigfrciq.sHtML

const double PI = 3.14159;
来源：http://m.share.fehbvm.com/Article/details/glqzckzri.sHtML

[S28] C：静态变量
来源：http://baike.fehbvm.com/Article/details/glexogklg.sHtML

static int counter = 0;
来源：http://read.share.fehbvm.com/Article/details/gfuvvznoz.sHtML

[S29] C：变参函数
来源：http://read.share.fehbvm.com/Article/details/gcgimrxsz.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://read.share.zdbjq.cn/Article/details/gwdxpebiy.sHtML

[S30] C：头文件保护
来源：http://www.share.zdbjq.cn/Article/details/gqpkbsxoz.sHtML

#ifndef X_H
来源：http://www.m.share.hesvh.cn/Article/details/gxrqihwqp.sHtML

#define X_H
来源：http://3g.hesvh.cn/Article/details/gymkkppve.sHtML

#endif
来源：http://wap.hesvh.cn/Article/details/gctvjqrcd.sHtML

[S31] C++：Hello World
来源：http://read.share.fehbvm.com/Article/details/goacyuvqg.sHtML

#include <iostream>
来源：http://blog.zdbjq.cn/Article/details/gftdpazdd.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.zdbjq.cn/Article/details/guxbuzspq.sHtML

[S32] C++：字符串
来源：http://m.share.zdbjq.cn/Article/details/gdbcjkdmw.sHtML

std::string s = "hi";  s += "!";
来源：http://www.share.zdbjq.cn/Article/details/gjfyjhinp.sHtML

[S33] C++：vector 增删
来源：http://3g.zdbjq.cn/Article/details/gdpidzqld.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wap.fehbvm.com/Article/details/grfvjxzfp.sHtML

[S34] C++：遍历 vector
来源：http://3g.fehbvm.com/Article/details/ggtxhsxqu.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.hesvh.cn/Article/details/gtnngevzb.sHtML

[S35] C++：map
来源：http://3g.zdbjq.cn/Article/details/gwvpotxsd.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gzkeoxzcx.sHtML

[S36] C++：unordered_map
来源：http://blog.fehbvm.com/Article/details/gyoumlbiw.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.fehbvm.com/Article/details/gmgjiabif.sHtML

[S37] C++：set
来源：http://m.share.fehbvm.com/Article/details/gmqxdsdkx.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mobile.hesvh.cn/Article/details/gseivdare.sHtML

[S38] C++：排序
来源：http://blog.fehbvm.com/Article/details/gsfzuarxz.sHtML

std::sort(v.begin(), v.end());
来源：http://m.share.fehbvm.com/Article/details/greoavgkm.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fehbvm.com/Article/details/gmrhxvvbb.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.m.share.hesvh.cn/Article/details/gkhmobzze.sHtML

[S40] C++：查找元素
来源：http://baike.zdbjq.cn/Article/details/gombrbnjz.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.share.hesvh.cn/Article/details/gbgqubozr.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.hesvh.cn/Article/details/gxltkmkah.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://blog.fehbvm.com/Article/details/gcdrydjro.sHtML

[S42] C++：继承与虚函数
来源：http://3g.fehbvm.com/Article/details/gtudifmoc.sHtML

class B : public Base { public: void f() override {} };
来源：http://mobile.fehbvm.com/Article/details/gogmxdycc.sHtML

[S43] C++：智能指针
来源：http://m.share.fehbvm.com/Article/details/gqnghwcpo.sHtML

auto p = std::make_unique<int>(5);
来源：http://wap.zdbjq.cn/Article/details/gifeqbcej.sHtML

[S44] C++：引用传参
来源：http://blog.hesvh.cn/Article/details/grhqvxoef.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.hesvh.cn/Article/details/gemopuruc.sHtML

[S45] C++：lambda
来源：http://baike.fehbvm.com/Article/details/grddsfucb.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.share.fehbvm.com/Article/details/gffhukjjs.sHtML

[S46] C++：函数模板
来源：http://mobile.zdbjq.cn/Article/details/gqtcmfjnx.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.m.share.hesvh.cn/Article/details/ghehjsqlj.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.zdbjq.cn/Article/details/gynwaugbb.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.blog.hesvh.cn/Article/details/gkvwqqzvx.sHtML

[S48] C++：逐行读文件
来源：http://blog.zdbjq.cn/Article/details/glypaczjt.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://blog.hesvh.cn/Article/details/gpaondslh.sHtML

while (std::getline(in, line)) { }
来源：http://baike.hesvh.cn/Article/details/ggyyoquqm.sHtML

[S49] C++：写文件
来源：http://wap.fehbvm.com/Article/details/guvzfukfl.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://baike.zdbjq.cn/Article/details/gvkwvxcft.sHtML

[S50] C++：格式化数字
来源：http://read.share.hesvh.cn/Article/details/gmgwdsjjs.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.zdbjq.cn/Article/details/gfkcfjozv.sHtML

[S51] C++：显式类型转换
来源：http://blog.zdbjq.cn/Article/details/gezreyaiu.sHtML

static_cast<double>(a) / b
来源：http://baike.zdbjq.cn/Article/details/gbyzxlzeq.sHtML

[S52] C++：const 与 noexcept
来源：http://baike.fehbvm.com/Article/details/gxwsnfwbk.sHtML

int size() const noexcept { return n_; }
来源：http://www.share.hesvh.cn/Article/details/gasfvnsiz.sHtML

[S53] C++：移动语义
来源：http://m.share.hesvh.cn/Article/details/gedcyxgsl.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fehbvm.com/Article/details/gkhbnmyic.sHtML

[S54] C++：异常处理
来源：http://mobile.fehbvm.com/Article/details/gjsczdghv.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://baike.hesvh.cn/Article/details/gnoxxfhkt.sHtML

[S55] C++：结构化绑定
来源：http://baike.fehbvm.com/Article/details/glftzrwhq.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.fehbvm.com/Article/details/gwphgsjgq.sHtML

[S56] C++：optional
来源：http://mobile.fehbvm.com/Article/details/gyhuwafzg.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://3g.zdbjq.cn/Article/details/ginpmexdl.sHtML

[S57] C++：编译期常量
来源：http://m.share.zdbjq.cn/Article/details/glesthqzf.sHtML

constexpr int N = 10;
来源：http://m.share.hesvh.cn/Article/details/gfkhvobco.sHtML

[S58] C++：命名空间
来源：http://www.blog.zdbjq.cn/Article/details/gthjivhva.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.fehbvm.com/Article/details/gchptsiaj.sHtML

[S59] C++：静态断言
来源：http://baike.zdbjq.cn/Article/details/gcdvkdhnk.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://blog.fehbvm.com/Article/details/gsqelrjrz.sHtML

[S60] C++：遍历并删除元素
来源：http://www.blog.zdbjq.cn/Article/details/gzpclrtdb.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://3g.zdbjq.cn/Article/details/gzvjlzual.sHtML

================================================================================
来源：http://www.share.hesvh.cn/Article/details/gygsblkcp.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.zdbjq.cn/Article/details/gczdrfktv.sHtML

================================================================================
来源：http://read.share.zdbjq.cn/Article/details/gfyizkrml.sHtML

[T01] Kotlin：Hello World
来源：http://mobile.hesvh.cn/Article/details/gefordolb.sHtML

println("Hello")
来源：http://m.share.hesvh.cn/Article/details/gyfqydghn.sHtML

[T02] Kotlin：变量
来源：http://read.share.fehbvm.com/Article/details/gleyalmfl.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wap.hesvh.cn/Article/details/gnsktxivk.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.zdbjq.cn/Article/details/glcjhfrmo.sHtML

"值: $b"
来源：http://wap.hesvh.cn/Article/details/glkhshozk.sHtML

[T04] Kotlin：空安全
来源：http://blog.hesvh.cn/Article/details/geyeidnhq.sHtML

val n: String? = null;  n?.length
来源：http://blog.zdbjq.cn/Article/details/gdfcvxoto.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.hesvh.cn/Article/details/gmkqkhgau.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.blog.hesvh.cn/Article/details/gtuvaffyk.sHtML

[T06] Kotlin：集合映射
来源：http://blog.fehbvm.com/Article/details/gpdpvsigq.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fehbvm.com/Article/details/gmcvwuror.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.hesvh.cn/Article/details/gejriszdv.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.share.fehbvm.com/Article/details/gtrcwyyst.sHtML

[T08] Kotlin：数据类
来源：http://3g.fehbvm.com/Article/details/ganhsbzfr.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.zdbjq.cn/Article/details/gspapfcdt.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.zdbjq.cn/Article/details/gtvanomqz.sHtML

fun String.exclaim() = this + "!"
来源：http://mobile.hesvh.cn/Article/details/gzcxrckcz.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fehbvm.com/Article/details/gujmdxhhl.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://mobile.hesvh.cn/Article/details/gywpwsxpm.sHtML

[T11] Kotlin：协程
来源：http://www.share.fehbvm.com/Article/details/ghibdnpgw.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.m.share.fehbvm.com/Article/details/gekhcrfdl.sHtML

[T12] Kotlin：解构声明
来源：http://www.share.hesvh.cn/Article/details/geagpwcao.sHtML

val (a, b) = Pair(1, 2)
来源：http://blog.fehbvm.com/Article/details/glbqfgnom.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.zdbjq.cn/Article/details/gwrshfmia.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.fehbvm.com/Article/details/gclzjwopb.sHtML

[T14] Kotlin：循环
来源：http://3g.zdbjq.cn/Article/details/gxkihorgs.sHtML

for (i in 1..10) println(i)
来源：http://www.share.zdbjq.cn/Article/details/gtgpuaist.sHtML

[T15] Kotlin：接口
来源：http://baike.hesvh.cn/Article/details/gerjqilio.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fehbvm.com/Article/details/glgbjzohk.sHtML

[T16] Swift：Hello World
来源：http://m.share.hesvh.cn/Article/details/gmuogoobd.sHtML

print("Hello")
来源：http://baike.fehbvm.com/Article/details/gitnkxemb.sHtML

[T17] Swift：变量与常量
来源：http://www.blog.zdbjq.cn/Article/details/ghwlgmdit.sHtML

var a = 1;  let b = 2
来源：http://wap.hesvh.cn/Article/details/gihtnqczi.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/gsketewaz.sHtML

"值: \(b)"
来源：http://mobile.zdbjq.cn/Article/details/gfzgcpviv.sHtML

[T19] Swift：可选绑定
来源：http://blog.zdbjq.cn/Article/details/gjkzsgfqw.sHtML

if let n = opt { print(n) }
来源：http://baike.fehbvm.com/Article/details/galfdbypo.sHtML

[T20] Swift：数组操作
来源：http://3g.zdbjq.cn/Article/details/gfrhrlilv.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.hesvh.cn/Article/details/gzpcyjuqf.sHtML

[T21] Swift：遍历
来源：http://www.m.share.hesvh.cn/Article/details/gzxmgpgqn.sHtML

for x in a { print(x) }
来源：http://3g.hesvh.cn/Article/details/guxvsvryk.sHtML

[T22] Swift：字典
来源：http://3g.zdbjq.cn/Article/details/ggznrhfgb.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.share.fehbvm.com/Article/details/gdjqvabtq.sHtML

[T23] Swift：函数
来源：http://wap.fehbvm.com/Article/details/gkzhopzsi.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://3g.zdbjq.cn/Article/details/glsaxbvdq.sHtML

[T24] Swift：闭包
来源：http://read.share.hesvh.cn/Article/details/gxnewfjzf.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gpqzlbrvu.sHtML

[T25] Swift：结构体
来源：http://m.share.zdbjq.cn/Article/details/grpctexcq.sHtML

struct P { var x: Int }
来源：http://wap.hesvh.cn/Article/details/gcooufung.sHtML

[T26] Swift：类与重写
来源：http://www.blog.zdbjq.cn/Article/details/gnxrqqwkf.sHtML

class A: Base { override func f() {} }
来源：http://baike.fehbvm.com/Article/details/gwmwwlqaq.sHtML

[T27] Swift：错误处理
来源：http://baike.fehbvm.com/Article/details/giunnkwvs.sHtML

do { try f() } catch { print(error) }
来源：http://wap.fehbvm.com/Article/details/geuslrrfk.sHtML

[T28] Swift：枚举
来源：http://mobile.zdbjq.cn/Article/details/gllipnzbx.sHtML

enum Color { case red, green }
来源：http://mobile.zdbjq.cn/Article/details/gilejsbez.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.fehbvm.com/Article/details/giidsadpv.sHtML

guard let x = opt else { return }
来源：http://mobile.zdbjq.cn/Article/details/ggbxpbokm.sHtML

[T30] Swift：协议
来源：http://wap.hesvh.cn/Article/details/gevxffeuc.sHtML

protocol Shape { func area() -> Double }
来源：http://m.share.hesvh.cn/Article/details/gcdvwnpcg.sHtML

[T31] Lua：Hello World
来源：http://read.share.hesvh.cn/Article/details/giwatyepa.sHtML

print("Hello")
来源：http://blog.hesvh.cn/Article/details/gzxylbnpi.sHtML

[T32] Lua：局部变量
来源：http://baike.fehbvm.com/Article/details/gqcrgsdfv.sHtML

local a = 1
来源：http://wap.hesvh.cn/Article/details/gxkngyvdh.sHtML

[T33] Lua：表（数组）
来源：http://www.blog.hesvh.cn/Article/details/grmxzhtfw.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.blog.zdbjq.cn/Article/details/gvgjspduo.sHtML

[T34] Lua：遍历表
来源：http://baike.fehbvm.com/Article/details/gvjgbtfsk.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.fehbvm.com/Article/details/gxdvgyvhw.sHtML

[T35] Lua：字典表
来源：http://baike.hesvh.cn/Article/details/gyrszitvu.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.hesvh.cn/Article/details/gwxgzobks.sHtML

[T36] Lua：函数
来源：http://read.share.hesvh.cn/Article/details/gukvhsbmu.sHtML

function add(a, b) return a + b end
来源：http://www.m.share.fehbvm.com/Article/details/gakodqyxd.sHtML

[T37] Lua：字符串拼接
来源：http://baike.fehbvm.com/Article/details/gxglnvquu.sHtML

"a" .. "b"
来源：http://wap.zdbjq.cn/Article/details/giuhtaxcf.sHtML

[T38] Lua：条件
来源：http://baike.zdbjq.cn/Article/details/gxrwnsrtd.sHtML

if x > 0 then print("正") end
来源：http://read.share.zdbjq.cn/Article/details/gkaurqeej.sHtML

[T39] Lua：模式匹配
来源：http://read.share.zdbjq.cn/Article/details/gmnqoppwa.sHtML

string.find(s, "%d+")
来源：http://blog.zdbjq.cn/Article/details/gkujnbaqg.sHtML

[T40] Lua：元表
来源：http://www.share.zdbjq.cn/Article/details/gwgximcyb.sHtML

setmetatable({}, { __index = base })
来源：http://www.share.fehbvm.com/Article/details/gvegpzdhd.sHtML

[T41] Perl：Hello World
来源：http://www.share.fehbvm.com/Article/details/gpzmkitet.sHtML

print "Hello\n";
来源：http://www.m.share.fehbvm.com/Article/details/gmkbpjicf.sHtML

[T42] Perl：变量类型
来源：http://mobile.fehbvm.com/Article/details/gypbxoohg.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://m.share.hesvh.cn/Article/details/gnnqcqajt.sHtML

[T43] Perl：字符串插值
来源：http://www.share.hesvh.cn/Article/details/grtzjlnyt.sHtML

"值: $a"
来源：http://m.share.zdbjq.cn/Article/details/gevauypfk.sHtML

[T44] Perl：条件
来源：http://wap.fehbvm.com/Article/details/gkswmiamp.sHtML

if ($a > 0) { print "正"; }
来源：http://blog.fehbvm.com/Article/details/grxgflrcj.sHtML

[T45] Perl：数组遍历
来源：http://www.share.zdbjq.cn/Article/details/grhvdpaju.sHtML

for my $x (@arr) { print $x; }
来源：http://www.blog.hesvh.cn/Article/details/gzbqzrzzj.sHtML

[T46] Perl：哈希操作
来源：http://mobile.fehbvm.com/Article/details/gehvlxrfy.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://read.share.zdbjq.cn/Article/details/gzqoladkk.sHtML

[T47] Perl：正则捕获
来源：http://m.share.zdbjq.cn/Article/details/gpkojyjds.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.hesvh.cn/Article/details/gwcxuwadv.sHtML

[T48] Perl：正则替换
来源：http://blog.zdbjq.cn/Article/details/gqtwbmqfb.sHtML

$s =~ s/old/new/g;
来源：http://baike.fehbvm.com/Article/details/ghrztdnmu.sHtML

[T49] Perl：函数
来源：http://mobile.fehbvm.com/Article/details/gepupzowz.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.m.share.hesvh.cn/Article/details/gaswgwtuz.sHtML

[T50] Perl：逐行读文件
来源：http://3g.fehbvm.com/Article/details/gkcvyxrmj.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://mobile.zdbjq.cn/Article/details/gxepzazjj.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.zdbjq.cn/Article/details/gvhogsqjq.sHtML

[T51] Scala：Hello World
来源：http://wap.fehbvm.com/Article/details/gpphcglsp.sHtML

println("Hello")
来源：http://blog.fehbvm.com/Article/details/gmsgoqewy.sHtML

[T52] Scala：变量
来源：http://baike.fehbvm.com/Article/details/gyzghxmwm.sHtML

val a = 1;  var b = 2
来源：http://baike.fehbvm.com/Article/details/gggyjmppl.sHtML

[T53] Scala：字符串插值
来源：http://blog.fehbvm.com/Article/details/gxlkyzdxy.sHtML

s"值: $b"
来源：http://baike.zdbjq.cn/Article/details/gvysmwssk.sHtML

[T54] Scala：集合映射
来源：http://www.m.share.fehbvm.com/Article/details/gaswnumlr.sHtML


<!-- 参考信息 -->