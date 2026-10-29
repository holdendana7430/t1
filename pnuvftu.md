代发 wailian999

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://read.share.zdbjq.cn/Article/details/ggzhyqvcw.sHtML

[R60] 只看 HTTP 状态码
来源：http://www.blog.fehbvm.com/Article/details/gymlnbiav.sHtML

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://www.share.fehbvm.com/Article/details/gicbjsiie.sHtML

[R61] 磁盘占用
来源：http://mobile.hesvh.cn/Article/details/gqplxfvpf.sHtML

df -h;  du -sh *
来源：http://mobile.zdbjq.cn/Article/details/gyaezhmsr.sHtML

[R62] 找最占空间的文件
来源：http://baike.zdbjq.cn/Article/details/gqauxbysz.sHtML

du -ah . | sort -rh | head -10
来源：http://www.blog.fehbvm.com/Article/details/gpoyfsyan.sHtML

[R63] 内存与进程
来源：http://read.share.zdbjq.cn/Article/details/gqpwsoevm.sHtML

free -h;  ps aux | grep nginx
来源：http://m.share.zdbjq.cn/Article/details/glsqsfekg.sHtML

[R64] 结束进程
来源：http://blog.fehbvm.com/Article/details/gqzqjknyn.sHtML

kill -9 $(pgrep -f app.py)
来源：http://www.share.fehbvm.com/Article/details/geahejela.sHtML

[R65] 查看端口占用
来源：http://www.blog.hesvh.cn/Article/details/gfmgjctny.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wap.fehbvm.com/Article/details/gffsntphb.sHtML

[R66] 定时任务
来源：http://read.share.hesvh.cn/Article/details/gegemoerq.sHtML

crontab -e;  crontab -l
来源：http://read.share.zdbjq.cn/Article/details/gwvmeeufc.sHtML

[R67] 生成随机十六进制串
来源：http://mobile.fehbvm.com/Article/details/gbqqmuuqy.sHtML

openssl rand -hex 16
来源：http://m.share.zdbjq.cn/Article/details/gcnxaduma.sHtML

[R68] 计算文件校验值
来源：http://www.share.hesvh.cn/Article/details/glhfssxft.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://www.m.share.fehbvm.com/Article/details/gdychhfzr.sHtML

[R69] 生成随机密码
来源：http://wap.hesvh.cn/Article/details/glkuboqfo.sHtML

head -c 16 /dev/urandom | base64
来源：http://read.share.zdbjq.cn/Article/details/gsufpfxbx.sHtML

[R70] 时间戳与互转
来源：http://3g.hesvh.cn/Article/details/geyujcciy.sHtML

date +%s;  date -d @1700000000
来源：http://mobile.fehbvm.com/Article/details/gehspklmm.sHtML

[R71] 日期格式化
来源：http://www.m.share.fehbvm.com/Article/details/gsyqgebep.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.blog.hesvh.cn/Article/details/gbynpvjug.sHtML

[R72] 等待端口就绪
来源：http://3g.zdbjq.cn/Article/details/gijsnfwue.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://blog.hesvh.cn/Article/details/gzrowlhih.sHtML

[R73] 分割大日志
来源：http://www.share.hesvh.cn/Article/details/gkdhxqhhc.sHtML

split -l 1000 big.log part_
来源：http://www.m.share.fehbvm.com/Article/details/grsldmvdv.sHtML

[R74] 批量重命名
来源：http://mobile.hesvh.cn/Article/details/gaopzvzcp.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.blog.fehbvm.com/Article/details/gtzyuzmht.sHtML

[R75] 导出环境变量
来源：http://mobile.zdbjq.cn/Article/details/gpyfyjsow.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://read.share.zdbjq.cn/Article/details/guuwwzfcj.sHtML

[R76] 使用临时文件
来源：http://blog.hesvh.cn/Article/details/gvqzcpvad.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://read.share.fehbvm.com/Article/details/gjwumouze.sHtML

