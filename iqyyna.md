代发 wailian999

df -h;  du -sh *
来源：http://www.ydjk.org.cn/Article/details/gt3aboayrwv.html

[R62] 找最占空间的文件
来源：http://www.52xcode.cn/Article/details/gt3hhmmgtdf.html

du -ah . | sort -rh | head -10
来源：http://www.52xcode.cn/Article/details/gt3pmmxsrxd.html

[R63] 内存与进程
来源：http://www.ydjk.org.cn/Article/details/gt3gwrowcmc.html

free -h;  ps aux | grep nginx
来源：http://www.52xcode.cn/Article/details/gt3nlslunjx.html

[R64] 结束进程
来源：http://www.52xcode.cn/Article/details/gt3rnvdjovn.html

kill -9 $(pgrep -f app.py)
来源：http://www.52xcode.cn/Article/details/gt3eccmmrik.html

[R65] 查看端口占用
来源：http://www.52xcode.cn/Article/details/gt3dnvqqkph.html

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://www.ydjk.org.cn/Article/details/gt3zhttupfk.html

[R66] 定时任务
来源：http://www.ydjk.org.cn/Article/details/gt3ccjazazw.html

crontab -e;  crontab -l
来源：http://www.52xcode.cn/Article/details/gt3solkfzpz.html

[R67] 生成随机十六进制串
来源：http://www.52xcode.cn/Article/details/gt3stipaqgs.html

openssl rand -hex 16
来源：http://www.ydjk.org.cn/Article/details/gt3txxoocjs.html

[R68] 计算文件校验值
来源：http://www.ydjk.org.cn/Article/details/gt3yooupjjm.html

sha256sum a.txt;  md5sum a.txt
来源：http://www.ydjk.org.cn/Article/details/gt3evleodou.html

[R69] 生成随机密码
来源：http://www.ydjk.org.cn/Article/details/gt3ppdeecxs.html

head -c 16 /dev/urandom | base64
来源：http://www.ydjk.org.cn/Article/details/gt3suieoqeo.html

[R70] 时间戳与互转
来源：http://www.52xcode.cn/Article/details/gt3ofswwyhv.html

date +%s;  date -d @1700000000
来源：http://www.ydjk.org.cn/Article/details/gt3nximqclu.html

[R71] 日期格式化
来源：http://www.52xcode.cn/Article/details/gt3alhkamdt.html

date +"%Y-%m-%d %H:%M:%S"
来源：http://www.ydjk.org.cn/Article/details/gt3bqakbeft.html

[R72] 等待端口就绪
来源：http://www.52xcode.cn/Article/details/gt3rglvsexc.html

until nc -z localhost 3306; do sleep 1; done
来源：http://www.52xcode.cn/Article/details/gt3eazfhkpk.html

[R73] 分割大日志
来源：http://www.52xcode.cn/Article/details/gt3dakzyuju.html

split -l 1000 big.log part_
来源：http://www.ydjk.org.cn/Article/details/gt3oywtsafl.html

[R74] 批量重命名
来源：http://www.ydjk.org.cn/Article/details/gt3dvgmdnvc.html

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://www.ydjk.org.cn/Article/details/gt3dwlteqgr.html

[R75] 导出环境变量
来源：http://www.52xcode.cn/Article/details/gt3omdahbrf.html

export PATH="$HOME/bin:$PATH"
来源：http://www.ydjk.org.cn/Article/details/gt3jvwwqdir.html

[R76] 使用临时文件
来源：http://www.ydjk.org.cn/Article/details/gt3usrnktqq.html

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://www.ydjk.org.cn/Article/details/gt3gfpghndr.html

[R77] 读取用户输入
来源：http://www.52xcode.cn/Article/details/gt3gspriwxe.html

read -rp "请输入: " ans
来源：http://www.52xcode.cn/Article/details/gt3lwzfctjf.html

[R78] 交互式菜单
来源：http://www.52xcode.cn/Article/details/gt3mjntsbyt.html

select opt in a b c; do echo "$opt"; break; done
来源：http://www.ydjk.org.cn/Article/details/gt3pkzmmajf.html

