代发 wailian999

df -h;  du -sh *
来源：http://3g.zdbjq.cn/Article/details/gwuzkjozf.sHtML

[R62] 找最占空间的文件
来源：http://mobile.hesvh.cn/Article/details/gzmwurzsd.sHtML

du -ah . | sort -rh | head -10
来源：http://wap.hesvh.cn/Article/details/grbvtdpgw.sHtML

[R63] 内存与进程
来源：http://baike.fehbvm.com/Article/details/giozamliv.sHtML

free -h;  ps aux | grep nginx
来源：http://3g.zdbjq.cn/Article/details/gzuqnbvjl.sHtML

[R64] 结束进程
来源：http://www.blog.fehbvm.com/Article/details/gkhqwxwoj.sHtML

kill -9 $(pgrep -f app.py)
来源：http://wap.hesvh.cn/Article/details/gkrmovjkv.sHtML

[R65] 查看端口占用
来源：http://read.share.fehbvm.com/Article/details/gnwdcpfkd.sHtML

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.m.share.hesvh.cn/Article/details/gyukisybn.sHtML

[R66] 定时任务
来源：http://mobile.fehbvm.com/Article/details/gnuhcvlcn.sHtML

crontab -e;  crontab -l
来源：http://m.share.hesvh.cn/Article/details/grayazitx.sHtML

[R67] 生成随机十六进制串
来源：http://m.share.zdbjq.cn/Article/details/gsolwqeea.sHtML

openssl rand -hex 16
来源：http://www.blog.zdbjq.cn/Article/details/gzozvlhgs.sHtML

[R68] 计算文件校验值
来源：http://mobile.zdbjq.cn/Article/details/gpbigqcyt.sHtML

sha256sum a.txt;  md5sum a.txt
来源：http://baike.zdbjq.cn/Article/details/gqhwgxwws.sHtML

[R69] 生成随机密码
来源：http://read.share.zdbjq.cn/Article/details/gyqxftcjh.sHtML

head -c 16 /dev/urandom | base64
来源：http://mobile.hesvh.cn/Article/details/gbbpaxiue.sHtML

[R70] 时间戳与互转
来源：http://www.m.share.hesvh.cn/Article/details/gmuhxweol.sHtML

date +%s;  date -d @1700000000
来源：http://www.share.fehbvm.com/Article/details/gprfcwyzk.sHtML

[R71] 日期格式化
来源：http://wap.hesvh.cn/Article/details/gvidwxges.sHtML

date +"%Y-%m-%d %H:%M:%S"
来源：http://m.share.fehbvm.com/Article/details/ghacjpsee.sHtML

[R72] 等待端口就绪
来源：http://3g.zdbjq.cn/Article/details/gbwquexau.sHtML

until nc -z localhost 3306; do sleep 1; done
来源：http://mobile.hesvh.cn/Article/details/gvecoouee.sHtML

[R73] 分割大日志
来源：http://baike.hesvh.cn/Article/details/gzwscciry.sHtML

split -l 1000 big.log part_
来源：http://read.share.fehbvm.com/Article/details/gnrilbpyl.sHtML

[R74] 批量重命名
来源：http://3g.hesvh.cn/Article/details/gszxdqeyh.sHtML

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://baike.zdbjq.cn/Article/details/gijcywdnc.sHtML

[R75] 导出环境变量
来源：http://m.share.zdbjq.cn/Article/details/gezleqfqv.sHtML

export PATH="$HOME/bin:$PATH"
来源：http://www.share.fehbvm.com/Article/details/gdjihmhoq.sHtML

[R76] 使用临时文件
来源：http://m.share.fehbvm.com/Article/details/gufpgjuoz.sHtML

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://blog.fehbvm.com/Article/details/goqzopzkx.sHtML

[R77] 读取用户输入
来源：http://mobile.zdbjq.cn/Article/details/gmeoetpaw.sHtML

read -rp "请输入: " ans
来源：http://mobile.fehbvm.com/Article/details/gzusibldq.sHtML

[R78] 交互式菜单
来源：http://www.m.share.fehbvm.com/Article/details/gylvlgfgv.sHtML

select opt in a b c; do echo "$opt"; break; done
来源：http://3g.fehbvm.com/Article/details/geoupsreu.sHtML

[R79] 解析命令行选项
来源：http://read.share.zdbjq.cn/Article/details/gfstyslhd.sHtML

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://read.share.fehbvm.com/Article/details/gmkppliox.sHtML

