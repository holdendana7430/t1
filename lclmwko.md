代发 wailian999

int x; scanf("%d", &x);
来源：http://hc.shxzukj.cn

[S04] C：字符串复制
来源：http://pg.hahajie.cn

char dst[32]; strcpy(dst, "hi");
来源：http://bp.bookmarksfly.cn

[S05] C：字符串长度
来源：http://tt.bjjhwx.cn

strlen(s)
来源：http://qk.jctech888.com.cn

[S06] C：字符串比较
来源：http://br.yuexingan06.cn

strcmp(a, b) == 0
来源：http://ki.huanxung.cn

[S07] C：数组遍历求和
来源：http://ov.chemitech.net.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://qc.jianghongdianzi.cn

[S08] C：动态内存分配与释放
来源：http://km.panjiajie.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://mg.nszjky.cn

[S09] C：结构体定义与初始化
来源：http://fc.9csxet.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://qe.szsharing.cn

[S10] C：指针与解引用
来源：http://aw.yuntaijiaju.cn

int *p = &a;  *p = 5;
来源：http://kx.huixinmuqiang.cn

[S11] C：逐行读文件
来源：http://wl.bjjhwx.cn

FILE *f = fopen("a.txt", "r");
来源：http://qy.yuexingan06.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://by.jctech888.com.cn

fclose(f);
来源：http://mx.yuexingan06.cn

[S12] C：写文件
来源：http://ru.colortex.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://bh.9csxet.cn

[S13] C：宏定义
来源：http://qv.yuntaijiaju.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://oz.yuexingan06.cn

[S14] C：枚举
来源：http://ir.gzmigu.cn

enum Color { RED, GREEN, BLUE };
来源：http://qo.muxihuayi.cn

[S15] C：类型转换
来源：http://jc.bjjhwx.cn

(double) a / b
来源：http://gy.bookmarksfly.cn

[S16] C：位操作置位
来源：http://sb.shxzskj.cn

x |= (1 << 3);
来源：http://ko.9csxet.cn

[S17] C：安全拼接字符串
来源：http://th.shxzukj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://lb.jctech888.com.cn

[S18] C：命令行参数
来源：http://nd.haigaiapp.cn

int main(int argc, char **argv)
来源：http://jx.chemitech.net.cn

[S19] C：快速排序
来源：http://ce.jianghongdianzi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ug.bjjhwx.cn

[S20] C：二分查找
来源：http://va.huixiangedu.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hw.lnxyls.cn

[S21] C：字符类别判断
来源：http://ne.9csxet.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wo.huixiangedu.cn

[S22] C：字符串转数字
来源：http://rv.huanxung.cn

atoi("42");  strtod("3.14", NULL);
来源：http://xd.hnjuh.cn

[S23] C：随机数
来源：http://pb.yuexingan06.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://uh.newstarts.cn

[S24] C：获取本地时间
来源：http://gw.szsharing.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://qf.9csxet.cn

[S25] C：内存拷贝
来源：http://en.shxzskj.cn

memcpy(dst, src, n);
来源：http://qq.521024.cn

[S26] C：内存清零
来源：http://yd.9csxet.cn

memset(a, 0, sizeof a);
来源：http://ym.jctech888.com.cn

[S27] C：定义常量
来源：http://um.szxytkj.cn

const double PI = 3.14159;
来源：http://xp.gzmigu.cn

[S28] C：静态变量
来源：http://hp.huixinmuqiang.cn

static int counter = 0;
来源：http://oe.bjjhwx.cn

[S29] C：变参函数
来源：http://pq.chemitech.net.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://fe.haigaiapp.cn

[S30] C：头文件保护
来源：http://mf.bookmarksfly.cn

#ifndef X_H
来源：http://ta.shtwfgs.cn

#define X_H
来源：http://yd.hahajie.cn

#endif
来源：http://gi.gzmigu.cn

[S31] C++：Hello World
来源：http://ev.bookmarksfly.cn

#include <iostream>
来源：http://oo.nszjky.cn