[R77] 读取用户输入
来源：http://read.share.zdbjq.cn/Article/details/ghmsqbbqg.sHtML

read -rp "请输入: " ans
来源：http://www.m.share.fehbvm.com/Article/details/goamegweb.sHtML

[R78] 交互式菜单
来源：http://wap.hesvh.cn/Article/details/gkfcfjenk.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://m.share.fehbvm.com/Article/details/gwbioyfcs.sHtML

[R79] 解析命令行选项
来源：http://wap.fehbvm.com/Article/details/goalixinm.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wap.hesvh.cn/Article/details/govbxxszz.sHtML

[R80] 查看脚本执行耗时
来源：http://m.share.fehbvm.com/Article/details/galxvzarf.sHtML

time ./run.sh
来源：http://mobile.zdbjq.cn/Article/details/gpcmbdcxg.sHtML

================================================================================
来源：http://www.blog.hesvh.cn/Article/details/grgghkcqf.sHtML

S. C / C++ 专题
来源：http://www.m.share.fehbvm.com/Article/details/gsxrhvjdn.sHtML

================================================================================
来源：http://mobile.fehbvm.com/Article/details/gprkglejj.sHtML

[S01] C：Hello World
来源：http://read.share.zdbjq.cn/Article/details/gpemmmkot.sHtML

#include <stdio.h>
来源：http://3g.fehbvm.com/Article/details/gmznaekea.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://m.share.zdbjq.cn/Article/details/gjfxbgdba.sHtML

[S02] C：变量与格式化输出
来源：http://read.share.fehbvm.com/Article/details/gwegceoea.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.m.share.zdbjq.cn/Article/details/gzcdcarif.sHtML

[S03] C：读入整数
来源：http://read.share.fehbvm.com/Article/details/gnjwcqruy.sHtML

int x; scanf("%d", &x);
来源：http://www.m.share.hesvh.cn/Article/details/gyfbcwqle.sHtML

[S04] C：字符串复制
来源：http://www.m.share.fehbvm.com/Article/details/gcpfizzky.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://wap.fehbvm.com/Article/details/gmlusrfxy.sHtML

[S05] C：字符串长度
来源：http://www.blog.fehbvm.com/Article/details/ghwpoymls.sHtML

strlen(s)
来源：http://wap.hesvh.cn/Article/details/gwoaowbjh.sHtML

[S06] C：字符串比较
来源：http://www.blog.fehbvm.com/Article/details/gaccbtxsx.sHtML

strcmp(a, b) == 0
来源：http://baike.hesvh.cn/Article/details/ggurashct.sHtML

[S07] C：数组遍历求和
来源：http://mobile.hesvh.cn/Article/details/ghcvpsegr.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mobile.hesvh.cn/Article/details/givetszxo.sHtML

[S08] C：动态内存分配与释放
来源：http://blog.hesvh.cn/Article/details/gqzlgnalz.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.m.share.zdbjq.cn/Article/details/goeuwojee.sHtML

[S09] C：结构体定义与初始化
来源：http://3g.zdbjq.cn/Article/details/galjebajl.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.m.share.fehbvm.com/Article/details/gudcewzws.sHtML

[S10] C：指针与解引用
来源：http://read.share.fehbvm.com/Article/details/gtlnzcsfa.sHtML

int *p = &a;  *p = 5;
来源：http://www.m.share.hesvh.cn/Article/details/glmddfssq.sHtML

[S11] C：逐行读文件
来源：http://wap.fehbvm.com/Article/details/giegggndk.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://wap.hesvh.cn/Article/details/gkvdsqzxi.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://wap.fehbvm.com/Article/details/gpaqnfzir.sHtML

fclose(f);
来源：http://wap.zdbjq.cn/Article/details/gjytpxrzi.sHtML

[S12] C：写文件
来源：http://www.blog.zdbjq.cn/Article/details/gpyasjnon.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://blog.fehbvm.com/Article/details/gtrnylpjk.sHtML

