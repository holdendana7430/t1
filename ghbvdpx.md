代发 wailian999

strlen(s)
来源：http://dt.bookmarksfly.cn

[S06] C：字符串比较
来源：http://iv.szxytkj.cn

strcmp(a, b) == 0
来源：http://st.yuexingan06.cn

[S07] C：数组遍历求和
来源：http://lf.muxihuayi.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wr.asd995.cn

[S08] C：动态内存分配与释放
来源：http://ik.haigaiapp.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hd.hahajie.cn

[S09] C：结构体定义与初始化
来源：http://ju.9csxet.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://np.shxzukj.cn

[S10] C：指针与解引用
来源：http://bn.9csxet.cn

int *p = &a;  *p = 5;
来源：http://hd.jctech888.com.cn

[S11] C：逐行读文件
来源：http://ll.jianghongdianzi.cn

FILE *f = fopen("a.txt", "r");
来源：http://ka.nicolike.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://jy.9csxet.cn

fclose(f);
来源：http://fx.chemitech.net.cn

[S12] C：写文件
来源：http://tu.shxzskj.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://lv.nszjky.cn

[S13] C：宏定义
来源：http://pa.jianghongdianzi.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ic.gzmigu.cn

[S14] C：枚举
来源：http://xu.huixinmuqiang.cn

enum Color { RED, GREEN, BLUE };
来源：http://qe.panjiajie.cn

[S15] C：类型转换
来源：http://jj.9csxet.cn

(double) a / b
来源：http://ks.nicolike.cn

[S16] C：位操作置位
来源：http://re.hahajie.cn

x |= (1 << 3);
来源：http://fe.lnxyls.cn

[S17] C：安全拼接字符串
来源：http://er.hahajie.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://pi.chemitech.net.cn

[S18] C：命令行参数
来源：http://cv.huixiangedu.cn

int main(int argc, char **argv)
来源：http://wc.nicolike.cn

[S19] C：快速排序
来源：http://rp.hahajie.cn

qsort(a, n, sizeof(int), cmp);
来源：http://il.chemitech.net.cn

[S20] C：二分查找
来源：http://tz.jctech888.com.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ca.jctech888.com.cn

[S21] C：字符类别判断
来源：http://fq.szsharing.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://kf.colortex.cn

[S22] C：字符串转数字
来源：http://gc.wgjwhj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://li.szsharing.cn

[S23] C：随机数
来源：http://mw.lnxyls.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://qs.nicolike.cn

[S24] C：获取本地时间
来源：http://xe.bjjhwx.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://pf.hahajie.cn

[S25] C：内存拷贝
来源：http://le.gzmigu.cn

memcpy(dst, src, n);
来源：http://ne.szsharing.cn

[S26] C：内存清零
来源：http://ub.jianghongdianzi.cn

memset(a, 0, sizeof a);
来源：http://su.shxzskj.cn

[S27] C：定义常量
来源：http://rs.9csxet.cn

const double PI = 3.14159;
来源：http://hf.wgjwhj.cn

[S28] C：静态变量
来源：http://eh.jianghongdianzi.cn

static int counter = 0;
来源：http://oz.colortex.cn

[S29] C：变参函数
来源：http://jr.shxzukj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ex.muxihuayi.cn

[S30] C：头文件保护
来源：http://tf.huixiangedu.cn

#ifndef X_H
来源：http://jw.muxihuayi.cn

#define X_H
来源：http://jw.muxihuayi.cn

#endif
来源：http://ne.9csxet.cn

[S31] C++：Hello World
来源：http://ph.hahajie.cn

#include <iostream>
来源：http://vx.panjiajie.cn

int main() { std::cout << "Hello\n"; }
来源：http://uf.huixiangedu.cn

[S32] C++：字符串
来源：http://bj.nszjky.cn

std::string s = "hi";  s += "!";
来源：http://sk.wgjwhj.cn

[S33] C++：vector 增删
来源：http://da.haigaiapp.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://os.gzmigu.cn

