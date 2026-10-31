代发 wailian999

FILE *f = fopen("a.txt", "r");
来源：http://kp.bookmarksfly.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://xw.bjjhwx.cn

fclose(f);
来源：http://tv.szsharing.cn

[S12] C：写文件
来源：http://tq.shtwfgs.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://dg.haigaiapp.cn

[S13] C：宏定义
来源：http://la.hahajie.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://dv.szsharing.cn

[S14] C：枚举
来源：http://pa.yuntaijiaju.cn

enum Color { RED, GREEN, BLUE };
来源：http://cw.jianghongdianzi.cn

[S15] C：类型转换
来源：http://en.yuntaijiaju.cn

(double) a / b
来源：http://wi.yuntaijiaju.cn

[S16] C：位操作置位
来源：http://zn.szsharing.cn

x |= (1 << 3);
来源：http://wp.szxytkj.cn

[S17] C：安全拼接字符串
来源：http://mq.huixinmuqiang.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://zo.jianghongdianzi.cn

[S18] C：命令行参数
来源：http://xy.nicolike.cn

int main(int argc, char **argv)
来源：http://jg.wgjwhj.cn

[S19] C：快速排序
来源：http://sh.nszjky.cn

qsort(a, n, sizeof(int), cmp);
来源：http://gs.gzmigu.cn

[S20] C：二分查找
来源：http://tm.asd995.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://oz.szxytkj.cn

[S21] C：字符类别判断
来源：http://vt.newstarts.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xy.muxihuayi.cn

[S22] C：字符串转数字
来源：http://gq.colortex.cn

atoi("42");  strtod("3.14", NULL);
来源：http://cu.huanxung.cn

[S23] C：随机数
来源：http://ym.szsharing.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://sq.jianghongdianzi.cn

[S24] C：获取本地时间
来源：http://jd.yuexingan06.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://sb.shxzukj.cn

[S25] C：内存拷贝
来源：http://yn.yuexingan06.cn

memcpy(dst, src, n);
来源：http://mc.huixinmuqiang.cn

[S26] C：内存清零
来源：http://sk.szxytkj.cn

memset(a, 0, sizeof a);
来源：http://de.newstarts.cn

[S27] C：定义常量
来源：http://hd.jctech888.com.cn

const double PI = 3.14159;
来源：http://ur.szsharing.cn

[S28] C：静态变量
来源：http://gt.jianghongdianzi.cn

static int counter = 0;
来源：http://hf.huixinmuqiang.cn

[S29] C：变参函数
来源：http://fs.lnxyls.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://og.colortex.cn

[S30] C：头文件保护
来源：http://ih.nszjky.cn

#ifndef X_H
来源：http://up.9csxet.cn

#define X_H
来源：http://yq.bjjhwx.cn

#endif
来源：http://px.nicolike.cn

[S31] C++：Hello World
来源：http://wn.nszjky.cn

#include <iostream>
来源：http://tk.szxytkj.cn

int main() { std::cout << "Hello\n"; }
来源：http://gn.colortex.cn

[S32] C++：字符串
来源：http://ad.lnxyls.cn

std::string s = "hi";  s += "!";
来源：http://rh.521024.cn

[S33] C++：vector 增删
来源：http://tt.shxzskj.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://zu.bookmarksfly.cn

[S34] C++：遍历 vector
来源：http://ph.haigaiapp.cn

for (auto &x : v) { std::cout << x; }
来源：http://rj.huanxung.cn

[S35] C++：map
来源：http://nb.bjjhwx.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://zl.wgjwhj.cn

[S36] C++：unordered_map
来源：http://qa.gzmigu.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ms.lnxyls.cn

[S37] C++：set
来源：http://ji.chemitech.net.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ai.haigaiapp.cn

[S38] C++：排序
来源：http://se.9csxet.cn

std::sort(v.begin(), v.end());
来源：http://ff.9csxet.cn

[S39] C++：自定义比较器排序
来源：http://rk.521024.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://be.521024.cn

[S40] C++：查找元素
来源：http://nm.newstarts.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://in.gzmigu.cn

