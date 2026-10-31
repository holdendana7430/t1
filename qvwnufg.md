代发 wailian999

strlen(s)
来源：http://qc.panjiajie.cn

[S06] C：字符串比较
来源：http://bd.gzmigu.cn

strcmp(a, b) == 0
来源：http://gu.yuexingan06.cn

[S07] C：数组遍历求和
来源：http://ij.gzmigu.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://rj.shtwfgs.cn

[S08] C：动态内存分配与释放
来源：http://no.nicolike.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://nl.nszjky.cn

[S09] C：结构体定义与初始化
来源：http://nr.521024.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://bi.shxzskj.cn

[S10] C：指针与解引用
来源：http://cb.muxihuayi.cn

int *p = &a;  *p = 5;
来源：http://tb.yuntaijiaju.cn

[S11] C：逐行读文件
来源：http://an.nszjky.cn

FILE *f = fopen("a.txt", "r");
来源：http://ts.haigaiapp.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://xz.9csxet.cn

fclose(f);
来源：http://bu.huanxung.cn

[S12] C：写文件
来源：http://qz.bookmarksfly.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://cb.yuexingan06.cn

[S13] C：宏定义
来源：http://dh.shxzskj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://yd.szxytkj.cn

[S14] C：枚举
来源：http://zy.nicolike.cn

enum Color { RED, GREEN, BLUE };
来源：http://rk.hnjuh.cn

[S15] C：类型转换
来源：http://vk.jianghongdianzi.cn

(double) a / b
来源：http://qf.bjjhwx.cn

[S16] C：位操作置位
来源：http://mv.huanxung.cn

x |= (1 << 3);
来源：http://yb.huanxung.cn

[S17] C：安全拼接字符串
来源：http://pe.bookmarksfly.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://xa.lnxyls.cn

[S18] C：命令行参数
来源：http://km.bjjhwx.cn

int main(int argc, char **argv)
来源：http://kn.yuexingan06.cn

[S19] C：快速排序
来源：http://as.wgjwhj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://rs.wgjwhj.cn

[S20] C：二分查找
来源：http://yy.lnxyls.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://sc.yuexingan06.cn

[S21] C：字符类别判断
来源：http://ru.nicolike.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ek.9csxet.cn

[S22] C：字符串转数字
来源：http://li.asd995.cn

atoi("42");  strtod("3.14", NULL);
来源：http://rg.colortex.cn

[S23] C：随机数
来源：http://eu.szsharing.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://qi.szxytkj.cn

[S24] C：获取本地时间
来源：http://ee.huanxung.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://du.asd995.cn

[S25] C：内存拷贝
来源：http://zk.jianghongdianzi.cn

memcpy(dst, src, n);
来源：http://ed.bookmarksfly.cn

[S26] C：内存清零
来源：http://ba.hnjuh.cn

memset(a, 0, sizeof a);
来源：http://jx.bjjhwx.cn

[S27] C：定义常量
来源：http://mt.asd995.cn

const double PI = 3.14159;
来源：http://it.szxytkj.cn

[S28] C：静态变量
来源：http://qd.bjjhwx.cn

static int counter = 0;
来源：http://fm.szxytkj.cn

[S29] C：变参函数
来源：http://tv.521024.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://bf.hnjuh.cn

[S30] C：头文件保护
来源：http://bc.panjiajie.cn

#ifndef X_H
来源：http://pl.szsharing.cn

#define X_H
来源：http://aw.muxihuayi.cn

#endif
来源：http://ux.muxihuayi.cn

[S31] C++：Hello World
来源：http://gc.shxzukj.cn

#include <iostream>
来源：http://lx.panjiajie.cn

int main() { std::cout << "Hello\n"; }
来源：http://bw.panjiajie.cn

[S32] C++：字符串
来源：http://de.hnjuh.cn

std::string s = "hi";  s += "!";
来源：http://rw.9csxet.cn

[S33] C++：vector 增删
来源：http://ub.huanxung.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ew.szxytkj.cn

[S34] C++：遍历 vector
来源：http://bs.hahajie.cn