[S34] C++：遍历 vector
来源：http://rq.chemitech.net.cn

for (auto &x : v) { std::cout << x; }
来源：http://gz.shxzukj.cn

[S35] C++：map
来源：http://ha.bookmarksfly.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://lm.colortex.cn

[S36] C++：unordered_map
来源：http://lg.haigaiapp.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hu.huanxung.cn

[S37] C++：set
来源：http://yk.huixiangedu.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://rr.shtwfgs.cn

[S38] C++：排序
来源：http://by.521024.cn

std::sort(v.begin(), v.end());
来源：http://lm.muxihuayi.cn

[S39] C++：自定义比较器排序
来源：http://hd.bookmarksfly.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://rp.hnjuh.cn

[S40] C++：查找元素
来源：http://ve.hnjuh.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://bi.wgjwhj.cn

[S41] C++：类与构造函数
来源：http://el.hahajie.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://nq.huixiangedu.cn

[S42] C++：继承与虚函数
来源：http://gx.newstarts.cn

class B : public Base { public: void f() override {} };
来源：http://xt.bookmarksfly.cn

[S43] C++：智能指针
来源：http://wz.bookmarksfly.cn

auto p = std::make_unique<int>(5);
来源：http://ep.muxihuayi.cn

[S44] C++：引用传参
来源：http://tp.wgjwhj.cn

void inc(int &x) { ++x; }
来源：http://tl.newstarts.cn

[S45] C++：lambda
来源：http://lb.shxzskj.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ge.521024.cn

[S46] C++：函数模板
来源：http://pb.panjiajie.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://bc.huixinmuqiang.cn

[S47] C++：结构化绑定遍历
来源：http://jj.bookmarksfly.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://rm.bookmarksfly.cn

[S48] C++：逐行读文件
来源：http://sr.szxytkj.cn

std::ifstream in("a.txt");  std::string line;
来源：http://vp.wgjwhj.cn

while (std::getline(in, line)) { }
来源：http://gh.hahajie.cn

[S49] C++：写文件
来源：http://sr.colortex.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://xb.jctech888.com.cn

[S50] C++：格式化数字
来源：http://is.colortex.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://vg.hahajie.cn

[S51] C++：显式类型转换
来源：http://ky.jianghongdianzi.cn

static_cast<double>(a) / b
来源：http://fl.wgjwhj.cn

[S52] C++：const 与 noexcept
来源：http://sr.jianghongdianzi.cn

int size() const noexcept { return n_; }
来源：http://nh.bjjhwx.cn

[S53] C++：移动语义
来源：http://vk.gzmigu.cn

std::vector<int> w = std::move(v);
来源：http://io.shxzskj.cn

[S54] C++：异常处理
来源：http://fh.asd995.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://lp.newstarts.cn

[S55] C++：结构化绑定
来源：http://oa.bookmarksfly.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://po.jctech888.com.cn

[S56] C++：optional
来源：http://zv.lnxyls.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://yi.huanxung.cn

[S57] C++：编译期常量
来源：http://fw.bjjhwx.cn

constexpr int N = 10;
来源：http://tn.jianghongdianzi.cn

[S58] C++：命名空间
来源：http://cu.hahajie.cn

namespace ns { int f() { return 1; } }
来源：http://fo.hnjuh.cn

[S59] C++：静态断言
来源：http://ki.jianghongdianzi.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://yw.haigaiapp.cn

[S60] C++：遍历并删除元素
来源：http://ih.panjiajie.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ms.wgjwhj.cn

================================================================================
来源：http://jh.hahajie.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://qd.nicolike.cn

================================================================================
来源：http://kn.huixiangedu.cn

[T01] Kotlin：Hello World
来源：http://xs.szsharing.cn

println("Hello")
来源：http://ot.huanxung.cn

[T02] Kotlin：变量
来源：http://gz.bookmarksfly.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://nx.huanxung.cn

[T03] Kotlin：字符串模板
来源：http://lv.panjiajie.cn

"值: $b"
来源：http://fj.jctech888.com.cn