[S41] C++：类与构造函数
来源：http://ei.yuntaijiaju.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://og.szxytkj.cn

[S42] C++：继承与虚函数
来源：http://gy.hahajie.cn

class B : public Base { public: void f() override {} };
来源：http://ud.nicolike.cn

[S43] C++：智能指针
来源：http://bg.jianghongdianzi.cn

auto p = std::make_unique<int>(5);
来源：http://do.9csxet.cn

[S44] C++：引用传参
来源：http://yj.yuexingan06.cn

void inc(int &x) { ++x; }
来源：http://rl.521024.cn

[S45] C++：lambda
来源：http://rn.muxihuayi.cn

auto add = [](int a, int b) { return a + b; };
来源：http://xp.haigaiapp.cn

[S46] C++：函数模板
来源：http://rs.nicolike.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ul.bjjhwx.cn

[S47] C++：结构化绑定遍历
来源：http://ip.asd995.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://jt.yuntaijiaju.cn

[S48] C++：逐行读文件
来源：http://qg.hahajie.cn

std::ifstream in("a.txt");  std::string line;
来源：http://vy.huixinmuqiang.cn

while (std::getline(in, line)) { }
来源：http://bg.colortex.cn

[S49] C++：写文件
来源：http://ya.9csxet.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://os.haigaiapp.cn

[S50] C++：格式化数字
来源：http://jv.9csxet.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://gr.bjjhwx.cn

[S51] C++：显式类型转换
来源：http://wm.shtwfgs.cn

static_cast<double>(a) / b
来源：http://gt.hnjuh.cn

[S52] C++：const 与 noexcept
来源：http://yr.9csxet.cn

int size() const noexcept { return n_; }
来源：http://ae.9csxet.cn

[S53] C++：移动语义
来源：http://xi.521024.cn

std::vector<int> w = std::move(v);
来源：http://re.nszjky.cn

[S54] C++：异常处理
来源：http://nl.hahajie.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://sz.shxzskj.cn

[S55] C++：结构化绑定
来源：http://nc.huixinmuqiang.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://pr.wgjwhj.cn

[S56] C++：optional
来源：http://bd.jianghongdianzi.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ul.nicolike.cn

[S57] C++：编译期常量
来源：http://cq.szsharing.cn

constexpr int N = 10;
来源：http://mj.muxihuayi.cn

[S58] C++：命名空间
来源：http://xk.haigaiapp.cn

namespace ns { int f() { return 1; } }
来源：http://yf.newstarts.cn

[S59] C++：静态断言
来源：http://ir.shxzukj.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ha.huanxung.cn

[S60] C++：遍历并删除元素
来源：http://cd.bjjhwx.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ba.yuexingan06.cn

================================================================================
来源：http://us.haigaiapp.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://qm.wgjwhj.cn

================================================================================
来源：http://kv.huixinmuqiang.cn

[T01] Kotlin：Hello World
来源：http://tm.jianghongdianzi.cn

println("Hello")
来源：http://wt.newstarts.cn

[T02] Kotlin：变量
来源：http://jw.chemitech.net.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://fr.haigaiapp.cn

[T03] Kotlin：字符串模板
来源：http://yf.jianghongdianzi.cn

"值: $b"
来源：http://sp.panjiajie.cn

[T04] Kotlin：空安全
来源：http://kx.panjiajie.cn

val n: String? = null;  n?.length
来源：http://xz.bjjhwx.cn

[T05] Kotlin：when 表达式
来源：http://gm.hnjuh.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ni.bjjhwx.cn

[T06] Kotlin：集合映射
来源：http://ac.panjiajie.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ee.chemitech.net.cn

[T07] Kotlin：集合过滤
来源：http://uw.hnjuh.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://rg.yuexingan06.cn

[T08] Kotlin：数据类
来源：http://ni.chemitech.net.cn

data class User(val name: String, val age: Int)
来源：http://qt.bookmarksfly.cn

[T09] Kotlin：扩展函数
来源：http://ar.9csxet.cn

fun String.exclaim() = this + "!"
来源：http://kv.nicolike.cn

