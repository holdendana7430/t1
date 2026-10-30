代发 wailian999

ssh user@host 'uptime'
来源：http://blog.fanxiaobao.xyz/Article/details/gwqvirjlo.sHtML

[R58] 下载文件
来源：http://baike.fanxiaobao.xyz/Article/details/glqushksl.sHtML

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://www.share.fanxiaobao.xyz/Article/details/gkmfoyqfs.sHtML

[R59] 发 POST JSON
来源：http://www.blog.fanxiaobao.xyz/Article/details/gewlnzbeq.sHtML

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.fanxiaobao.xyz/Article/details/gnjnvjsrb.sHtML

[R60] 只看 HTTP 状态码
来源：http://baike.fanxiaobao.xyz/Article/details/gyyoxwmbu.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fanxiaobao.xyz/Article/details/gtsxkvaxy.sHtML

[R61] 磁盘占用
来源：http://wap.fanxiaobao.xyz/Article/details/gegioboiu.sHtML

df -h;  du -sh *
来源：http://read.share.fanxiaobao.xyz/Article/details/gvljoteuy.sHtML

[R62] 找最占空间的文件
来源：http://blog.fanxiaobao.xyz/Article/details/gfwgzxsqz.sHtML

du -ah . | sort -rh | head -10
来源：http://m.share.fanxiaobao.xyz/Article/details/ggtwutzss.sHtML

[R63] 内存与进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gcivacjui.sHtML

free -h;  ps aux | grep nginx
来源：http://www.blog.fanxiaobao.xyz/Article/details/gonxkqqds.sHtML

[R64] 结束进程
来源：http://www.share.fanxiaobao.xyz/Article/details/gbnhabynz.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.blog.fanxiaobao.xyz/Article/details/gydvzuurs.sHtML

[R65] 查看端口占用
来源：http://read.share.fanxiaobao.xyz/Article/details/grbyobimk.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.blog.fanxiaobao.xyz/Article/details/gffqfdpkf.sHtML

[R66] 定时任务
来源：http://www.share.fanxiaobao.xyz/Article/details/gextalqdf.sHtML

crontab -e;  crontab -l
来源：http://www.blog.fanxiaobao.xyz/Article/details/glqabdwcv.sHtML

[R67] 生成随机十六进制串
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbpzcmjkl.sHtML

openssl rand -hex 16
来源：http://baike.fanxiaobao.xyz/Article/details/gqhcviifu.sHtML

[R68] 计算文件校验值
来源：http://mobile.fanxiaobao.xyz/Article/details/gzactoxqo.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyczylmpt.sHtML

[R69] 生成随机密码
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghiyteikb.sHtML

head -c 16 /dev/urandom | base64
来源：http://blog.fanxiaobao.xyz/Article/details/grqkykmcs.sHtML

[R70] 时间戳与互转
来源：http://baike.fanxiaobao.xyz/Article/details/gtthdoilq.sHtML

date +%s;  date -d @1700000000
来源：http://www.blog.fanxiaobao.xyz/Article/details/grrjgqpuw.sHtML

[R71] 日期格式化
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gesqnltlc.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.fanxiaobao.xyz/Article/details/gslnvvnxq.sHtML

[R72] 等待端口就绪
来源：http://baike.fanxiaobao.xyz/Article/details/gzoveowvr.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.fanxiaobao.xyz/Article/details/gzfjgwdpl.sHtML

[R73] 分割大日志
来源：http://mobile.fanxiaobao.xyz/Article/details/gnswttrzp.sHtML

split -l 1000 big.log part_
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfkwlbvha.sHtML

[R74] 批量重命名
来源：http://baike.fanxiaobao.xyz/Article/details/gyfjhrgui.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://read.share.fanxiaobao.xyz/Article/details/guheunlxn.sHtML

[R75] 导出环境变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gkuwmtccg.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://mobile.fanxiaobao.xyz/Article/details/gkhanlrfh.sHtML