int main() { std::cout << "Hello\n"; }
来源：http://hh.521024.cn

[S32] C++：字符串
来源：http://wl.lnxyls.cn

std::string s = "hi";  s += "!";
来源：http://mq.muxihuayi.cn

[S33] C++：vector 增删
来源：http://ug.lnxyls.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://bz.chemitech.net.cn

[S34] C++：遍历 vector
来源：http://qd.szxytkj.cn

for (auto &x : v) { std::cout << x; }
来源：http://me.nicolike.cn

[S35] C++：map
来源：http://nu.haigaiapp.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://pl.521024.cn

[S36] C++：unordered_map
来源：http://xg.wgjwhj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://vz.chemitech.net.cn

[S37] C++：set
来源：http://vo.haigaiapp.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ar.shxzskj.cn

[S38] C++：排序
来源：http://zk.jctech888.com.cn

std::sort(v.begin(), v.end());
来源：http://bq.hnjuh.cn

[S39] C++：自定义比较器排序
来源：http://ws.jctech888.com.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://pk.yuntaijiaju.cn

[S40] C++：查找元素
来源：http://zw.colortex.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://bw.huixinmuqiang.cn

[S41] C++：类与构造函数
来源：http://jx.shxzukj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://rn.jctech888.com.cn

[S42] C++：继承与虚函数
来源：http://td.chemitech.net.cn

class B : public Base { public: void f() override {} };
来源：http://oo.newstarts.cn

[S43] C++：智能指针
来源：http://ze.jctech888.com.cn

auto p = std::make_unique<int>(5);
来源：http://qs.jianghongdianzi.cn

[S44] C++：引用传参
来源：http://hi.hnjuh.cn

void inc(int &x) { ++x; }
来源：http://hw.colortex.cn

[S45] C++：lambda
来源：http://ph.colortex.cn

auto add = [](int a, int b) { return a + b; };
来源：http://gf.bjjhwx.cn

[S46] C++：函数模板
来源：http://uq.muxihuayi.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ym.szsharing.cn

[S47] C++：结构化绑定遍历
来源：http://np.hnjuh.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ot.nicolike.cn

[S48] C++：逐行读文件
来源：http://ba.9csxet.cn

std::ifstream in("a.txt");  std::string line;
来源：http://je.jianghongdianzi.cn

while (std::getline(in, line)) { }
来源：http://bl.lnxyls.cn

[S49] C++：写文件
来源：http://iw.szsharing.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://sr.chemitech.net.cn

[S50] C++：格式化数字
来源：http://xf.lnxyls.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://in.haigaiapp.cn

[S51] C++：显式类型转换
来源：http://xd.hahajie.cn

static_cast<double>(a) / b
来源：http://pr.hahajie.cn

[S52] C++：const 与 noexcept
来源：http://sp.bookmarksfly.cn

int size() const noexcept { return n_; }
来源：http://af.shtwfgs.cn

[S53] C++：移动语义
来源：http://im.colortex.cn

std::vector<int> w = std::move(v);
来源：http://ob.hahajie.cn

[S54] C++：异常处理
来源：http://if.jctech888.com.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ot.shxzskj.cn

[S55] C++：结构化绑定
来源：http://zw.lnxyls.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://pa.jianghongdianzi.cn

[S56] C++：optional
来源：http://wm.gzmigu.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://uq.newstarts.cn

[S57] C++：编译期常量
来源：http://nd.nszjky.cn

constexpr int N = 10;
来源：http://va.bookmarksfly.cn

[S58] C++：命名空间
来源：http://ks.shtwfgs.cn

namespace ns { int f() { return 1; } }
来源：http://bc.hahajie.cn

[S59] C++：静态断言
来源：http://is.hahajie.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fj.hahajie.cn

[S60] C++：遍历并删除元素
来源：http://nm.newstarts.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://bq.shtwfgs.cn

================================================================================
来源：http://wf.jianghongdianzi.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://lz.jianghongdianzi.cn