[S13] C：宏定义
来源：http://www.share.zdbjq.cn/Article/details/getwgfbgm.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://blog.hesvh.cn/Article/details/gerqumpjk.sHtML

[S14] C：枚举
来源：http://blog.hesvh.cn/Article/details/glzlrghyy.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://wap.hesvh.cn/Article/details/grrgprfrx.sHtML

[S15] C：类型转换
来源：http://www.m.share.zdbjq.cn/Article/details/gmppxtfpy.sHtML

(double) a / b
来源：http://baike.hesvh.cn/Article/details/gcjjliibt.sHtML

[S16] C：位操作置位
来源：http://baike.hesvh.cn/Article/details/geknjoohi.sHtML

x |= (1 << 3);
来源：http://m.share.hesvh.cn/Article/details/giwkgpseo.sHtML

[S17] C：安全拼接字符串
来源：http://www.blog.hesvh.cn/Article/details/gsqcqxzeu.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://read.share.hesvh.cn/Article/details/ghqyutrvj.sHtML

[S18] C：命令行参数
来源：http://www.m.share.zdbjq.cn/Article/details/glehhloda.sHtML

int main(int argc, char **argv)
来源：http://www.blog.hesvh.cn/Article/details/gsojmkkbk.sHtML

[S19] C：快速排序
来源：http://www.m.share.fehbvm.com/Article/details/ghlnhnfey.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://mobile.fehbvm.com/Article/details/gvkfcarcz.sHtML

[S20] C：二分查找
来源：http://read.share.zdbjq.cn/Article/details/gjiizrxcx.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://read.share.zdbjq.cn/Article/details/gponmorgs.sHtML

[S21] C：字符类别判断
来源：http://baike.fehbvm.com/Article/details/gimycqyop.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mobile.hesvh.cn/Article/details/gslvkwcdg.sHtML

[S22] C：字符串转数字
来源：http://3g.hesvh.cn/Article/details/ggnluawiz.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://mobile.hesvh.cn/Article/details/gshqxshpt.sHtML

[S23] C：随机数
来源：http://baike.zdbjq.cn/Article/details/gelduuuag.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://baike.hesvh.cn/Article/details/guejnqxdy.sHtML

[S24] C：获取本地时间
来源：http://baike.fehbvm.com/Article/details/gpbmvclfh.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.m.share.zdbjq.cn/Article/details/gfbzlnphm.sHtML

[S25] C：内存拷贝
来源：http://www.blog.fehbvm.com/Article/details/ghybnmdog.sHtML

memcpy(dst, src, n);
来源：http://wap.zdbjq.cn/Article/details/gilyckfnc.sHtML

[S26] C：内存清零
来源：http://blog.fehbvm.com/Article/details/giqxgdbwj.sHtML

memset(a, 0, sizeof a);
来源：http://m.share.zdbjq.cn/Article/details/gjpxbnngr.sHtML

[S27] C：定义常量
来源：http://m.share.zdbjq.cn/Article/details/gowiypmyu.sHtML

const double PI = 3.14159;
来源：http://www.m.share.zdbjq.cn/Article/details/gdqnvlcbr.sHtML

[S28] C：静态变量
来源：http://www.share.hesvh.cn/Article/details/gbsxfpczk.sHtML

static int counter = 0;
来源：http://wap.hesvh.cn/Article/details/gqxubyvgy.sHtML

[S29] C：变参函数
来源：http://www.blog.fehbvm.com/Article/details/gyczsgvel.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://baike.zdbjq.cn/Article/details/gsjrpgsxz.sHtML

[S30] C：头文件保护
来源：http://blog.fehbvm.com/Article/details/gdjlamknt.sHtML

#ifndef X_H
来源：http://read.share.hesvh.cn/Article/details/gslkjrahf.sHtML

#define X_H
来源：http://3g.zdbjq.cn/Article/details/gfmlenxka.sHtML

#endif
来源：http://www.blog.zdbjq.cn/Article/details/ghapnhetn.sHtML

