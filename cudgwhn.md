代发 wailian999

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://hu.yuntaijiaju.cn

[S13] C：宏定义
来源：http://ck.shtwfgs.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mv.asd995.cn

[S14] C：枚举
来源：http://ps.nszjky.cn

enum Color { RED, GREEN, BLUE };
来源：http://ov.nicolike.cn

[S15] C：类型转换
来源：http://fp.huanxung.cn

(double) a / b
来源：http://sb.hahajie.cn

[S16] C：位操作置位
来源：http://yv.shxzukj.cn

x |= (1 << 3);
来源：http://he.huanxung.cn

[S17] C：安全拼接字符串
来源：http://il.wgjwhj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://kp.haigaiapp.cn

[S18] C：命令行参数
来源：http://ld.haigaiapp.cn

int main(int argc, char **argv)
来源：http://re.shtwfgs.cn

[S19] C：快速排序
来源：http://va.gzmigu.cn

qsort(a, n, sizeof(int), cmp);
来源：http://fv.shxzukj.cn

[S20] C：二分查找
来源：http://ia.shxzukj.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://kg.nicolike.cn

[S21] C：字符类别判断
来源：http://sv.hahajie.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://uh.asd995.cn

[S22] C：字符串转数字
来源：http://gn.yuexingan06.cn

atoi("42");  strtod("3.14", NULL);
来源：http://hs.huixiangedu.cn

[S23] C：随机数
来源：http://wr.521024.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ru.panjiajie.cn

[S24] C：获取本地时间
来源：http://he.haigaiapp.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://kw.9csxet.cn

[S25] C：内存拷贝
来源：http://bu.bjjhwx.cn

memcpy(dst, src, n);
来源：http://rt.jctech888.com.cn

[S26] C：内存清零
来源：http://oq.shxzskj.cn

memset(a, 0, sizeof a);
来源：http://tf.shtwfgs.cn

[S27] C：定义常量
来源：http://jb.panjiajie.cn

const double PI = 3.14159;
来源：http://zj.wgjwhj.cn

[S28] C：静态变量
来源：http://ds.huanxung.cn

static int counter = 0;
来源：http://kk.newstarts.cn

[S29] C：变参函数
来源：http://nc.haigaiapp.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://qg.chemitech.net.cn

[S30] C：头文件保护
来源：http://hn.shtwfgs.cn

#ifndef X_H
来源：http://ia.haigaiapp.cn

#define X_H
来源：http://dk.huanxung.cn

#endif
来源：http://op.yuntaijiaju.cn

[S31] C++：Hello World
来源：http://wf.huixinmuqiang.cn

#include <iostream>
来源：http://wr.jianghongdianzi.cn

int main() { std::cout << "Hello\n"; }
来源：http://xf.521024.cn

[S32] C++：字符串
来源：http://nf.huixinmuqiang.cn

std::string s = "hi";  s += "!";
来源：http://zp.yuntaijiaju.cn

[S33] C++：vector 增删
来源：http://gw.nszjky.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qu.szsharing.cn

[S34] C++：遍历 vector
来源：http://il.colortex.cn

for (auto &x : v) { std::cout << x; }
来源：http://pz.jianghongdianzi.cn

[S35] C++：map
来源：http://hw.yuntaijiaju.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://nr.huixinmuqiang.cn

[S36] C++：unordered_map
来源：http://mj.jianghongdianzi.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://xc.shxzukj.cn

[S37] C++：set
来源：http://vo.bookmarksfly.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ze.szsharing.cn

[S38] C++：排序
来源：http://zj.hahajie.cn

std::sort(v.begin(), v.end());
来源：http://tx.jctech888.com.cn

[S39] C++：自定义比较器排序
来源：http://xw.shxzskj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://qn.yuntaijiaju.cn

[S40] C++：查找元素
来源：http://rn.huanxung.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ex.huixinmuqiang.cn

[S41] C++：类与构造函数
来源：http://kw.hahajie.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://lj.nicolike.cn

[S42] C++：继承与虚函数
来源：http://jo.521024.cn

