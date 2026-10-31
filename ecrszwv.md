代发 wailian999

FILE *f = fopen("a.txt", "r");
来源：http://ad.huanxung.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://vv.szxytkj.cn

fclose(f);
来源：http://pn.gzmigu.cn

[S12] C：写文件
来源：http://eh.huixiangedu.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://gx.chemitech.net.cn

[S13] C：宏定义
来源：http://os.nszjky.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hw.panjiajie.cn

[S14] C：枚举
来源：http://wo.chemitech.net.cn

enum Color { RED, GREEN, BLUE };
来源：http://wz.yuntaijiaju.cn

[S15] C：类型转换
来源：http://in.521024.cn

(double) a / b
来源：http://sr.haigaiapp.cn

[S16] C：位操作置位
来源：http://wa.muxihuayi.cn

x |= (1 << 3);
来源：http://sr.nicolike.cn

[S17] C：安全拼接字符串
来源：http://ed.newstarts.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ry.wgjwhj.cn

[S18] C：命令行参数
来源：http://wc.wgjwhj.cn

int main(int argc, char **argv)
来源：http://wk.szxytkj.cn

[S19] C：快速排序
来源：http://ff.colortex.cn

qsort(a, n, sizeof(int), cmp);
来源：http://dh.shtwfgs.cn

[S20] C：二分查找
来源：http://ax.chemitech.net.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://lw.nszjky.cn

[S21] C：字符类别判断
来源：http://ee.521024.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wd.521024.cn

[S22] C：字符串转数字
来源：http://gl.yuexingan06.cn

atoi("42");  strtod("3.14", NULL);
来源：http://jp.asd995.cn

[S23] C：随机数
来源：http://ca.yuexingan06.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://fn.521024.cn

[S24] C：获取本地时间
来源：http://uz.jianghongdianzi.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mm.hahajie.cn

[S25] C：内存拷贝
来源：http://yl.bookmarksfly.cn

memcpy(dst, src, n);
来源：http://tb.lnxyls.cn

[S26] C：内存清零
来源：http://ey.huanxung.cn

memset(a, 0, sizeof a);
来源：http://tp.yuexingan06.cn

[S27] C：定义常量
来源：http://jc.colortex.cn

const double PI = 3.14159;
来源：http://hq.lnxyls.cn

[S28] C：静态变量
来源：http://oe.bjjhwx.cn

static int counter = 0;
来源：http://mt.yuntaijiaju.cn

[S29] C：变参函数
来源：http://rx.huanxung.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://xq.newstarts.cn

[S30] C：头文件保护
来源：http://bu.bjjhwx.cn

#ifndef X_H
来源：http://hd.szxytkj.cn

#define X_H
来源：http://jh.yuexingan06.cn

#endif
来源：http://rw.panjiajie.cn

[S31] C++：Hello World
来源：http://bp.szxytkj.cn

#include <iostream>
来源：http://vu.9csxet.cn

int main() { std::cout << "Hello\n"; }
来源：http://qc.hnjuh.cn

[S32] C++：字符串
来源：http://ij.gzmigu.cn

std::string s = "hi";  s += "!";
来源：http://ze.wgjwhj.cn

[S33] C++：vector 增删
来源：http://cs.yuexingan06.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wl.chemitech.net.cn

[S34] C++：遍历 vector
来源：http://lq.wgjwhj.cn

for (auto &x : v) { std::cout << x; }
来源：http://xr.huixinmuqiang.cn

[S35] C++：map
来源：http://gr.asd995.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://xo.gzmigu.cn

[S36] C++：unordered_map
来源：http://pm.colortex.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://rp.yuexingan06.cn

[S37] C++：set
来源：http://gq.bjjhwx.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://pi.bookmarksfly.cn

[S38] C++：排序
来源：http://ka.szxytkj.cn

std::sort(v.begin(), v.end());
来源：http://cq.hahajie.cn

[S39] C++：自定义比较器排序
来源：http://ne.9csxet.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://nw.panjiajie.cn

[S40] C++：查找元素
来源：http://oe.huixinmuqiang.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hp.shxzukj.cn