for (auto &x : v) { std::cout << x; }
来源：http://oc.bookmarksfly.cn

[S35] C++：map
来源：http://nk.huanxung.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://vr.hahajie.cn

[S36] C++：unordered_map
来源：http://qz.huanxung.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://cg.9csxet.cn

[S37] C++：set
来源：http://rc.nszjky.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://dg.521024.cn

[S38] C++：排序
来源：http://cy.bookmarksfly.cn

std::sort(v.begin(), v.end());
来源：http://lz.haigaiapp.cn

[S39] C++：自定义比较器排序
来源：http://bt.bjjhwx.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://av.chemitech.net.cn

[S40] C++：查找元素
来源：http://fh.jctech888.com.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://en.lnxyls.cn

[S41] C++：类与构造函数
来源：http://ga.bjjhwx.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://bg.panjiajie.cn

[S42] C++：继承与虚函数
来源：http://si.huixinmuqiang.cn

class B : public Base { public: void f() override {} };
来源：http://fk.jianghongdianzi.cn

[S43] C++：智能指针
来源：http://vs.muxihuayi.cn

auto p = std::make_unique<int>(5);
来源：http://zn.asd995.cn

[S44] C++：引用传参
来源：http://ns.szxytkj.cn

void inc(int &x) { ++x; }
来源：http://ak.huanxung.cn

[S45] C++：lambda
来源：http://xy.huixiangedu.cn

auto add = [](int a, int b) { return a + b; };
来源：http://cd.haigaiapp.cn

[S46] C++：函数模板
来源：http://li.chemitech.net.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://bg.lnxyls.cn

[S47] C++：结构化绑定遍历
来源：http://zj.muxihuayi.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://zn.szsharing.cn

[S48] C++：逐行读文件
来源：http://xc.gzmigu.cn

std::ifstream in("a.txt");  std::string line;
来源：http://sk.hnjuh.cn

while (std::getline(in, line)) { }
来源：http://kd.jianghongdianzi.cn

[S49] C++：写文件
来源：http://px.9csxet.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://vc.nszjky.cn

[S50] C++：格式化数字
来源：http://sw.panjiajie.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://pr.9csxet.cn

[S51] C++：显式类型转换
来源：http://ea.haigaiapp.cn

static_cast<double>(a) / b
来源：http://es.shtwfgs.cn

[S52] C++：const 与 noexcept
来源：http://ax.szsharing.cn

int size() const noexcept { return n_; }
来源：http://wd.gzmigu.cn

[S53] C++：移动语义
来源：http://fn.9csxet.cn

std::vector<int> w = std::move(v);
来源：http://gu.jianghongdianzi.cn

[S54] C++：异常处理
来源：http://ey.bjjhwx.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://dk.asd995.cn

[S55] C++：结构化绑定
来源：http://fo.jctech888.com.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ln.haigaiapp.cn

[S56] C++：optional
来源：http://rx.chemitech.net.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://cz.yuexingan06.cn

[S57] C++：编译期常量
来源：http://uf.bookmarksfly.cn

constexpr int N = 10;
来源：http://vv.shtwfgs.cn

[S58] C++：命名空间
来源：http://lb.szxytkj.cn

namespace ns { int f() { return 1; } }
来源：http://zr.jianghongdianzi.cn

[S59] C++：静态断言
来源：http://hj.szsharing.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://bb.hahajie.cn

[S60] C++：遍历并删除元素
来源：http://gb.hnjuh.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://gz.panjiajie.cn

================================================================================
来源：http://hq.chemitech.net.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hl.hnjuh.cn

================================================================================
来源：http://fm.haigaiapp.cn

[T01] Kotlin：Hello World
来源：http://rp.shtwfgs.cn

println("Hello")
来源：http://sn.muxihuayi.cn

[T02] Kotlin：变量
来源：http://mf.hnjuh.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://cn.jianghongdianzi.cn

[T03] Kotlin：字符串模板
来源：http://ac.szsharing.cn

"值: $b"
来源：http://gb.haigaiapp.cn

