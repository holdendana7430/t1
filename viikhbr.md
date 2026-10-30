代发 wailian999

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://3g.fanxiaobao.xyz/Article/details/gkjslwwyk.sHtML

[R60] 只看 HTTP 状态码
来源：http://wap.fanxiaobao.xyz/Article/details/gywyoesvb.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://m.share.fanxiaobao.xyz/Article/details/gujukstvr.sHtML

[R61] 磁盘占用
来源：http://blog.fanxiaobao.xyz/Article/details/gxtyqlmfv.sHtML

df -h;  du -sh *
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyvxgdjwy.sHtML

[R62] 找最占空间的文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghtmdnjot.sHtML

du -ah . | sort -rh | head -10
来源：http://www.share.fanxiaobao.xyz/Article/details/gujdbpuvo.sHtML

[R63] 内存与进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gvqvqpgbd.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.fanxiaobao.xyz/Article/details/gbrvjlwdy.sHtML

[R64] 结束进程
来源：http://wap.fanxiaobao.xyz/Article/details/gdmtilcnh.sHtML

kill -9 $(pgrep -f app.py)
来源：http://mobile.fanxiaobao.xyz/Article/details/gfrmthdok.sHtML

[R65] 查看端口占用
来源：http://wap.fanxiaobao.xyz/Article/details/gwtkwfeqz.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fanxiaobao.xyz/Article/details/gzelxhwit.sHtML

[R66] 定时任务
来源：http://read.share.fanxiaobao.xyz/Article/details/gwjiwnemg.sHtML

crontab -e;  crontab -l
来源：http://wap.fanxiaobao.xyz/Article/details/glhgpzasb.sHtML

[R67] 生成随机十六进制串
来源：http://read.share.fanxiaobao.xyz/Article/details/gcieedvgo.sHtML

openssl rand -hex 16
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggtclqlys.sHtML

[R68] 计算文件校验值
来源：http://3g.fanxiaobao.xyz/Article/details/gwotppiis.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmygobmbs.sHtML

[R69] 生成随机密码
来源：http://read.share.fanxiaobao.xyz/Article/details/gfittsuvw.sHtML

head -c 16 /dev/urandom | base64
来源：http://wap.fanxiaobao.xyz/Article/details/glcfzfbzm.sHtML

[R70] 时间戳与互转
来源：http://blog.fanxiaobao.xyz/Article/details/gjtmypzio.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fanxiaobao.xyz/Article/details/gwvxiteuu.sHtML

[R71] 日期格式化
来源：http://read.share.fanxiaobao.xyz/Article/details/gvradpsct.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://baike.fanxiaobao.xyz/Article/details/gvggwmffx.sHtML

[R72] 等待端口就绪
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkdkzuzcp.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.fanxiaobao.xyz/Article/details/gdslhucqv.sHtML

[R73] 分割大日志
来源：http://wap.fanxiaobao.xyz/Article/details/gltgrhbbe.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghadjfjir.sHtML

[R74] 批量重命名
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gciizenmo.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.fanxiaobao.xyz/Article/details/gcgqwlwbn.sHtML

[R75] 导出环境变量
来源：http://wap.fanxiaobao.xyz/Article/details/gyzuctmtg.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://blog.fanxiaobao.xyz/Article/details/gwmhlfonq.sHtML

[R76] 使用临时文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gpnowunva.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://3g.fanxiaobao.xyz/Article/details/gubraqdgp.sHtML

[R77] 读取用户输入
来源：http://read.share.fanxiaobao.xyz/Article/details/gemjycmoj.sHtML

read -rp "请输入: " ans
来源：http://read.share.fanxiaobao.xyz/Article/details/grxujbzzb.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gruogbhan.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fanxiaobao.xyz/Article/details/gkwekvysk.sHtML

[R79] 解析命令行选项
来源：http://blog.fanxiaobao.xyz/Article/details/gmoznrwqt.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gbrbuaadf.sHtML