[R76] 使用临时文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gikahxffc.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wap.fanxiaobao.xyz/Article/details/gvqutrwat.sHtML

[R77] 读取用户输入
来源：http://read.share.fanxiaobao.xyz/Article/details/gcxwfrrmj.sHtML

read -rp "请输入: " ans
来源：http://m.share.fanxiaobao.xyz/Article/details/gisbmcqqp.sHtML

[R78] 交互式菜单
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjvfprfzq.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://wap.fanxiaobao.xyz/Article/details/gvdhwulhb.sHtML

[R79] 解析命令行选项
来源：http://blog.fanxiaobao.xyz/Article/details/gbhcbnaxy.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.share.fanxiaobao.xyz/Article/details/gqpbdisza.sHtML

[R80] 查看脚本执行耗时
来源：http://www.m.share.fanxiaobao.xyz/Article/details/govegnjsz.sHtML

time ./run.sh
来源：http://mobile.fanxiaobao.xyz/Article/details/ghduvoupm.sHtML

================================================================================
来源：http://baike.fanxiaobao.xyz/Article/details/gwlcxdzon.sHtML

S. C / C++ 专题
来源：http://www.share.fanxiaobao.xyz/Article/details/gxbxwzbsa.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gfjezrfmu.sHtML

[S01] C：Hello World
来源：http://read.share.fanxiaobao.xyz/Article/details/gpnkdagrw.sHtML

#include <stdio.h>
来源：http://blog.fanxiaobao.xyz/Article/details/gbznqgrtp.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://blog.fanxiaobao.xyz/Article/details/gaamylqzr.sHtML

[S02] C：变量与格式化输出
来源：http://wap.fanxiaobao.xyz/Article/details/gzsltskzy.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gacznruer.sHtML

[S03] C：读入整数
来源：http://blog.fanxiaobao.xyz/Article/details/gjpwdqtso.sHtML

int x; scanf("%d", &x);
来源：http://m.share.fanxiaobao.xyz/Article/details/gmpepkxuh.sHtML

[S04] C：字符串复制
来源：http://m.share.fanxiaobao.xyz/Article/details/gvisbqbrq.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpdxenqmb.sHtML

[S05] C：字符串长度
来源：http://baike.fanxiaobao.xyz/Article/details/gnoqsctns.sHtML

strlen(s)
来源：http://blog.fanxiaobao.xyz/Article/details/gkkjdjojh.sHtML

[S06] C：字符串比较
来源：http://baike.fanxiaobao.xyz/Article/details/ggufngpcw.sHtML

strcmp(a, b) == 0
来源：http://3g.fanxiaobao.xyz/Article/details/gkfyeblhp.sHtML

[S07] C：数组遍历求和
来源：http://3g.fanxiaobao.xyz/Article/details/gclutcsze.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://baike.fanxiaobao.xyz/Article/details/geqzuddue.sHtML

[S08] C：动态内存分配与释放
来源：http://www.share.fanxiaobao.xyz/Article/details/gubyexhpm.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://read.share.fanxiaobao.xyz/Article/details/gfnweusmt.sHtML

[S09] C：结构体定义与初始化
来源：http://baike.fanxiaobao.xyz/Article/details/gbadqduyz.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://mobile.fanxiaobao.xyz/Article/details/gyzonfzwm.sHtML

[S10] C：指针与解引用
来源：http://3g.fanxiaobao.xyz/Article/details/giincviku.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.fanxiaobao.xyz/Article/details/gskohksmj.sHtML

[S11] C：逐行读文件
来源：http://www.share.fanxiaobao.xyz/Article/details/gpnrtukbv.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://m.share.fanxiaobao.xyz/Article/details/gqomkebdk.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://blog.fanxiaobao.xyz/Article/details/gyrgqnkcc.sHtML

fclose(f);
来源：http://mobile.fanxiaobao.xyz/Article/details/gksjbrmfn.sHtML