================================================================================
来源：http://nq.gzmigu.cn

[T01] Kotlin：Hello World
来源：http://ar.haigaiapp.cn

println("Hello")
来源：http://js.newstarts.cn

[T02] Kotlin：变量
来源：http://gj.hahajie.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://vr.9csxet.cn

[T03] Kotlin：字符串模板
来源：http://cf.muxihuayi.cn

"值: $b"
来源：http://db.shtwfgs.cn

[T04] Kotlin：空安全
来源：http://xr.newstarts.cn

val n: String? = null;  n?.length
来源：http://fo.szxytkj.cn

[T05] Kotlin：when 表达式
来源：http://zj.yuntaijiaju.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://sz.asd995.cn

[T06] Kotlin：集合映射
来源：http://ct.jianghongdianzi.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://mk.yuntaijiaju.cn

[T07] Kotlin：集合过滤
来源：http://ab.colortex.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://wg.nszjky.cn

[T08] Kotlin：数据类
来源：http://oq.szsharing.cn

data class User(val name: String, val age: Int)
来源：http://ya.colortex.cn

[T09] Kotlin：扩展函数
来源：http://oc.huixinmuqiang.cn

fun String.exclaim() = this + "!"
来源：http://ll.nicolike.cn

[T10] Kotlin：默认参数
来源：http://hy.jctech888.com.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://id.szxytkj.cn

[T11] Kotlin：协程
来源：http://hp.hahajie.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://qj.gzmigu.cn

[T12] Kotlin：解构声明
来源：http://wa.hahajie.cn

val (a, b) = Pair(1, 2)
来源：http://lu.hahajie.cn

[T13] Kotlin：只读 Map
来源：http://ey.huanxung.cn

val m = mapOf("a" to 1)
来源：http://tt.9csxet.cn

[T14] Kotlin：循环
来源：http://lz.newstarts.cn

for (i in 1..10) println(i)
来源：http://hq.chemitech.net.cn

[T15] Kotlin：接口
来源：http://le.9csxet.cn

interface Shape { fun area(): Double }
来源：http://yu.asd995.cn

[T16] Swift：Hello World
来源：http://kg.yuntaijiaju.cn

print("Hello")
来源：http://bh.gzmigu.cn

[T17] Swift：变量与常量
来源：http://vl.jctech888.com.cn

var a = 1;  let b = 2
来源：http://bg.yuntaijiaju.cn

[T18] Swift：字符串插值
来源：http://xk.shtwfgs.cn

"值: \(b)"
来源：http://tc.shxzukj.cn

[T19] Swift：可选绑定
来源：http://cg.panjiajie.cn

if let n = opt { print(n) }
来源：http://wr.chemitech.net.cn

[T20] Swift：数组操作
来源：http://wo.yuntaijiaju.cn

var a = [1, 2, 3];  a.append(4)
来源：http://cm.szsharing.cn

[T21] Swift：遍历
来源：http://rd.jctech888.com.cn

for x in a { print(x) }
来源：http://is.lnxyls.cn

[T22] Swift：字典
来源：http://qm.shxzukj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://su.hahajie.cn

[T23] Swift：函数
来源：http://uc.nszjky.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://bo.521024.cn

[T24] Swift：闭包
来源：http://ol.hnjuh.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://kh.lnxyls.cn

[T25] Swift：结构体
来源：http://hd.hnjuh.cn

struct P { var x: Int }
来源：http://om.nicolike.cn

[T26] Swift：类与重写
来源：http://by.wgjwhj.cn

class A: Base { override func f() {} }
来源：http://xb.newstarts.cn

[T27] Swift：错误处理
来源：http://vn.haigaiapp.cn

do { try f() } catch { print(error) }
来源：http://wr.asd995.cn

[T28] Swift：枚举
来源：http://ho.haigaiapp.cn

enum Color { case red, green }
来源：http://fz.shxzskj.cn

[T29] Swift：guard 提前返回
来源：http://in.colortex.cn