[R80] 查看脚本执行耗时
来源：http://www.share.fanxiaobao.xyz/Article/details/gtkgcnckg.sHtML

time ./run.sh
来源：http://3g.fanxiaobao.xyz/Article/details/gvsjpyyoj.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/guhwhzxon.sHtML

S. C / C++ 专题
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gilgvkktb.sHtML

================================================================================
来源：http://wap.fanxiaobao.xyz/Article/details/gdvjfwimq.sHtML

[S01] C：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gbnitdkud.sHtML

#include <stdio.h>
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gdbessnve.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfjtmvpbj.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fanxiaobao.xyz/Article/details/gpetjwebe.sHtML

int a = 10; printf("%d\n", a);
来源：http://read.share.fanxiaobao.xyz/Article/details/glarelwji.sHtML

[S03] C：读入整数
来源：http://3g.fanxiaobao.xyz/Article/details/goqrzapld.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fanxiaobao.xyz/Article/details/gsrrhjejh.sHtML

[S04] C：字符串复制
来源：http://m.share.fanxiaobao.xyz/Article/details/gysuwwreo.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://blog.fanxiaobao.xyz/Article/details/gzjiayqmx.sHtML

[S05] C：字符串长度
来源：http://read.share.fanxiaobao.xyz/Article/details/glifwmkee.sHtML

strlen(s)
来源：http://mobile.fanxiaobao.xyz/Article/details/gfdozskbv.sHtML

[S06] C：字符串比较
来源：http://wap.fanxiaobao.xyz/Article/details/gglcbspqj.sHtML

strcmp(a, b) == 0
来源：http://www.blog.fanxiaobao.xyz/Article/details/gflraaosu.sHtML

[S07] C：数组遍历求和
来源：http://blog.fanxiaobao.xyz/Article/details/gvqxvpepb.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fanxiaobao.xyz/Article/details/gflospoha.sHtML

[S08] C：动态内存分配与释放
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggbcjvspy.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fanxiaobao.xyz/Article/details/gycqkcmwg.sHtML

[S09] C：结构体定义与初始化
来源：http://www.blog.fanxiaobao.xyz/Article/details/gxrtxljyu.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvxgnzrdv.sHtML

[S10] C：指针与解引用
来源：http://mobile.fanxiaobao.xyz/Article/details/gynhdnwbc.sHtML

int *p = &a;  *p = 5;
来源：http://www.blog.fanxiaobao.xyz/Article/details/golwnuodr.sHtML

[S11] C：逐行读文件
来源：http://wap.fanxiaobao.xyz/Article/details/gqufdtaai.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fanxiaobao.xyz/Article/details/ggfixwxep.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/gzaoaitai.sHtML

fclose(f);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfncxflem.sHtML

[S12] C：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gqloqhsfk.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtibgefsd.sHtML

[S13] C：宏定义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcofyzrsv.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.share.fanxiaobao.xyz/Article/details/gklvcassx.sHtML

[S14] C：枚举
来源：http://baike.fanxiaobao.xyz/Article/details/gwkrlywfl.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://mobile.fanxiaobao.xyz/Article/details/gwpegvrcq.sHtML

[S15] C：类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/gkuraganq.sHtML

(double) a / b
来源：http://3g.fanxiaobao.xyz/Article/details/gswikxxku.sHtML

[S16] C：位操作置位
来源：http://read.share.fanxiaobao.xyz/Article/details/gwnblicjv.sHtML

x |= (1 << 3);
来源：http://read.share.fanxiaobao.xyz/Article/details/gjtzqpbac.sHtML

[S17] C：安全拼接字符串
来源：http://www.share.fanxiaobao.xyz/Article/details/gelvbxfxm.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpiildbnx.sHtML

[S18] C：命令行参数
来源：http://baike.fanxiaobao.xyz/Article/details/gihikerou.sHtML

int main(int argc, char **argv)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwelgjoqm.sHtML

[S19] C：快速排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gkvctpjcn.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gxztaqsji.sHtML

