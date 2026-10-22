代发 wailian999

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt2wrppcrdb.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt2lsdojcnh.html

du -ah . | sort -rh | head -10
来源：http://www.ydjk.org.cn/Article/details/gt2vfzbzjnx.html

[R63] 内存与进程
来源：http://www.52xcode.cn/Article/details/gt2pttwpdxm.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt2iimgyvhk.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt2tagfbmwm.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt2kodtjbkw.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt2qdgkahso.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.52xcode.cn/Article/details/gt2qnadzwlp.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt2ddrcluxx.html

crontab -e;  crontab -l
来源：http://www.ydjk.org.cn/Article/details/gt2zmbmuojc.html

[R67] 生成随机十六进制串
来源：http://www.ydjk.org.cn/Article/details/gt2zdzljbjs.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt2tzuwmwfl.html

[R68] 计算文件校验值
来源：http://www.52xcode.cn/Article/details/gt2flvyjsyl.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt2qgyphbjk.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt2xxfdyqfb.html

head -c 16 /dev/urandom | base64
来源：http://www.52xcode.cn/Article/details/gt2qyiggiqh.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt2lgkxzbsh.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt2vdhekfex.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt2dnsklxud.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.52xcode.cn/Article/details/gt2xnaseaqt.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt2xvntctpk.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.ydjk.org.cn/Article/details/gt2cdgjvlee.html

[R73] 分割大日志
来源：http://www.ydjk.org.cn/Article/details/gt2rdxnprrh.html

split -l 1000 big.log part_
来源：http://www.52xcode.cn/Article/details/gt2lhvedbyz.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt2uosismuq.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.52xcode.cn/Article/details/gt2rslmmefa.html

[R75] 导出环境变量
来源：http://www.ydjk.org.cn/Article/details/gt2hcinxlid.html

export PATH="$HOME/bin:$PATH"
来源：http://www.52xcode.cn/Article/details/gt2utwpawqo.html

[R76] 使用临时文件
来源：http://www.52xcode.cn/Article/details/gt2mlylxniv.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt2luqbdqpj.html

[R77] 读取用户输入
来源：http://www.ydjk.org.cn/Article/details/gt2mbotufog.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt2zknjoorr.html

[R78] 交互式菜单
来源：http://www.ydjk.org.cn/Article/details/gt2wgpesnid.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt2cpvyoiue.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt2jermfimo.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.52xcode.cn/Article/details/gt2sezbssra.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt2panlhops.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt2truczjcf.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2hmlubxhq.html

S. C / C++ 专题
来源：http://www.ydjk.org.cn/Article/details/gt2ysrucprm.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2iaawecur.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt2lrsmdcaf.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt2hipxdfon.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.ydjk.org.cn/Article/details/gt2vavphqjc.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt2uxxsprpx.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt2xqmnztqo.html

[S03] C：读入整数
来源：http://www.52xcode.cn/Article/details/gt2aegtvavu.html

int x; scanf("%d", &x);
来源：http://www.ydjk.org.cn/Article/details/gt2pxjbskhu.html

[S04] C：字符串复制
来源：http://www.ydjk.org.cn/Article/details/gt2ornnkkxo.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt2drgufput.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt2gokwecro.html

strlen(s)
来源：http://www.52xcode.cn/Article/details/gt2pfbzoycs.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt2yzigxeam.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt2nfnuzfov.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt2cqpcmswp.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt2ytjcrsnt.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt2ykeicbos.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt2bncfbort.html

[S09] C：结构体定义与初始化
来源：http://www.52xcode.cn/Article/details/gt2jtjgeatz.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt2zncxfedt.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt2xrfvgkif.html

int *p = &a;  *p = 5;
来源：http://www.52xcode.cn/Article/details/gt2gywtjucv.html

[S11] C：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2aeeoabev.html

FILE *f = fopen("a.txt", "r");
来源：http://www.ydjk.org.cn/Article/details/gt2hsxastxu.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2pngnzdim.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt2kzlcdobe.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt2jtrsymmj.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt2crbjgsus.html

