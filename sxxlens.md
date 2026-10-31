代发 wailian999

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ti.shxzskj.cn

[S08] C：动态内存分配与释放
来源：http://og.huixiangedu.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ho.szxytkj.cn

[S09] C：结构体定义与初始化
来源：http://bw.gzmigu.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://oy.szsharing.cn

[S10] C：指针与解引用
来源：http://db.huanxung.cn

int *p = &a;  *p = 5;
来源：http://ae.panjiajie.cn

[S11] C：逐行读文件
来源：http://ov.huixinmuqiang.cn

FILE *f = fopen("a.txt", "r");
来源：http://sj.521024.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://vf.panjiajie.cn

fclose(f);
来源：http://cc.jctech888.com.cn

[S12] C：写文件
来源：http://ft.wgjwhj.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ta.gzmigu.cn

[S13] C：宏定义
来源：http://jc.bookmarksfly.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ec.szxytkj.cn

[S14] C：枚举
来源：http://pm.shtwfgs.cn

enum Color { RED, GREEN, BLUE };
来源：http://eu.shtwfgs.cn

[S15] C：类型转换
来源：http://id.szsharing.cn

(double) a / b
来源：http://zi.shtwfgs.cn

[S16] C：位操作置位
来源：http://wl.szxytkj.cn

x |= (1 << 3);
来源：http://kd.yuexingan06.cn

[S17] C：安全拼接字符串
来源：http://tv.gzmigu.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://my.asd995.cn

[S18] C：命令行参数
来源：http://ru.chemitech.net.cn

int main(int argc, char **argv)
来源：http://iz.panjiajie.cn

[S19] C：快速排序
来源：http://rs.szxytkj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://sp.hnjuh.cn

[S20] C：二分查找
来源：http://bb.shtwfgs.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://rr.wgjwhj.cn

[S21] C：字符类别判断
来源：http://kw.szsharing.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://pa.jianghongdianzi.cn

[S22] C：字符串转数字
来源：http://ii.huanxung.cn

atoi("42");  strtod("3.14", NULL);
来源：http://qe.panjiajie.cn

[S23] C：随机数
来源：http://fr.bookmarksfly.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://cn.colortex.cn

[S24] C：获取本地时间
来源：http://vo.9csxet.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ln.nszjky.cn

[S25] C：内存拷贝
来源：http://sk.yuexingan06.cn

memcpy(dst, src, n);
来源：http://id.colortex.cn

[S26] C：内存清零
来源：http://wo.hnjuh.cn

memset(a, 0, sizeof a);
来源：http://ij.huanxung.cn

[S27] C：定义常量
来源：http://lu.jctech888.com.cn

const double PI = 3.14159;
来源：http://yp.bjjhwx.cn

[S28] C：静态变量
来源：http://xx.nszjky.cn

static int counter = 0;
来源：http://jb.huixiangedu.cn

[S29] C：变参函数
来源：http://hq.521024.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ay.panjiajie.cn

[S30] C：头文件保护
来源：http://cl.bookmarksfly.cn

#ifndef X_H
来源：http://ju.shxzskj.cn

#define X_H
来源：http://xp.panjiajie.cn

#endif
来源：http://nu.wgjwhj.cn

[S31] C++：Hello World
来源：http://xp.szxytkj.cn

#include <iostream>
来源：http://xz.shxzukj.cn

int main() { std::cout << "Hello\n"; }
来源：http://gd.muxihuayi.cn

[S32] C++：字符串
来源：http://ht.jianghongdianzi.cn

std::string s = "hi";  s += "!";
来源：http://dp.bookmarksfly.cn

[S33] C++：vector 增删
来源：http://ot.szsharing.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qa.szxytkj.cn

[S34] C++：遍历 vector
来源：http://zr.szxytkj.cn

for (auto &x : v) { std::cout << x; }
来源：http://je.gzmigu.cn

[S35] C++：map
来源：http://zh.hahajie.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ga.nszjky.cn

[S36] C++：unordered_map
来源：http://or.bjjhwx.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://dr.newstarts.cn