class B : public Base { public: void f() override {} };
来源：http://oz.shtwfgs.cn

[S43] C++：智能指针
来源：http://mg.nszjky.cn

auto p = std::make_unique<int>(5);
来源：http://ko.shxzskj.cn

[S44] C++：引用传参
来源：http://tg.nicolike.cn

void inc(int &x) { ++x; }
来源：http://cg.jianghongdianzi.cn

[S45] C++：lambda
来源：http://hw.chemitech.net.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ie.bjjhwx.cn

[S46] C++：函数模板
来源：http://qi.chemitech.net.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wq.muxihuayi.cn

[S47] C++：结构化绑定遍历
来源：http://mx.bookmarksfly.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://jc.colortex.cn

[S48] C++：逐行读文件
来源：http://ic.wgjwhj.cn

std::ifstream in("a.txt");  std::string line;
来源：http://rz.gzmigu.cn

while (std::getline(in, line)) { }
来源：http://fd.newstarts.cn

[S49] C++：写文件
来源：http://gu.hnjuh.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://yv.nicolike.cn

[S50] C++：格式化数字
来源：http://aa.bjjhwx.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://kg.shtwfgs.cn

[S51] C++：显式类型转换
来源：http://gf.huixinmuqiang.cn

static_cast<double>(a) / b
来源：http://cf.bjjhwx.cn

[S52] C++：const 与 noexcept
来源：http://ao.huixiangedu.cn

int size() const noexcept { return n_; }
来源：http://qd.bookmarksfly.cn

[S53] C++：移动语义
来源：http://kw.nicolike.cn

std::vector<int> w = std::move(v);
来源：http://sk.lnxyls.cn

[S54] C++：异常处理
来源：http://qs.bjjhwx.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://jz.jctech888.com.cn

[S55] C++：结构化绑定
来源：http://xz.chemitech.net.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://sj.9csxet.cn

[S56] C++：optional
来源：http://dx.chemitech.net.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hg.nicolike.cn

[S57] C++：编译期常量
来源：http://tg.panjiajie.cn

constexpr int N = 10;
来源：http://bh.bjjhwx.cn

[S58] C++：命名空间
来源：http://tf.asd995.cn

namespace ns { int f() { return 1; } }
来源：http://yk.colortex.cn

[S59] C++：静态断言
来源：http://wb.colortex.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://sc.huixinmuqiang.cn

[S60] C++：遍历并删除元素
来源：http://ib.colortex.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://kl.yuexingan06.cn

================================================================================
来源：http://cn.bookmarksfly.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://uk.yuexingan06.cn

================================================================================
来源：http://wh.huixiangedu.cn

[T01] Kotlin：Hello World
来源：http://yb.bookmarksfly.cn

println("Hello")
来源：http://yz.nszjky.cn

[T02] Kotlin：变量
来源：http://mw.huixinmuqiang.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://xg.shtwfgs.cn

[T03] Kotlin：字符串模板
来源：http://le.nszjky.cn

"值: $b"
来源：http://rm.shtwfgs.cn

[T04] Kotlin：空安全
来源：http://fd.yuntaijiaju.cn

val n: String? = null;  n?.length
来源：http://uc.newstarts.cn

[T05] Kotlin：when 表达式
来源：http://rz.9csxet.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wl.huanxung.cn

[T06] Kotlin：集合映射
来源：http://qj.colortex.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://si.shxzskj.cn

[T07] Kotlin：集合过滤
来源：http://dm.nicolike.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://vy.huanxung.cn

[T08] Kotlin：数据类
来源：http://gy.nszjky.cn

data class User(val name: String, val age: Int)
来源：http://gu.huixinmuqiang.cn

[T09] Kotlin：扩展函数
来源：http://pr.9csxet.cn

fun String.exclaim() = this + "!"
来源：http://zb.yuexingan06.cn

[T10] Kotlin：默认参数
来源：http://je.gzmigu.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://mv.yuexingan06.cn

[T11] Kotlin：协程
来源：http://bp.yuntaijiaju.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://mo.shxzskj.cn

