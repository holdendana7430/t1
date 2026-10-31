代发 wailian999

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ca.gzmigu.cn

[S13] C：宏定义
来源：http://sj.szsharing.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ij.bookmarksfly.cn

[S14] C：枚举
来源：http://ni.szxytkj.cn

enum Color { RED, GREEN, BLUE };
来源：http://jr.bjjhwx.cn

[S15] C：类型转换
来源：http://cj.nicolike.cn

(double) a / b
来源：http://lg.panjiajie.cn

[S16] C：位操作置位
来源：http://qf.szxytkj.cn

x |= (1 << 3);
来源：http://hh.huixiangedu.cn

[S17] C：安全拼接字符串
来源：http://mk.lnxyls.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://tk.chemitech.net.cn

[S18] C：命令行参数
来源：http://aw.shxzskj.cn

int main(int argc, char **argv)
来源：http://hs.huixinmuqiang.cn

[S19] C：快速排序
来源：http://qm.9csxet.cn

qsort(a, n, sizeof(int), cmp);
来源：http://kz.521024.cn

[S20] C：二分查找
来源：http://kw.shxzukj.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://gj.huixinmuqiang.cn

[S21] C：字符类别判断
来源：http://wo.shxzukj.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://za.wgjwhj.cn

[S22] C：字符串转数字
来源：http://ar.hnjuh.cn

atoi("42");  strtod("3.14", NULL);
来源：http://tn.bookmarksfly.cn

[S23] C：随机数
来源：http://ki.szxytkj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://bk.hahajie.cn

[S24] C：获取本地时间
来源：http://yr.jctech888.com.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://pj.bookmarksfly.cn

[S25] C：内存拷贝
来源：http://gr.shtwfgs.cn

memcpy(dst, src, n);
来源：http://fe.huanxung.cn

[S26] C：内存清零
来源：http://bz.huanxung.cn

memset(a, 0, sizeof a);
来源：http://cl.panjiajie.cn

[S27] C：定义常量
来源：http://tq.gzmigu.cn

const double PI = 3.14159;
来源：http://hp.asd995.cn

[S28] C：静态变量
来源：http://ny.yuntaijiaju.cn

static int counter = 0;
来源：http://yi.bookmarksfly.cn

[S29] C：变参函数
来源：http://rj.asd995.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://um.lnxyls.cn

[S30] C：头文件保护
来源：http://qq.yuntaijiaju.cn

#ifndef X_H
来源：http://co.yuntaijiaju.cn

#define X_H
来源：http://ml.shxzskj.cn

#endif
来源：http://ew.shxzskj.cn

[S31] C++：Hello World
来源：http://yu.gzmigu.cn

#include <iostream>
来源：http://qz.szsharing.cn

int main() { std::cout << "Hello\n"; }
来源：http://xt.szxytkj.cn

[S32] C++：字符串
来源：http://zl.yuntaijiaju.cn

std::string s = "hi";  s += "!";
来源：http://fs.colortex.cn

[S33] C++：vector 增删
来源：http://ep.szxytkj.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ug.yuexingan06.cn

[S34] C++：遍历 vector
来源：http://rc.haigaiapp.cn

for (auto &x : v) { std::cout << x; }
来源：http://xz.panjiajie.cn

[S35] C++：map
来源：http://yb.bookmarksfly.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://aw.gzmigu.cn

[S36] C++：unordered_map
来源：http://jc.shtwfgs.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ux.yuntaijiaju.cn

[S37] C++：set
来源：http://zg.bookmarksfly.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://vr.nszjky.cn

[S38] C++：排序
来源：http://rx.huanxung.cn

std::sort(v.begin(), v.end());
来源：http://ao.huixiangedu.cn

[S39] C++：自定义比较器排序
来源：http://pn.shxzukj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://sf.jianghongdianzi.cn

[S40] C++：查找元素
来源：http://xr.nszjky.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://zh.wgjwhj.cn

[S41] C++：类与构造函数
来源：http://eu.szsharing.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://oa.colortex.cn