[S31] C++：Hello World
来源：http://mobile.hesvh.cn/Article/details/gmiozietj.sHtML

#include <iostream>
来源：http://read.share.hesvh.cn/Article/details/gfytdkoaz.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://www.m.share.fehbvm.com/Article/details/gjzpxjync.sHtML

[S32] C++：字符串
来源：http://www.share.zdbjq.cn/Article/details/gyfihxuog.sHtML

std::string s = "hi";  s += "!";
来源：http://wap.fehbvm.com/Article/details/grhiainkc.sHtML

[S33] C++：vector 增删
来源：http://read.share.zdbjq.cn/Article/details/gfzvwpfcr.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mobile.zdbjq.cn/Article/details/gckkxwykm.sHtML

[S34] C++：遍历 vector
来源：http://www.m.share.hesvh.cn/Article/details/gvypwyjxe.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.zdbjq.cn/Article/details/gdcrzaxip.sHtML

[S35] C++：map
来源：http://wap.zdbjq.cn/Article/details/gzpysydyk.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://blog.hesvh.cn/Article/details/gwnfnekyt.sHtML

[S36] C++：unordered_map
来源：http://3g.fehbvm.com/Article/details/glcftxvwz.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.m.share.fehbvm.com/Article/details/gvlsybfyk.sHtML

[S37] C++：set
来源：http://read.share.zdbjq.cn/Article/details/gxfumfuig.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.m.share.fehbvm.com/Article/details/guzuwrqpy.sHtML

[S38] C++：排序
来源：http://www.m.share.zdbjq.cn/Article/details/gophdoghj.sHtML

std::sort(v.begin(), v.end());
来源：http://www.m.share.fehbvm.com/Article/details/guywzneeo.sHtML

[S39] C++：自定义比较器排序
来源：http://wap.zdbjq.cn/Article/details/ggnfqdebj.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://3g.hesvh.cn/Article/details/girmuahpe.sHtML

[S40] C++：查找元素
来源：http://m.share.fehbvm.com/Article/details/gfsvkxyor.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.m.share.zdbjq.cn/Article/details/gomznwbek.sHtML

[S41] C++：类与构造函数
来源：http://mobile.hesvh.cn/Article/details/gpzpprwov.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mobile.hesvh.cn/Article/details/gwfboudnr.sHtML

[S42] C++：继承与虚函数
来源：http://www.share.fehbvm.com/Article/details/gxxodthsz.sHtML

class B : public Base { public: void f() override {} };
来源：http://www.blog.hesvh.cn/Article/details/gbbghtlzx.sHtML

[S43] C++：智能指针
来源：http://blog.fehbvm.com/Article/details/goynvdboy.sHtML

auto p = std::make_unique<int>(5);
来源：http://blog.zdbjq.cn/Article/details/gbghfrrwg.sHtML

[S44] C++：引用传参
来源：http://m.share.fehbvm.com/Article/details/gkuyanbzq.sHtML

void inc(int &x) { ++x; }
来源：http://www.share.zdbjq.cn/Article/details/ghnutslko.sHtML

[S45] C++：lambda
来源：http://www.m.share.zdbjq.cn/Article/details/gakmwzfkj.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://www.m.share.fehbvm.com/Article/details/gkuwyrgha.sHtML

[S46] C++：函数模板
来源：http://www.blog.zdbjq.cn/Article/details/gumzrwdqh.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://m.share.hesvh.cn/Article/details/gpmoursbc.sHtML

[S47] C++：结构化绑定遍历
来源：http://mobile.hesvh.cn/Article/details/gxxljkdxh.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wap.fehbvm.com/Article/details/gwymgwafc.sHtML

[S48] C++：逐行读文件
来源：http://3g.hesvh.cn/Article/details/gnriiwnfl.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://wap.zdbjq.cn/Article/details/gdbzjvhzr.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.fehbvm.com/Article/details/gjgdusxeg.sHtML