[R79] 解析命令行选项
来源：http://www.52xcode.cn/Article/details/gt3exefdnfv.html

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://www.ydjk.org.cn/Article/details/gt3qljjprnw.html

[R80] 查看脚本执行耗时
来源：http://www.ydjk.org.cn/Article/details/gt3hcfdsxmc.html

time ./run.sh
来源：http://www.52xcode.cn/Article/details/gt3uwfiowai.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3xsezrekw.html

S. C / C++ 专题
来源：http://www.52xcode.cn/Article/details/gt3nwylxidd.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3ifqfghoz.html

[S01] C：Hello World
来源：http://www.52xcode.cn/Article/details/gt3velqhunu.html

#include <stdio.h>
来源：http://www.ydjk.org.cn/Article/details/gt3dkbvnsnq.html

int main(void) { printf("Hello\n"); return 0; }
来源：http://www.52xcode.cn/Article/details/gt3qvilbmui.html

[S02] C：变量与格式化输出
来源：http://www.ydjk.org.cn/Article/details/gt3nkqkupro.html

int a = 10; printf("%d\n", a);
来源：http://www.52xcode.cn/Article/details/gt3vjrvgpef.html

[S03] C：读入整数
来源：http://www.ydjk.org.cn/Article/details/gt3vcjexahu.html

int x; scanf("%d", &x);
来源：http://www.52xcode.cn/Article/details/gt3ahbirggk.html

[S04] C：字符串复制
来源：http://www.52xcode.cn/Article/details/gt3ozboeckb.html

char dst[32]; strcpy(dst, "hi");
来源：http://www.52xcode.cn/Article/details/gt3hynnmcgy.html

[S05] C：字符串长度
来源：http://www.ydjk.org.cn/Article/details/gt3oifmeatv.html

strlen(s)
来源：http://www.ydjk.org.cn/Article/details/gt3lndejzyb.html

[S06] C：字符串比较
来源：http://www.52xcode.cn/Article/details/gt3cfzsltnc.html

strcmp(a, b) == 0
来源：http://www.52xcode.cn/Article/details/gt3englygmy.html

[S07] C：数组遍历求和
来源：http://www.52xcode.cn/Article/details/gt3pmnqwqtg.html

for (int i = 0; i < n; i++) sum += a[i];
来源：http://www.ydjk.org.cn/Article/details/gt3ggulavlw.html

[S08] C：动态内存分配与释放
来源：http://www.ydjk.org.cn/Article/details/gt3ezdblrrd.html

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://www.ydjk.org.cn/Article/details/gt3gvodmrcl.html

[S09] C：结构体定义与初始化
来源：http://www.ydjk.org.cn/Article/details/gt3wgurvqyh.html

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://www.52xcode.cn/Article/details/gt3pkzipbog.html

[S10] C：指针与解引用
来源：http://www.52xcode.cn/Article/details/gt3cswexnjo.html

int *p = &a;  *p = 5;
来源：http://www.ydjk.org.cn/Article/details/gt3miwwnxxg.html

[S11] C：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3hsnfgdws.html

FILE *f = fopen("a.txt", "r");
来源：http://www.52xcode.cn/Article/details/gt3gstxgbdj.html

while (fgets(buf, sizeof buf, f)) { }
来源：http://www.ydjk.org.cn/Article/details/gt3sbpcknfe.html

fclose(f);
来源：http://www.52xcode.cn/Article/details/gt3tifiipub.html

[S12] C：写文件
来源：http://www.ydjk.org.cn/Article/details/gt3ujwoncqs.html

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://www.ydjk.org.cn/Article/details/gt3xizapvgy.html

[S13] C：宏定义
来源：http://www.ydjk.org.cn/Article/details/gt3uvozwjjs.html

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://www.52xcode.cn/Article/details/gt3cdlhdjgh.html

[S14] C：枚举
来源：http://www.ydjk.org.cn/Article/details/gt3bxugjmiv.html

enum Color { RED, GREEN, BLUE };
来源：http://www.52xcode.cn/Article/details/gt3nfihofwt.html

[S15] C：类型转换
来源：http://www.52xcode.cn/Article/details/gt3lllkeced.html