[S42] C++：继承与虚函数
来源：http://lh.nicolike.cn

class B : public Base { public: void f() override {} };
来源：http://be.szxytkj.cn

[S43] C++：智能指针
来源：http://xk.yuntaijiaju.cn

auto p = std::make_unique<int>(5);
来源：http://cz.9csxet.cn

[S44] C++：引用传参
来源：http://rt.nicolike.cn

void inc(int &x) { ++x; }
来源：http://ls.chemitech.net.cn

[S45] C++：lambda
来源：http://js.panjiajie.cn

auto add = [](int a, int b) { return a + b; };
来源：http://gn.hnjuh.cn

[S46] C++：函数模板
来源：http://si.hnjuh.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xf.huixinmuqiang.cn

[S47] C++：结构化绑定遍历
来源：http://qi.szxytkj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://vx.yuexingan06.cn

[S48] C++：逐行读文件
来源：http://qd.yuntaijiaju.cn

std::ifstream in("a.txt");  std::string line;
来源：http://mj.panjiajie.cn

while (std::getline(in, line)) { }
来源：http://qu.hnjuh.cn

[S49] C++：写文件
来源：http://ct.shtwfgs.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ta.haigaiapp.cn

[S50] C++：格式化数字
来源：http://kt.nicolike.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://de.shxzskj.cn

[S51] C++：显式类型转换
来源：http://wg.shtwfgs.cn

static_cast<double>(a) / b
来源：http://uc.shtwfgs.cn

[S52] C++：const 与 noexcept
来源：http://of.yuexingan06.cn

int size() const noexcept { return n_; }
来源：http://xf.9csxet.cn

[S53] C++：移动语义
来源：http://hc.jianghongdianzi.cn

std::vector<int> w = std::move(v);
来源：http://lu.hahajie.cn

[S54] C++：异常处理
来源：http://re.nicolike.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hb.nszjky.cn

[S55] C++：结构化绑定
来源：http://bp.jianghongdianzi.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://jc.newstarts.cn

[S56] C++：optional
来源：http://jk.colortex.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ih.hahajie.cn

[S57] C++：编译期常量
来源：http://yq.newstarts.cn

constexpr int N = 10;
来源：http://sa.wgjwhj.cn

[S58] C++：命名空间
来源：http://ky.521024.cn

namespace ns { int f() { return 1; } }
来源：http://cu.9csxet.cn

[S59] C++：静态断言
来源：http://hz.szsharing.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://pn.panjiajie.cn

[S60] C++：遍历并删除元素
来源：http://sz.chemitech.net.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://yt.chemitech.net.cn

================================================================================
来源：http://yx.haigaiapp.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://km.asd995.cn

================================================================================
来源：http://qg.521024.cn

[T01] Kotlin：Hello World
来源：http://zv.lnxyls.cn

println("Hello")
来源：http://sj.bjjhwx.cn

[T02] Kotlin：变量
来源：http://fn.chemitech.net.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ct.9csxet.cn

[T03] Kotlin：字符串模板
来源：http://oj.521024.cn

"值: $b"
来源：http://gv.nicolike.cn

[T04] Kotlin：空安全
来源：http://fu.nicolike.cn

val n: String? = null;  n?.length
来源：http://zp.9csxet.cn

[T05] Kotlin：when 表达式
来源：http://im.chemitech.net.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://sc.nszjky.cn

[T06] Kotlin：集合映射
来源：http://wz.shxzskj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ux.shxzskj.cn

[T07] Kotlin：集合过滤
来源：http://bk.nicolike.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://hc.asd995.cn

[T08] Kotlin：数据类
来源：http://gx.szxytkj.cn

data class User(val name: String, val age: Int)
来源：http://ld.huixinmuqiang.cn

[T09] Kotlin：扩展函数
来源：http://bb.bookmarksfly.cn

fun String.exclaim() = this + "!"
来源：http://uw.shtwfgs.cn

[T10] Kotlin：默认参数
来源：http://qk.lnxyls.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ip.szxytkj.cn