[S49] C++：写文件
来源：http://blog.fehbvm.com/Article/details/ggazecivh.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://3g.zdbjq.cn/Article/details/grnyshevl.sHtML

[S50] C++：格式化数字
来源：http://blog.hesvh.cn/Article/details/gkysvfqom.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://blog.fehbvm.com/Article/details/goljyskhm.sHtML

[S51] C++：显式类型转换
来源：http://wap.hesvh.cn/Article/details/gkmidmrnq.sHtML

static_cast<double>(a) / b
来源：http://m.share.fehbvm.com/Article/details/gopcyodni.sHtML

[S52] C++：const 与 noexcept
来源：http://blog.zdbjq.cn/Article/details/grftxaejk.sHtML

int size() const noexcept { return n_; }
来源：http://read.share.fehbvm.com/Article/details/gihukqsyz.sHtML

[S53] C++：移动语义
来源：http://www.m.share.fehbvm.com/Article/details/gsfmydjjd.sHtML

std::vector<int> w = std::move(v);
来源：http://mobile.zdbjq.cn/Article/details/gegqlhucr.sHtML

[S54] C++：异常处理
来源：http://www.share.fehbvm.com/Article/details/gomnhnlhf.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mobile.hesvh.cn/Article/details/gvjqxfwjr.sHtML

[S55] C++：结构化绑定
来源：http://blog.hesvh.cn/Article/details/ghiottprr.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.hesvh.cn/Article/details/ggppmefch.sHtML

[S56] C++：optional
来源：http://m.share.fehbvm.com/Article/details/gwztxhnvh.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.hesvh.cn/Article/details/gymtkttzx.sHtML

[S57] C++：编译期常量
来源：http://blog.fehbvm.com/Article/details/gdudkunab.sHtML

constexpr int N = 10;
来源：http://baike.hesvh.cn/Article/details/giusikyku.sHtML

[S58] C++：命名空间
来源：http://baike.fehbvm.com/Article/details/gzmtvexeo.sHtML

namespace ns { int f() { return 1; } }
来源：http://www.share.zdbjq.cn/Article/details/gmqmnazev.sHtML

[S59] C++：静态断言
来源：http://read.share.zdbjq.cn/Article/details/gawqaqldj.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.zdbjq.cn/Article/details/gaekawjnn.sHtML

[S60] C++：遍历并删除元素
来源：http://baike.fehbvm.com/Article/details/gjdfgdlsr.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.hesvh.cn/Article/details/gucvdhbkb.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gewgudnop.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://blog.zdbjq.cn/Article/details/gjrwiuabi.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gjymgrnkp.sHtML

[T01] Kotlin：Hello World
来源：http://blog.hesvh.cn/Article/details/gxkpfuyqc.sHtML

println("Hello")
来源：http://wap.fehbvm.com/Article/details/gfmajoqhd.sHtML

[T02] Kotlin：变量
来源：http://m.share.fehbvm.com/Article/details/gmbcdjcus.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.fehbvm.com/Article/details/gizcxycai.sHtML

[T03] Kotlin：字符串模板
来源：http://read.share.zdbjq.cn/Article/details/gesxgzzwm.sHtML

"值: $b"
来源：http://blog.hesvh.cn/Article/details/gtfnqrxnq.sHtML

[T04] Kotlin：空安全
来源：http://blog.fehbvm.com/Article/details/geusyxyhg.sHtML

val n: String? = null;  n?.length
来源：http://blog.fehbvm.com/Article/details/gzdmiqjnm.sHtML

[T05] Kotlin：when 表达式
来源：http://mobile.zdbjq.cn/Article/details/gqvgtbyis.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://m.share.fehbvm.com/Article/details/gzmcidhkd.sHtML

[T06] Kotlin：集合映射
来源：http://m.share.zdbjq.cn/Article/details/gsyqacdbb.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://blog.zdbjq.cn/Article/details/gkpwgdhfs.sHtML