(double) a / b
来源：http://www.ydjk.org.cn/Article/details/gt3cbcgknsy.html

[S16] C：位操作置位
来源：http://www.52xcode.cn/Article/details/gt3cgkybftf.html

x |= (1 << 3);
来源：http://www.ydjk.org.cn/Article/details/gt3mwjfvacq.html

[S17] C：安全拼接字符串
来源：http://www.52xcode.cn/Article/details/gt3kurnwskt.html

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://www.ydjk.org.cn/Article/details/gt3gmtvajuh.html

[S18] C：命令行参数
来源：http://www.52xcode.cn/Article/details/gt3hlhodxxt.html

int main(int argc, char **argv)
来源：http://www.52xcode.cn/Article/details/gt3qzjruyqa.html

[S19] C：快速排序
来源：http://www.ydjk.org.cn/Article/details/gt3lzhklrlz.html

qsort(a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3gcxugioq.html

[S20] C：二分查找
来源：http://www.ydjk.org.cn/Article/details/gt3nnkrxtzu.html

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://www.52xcode.cn/Article/details/gt3zvunbjaq.html

[S21] C：字符类别判断
来源：http://www.52xcode.cn/Article/details/gt3alkgobqp.html

isdigit(c);  isalpha(c);  isspace(c);
来源：http://www.ydjk.org.cn/Article/details/gt3arorufrs.html

[S22] C：字符串转数字
来源：http://www.52xcode.cn/Article/details/gt3yqgjllvo.html

atoi("42");  strtod("3.14", NULL);
来源：http://www.ydjk.org.cn/Article/details/gt3dvlimvsx.html

[S23] C：随机数
来源：http://www.ydjk.org.cn/Article/details/gt3lhcetgrn.html

srand(time(NULL));  int r = rand() % 100;
来源：http://www.ydjk.org.cn/Article/details/gt3rcctvoct.html

[S24] C：获取本地时间
来源：http://www.ydjk.org.cn/Article/details/gt3omvtohml.html

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://www.ydjk.org.cn/Article/details/gt3vbctpndy.html

[S25] C：内存拷贝
来源：http://www.ydjk.org.cn/Article/details/gt3tmdvznin.html

memcpy(dst, src, n);
来源：http://www.ydjk.org.cn/Article/details/gt3wxrwxixf.html

[S26] C：内存清零
来源：http://www.ydjk.org.cn/Article/details/gt3imaumrjy.html

memset(a, 0, sizeof a);
来源：http://www.52xcode.cn/Article/details/gt3pxuabxlx.html

[S27] C：定义常量
来源：http://www.ydjk.org.cn/Article/details/gt3zdlahyod.html

const double PI = 3.14159;
来源：http://www.ydjk.org.cn/Article/details/gt3kzxblglb.html

[S28] C：静态变量
来源：http://www.52xcode.cn/Article/details/gt3inptvaqm.html

static int counter = 0;
来源：http://www.ydjk.org.cn/Article/details/gt3vdlvwkke.html

[S29] C：变参函数
来源：http://www.52xcode.cn/Article/details/gt3johwhsoz.html

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://www.ydjk.org.cn/Article/details/gt3qdtfplzk.html

[S30] C：头文件保护
来源：http://www.ydjk.org.cn/Article/details/gt3ftizvfvg.html

#ifndef X_H
来源：http://www.52xcode.cn/Article/details/gt3blekedtk.html

#define X_H
来源：http://www.52xcode.cn/Article/details/gt3ltvoruql.html

#endif
来源：http://www.52xcode.cn/Article/details/gt3bqegbdih.html

[S31] C++：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3gcmkcetn.html

#include <iostream>
来源：http://www.52xcode.cn/Article/details/gt3vuvdpdqn.html

int main() { std::cout << "Hello\n"; }
来源：http://www.ydjk.org.cn/Article/details/gt3oxlnepor.html

[S32] C++：字符串
来源：http://www.52xcode.cn/Article/details/gt3kmfjaiyi.html

std::string s = "hi";  s += "!";
来源：http://www.52xcode.cn/Article/details/gt3wskkxzqy.html

[S33] C++：vector 增删
来源：http://www.52xcode.cn/Article/details/gt3zlhvjseg.html

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://www.ydjk.org.cn/Article/details/gt3qzxkmkns.html

[S34] C++：遍历 vector
来源：http://www.ydjk.org.cn/Article/details/gt3jamxfxlr.html

for (auto &x : v) { std::cout << x; }
来源：http://www.ydjk.org.cn/Article/details/gt3uzumkqeb.html

[S35] C++：map
来源：http://www.ydjk.org.cn/Article/details/gt3kzlrqcem.html

std::map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3kdjwrtjd.html

[S36] C++：unordered_map
来源：http://www.ydjk.org.cn/Article/details/gt3zitoqdij.html

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://www.ydjk.org.cn/Article/details/gt3rzwtjyht.html

[S37] C++：set
来源：http://www.ydjk.org.cn/Article/details/gt3icblmqep.html

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://www.52xcode.cn/Article/details/gt3lcmfdduk.html

[S38] C++：排序
来源：http://www.52xcode.cn/Article/details/gt3wffdotqc.html

std::sort(v.begin(), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3kmkxliso.html

[S39] C++：自定义比较器排序
来源：http://www.ydjk.org.cn/Article/details/gt3kjtgbupg.html

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://www.52xcode.cn/Article/details/gt3dpunhtmk.html

[S40] C++：查找元素
来源：http://www.52xcode.cn/Article/details/gt3jdmynymw.html

auto it = std::find(v.begin(), v.end(), 3);
来源：http://www.52xcode.cn/Article/details/gt3qugiuixd.html

[S41] C++：类与构造函数
来源：http://www.ydjk.org.cn/Article/details/gt3vgglybqp.html

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://www.52xcode.cn/Article/details/gt3cgkydthh.html

[S42] C++：继承与虚函数
来源：http://www.52xcode.cn/Article/details/gt3epfetzga.html

class B : public Base { public: void f() override {} };
来源：http://www.ydjk.org.cn/Article/details/gt3cfdpvavd.html

[S43] C++：智能指针
来源：http://www.ydjk.org.cn/Article/details/gt3ovximjtf.html

auto p = std::make_unique<int>(5);
来源：http://www.52xcode.cn/Article/details/gt3vxozihco.html

[S44] C++：引用传参
来源：http://www.52xcode.cn/Article/details/gt3ueijtemv.html

void inc(int &x) { ++x; }
来源：http://www.52xcode.cn/Article/details/gt3bllvvwlx.html

[S45] C++：lambda
来源：http://www.52xcode.cn/Article/details/gt3dndwuccw.html

auto add = [](int a, int b) { return a + b; };
来源：http://www.ydjk.org.cn/Article/details/gt3mggtzzls.html

[S46] C++：函数模板
来源：http://www.ydjk.org.cn/Article/details/gt3kzsuguks.html

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://www.ydjk.org.cn/Article/details/gt3zkzzelxw.html

[S47] C++：结构化绑定遍历
来源：http://www.ydjk.org.cn/Article/details/gt3aneavhfc.html

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://www.ydjk.org.cn/Article/details/gt3jjznvcym.html

[S48] C++：逐行读文件
来源：http://www.ydjk.org.cn/Article/details/gt3sftrruey.html

std::ifstream in("a.txt");  std::string line;
来源：http://www.ydjk.org.cn/Article/details/gt3wfjdokyo.html

while (std::getline(in, line)) { }
来源：http://www.52xcode.cn/Article/details/gt3qfmlppoy.html

[S49] C++：写文件
来源：http://www.52xcode.cn/Article/details/gt3mazfhytf.html

std::ofstream out("a.txt");  out << "hi\n";
来源：http://www.ydjk.org.cn/Article/details/gt3xcvhxkqf.html

[S50] C++：格式化数字
来源：http://www.52xcode.cn/Article/details/gt3xnrsctmg.html

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://www.52xcode.cn/Article/details/gt3biqqtngi.html

[S51] C++：显式类型转换
来源：http://www.ydjk.org.cn/Article/details/gt3cuyiikzq.html

static_cast<double>(a) / b
来源：http://www.52xcode.cn/Article/details/gt3sghpxosq.html

[S52] C++：const 与 noexcept
来源：http://www.ydjk.org.cn/Article/details/gt3qlxxqhky.html

int size() const noexcept { return n_; }
来源：http://www.ydjk.org.cn/Article/details/gt3opcnqqdo.html

[S53] C++：移动语义
来源：http://www.52xcode.cn/Article/details/gt3rhujqwul.html

std::vector<int> w = std::move(v);
来源：http://www.ydjk.org.cn/Article/details/gt3rgxihnzs.html

[S54] C++：异常处理
来源：http://www.ydjk.org.cn/Article/details/gt3djhvwnfz.html

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://www.52xcode.cn/Article/details/gt3hpbsgzqy.html

[S55] C++：结构化绑定
来源：http://www.ydjk.org.cn/Article/details/gt3khigmsgv.html

auto [a, b] = std::make_pair(1, 2);
来源：http://www.52xcode.cn/Article/details/gt3vfazlmqx.html

[S56] C++：optional
来源：http://www.52xcode.cn/Article/details/gt3htyqvlkz.html

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://www.ydjk.org.cn/Article/details/gt3xoorcfcs.html

[S57] C++：编译期常量
来源：http://www.ydjk.org.cn/Article/details/gt3rwvdavsy.html

constexpr int N = 10;
来源：http://www.ydjk.org.cn/Article/details/gt3bixwpctu.html

[S58] C++：命名空间
来源：http://www.ydjk.org.cn/Article/details/gt3jxqzjttg.html

namespace ns { int f() { return 1; } }
来源：http://www.52xcode.cn/Article/details/gt3mwvcgllj.html

[S59] C++：静态断言
来源：http://www.ydjk.org.cn/Article/details/gt3ucmbmwsg.html

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://www.52xcode.cn/Article/details/gt3tsqpuwao.html

[S60] C++：遍历并删除元素
来源：http://www.52xcode.cn/Article/details/gt3yyejdnyf.html

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://www.ydjk.org.cn/Article/details/gt3zbgthxul.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3bsicjpge.html

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://www.ydjk.org.cn/Article/details/gt3mbeqgdzl.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3jczrelda.html

[T01] Kotlin：Hello World
来源：http://www.52xcode.cn/Article/details/gt3rpuwirvi.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3qeuxiwoq.html

[T02] Kotlin：变量
来源：http://www.ydjk.org.cn/Article/details/gt3szqnwcrc.html

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://www.52xcode.cn/Article/details/gt3tqwuktzl.html

[T03] Kotlin：字符串模板
来源：http://www.52xcode.cn/Article/details/gt3vaqzktkd.html

"值: $b"
来源：http://www.ydjk.org.cn/Article/details/gt3qetrmlyg.html

[T04] Kotlin：空安全
来源：http://www.ydjk.org.cn/Article/details/gt3hgbqoywv.html

val n: String? = null;  n?.length
来源：http://www.52xcode.cn/Article/details/gt3zpcgmvbk.html

[T05] Kotlin：when 表达式
来源：http://www.ydjk.org.cn/Article/details/gt3fgmmvwfd.html

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://www.52xcode.cn/Article/details/gt3unvfizjq.html

[T06] Kotlin：集合映射
来源：http://www.ydjk.org.cn/Article/details/gt3tkxuqvxs.html

listOf(1, 2, 3).map { it * 2 }
来源：http://www.52xcode.cn/Article/details/gt3vflcxnzc.html

[T07] Kotlin：集合过滤
来源：http://www.ydjk.org.cn/Article/details/gt3agwospnc.html

listOf(1, 2, 3).filter { it > 1 }
来源：http://www.52xcode.cn/Article/details/gt3vopinpig.html

[T08] Kotlin：数据类
来源：http://www.52xcode.cn/Article/details/gt3podzjgdo.html

data class User(val name: String, val age: Int)
来源：http://www.52xcode.cn/Article/details/gt3fsnakrkf.html

[T09] Kotlin：扩展函数
来源：http://www.ydjk.org.cn/Article/details/gt3svxmkulm.html

fun String.exclaim() = this + "!"
来源：http://www.ydjk.org.cn/Article/details/gt3qmoxrjoe.html

[T10] Kotlin：默认参数
来源：http://www.ydjk.org.cn/Article/details/gt3tvfbuins.html

fun greet(name: String = "World") = "Hi $name"
来源：http://www.52xcode.cn/Article/details/gt3oigqqzzs.html

[T11] Kotlin：协程
来源：http://www.52xcode.cn/Article/details/gt3lvhqkmpt.html

GlobalScope.launch { delay(1000); println("done") }
来源：http://www.52xcode.cn/Article/details/gt3kmlkzvgs.html

[T12] Kotlin：解构声明
来源：http://www.ydjk.org.cn/Article/details/gt3quupqrlf.html

val (a, b) = Pair(1, 2)
来源：http://www.52xcode.cn/Article/details/gt3nhkrmsdx.html

[T13] Kotlin：只读 Map
来源：http://www.52xcode.cn/Article/details/gt3eytrsvck.html

val m = mapOf("a" to 1)
来源：http://www.ydjk.org.cn/Article/details/gt3gmacgrjl.html

[T14] Kotlin：循环
来源：http://www.ydjk.org.cn/Article/details/gt3hshrlfza.html

for (i in 1..10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3utewbvfz.html

[T15] Kotlin：接口
来源：http://www.52xcode.cn/Article/details/gt3qyjqkdkm.html

interface Shape { fun area(): Double }
来源：http://www.ydjk.org.cn/Article/details/gt3szpslhjt.html

[T16] Swift：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3swzmgyfh.html

print("Hello")
来源：http://www.52xcode.cn/Article/details/gt3dbtfbzzk.html

[T17] Swift：变量与常量
来源：http://www.ydjk.org.cn/Article/details/gt3jedadxmf.html

var a = 1;  let b = 2
来源：http://www.52xcode.cn/Article/details/gt3ghtbzcey.html

[T18] Swift：字符串插值
来源：http://www.ydjk.org.cn/Article/details/gt3hzvvdicc.html

"值: \(b)"
来源：http://www.52xcode.cn/Article/details/gt3fwdadsmh.html

[T19] Swift：可选绑定
来源：http://www.ydjk.org.cn/Article/details/gt3lvqjrrex.html

if let n = opt { print(n) }
来源：http://www.52xcode.cn/Article/details/gt3nhhxcyll.html

[T20] Swift：数组操作
来源：http://www.52xcode.cn/Article/details/gt3ckligiyc.html

var a = [1, 2, 3];  a.append(4)
来源：http://www.52xcode.cn/Article/details/gt3oapizobd.html

[T21] Swift：遍历
来源：http://www.52xcode.cn/Article/details/gt3donmmdtb.html

for x in a { print(x) }
来源：http://www.52xcode.cn/Article/details/gt3samibcnh.html

[T22] Swift：字典
来源：http://www.ydjk.org.cn/Article/details/gt3ywlckcpp.html

var d = ["a": 1];  d["b"] = 2
来源：http://www.ydjk.org.cn/Article/details/gt3hixrfnwe.html

[T23] Swift：函数
来源：http://www.ydjk.org.cn/Article/details/gt3urigfuqs.html

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://www.52xcode.cn/Article/details/gt3vkmpgqdl.html

[T24] Swift：闭包
来源：http://www.52xcode.cn/Article/details/gt3ggpdyhdz.html

let f = { (x: Int) -> Int in x * 2 }
来源：http://www.ydjk.org.cn/Article/details/gt3xqnlmkkj.html

[T25] Swift：结构体
来源：http://www.ydjk.org.cn/Article/details/gt3pifnvyqc.html

struct P { var x: Int }
来源：http://www.52xcode.cn/Article/details/gt3wcyoujpe.html

[T26] Swift：类与重写
来源：http://www.52xcode.cn/Article/details/gt3qdfernwv.html

class A: Base { override func f() {} }
来源：http://www.ydjk.org.cn/Article/details/gt3qmibnawb.html

[T27] Swift：错误处理
来源：http://www.ydjk.org.cn/Article/details/gt3itbjitiz.html

do { try f() } catch { print(error) }
来源：http://www.52xcode.cn/Article/details/gt3hjhjqiby.html

[T28] Swift：枚举
来源：http://www.52xcode.cn/Article/details/gt3uigdsmxb.html

enum Color { case red, green }
来源：http://www.ydjk.org.cn/Article/details/gt3oehfcprm.html

[T29] Swift：guard 提前返回
来源：http://www.ydjk.org.cn/Article/details/gt3rhdlxpcz.html

guard let x = opt else { return }
来源：http://www.52xcode.cn/Article/details/gt3qicbxazd.html

[T30] Swift：协议
来源：http://www.52xcode.cn/Article/details/gt3pgljxqdo.html

protocol Shape { func area() -> Double }
来源：http://www.52xcode.cn/Article/details/gt3kgusavou.html

[T31] Lua：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3qykipzua.html

print("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3rzodjmlv.html

[T32] Lua：局部变量
来源：http://www.ydjk.org.cn/Article/details/gt3jepytpyq.html

local a = 1
来源：http://www.52xcode.cn/Article/details/gt3plesjgko.html

[T33] Lua：表（数组）
来源：http://www.52xcode.cn/Article/details/gt3ntciwogh.html

local t = {1, 2, 3};  t[4] = 4
来源：http://www.52xcode.cn/Article/details/gt3eskgjbdz.html

[T34] Lua：遍历表
来源：http://www.52xcode.cn/Article/details/gt3zhrnqjbk.html

for i, v in ipairs(t) do print(i, v) end
来源：http://www.52xcode.cn/Article/details/gt3xxqsfdzt.html

[T35] Lua：字典表
来源：http://www.ydjk.org.cn/Article/details/gt3uvlkmjwv.html

local d = { a = 1 };  d.b = 2
来源：http://www.52xcode.cn/Article/details/gt3tirtlxaq.html

[T36] Lua：函数
来源：http://www.52xcode.cn/Article/details/gt3fjyjfjyg.html

function add(a, b) return a + b end
来源：http://www.ydjk.org.cn/Article/details/gt3kfrqbhpg.html

[T37] Lua：字符串拼接
来源：http://www.ydjk.org.cn/Article/details/gt3dfdjbbfy.html

"a" .. "b"
来源：http://www.ydjk.org.cn/Article/details/gt3hhnvwhph.html

[T38] Lua：条件
来源：http://www.52xcode.cn/Article/details/gt3huybrqcy.html

if x > 0 then print("正") end
来源：http://www.52xcode.cn/Article/details/gt3njqxnqvr.html

[T39] Lua：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3fkdbmmsc.html

string.find(s, "%d+")
来源：http://www.ydjk.org.cn/Article/details/gt3ygweulxe.html

[T40] Lua：元表
来源：http://www.ydjk.org.cn/Article/details/gt3cpxbpwtt.html

setmetatable({}, { __index = base })
来源：http://www.ydjk.org.cn/Article/details/gt3evqabndr.html

[T41] Perl：Hello World
来源：http://www.ydjk.org.cn/Article/details/gt3slrvydwl.html

print "Hello\n";
来源：http://www.ydjk.org.cn/Article/details/gt3mqdnsgye.html

[T42] Perl：变量类型
来源：http://www.52xcode.cn/Article/details/gt3cytsausf.html

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://www.ydjk.org.cn/Article/details/gt3edkdcjex.html

[T43] Perl：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3uoifwkau.html

"值: $a"
来源：http://www.52xcode.cn/Article/details/gt3jbmzwrut.html

[T44] Perl：条件
来源：http://www.52xcode.cn/Article/details/gt3logbgylp.html

if ($a > 0) { print "正"; }
来源：http://www.52xcode.cn/Article/details/gt3otqqgpmc.html

[T45] Perl：数组遍历
来源：http://www.ydjk.org.cn/Article/details/gt3nlpajfnt.html

for my $x (@arr) { print $x; }
来源：http://www.ydjk.org.cn/Article/details/gt3hywglicp.html

[T46] Perl：哈希操作
来源：http://www.52xcode.cn/Article/details/gt3rkbldmnd.html

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://www.52xcode.cn/Article/details/gt3qaxrcwxe.html

[T47] Perl：正则捕获
来源：http://www.52xcode.cn/Article/details/gt3gpefngmy.html

if ($s =~ /(\d+)/) { print $1; }
来源：http://www.52xcode.cn/Article/details/gt3loscnvbb.html

[T48] Perl：正则替换
来源：http://www.52xcode.cn/Article/details/gt3zefkrqhn.html

$s =~ s/old/new/g;
来源：http://www.52xcode.cn/Article/details/gt3dfnzoelo.html

[T49] Perl：函数
来源：http://www.ydjk.org.cn/Article/details/gt3qbugoaey.html

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://www.52xcode.cn/Article/details/gt3xffipvbq.html

[T50] Perl：逐行读文件
来源：http://www.52xcode.cn/Article/details/gt3fafjwgyq.html

open my $fh, "<", "a.txt" or die $!;
来源：http://www.ydjk.org.cn/Article/details/gt3zwctdysn.html

while (my $line = <$fh>) { print $line; }
来源：http://www.ydjk.org.cn/Article/details/gt3gyjxrqom.html

[T51] Scala：Hello World
来源：http://www.52xcode.cn/Article/details/gt3huwwvops.html

println("Hello")
来源：http://www.ydjk.org.cn/Article/details/gt3hhxklbgf.html

[T52] Scala：变量
来源：http://www.52xcode.cn/Article/details/gt3niemrafn.html

val a = 1;  var b = 2
来源：http://www.52xcode.cn/Article/details/gt3gcqizhxb.html

[T53] Scala：字符串插值
来源：http://www.52xcode.cn/Article/details/gt3rrvypjpt.html

s"值: $b"
来源：http://www.52xcode.cn/Article/details/gt3ilqayqla.html

[T54] Scala：集合映射
来源：http://www.52xcode.cn/Article/details/gt3ukpvapcx.html

List(1, 2, 3).map(_ * 2)
来源：http://www.ydjk.org.cn/Article/details/gt3uhwsafek.html

[T55] Scala：集合过滤
来源：http://www.52xcode.cn/Article/details/gt3ptoddnoj.html

List(1, 2, 3).filter(_ > 1)
来源：http://www.52xcode.cn/Article/details/gt3stmwpvug.html

[T56] Scala：样例类
来源：http://www.52xcode.cn/Article/details/gt3mstglnlx.html

case class User(name: String, age: Int)
来源：http://www.ydjk.org.cn/Article/details/gt3lwevxnfg.html

[T57] Scala：模式匹配
来源：http://www.ydjk.org.cn/Article/details/gt3qdtvsqvy.html

x match { case 1 => "一"; case _ => "其他" }
来源：http://www.ydjk.org.cn/Article/details/gt3ahunyynp.html

[T58] Scala：函数定义
来源：http://www.ydjk.org.cn/Article/details/gt3cgybzabi.html

def add(a: Int, b: Int): Int = a + b
来源：http://www.52xcode.cn/Article/details/gt3gamlaphx.html

[T59] Scala：循环
来源：http://www.ydjk.org.cn/Article/details/gt3wtrpyqkd.html

for (i <- 1 to 10) println(i)
来源：http://www.52xcode.cn/Article/details/gt3vhikzdsw.html

[T60] Scala：折叠
来源：http://www.52xcode.cn/Article/details/gt3zghcnwzu.html

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://www.52xcode.cn/Article/details/gt3rjouzmba.html

================================================================================
来源：http://www.52xcode.cn/Article/details/gt3pcwfpgnq.html

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://www.ydjk.org.cn/Article/details/gt3lhwleszj.html

================================================================================
来源：http://www.ydjk.org.cn/Article/details/gt3scglnyma.html

[U01] Py：创建虚拟环境
来源：http://www.52xcode.cn/Article/details/gt3aqblbxtp.html

python -m venv .venv && source .venv/bin/activate
来源：http://www.ydjk.org.cn/Article/details/gt3qztxclvq.html

[U02] Py：导出 / 安装依赖
来源：http://www.ydjk.org.cn/Article/details/gt3ypvecsyj.html

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://www.ydjk.org.cn/Article/details/gt3wvcotlyx.html


<!-- 参考信息 -->