guard let x = opt else { return }
来源：http://st.jianghongdianzi.cn

[T30] Swift：协议
来源：http://dr.huixiangedu.cn

protocol Shape { func area() -> Double }
来源：http://rt.521024.cn

[T31] Lua：Hello World
来源：http://lm.hnjuh.cn

print("Hello")
来源：http://mq.jianghongdianzi.cn

[T32] Lua：局部变量
来源：http://um.jctech888.com.cn

local a = 1
来源：http://jb.huixinmuqiang.cn

[T33] Lua：表（数组）
来源：http://ae.szxytkj.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://tr.521024.cn

[T34] Lua：遍历表
来源：http://hh.gzmigu.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ph.gzmigu.cn

[T35] Lua：字典表
来源：http://qk.szsharing.cn

local d = { a = 1 };  d.b = 2
来源：http://qj.nszjky.cn

[T36] Lua：函数
来源：http://jm.hahajie.cn

function add(a, b) return a + b end
来源：http://px.muxihuayi.cn

[T37] Lua：字符串拼接
来源：http://je.muxihuayi.cn

"a" .. "b"
来源：http://ld.newstarts.cn

[T38] Lua：条件
来源：http://rc.jianghongdianzi.cn

if x > 0 then print("正") end
来源：http://fg.yuntaijiaju.cn

[T39] Lua：模式匹配
来源：http://hn.szxytkj.cn

string.find(s, "%d+")
来源：http://hx.nicolike.cn

[T40] Lua：元表
来源：http://fh.szsharing.cn

setmetatable({}, { __index = base })
来源：http://yp.jctech888.com.cn

[T41] Perl：Hello World
来源：http://ww.huixinmuqiang.cn

print "Hello\n";
来源：http://pc.chemitech.net.cn

[T42] Perl：变量类型
来源：http://yr.9csxet.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://he.hahajie.cn

[T43] Perl：字符串插值
来源：http://vn.asd995.cn

"值: $a"
来源：http://xq.nicolike.cn

[T44] Perl：条件
来源：http://or.9csxet.cn

if ($a > 0) { print "正"; }
来源：http://jg.colortex.cn

[T45] Perl：数组遍历
来源：http://uh.szsharing.cn

for my $x (@arr) { print $x; }
来源：http://hv.bookmarksfly.cn

[T46] Perl：哈希操作
来源：http://ei.shxzskj.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wn.muxihuayi.cn

[T47] Perl：正则捕获
来源：http://ii.panjiajie.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://vm.szsharing.cn

[T48] Perl：正则替换
来源：http://lm.muxihuayi.cn

$s =~ s/old/new/g;
来源：http://iu.asd995.cn

[T49] Perl：函数
来源：http://km.shtwfgs.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://vf.9csxet.cn

[T50] Perl：逐行读文件
来源：http://ws.yuntaijiaju.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://rx.asd995.cn

while (my $line = <$fh>) { print $line; }
来源：http://kr.bjjhwx.cn

[T51] Scala：Hello World
来源：http://ng.asd995.cn

println("Hello")
来源：http://oh.bookmarksfly.cn

[T52] Scala：变量
来源：http://bh.521024.cn

val a = 1;  var b = 2
来源：http://kg.shxzukj.cn

[T53] Scala：字符串插值
来源：http://le.hahajie.cn

s"值: $b"
来源：http://ej.bjjhwx.cn

[T54] Scala：集合映射
来源：http://er.colortex.cn

List(1, 2, 3).map(_ * 2)
来源：http://ta.hnjuh.cn

[T55] Scala：集合过滤
来源：http://sx.muxihuayi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://dw.bookmarksfly.cn

[T56] Scala：样例类
来源：http://au.huixinmuqiang.cn

case class User(name: String, age: Int)
来源：http://ti.shxzskj.cn

[T57] Scala：模式匹配
来源：http://gj.nicolike.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://yo.jianghongdianzi.cn

[T58] Scala：函数定义
来源：http://lh.newstarts.cn