[S37] C++：set
来源：http://ip.wgjwhj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://tw.colortex.cn

[S38] C++：排序
来源：http://mb.jianghongdianzi.cn

std::sort(v.begin(), v.end());
来源：http://rd.lnxyls.cn

[S39] C++：自定义比较器排序
来源：http://uc.huixiangedu.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ey.colortex.cn

[S40] C++：查找元素
来源：http://to.bjjhwx.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ju.shxzukj.cn

[S41] C++：类与构造函数
来源：http://nq.lnxyls.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://qs.shtwfgs.cn

[S42] C++：继承与虚函数
来源：http://nv.haigaiapp.cn

class B : public Base { public: void f() override {} };
来源：http://sk.nszjky.cn

[S43] C++：智能指针
来源：http://ib.newstarts.cn

auto p = std::make_unique<int>(5);
来源：http://pe.shxzukj.cn

[S44] C++：引用传参
来源：http://bd.521024.cn

void inc(int &x) { ++x; }
来源：http://tj.asd995.cn

[S45] C++：lambda
来源：http://lh.yuexingan06.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ns.shxzskj.cn

[S46] C++：函数模板
来源：http://sw.szxytkj.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://dl.nszjky.cn

[S47] C++：结构化绑定遍历
来源：http://cl.yuntaijiaju.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hl.colortex.cn

[S48] C++：逐行读文件
来源：http://qm.nszjky.cn

std::ifstream in("a.txt");  std::string line;
来源：http://jq.szsharing.cn

while (std::getline(in, line)) { }
来源：http://pd.jctech888.com.cn

[S49] C++：写文件
来源：http://je.lnxyls.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hv.bookmarksfly.cn

[S50] C++：格式化数字
来源：http://yx.huixinmuqiang.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://nk.colortex.cn

[S51] C++：显式类型转换
来源：http://zl.bookmarksfly.cn

static_cast<double>(a) / b
来源：http://sa.szsharing.cn

[S52] C++：const 与 noexcept
来源：http://lc.bjjhwx.cn

int size() const noexcept { return n_; }
来源：http://mx.muxihuayi.cn

[S53] C++：移动语义
来源：http://qc.haigaiapp.cn

std::vector<int> w = std::move(v);
来源：http://mp.huixinmuqiang.cn

[S54] C++：异常处理
来源：http://kg.colortex.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://xf.jianghongdianzi.cn

[S55] C++：结构化绑定
来源：http://eh.wgjwhj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://mz.wgjwhj.cn

[S56] C++：optional
来源：http://jv.muxihuayi.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hy.huixinmuqiang.cn

[S57] C++：编译期常量
来源：http://tk.huixiangedu.cn

constexpr int N = 10;
来源：http://xh.shxzukj.cn

[S58] C++：命名空间
来源：http://jm.yuntaijiaju.cn

namespace ns { int f() { return 1; } }
来源：http://gj.chemitech.net.cn

[S59] C++：静态断言
来源：http://dn.shxzukj.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ko.colortex.cn

[S60] C++：遍历并删除元素
来源：http://eq.nszjky.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mv.jianghongdianzi.cn

================================================================================
来源：http://ji.haigaiapp.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hu.panjiajie.cn

================================================================================
来源：http://dq.bookmarksfly.cn

[T01] Kotlin：Hello World
来源：http://yp.shxzukj.cn

println("Hello")
来源：http://xs.jianghongdianzi.cn

[T02] Kotlin：变量
来源：http://uc.szsharing.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wt.huixinmuqiang.cn

[T03] Kotlin：字符串模板
来源：http://wc.yuexingan06.cn

"值: $b"
来源：http://cz.chemitech.net.cn

[T04] Kotlin：空安全
来源：http://np.wgjwhj.cn

val n: String? = null;  n?.length
来源：http://sp.nszjky.cn

[T05] Kotlin：when 表达式
来源：http://yq.nicolike.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://oa.huixinmuqiang.cn

[T06] Kotlin：集合映射
来源：http://rm.hahajie.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://nt.newstarts.cn