[S41] C++：类与构造函数
来源：http://li.521024.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mg.shxzskj.cn

[S42] C++：继承与虚函数
来源：http://cy.newstarts.cn

class B : public Base { public: void f() override {} };
来源：http://mp.szxytkj.cn

[S43] C++：智能指针
来源：http://ut.wgjwhj.cn

auto p = std::make_unique<int>(5);
来源：http://vj.jianghongdianzi.cn

[S44] C++：引用传参
来源：http://uq.asd995.cn

void inc(int &x) { ++x; }
来源：http://ou.lnxyls.cn

[S45] C++：lambda
来源：http://ox.jctech888.com.cn

auto add = [](int a, int b) { return a + b; };
来源：http://uv.panjiajie.cn

[S46] C++：函数模板
来源：http://pv.nszjky.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://fv.jctech888.com.cn

[S47] C++：结构化绑定遍历
来源：http://uc.shtwfgs.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mh.muxihuayi.cn

[S48] C++：逐行读文件
来源：http://ki.szxytkj.cn

std::ifstream in("a.txt");  std::string line;
来源：http://nz.szsharing.cn

while (std::getline(in, line)) { }
来源：http://qp.huixinmuqiang.cn

[S49] C++：写文件
来源：http://xm.jctech888.com.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://cr.shtwfgs.cn

[S50] C++：格式化数字
来源：http://vr.wgjwhj.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://gk.nicolike.cn

[S51] C++：显式类型转换
来源：http://gf.haigaiapp.cn

static_cast<double>(a) / b
来源：http://fs.asd995.cn

[S52] C++：const 与 noexcept
来源：http://bh.szxytkj.cn

int size() const noexcept { return n_; }
来源：http://qe.9csxet.cn

[S53] C++：移动语义
来源：http://gt.jianghongdianzi.cn

std::vector<int> w = std::move(v);
来源：http://ca.szsharing.cn

[S54] C++：异常处理
来源：http://vy.hnjuh.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wg.bookmarksfly.cn

[S55] C++：结构化绑定
来源：http://sz.lnxyls.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://hh.9csxet.cn

[S56] C++：optional
来源：http://ms.nicolike.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wm.chemitech.net.cn

[S57] C++：编译期常量
来源：http://ly.newstarts.cn

constexpr int N = 10;
来源：http://cb.szsharing.cn

[S58] C++：命名空间
来源：http://wp.jianghongdianzi.cn

namespace ns { int f() { return 1; } }
来源：http://nl.yuexingan06.cn

[S59] C++：静态断言
来源：http://py.hahajie.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://xa.panjiajie.cn

[S60] C++：遍历并删除元素
来源：http://ar.muxihuayi.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://va.yuexingan06.cn

================================================================================
来源：http://jh.shxzskj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://st.shtwfgs.cn

================================================================================
来源：http://ne.huanxung.cn

[T01] Kotlin：Hello World
来源：http://tt.yuntaijiaju.cn

println("Hello")
来源：http://xw.hahajie.cn

[T02] Kotlin：变量
来源：http://hq.shtwfgs.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://uv.newstarts.cn

[T03] Kotlin：字符串模板
来源：http://ns.521024.cn

"值: $b"
来源：http://lm.jctech888.com.cn

[T04] Kotlin：空安全
来源：http://bs.asd995.cn

val n: String? = null;  n?.length
来源：http://yx.nszjky.cn

[T05] Kotlin：when 表达式
来源：http://qg.asd995.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://yr.shxzukj.cn

[T06] Kotlin：集合映射
来源：http://wv.huixinmuqiang.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://rv.huanxung.cn

[T07] Kotlin：集合过滤
来源：http://nr.yuexingan06.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://zg.hahajie.cn

[T08] Kotlin：数据类
来源：http://aw.shxzskj.cn

data class User(val name: String, val age: Int)
来源：http://tu.yuntaijiaju.cn

[T09] Kotlin：扩展函数
来源：http://vn.huixiangedu.cn