[T12] Kotlin：解构声明
来源：http://zi.colortex.cn

val (a, b) = Pair(1, 2)
来源：http://es.shxzukj.cn

[T13] Kotlin：只读 Map
来源：http://bk.muxihuayi.cn

val m = mapOf("a" to 1)
来源：http://ke.bjjhwx.cn

[T14] Kotlin：循环
来源：http://tq.yuntaijiaju.cn

for (i in 1..10) println(i)
来源：http://ex.panjiajie.cn

[T15] Kotlin：接口
来源：http://eh.muxihuayi.cn

interface Shape { fun area(): Double }
来源：http://ta.haigaiapp.cn

[T16] Swift：Hello World
来源：http://jx.nicolike.cn

print("Hello")
来源：http://uk.huixiangedu.cn

[T17] Swift：变量与常量
来源：http://xg.hnjuh.cn

var a = 1;  let b = 2
来源：http://wz.shxzskj.cn

[T18] Swift：字符串插值
来源：http://ks.szsharing.cn

"值: \(b)"
来源：http://qf.asd995.cn

[T19] Swift：可选绑定
来源：http://jp.szxytkj.cn

if let n = opt { print(n) }
来源：http://ea.colortex.cn

[T20] Swift：数组操作
来源：http://mr.521024.cn

var a = [1, 2, 3];  a.append(4)
来源：http://wd.colortex.cn

[T21] Swift：遍历
来源：http://rh.szsharing.cn

for x in a { print(x) }
来源：http://hn.hnjuh.cn

[T22] Swift：字典
来源：http://ng.muxihuayi.cn

var d = ["a": 1];  d["b"] = 2
来源：http://wk.muxihuayi.cn

[T23] Swift：函数
来源：http://no.hnjuh.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ec.hahajie.cn

[T24] Swift：闭包
来源：http://yu.gzmigu.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://uz.gzmigu.cn

[T25] Swift：结构体
来源：http://ws.chemitech.net.cn

struct P { var x: Int }
来源：http://dv.szsharing.cn

[T26] Swift：类与重写
来源：http://xo.nszjky.cn

class A: Base { override func f() {} }
来源：http://wl.huixinmuqiang.cn

[T27] Swift：错误处理
来源：http://bj.shtwfgs.cn

do { try f() } catch { print(error) }
来源：http://jl.yuexingan06.cn

[T28] Swift：枚举
来源：http://kb.asd995.cn

enum Color { case red, green }
来源：http://mp.gzmigu.cn

[T29] Swift：guard 提前返回
来源：http://dd.yuntaijiaju.cn

guard let x = opt else { return }
来源：http://jo.jianghongdianzi.cn

[T30] Swift：协议
来源：http://fp.panjiajie.cn

protocol Shape { func area() -> Double }
来源：http://lr.nicolike.cn

[T31] Lua：Hello World
来源：http://lf.bookmarksfly.cn

print("Hello")
来源：http://sh.yuexingan06.cn

[T32] Lua：局部变量
来源：http://om.yuexingan06.cn

local a = 1
来源：http://td.huixinmuqiang.cn

[T33] Lua：表（数组）
来源：http://ch.asd995.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ox.newstarts.cn

[T34] Lua：遍历表
来源：http://mo.hnjuh.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://bj.bookmarksfly.cn

[T35] Lua：字典表
来源：http://gi.shxzskj.cn

local d = { a = 1 };  d.b = 2
来源：http://cp.gzmigu.cn

[T36] Lua：函数
来源：http://pj.521024.cn

function add(a, b) return a + b end
来源：http://ij.huixiangedu.cn

[T37] Lua：字符串拼接
来源：http://kd.bjjhwx.cn

"a" .. "b"
来源：http://aw.szsharing.cn

[T38] Lua：条件
来源：http://mw.hahajie.cn

if x > 0 then print("正") end
来源：http://gj.shxzskj.cn

[T39] Lua：模式匹配
来源：http://sv.yuexingan06.cn

string.find(s, "%d+")
来源：http://fi.newstarts.cn