[T07] Kotlin：集合过滤
来源：http://xp.szsharing.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ye.szsharing.cn

[T08] Kotlin：数据类
来源：http://av.521024.cn

data class User(val name: String, val age: Int)
来源：http://oh.bjjhwx.cn

[T09] Kotlin：扩展函数
来源：http://xf.gzmigu.cn

fun String.exclaim() = this + "!"
来源：http://sq.szsharing.cn

[T10] Kotlin：默认参数
来源：http://tz.szxytkj.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://vs.muxihuayi.cn

[T11] Kotlin：协程
来源：http://qn.shxzskj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://pj.9csxet.cn

[T12] Kotlin：解构声明
来源：http://iq.yuntaijiaju.cn

val (a, b) = Pair(1, 2)
来源：http://os.huixiangedu.cn

[T13] Kotlin：只读 Map
来源：http://gw.shxzukj.cn

val m = mapOf("a" to 1)
来源：http://mq.haigaiapp.cn

[T14] Kotlin：循环
来源：http://ws.nicolike.cn

for (i in 1..10) println(i)
来源：http://an.shxzukj.cn

[T15] Kotlin：接口
来源：http://xz.jctech888.com.cn

interface Shape { fun area(): Double }
来源：http://ew.chemitech.net.cn

[T16] Swift：Hello World
来源：http://og.huanxung.cn

print("Hello")
来源：http://uh.jianghongdianzi.cn

[T17] Swift：变量与常量
来源：http://pj.shtwfgs.cn

var a = 1;  let b = 2
来源：http://fi.shxzukj.cn

[T18] Swift：字符串插值
来源：http://fr.jianghongdianzi.cn

"值: \(b)"
来源：http://fd.hnjuh.cn

[T19] Swift：可选绑定
来源：http://ct.chemitech.net.cn

if let n = opt { print(n) }
来源：http://oy.haigaiapp.cn

[T20] Swift：数组操作
来源：http://nj.panjiajie.cn

var a = [1, 2, 3];  a.append(4)
来源：http://gw.521024.cn

[T21] Swift：遍历
来源：http://dk.hnjuh.cn

for x in a { print(x) }
来源：http://gh.hnjuh.cn

[T22] Swift：字典
来源：http://vw.yuntaijiaju.cn

var d = ["a": 1];  d["b"] = 2
来源：http://xo.yuexingan06.cn

[T23] Swift：函数
来源：http://jh.hnjuh.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://xt.muxihuayi.cn

[T24] Swift：闭包
来源：http://cz.jianghongdianzi.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://wp.jctech888.com.cn

[T25] Swift：结构体
来源：http://it.colortex.cn

struct P { var x: Int }
来源：http://cb.shtwfgs.cn

[T26] Swift：类与重写
来源：http://tt.szxytkj.cn

class A: Base { override func f() {} }
来源：http://at.nicolike.cn

[T27] Swift：错误处理
来源：http://ms.shtwfgs.cn

do { try f() } catch { print(error) }
来源：http://xh.nicolike.cn

[T28] Swift：枚举
来源：http://ls.huixinmuqiang.cn

enum Color { case red, green }
来源：http://vv.wgjwhj.cn

[T29] Swift：guard 提前返回
来源：http://np.colortex.cn

guard let x = opt else { return }
来源：http://zj.colortex.cn

[T30] Swift：协议
来源：http://gi.szsharing.cn

protocol Shape { func area() -> Double }
来源：http://sa.chemitech.net.cn

[T31] Lua：Hello World
来源：http://zn.hnjuh.cn

print("Hello")
来源：http://yc.huanxung.cn

[T32] Lua：局部变量
来源：http://mu.gzmigu.cn

local a = 1
来源：http://ik.hahajie.cn

[T33] Lua：表（数组）
来源：http://vr.jctech888.com.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://qf.newstarts.cn

[T34] Lua：遍历表
来源：http://re.hnjuh.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://kv.haigaiapp.cn

[T35] Lua：字典表
来源：http://xi.asd995.cn