[R80] 查看脚本执行耗时
来源：http://3g.zdbjq.cn/Article/details/gqihemskv.sHtML

time ./run.sh
来源：http://wap.hesvh.cn/Article/details/gzakiteee.sHtML

================================================================================
来源：http://read.share.hesvh.cn/Article/details/gwkopcccb.sHtML

S. C / C++ 专题
来源：http://mobile.zdbjq.cn/Article/details/gbzcaguxz.sHtML

================================================================================
来源：http://3g.zdbjq.cn/Article/details/gxbzunxop.sHtML

[S01] C：Hello World
来源：http://wap.fehbvm.com/Article/details/glygkbnwg.sHtML

#include <stdio.h>
来源：http://3g.fehbvm.com/Article/details/gnaxgkeld.sHtML

int main(void) { printf("Hello\n"); return 0; }
来源：http://3g.zdbjq.cn/Article/details/gbpbbkbxk.sHtML

[S02] C：变量与格式化输出
来源：http://www.share.hesvh.cn/Article/details/gotqpsuvm.sHtML

int a = 10; printf("%d\n", a);
来源：http://www.share.hesvh.cn/Article/details/gicuybfbw.sHtML

[S03] C：读入整数
来源：http://www.m.share.fehbvm.com/Article/details/gxcmqbikh.sHtML

int x; scanf("%d", &x);
来源：http://3g.fehbvm.com/Article/details/goeoajnor.sHtML

[S04] C：字符串复制
来源：http://read.share.fehbvm.com/Article/details/gebnpmkxh.sHtML

char dst[32]; strcpy(dst, "hi");
来源：http://www.m.share.fehbvm.com/Article/details/grxwumvxa.sHtML

[S05] C：字符串长度
来源：http://baike.fehbvm.com/Article/details/gmikjebtn.sHtML

strlen(s)
来源：http://blog.zdbjq.cn/Article/details/gvkjmsagz.sHtML

[S06] C：字符串比较
来源：http://read.share.zdbjq.cn/Article/details/gryxflkop.sHtML

strcmp(a, b) == 0
来源：http://read.share.zdbjq.cn/Article/details/gnteduuvi.sHtML

[S07] C：数组遍历求和
来源：http://baike.fehbvm.com/Article/details/gyalkvksv.sHtML

for (int i = 0; i < n; i++) sum += a[i];
来源：http://m.share.hesvh.cn/Article/details/gqhqateno.sHtML

[S08] C：动态内存分配与释放
来源：http://read.share.hesvh.cn/Article/details/gglpqvybh.sHtML

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mobile.zdbjq.cn/Article/details/gzdjguyxf.sHtML

[S09] C：结构体定义与初始化
来源：http://wap.hesvh.cn/Article/details/gcxmbghev.sHtML

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://blog.hesvh.cn/Article/details/gksktjnkf.sHtML

[S10] C：指针与解引用
来源：http://www.share.hesvh.cn/Article/details/gyrcyjxyh.sHtML

int *p = &a;  *p = 5;
来源：http://www.share.hesvh.cn/Article/details/grkybyjgl.sHtML

[S11] C：逐行读文件
来源：http://mobile.fehbvm.com/Article/details/gvhulbtxu.sHtML

FILE *f = fopen("a.txt", "r");
来源：http://baike.hesvh.cn/Article/details/ggxvbgvxl.sHtML

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.m.share.zdbjq.cn/Article/details/gyddfdogo.sHtML

fclose(f);
来源：http://baike.fehbvm.com/Article/details/gvwzgzpyx.sHtML

[S12] C：写文件
来源：http://m.share.fehbvm.com/Article/details/gfwnmexil.sHtML

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wap.hesvh.cn/Article/details/gzopfjfga.sHtML

[S13] C：宏定义
来源：http://baike.zdbjq.cn/Article/details/ggzhydnoh.sHtML

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mobile.fehbvm.com/Article/details/gijlybzto.sHtML

[S14] C：枚举
来源：http://read.share.zdbjq.cn/Article/details/gkvcjjlyx.sHtML

enum Color { RED, GREEN, BLUE };
来源：http://www.share.fehbvm.com/Article/details/griqjytzc.sHtML

[S15] C：类型转换
来源：http://www.share.zdbjq.cn/Article/details/gxlirjpfp.sHtML

(double) a / b
来源：http://wap.fehbvm.com/Article/details/gcsfhdseh.sHtML