[T10] Kotlin：默认参数
来源：http://vo.hnjuh.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://hk.jctech888.com.cn

[T11] Kotlin：协程
来源：http://tz.szsharing.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ou.colortex.cn

[T12] Kotlin：解构声明
来源：http://ww.szsharing.cn

val (a, b) = Pair(1, 2)
来源：http://jq.hnjuh.cn

[T13] Kotlin：只读 Map
来源：http://bi.yuntaijiaju.cn

val m = mapOf("a" to 1)
来源：http://yc.huanxung.cn

[T14] Kotlin：循环
来源：http://lw.huixiangedu.cn

for (i in 1..10) println(i)
来源：http://bf.asd995.cn

[T15] Kotlin：接口
来源：http://kd.shtwfgs.cn

interface Shape { fun area(): Double }
来源：http://if.gzmigu.cn

[T16] Swift：Hello World
来源：http://sb.newstarts.cn

print("Hello")
来源：http://ck.nszjky.cn

[T17] Swift：变量与常量
来源：http://es.chemitech.net.cn

var a = 1;  let b = 2
来源：http://nx.hahajie.cn

[T18] Swift：字符串插值
来源：http://md.521024.cn

"值: \(b)"
来源：http://gf.szxytkj.cn

[T19] Swift：可选绑定
来源：http://nl.bookmarksfly.cn

if let n = opt { print(n) }
来源：http://iz.jianghongdianzi.cn

[T20] Swift：数组操作
来源：http://yt.shtwfgs.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ip.jctech888.com.cn

[T21] Swift：遍历
来源：http://tg.colortex.cn

for x in a { print(x) }
来源：http://ow.wgjwhj.cn

[T22] Swift：字典
来源：http://ev.yuexingan06.cn

var d = ["a": 1];  d["b"] = 2
来源：http://wb.hahajie.cn

[T23] Swift：函数
来源：http://mg.huixiangedu.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://cq.chemitech.net.cn

[T24] Swift：闭包
来源：http://fv.jctech888.com.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://mx.bookmarksfly.cn

[T25] Swift：结构体
来源：http://pb.bjjhwx.cn

struct P { var x: Int }
来源：http://px.huanxung.cn

[T26] Swift：类与重写
来源：http://zq.wgjwhj.cn

class A: Base { override func f() {} }
来源：http://gt.hahajie.cn

[T27] Swift：错误处理
来源：http://qc.yuexingan06.cn

do { try f() } catch { print(error) }
来源：http://an.huixinmuqiang.cn

[T28] Swift：枚举
来源：http://ca.hnjuh.cn

enum Color { case red, green }
来源：http://do.jctech888.com.cn

[T29] Swift：guard 提前返回
来源：http://qh.wgjwhj.cn

guard let x = opt else { return }
来源：http://pg.bjjhwx.cn

[T30] Swift：协议
来源：http://ip.panjiajie.cn

protocol Shape { func area() -> Double }
来源：http://gg.huixiangedu.cn

[T31] Lua：Hello World
来源：http://mw.panjiajie.cn

print("Hello")
来源：http://dm.newstarts.cn

[T32] Lua：局部变量
来源：http://jn.jianghongdianzi.cn

local a = 1
来源：http://bt.yuntaijiaju.cn

[T33] Lua：表（数组）
来源：http://dp.9csxet.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ru.shxzukj.cn

[T34] Lua：遍历表
来源：http://nt.shtwfgs.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://uq.shxzukj.cn

[T35] Lua：字典表
来源：http://eb.521024.cn

local d = { a = 1 };  d.b = 2
来源：http://xz.newstarts.cn

[T36] Lua：函数
来源：http://hc.muxihuayi.cn

function add(a, b) return a + b end
来源：http://th.jctech888.com.cn

[T37] Lua：字符串拼接
来源：http://sj.haigaiapp.cn

"a" .. "b"
来源：http://fi.hnjuh.cn

[T38] Lua：条件
来源：http://hj.shxzskj.cn

if x > 0 then print("正") end
来源：http://nb.huanxung.cn