local d = { a = 1 };  d.b = 2
来源：http://br.521024.cn

[T36] Lua：函数
来源：http://fg.muxihuayi.cn

function add(a, b) return a + b end
来源：http://gn.muxihuayi.cn

[T37] Lua：字符串拼接
来源：http://wl.yuntaijiaju.cn

"a" .. "b"
来源：http://vk.nicolike.cn

[T38] Lua：条件
来源：http://ti.newstarts.cn

if x > 0 then print("正") end
来源：http://be.huixiangedu.cn

[T39] Lua：模式匹配
来源：http://bd.yuntaijiaju.cn

string.find(s, "%d+")
来源：http://xl.lnxyls.cn

[T40] Lua：元表
来源：http://el.jctech888.com.cn

setmetatable({}, { __index = base })
来源：http://sh.shxzskj.cn

[T41] Perl：Hello World
来源：http://la.yuexingan06.cn

print "Hello\n";
来源：http://gb.wgjwhj.cn

[T42] Perl：变量类型
来源：http://yh.hnjuh.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://km.9csxet.cn

[T43] Perl：字符串插值
来源：http://bn.asd995.cn

"值: $a"
来源：http://jy.wgjwhj.cn

[T44] Perl：条件
来源：http://zx.haigaiapp.cn

if ($a > 0) { print "正"; }
来源：http://ls.shtwfgs.cn

[T45] Perl：数组遍历
来源：http://lf.shxzskj.cn

for my $x (@arr) { print $x; }
来源：http://mn.panjiajie.cn

[T46] Perl：哈希操作
来源：http://jv.haigaiapp.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://og.newstarts.cn

[T47] Perl：正则捕获
来源：http://ig.colortex.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://mg.yuntaijiaju.cn

[T48] Perl：正则替换
来源：http://bx.hahajie.cn

$s =~ s/old/new/g;
来源：http://fc.haigaiapp.cn

[T49] Perl：函数
来源：http://rs.jianghongdianzi.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mn.jianghongdianzi.cn

[T50] Perl：逐行读文件
来源：http://tu.bookmarksfly.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ec.panjiajie.cn

while (my $line = <$fh>) { print $line; }
来源：http://ve.haigaiapp.cn

[T51] Scala：Hello World
来源：http://be.yuexingan06.cn

println("Hello")
来源：http://as.nicolike.cn

[T52] Scala：变量
来源：http://ge.lnxyls.cn

val a = 1;  var b = 2
来源：http://qj.shtwfgs.cn

[T53] Scala：字符串插值
来源：http://sc.haigaiapp.cn

s"值: $b"
来源：http://gc.9csxet.cn

[T54] Scala：集合映射
来源：http://uy.huixiangedu.cn

List(1, 2, 3).map(_ * 2)
来源：http://pq.huanxung.cn

[T55] Scala：集合过滤
来源：http://bf.9csxet.cn

List(1, 2, 3).filter(_ > 1)
来源：http://uq.huixiangedu.cn

[T56] Scala：样例类
来源：http://hj.haigaiapp.cn

case class User(name: String, age: Int)
来源：http://gn.shxzukj.cn

[T57] Scala：模式匹配
来源：http://wd.hnjuh.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://su.huixiangedu.cn

[T58] Scala：函数定义
来源：http://sz.shxzukj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://au.szsharing.cn

[T59] Scala：循环
来源：http://ca.bookmarksfly.cn

for (i <- 1 to 10) println(i)
来源：http://rc.jianghongdianzi.cn

[T60] Scala：折叠
来源：http://ky.nicolike.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://fa.yuntaijiaju.cn

================================================================================
来源：http://dh.bookmarksfly.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://zl.jctech888.com.cn

================================================================================
来源：http://tr.521024.cn

[U01] Py：创建虚拟环境
来源：http://vy.nszjky.cn

python -m venv .venv && source .venv/bin/activate
来源：http://fe.huixinmuqiang.cn

[U02] Py：导出 / 安装依赖
来源：http://vr.shxzskj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://lc.9csxet.cn