[T04] Kotlin：空安全
来源：http://dk.bjjhwx.cn

val n: String? = null;  n?.length
来源：http://vl.jctech888.com.cn

[T05] Kotlin：when 表达式
来源：http://lo.nicolike.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://vz.haigaiapp.cn

[T06] Kotlin：集合映射
来源：http://vb.asd995.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://da.panjiajie.cn

[T07] Kotlin：集合过滤
来源：http://wf.muxihuayi.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://hh.asd995.cn

[T08] Kotlin：数据类
来源：http://qe.jianghongdianzi.cn

data class User(val name: String, val age: Int)
来源：http://ep.newstarts.cn

[T09] Kotlin：扩展函数
来源：http://om.bookmarksfly.cn

fun String.exclaim() = this + "!"
来源：http://dd.chemitech.net.cn

[T10] Kotlin：默认参数
来源：http://iq.shxzukj.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://pk.panjiajie.cn

[T11] Kotlin：协程
来源：http://xx.haigaiapp.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ob.colortex.cn

[T12] Kotlin：解构声明
来源：http://xs.521024.cn

val (a, b) = Pair(1, 2)
来源：http://ff.shtwfgs.cn

[T13] Kotlin：只读 Map
来源：http://td.jctech888.com.cn

val m = mapOf("a" to 1)
来源：http://ea.shtwfgs.cn

[T14] Kotlin：循环
来源：http://bf.lnxyls.cn

for (i in 1..10) println(i)
来源：http://st.szsharing.cn

[T15] Kotlin：接口
来源：http://gi.jianghongdianzi.cn

interface Shape { fun area(): Double }
来源：http://vg.szxytkj.cn

[T16] Swift：Hello World
来源：http://oy.nszjky.cn

print("Hello")
来源：http://uj.yuexingan06.cn

[T17] Swift：变量与常量
来源：http://fg.huanxung.cn

var a = 1;  let b = 2
来源：http://qt.haigaiapp.cn

[T18] Swift：字符串插值
来源：http://qq.jianghongdianzi.cn

"值: \(b)"
来源：http://lw.colortex.cn

[T19] Swift：可选绑定
来源：http://qr.9csxet.cn

if let n = opt { print(n) }
来源：http://er.shxzukj.cn

[T20] Swift：数组操作
来源：http://dv.wgjwhj.cn

var a = [1, 2, 3];  a.append(4)
来源：http://as.shxzskj.cn

[T21] Swift：遍历
来源：http://pa.panjiajie.cn

for x in a { print(x) }
来源：http://oq.jctech888.com.cn

[T22] Swift：字典
来源：http://cm.asd995.cn

var d = ["a": 1];  d["b"] = 2
来源：http://lh.hnjuh.cn

[T23] Swift：函数
来源：http://vm.szsharing.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://cy.lnxyls.cn

[T24] Swift：闭包
来源：http://gu.lnxyls.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://pe.hahajie.cn

[T25] Swift：结构体
来源：http://bs.chemitech.net.cn

struct P { var x: Int }
来源：http://aw.bjjhwx.cn

[T26] Swift：类与重写
来源：http://td.wgjwhj.cn

class A: Base { override func f() {} }
来源：http://cn.bookmarksfly.cn

[T27] Swift：错误处理
来源：http://dk.chemitech.net.cn

do { try f() } catch { print(error) }
来源：http://bk.jctech888.com.cn

[T28] Swift：枚举
来源：http://vo.panjiajie.cn

enum Color { case red, green }
来源：http://nw.huixinmuqiang.cn

[T29] Swift：guard 提前返回
来源：http://fd.newstarts.cn

guard let x = opt else { return }
来源：http://wp.nicolike.cn

[T30] Swift：协议
来源：http://zn.lnxyls.cn

protocol Shape { func area() -> Double }
来源：http://hu.hahajie.cn

[T31] Lua：Hello World
来源：http://rl.shxzukj.cn

print("Hello")
来源：http://al.bjjhwx.cn