[S20] C：二分查找
来源：http://3g.fanxiaobao.xyz/Article/details/graiwjhkc.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://m.share.fanxiaobao.xyz/Article/details/gtmiqhpel.sHtML

[S21] C：字符类别判断
来源：http://baike.fanxiaobao.xyz/Article/details/gwlothcvs.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fanxiaobao.xyz/Article/details/gqmavimap.sHtML

[S22] C：字符串转数字
来源：http://m.share.fanxiaobao.xyz/Article/details/gxyuieazv.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://blog.fanxiaobao.xyz/Article/details/giqgawrda.sHtML

[S23] C：随机数
来源：http://read.share.fanxiaobao.xyz/Article/details/goejryovd.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.fanxiaobao.xyz/Article/details/goofnrjez.sHtML

[S24] C：获取本地时间
来源：http://3g.fanxiaobao.xyz/Article/details/gknarnaqv.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.share.fanxiaobao.xyz/Article/details/gufldnlzx.sHtML

[S25] C：内存拷贝
来源：http://mobile.fanxiaobao.xyz/Article/details/ghlvkfnvz.sHtML

memcpy(dst, src, n);
来源：http://m.share.fanxiaobao.xyz/Article/details/glpjqzosg.sHtML

[S26] C：内存清零
来源：http://wap.fanxiaobao.xyz/Article/details/ghcjvhuna.sHtML