[T04] Kotlin：空安全
来源：http://qx.lnxyls.cn

val n: String? = null;  n?.length
来源：http://cn.huanxung.cn

[T05] Kotlin：when 表达式
来源：http://ks.9csxet.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://sn.shtwfgs.cn

[T06] Kotlin：集合映射
来源：http://ok.szxytkj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ov.muxihuayi.cn

[T07] Kotlin：集合过滤
来源：http://wy.jctech888.com.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://dk.newstarts.cn

[T08] Kotlin：数据类
来源：http://hl.huixinmuqiang.cn

data class User(val name: String, val age: Int)
来源：http://jz.bookmarksfly.cn

[T09] Kotlin：扩展函数
来源：http://wy.9csxet.cn

fun String.exclaim() = this + "!"
来源：http://xx.newstarts.cn

[T10] Kotlin：默认参数
来源：http://wg.hahajie.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://to.yuexingan06.cn

[T11] Kotlin：协程
来源：http://zp.asd995.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ae.hnjuh.cn

[T12] Kotlin：解构声明
来源：http://wd.asd995.cn

val (a, b) = Pair(1, 2)
来源：http://jt.huixiangedu.cn

[T13] Kotlin：只读 Map
来源：http://tt.hnjuh.cn

val m = mapOf("a" to 1)
来源：http://si.yuexingan06.cn

[T14] Kotlin：循环
来源：http://ta.hahajie.cn

for (i in 1..10) println(i)
来源：http://hb.huanxung.cn

[T15] Kotlin：接口
来源：http://hl.szxytkj.cn

interface Shape { fun area(): Double }
来源：http://mt.bjjhwx.cn

[T16] Swift：Hello World
来源：http://yp.nszjky.cn

print("Hello")
来源：http://ks.521024.cn

[T17] Swift：变量与常量
来源：http://tz.521024.cn

var a = 1;  let b = 2
来源：http://oo.panjiajie.cn

[T18] Swift：字符串插值
来源：http://tu.panjiajie.cn

"值: \(b)"
来源：http://rd.nicolike.cn

[T19] Swift：可选绑定
来源：http://nq.shxzskj.cn

if let n = opt { print(n) }
来源：http://ea.szsharing.cn

[T20] Swift：数组操作
来源：http://eg.lnxyls.cn

var a = [1, 2, 3];  a.append(4)
来源：http://zb.huanxung.cn

[T21] Swift：遍历
来源：http://cd.lnxyls.cn

for x in a { print(x) }
来源：http://xh.haigaiapp.cn

[T22] Swift：字典
来源：http://lj.asd995.cn

var d = ["a": 1];  d["b"] = 2
来源：http://af.muxihuayi.cn

[T23] Swift：函数
来源：http://te.asd995.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://xs.nicolike.cn

[T24] Swift：闭包
来源：http://rh.huanxung.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://iu.huixinmuqiang.cn

[T25] Swift：结构体
来源：http://uk.yuntaijiaju.cn

struct P { var x: Int }
来源：http://uq.panjiajie.cn

[T26] Swift：类与重写
来源：http://ng.szxytkj.cn

class A: Base { override func f() {} }
来源：http://xz.jctech888.com.cn

[T27] Swift：错误处理
来源：http://fb.huixinmuqiang.cn

do { try f() } catch { print(error) }
来源：http://uw.huixiangedu.cn

[T28] Swift：枚举
来源：http://ms.newstarts.cn

enum Color { case red, green }
来源：http://bz.newstarts.cn

[T29] Swift：guard 提前返回
来源：http://lu.szsharing.cn

guard let x = opt else { return }
来源：http://as.nszjky.cn

[T30] Swift：协议
来源：http://qt.muxihuayi.cn

protocol Shape { func area() -> Double }
来源：http://kx.szsharing.cn

[T31] Lua：Hello World
来源：http://jj.yuexingan06.cn

print("Hello")
来源：http://nv.lnxyls.cn

[T32] Lua：局部变量
来源：http://wc.hahajie.cn