[T39] Lua：模式匹配
来源：http://jf.muxihuayi.cn

string.find(s, "%d+")
来源：http://iq.huixinmuqiang.cn

[T40] Lua：元表
来源：http://cs.jctech888.com.cn

setmetatable({}, { __index = base })
来源：http://of.huixinmuqiang.cn

[T41] Perl：Hello World
来源：http://cj.bookmarksfly.cn

print "Hello\n";
来源：http://xi.bookmarksfly.cn

[T42] Perl：变量类型
来源：http://jt.hahajie.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://pf.yuexingan06.cn

[T43] Perl：字符串插值
来源：http://pi.jctech888.com.cn

"值: $a"
来源：http://ua.colortex.cn

[T44] Perl：条件
来源：http://bv.huixinmuqiang.cn

if ($a > 0) { print "正"; }
来源：http://di.521024.cn

[T45] Perl：数组遍历
来源：http://sa.szxytkj.cn

for my $x (@arr) { print $x; }
来源：http://yp.yuexingan06.cn

[T46] Perl：哈希操作
来源：http://wa.haigaiapp.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://bu.asd995.cn

[T47] Perl：正则捕获
来源：http://pq.shtwfgs.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://sp.shtwfgs.cn

[T48] Perl：正则替换
来源：http://qn.jctech888.com.cn

$s =~ s/old/new/g;
来源：http://sb.szsharing.cn

[T49] Perl：函数
来源：http://jv.szxytkj.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hc.huixiangedu.cn

[T50] Perl：逐行读文件
来源：http://id.bjjhwx.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://bu.wgjwhj.cn

while (my $line = <$fh>) { print $line; }
来源：http://ta.gzmigu.cn

[T51] Scala：Hello World
来源：http://np.shtwfgs.cn

println("Hello")
来源：http://cc.colortex.cn

[T52] Scala：变量
来源：http://oc.nszjky.cn

val a = 1;  var b = 2
来源：http://mb.lnxyls.cn

[T53] Scala：字符串插值
来源：http://fw.nszjky.cn

s"值: $b"
来源：http://se.bookmarksfly.cn

[T54] Scala：集合映射
来源：http://vp.asd995.cn

List(1, 2, 3).map(_ * 2)
来源：http://oi.jianghongdianzi.cn

[T55] Scala：集合过滤
来源：http://pl.asd995.cn

List(1, 2, 3).filter(_ > 1)
来源：http://wd.newstarts.cn

[T56] Scala：样例类
来源：http://yi.yuntaijiaju.cn

case class User(name: String, age: Int)
来源：http://pf.bookmarksfly.cn

[T57] Scala：模式匹配
来源：http://aw.bjjhwx.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://jo.asd995.cn

[T58] Scala：函数定义
来源：http://tt.hahajie.cn

def add(a: Int, b: Int): Int = a + b
来源：http://sc.szsharing.cn

[T59] Scala：循环
来源：http://ed.gzmigu.cn

for (i <- 1 to 10) println(i)
来源：http://sh.nicolike.cn

[T60] Scala：折叠
来源：http://di.shtwfgs.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://nc.szxytkj.cn

================================================================================
来源：http://og.szsharing.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wd.asd995.cn

================================================================================
来源：http://ia.huixinmuqiang.cn

[U01] Py：创建虚拟环境
来源：http://gh.huanxung.cn

python -m venv .venv && source .venv/bin/activate
来源：http://qf.yuexingan06.cn

[U02] Py：导出 / 安装依赖
来源：http://al.nszjky.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://pt.muxihuayi.cn

[U03] Py：加载 .env 配置
来源：http://hy.bjjhwx.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ci.muxihuayi.cn

[U04] Py：变量调试打印
来源：http://rl.muxihuayi.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hk.shxzskj.cn

[U05] Py：列表去重且保序
来源：http://bg.muxihuayi.cn

list(dict.fromkeys(arr))
来源：http://xm.wgjwhj.cn

[U06] Py：合并两个字典
来源：http://gu.nicolike.cn

{**a, **b}
来源：http://ei.colortex.cn