memset(a, 0, sizeof a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvyddxskh.sHtML

[S27] C：定义常量
来源：http://m.share.fanxiaobao.xyz/Article/details/gmdcgfotm.sHtML

const double PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gouqemlgh.sHtML

[S28] C：静态变量
来源：http://wap.fanxiaobao.xyz/Article/details/gjxoubzkb.sHtML

static int counter = 0;
来源：http://wap.fanxiaobao.xyz/Article/details/gwkmmfgkl.sHtML

[S29] C：变参函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gcprcnsfk.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fanxiaobao.xyz/Article/details/grutcncmz.sHtML

[S30] C：头文件保护
来源：http://3g.fanxiaobao.xyz/Article/details/gqxkuscxn.sHtML

#ifndef X_H
来源：http://www.share.fanxiaobao.xyz/Article/details/gykmonwkn.sHtML

#define X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gsbzjveal.sHtML

#endif
来源：http://wap.fanxiaobao.xyz/Article/details/gnzmxllhu.sHtML

[S31] C++：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gjaeydjji.sHtML

#include <iostream>
来源：http://m.share.fanxiaobao.xyz/Article/details/gpxjwrbgo.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://baike.fanxiaobao.xyz/Article/details/gufyowlwp.sHtML

[S32] C++：字符串
来源：http://blog.fanxiaobao.xyz/Article/details/gnxcnkcyz.sHtML

std::string s = "hi";  s += "!";
来源：http://www.blog.fanxiaobao.xyz/Article/details/gufjdlfrv.sHtML

[S33] C++：vector 增删
来源：http://read.share.fanxiaobao.xyz/Article/details/gufydjuls.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://3g.fanxiaobao.xyz/Article/details/gemodjyqk.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fanxiaobao.xyz/Article/details/gctzqkfsg.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpspdbela.sHtML

[S35] C++：map
来源：http://baike.fanxiaobao.xyz/Article/details/gzmxzwzpb.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvppvnztv.sHtML

[S36] C++：unordered_map
来源：http://read.share.fanxiaobao.xyz/Article/details/gjdqsmaqx.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gjvfkedjq.sHtML

[S37] C++：set
来源：http://3g.fanxiaobao.xyz/Article/details/glujncetu.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwxczszum.sHtML

[S38] C++：排序
来源：http://m.share.fanxiaobao.xyz/Article/details/gsexpvucw.sHtML

std::sort(v.begin(), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghhufyklh.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.fanxiaobao.xyz/Article/details/gsslgwimv.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://baike.fanxiaobao.xyz/Article/details/gpaouibmk.sHtML

[S40] C++：查找元素
来源：http://mobile.fanxiaobao.xyz/Article/details/grdkpzaxc.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gtilqvcqj.sHtML

[S41] C++：类与构造函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/geizuwgyl.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.fanxiaobao.xyz/Article/details/gbsyzbedd.sHtML

[S42] C++：继承与虚函数
来源：http://m.share.fanxiaobao.xyz/Article/details/gmlsxzvsm.sHtML

class B : public Base { public: void f() override {} };
来源：http://wap.fanxiaobao.xyz/Article/details/gfqliuxyh.sHtML

[S43] C++：智能指针
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gapwssksy.sHtML

auto p = std::make_unique<int>(5);
来源：http://3g.fanxiaobao.xyz/Article/details/gxfvzltjf.sHtML

[S44] C++：引用传参
来源：http://wap.fanxiaobao.xyz/Article/details/grydrdqnd.sHtML

void inc(int &x) { ++x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gpkgkruzv.sHtML

[S45] C++：lambda
来源：http://www.share.fanxiaobao.xyz/Article/details/gjvhtqjul.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://m.share.fanxiaobao.xyz/Article/details/gyuuzysff.sHtML

[S46] C++：函数模板
来源：http://www.share.fanxiaobao.xyz/Article/details/gfvbkraan.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gksxlnvmb.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.share.fanxiaobao.xyz/Article/details/gkcptwruv.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://m.share.fanxiaobao.xyz/Article/details/gothshrpk.sHtML

[S48] C++：逐行读文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gfgpimngo.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjhnvwnas.sHtML

while (std::getline(in, line)) { }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpsxojecj.sHtML

[S49] C++：写文件
来源：http://mobile.fanxiaobao.xyz/Article/details/ggnofylur.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghwtiwynk.sHtML

[S50] C++：格式化数字
来源：http://3g.fanxiaobao.xyz/Article/details/gigkvrwmr.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://read.share.fanxiaobao.xyz/Article/details/gfqheggek.sHtML

[S51] C++：显式类型转换
来源：http://blog.fanxiaobao.xyz/Article/details/gennweeht.sHtML

static_cast<double>(a) / b
来源：http://baike.fanxiaobao.xyz/Article/details/ggyvwnxrq.sHtML

[S52] C++：const 与 noexcept
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gycrjdyxw.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gwjgoccft.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fanxiaobao.xyz/Article/details/geyarprbr.sHtML

std::vector<int> w = std::move(v);
来源：http://m.share.fanxiaobao.xyz/Article/details/gnhirdyuk.sHtML

[S54] C++：异常处理
来源：http://3g.fanxiaobao.xyz/Article/details/gvghlmmhf.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gssrybcad.sHtML

[S55] C++：结构化绑定
来源：http://wap.fanxiaobao.xyz/Article/details/guxclqlbz.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://baike.fanxiaobao.xyz/Article/details/gcwidgumz.sHtML

[S56] C++：optional
来源：http://3g.fanxiaobao.xyz/Article/details/gyqmbiwxg.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://blog.fanxiaobao.xyz/Article/details/gootoqmtn.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gaiikyyss.sHtML

constexpr int N = 10;
来源：http://wap.fanxiaobao.xyz/Article/details/gbigvjmay.sHtML

[S58] C++：命名空间
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfifvhnrm.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.fanxiaobao.xyz/Article/details/gzhzjjudv.sHtML

[S59] C++：静态断言
来源：http://baike.fanxiaobao.xyz/Article/details/gogorztfl.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvdqakthq.sHtML

[S60] C++：遍历并删除元素
来源：http://mobile.fanxiaobao.xyz/Article/details/ghqozwygv.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcpgkoloc.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gmjkesnty.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://baike.fanxiaobao.xyz/Article/details/grszojwsf.sHtML

================================================================================
来源：http://www.share.fanxiaobao.xyz/Article/details/gfjmcfwkn.sHtML

[T01] Kotlin：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gyososzgc.sHtML

println("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gscfsokkq.sHtML

[T02] Kotlin：变量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gmgrolutu.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://blog.fanxiaobao.xyz/Article/details/gpfetowwn.sHtML

[T03] Kotlin：字符串模板
来源：http://mobile.fanxiaobao.xyz/Article/details/grgixsmby.sHtML

"值: $b"
来源：http://read.share.fanxiaobao.xyz/Article/details/guefrctcf.sHtML

[T04] Kotlin：空安全
来源：http://read.share.fanxiaobao.xyz/Article/details/gemrfmvcc.sHtML

val n: String? = null;  n?.length
来源：http://baike.fanxiaobao.xyz/Article/details/gebhjfrra.sHtML

[T05] Kotlin：when 表达式
来源：http://www.share.fanxiaobao.xyz/Article/details/gfvsptcib.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://read.share.fanxiaobao.xyz/Article/details/gtzwacwid.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fanxiaobao.xyz/Article/details/gjoeopayk.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/gtnxenmim.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/gephbjlol.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://baike.fanxiaobao.xyz/Article/details/gvaqskkao.sHtML

[T08] Kotlin：数据类
来源：http://www.blog.fanxiaobao.xyz/Article/details/gixatgavo.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fanxiaobao.xyz/Article/details/gikfrjlwa.sHtML

[T09] Kotlin：扩展函数
来源：http://blog.fanxiaobao.xyz/Article/details/gdctjvxdd.sHtML

fun String.exclaim() = this + "!"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guivkevay.sHtML

[T10] Kotlin：默认参数
来源：http://blog.fanxiaobao.xyz/Article/details/gcndllzdy.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://3g.fanxiaobao.xyz/Article/details/gimqophlw.sHtML

[T11] Kotlin：协程
来源：http://blog.fanxiaobao.xyz/Article/details/gxzcgphuk.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fanxiaobao.xyz/Article/details/gfzmtugsk.sHtML

[T12] Kotlin：解构声明
来源：http://wap.fanxiaobao.xyz/Article/details/gjgsqgqqy.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfytlnsbb.sHtML

[T13] Kotlin：只读 Map
来源：http://3g.fanxiaobao.xyz/Article/details/gzsofpkpo.sHtML

val m = mapOf("a" to 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gzebijdon.sHtML

[T14] Kotlin：循环
来源：http://mobile.fanxiaobao.xyz/Article/details/gywnrcels.sHtML

for (i in 1..10) println(i)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtexwakar.sHtML

[T15] Kotlin：接口
来源：http://3g.fanxiaobao.xyz/Article/details/goybqbnjg.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gejxoqupp.sHtML

[T16] Swift：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gahtvkwdo.sHtML

print("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gekpretuf.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gubutajmo.sHtML

var a = 1;  let b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gmjbolovr.sHtML

[T18] Swift：字符串插值
来源：http://3g.fanxiaobao.xyz/Article/details/gzfdhahni.sHtML

"值: \(b)"
来源：http://m.share.fanxiaobao.xyz/Article/details/gyogmaovc.sHtML

[T19] Swift：可选绑定
来源：http://www.share.fanxiaobao.xyz/Article/details/gkotwxgkv.sHtML

if let n = opt { print(n) }
来源：http://baike.fanxiaobao.xyz/Article/details/gyywvmljj.sHtML

[T20] Swift：数组操作
来源：http://3g.fanxiaobao.xyz/Article/details/gjcscgito.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://mobile.fanxiaobao.xyz/Article/details/gwxpkhfam.sHtML

[T21] Swift：遍历
来源：http://blog.fanxiaobao.xyz/Article/details/grmpettjx.sHtML

for x in a { print(x) }
来源：http://mobile.fanxiaobao.xyz/Article/details/ghfaaifeq.sHtML

[T22] Swift：字典
来源：http://3g.fanxiaobao.xyz/Article/details/gfrotpish.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpyydqxhk.sHtML

[T23] Swift：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjjqqcnck.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.share.fanxiaobao.xyz/Article/details/ggoxjbhrj.sHtML

[T24] Swift：闭包
来源：http://www.share.fanxiaobao.xyz/Article/details/gsptzomzm.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://read.share.fanxiaobao.xyz/Article/details/guocewrkq.sHtML

[T25] Swift：结构体
来源：http://read.share.fanxiaobao.xyz/Article/details/gbjrlaeud.sHtML

struct P { var x: Int }
来源：http://baike.fanxiaobao.xyz/Article/details/gjbwprjpj.sHtML

[T26] Swift：类与重写
来源：http://www.blog.fanxiaobao.xyz/Article/details/grqtrazoy.sHtML

class A: Base { override func f() {} }
来源：http://baike.fanxiaobao.xyz/Article/details/ghjwgjltx.sHtML

[T27] Swift：错误处理
来源：http://baike.fanxiaobao.xyz/Article/details/gzoecxdxw.sHtML

do { try f() } catch { print(error) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbdvvacxm.sHtML

[T28] Swift：枚举
来源：http://www.share.fanxiaobao.xyz/Article/details/gaxffafmo.sHtML

enum Color { case red, green }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjlghjfam.sHtML

[T29] Swift：guard 提前返回
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfogvprpj.sHtML

guard let x = opt else { return }
来源：http://read.share.fanxiaobao.xyz/Article/details/gvrhsieud.sHtML

[T30] Swift：协议
来源：http://www.share.fanxiaobao.xyz/Article/details/gjbdbxvaz.sHtML

protocol Shape { func area() -> Double }
来源：http://baike.fanxiaobao.xyz/Article/details/goaouzeqt.sHtML

[T31] Lua：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gqbeemvrc.sHtML

print("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gjamcakzb.sHtML

[T32] Lua：局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/grmwgvppf.sHtML

local a = 1
来源：http://www.share.fanxiaobao.xyz/Article/details/gehnvldhv.sHtML

[T33] Lua：表（数组）
来源：http://blog.fanxiaobao.xyz/Article/details/gxumzzooa.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://www.share.fanxiaobao.xyz/Article/details/glepfjriq.sHtML

[T34] Lua：遍历表
来源：http://mobile.fanxiaobao.xyz/Article/details/grjorozcv.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://baike.fanxiaobao.xyz/Article/details/gjzmwiczh.sHtML

[T35] Lua：字典表
来源：http://wap.fanxiaobao.xyz/Article/details/gwwhkbvgh.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/grbsymgby.sHtML

[T36] Lua：函数
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvcfgjsib.sHtML

function add(a, b) return a + b end
来源：http://m.share.fanxiaobao.xyz/Article/details/gzvjlkxam.sHtML

[T37] Lua：字符串拼接
来源：http://www.share.fanxiaobao.xyz/Article/details/gkvzoalzc.sHtML

"a" .. "b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvekhrtdf.sHtML

[T38] Lua：条件
来源：http://blog.fanxiaobao.xyz/Article/details/gvagdtoue.sHtML

if x > 0 then print("正") end
来源：http://mobile.fanxiaobao.xyz/Article/details/gamcdonrx.sHtML

[T39] Lua：模式匹配
来源：http://blog.fanxiaobao.xyz/Article/details/gjvoqcwfx.sHtML

string.find(s, "%d+")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gzyrxnebb.sHtML

[T40] Lua：元表
来源：http://3g.fanxiaobao.xyz/Article/details/gavbixeqz.sHtML

setmetatable({}, { __index = base })
来源：http://www.blog.fanxiaobao.xyz/Article/details/gspxeanvs.sHtML

[T41] Perl：Hello World
来源：http://mobile.fanxiaobao.xyz/Article/details/gqomnqppb.sHtML

print "Hello\n";
来源：http://baike.fanxiaobao.xyz/Article/details/gwafthbzv.sHtML

[T42] Perl：变量类型
来源：http://read.share.fanxiaobao.xyz/Article/details/glrxgkegx.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.fanxiaobao.xyz/Article/details/ggqnzbikn.sHtML

[T43] Perl：字符串插值
来源：http://mobile.fanxiaobao.xyz/Article/details/ggxuwchcj.sHtML

"值: $a"
来源：http://blog.fanxiaobao.xyz/Article/details/gxotmswlk.sHtML

[T44] Perl：条件
来源：http://mobile.fanxiaobao.xyz/Article/details/glfhsfqqd.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/giyteyhwg.sHtML

[T45] Perl：数组遍历
来源：http://blog.fanxiaobao.xyz/Article/details/gqbklhfbx.sHtML

for my $x (@arr) { print $x; }
来源：http://wap.fanxiaobao.xyz/Article/details/gnrlvdrwp.sHtML

[T46] Perl：哈希操作
来源：http://www.share.fanxiaobao.xyz/Article/details/gjccqfito.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mobile.fanxiaobao.xyz/Article/details/gxnisjasv.sHtML

[T47] Perl：正则捕获
来源：http://wap.fanxiaobao.xyz/Article/details/gxibwttbg.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://wap.fanxiaobao.xyz/Article/details/gslgvwoxu.sHtML

[T48] Perl：正则替换
来源：http://read.share.fanxiaobao.xyz/Article/details/gymyfamoo.sHtML

$s =~ s/old/new/g;
来源：http://baike.fanxiaobao.xyz/Article/details/gwhpnlcoz.sHtML

[T49] Perl：函数
来源：http://www.blog.fanxiaobao.xyz/Article/details/gyxqcajtq.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gvfoeearu.sHtML

[T50] Perl：逐行读文件
来源：http://m.share.fanxiaobao.xyz/Article/details/gyvxfnkms.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtcmkqnss.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gxtfymbgy.sHtML

[T51] Scala：Hello World
来源：http://baike.fanxiaobao.xyz/Article/details/gugvilsif.sHtML

println("Hello")
来源：http://www.share.fanxiaobao.xyz/Article/details/gzuhhwbdm.sHtML

[T52] Scala：变量
来源：http://www.blog.fanxiaobao.xyz/Article/details/glngzycov.sHtML

val a = 1;  var b = 2
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvmeqztga.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gysaqbrrj.sHtML

s"值: $b"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gphrluvvh.sHtML

[T54] Scala：集合映射
来源：http://mobile.fanxiaobao.xyz/Article/details/gdezkadmb.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://3g.fanxiaobao.xyz/Article/details/gxcvoqhyr.sHtML

[T55] Scala：集合过滤
来源：http://www.share.fanxiaobao.xyz/Article/details/gpwmlwbpe.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsvmnptqm.sHtML

[T56] Scala：样例类
来源：http://blog.fanxiaobao.xyz/Article/details/gqereecxf.sHtML

case class User(name: String, age: Int)
来源：http://m.share.fanxiaobao.xyz/Article/details/gnkcqzhax.sHtML

[T57] Scala：模式匹配
来源：http://mobile.fanxiaobao.xyz/Article/details/gceryvjjt.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://mobile.fanxiaobao.xyz/Article/details/gqfxswzvk.sHtML

[T58] Scala：函数定义
来源：http://3g.fanxiaobao.xyz/Article/details/gzlvaklxg.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.share.fanxiaobao.xyz/Article/details/geinupctz.sHtML

[T59] Scala：循环
来源：http://m.share.fanxiaobao.xyz/Article/details/gxvhjncij.sHtML

for (i <- 1 to 10) println(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/gdaiknhgm.sHtML

[T60] Scala：折叠
来源：http://m.share.fanxiaobao.xyz/Article/details/gqsdycmhx.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://m.share.fanxiaobao.xyz/Article/details/gxfolbhvx.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/ggiblyhxe.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://blog.fanxiaobao.xyz/Article/details/gnuyqcabi.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gedbglsbt.sHtML


<!-- 参考信息 -->