local a = 1
来源：http://al.shtwfgs.cn

[T33] Lua：表（数组）
来源：http://fb.bjjhwx.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://je.gzmigu.cn

[T34] Lua：遍历表
来源：http://iy.9csxet.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ki.huixiangedu.cn

[T35] Lua：字典表
来源：http://ls.gzmigu.cn

local d = { a = 1 };  d.b = 2
来源：http://dm.huixiangedu.cn

[T36] Lua：函数
来源：http://ie.9csxet.cn

function add(a, b) return a + b end
来源：http://gx.yuexingan06.cn

[T37] Lua：字符串拼接
来源：http://ie.szsharing.cn

"a" .. "b"
来源：http://rv.panjiajie.cn

[T38] Lua：条件
来源：http://ij.newstarts.cn

if x > 0 then print("正") end
来源：http://is.chemitech.net.cn

[T39] Lua：模式匹配
来源：http://ce.newstarts.cn

string.find(s, "%d+")
来源：http://uy.shxzukj.cn

[T40] Lua：元表
来源：http://vd.szxytkj.cn

setmetatable({}, { __index = base })
来源：http://vp.newstarts.cn

[T41] Perl：Hello World
来源：http://dj.nszjky.cn

print "Hello\n";
来源：http://nz.huixinmuqiang.cn

[T42] Perl：变量类型
来源：http://hp.lnxyls.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://na.bookmarksfly.cn

[T43] Perl：字符串插值
来源：http://oa.gzmigu.cn

"值: $a"
来源：http://mw.colortex.cn

[T44] Perl：条件
来源：http://vv.nicolike.cn

if ($a > 0) { print "正"; }
来源：http://mr.colortex.cn

[T45] Perl：数组遍历
来源：http://si.shtwfgs.cn

for my $x (@arr) { print $x; }
来源：http://ig.nicolike.cn

[T46] Perl：哈希操作
来源：http://mu.muxihuayi.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://eg.huixiangedu.cn

[T47] Perl：正则捕获
来源：http://ky.shtwfgs.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ma.wgjwhj.cn

[T48] Perl：正则替换
来源：http://tz.newstarts.cn

$s =~ s/old/new/g;
来源：http://ij.jianghongdianzi.cn

[T49] Perl：函数
来源：http://dt.jianghongdianzi.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://yh.gzmigu.cn

[T50] Perl：逐行读文件
来源：http://im.huixiangedu.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://mn.9csxet.cn

while (my $line = <$fh>) { print $line; }
来源：http://gh.szsharing.cn

[T51] Scala：Hello World
来源：http://vk.shtwfgs.cn

println("Hello")
来源：http://mx.panjiajie.cn

[T52] Scala：变量
来源：http://eb.colortex.cn

val a = 1;  var b = 2
来源：http://rs.gzmigu.cn

[T53] Scala：字符串插值
来源：http://uo.yuntaijiaju.cn

s"值: $b"
来源：http://fy.yuntaijiaju.cn

[T54] Scala：集合映射
来源：http://zu.shxzukj.cn

List(1, 2, 3).map(_ * 2)
来源：http://ol.lnxyls.cn

[T55] Scala：集合过滤
来源：http://za.muxihuayi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://rr.bjjhwx.cn

[T56] Scala：样例类
来源：http://gj.gzmigu.cn

case class User(name: String, age: Int)
来源：http://kl.huixiangedu.cn

[T57] Scala：模式匹配
来源：http://qx.szsharing.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://cv.bookmarksfly.cn

[T58] Scala：函数定义
来源：http://kb.hnjuh.cn

def add(a: Int, b: Int): Int = a + b
来源：http://wa.nszjky.cn

[T59] Scala：循环
来源：http://pc.9csxet.cn

for (i <- 1 to 10) println(i)
来源：http://in.hnjuh.cn

[T60] Scala：折叠
来源：http://br.chemitech.net.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://jm.bjjhwx.cn

================================================================================
来源：http://wg.shtwfgs.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ic.szxytkj.cn

================================================================================
来源：http://yo.hnjuh.cn