[S12] C：写文件
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqfmeapkb.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://m.share.fanxiaobao.xyz/Article/details/gwdcbidas.sHtML

[S13] C：宏定义
来源：http://mobile.fanxiaobao.xyz/Article/details/gghdbcgdi.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://read.share.fanxiaobao.xyz/Article/details/gdwzslgjk.sHtML

[S14] C：枚举
来源：http://m.share.fanxiaobao.xyz/Article/details/gtixihzmv.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.fanxiaobao.xyz/Article/details/glvndfviy.sHtML

[S15] C：类型转换
来源：http://baike.fanxiaobao.xyz/Article/details/gnknxuese.sHtML

(double) a / b
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsxvokhmt.sHtML

[S16] C：位操作置位
来源：http://wap.fanxiaobao.xyz/Article/details/gplxazxmr.sHtML

x |= (1 << 3);
来源：http://wap.fanxiaobao.xyz/Article/details/gkaxkfrgs.sHtML

[S17] C：安全拼接字符串
来源：http://read.share.fanxiaobao.xyz/Article/details/gdxmzgpfl.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mobile.fanxiaobao.xyz/Article/details/gzsrraprz.sHtML

[S18] C：命令行参数
来源：http://read.share.fanxiaobao.xyz/Article/details/gsmkdjmeg.sHtML

int main(int argc, char **argv)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghmmbgxdg.sHtML

[S19] C：快速排序
来源：http://mobile.fanxiaobao.xyz/Article/details/gwroudwkp.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://wap.fanxiaobao.xyz/Article/details/gyfecshkh.sHtML

[S20] C：二分查找
来源：http://www.share.fanxiaobao.xyz/Article/details/gywzbwmkg.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.share.fanxiaobao.xyz/Article/details/gcnqhqwus.sHtML

[S21] C：字符类别判断
来源：http://mobile.fanxiaobao.xyz/Article/details/gvvgjeifn.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://read.share.fanxiaobao.xyz/Article/details/gaxqmopmp.sHtML

[S22] C：字符串转数字
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpdsetctk.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://baike.fanxiaobao.xyz/Article/details/gozzwstjn.sHtML

[S23] C：随机数
来源：http://blog.fanxiaobao.xyz/Article/details/gljesnzjl.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzbrosptm.sHtML

[S24] C：获取本地时间
来源：http://wap.fanxiaobao.xyz/Article/details/gummzxdsp.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://baike.fanxiaobao.xyz/Article/details/gedkfniqx.sHtML

[S25] C：内存拷贝
来源：http://www.share.fanxiaobao.xyz/Article/details/gurruxxyq.sHtML

memcpy(dst, src, n);
来源：http://3g.fanxiaobao.xyz/Article/details/gnxuusaqp.sHtML

[S26] C：内存清零
来源：http://m.share.fanxiaobao.xyz/Article/details/geypykxcc.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.fanxiaobao.xyz/Article/details/gthyndmxq.sHtML

[S27] C：定义常量
来源：http://www.share.fanxiaobao.xyz/Article/details/grkwuwymc.sHtML

const double PI = 3.14159;
来源：http://mobile.fanxiaobao.xyz/Article/details/gzbsybywy.sHtML

[S28] C：静态变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gdjiqfphj.sHtML

static int counter = 0;
来源：http://www.blog.fanxiaobao.xyz/Article/details/guaeezchh.sHtML

[S29] C：变参函数
来源：http://mobile.fanxiaobao.xyz/Article/details/gtigaccee.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wap.fanxiaobao.xyz/Article/details/gynlpyaah.sHtML

[S30] C：头文件保护
来源：http://www.blog.fanxiaobao.xyz/Article/details/gkrzsbjrm.sHtML

#ifndef X_H
来源：http://wap.fanxiaobao.xyz/Article/details/gczzuaepn.sHtML

#define X_H
来源：http://3g.fanxiaobao.xyz/Article/details/gellombay.sHtML