[T07] Kotlin：集合过滤
来源：http://m.share.fehbvm.com/Article/details/gwhwfiejv.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://blog.fehbvm.com/Article/details/gmskbukhv.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.hesvh.cn/Article/details/gmxzcogay.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.zdbjq.cn/Article/details/gdzkiljvw.sHtML

[T09] Kotlin：扩展函数
来源：http://mobile.fehbvm.com/Article/details/gudvucihe.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.hesvh.cn/Article/details/gzmqjzefl.sHtML

[T10] Kotlin：默认参数
来源：http://read.share.fehbvm.com/Article/details/gzeaxqrcq.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://read.share.zdbjq.cn/Article/details/gxqfbahxx.sHtML

[T11] Kotlin：协程
来源：http://www.m.share.fehbvm.com/Article/details/gdewpwjaa.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.zdbjq.cn/Article/details/gcregzddi.sHtML

[T12] Kotlin：解构声明
来源：http://www.m.share.fehbvm.com/Article/details/gxqctckvn.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.share.hesvh.cn/Article/details/gyokbqurs.sHtML

[T13] Kotlin：只读 Map
来源：http://www.m.share.zdbjq.cn/Article/details/gexzkxokg.sHtML

val m = mapOf("a" to 1)
来源：http://wap.zdbjq.cn/Article/details/gxmlgkmkh.sHtML

[T14] Kotlin：循环
来源：http://wap.fehbvm.com/Article/details/gkgbzpzwu.sHtML

for (i in 1..10) println(i)
来源：http://www.m.share.fehbvm.com/Article/details/gqynngvqt.sHtML

[T15] Kotlin：接口
来源：http://www.share.fehbvm.com/Article/details/gdcsdorwg.sHtML

interface Shape { fun area(): Double }
来源：http://www.share.zdbjq.cn/Article/details/gcgnmzvnz.sHtML

[T16] Swift：Hello World
来源：http://blog.fehbvm.com/Article/details/ghmfctang.sHtML

print("Hello")
来源：http://www.m.share.hesvh.cn/Article/details/gsmrjcvec.sHtML

[T17] Swift：变量与常量
来源：http://m.share.fehbvm.com/Article/details/gwgldfibe.sHtML

var a = 1;  let b = 2
来源：http://blog.zdbjq.cn/Article/details/glnthkssa.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.zdbjq.cn/Article/details/gepulgsow.sHtML

"值: \(b)"
来源：http://m.share.zdbjq.cn/Article/details/goyygpiws.sHtML

[T19] Swift：可选绑定
来源：http://www.m.share.zdbjq.cn/Article/details/gkkhzyjlx.sHtML

if let n = opt { print(n) }
来源：http://www.m.share.hesvh.cn/Article/details/gtevhmqzg.sHtML

[T20] Swift：数组操作
来源：http://m.share.fehbvm.com/Article/details/gskeyrubv.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://www.blog.fehbvm.com/Article/details/gogsphczb.sHtML

[T21] Swift：遍历
来源：http://www.m.share.hesvh.cn/Article/details/ghukzafph.sHtML

for x in a { print(x) }
来源：http://www.blog.fehbvm.com/Article/details/gmvyhdpcp.sHtML

[T22] Swift：字典
来源：http://baike.fehbvm.com/Article/details/geaoveuco.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.zdbjq.cn/Article/details/grbvnllgc.sHtML

[T23] Swift：函数
来源：http://www.share.hesvh.cn/Article/details/gelgnrlwt.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.m.share.hesvh.cn/Article/details/gkqrnfbgf.sHtML

[T24] Swift：闭包
来源：http://3g.fehbvm.com/Article/details/gifgbceln.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.m.share.hesvh.cn/Article/details/gcumerwkl.sHtML

[T25] Swift：结构体
来源：http://www.m.share.zdbjq.cn/Article/details/glrntrddt.sHtML

struct P { var x: Int }
来源：http://wap.hesvh.cn/Article/details/ggdnxkaeg.sHtML

[T26] Swift：类与重写
来源：http://www.m.share.hesvh.cn/Article/details/gmvesjcza.sHtML