[S16] C：位操作置位
来源：http://blog.fehbvm.com/Article/details/gvpsrikyk.sHtML

x |= (1 << 3);
来源：http://mobile.fehbvm.com/Article/details/gmybfrioi.sHtML

[S17] C：安全拼接字符串
来源：http://mobile.fehbvm.com/Article/details/gkomyemya.sHtML

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.blog.fehbvm.com/Article/details/ggvshhxgs.sHtML

[S18] C：命令行参数
来源：http://www.share.hesvh.cn/Article/details/gzqzqolkp.sHtML

int main(int argc, char **argv)
来源：http://baike.fehbvm.com/Article/details/gjquykrfq.sHtML

[S19] C：快速排序
来源：http://read.share.zdbjq.cn/Article/details/gdkqxcbmt.sHtML

qsort(a, n, sizeof(int), cmp);
来源：http://3g.fehbvm.com/Article/details/gnszeusau.sHtML

[S20] C：二分查找
来源：http://3g.hesvh.cn/Article/details/gfhrrysve.sHtML

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wap.fehbvm.com/Article/details/gnvtgywef.sHtML

[S21] C：字符类别判断
来源：http://baike.fehbvm.com/Article/details/ggotijivi.sHtML

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.share.fehbvm.com/Article/details/gsfgrefik.sHtML

[S22] C：字符串转数字
来源：http://wap.zdbjq.cn/Article/details/gxizyyajx.sHtML

atoi("42");  strtod("3.14", NULL);
来源：http://www.m.share.fehbvm.com/Article/details/ggewppioj.sHtML

[S23] C：随机数
来源：http://m.share.zdbjq.cn/Article/details/ggsyoaktb.sHtML

srand(time(NULL));  int r = rand() % 100;
来源：http://m.share.hesvh.cn/Article/details/gktpuwbhx.sHtML

[S24] C：获取本地时间
来源：http://www.blog.zdbjq.cn/Article/details/gqwadogix.sHtML

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://blog.hesvh.cn/Article/details/gqdzydmqm.sHtML

[S25] C：内存拷贝
来源：http://www.share.hesvh.cn/Article/details/gaapsusxt.sHtML

memcpy(dst, src, n);
来源：http://blog.fehbvm.com/Article/details/ggqovnydr.sHtML

[S26] C：内存清零
来源：http://3g.fehbvm.com/Article/details/gvvjqpoga.sHtML

memset(a, 0, sizeof a);
来源：http://blog.fehbvm.com/Article/details/gfpxrxoax.sHtML

[S27] C：定义常量
来源：http://wap.hesvh.cn/Article/details/gvgplnxgf.sHtML

const double PI = 3.14159;
来源：http://3g.zdbjq.cn/Article/details/gtduwdwvm.sHtML

[S28] C：静态变量
来源：http://www.m.share.fehbvm.com/Article/details/gbzxyadai.sHtML

static int counter = 0;
来源：http://baike.zdbjq.cn/Article/details/glqwehstc.sHtML

[S29] C：变参函数
来源：http://blog.fehbvm.com/Article/details/gvixfsyds.sHtML

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mobile.hesvh.cn/Article/details/gmdhjdglo.sHtML

[S30] C：头文件保护
来源：http://wap.zdbjq.cn/Article/details/ghuysympl.sHtML

#ifndef X_H
来源：http://www.blog.fehbvm.com/Article/details/gmvvmuhey.sHtML

#define X_H
来源：http://mobile.hesvh.cn/Article/details/gayfnqqcm.sHtML

#endif
来源：http://mobile.zdbjq.cn/Article/details/gtrdlroff.sHtML

[S31] C++：Hello World
来源：http://read.share.fehbvm.com/Article/details/gyxaxzoef.sHtML

#include <iostream>
来源：http://3g.fehbvm.com/Article/details/gizwcsnra.sHtML

int main() { std::cout << "Hello\n"; }
来源：http://blog.hesvh.cn/Article/details/gvjhprnxj.sHtML

[S32] C++：字符串
来源：http://www.share.fehbvm.com/Article/details/gidazatex.sHtML

std::string s = "hi";  s += "!";
来源：http://m.share.zdbjq.cn/Article/details/gyfseqdwj.sHtML

[S33] C++：vector 增删
来源：http://3g.zdbjq.cn/Article/details/gltgkxoan.sHtML

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://baike.hesvh.cn/Article/details/gcebvoyaa.sHtML