def add(a: Int, b: Int): Int = a + b
来源：http://fg.chemitech.net.cn

[T59] Scala：循环
来源：http://nh.wgjwhj.cn

for (i <- 1 to 10) println(i)
来源：http://we.hnjuh.cn

[T60] Scala：折叠
来源：http://he.huixiangedu.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://gh.gzmigu.cn

================================================================================
来源：http://ze.huixiangedu.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mc.nszjky.cn

================================================================================
来源：http://qr.shxzskj.cn

[U01] Py：创建虚拟环境
来源：http://sk.szsharing.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ek.gzmigu.cn

[U02] Py：导出 / 安装依赖
来源：http://ej.gzmigu.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hr.newstarts.cn

[U03] Py：加载 .env 配置
来源：http://fc.nicolike.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://zm.lnxyls.cn

[U04] Py：变量调试打印
来源：http://uq.bookmarksfly.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://zc.bookmarksfly.cn

[U05] Py：列表去重且保序
来源：http://hj.shtwfgs.cn

list(dict.fromkeys(arr))
来源：http://sk.nicolike.cn

[U06] Py：合并两个字典
来源：http://em.hahajie.cn

{**a, **b}
来源：http://ky.9csxet.cn

[U07] Py：反转字典键值
来源：http://kr.haigaiapp.cn

{v: k for k, v in d.items()}
来源：http://bn.chemitech.net.cn

[U08] Py：展平二维列表
来源：http://ej.wgjwhj.cn

[y for x in nested for y in x]
来源：http://eq.bookmarksfly.cn

[U09] Py：字典取最大值的键
来源：http://we.asd995.cn

max(d, key=d.get)
来源：http://rz.shxzukj.cn

[U10] Py：按值排序字典
来源：http://ve.huixiangedu.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://cx.bookmarksfly.cn

[U11] Py：生成器表达式
来源：http://ci.shxzukj.cn

(x * 2 for x in arr)
来源：http://yq.huanxung.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ot.huixiangedu.cn

Counter(arr).most_common(3)
来源：http://ne.muxihuayi.cn

[U13] Py：固定长度队列
来源：http://tf.szsharing.cn

deque(maxlen=10)
来源：http://af.521024.cn

[U14] Py：分组收集到列表
来源：http://kv.hnjuh.cn

defaultdict(list)
来源：http://jb.asd995.cn

[U15] Py：高精度计时
来源：http://rd.szsharing.cn

t = time.perf_counter()
来源：http://cq.nszjky.cn

[U16] Py：命令行参数解析
来源：http://mc.nszjky.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://bf.gzmigu.cn

[U17] Py：初始化日志
来源：http://wi.jianghongdianzi.cn

logging.basicConfig(level=logging.INFO)
来源：http://dj.lnxyls.cn

[U18] Py：预编译正则
来源：http://wh.jianghongdianzi.cn

pat = re.compile(r"\d+")
来源：http://hm.yuexingan06.cn

[U19] Py：正则替换带回调
来源：http://pt.yuntaijiaju.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://qo.huixiangedu.cn

[U20] Py：缓存函数结果
来源：http://qi.haigaiapp.cn

@functools.lru_cache(maxsize=None)
来源：http://mb.shxzskj.cn

[U21] Py：自定义上下文管理器
来源：http://si.chemitech.net.cn

@contextlib.contextmanager
来源：http://ak.9csxet.cn

[U22] Py：矩阵转置
来源：http://hu.shxzukj.cn

list(zip(*m))
来源：http://ls.nszjky.cn

[U23] Py：分块读取大文件
来源：http://xr.bjjhwx.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://rp.9csxet.cn

[U24] Py：路径操作
来源：http://ft.shtwfgs.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://zr.gzmigu.cn

[U25] Py：CSV 按字典读
来源：http://gt.muxihuayi.cn

csv.DictReader(f)
来源：http://cu.9csxet.cn

[U26] Py：并发下载
来源：http://ks.haigaiapp.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://kn.bjjhwx.cn


<!-- 参考信息 -->