class A: Base { override func f() {} }
来源：http://baike.fehbvm.com/Article/details/grnzvysro.sHtML

[T27] Swift：错误处理
来源：http://m.share.fehbvm.com/Article/details/gcgbejsbp.sHtML

do { try f() } catch { print(error) }
来源：http://www.m.share.zdbjq.cn/Article/details/ghvgmfffh.sHtML

[T28] Swift：枚举
来源：http://blog.fehbvm.com/Article/details/gmiincina.sHtML

enum Color { case red, green }
来源：http://wap.hesvh.cn/Article/details/gzhnkdfew.sHtML

[T29] Swift：guard 提前返回
来源：http://3g.hesvh.cn/Article/details/gtotvxdrr.sHtML

guard let x = opt else { return }
来源：http://baike.fehbvm.com/Article/details/gkcebutko.sHtML

[T30] Swift：协议
来源：http://baike.fehbvm.com/Article/details/gtuuwonir.sHtML

protocol Shape { func area() -> Double }
来源：http://3g.hesvh.cn/Article/details/grfffxytq.sHtML

[T31] Lua：Hello World
来源：http://wap.fehbvm.com/Article/details/gxigntbhd.sHtML

print("Hello")
来源：http://www.blog.fehbvm.com/Article/details/gvplpsinb.sHtML

[T32] Lua：局部变量
来源：http://www.share.zdbjq.cn/Article/details/gaiwjopxj.sHtML

local a = 1
来源：http://www.blog.zdbjq.cn/Article/details/gneyvedig.sHtML

[T33] Lua：表（数组）
来源：http://www.m.share.fehbvm.com/Article/details/gbscvsbqa.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://3g.zdbjq.cn/Article/details/gnylnqbgk.sHtML

[T34] Lua：遍历表
来源：http://wap.zdbjq.cn/Article/details/ghsphidji.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://www.blog.hesvh.cn/Article/details/gpspguekv.sHtML

[T35] Lua：字典表
来源：http://www.m.share.hesvh.cn/Article/details/ggtspqpne.sHtML

local d = { a = 1 };  d.b = 2
来源：http://www.m.share.zdbjq.cn/Article/details/geakohurf.sHtML

[T36] Lua：函数
来源：http://blog.fehbvm.com/Article/details/gdrqfnavz.sHtML

function add(a, b) return a + b end
来源：http://3g.zdbjq.cn/Article/details/gzozkaikg.sHtML

[T37] Lua：字符串拼接
来源：http://baike.hesvh.cn/Article/details/gbuiufdog.sHtML

"a" .. "b"
来源：http://blog.zdbjq.cn/Article/details/gnejyunqc.sHtML

[T38] Lua：条件
来源：http://wap.fehbvm.com/Article/details/gsaruksja.sHtML

if x > 0 then print("正") end
来源：http://mobile.zdbjq.cn/Article/details/gucomlenb.sHtML

[T39] Lua：模式匹配
来源：http://mobile.zdbjq.cn/Article/details/gjemzhacf.sHtML

string.find(s, "%d+")
来源：http://www.blog.zdbjq.cn/Article/details/gcigrvacr.sHtML

[T40] Lua：元表
来源：http://m.share.hesvh.cn/Article/details/gjguguxku.sHtML

setmetatable({}, { __index = base })
来源：http://wap.zdbjq.cn/Article/details/gowahitdc.sHtML

[T41] Perl：Hello World
来源：http://3g.fehbvm.com/Article/details/gtczmzcjz.sHtML

print "Hello\n";
来源：http://3g.zdbjq.cn/Article/details/gwyeckbfc.sHtML

[T42] Perl：变量类型
来源：http://www.m.share.zdbjq.cn/Article/details/gefsjsglc.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.fehbvm.com/Article/details/gxkiruizj.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gipubkymx.sHtML

"值: $a"
来源：http://read.share.hesvh.cn/Article/details/gxgadlsrv.sHtML