[S13] C：宏定义
来源：http://www.52xcode.cn/Article/details/gt2pvulokbr.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt2rwcpotdo.html

[S14] C：枚举
来源：http://www.52xcode.cn/Article/details/gt2vhnoyfuw.html

enum Color { RED, GREEN, BLUE };
来源：http://www.ydjk.org.cn/Article/details/gt2nfgrakhi.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt2xpixxnxx.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt2vurdzfrz.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt2jsuxlvwn.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt2dmjoejdp.html

[S17] C：安全拼接字符串
来源：http://www.ydjk.org.cn/Article/details/gt2xqnxpeqx.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.52xcode.cn/Article/details/gt2hpulldcx.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt2uasqkhhj.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt2rxinmhfe.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt2nwnjllyp.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.ydjk.org.cn/Article/details/gt2gieqwpie.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt2outsskoc.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt2cfgejxlm.html

[S21] C：字符类别判断
来源：http://www.ydjk.org.cn/Article/details/gt2aufpuhfw.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.52xcode.cn/Article/details/gt2lwlxeljf.html

[S22] C：字符串转数字
来源：http://www.ydjk.org.cn/Article/details/gt2wzzgnjlq.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.52xcode.cn/Article/details/gt2oaetaxjc.html

[S23] C：随机数
来源：http://www.52xcode.cn/Article/details/gt2nqyagflm.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt2knhhvikz.html

[S24] C：获取本地时间
来源：http://www.52xcode.cn/Article/details/gt2nevxomuc.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.52xcode.cn/Article/details/gt2ktfmhwfv.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt2lltylpml.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt2ivpkagly.html

[S26] C：内存清零
来源：http://www.52xcode.cn/Article/details/gt2loxdkpgm.html

memset(a, 0, sizeof a);
来源：http://www.ydjk.org.cn/Article/details/gt2cgynybnm.html

[S27] C：定义常量
来源：http://www.52xcode.cn/Article/details/gt2dxkevsus.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2bhnopkci.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt2xvwuclnx.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt2kfivtasy.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt2zwwnifct.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.52xcode.cn/Article/details/gt2lukjsxex.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt2ucbntxja.html

#ifndef X_H
来源：http://www.ydjk.org.cn/Article/details/gt2qkyyhgux.html

#define X_H
来源：http://www.ydjk.org.cn/Article/details/gt2dcgqxech.html

#endif
来源：http://www.52xcode.cn/Article/details/gt2ojdulfxz.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2hlffmbzs.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt2oxrhkefy.html

int main() { std::cout << "Hello\n"; }
来源：http://www.52xcode.cn/Article/details/gt2pjuuzibq.html

[S32] C++：字符串
来源：http://www.ydjk.org.cn/Article/details/gt2ljokzgjy.html

std::string s = "hi";  s += "!";
来源：http://www.ydjk.org.cn/Article/details/gt2lxofhrox.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt2sgngixkq.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.52xcode.cn/Article/details/gt2qyjztxkz.html

[S34] C++：遍历 vector
来源：http://www.52xcode.cn/Article/details/gt2sxspfqls.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt2kkzpejin.html

[S35] C++：map
来源：http://www.52xcode.cn/Article/details/gt2myevizim.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2ngsjcsdd.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt2kcbtbgdq.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt2hbagtoiy.html

[S37] C++：set
来源：http://www.52xcode.cn/Article/details/gt2vorowrnp.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt2ghlncjbz.html

[S38] C++：排序
来源：http://www.ydjk.org.cn/Article/details/gt2kkjamlbs.html

std::sort(v.begin(), v.end());
来源：http://www.52xcode.cn/Article/details/gt2nbobcfve.html

[S39] C++：自定义比较器排序
来源：http://www.52xcode.cn/Article/details/gt2qvpkmgdh.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt2pbaltxwr.html