fun String.exclaim() = this + "!"
来源：http://il.bjjhwx.cn

[T10] Kotlin：默认参数
来源：http://gq.asd995.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://sj.jianghongdianzi.cn

[T11] Kotlin：协程
来源：http://cf.huanxung.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://gi.yuntaijiaju.cn

[T12] Kotlin：解构声明
来源：http://nt.shxzskj.cn

val (a, b) = Pair(1, 2)
来源：http://wl.shtwfgs.cn

[T13] Kotlin：只读 Map
来源：http://ll.jianghongdianzi.cn

val m = mapOf("a" to 1)
来源：http://tv.jianghongdianzi.cn

[T14] Kotlin：循环
来源：http://gu.huixiangedu.cn

for (i in 1..10) println(i)
来源：http://rj.asd995.cn

[T15] Kotlin：接口
来源：http://ol.9csxet.cn

interface Shape { fun area(): Double }
来源：http://ge.gzmigu.cn

[T16] Swift：Hello World
来源：http://zn.lnxyls.cn

print("Hello")
来源：http://yi.szxytkj.cn

[T17] Swift：变量与常量
来源：http://ua.shxzukj.cn

var a = 1;  let b = 2
来源：http://rj.haigaiapp.cn

[T18] Swift：字符串插值
来源：http://rd.shxzskj.cn

"值: \(b)"
来源：http://sc.yuntaijiaju.cn

[T19] Swift：可选绑定
来源：http://er.chemitech.net.cn

if let n = opt { print(n) }
来源：http://dz.jianghongdianzi.cn

[T20] Swift：数组操作
来源：http://jy.szxytkj.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ql.nicolike.cn

[T21] Swift：遍历
来源：http://lz.szxytkj.cn

for x in a { print(x) }
来源：http://cl.gzmigu.cn

[T22] Swift：字典
来源：http://ll.jctech888.com.cn

var d = ["a": 1];  d["b"] = 2
来源：http://mw.shtwfgs.cn

[T23] Swift：函数
来源：http://ug.shxzukj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://zz.wgjwhj.cn

[T24] Swift：闭包
来源：http://xr.newstarts.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://di.szsharing.cn

[T25] Swift：结构体
来源：http://xr.huanxung.cn

struct P { var x: Int }
来源：http://vo.asd995.cn

[T26] Swift：类与重写
来源：http://oz.colortex.cn

class A: Base { override func f() {} }
来源：http://qk.gzmigu.cn

[T27] Swift：错误处理
来源：http://vd.newstarts.cn

do { try f() } catch { print(error) }
来源：http://lz.szxytkj.cn

[T28] Swift：枚举
来源：http://hh.chemitech.net.cn

enum Color { case red, green }
来源：http://la.521024.cn

[T29] Swift：guard 提前返回
来源：http://dm.chemitech.net.cn

guard let x = opt else { return }
来源：http://rf.szsharing.cn

[T30] Swift：协议
来源：http://qa.szsharing.cn

protocol Shape { func area() -> Double }
来源：http://wm.jianghongdianzi.cn

[T31] Lua：Hello World
来源：http://ip.huanxung.cn

print("Hello")
来源：http://gd.nszjky.cn

[T32] Lua：局部变量
来源：http://ct.haigaiapp.cn

local a = 1
来源：http://ll.nszjky.cn

[T33] Lua：表（数组）
来源：http://fw.haigaiapp.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://wt.szxytkj.cn

[T34] Lua：遍历表
来源：http://lt.9csxet.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://nl.muxihuayi.cn

[T35] Lua：字典表
来源：http://ea.bjjhwx.cn

local d = { a = 1 };  d.b = 2
来源：http://wv.panjiajie.cn

[T36] Lua：函数
来源：http://dl.521024.cn

function add(a, b) return a + b end
来源：http://qu.nicolike.cn

[T37] Lua：字符串拼接
来源：http://hw.colortex.cn

"a" .. "b"
来源：http://wd.wgjwhj.cn

[T38] Lua：条件
来源：http://uy.colortex.cn