[U03] Py：加载 .env 配置
来源：http://tv.szxytkj.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://mc.9csxet.cn

[U04] Py：变量调试打印
来源：http://lp.colortex.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://kv.jianghongdianzi.cn

[U05] Py：列表去重且保序
来源：http://mo.yuexingan06.cn

list(dict.fromkeys(arr))
来源：http://vf.lnxyls.cn

[U06] Py：合并两个字典
来源：http://qq.shxzukj.cn

{**a, **b}
来源：http://xk.bjjhwx.cn

[U07] Py：反转字典键值
来源：http://pr.wgjwhj.cn

{v: k for k, v in d.items()}
来源：http://pd.muxihuayi.cn

[U08] Py：展平二维列表
来源：http://qz.huixinmuqiang.cn

[y for x in nested for y in x]
来源：http://nc.colortex.cn

[U09] Py：字典取最大值的键
来源：http://vx.szsharing.cn

max(d, key=d.get)
来源：http://qc.jianghongdianzi.cn

[U10] Py：按值排序字典
来源：http://ig.szxytkj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://sq.9csxet.cn

[U11] Py：生成器表达式
来源：http://lv.gzmigu.cn

(x * 2 for x in arr)
来源：http://je.shtwfgs.cn

[U12] Py：取出现最多的 3 个元素
来源：http://xw.shxzskj.cn

Counter(arr).most_common(3)
来源：http://rr.bookmarksfly.cn

[U13] Py：固定长度队列
来源：http://ea.lnxyls.cn

deque(maxlen=10)
来源：http://df.yuntaijiaju.cn

[U14] Py：分组收集到列表
来源：http://om.shxzskj.cn

defaultdict(list)
来源：http://vr.muxihuayi.cn

[U15] Py：高精度计时
来源：http://xo.huixinmuqiang.cn

t = time.perf_counter()
来源：http://lr.panjiajie.cn

[U16] Py：命令行参数解析
来源：http://cb.shxzukj.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://zu.jianghongdianzi.cn

[U17] Py：初始化日志
来源：http://ve.jianghongdianzi.cn

logging.basicConfig(level=logging.INFO)
来源：http://cw.bjjhwx.cn

[U18] Py：预编译正则
来源：http://az.asd995.cn

pat = re.compile(r"\d+")
来源：http://uz.gzmigu.cn

[U19] Py：正则替换带回调
来源：http://yq.hnjuh.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://su.colortex.cn

[U20] Py：缓存函数结果
来源：http://tx.newstarts.cn

@functools.lru_cache(maxsize=None)
来源：http://fu.nicolike.cn

[U21] Py：自定义上下文管理器
来源：http://up.newstarts.cn

@contextlib.contextmanager
来源：http://eu.shtwfgs.cn

[U22] Py：矩阵转置
来源：http://rw.lnxyls.cn

list(zip(*m))
来源：http://ha.hnjuh.cn

[U23] Py：分块读取大文件
来源：http://hv.newstarts.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://gs.jctech888.com.cn

[U24] Py：路径操作
来源：http://db.newstarts.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ir.panjiajie.cn

[U25] Py：CSV 按字典读
来源：http://ud.newstarts.cn

csv.DictReader(f)
来源：http://ds.chemitech.net.cn

[U26] Py：并发下载
来源：http://sj.newstarts.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ig.haigaiapp.cn

[U27] Py：异步 HTTP
来源：http://ey.nszjky.cn

aiohttp.ClientSession() 配合 async with
来源：http://xp.nszjky.cn

[U28] Py：类型别名
来源：http://ll.haigaiapp.cn

UserId = int
来源：http://vx.jianghongdianzi.cn

[U29] Py：属性校验
来源：http://bf.muxihuayi.cn

@property 与 @x.setter 配合
来源：http://yo.huanxung.cn

[U30] Py：数据类
来源：http://lr.wgjwhj.cn

@dataclass(slots=True)
来源：http://wj.huixinmuqiang.cn


<!-- 参考信息 -->