[S34] C++：遍历 vector
来源：http://read.share.fehbvm.com/Article/details/grhjoeaeb.sHtML

for (auto &x : v) { std::cout << x; }
来源：http://read.share.hesvh.cn/Article/details/ghpdddlpt.sHtML

[S35] C++：map
来源：http://www.blog.fehbvm.com/Article/details/gsnwiwtcq.sHtML

std::map<std::string, int> m;  m["a"] = 1;
来源：http://m.share.hesvh.cn/Article/details/gusgpnakx.sHtML

[S36] C++：unordered_map
来源：http://3g.fehbvm.com/Article/details/gcueiqgjh.sHtML

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://blog.zdbjq.cn/Article/details/gfxnnftqu.sHtML

[S37] C++：set
来源：http://mobile.zdbjq.cn/Article/details/gpfpwwsga.sHtML

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.share.zdbjq.cn/Article/details/gmmqmmvvn.sHtML

[S38] C++：排序
来源：http://mobile.hesvh.cn/Article/details/gqfniorka.sHtML

std::sort(v.begin(), v.end());
来源：http://baike.fehbvm.com/Article/details/gbcktijgh.sHtML

[S39] C++：自定义比较器排序
来源：http://blog.fehbvm.com/Article/details/gdlbcockm.sHtML

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://m.share.hesvh.cn/Article/details/ggheguonr.sHtML

[S40] C++：查找元素
来源：http://m.share.fehbvm.com/Article/details/gjqkrhzkn.sHtML

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.blog.fehbvm.com/Article/details/gnjkpzhlz.sHtML

[S41] C++：类与构造函数
来源：http://mobile.hesvh.cn/Article/details/gnkcigpyv.sHtML

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://baike.hesvh.cn/Article/details/gyfqdptxl.sHtML

[S42] C++：继承与虚函数
来源：http://www.m.share.zdbjq.cn/Article/details/ggygwvqtx.sHtML

class B : public Base { public: void f() override {} };
来源：http://baike.fehbvm.com/Article/details/gxonqfyli.sHtML

[S43] C++：智能指针
来源：http://wap.zdbjq.cn/Article/details/glpoizqmq.sHtML

auto p = std::make_unique<int>(5);
来源：http://baike.zdbjq.cn/Article/details/ghjflxhiq.sHtML

[S44] C++：引用传参
来源：http://blog.fehbvm.com/Article/details/grubwaiye.sHtML

void inc(int &x) { ++x; }
来源：http://baike.zdbjq.cn/Article/details/gtikihkeh.sHtML

[S45] C++：lambda
来源：http://m.share.fehbvm.com/Article/details/gkjmpzjao.sHtML

auto add = [](int a, int b) { return a + b; };
来源：http://blog.hesvh.cn/Article/details/gcbspwtem.sHtML

[S46] C++：函数模板
来源：http://mobile.hesvh.cn/Article/details/gmfxqiweu.sHtML

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.share.fehbvm.com/Article/details/gtdkzcfut.sHtML

[S47] C++：结构化绑定遍历
来源：http://read.share.hesvh.cn/Article/details/gxqhtfvnl.sHtML

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mobile.hesvh.cn/Article/details/ggkhdhnem.sHtML

[S48] C++：逐行读文件
来源：http://wap.fehbvm.com/Article/details/gsyrdpwpq.sHtML

std::ifstream in("a.txt");  std::string line;
来源：http://read.share.fehbvm.com/Article/details/gclltbwip.sHtML

while (std::getline(in, line)) { }
来源：http://www.share.zdbjq.cn/Article/details/grjfiiuni.sHtML

[S49] C++：写文件
来源：http://baike.zdbjq.cn/Article/details/glimwqajl.sHtML

std::ofstream out("a.txt");  out << "hi\n";
来源：http://m.share.zdbjq.cn/Article/details/gfyoyameh.sHtML

[S50] C++：格式化数字
来源：http://www.m.share.fehbvm.com/Article/details/gqxuwlzcu.sHtML

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.share.fehbvm.com/Article/details/gozsnpkka.sHtML

[S51] C++：显式类型转换
来源：http://blog.zdbjq.cn/Article/details/glhucjvqe.sHtML

static_cast<double>(a) / b
来源：http://baike.fehbvm.com/Article/details/gqgxulcps.sHtML

[S52] C++：const 与 noexcept
来源：http://read.share.fehbvm.com/Article/details/gcczsvubb.sHtML