[T11] Kotlin：协程
来源：http://ho.chemitech.net.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://gu.wgjwhj.cn

[T12] Kotlin：解构声明
来源：http://om.hahajie.cn

val (a, b) = Pair(1, 2)
来源：http://ja.hahajie.cn

[T13] Kotlin：只读 Map
来源：http://ke.newstarts.cn

val m = mapOf("a" to 1)
来源：http://sq.jianghongdianzi.cn

[T14] Kotlin：循环
来源：http://ag.bjjhwx.cn

for (i in 1..10) println(i)
来源：http://sz.hahajie.cn

[T15] Kotlin：接口
来源：http://sx.jianghongdianzi.cn

interface Shape { fun area(): Double }
来源：http://lw.bookmarksfly.cn

[T16] Swift：Hello World
来源：http://hy.nicolike.cn

print("Hello")
来源：http://en.huanxung.cn

[T17] Swift：变量与常量
来源：http://ox.yuexingan06.cn

var a = 1;  let b = 2
来源：http://bu.panjiajie.cn

[T18] Swift：字符串插值
来源：http://nu.huanxung.cn

"值: \(b)"
来源：http://pw.colortex.cn

[T19] Swift：可选绑定
来源：http://wn.shxzukj.cn

if let n = opt { print(n) }
来源：http://yo.hahajie.cn

[T20] Swift：数组操作
来源：http://om.nszjky.cn

var a = [1, 2, 3];  a.append(4)
来源：http://as.jctech888.com.cn

[T21] Swift：遍历
来源：http://mk.colortex.cn

for x in a { print(x) }
来源：http://pv.huanxung.cn

[T22] Swift：字典
来源：http://bu.shxzukj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://fw.szsharing.cn

[T23] Swift：函数
来源：http://bx.jianghongdianzi.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://wz.yuexingan06.cn

[T24] Swift：闭包
来源：http://qm.muxihuayi.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://mu.jctech888.com.cn

[T25] Swift：结构体
来源：http://ep.newstarts.cn

struct P { var x: Int }
来源：http://yl.szxytkj.cn

[T26] Swift：类与重写
来源：http://tn.bjjhwx.cn

class A: Base { override func f() {} }
来源：http://lu.9csxet.cn

[T27] Swift：错误处理
来源：http://db.bjjhwx.cn

do { try f() } catch { print(error) }
来源：http://jn.huixinmuqiang.cn

[T28] Swift：枚举
来源：http://gs.yuexingan06.cn

enum Color { case red, green }
来源：http://lv.hnjuh.cn

[T29] Swift：guard 提前返回
来源：http://wr.huixiangedu.cn

guard let x = opt else { return }
来源：http://vp.yuexingan06.cn

[T30] Swift：协议
来源：http://zr.szsharing.cn

protocol Shape { func area() -> Double }
来源：http://km.yuexingan06.cn

[T31] Lua：Hello World
来源：http://tu.gzmigu.cn

print("Hello")
来源：http://ql.haigaiapp.cn

[T32] Lua：局部变量
来源：http://nm.bookmarksfly.cn

local a = 1
来源：http://iq.asd995.cn

[T33] Lua：表（数组）
来源：http://pn.9csxet.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ze.521024.cn

[T34] Lua：遍历表
来源：http://gy.haigaiapp.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://xh.muxihuayi.cn

[T35] Lua：字典表
来源：http://on.huixinmuqiang.cn

local d = { a = 1 };  d.b = 2
来源：http://ub.hnjuh.cn

[T36] Lua：函数
来源：http://lm.hahajie.cn

function add(a, b) return a + b end
来源：http://rn.hahajie.cn

[T37] Lua：字符串拼接
来源：http://yc.chemitech.net.cn

"a" .. "b"
来源：http://gg.asd995.cn

[T38] Lua：条件
来源：http://fd.yuexingan06.cn

if x > 0 then print("正") end
来源：http://xv.huixiangedu.cn

[T39] Lua：模式匹配
来源：http://mf.huixinmuqiang.cn

string.find(s, "%d+")
来源：http://ha.9csxet.cn