[T44] Perl：条件
来源：http://read.share.hesvh.cn/Article/details/gyadmpetz.sHtML

if ($a > 0) { print "正"; }
来源：http://read.share.fehbvm.com/Article/details/gmcolxrca.sHtML

[T45] Perl：数组遍历
来源：http://blog.zdbjq.cn/Article/details/giuoyvzbp.sHtML

for my $x (@arr) { print $x; }
来源：http://blog.fehbvm.com/Article/details/gqdwbpbvw.sHtML

[T46] Perl：哈希操作
来源：http://www.share.hesvh.cn/Article/details/gzjsfkqmy.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wap.hesvh.cn/Article/details/gimaojrww.sHtML

[T47] Perl：正则捕获
来源：http://wap.zdbjq.cn/Article/details/gkvykpfql.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://mobile.hesvh.cn/Article/details/gdpcdihgx.sHtML

[T48] Perl：正则替换
来源：http://3g.fehbvm.com/Article/details/glxptxtqb.sHtML

$s =~ s/old/new/g;
来源：http://mobile.hesvh.cn/Article/details/gzlgmrjyy.sHtML

[T49] Perl：函数
来源：http://m.share.fehbvm.com/Article/details/gulqzvwpk.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.share.zdbjq.cn/Article/details/gkvwmtjja.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.hesvh.cn/Article/details/gvkmjsweg.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://www.share.fehbvm.com/Article/details/gexdpwsrp.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://mobile.zdbjq.cn/Article/details/glooypvgi.sHtML

[T51] Scala：Hello World
来源：http://wap.fehbvm.com/Article/details/gjrkeledw.sHtML

println("Hello")
来源：http://www.share.fehbvm.com/Article/details/gdmluwuur.sHtML

[T52] Scala：变量
来源：http://www.m.share.zdbjq.cn/Article/details/garzxyfmd.sHtML

val a = 1;  var b = 2
来源：http://www.share.zdbjq.cn/Article/details/gvwfslwsc.sHtML

[T53] Scala：字符串插值
来源：http://wap.fehbvm.com/Article/details/gcxiyqiiv.sHtML

s"值: $b"
来源：http://www.share.fehbvm.com/Article/details/gaqklssam.sHtML

[T54] Scala：集合映射
来源：http://www.blog.zdbjq.cn/Article/details/ghqskouym.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://www.share.zdbjq.cn/Article/details/gesgxblhj.sHtML

[T55] Scala：集合过滤
来源：http://www.blog.fehbvm.com/Article/details/gjlezqtnq.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://wap.fehbvm.com/Article/details/giccvmhvq.sHtML

[T56] Scala：样例类
来源：http://mobile.fehbvm.com/Article/details/gcrorvgyb.sHtML

case class User(name: String, age: Int)
来源：http://mobile.fehbvm.com/Article/details/glrhwlfeb.sHtML

[T57] Scala：模式匹配
来源：http://m.share.zdbjq.cn/Article/details/gcewumijl.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://3g.hesvh.cn/Article/details/gggkxkqws.sHtML

[T58] Scala：函数定义
来源：http://www.share.zdbjq.cn/Article/details/gytkglrmy.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://www.m.share.hesvh.cn/Article/details/grzjggolt.sHtML

[T59] Scala：循环
来源：http://m.share.hesvh.cn/Article/details/gaqvgkzua.sHtML

for (i <- 1 to 10) println(i)
来源：http://www.m.share.fehbvm.com/Article/details/gsrxfyqeq.sHtML

[T60] Scala：折叠
来源：http://mobile.fehbvm.com/Article/details/ghjxplsqi.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.blog.zdbjq.cn/Article/details/gjbyfanun.sHtML

================================================================================
来源：http://blog.hesvh.cn/Article/details/ggyzikant.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.m.share.fehbvm.com/Article/details/gvhtufnob.sHtML

================================================================================
来源：http://baike.hesvh.cn/Article/details/gjvtqhxvf.sHtML


<!-- 参考信息 -->