int size() const noexcept { return n_; }
来源：http://wap.fehbvm.com/Article/details/grbtplret.sHtML

[S53] C++：移动语义
来源：http://www.m.share.hesvh.cn/Article/details/gxnkagayv.sHtML

std::vector<int> w = std::move(v);
来源：http://www.m.share.zdbjq.cn/Article/details/ggwerhcoi.sHtML

[S54] C++：异常处理
来源：http://www.share.hesvh.cn/Article/details/gskpuyhli.sHtML

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wap.zdbjq.cn/Article/details/grhovzrtc.sHtML

[S55] C++：结构化绑定
来源：http://blog.zdbjq.cn/Article/details/gjluxupzj.sHtML

auto [a, b] = std::make_pair(1, 2);
来源：http://mobile.hesvh.cn/Article/details/gxovphuqi.sHtML

[S56] C++：optional
来源：http://www.m.share.zdbjq.cn/Article/details/gbspoeird.sHtML

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.blog.hesvh.cn/Article/details/gooxxnoqc.sHtML

[S57] C++：编译期常量
来源：http://www.m.share.hesvh.cn/Article/details/gkfsxyenh.sHtML

constexpr int N = 10;
来源：http://www.blog.fehbvm.com/Article/details/gfmxhvkfl.sHtML

[S58] C++：命名空间
来源：http://www.share.zdbjq.cn/Article/details/gfphgmykp.sHtML

namespace ns { int f() { return 1; } }
来源：http://m.share.zdbjq.cn/Article/details/guvztwvuh.sHtML

[S59] C++：静态断言
来源：http://www.blog.hesvh.cn/Article/details/gzhhfxkus.sHtML

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.share.hesvh.cn/Article/details/gqmckzsin.sHtML

[S60] C++：遍历并删除元素
来源：http://blog.hesvh.cn/Article/details/gkztogixs.sHtML

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wap.fehbvm.com/Article/details/gkwibtvzv.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/geatpated.sHtML

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://read.share.fehbvm.com/Article/details/gxeskaamk.sHtML

================================================================================
来源：http://www.share.zdbjq.cn/Article/details/gwvwcffdy.sHtML

[T01] Kotlin：Hello World
来源：http://3g.fehbvm.com/Article/details/gcsvkxqyi.sHtML

println("Hello")
来源：http://3g.hesvh.cn/Article/details/gkoodozmk.sHtML

[T02] Kotlin：变量
来源：http://3g.hesvh.cn/Article/details/ghnbujspa.sHtML

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mobile.hesvh.cn/Article/details/ggqiuhydf.sHtML

[T03] Kotlin：字符串模板
来源：http://baike.zdbjq.cn/Article/details/gyqjlwiyb.sHtML

"值: $b"
来源：http://blog.zdbjq.cn/Article/details/geiixcdna.sHtML

[T04] Kotlin：空安全
来源：http://wap.zdbjq.cn/Article/details/gbwbsuqbl.sHtML

val n: String? = null;  n?.length
来源：http://www.share.fehbvm.com/Article/details/gdfnwwydh.sHtML

[T05] Kotlin：when 表达式
来源：http://www.m.share.fehbvm.com/Article/details/gkoyaznaf.sHtML

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://blog.zdbjq.cn/Article/details/glqeardum.sHtML

[T06] Kotlin：集合映射
来源：http://3g.fehbvm.com/Article/details/gxydxwrom.sHtML

listOf(1, 2, 3).map { it * 2 }
来源：http://www.blog.zdbjq.cn/Article/details/gezykumhz.sHtML

[T07] Kotlin：集合过滤
来源：http://www.share.zdbjq.cn/Article/details/gpamrmgyp.sHtML

listOf(1, 2, 3).filter { it > 1 }
来源：http://read.share.zdbjq.cn/Article/details/gmehslxmd.sHtML

[T08] Kotlin：数据类
来源：http://www.m.share.fehbvm.com/Article/details/genaczeqg.sHtML

data class User(val name: String, val age: Int)
来源：http://3g.fehbvm.com/Article/details/gdhmxaftb.sHtML

[T09] Kotlin：扩展函数
来源：http://www.blog.hesvh.cn/Article/details/grwirpkpc.sHtML

fun String.exclaim() = this + "!"
来源：http://www.blog.zdbjq.cn/Article/details/gjvrrleky.sHtML