[T40] Lua：元表
来源：http://oc.9csxet.cn

setmetatable({}, { __index = base })
来源：http://pr.haigaiapp.cn

[T41] Perl：Hello World
来源：http://ng.shtwfgs.cn

print "Hello\n";
来源：http://ln.bookmarksfly.cn

[T42] Perl：变量类型
来源：http://wo.panjiajie.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://dp.huixiangedu.cn

[T43] Perl：字符串插值
来源：http://xd.asd995.cn

"值: $a"
来源：http://jl.9csxet.cn

[T44] Perl：条件
来源：http://ey.yuexingan06.cn

if ($a > 0) { print "正"; }
来源：http://hs.bookmarksfly.cn

[T45] Perl：数组遍历
来源：http://zo.yuexingan06.cn

for my $x (@arr) { print $x; }
来源：http://ci.szxytkj.cn

[T46] Perl：哈希操作
来源：http://ss.nszjky.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://pq.yuexingan06.cn

[T47] Perl：正则捕获
来源：http://bv.muxihuayi.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://db.lnxyls.cn

[T48] Perl：正则替换
来源：http://op.shxzskj.cn

$s =~ s/old/new/g;
来源：http://qu.hahajie.cn

[T49] Perl：函数
来源：http://rq.jctech888.com.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://kk.9csxet.cn

[T50] Perl：逐行读文件
来源：http://rg.bookmarksfly.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ei.nszjky.cn

while (my $line = <$fh>) { print $line; }
来源：http://li.shxzskj.cn

[T51] Scala：Hello World
来源：http://er.hnjuh.cn

println("Hello")
来源：http://cq.nicolike.cn

[T52] Scala：变量
来源：http://lj.jctech888.com.cn

val a = 1;  var b = 2
来源：http://ws.bookmarksfly.cn

[T53] Scala：字符串插值
来源：http://xz.huixinmuqiang.cn

s"值: $b"
来源：http://et.wgjwhj.cn

[T54] Scala：集合映射
来源：http://cc.huanxung.cn

List(1, 2, 3).map(_ * 2)
来源：http://wi.nicolike.cn

[T55] Scala：集合过滤
来源：http://bz.9csxet.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ao.huixinmuqiang.cn

[T56] Scala：样例类
来源：http://kc.jianghongdianzi.cn

case class User(name: String, age: Int)
来源：http://li.hnjuh.cn

[T57] Scala：模式匹配
来源：http://ms.nszjky.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ql.shxzskj.cn

[T58] Scala：函数定义
来源：http://uv.newstarts.cn

def add(a: Int, b: Int): Int = a + b
来源：http://bx.bookmarksfly.cn

[T59] Scala：循环
来源：http://vt.szsharing.cn

for (i <- 1 to 10) println(i)
来源：http://dp.newstarts.cn

[T60] Scala：折叠
来源：http://tr.muxihuayi.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://dv.hahajie.cn

================================================================================
来源：http://iy.shtwfgs.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://qe.yuntaijiaju.cn

================================================================================
来源：http://of.yuexingan06.cn

[U01] Py：创建虚拟环境
来源：http://rl.huixiangedu.cn

python -m venv .venv && source .venv/bin/activate
来源：http://jz.shtwfgs.cn

[U02] Py：导出 / 安装依赖
来源：http://pp.huixiangedu.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://gx.jianghongdianzi.cn

[U03] Py：加载 .env 配置
来源：http://gy.hahajie.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://dm.shxzukj.cn

[U04] Py：变量调试打印
来源：http://du.newstarts.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ml.shtwfgs.cn

[U05] Py：列表去重且保序
来源：http://dw.lnxyls.cn

list(dict.fromkeys(arr))
来源：http://pb.panjiajie.cn

[U06] Py：合并两个字典
来源：http://ly.huanxung.cn

{**a, **b}
来源：http://kl.bjjhwx.cn

[U07] Py：反转字典键值
来源：http://vp.muxihuayi.cn

{v: k for k, v in d.items()}
来源：http://qi.huanxung.cn