#endif
来源：http://www.share.fanxiaobao.xyz/Article/details/gwwnslhbz.sHtML

[S31] C++：Hello World
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyzlkxsbm.sHtML

#include <iostream>
来源：http://blog.fanxiaobao.xyz/Article/details/gwcvwypqc.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gmozhfixk.sHtML

[S32] C++：字符串
来源：http://wap.fanxiaobao.xyz/Article/details/gxhpnyewq.sHtML

std::string s = "hi";  s += "!";
来源：http://blog.fanxiaobao.xyz/Article/details/giazbnlsi.sHtML

[S33] C++：vector 增删
来源：http://mobile.fanxiaobao.xyz/Article/details/ggcpdecre.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://read.share.fanxiaobao.xyz/Article/details/gxzljgexk.sHtML

[S34] C++：遍历 vector
来源：http://mobile.fanxiaobao.xyz/Article/details/ghxrtyklp.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gsduhakto.sHtML

[S35] C++：map
来源：http://blog.fanxiaobao.xyz/Article/details/gxiypwtuj.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gfwqqilrm.sHtML

[S36] C++：unordered_map
来源：http://read.share.fanxiaobao.xyz/Article/details/gazkecopq.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://baike.fanxiaobao.xyz/Article/details/gtmluejws.sHtML

[S37] C++：set
来源：http://mobile.fanxiaobao.xyz/Article/details/gjmfdpwma.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwutrcunt.sHtML

[S38] C++：排序
来源：http://baike.fanxiaobao.xyz/Article/details/gpaoaxwjy.sHtML