[S40] C++：查找元素
来源：http://www.ydjk.org.cn/Article/details/gt2dmrbodyg.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt2kmdirhrs.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt2rgtpbfsp.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.ydjk.org.cn/Article/details/gt2anzxvjgu.html

[S42] C++：继承与虚函数
来源：http://www.ydjk.org.cn/Article/details/gt2xzhzhmhj.html

class B : public Base { public: void f() override {} };
来源：http://www.52xcode.cn/Article/details/gt2zkngbvbs.html

[S43] C++：智能指针
来源：http://www.52xcode.cn/Article/details/gt2foonohmt.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt2erdxxeoo.html

[S44] C++：引用传参
来源：http://www.ydjk.org.cn/Article/details/gt2jgxmbowl.html

void inc(int &x) { ++x; }
来源：http://www.ydjk.org.cn/Article/details/gt2zlnvlbcz.html

[S45] C++：lambda
来源：http://www.ydjk.org.cn/Article/details/gt2dynuicgn.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.52xcode.cn/Article/details/gt2kmnbzsak.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt2eepuxrrw.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt2kbimlmnm.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt2zbzzeuld.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt2gxcjtcgc.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt2jvauxjax.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.52xcode.cn/Article/details/gt2wslkjyld.html

while (std::getline(in, line)) { }
来源：http://www.ydjk.org.cn/Article/details/gt2afggwpxh.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt2oavpgiyq.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.52xcode.cn/Article/details/gt2xmqspkvf.html

[S50] C++：格式化数字
来源：http://www.ydjk.org.cn/Article/details/gt2dafzkxko.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt2nmbsgono.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt2uprtlvry.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt2fysrvklp.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt2copiqqzk.html

int size() const noexcept { return n_; }
来源：http://www.52xcode.cn/Article/details/gt2pzfiqjve.html

[S53] C++：移动语义
来源：http://www.ydjk.org.cn/Article/details/gt2pyssteaj.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt2uursyvwr.html

[S54] C++：异常处理
来源：http://www.52xcode.cn/Article/details/gt2ukshbxer.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.ydjk.org.cn/Article/details/gt2axrmnlws.html

[S55] C++：结构化绑定
来源：http://www.52xcode.cn/Article/details/gt2seisbacr.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.ydjk.org.cn/Article/details/gt2dsrehvrn.html

[S56] C++：optional
来源：http://www.ydjk.org.cn/Article/details/gt2ebvuktle.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.52xcode.cn/Article/details/gt2eysqcivm.html

[S57] C++：编译期常量
来源：http://www.52xcode.cn/Article/details/gt2dlynkktv.html

constexpr int N = 10;
来源：http://www.52xcode.cn/Article/details/gt2jvdvpemu.html

[S58] C++：命名空间
来源：http://www.52xcode.cn/Article/details/gt2uqtcptyh.html

namespace ns { int f() { return 1; } }
来源：http://www.ydjk.org.cn/Article/details/gt2dvrrobhx.html

[S59] C++：静态断言
来源：http://www.52xcode.cn/Article/details/gt2eluvgkyf.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.ydjk.org.cn/Article/details/gt2yktqswaw.html

[S60] C++：遍历并删除元素
来源：http://www.ydjk.org.cn/Article/details/gt2khtgrwfc.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.52xcode.cn/Article/details/gt2emqvmniu.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2pnauysdh.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt2cepaieno.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt2ohajisph.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt2ddpmefvt.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2yaojycfb.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt2hkgrvciy.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.ydjk.org.cn/Article/details/gt2twtbdxvg.html

[T03] Kotlin：字符串模板
来源：http://www.ydjk.org.cn/Article/details/gt2obyctpmf.html

"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2efarafhn.html

[T04] Kotlin：空安全
来源：http://www.52xcode.cn/Article/details/gt2jhfxzmjc.html

val n: String? = null;  n?.length
来源：http://www.ydjk.org.cn/Article/details/gt2gawnloje.html