[T10] Kotlin：默认参数
来源：http://mobile.zdbjq.cn/Article/details/gpocyvjkl.sHtML

fun greet(name: String = "World") = "Hi $name"
来源：http://blog.hesvh.cn/Article/details/gjuolkntf.sHtML

[T11] Kotlin：协程
来源：http://www.share.zdbjq.cn/Article/details/gubncluod.sHtML

GlobalScope.launch { delay(1000); println("done") }
来源：http://wap.zdbjq.cn/Article/details/gsqavmhte.sHtML

[T12] Kotlin：解构声明
来源：http://m.share.zdbjq.cn/Article/details/grymzpllp.sHtML

val (a, b) = Pair(1, 2)
来源：http://www.m.share.fehbvm.com/Article/details/gktrckyqu.sHtML

[T13] Kotlin：只读 Map
来源：http://www.share.hesvh.cn/Article/details/gjldhanol.sHtML

val m = mapOf("a" to 1)
来源：http://mobile.hesvh.cn/Article/details/gpbjzrjkd.sHtML

[T14] Kotlin：循环
来源：http://mobile.zdbjq.cn/Article/details/gurahhwsx.sHtML

for (i in 1..10) println(i)
来源：http://baike.hesvh.cn/Article/details/gwbxlnxss.sHtML

[T15] Kotlin：接口
来源：http://blog.zdbjq.cn/Article/details/gewobpjrs.sHtML

interface Shape { fun area(): Double }
来源：http://www.blog.fehbvm.com/Article/details/gdziuqkpy.sHtML

[T16] Swift：Hello World
来源：http://www.share.hesvh.cn/Article/details/gbcbwkuar.sHtML

print("Hello")
来源：http://mobile.hesvh.cn/Article/details/gqndxtxbs.sHtML

[T17] Swift：变量与常量
来源：http://www.m.share.fehbvm.com/Article/details/gqrosnrbm.sHtML

var a = 1;  let b = 2
来源：http://wap.hesvh.cn/Article/details/gihdaytdp.sHtML

[T18] Swift：字符串插值
来源：http://www.m.share.hesvh.cn/Article/details/gmipujrcb.sHtML

"值: \(b)"
来源：http://www.m.share.fehbvm.com/Article/details/gyhgtfxdt.sHtML

[T19] Swift：可选绑定
来源：http://www.blog.zdbjq.cn/Article/details/gllonvhnj.sHtML

if let n = opt { print(n) }
来源：http://wap.hesvh.cn/Article/details/gmhanhcre.sHtML

[T20] Swift：数组操作
来源：http://m.share.zdbjq.cn/Article/details/ggydnecmh.sHtML

var a = [1, 2, 3];  a.append(4)
来源：http://m.share.hesvh.cn/Article/details/gsfmwmvjl.sHtML

[T21] Swift：遍历
来源：http://blog.zdbjq.cn/Article/details/gqyfxcfmj.sHtML

for x in a { print(x) }
来源：http://wap.hesvh.cn/Article/details/givvftkkh.sHtML

[T22] Swift：字典
来源：http://wap.fehbvm.com/Article/details/glgaczyjn.sHtML

var d = ["a": 1];  d["b"] = 2
来源：http://www.m.share.zdbjq.cn/Article/details/gngxqompp.sHtML

[T23] Swift：函数
来源：http://m.share.hesvh.cn/Article/details/gtibkxfrn.sHtML

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://read.share.zdbjq.cn/Article/details/gvxhradox.sHtML

[T24] Swift：闭包
来源：http://wap.fehbvm.com/Article/details/gynbafcrw.sHtML

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.share.zdbjq.cn/Article/details/govcsuvzj.sHtML

[T25] Swift：结构体
来源：http://www.blog.fehbvm.com/Article/details/gsjhfrkny.sHtML

struct P { var x: Int }
来源：http://www.share.hesvh.cn/Article/details/gflekmero.sHtML

[T26] Swift：类与重写
来源：http://blog.hesvh.cn/Article/details/gghfzppbw.sHtML

class A: Base { override func f() {} }
来源：http://blog.hesvh.cn/Article/details/gsfppcxfh.sHtML

[T27] Swift：错误处理
来源：http://mobile.fehbvm.com/Article/details/gwcycrkab.sHtML

do { try f() } catch { print(error) }
来源：http://read.share.zdbjq.cn/Article/details/gbzycktmb.sHtML