if x > 0 then print("正") end
来源：http://ef.jianghongdianzi.cn

[T39] Lua：模式匹配
来源：http://mf.szxytkj.cn

string.find(s, "%d+")
来源：http://xm.szsharing.cn

[T40] Lua：元表
来源：http://wk.panjiajie.cn

setmetatable({}, { __index = base })
来源：http://kb.yuexingan06.cn

[T41] Perl：Hello World
来源：http://hr.jctech888.com.cn

print "Hello\n";
来源：http://rk.gzmigu.cn

[T42] Perl：变量类型
来源：http://wl.szxytkj.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ge.shxzukj.cn

[T43] Perl：字符串插值
来源：http://qz.bookmarksfly.cn

"值: $a"
来源：http://pg.haigaiapp.cn

[T44] Perl：条件
来源：http://nn.chemitech.net.cn

if ($a > 0) { print "正"; }
来源：http://mk.hahajie.cn

[T45] Perl：数组遍历
来源：http://dz.jianghongdianzi.cn

for my $x (@arr) { print $x; }
来源：http://cj.panjiajie.cn

[T46] Perl：哈希操作
来源：http://ja.huanxung.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://rn.nicolike.cn

[T47] Perl：正则捕获
来源：http://ny.wgjwhj.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://wp.huanxung.cn

[T48] Perl：正则替换
来源：http://cw.bjjhwx.cn

$s =~ s/old/new/g;
来源：http://sk.huanxung.cn

[T49] Perl：函数
来源：http://ue.shxzskj.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://we.hnjuh.cn

[T50] Perl：逐行读文件
来源：http://qc.chemitech.net.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ce.huanxung.cn

while (my $line = <$fh>) { print $line; }
来源：http://ev.shxzskj.cn

[T51] Scala：Hello World
来源：http://gd.hahajie.cn

println("Hello")
来源：http://hu.gzmigu.cn

[T52] Scala：变量
来源：http://qo.muxihuayi.cn

val a = 1;  var b = 2
来源：http://uw.bookmarksfly.cn

[T53] Scala：字符串插值
来源：http://ty.bjjhwx.cn

s"值: $b"
来源：http://yl.huixiangedu.cn

[T54] Scala：集合映射
来源：http://uv.nicolike.cn

List(1, 2, 3).map(_ * 2)
来源：http://yk.yuntaijiaju.cn

[T55] Scala：集合过滤
来源：http://tz.9csxet.cn

List(1, 2, 3).filter(_ > 1)
来源：http://qd.nszjky.cn

[T56] Scala：样例类
来源：http://ig.bjjhwx.cn

case class User(name: String, age: Int)
来源：http://lm.newstarts.cn

[T57] Scala：模式匹配
来源：http://au.chemitech.net.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://mq.newstarts.cn

[T58] Scala：函数定义
来源：http://qc.asd995.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ji.9csxet.cn

[T59] Scala：循环
来源：http://cb.asd995.cn

for (i <- 1 to 10) println(i)
来源：http://as.lnxyls.cn

[T60] Scala：折叠
来源：http://kr.hnjuh.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://eq.huixinmuqiang.cn

================================================================================
来源：http://oo.szxytkj.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://km.huixinmuqiang.cn

================================================================================
来源：http://jh.szsharing.cn

[U01] Py：创建虚拟环境
来源：http://wz.nicolike.cn

python -m venv .venv && source .venv/bin/activate
来源：http://hc.yuntaijiaju.cn

[U02] Py：导出 / 安装依赖
来源：http://qx.hnjuh.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://cp.panjiajie.cn

[U03] Py：加载 .env 配置
来源：http://ec.bjjhwx.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://zk.hahajie.cn

[U04] Py：变量调试打印
来源：http://ma.521024.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://yg.haigaiapp.cn

[U05] Py：列表去重且保序
来源：http://ca.bjjhwx.cn

list(dict.fromkeys(arr))
来源：http://fq.szsharing.cn

[U06] Py：合并两个字典
来源：http://fc.nszjky.cn

{**a, **b}
来源：http://mn.newstarts.cn