[T32] Lua：局部变量
来源：http://rf.bjjhwx.cn

local a = 1
来源：http://xl.shtwfgs.cn

[T33] Lua：表（数组）
来源：http://pq.huixinmuqiang.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://re.newstarts.cn

[T34] Lua：遍历表
来源：http://ud.yuntaijiaju.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://cg.chemitech.net.cn

[T35] Lua：字典表
来源：http://bp.chemitech.net.cn

local d = { a = 1 };  d.b = 2
来源：http://fd.jianghongdianzi.cn

[T36] Lua：函数
来源：http://ni.huanxung.cn

function add(a, b) return a + b end
来源：http://tv.yuexingan06.cn

[T37] Lua：字符串拼接
来源：http://fk.bookmarksfly.cn

"a" .. "b"
来源：http://pm.jianghongdianzi.cn

[T38] Lua：条件
来源：http://xq.shtwfgs.cn

if x > 0 then print("正") end
来源：http://bv.shxzskj.cn

[T39] Lua：模式匹配
来源：http://od.jianghongdianzi.cn

string.find(s, "%d+")
来源：http://ad.hnjuh.cn

[T40] Lua：元表
来源：http://rq.521024.cn

setmetatable({}, { __index = base })
来源：http://pk.gzmigu.cn

[T41] Perl：Hello World
来源：http://pf.hahajie.cn

print "Hello\n";
来源：http://js.huanxung.cn

[T42] Perl：变量类型
来源：http://op.nszjky.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://kd.hnjuh.cn

[T43] Perl：字符串插值
来源：http://uh.9csxet.cn

"值: $a"
来源：http://ig.bjjhwx.cn

[T44] Perl：条件
来源：http://nl.szxytkj.cn

if ($a > 0) { print "正"; }
来源：http://uh.lnxyls.cn

[T45] Perl：数组遍历
来源：http://as.haigaiapp.cn

for my $x (@arr) { print $x; }
来源：http://ig.shxzukj.cn

[T46] Perl：哈希操作
来源：http://ra.huanxung.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://nm.szxytkj.cn

[T47] Perl：正则捕获
来源：http://dk.huixinmuqiang.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://tv.nszjky.cn

[T48] Perl：正则替换
来源：http://hj.huixiangedu.cn

$s =~ s/old/new/g;
来源：http://dh.szsharing.cn

[T49] Perl：函数
来源：http://zo.jctech888.com.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://lh.9csxet.cn

[T50] Perl：逐行读文件
来源：http://zk.bookmarksfly.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://pt.hnjuh.cn

while (my $line = <$fh>) { print $line; }
来源：http://bh.huanxung.cn

[T51] Scala：Hello World
来源：http://wj.huixiangedu.cn

println("Hello")
来源：http://ag.9csxet.cn

[T52] Scala：变量
来源：http://dq.szsharing.cn

val a = 1;  var b = 2
来源：http://sh.shtwfgs.cn

[T53] Scala：字符串插值
来源：http://qc.hahajie.cn

s"值: $b"
来源：http://vs.colortex.cn

[T54] Scala：集合映射
来源：http://ss.chemitech.net.cn

List(1, 2, 3).map(_ * 2)
来源：http://qv.nszjky.cn

[T55] Scala：集合过滤
来源：http://xw.jctech888.com.cn

List(1, 2, 3).filter(_ > 1)
来源：http://in.lnxyls.cn

[T56] Scala：样例类
来源：http://va.bjjhwx.cn

case class User(name: String, age: Int)
来源：http://ta.shtwfgs.cn

[T57] Scala：模式匹配
来源：http://yk.jianghongdianzi.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ro.yuntaijiaju.cn

[T58] Scala：函数定义
来源：http://th.bookmarksfly.cn

def add(a: Int, b: Int): Int = a + b
来源：http://rm.haigaiapp.cn

[T59] Scala：循环
来源：http://ju.colortex.cn

for (i <- 1 to 10) println(i)
来源：http://nw.wgjwhj.cn

[T60] Scala：折叠
来源：http://dq.huanxung.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://fr.hahajie.cn