[T28] Swift：枚举
来源：http://wap.zdbjq.cn/Article/details/gvaauywdg.sHtML

enum Color { case red, green }
来源：http://wap.hesvh.cn/Article/details/geewcxxpm.sHtML

[T29] Swift：guard 提前返回
来源：http://blog.zdbjq.cn/Article/details/gcnhxcahy.sHtML

guard let x = opt else { return }
来源：http://www.m.share.zdbjq.cn/Article/details/gqtylpsuu.sHtML

[T30] Swift：协议
来源：http://blog.zdbjq.cn/Article/details/gzwydrhhr.sHtML

protocol Shape { func area() -> Double }
来源：http://www.share.zdbjq.cn/Article/details/ggsynsjyt.sHtML

[T31] Lua：Hello World
来源：http://read.share.hesvh.cn/Article/details/gtfitrono.sHtML

print("Hello")
来源：http://blog.hesvh.cn/Article/details/gunhkvdnx.sHtML

[T32] Lua：局部变量
来源：http://3g.fehbvm.com/Article/details/gzdqsfxuy.sHtML

local a = 1
来源：http://www.m.share.zdbjq.cn/Article/details/grckpaaao.sHtML

[T33] Lua：表（数组）
来源：http://www.share.hesvh.cn/Article/details/gocsesqar.sHtML

local t = {1, 2, 3};  t[4] = 4
来源：http://wap.hesvh.cn/Article/details/gnxfzbdzs.sHtML

[T34] Lua：遍历表
来源：http://read.share.fehbvm.com/Article/details/gczjcufil.sHtML

for i, v in ipairs(t) do print(i, v) end
来源：http://wap.zdbjq.cn/Article/details/gaimakbph.sHtML

[T35] Lua：字典表
来源：http://www.blog.zdbjq.cn/Article/details/gilgtjihb.sHtML

local d = { a = 1 };  d.b = 2
来源：http://blog.fehbvm.com/Article/details/gqcuxkgvf.sHtML

[T36] Lua：函数
来源：http://blog.zdbjq.cn/Article/details/gmkcnprjw.sHtML

function add(a, b) return a + b end
来源：http://blog.hesvh.cn/Article/details/gmpsqbera.sHtML

[T37] Lua：字符串拼接
来源：http://www.blog.fehbvm.com/Article/details/gvzosmpbu.sHtML

"a" .. "b"
来源：http://www.share.zdbjq.cn/Article/details/gjjsknjtb.sHtML

[T38] Lua：条件
来源：http://blog.fehbvm.com/Article/details/gmrvnvdtc.sHtML

if x > 0 then print("正") end
来源：http://read.share.hesvh.cn/Article/details/gdqpnkwxb.sHtML

[T39] Lua：模式匹配
来源：http://m.share.hesvh.cn/Article/details/gqxlflypu.sHtML

string.find(s, "%d+")
来源：http://www.m.share.hesvh.cn/Article/details/gxtybwmmb.sHtML

[T40] Lua：元表
来源：http://www.m.share.hesvh.cn/Article/details/gapnilfaz.sHtML

setmetatable({}, { __index = base })
来源：http://m.share.zdbjq.cn/Article/details/ghocrmniy.sHtML

[T41] Perl：Hello World
来源：http://www.m.share.zdbjq.cn/Article/details/gujjbytsh.sHtML

print "Hello\n";
来源：http://wap.zdbjq.cn/Article/details/gzxbvykzi.sHtML

[T42] Perl：变量类型
来源：http://m.share.fehbvm.com/Article/details/gyvbjwavf.sHtML

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://3g.fehbvm.com/Article/details/gwbnelwbb.sHtML

[T43] Perl：字符串插值
来源：http://www.m.share.fehbvm.com/Article/details/grgydfaap.sHtML

"值: $a"
来源：http://mobile.zdbjq.cn/Article/details/gpkgkhlhb.sHtML

[T44] Perl：条件
来源：http://www.blog.hesvh.cn/Article/details/gkupyczwb.sHtML

if ($a > 0) { print "正"; }
来源：http://www.share.zdbjq.cn/Article/details/ggconysux.sHtML

[T45] Perl：数组遍历
来源：http://m.share.hesvh.cn/Article/details/gjfpqzdyu.sHtML

for my $x (@arr) { print $x; }
来源：http://www.share.hesvh.cn/Article/details/gvmmlimna.sHtML