std::sort(v.begin(), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/ghaqnridj.sHtML

[S39] C++：自定义比较器排序
来源：http://www.blog.fanxiaobao.xyz/Article/details/guitcwjmh.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://read.share.fanxiaobao.xyz/Article/details/gxxcunmxk.sHtML

[S40] C++：查找元素
来源：http://read.share.fanxiaobao.xyz/Article/details/gjurxipnw.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mobile.fanxiaobao.xyz/Article/details/gyxscihaq.sHtML

[S41] C++：类与构造函数
来源：http://www.share.fanxiaobao.xyz/Article/details/gjqaylclc.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.blog.fanxiaobao.xyz/Article/details/gpeippzma.sHtML

[S42] C++：继承与虚函数
来源：http://wap.fanxiaobao.xyz/Article/details/gchqhwkih.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gchzrwewq.sHtML

[S43] C++：智能指针
来源：http://read.share.fanxiaobao.xyz/Article/details/gshhulnsi.sHtML

auto p = std::make_unique<int>(5);
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gjuowmyxe.sHtML

[S44] C++：引用传参
来源：http://blog.fanxiaobao.xyz/Article/details/gqaegywab.sHtML

void inc(int &x) { ++x; }
来源：http://3g.fanxiaobao.xyz/Article/details/gdauuyvzy.sHtML

[S45] C++：lambda
来源：http://read.share.fanxiaobao.xyz/Article/details/govuamspl.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://wap.fanxiaobao.xyz/Article/details/gnieggbzm.sHtML

[S46] C++：函数模板
来源：http://baike.fanxiaobao.xyz/Article/details/gjeolrgah.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gwkdqrzts.sHtML

[S47] C++：结构化绑定遍历
来源：http://www.blog.fanxiaobao.xyz/Article/details/gqatpftco.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggiqtvpzh.sHtML

[S48] C++：逐行读文件
来源：http://blog.fanxiaobao.xyz/Article/details/gtntxdxsr.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://baike.fanxiaobao.xyz/Article/details/gmybanfqh.sHtML

while (std::getline(in, line)) { }
来源：http://wap.fanxiaobao.xyz/Article/details/gycteynys.sHtML

[S49] C++：写文件
来源：http://read.share.fanxiaobao.xyz/Article/details/gwfttcqgx.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://blog.fanxiaobao.xyz/Article/details/gmadjchnb.sHtML

[S50] C++：格式化数字
来源：http://blog.fanxiaobao.xyz/Article/details/ghpekpmjg.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghqahmibg.sHtML

[S51] C++：显式类型转换
来源：http://www.share.fanxiaobao.xyz/Article/details/grkyexdyt.sHtML

static_cast<double>(a) / b
来源：http://wap.fanxiaobao.xyz/Article/details/gzzykctfe.sHtML

[S52] C++：const 与 noexcept
来源：http://3g.fanxiaobao.xyz/Article/details/gdezfwbmm.sHtML

int size() const noexcept { return n_; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gllqlvrey.sHtML

[S53] C++：移动语义
来源：http://www.share.fanxiaobao.xyz/Article/details/gakhgbmqs.sHtML

std::vector<int> w = std::move(v);
来源：http://wap.fanxiaobao.xyz/Article/details/ghsvzpkfw.sHtML

[S54] C++：异常处理
来源：http://www.share.fanxiaobao.xyz/Article/details/gukexmwkb.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://read.share.fanxiaobao.xyz/Article/details/galffxywh.sHtML

[S55] C++：结构化绑定
来源：http://blog.fanxiaobao.xyz/Article/details/gjzpjoikr.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://wap.fanxiaobao.xyz/Article/details/gbshumsyk.sHtML

[S56] C++：optional
来源：http://baike.fanxiaobao.xyz/Article/details/gipzpcdky.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wap.fanxiaobao.xyz/Article/details/gvotnswzd.sHtML

[S57] C++：编译期常量
来源：http://wap.fanxiaobao.xyz/Article/details/gwjbaojea.sHtML

constexpr int N = 10;
来源：http://www.share.fanxiaobao.xyz/Article/details/gcrhviseq.sHtML

[S58] C++：命名空间
来源：http://www.blog.fanxiaobao.xyz/Article/details/guthodpbh.sHtML

namespace ns { int f() { return 1; } }
来源：http://baike.fanxiaobao.xyz/Article/details/gvqlymwqx.sHtML

[S59] C++：静态断言
来源：http://www.share.fanxiaobao.xyz/Article/details/gbaqynfsz.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mobile.fanxiaobao.xyz/Article/details/gzovlgfeo.sHtML

[S60] C++：遍历并删除元素
来源：http://3g.fanxiaobao.xyz/Article/details/gsyyegill.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fanxiaobao.xyz/Article/details/ggrxsovht.sHtML

================================================================================
来源：http://read.share.fanxiaobao.xyz/Article/details/gdtzgnqwt.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.share.fanxiaobao.xyz/Article/details/gddvmadrr.sHtML

================================================================================
来源：http://mobile.fanxiaobao.xyz/Article/details/gvoosviwg.sHtML

[T01] Kotlin：Hello World
来源：http://www.share.fanxiaobao.xyz/Article/details/ghqytamwv.sHtML

println("Hello")
来源：http://wap.fanxiaobao.xyz/Article/details/gdagyxawv.sHtML

[T02] Kotlin：变量
来源：http://read.share.fanxiaobao.xyz/Article/details/gmqgpcfry.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggsxpqjxu.sHtML

[T03] Kotlin：字符串模板
来源：http://www.blog.fanxiaobao.xyz/Article/details/gcpszinoa.sHtML

"值: $b"
来源：http://www.share.fanxiaobao.xyz/Article/details/gjqhxdbrn.sHtML

[T04] Kotlin：空安全
来源：http://www.share.fanxiaobao.xyz/Article/details/gtunmgrdv.sHtML

val n: String? = null;  n?.length
来源：http://baike.fanxiaobao.xyz/Article/details/grfmmglvr.sHtML

[T05] Kotlin：when 表达式
来源：http://blog.fanxiaobao.xyz/Article/details/gcxqiyatu.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.fanxiaobao.xyz/Article/details/gzisspsng.sHtML

[T06] Kotlin：集合映射
来源：http://read.share.fanxiaobao.xyz/Article/details/gtbnrdpjt.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbbsvrsuk.sHtML

[T07] Kotlin：集合过滤
来源：http://www.m.share.fanxiaobao.xyz/Article/details/guopdmigy.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gyrykrxpl.sHtML

[T08] Kotlin：数据类
来源：http://read.share.fanxiaobao.xyz/Article/details/gjoezubvu.sHtML

data class User(val name: String, val age: Int)
来源：http://wap.fanxiaobao.xyz/Article/details/gdrjrfsye.sHtML

[T09] Kotlin：扩展函数
来源：http://baike.fanxiaobao.xyz/Article/details/govafhkxk.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghhfeuhah.sHtML

[T10] Kotlin：默认参数
来源：http://m.share.fanxiaobao.xyz/Article/details/gajeeltlw.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://wap.fanxiaobao.xyz/Article/details/ginfvpmkw.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gvcotrcis.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://m.share.fanxiaobao.xyz/Article/details/gvlzhtxjs.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghmtfojrh.sHtML

val (a, b) = Pair(1, 2)
来源：http://m.share.fanxiaobao.xyz/Article/details/gqhuwuieo.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gcsfzqqpu.sHtML

val m = mapOf("a" to 1)
来源：http://3g.fanxiaobao.xyz/Article/details/gmwhvczdp.sHtML

[T14] Kotlin：循环
来源：http://www.blog.fanxiaobao.xyz/Article/details/geymmlxcg.sHtML

for (i in 1..10) println(i)
来源：http://m.share.fanxiaobao.xyz/Article/details/gmlxtgoqq.sHtML

[T15] Kotlin：接口
来源：http://read.share.fanxiaobao.xyz/Article/details/gbgjrrgdp.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.fanxiaobao.xyz/Article/details/gtiwgvwka.sHtML

[T16] Swift：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/gejwwutnd.sHtML

print("Hello")
来源：http://read.share.fanxiaobao.xyz/Article/details/gcloilzuo.sHtML

[T17] Swift：变量与常量
来源：http://3g.fanxiaobao.xyz/Article/details/gjjvieiud.sHtML

var a = 1;  let b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gsxtfgwzv.sHtML

[T18] Swift：字符串插值
来源：http://baike.fanxiaobao.xyz/Article/details/gtypjcbgd.sHtML

"值: \(b)"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/golwuqwuk.sHtML

[T19] Swift：可选绑定
来源：http://3g.fanxiaobao.xyz/Article/details/gyqmijqcg.sHtML

if let n = opt { print(n) }
来源：http://www.blog.fanxiaobao.xyz/Article/details/guwqcxorj.sHtML

[T20] Swift：数组操作
来源：http://blog.fanxiaobao.xyz/Article/details/gjovfeujn.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gsxomtibo.sHtML

[T21] Swift：遍历
来源：http://3g.fanxiaobao.xyz/Article/details/gmuhfrhpm.sHtML

for x in a { print(x) }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gevxunjue.sHtML

[T22] Swift：字典
来源：http://3g.fanxiaobao.xyz/Article/details/gfbtgcsdu.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gqcsndgzh.sHtML

[T23] Swift：函数
来源：http://wap.fanxiaobao.xyz/Article/details/gazpvlsgm.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mobile.fanxiaobao.xyz/Article/details/gzwmymewz.sHtML

[T24] Swift：闭包
来源：http://www.blog.fanxiaobao.xyz/Article/details/gwzklupty.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://blog.fanxiaobao.xyz/Article/details/gseuadgyh.sHtML

[T25] Swift：结构体
来源：http://www.blog.fanxiaobao.xyz/Article/details/gbcsytnof.sHtML

struct P { var x: Int }
来源：http://read.share.fanxiaobao.xyz/Article/details/glahsqljn.sHtML

[T26] Swift：类与重写
来源：http://www.share.fanxiaobao.xyz/Article/details/gqqlrpbmx.sHtML

class A: Base { override func f() {} }
来源：http://wap.fanxiaobao.xyz/Article/details/glkrswspm.sHtML

[T27] Swift：错误处理
来源：http://3g.fanxiaobao.xyz/Article/details/grtjluwad.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.fanxiaobao.xyz/Article/details/gignhxrag.sHtML

[T28] Swift：枚举
来源：http://www.blog.fanxiaobao.xyz/Article/details/gabepkgcf.sHtML

enum Color { case red, green }
来源：http://read.share.fanxiaobao.xyz/Article/details/gfsmouqih.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.fanxiaobao.xyz/Article/details/gjpapfqdj.sHtML

guard let x = opt else { return }
来源：http://www.share.fanxiaobao.xyz/Article/details/gdksosljf.sHtML

[T30] Swift：协议
来源：http://read.share.fanxiaobao.xyz/Article/details/gywvblwub.sHtML

protocol Shape { func area() -> Double }
来源：http://wap.fanxiaobao.xyz/Article/details/gxbrsvgze.sHtML

[T31] Lua：Hello World
来源：http://www.blog.fanxiaobao.xyz/Article/details/gccyhyelr.sHtML

print("Hello")
来源：http://mobile.fanxiaobao.xyz/Article/details/gvsvqxjur.sHtML

[T32] Lua：局部变量
来源：http://www.share.fanxiaobao.xyz/Article/details/gcsfgxneg.sHtML

local a = 1
来源：http://blog.fanxiaobao.xyz/Article/details/gdbkxpfcx.sHtML

[T33] Lua：表（数组）
来源：http://www.share.fanxiaobao.xyz/Article/details/ghkhkwlyw.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://read.share.fanxiaobao.xyz/Article/details/gofarhity.sHtML

[T34] Lua：遍历表
来源：http://www.blog.fanxiaobao.xyz/Article/details/ghmevuenl.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gunhygtmp.sHtML

[T35] Lua：字典表
来源：http://baike.fanxiaobao.xyz/Article/details/gnihfjatc.sHtML

local d = { a = 1 };  d.b = 2
来源：http://read.share.fanxiaobao.xyz/Article/details/gtofkdqmd.sHtML

[T36] Lua：函数
来源：http://blog.fanxiaobao.xyz/Article/details/gafagmfrm.sHtML

function add(a, b) return a + b end
来源：http://www.share.fanxiaobao.xyz/Article/details/gmiiuyldr.sHtML

[T37] Lua：字符串拼接
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gnwimvxku.sHtML

"a" .. "b"
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggnrfrvjg.sHtML

[T38] Lua：条件
来源：http://read.share.fanxiaobao.xyz/Article/details/gwkgalkbd.sHtML

if x > 0 then print("正") end
来源：http://blog.fanxiaobao.xyz/Article/details/gykbsbwpd.sHtML

[T39] Lua：模式匹配
来源：http://wap.fanxiaobao.xyz/Article/details/gcsrneyfy.sHtML

string.find(s, "%d+")
来源：http://read.share.fanxiaobao.xyz/Article/details/gmbkinkuq.sHtML

[T40] Lua：元表
来源：http://www.share.fanxiaobao.xyz/Article/details/gwcyttaxs.sHtML

setmetatable({}, { __index = base })
来源：http://read.share.fanxiaobao.xyz/Article/details/gosqlarjw.sHtML

[T41] Perl：Hello World
来源：http://3g.fanxiaobao.xyz/Article/details/gxdslrqdh.sHtML

print "Hello\n";
来源：http://blog.fanxiaobao.xyz/Article/details/ganlbutzy.sHtML

[T42] Perl：变量类型
来源：http://baike.fanxiaobao.xyz/Article/details/gxxjlmyqy.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://blog.fanxiaobao.xyz/Article/details/gkxcbavie.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ghtphtmsl.sHtML

"值: $a"
来源：http://m.share.fanxiaobao.xyz/Article/details/govezrzjk.sHtML

[T44] Perl：条件
来源：http://blog.fanxiaobao.xyz/Article/details/gasxyniri.sHtML

if ($a > 0) { print "正"; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/ggcqwonlg.sHtML

[T45] Perl：数组遍历
来源：http://blog.fanxiaobao.xyz/Article/details/goiankoig.sHtML

for my $x (@arr) { print $x; }
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gpzkhcqip.sHtML

[T46] Perl：哈希操作
来源：http://baike.fanxiaobao.xyz/Article/details/gctamwftz.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.share.fanxiaobao.xyz/Article/details/gcxynhywg.sHtML

[T47] Perl：正则捕获
来源：http://read.share.fanxiaobao.xyz/Article/details/gmpqdrsag.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://read.share.fanxiaobao.xyz/Article/details/gjvmhanpj.sHtML

[T48] Perl：正则替换
来源：http://www.share.fanxiaobao.xyz/Article/details/goisswazo.sHtML

$s =~ s/old/new/g;
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gixxehhil.sHtML

[T49] Perl：函数
来源：http://read.share.fanxiaobao.xyz/Article/details/gdsaqqdel.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wap.fanxiaobao.xyz/Article/details/gigzvytpl.sHtML

[T50] Perl：逐行读文件
来源：http://baike.fanxiaobao.xyz/Article/details/grvhdffzl.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://baike.fanxiaobao.xyz/Article/details/gujjfickz.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://www.blog.fanxiaobao.xyz/Article/details/gtuboamdq.sHtML

[T51] Scala：Hello World
来源：http://m.share.fanxiaobao.xyz/Article/details/giudsgrqt.sHtML

println("Hello")
来源：http://www.blog.fanxiaobao.xyz/Article/details/gfdeswqeg.sHtML

[T52] Scala：变量
来源：http://3g.fanxiaobao.xyz/Article/details/gkrifsvrz.sHtML

val a = 1;  var b = 2
来源：http://www.share.fanxiaobao.xyz/Article/details/gqnufeopl.sHtML

[T53] Scala：字符串插值
来源：http://www.m.share.fanxiaobao.xyz/Article/details/gonciafvy.sHtML

s"值: $b"
来源：http://mobile.fanxiaobao.xyz/Article/details/gsxrrwjrx.sHtML

[T54] Scala：集合映射
来源：http://baike.fanxiaobao.xyz/Article/details/guewaqpwa.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://mobile.fanxiaobao.xyz/Article/details/gsrxfyvmp.sHtML

[T55] Scala：集合过滤
来源：http://m.share.fanxiaobao.xyz/Article/details/glmozvjmd.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://www.blog.fanxiaobao.xyz/Article/details/ggnbjauiy.sHtML

[T56] Scala：样例类
来源：http://www.blog.fanxiaobao.xyz/Article/details/gjlqbzfhs.sHtML

case class User(name: String, age: Int)
来源：http://blog.fanxiaobao.xyz/Article/details/grzjmtbxv.sHtML

[T57] Scala：模式匹配
来源：http://read.share.fanxiaobao.xyz/Article/details/gjjskjykn.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.fanxiaobao.xyz/Article/details/gyxvmsayz.sHtML

[T58] Scala：函数定义
来源：http://www.blog.fanxiaobao.xyz/Article/details/gplitfyhq.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://mobile.fanxiaobao.xyz/Article/details/gqkfromft.sHtML

[T59] Scala：循环
来源：http://blog.fanxiaobao.xyz/Article/details/gsryzbccm.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.fanxiaobao.xyz/Article/details/gqsjsrvca.sHtML

[T60] Scala：折叠
来源：http://read.share.fanxiaobao.xyz/Article/details/goiormokj.sHtML


<!-- 参考信息 -->