================================================================================
来源：http://wf.newstarts.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://za.bjjhwx.cn

================================================================================
来源：http://lt.nszjky.cn

[U01] Py：创建虚拟环境
来源：http://zo.wgjwhj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://fu.colortex.cn

[U02] Py：导出 / 安装依赖
来源：http://ti.wgjwhj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://tg.haigaiapp.cn

[U03] Py：加载 .env 配置
来源：http://iq.szxytkj.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://im.shxzukj.cn

[U04] Py：变量调试打印
来源：http://lu.haigaiapp.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://lv.szxytkj.cn

[U05] Py：列表去重且保序
来源：http://jz.colortex.cn

list(dict.fromkeys(arr))
来源：http://xn.shtwfgs.cn

[U06] Py：合并两个字典
来源：http://yu.chemitech.net.cn

{**a, **b}
来源：http://gl.lnxyls.cn

[U07] Py：反转字典键值
来源：http://vg.muxihuayi.cn

{v: k for k, v in d.items()}
来源：http://pe.bookmarksfly.cn

[U08] Py：展平二维列表
来源：http://su.jianghongdianzi.cn

[y for x in nested for y in x]
来源：http://im.bjjhwx.cn

[U09] Py：字典取最大值的键
来源：http://dy.hahajie.cn

max(d, key=d.get)
来源：http://zr.jianghongdianzi.cn

[U10] Py：按值排序字典
来源：http://ll.521024.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://lk.huixiangedu.cn

[U11] Py：生成器表达式
来源：http://nb.panjiajie.cn

(x * 2 for x in arr)
来源：http://lt.haigaiapp.cn

[U12] Py：取出现最多的 3 个元素
来源：http://xi.panjiajie.cn

Counter(arr).most_common(3)
来源：http://ip.gzmigu.cn

[U13] Py：固定长度队列
来源：http://tm.nszjky.cn

deque(maxlen=10)
来源：http://iv.shxzukj.cn

[U14] Py：分组收集到列表
来源：http://jf.huixiangedu.cn

defaultdict(list)
来源：http://aw.chemitech.net.cn

[U15] Py：高精度计时
来源：http://xv.yuexingan06.cn

t = time.perf_counter()
来源：http://kp.hnjuh.cn

[U16] Py：命令行参数解析
来源：http://on.lnxyls.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://kc.nicolike.cn

[U17] Py：初始化日志
来源：http://hz.gzmigu.cn

logging.basicConfig(level=logging.INFO)
来源：http://gk.wgjwhj.cn

[U18] Py：预编译正则
来源：http://yl.hnjuh.cn

pat = re.compile(r"\d+")
来源：http://zz.gzmigu.cn

[U19] Py：正则替换带回调
来源：http://ik.bookmarksfly.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://is.9csxet.cn

[U20] Py：缓存函数结果
来源：http://ak.asd995.cn

@functools.lru_cache(maxsize=None)
来源：http://by.nicolike.cn

[U21] Py：自定义上下文管理器
来源：http://om.shxzskj.cn

@contextlib.contextmanager
来源：http://ck.jctech888.com.cn

[U22] Py：矩阵转置
来源：http://oy.haigaiapp.cn

list(zip(*m))
来源：http://al.nszjky.cn

[U23] Py：分块读取大文件
来源：http://ht.asd995.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://xa.521024.cn

[U24] Py：路径操作
来源：http://fo.shxzskj.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://yi.9csxet.cn

[U25] Py：CSV 按字典读
来源：http://jg.nszjky.cn

csv.DictReader(f)
来源：http://hf.szxytkj.cn

[U26] Py：并发下载
来源：http://cv.jianghongdianzi.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://qb.colortex.cn

[U27] Py：异步 HTTP
来源：http://jg.nszjky.cn

aiohttp.ClientSession() 配合 async with
来源：http://nl.yuexingan06.cn

[U28] Py：类型别名
来源：http://zj.chemitech.net.cn

UserId = int
来源：http://zc.hnjuh.cn


<!-- 参考信息 -->