[T46] Perl：哈希操作
来源：http://m.share.hesvh.cn/Article/details/gsbrbudir.sHtML

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.m.share.zdbjq.cn/Article/details/gtopsghym.sHtML

[T47] Perl：正则捕获
来源：http://www.share.zdbjq.cn/Article/details/gmvoxvujb.sHtML

if ($s =~ /(\d+)/) { print $1; }
来源：http://blog.hesvh.cn/Article/details/gltorphuk.sHtML

[T48] Perl：正则替换
来源：http://www.m.share.hesvh.cn/Article/details/gubhgzdvl.sHtML

$s =~ s/old/new/g;
来源：http://mobile.hesvh.cn/Article/details/gtalyprzt.sHtML

[T49] Perl：函数
来源：http://mobile.zdbjq.cn/Article/details/ghmgtnvwt.sHtML

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://read.share.hesvh.cn/Article/details/gzxwvwmib.sHtML

[T50] Perl：逐行读文件
来源：http://read.share.zdbjq.cn/Article/details/gkhjqkdkv.sHtML

open my $fh, "<", "a.txt" or die $!;
来源：http://m.share.hesvh.cn/Article/details/gityrctlq.sHtML

while (my $line = <$fh>) { print $line; }
来源：http://m.share.fehbvm.com/Article/details/gjbstfcxv.sHtML

[T51] Scala：Hello World
来源：http://wap.fehbvm.com/Article/details/gbspvkuxx.sHtML

println("Hello")
来源：http://m.share.fehbvm.com/Article/details/gerwzmvcu.sHtML

[T52] Scala：变量
来源：http://m.share.zdbjq.cn/Article/details/gquddmdve.sHtML

val a = 1;  var b = 2
来源：http://read.share.hesvh.cn/Article/details/gesudorky.sHtML

[T53] Scala：字符串插值
来源：http://m.share.hesvh.cn/Article/details/gcbehjgza.sHtML

s"值: $b"
来源：http://m.share.fehbvm.com/Article/details/gxfxmypmp.sHtML

[T54] Scala：集合映射
来源：http://m.share.fehbvm.com/Article/details/gdpyatujw.sHtML

List(1, 2, 3).map(_ * 2)
来源：http://m.share.zdbjq.cn/Article/details/gyypjgkmq.sHtML

[T55] Scala：集合过滤
来源：http://m.share.zdbjq.cn/Article/details/gkzsjzgdl.sHtML

List(1, 2, 3).filter(_ > 1)
来源：http://m.share.hesvh.cn/Article/details/gioxfmajy.sHtML

[T56] Scala：样例类
来源：http://www.m.share.hesvh.cn/Article/details/ggxprcbut.sHtML

case class User(name: String, age: Int)
来源：http://3g.hesvh.cn/Article/details/gehvwvhok.sHtML

[T57] Scala：模式匹配
来源：http://3g.zdbjq.cn/Article/details/grxhkoyws.sHtML

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.m.share.fehbvm.com/Article/details/gaiuayvgn.sHtML

[T58] Scala：函数定义
来源：http://www.share.zdbjq.cn/Article/details/gupvmaura.sHtML

def add(a: Int, b: Int): Int = a + b
来源：http://3g.hesvh.cn/Article/details/gdpdchjos.sHtML

[T59] Scala：循环
来源：http://blog.hesvh.cn/Article/details/ghnakyrox.sHtML

for (i <- 1 to 10) println(i)
来源：http://mobile.zdbjq.cn/Article/details/ghuudmovo.sHtML

[T60] Scala：折叠
来源：http://read.share.fehbvm.com/Article/details/ghldqzdja.sHtML

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://read.share.zdbjq.cn/Article/details/gvczdjppu.sHtML

================================================================================
来源：http://blog.fehbvm.com/Article/details/gvhywwysi.sHtML

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://3g.fehbvm.com/Article/details/glmiqdssu.sHtML

================================================================================
来源：http://baike.fehbvm.com/Article/details/gxdqnpxga.sHtML

[U01] Py：创建虚拟环境
来源：http://www.share.zdbjq.cn/Article/details/gufkhplld.sHtML

python -m venv .venv && source .venv/bin/activate
来源：http://wap.fehbvm.com/Article/details/gxtvmifgp.sHtML

[U02] Py：导出 / 安装依赖
来源：http://m.share.fehbvm.com/Article/details/gnnwakxad.sHtML

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://m.share.zdbjq.cn/Article/details/gjqccesmy.sHtML


<!-- 参考信息 -->