[U07] Py：反转字典键值
来源：http://fl.bookmarksfly.cn

{v: k for k, v in d.items()}
来源：http://ng.9csxet.cn

[U08] Py：展平二维列表
来源：http://xc.bookmarksfly.cn

[y for x in nested for y in x]
来源：http://ro.nszjky.cn

[U09] Py：字典取最大值的键
来源：http://bo.jctech888.com.cn

max(d, key=d.get)
来源：http://ix.lnxyls.cn

[U10] Py：按值排序字典
来源：http://oe.jianghongdianzi.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ri.shtwfgs.cn

[U11] Py：生成器表达式
来源：http://ee.colortex.cn

(x * 2 for x in arr)
来源：http://oy.yuntaijiaju.cn

[U12] Py：取出现最多的 3 个元素
来源：http://vy.colortex.cn

Counter(arr).most_common(3)
来源：http://le.521024.cn

[U13] Py：固定长度队列
来源：http://hl.huanxung.cn

deque(maxlen=10)
来源：http://tj.9csxet.cn

[U14] Py：分组收集到列表
来源：http://om.hahajie.cn

defaultdict(list)
来源：http://wg.yuntaijiaju.cn

[U15] Py：高精度计时
来源：http://bt.huixinmuqiang.cn

t = time.perf_counter()
来源：http://zz.muxihuayi.cn

[U16] Py：命令行参数解析
来源：http://mg.yuntaijiaju.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://uz.521024.cn

[U17] Py：初始化日志
来源：http://dz.yuntaijiaju.cn

logging.basicConfig(level=logging.INFO)
来源：http://tp.asd995.cn

[U18] Py：预编译正则
来源：http://yq.huixiangedu.cn

pat = re.compile(r"\d+")
来源：http://in.shtwfgs.cn

[U19] Py：正则替换带回调
来源：http://jn.521024.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://gw.bjjhwx.cn

[U20] Py：缓存函数结果
来源：http://fv.hnjuh.cn

@functools.lru_cache(maxsize=None)
来源：http://zh.asd995.cn

[U21] Py：自定义上下文管理器
来源：http://aw.hnjuh.cn

@contextlib.contextmanager
来源：http://qh.panjiajie.cn

[U22] Py：矩阵转置
来源：http://fs.huanxung.cn

list(zip(*m))
来源：http://bh.huixinmuqiang.cn

[U23] Py：分块读取大文件
来源：http://ww.huixiangedu.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://js.yuexingan06.cn

[U24] Py：路径操作
来源：http://jp.chemitech.net.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://af.hahajie.cn

[U25] Py：CSV 按字典读
来源：http://oc.newstarts.cn

csv.DictReader(f)
来源：http://xp.shtwfgs.cn

[U26] Py：并发下载
来源：http://ur.bjjhwx.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://aq.colortex.cn

[U27] Py：异步 HTTP
来源：http://nn.szsharing.cn

aiohttp.ClientSession() 配合 async with
来源：http://fy.chemitech.net.cn

[U28] Py：类型别名
来源：http://lt.szxytkj.cn

UserId = int
来源：http://mi.muxihuayi.cn

[U29] Py：属性校验
来源：http://xs.hahajie.cn

@property 与 @x.setter 配合
来源：http://kk.jctech888.com.cn

[U30] Py：数据类
来源：http://lh.hahajie.cn

@dataclass(slots=True)
来源：http://lj.haigaiapp.cn

[U31] Py：单测
来源：http://wo.nszjky.cn

python -m pytest -q
来源：http://pj.bookmarksfly.cn

[U32] Py：代码格式化
来源：http://eq.colortex.cn

ruff format . && ruff check --fix .
来源：http://qx.huanxung.cn

[U33] Py：打包发布
来源：http://hm.panjiajie.cn

python -m build  （依赖 pyproject.toml）
来源：http://bi.yuexingan06.cn

[U34] Py：判断编码
来源：http://dh.chemitech.net.cn

chardet.detect(raw)
来源：http://ok.haigaiapp.cn


<!-- 参考信息 -->