[U01] Py：创建虚拟环境
来源：http://bx.panjiajie.cn

python -m venv .venv && source .venv/bin/activate
来源：http://hf.yuntaijiaju.cn

[U02] Py：导出 / 安装依赖
来源：http://ei.yuntaijiaju.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://re.muxihuayi.cn

[U03] Py：加载 .env 配置
来源：http://xj.huixiangedu.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://fo.9csxet.cn

[U04] Py：变量调试打印
来源：http://lg.wgjwhj.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ry.chemitech.net.cn

[U05] Py：列表去重且保序
来源：http://nf.hahajie.cn

list(dict.fromkeys(arr))
来源：http://pk.nszjky.cn

[U06] Py：合并两个字典
来源：http://zi.yuexingan06.cn

{**a, **b}
来源：http://el.wgjwhj.cn

[U07] Py：反转字典键值
来源：http://ql.jctech888.com.cn

{v: k for k, v in d.items()}
来源：http://ym.yuexingan06.cn

[U08] Py：展平二维列表
来源：http://qt.nszjky.cn

[y for x in nested for y in x]
来源：http://gz.shxzskj.cn

[U09] Py：字典取最大值的键
来源：http://ye.jianghongdianzi.cn

max(d, key=d.get)
来源：http://ce.chemitech.net.cn

[U10] Py：按值排序字典
来源：http://ot.hnjuh.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://bl.shxzskj.cn

[U11] Py：生成器表达式
来源：http://hi.jctech888.com.cn

(x * 2 for x in arr)
来源：http://ip.huanxung.cn

[U12] Py：取出现最多的 3 个元素
来源：http://xb.yuexingan06.cn

Counter(arr).most_common(3)
来源：http://gj.shtwfgs.cn

[U13] Py：固定长度队列
来源：http://ys.yuntaijiaju.cn

deque(maxlen=10)
来源：http://kb.newstarts.cn

[U14] Py：分组收集到列表
来源：http://kt.colortex.cn

defaultdict(list)
来源：http://dd.shxzukj.cn

[U15] Py：高精度计时
来源：http://ds.huixiangedu.cn

t = time.perf_counter()
来源：http://hs.newstarts.cn

[U16] Py：命令行参数解析
来源：http://kp.yuntaijiaju.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://vl.jctech888.com.cn

[U17] Py：初始化日志
来源：http://yz.521024.cn

logging.basicConfig(level=logging.INFO)
来源：http://yc.yuexingan06.cn

[U18] Py：预编译正则
来源：http://pk.shxzskj.cn

pat = re.compile(r"\d+")
来源：http://iy.asd995.cn

[U19] Py：正则替换带回调
来源：http://fa.521024.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wi.yuntaijiaju.cn

[U20] Py：缓存函数结果
来源：http://od.chemitech.net.cn

@functools.lru_cache(maxsize=None)
来源：http://fd.9csxet.cn

[U21] Py：自定义上下文管理器
来源：http://ti.jctech888.com.cn

@contextlib.contextmanager
来源：http://vd.shxzskj.cn

[U22] Py：矩阵转置
来源：http://wa.shxzukj.cn

list(zip(*m))
来源：http://fk.asd995.cn

[U23] Py：分块读取大文件
来源：http://bf.chemitech.net.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://mn.521024.cn

[U24] Py：路径操作
来源：http://cd.yuntaijiaju.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mw.hahajie.cn

[U25] Py：CSV 按字典读
来源：http://vs.asd995.cn

csv.DictReader(f)
来源：http://jm.bjjhwx.cn

[U26] Py：并发下载
来源：http://yk.szxytkj.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://xi.huixinmuqiang.cn

[U27] Py：异步 HTTP
来源：http://hm.colortex.cn

aiohttp.ClientSession() 配合 async with
来源：http://pi.chemitech.net.cn

[U28] Py：类型别名
来源：http://cu.jianghongdianzi.cn

UserId = int
来源：http://pn.huixinmuqiang.cn


<!-- 参考信息 -->