[U07] Py：反转字典键值
来源：http://ge.panjiajie.cn

{v: k for k, v in d.items()}
来源：http://wc.lnxyls.cn

[U08] Py：展平二维列表
来源：http://cr.szsharing.cn

[y for x in nested for y in x]
来源：http://zx.chemitech.net.cn

[U09] Py：字典取最大值的键
来源：http://fz.yuexingan06.cn

max(d, key=d.get)
来源：http://wk.haigaiapp.cn

[U10] Py：按值排序字典
来源：http://ej.huixiangedu.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://hf.gzmigu.cn

[U11] Py：生成器表达式
来源：http://vw.bjjhwx.cn

(x * 2 for x in arr)
来源：http://ie.haigaiapp.cn

[U12] Py：取出现最多的 3 个元素
来源：http://fd.asd995.cn

Counter(arr).most_common(3)
来源：http://zc.521024.cn

[U13] Py：固定长度队列
来源：http://xz.521024.cn

deque(maxlen=10)
来源：http://rg.521024.cn

[U14] Py：分组收集到列表
来源：http://bv.gzmigu.cn

defaultdict(list)
来源：http://ij.szsharing.cn

[U15] Py：高精度计时
来源：http://fm.szsharing.cn

t = time.perf_counter()
来源：http://gg.jianghongdianzi.cn

[U16] Py：命令行参数解析
来源：http://xm.shxzskj.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ao.yuntaijiaju.cn

[U17] Py：初始化日志
来源：http://vt.yuntaijiaju.cn

logging.basicConfig(level=logging.INFO)
来源：http://xz.yuntaijiaju.cn

[U18] Py：预编译正则
来源：http://vb.huixinmuqiang.cn

pat = re.compile(r"\d+")
来源：http://bc.muxihuayi.cn

[U19] Py：正则替换带回调
来源：http://qd.panjiajie.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://va.haigaiapp.cn

[U20] Py：缓存函数结果
来源：http://gk.chemitech.net.cn

@functools.lru_cache(maxsize=None)
来源：http://uv.shxzskj.cn

[U21] Py：自定义上下文管理器
来源：http://sg.shtwfgs.cn

@contextlib.contextmanager
来源：http://ng.asd995.cn

[U22] Py：矩阵转置
来源：http://du.shxzukj.cn

list(zip(*m))
来源：http://yb.lnxyls.cn

[U23] Py：分块读取大文件
来源：http://cv.colortex.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://qv.huixiangedu.cn

[U24] Py：路径操作
来源：http://xg.bookmarksfly.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://tc.bookmarksfly.cn

[U25] Py：CSV 按字典读
来源：http://vf.colortex.cn

csv.DictReader(f)
来源：http://ss.bjjhwx.cn

[U26] Py：并发下载
来源：http://sc.nicolike.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ce.9csxet.cn

[U27] Py：异步 HTTP
来源：http://dp.yuntaijiaju.cn

aiohttp.ClientSession() 配合 async with
来源：http://bx.nszjky.cn

[U28] Py：类型别名
来源：http://yr.jctech888.com.cn

UserId = int
来源：http://by.nszjky.cn

[U29] Py：属性校验
来源：http://ce.huixinmuqiang.cn

@property 与 @x.setter 配合
来源：http://zy.hahajie.cn

[U30] Py：数据类
来源：http://ao.lnxyls.cn

@dataclass(slots=True)
来源：http://az.huixiangedu.cn

[U31] Py：单测
来源：http://fg.yuntaijiaju.cn

python -m pytest -q
来源：http://if.muxihuayi.cn

[U32] Py：代码格式化
来源：http://ls.jctech888.com.cn

ruff format . && ruff check --fix .
来源：http://eo.huixinmuqiang.cn

[U33] Py：打包发布
来源：http://di.asd995.cn

python -m build  （依赖 pyproject.toml）
来源：http://sa.hahajie.cn

[U34] Py：判断编码
来源：http://az.shxzskj.cn

chardet.detect(raw)
来源：http://gh.gzmigu.cn


<!-- 参考信息 -->