[T40] Lua：元表
来源：http://zx.shtwfgs.cn

setmetatable({}, { __index = base })
来源：http://wt.9csxet.cn

[T41] Perl：Hello World
来源：http://lq.wgjwhj.cn

print "Hello\n";
来源：http://rv.bjjhwx.cn

[T42] Perl：变量类型
来源：http://zo.colortex.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://fu.yuntaijiaju.cn

[T43] Perl：字符串插值
来源：http://fs.521024.cn

"值: $a"
来源：http://ln.muxihuayi.cn

[T44] Perl：条件
来源：http://cc.yuexingan06.cn

if ($a > 0) { print "正"; }
来源：http://bd.lnxyls.cn

[T45] Perl：数组遍历
来源：http://fh.panjiajie.cn

for my $x (@arr) { print $x; }
来源：http://li.wgjwhj.cn

[T46] Perl：哈希操作
来源：http://sx.shtwfgs.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://sp.shxzskj.cn

[T47] Perl：正则捕获
来源：http://fi.shxzskj.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://jl.huixiangedu.cn

[T48] Perl：正则替换
来源：http://ej.9csxet.cn

$s =~ s/old/new/g;
来源：http://uc.bookmarksfly.cn

[T49] Perl：函数
来源：http://od.panjiajie.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://pe.wgjwhj.cn

[T50] Perl：逐行读文件
来源：http://hi.521024.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ft.asd995.cn

while (my $line = <$fh>) { print $line; }
来源：http://cw.haigaiapp.cn

[T51] Scala：Hello World
来源：http://ap.yuntaijiaju.cn

println("Hello")
来源：http://lp.asd995.cn

[T52] Scala：变量
来源：http://fp.bookmarksfly.cn

val a = 1;  var b = 2
来源：http://mq.muxihuayi.cn

[T53] Scala：字符串插值
来源：http://bd.asd995.cn

s"值: $b"
来源：http://kn.muxihuayi.cn

[T54] Scala：集合映射
来源：http://oj.chemitech.net.cn

List(1, 2, 3).map(_ * 2)
来源：http://yw.9csxet.cn

[T55] Scala：集合过滤
来源：http://dg.shxzukj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://rn.wgjwhj.cn

[T56] Scala：样例类
来源：http://xq.hahajie.cn

case class User(name: String, age: Int)
来源：http://de.huixinmuqiang.cn

[T57] Scala：模式匹配
来源：http://hk.huixiangedu.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://jc.szxytkj.cn

[T58] Scala：函数定义
来源：http://bk.shxzukj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://fp.jctech888.com.cn

[T59] Scala：循环
来源：http://zw.muxihuayi.cn

for (i <- 1 to 10) println(i)
来源：http://ot.chemitech.net.cn

[T60] Scala：折叠
来源：http://oa.shtwfgs.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://iy.szsharing.cn

================================================================================
来源：http://wn.huixiangedu.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://te.lnxyls.cn

================================================================================
来源：http://os.jianghongdianzi.cn

[U01] Py：创建虚拟环境
来源：http://vc.shxzukj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://jy.521024.cn

[U02] Py：导出 / 安装依赖
来源：http://yo.jctech888.com.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://il.bookmarksfly.cn

[U03] Py：加载 .env 配置
来源：http://ph.muxihuayi.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://sk.shtwfgs.cn

[U04] Py：变量调试打印
来源：http://ux.bjjhwx.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://nx.newstarts.cn

[U05] Py：列表去重且保序
来源：http://bi.shtwfgs.cn

list(dict.fromkeys(arr))
来源：http://zh.chemitech.net.cn

[U06] Py：合并两个字典
来源：http://bj.9csxet.cn

{**a, **b}
来源：http://iq.bookmarksfly.cn

[U07] Py：反转字典键值
来源：http://en.shtwfgs.cn

{v: k for k, v in d.items()}
来源：http://sn.shtwfgs.cn

[U08] Py：展平二维列表
来源：http://sh.shxzskj.cn