[T05] Kotlin：when 表达式
来源：http://www.52xcode.cn/Article/details/gt2utmkuupq.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.ydjk.org.cn/Article/details/gt2xkippbvh.html

[T06] Kotlin：集合映射
来源：http://www.52xcode.cn/Article/details/gt2tdutstua.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt2zhldohol.html

[T07] Kotlin：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2ipvczmsl.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt2hcniumfc.html

[T08] Kotlin：数据类
来源：http://www.ydjk.org.cn/Article/details/gt2udtpdrie.html

data class User(val name: String, val age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt2vauaawav.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt2vcrupyqg.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt2djwuyopj.html

[T10] Kotlin：默认参数
来源：http://www.52xcode.cn/Article/details/gt2rjlypfri.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.ydjk.org.cn/Article/details/gt2wrozeboe.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt2qnlhozug.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt2hoxptmds.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt2sbvfqvuj.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt2rcyrwdjy.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt2npyzdcqn.html

val m = mapOf("a" to 1)
来源：http://www.52xcode.cn/Article/details/gt2eaurtdct.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt2hontvqzi.html

for (i in 1..10) println(i)
来源：http://www.ydjk.org.cn/Article/details/gt2bmwlkttl.html

[T15] Kotlin：接口
来源：http://www.ydjk.org.cn/Article/details/gt2fdzmozgv.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt2ajiwyrzf.html

[T16] Swift：Hello World
来源：http://www.52xcode.cn/Article/details/gt2zwmwcbjo.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt2eifnzhwj.html

[T17] Swift：变量与常量
来源：http://www.52xcode.cn/Article/details/gt2nqqhlvig.html

var a = 1;  let b = 2
来源：http://www.ydjk.org.cn/Article/details/gt2ehioclek.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2ktjzqyej.html

"值: \(b)"
来源：http://www.ydjk.org.cn/Article/details/gt2tdifjxhs.html

[T19] Swift：可选绑定
来源：http://www.52xcode.cn/Article/details/gt2wnpijbzt.html

if let n = opt { print(n) }
来源：http://www.ydjk.org.cn/Article/details/gt2bqlwpugw.html

[T20] Swift：数组操作
来源：http://www.ydjk.org.cn/Article/details/gt2vpsiamvy.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt2fvjpkzfe.html

[T21] Swift：遍历
来源：http://www.ydjk.org.cn/Article/details/gt2gkfldrmy.html

for x in a { print(x) }
来源：http://www.ydjk.org.cn/Article/details/gt2kstwugpp.html

[T22] Swift：字典
来源：http://www.52xcode.cn/Article/details/gt2zlvchopj.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.52xcode.cn/Article/details/gt2lwlygnse.html

[T23] Swift：函数
来源：http://www.52xcode.cn/Article/details/gt2sfhvtkbc.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt2rwxpofke.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt2rqpkodsx.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.52xcode.cn/Article/details/gt2oqztkppt.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt2lnkvgvod.html

struct P { var x: Int }
来源：http://www.ydjk.org.cn/Article/details/gt2dndzlnew.html

[T26] Swift：类与重写
来源：http://www.ydjk.org.cn/Article/details/gt2qghmzbns.html

class A: Base { override func f() {} }
来源：http://www.52xcode.cn/Article/details/gt2hcrcakvc.html

[T27] Swift：错误处理
来源：http://www.52xcode.cn/Article/details/gt2hlfafjjr.html

do { try f() } catch { print(error) }
来源：http://www.ydjk.org.cn/Article/details/gt2uvkluodh.html

[T28] Swift：枚举
来源：http://www.ydjk.org.cn/Article/details/gt2gugtrdpe.html

enum Color { case red, green }
来源：http://www.52xcode.cn/Article/details/gt2uqaiyefu.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt2uopvsren.html

guard let x = opt else { return }
来源：http://www.ydjk.org.cn/Article/details/gt2vcrxfvuh.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt2vlszixmr.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt2umerrrcv.html

[T31] Lua：Hello World
来源：http://www.52xcode.cn/Article/details/gt2llnjpgbp.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt2qagjojji.html

[T32] Lua：局部变量
来源：http://www.52xcode.cn/Article/details/gt2muvpbbpj.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt2niaepcwv.html

[T33] Lua：表（数组）
来源：http://www.ydjk.org.cn/Article/details/gt2bxaymcmx.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt2rypecrkg.html

[T34] Lua：遍历表
来源：http://www.ydjk.org.cn/Article/details/gt2sbtrhyxd.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt2vapldmdd.html

[T35] Lua：字典表
来源：http://www.52xcode.cn/Article/details/gt2eyljqwac.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt2glmesnsh.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt2hsftvzfa.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt2lgbpvobl.html

[T37] Lua：字符串拼接
来源：http://www.52xcode.cn/Article/details/gt2uqqpgvkd.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt2ywovzmzc.html

[T38] Lua：条件
来源：http://www.ydjk.org.cn/Article/details/gt2fdbocblk.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt2nfehdyfh.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2coszouzo.html

string.find(s, "%d+")
来源：http://www.52xcode.cn/Article/details/gt2mlemoeie.html

[T40] Lua：元表
来源：http://www.52xcode.cn/Article/details/gt2unftrhen.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt2jdctlsnv.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2aovnsdzp.html

print "Hello\n";
来源：http://www.52xcode.cn/Article/details/gt2zfqduyzz.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt2kfcjofzx.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.52xcode.cn/Article/details/gt2nouludjs.html

[T43] Perl：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt2pqwmfjzf.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt2vgxcipns.html

[T44] Perl：条件
来源：http://www.ydjk.org.cn/Article/details/gt2swjeacyv.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt2vdsbvirj.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt2xyozsgkp.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt2anpzlgst.html

[T46] Perl：哈希操作
来源：http://www.ydjk.org.cn/Article/details/gt2bvbuiyji.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.ydjk.org.cn/Article/details/gt2hybitexx.html

[T47] Perl：正则捕获
来源：http://www.ydjk.org.cn/Article/details/gt2hwxxrpog.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.ydjk.org.cn/Article/details/gt2njhyujcm.html

[T48] Perl：正则替换
来源：http://www.ydjk.org.cn/Article/details/gt2wwvhvykd.html

$s =~ s/old/new/g;
来源：http://www.ydjk.org.cn/Article/details/gt2equdiuse.html

[T49] Perl：函数
来源：http://www.52xcode.cn/Article/details/gt2pnbyxfhl.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt2nciqbzdi.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt2ksldiuue.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt2wjpwosgm.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt2pjkmlnqe.html

[T51] Scala：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt2zoziegaw.html

println("Hello")
来源：http://www.52xcode.cn/Article/details/gt2mdjkgnkl.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt2cijpbbqw.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt2izkodyva.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt2kovhqnci.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt2sukynfcq.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt2zjwpwgdy.html

List(1, 2, 3).map(_ * 2)
来源：http://www.52xcode.cn/Article/details/gt2qlkyqtuu.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt2bobzotgv.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.ydjk.org.cn/Article/details/gt2jdljcuub.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt2wraqgpwr.html

case class User(name: String, age: Int)
来源：http://www.52xcode.cn/Article/details/gt2mqwdjbol.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt2mttcnllw.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.52xcode.cn/Article/details/gt2plzoqwet.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt2fuckubnb.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.ydjk.org.cn/Article/details/gt2ghheyhkg.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt2swierxcb.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt2cyptgynd.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt2sxlnicji.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt2pqodsmbk.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2sejwravf.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.52xcode.cn/Article/details/gt2fipmyhut.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt2yexvcjdz.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt2fpqpygft.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.52xcode.cn/Article/details/gt2rwcklyuj.html

[U02] Py：导出 / 安装依赖
来源：http://www.52xcode.cn/Article/details/gt2tztbjitw.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt2dfejkjln.html


<!-- 参考信息 -->