[U08] Py：展平二维列表
来源：http://bg.huixinmuqiang.cn

[y for x in nested for y in x]
来源：http://oh.chemitech.net.cn

[U09] Py：字典取最大值的键
来源：http://yk.gzmigu.cn

max(d, key=d.get)
来源：http://zn.huixinmuqiang.cn

[U10] Py：按值排序字典
来源：http://gr.yuexingan06.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://qo.lnxyls.cn

[U11] Py：生成器表达式
来源：http://zj.bjjhwx.cn

(x * 2 for x in arr)
来源：http://cv.hnjuh.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ww.szsharing.cn

Counter(arr).most_common(3)
来源：http://el.bookmarksfly.cn

[U13] Py：固定长度队列
来源：http://fo.bookmarksfly.cn

deque(maxlen=10)
来源：http://vu.shxzukj.cn

[U14] Py：分组收集到列表
来源：http://fw.shxzskj.cn

defaultdict(list)
来源：http://qr.asd995.cn

[U15] Py：高精度计时
来源：http://ej.bookmarksfly.cn

t = time.perf_counter()
来源：http://ov.jianghongdianzi.cn

[U16] Py：命令行参数解析
来源：http://nt.huixiangedu.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://iv.shxzskj.cn

[U17] Py：初始化日志
来源：http://xj.shtwfgs.cn

logging.basicConfig(level=logging.INFO)
来源：http://oz.nszjky.cn

[U18] Py：预编译正则
来源：http://ek.bookmarksfly.cn

pat = re.compile(r"\d+")
来源：http://or.shxzukj.cn

[U19] Py：正则替换带回调
来源：http://wm.szsharing.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://tt.asd995.cn

[U20] Py：缓存函数结果
来源：http://of.521024.cn

@functools.lru_cache(maxsize=None)
来源：http://om.bookmarksfly.cn

[U21] Py：自定义上下文管理器
来源：http://zn.bookmarksfly.cn

@contextlib.contextmanager
来源：http://ta.huanxung.cn

[U22] Py：矩阵转置
来源：http://wv.hnjuh.cn

list(zip(*m))
来源：http://qq.jctech888.com.cn

[U23] Py：分块读取大文件
来源：http://rv.gzmigu.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://du.huixinmuqiang.cn

[U24] Py：路径操作
来源：http://ck.521024.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://vn.huanxung.cn

[U25] Py：CSV 按字典读
来源：http://kq.9csxet.cn

csv.DictReader(f)
来源：http://ac.jianghongdianzi.cn

[U26] Py：并发下载
来源：http://gd.panjiajie.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://jt.nszjky.cn

[U27] Py：异步 HTTP
来源：http://ja.chemitech.net.cn

aiohttp.ClientSession() 配合 async with
来源：http://ho.gzmigu.cn

[U28] Py：类型别名
来源：http://uj.newstarts.cn

UserId = int
来源：http://ut.yuntaijiaju.cn

[U29] Py：属性校验
来源：http://di.nszjky.cn

@property 与 @x.setter 配合
来源：http://el.hnjuh.cn

[U30] Py：数据类
来源：http://ml.szxytkj.cn

@dataclass(slots=True)
来源：http://xg.huixiangedu.cn

[U31] Py：单测
来源：http://mv.szsharing.cn

python -m pytest -q
来源：http://gm.colortex.cn

[U32] Py：代码格式化
来源：http://qn.nicolike.cn

ruff format . && ruff check --fix .
来源：http://ft.panjiajie.cn

[U33] Py：打包发布
来源：http://xb.nszjky.cn

python -m build  （依赖 pyproject.toml）
来源：http://ay.hnjuh.cn

[U34] Py：判断编码
来源：http://qj.haigaiapp.cn

chardet.detect(raw)
来源：http://mi.panjiajie.cn

[U35] Py：发送邮件
来源：http://uz.szsharing.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://qh.shxzskj.cn

[U36] Py：定时任务
来源：http://ow.hnjuh.cn

schedule.every(10).minutes.do(job)
来源：http://ol.szsharing.cn


<!-- 参考信息 -->