[y for x in nested for y in x]
来源：http://mn.huixinmuqiang.cn

[U09] Py：字典取最大值的键
来源：http://nf.huixinmuqiang.cn

max(d, key=d.get)
来源：http://dv.newstarts.cn

[U10] Py：按值排序字典
来源：http://ws.bookmarksfly.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ao.521024.cn

[U11] Py：生成器表达式
来源：http://db.shxzskj.cn

(x * 2 for x in arr)
来源：http://lk.jianghongdianzi.cn

[U12] Py：取出现最多的 3 个元素
来源：http://tg.asd995.cn

Counter(arr).most_common(3)
来源：http://mz.yuntaijiaju.cn

[U13] Py：固定长度队列
来源：http://wo.hnjuh.cn

deque(maxlen=10)
来源：http://sd.jianghongdianzi.cn

[U14] Py：分组收集到列表
来源：http://cy.haigaiapp.cn

defaultdict(list)
来源：http://zj.shxzskj.cn

[U15] Py：高精度计时
来源：http://ow.panjiajie.cn

t = time.perf_counter()
来源：http://km.newstarts.cn

[U16] Py：命令行参数解析
来源：http://rp.yuntaijiaju.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ot.nszjky.cn

[U17] Py：初始化日志
来源：http://hl.521024.cn

logging.basicConfig(level=logging.INFO)
来源：http://qr.huixiangedu.cn

[U18] Py：预编译正则
来源：http://uj.gzmigu.cn

pat = re.compile(r"\d+")
来源：http://wf.wgjwhj.cn

[U19] Py：正则替换带回调
来源：http://rg.lnxyls.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ap.yuexingan06.cn

[U20] Py：缓存函数结果
来源：http://iq.szsharing.cn

@functools.lru_cache(maxsize=None)
来源：http://we.szxytkj.cn

[U21] Py：自定义上下文管理器
来源：http://sb.9csxet.cn

@contextlib.contextmanager
来源：http://hd.colortex.cn

[U22] Py：矩阵转置
来源：http://lo.9csxet.cn

list(zip(*m))
来源：http://eo.chemitech.net.cn

[U23] Py：分块读取大文件
来源：http://rr.lnxyls.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://jv.wgjwhj.cn

[U24] Py：路径操作
来源：http://nv.szxytkj.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://da.hahajie.cn

[U25] Py：CSV 按字典读
来源：http://os.gzmigu.cn

csv.DictReader(f)
来源：http://qh.shxzskj.cn

[U26] Py：并发下载
来源：http://bm.huanxung.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://bd.yuntaijiaju.cn

[U27] Py：异步 HTTP
来源：http://iq.bjjhwx.cn

aiohttp.ClientSession() 配合 async with
来源：http://pa.bjjhwx.cn

[U28] Py：类型别名
来源：http://ih.haigaiapp.cn

UserId = int
来源：http://qh.hahajie.cn

[U29] Py：属性校验
来源：http://fr.huixiangedu.cn

@property 与 @x.setter 配合
来源：http://uo.shxzskj.cn

[U30] Py：数据类
来源：http://xh.huanxung.cn

@dataclass(slots=True)
来源：http://tm.hnjuh.cn

[U31] Py：单测
来源：http://xw.huanxung.cn

python -m pytest -q
来源：http://xe.bookmarksfly.cn

[U32] Py：代码格式化
来源：http://af.szsharing.cn

ruff format . && ruff check --fix .
来源：http://ip.shtwfgs.cn

[U33] Py：打包发布
来源：http://ff.shxzukj.cn

python -m build  （依赖 pyproject.toml）
来源：http://kg.shtwfgs.cn

[U34] Py：判断编码
来源：http://qp.shxzukj.cn

chardet.detect(raw)
来源：http://rd.szsharing.cn

[U35] Py：发送邮件
来源：http://ao.521024.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://tw.wgjwhj.cn

[U36] Py：定时任务
来源：http://wa.huixinmuqiang.cn

schedule.every(10).minutes.do(job)
来源：http://cl.panjiajie.cn


<!-- 参考信息 -->