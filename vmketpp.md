代发 wailian999

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ea.521024.cn

[S13] C：宏定义
来源：http://rl.nszjky.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ih.huanxung.cn

[S14] C：枚举
来源：http://zy.wgjwhj.cn

enum Color { RED, GREEN, BLUE };
来源：http://bw.jctech888.com.cn

[S15] C：类型转换
来源：http://bu.hnjuh.cn

(double) a / b
来源：http://wv.colortex.cn

[S16] C：位操作置位
来源：http://qu.haigaiapp.cn

x |= (1 << 3);
来源：http://ik.9csxet.cn

[S17] C：安全拼接字符串
来源：http://gq.nicolike.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://pj.jianghongdianzi.cn

[S18] C：命令行参数
来源：http://nv.panjiajie.cn

int main(int argc, char **argv)
来源：http://kp.bookmarksfly.cn

[S19] C：快速排序
来源：http://er.jianghongdianzi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ej.jianghongdianzi.cn

[S20] C：二分查找
来源：http://rj.huixinmuqiang.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://tl.shxzukj.cn

[S21] C：字符类别判断
来源：http://oo.jianghongdianzi.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://zy.asd995.cn

[S22] C：字符串转数字
来源：http://tx.muxihuayi.cn

atoi("42");  strtod("3.14", NULL);
来源：http://cd.shtwfgs.cn

[S23] C：随机数
来源：http://kq.jctech888.com.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://jm.lnxyls.cn

[S24] C：获取本地时间
来源：http://go.bjjhwx.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://li.shxzskj.cn

[S25] C：内存拷贝
来源：http://ph.newstarts.cn

memcpy(dst, src, n);
来源：http://fh.nszjky.cn

[S26] C：内存清零
来源：http://sh.haigaiapp.cn

memset(a, 0, sizeof a);
来源：http://jo.nszjky.cn

[S27] C：定义常量
来源：http://yw.shxzskj.cn

const double PI = 3.14159;
来源：http://an.hahajie.cn

[S28] C：静态变量
来源：http://ua.panjiajie.cn

static int counter = 0;
来源：http://sw.haigaiapp.cn

[S29] C：变参函数
来源：http://av.szxytkj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hm.szsharing.cn

[S30] C：头文件保护
来源：http://mv.lnxyls.cn

#ifndef X_H
来源：http://pg.yuntaijiaju.cn

#define X_H
来源：http://ee.huixiangedu.cn

#endif
来源：http://ep.panjiajie.cn

[S31] C++：Hello World
来源：http://wk.panjiajie.cn

#include <iostream>
来源：http://nk.shxzskj.cn

int main() { std::cout << "Hello\n"; }
来源：http://pj.wgjwhj.cn

[S32] C++：字符串
来源：http://ly.haigaiapp.cn

std::string s = "hi";  s += "!";
来源：http://hp.shxzukj.cn

[S33] C++：vector 增删
来源：http://im.huixinmuqiang.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://jd.bjjhwx.cn

[S34] C++：遍历 vector
来源：http://ou.shxzukj.cn

for (auto &x : v) { std::cout << x; }
来源：http://kt.shxzskj.cn

[S35] C++：map
来源：http://ei.szsharing.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hc.521024.cn

[S36] C++：unordered_map
来源：http://uh.gzmigu.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://wf.panjiajie.cn

[S37] C++：set
来源：http://tt.huanxung.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://uq.yuntaijiaju.cn

[S38] C++：排序
来源：http://pt.muxihuayi.cn

std::sort(v.begin(), v.end());
来源：http://ir.nszjky.cn

[S39] C++：自定义比较器排序
来源：http://kj.haigaiapp.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://an.shxzskj.cn

[S40] C++：查找元素
来源：http://xe.shxzskj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://et.szxytkj.cn

[S41] C++：类与构造函数
来源：http://pt.bjjhwx.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://nu.hahajie.cn

[S42] C++：继承与虚函数
来源：http://pu.hahajie.cn

class B : public Base { public: void f() override {} };
来源：http://ld.szsharing.cn

[S43] C++：智能指针
来源：http://nz.shxzukj.cn

auto p = std::make_unique<int>(5);
来源：http://ky.haigaiapp.cn

[S44] C++：引用传参
来源：http://xw.shxzukj.cn

void inc(int &x) { ++x; }
来源：http://mx.shxzskj.cn

[S45] C++：lambda
来源：http://cu.gzmigu.cn

auto add = [](int a, int b) { return a + b; };
来源：http://wb.panjiajie.cn

[S46] C++：函数模板
来源：http://cm.jianghongdianzi.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://qz.huanxung.cn

[S47] C++：结构化绑定遍历
来源：http://lq.nicolike.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://jt.hnjuh.cn

[S48] C++：逐行读文件
来源：http://ar.nszjky.cn

std::ifstream in("a.txt");  std::string line;
来源：http://nm.521024.cn

while (std::getline(in, line)) { }
来源：http://sd.nicolike.cn

[S49] C++：写文件
来源：http://fr.bjjhwx.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://vb.jctech888.com.cn

[S50] C++：格式化数字
来源：http://uk.shxzukj.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hv.nszjky.cn

[S51] C++：显式类型转换
来源：http://gr.szsharing.cn

static_cast<double>(a) / b
来源：http://mu.panjiajie.cn

[S52] C++：const 与 noexcept
来源：http://ex.9csxet.cn

int size() const noexcept { return n_; }
来源：http://nj.521024.cn

[S53] C++：移动语义
来源：http://mo.szsharing.cn

std::vector<int> w = std::move(v);
来源：http://dm.huixinmuqiang.cn

[S54] C++：异常处理
来源：http://sd.shxzskj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://cc.nszjky.cn

[S55] C++：结构化绑定
来源：http://hq.nicolike.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ev.521024.cn

[S56] C++：optional
来源：http://ox.shtwfgs.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://zb.yuexingan06.cn

[S57] C++：编译期常量
来源：http://qw.chemitech.net.cn

constexpr int N = 10;
来源：http://ee.newstarts.cn

[S58] C++：命名空间
来源：http://ab.nicolike.cn

namespace ns { int f() { return 1; } }
来源：http://md.szxytkj.cn

[S59] C++：静态断言
来源：http://qx.bookmarksfly.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://gh.shtwfgs.cn

[S60] C++：遍历并删除元素
来源：http://mt.szsharing.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://qu.yuexingan06.cn

================================================================================
来源：http://kt.colortex.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://jp.hnjuh.cn

================================================================================
来源：http://mo.huanxung.cn

[T01] Kotlin：Hello World
来源：http://hy.huixinmuqiang.cn

println("Hello")
来源：http://ls.521024.cn

[T02] Kotlin：变量
来源：http://sj.jctech888.com.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://bu.szxytkj.cn

[T03] Kotlin：字符串模板
来源：http://xv.panjiajie.cn

"值: $b"
来源：http://eo.hnjuh.cn

[T04] Kotlin：空安全
来源：http://fz.panjiajie.cn

val n: String? = null;  n?.length
来源：http://rv.muxihuayi.cn

[T05] Kotlin：when 表达式
来源：http://rx.jianghongdianzi.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://cm.chemitech.net.cn

[T06] Kotlin：集合映射
来源：http://zk.9csxet.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://yj.bookmarksfly.cn

[T07] Kotlin：集合过滤
来源：http://by.colortex.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://yn.asd995.cn

[T08] Kotlin：数据类
来源：http://zg.muxihuayi.cn

data class User(val name: String, val age: Int)
来源：http://wg.yuntaijiaju.cn

[T09] Kotlin：扩展函数
来源：http://mm.lnxyls.cn

fun String.exclaim() = this + "!"
来源：http://yn.nicolike.cn

[T10] Kotlin：默认参数
来源：http://tv.huixiangedu.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://fh.huixinmuqiang.cn

[T11] Kotlin：协程
来源：http://ng.szxytkj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://lc.nszjky.cn

[T12] Kotlin：解构声明
来源：http://ew.shtwfgs.cn

val (a, b) = Pair(1, 2)
来源：http://eh.muxihuayi.cn

[T13] Kotlin：只读 Map
来源：http://kq.colortex.cn

val m = mapOf("a" to 1)
来源：http://fm.panjiajie.cn

[T14] Kotlin：循环
来源：http://tr.bjjhwx.cn

for (i in 1..10) println(i)
来源：http://dq.hnjuh.cn

[T15] Kotlin：接口
来源：http://nx.gzmigu.cn

interface Shape { fun area(): Double }
来源：http://dg.gzmigu.cn

[T16] Swift：Hello World
来源：http://uc.szsharing.cn

print("Hello")
来源：http://se.chemitech.net.cn

[T17] Swift：变量与常量
来源：http://np.gzmigu.cn

var a = 1;  let b = 2
来源：http://hq.newstarts.cn

[T18] Swift：字符串插值
来源：http://lk.521024.cn

"值: \(b)"
来源：http://vb.jianghongdianzi.cn

[T19] Swift：可选绑定
来源：http://xr.shtwfgs.cn

if let n = opt { print(n) }
来源：http://wy.huixinmuqiang.cn

[T20] Swift：数组操作
来源：http://do.newstarts.cn

var a = [1, 2, 3];  a.append(4)
来源：http://vg.521024.cn

[T21] Swift：遍历
来源：http://ae.shxzukj.cn

for x in a { print(x) }
来源：http://ic.huixinmuqiang.cn

[T22] Swift：字典
来源：http://kc.hnjuh.cn

var d = ["a": 1];  d["b"] = 2
来源：http://rn.haigaiapp.cn

[T23] Swift：函数
来源：http://hh.shtwfgs.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://du.jianghongdianzi.cn

[T24] Swift：闭包
来源：http://ft.hahajie.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://mg.lnxyls.cn

[T25] Swift：结构体
来源：http://en.colortex.cn

struct P { var x: Int }
来源：http://yr.521024.cn

[T26] Swift：类与重写
来源：http://hx.hnjuh.cn

class A: Base { override func f() {} }
来源：http://jz.lnxyls.cn

[T27] Swift：错误处理
来源：http://pl.newstarts.cn

do { try f() } catch { print(error) }
来源：http://dg.gzmigu.cn

[T28] Swift：枚举
来源：http://dz.newstarts.cn

enum Color { case red, green }
来源：http://tt.9csxet.cn

[T29] Swift：guard 提前返回
来源：http://rs.nszjky.cn

guard let x = opt else { return }
来源：http://kn.hnjuh.cn

[T30] Swift：协议
来源：http://wh.yuexingan06.cn

protocol Shape { func area() -> Double }
来源：http://us.szsharing.cn

[T31] Lua：Hello World
来源：http://wb.newstarts.cn

print("Hello")
来源：http://tv.huanxung.cn

[T32] Lua：局部变量
来源：http://gu.jctech888.com.cn

local a = 1
来源：http://ag.bookmarksfly.cn

[T33] Lua：表（数组）
来源：http://bv.lnxyls.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ce.huanxung.cn

[T34] Lua：遍历表
来源：http://zy.shtwfgs.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://vu.jctech888.com.cn

[T35] Lua：字典表
来源：http://hp.shxzskj.cn

local d = { a = 1 };  d.b = 2
来源：http://my.newstarts.cn

[T36] Lua：函数
来源：http://pn.chemitech.net.cn

function add(a, b) return a + b end
来源：http://rb.jctech888.com.cn

[T37] Lua：字符串拼接
来源：http://lk.hnjuh.cn

"a" .. "b"
来源：http://pm.huanxung.cn

[T38] Lua：条件
来源：http://wz.wgjwhj.cn

if x > 0 then print("正") end
来源：http://hc.jianghongdianzi.cn

[T39] Lua：模式匹配
来源：http://bm.nicolike.cn

string.find(s, "%d+")
来源：http://pg.bjjhwx.cn

[T40] Lua：元表
来源：http://la.gzmigu.cn

setmetatable({}, { __index = base })
来源：http://hg.wgjwhj.cn

[T41] Perl：Hello World
来源：http://lc.lnxyls.cn

print "Hello\n";
来源：http://hp.colortex.cn

[T42] Perl：变量类型
来源：http://dg.yuntaijiaju.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://zz.colortex.cn

[T43] Perl：字符串插值
来源：http://sp.panjiajie.cn

"值: $a"
来源：http://kd.hahajie.cn

[T44] Perl：条件
来源：http://tg.9csxet.cn

if ($a > 0) { print "正"; }
来源：http://df.haigaiapp.cn

[T45] Perl：数组遍历
来源：http://jb.bjjhwx.cn

for my $x (@arr) { print $x; }
来源：http://gs.jianghongdianzi.cn

[T46] Perl：哈希操作
来源：http://jk.newstarts.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ml.lnxyls.cn

[T47] Perl：正则捕获
来源：http://fq.haigaiapp.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://qi.chemitech.net.cn

[T48] Perl：正则替换
来源：http://or.panjiajie.cn

$s =~ s/old/new/g;
来源：http://hr.shxzskj.cn

[T49] Perl：函数
来源：http://if.9csxet.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://go.bjjhwx.cn

[T50] Perl：逐行读文件
来源：http://gp.lnxyls.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ql.lnxyls.cn

while (my $line = <$fh>) { print $line; }
来源：http://mk.9csxet.cn

[T51] Scala：Hello World
来源：http://qd.chemitech.net.cn

println("Hello")
来源：http://cl.nszjky.cn

[T52] Scala：变量
来源：http://lr.jctech888.com.cn

val a = 1;  var b = 2
来源：http://qs.hahajie.cn

[T53] Scala：字符串插值
来源：http://eb.hnjuh.cn

s"值: $b"
来源：http://or.gzmigu.cn

[T54] Scala：集合映射
来源：http://qr.jianghongdianzi.cn

List(1, 2, 3).map(_ * 2)
来源：http://vs.bjjhwx.cn

[T55] Scala：集合过滤
来源：http://xk.521024.cn

List(1, 2, 3).filter(_ > 1)
来源：http://cl.nszjky.cn

[T56] Scala：样例类
来源：http://zn.jianghongdianzi.cn

case class User(name: String, age: Int)
来源：http://as.bookmarksfly.cn

[T57] Scala：模式匹配
来源：http://yv.hnjuh.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://od.chemitech.net.cn

[T58] Scala：函数定义
来源：http://sg.newstarts.cn

def add(a: Int, b: Int): Int = a + b
来源：http://gi.szxytkj.cn

[T59] Scala：循环
来源：http://hj.yuntaijiaju.cn

for (i <- 1 to 10) println(i)
来源：http://pa.nszjky.cn

[T60] Scala：折叠
来源：http://ok.hahajie.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://np.szxytkj.cn

================================================================================
来源：http://hp.9csxet.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ai.muxihuayi.cn

================================================================================
来源：http://gc.yuntaijiaju.cn

[U01] Py：创建虚拟环境
来源：http://qr.lnxyls.cn

python -m venv .venv && source .venv/bin/activate
来源：http://qb.shxzskj.cn

[U02] Py：导出 / 安装依赖
来源：http://hc.chemitech.net.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://fi.huixiangedu.cn

[U03] Py：加载 .env 配置
来源：http://sv.jctech888.com.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://se.gzmigu.cn

[U04] Py：变量调试打印
来源：http://ki.muxihuayi.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://lx.chemitech.net.cn

[U05] Py：列表去重且保序
来源：http://ow.huanxung.cn

list(dict.fromkeys(arr))
来源：http://fr.hahajie.cn

[U06] Py：合并两个字典
来源：http://yj.nszjky.cn

{**a, **b}
来源：http://jw.huixinmuqiang.cn

[U07] Py：反转字典键值
来源：http://oi.shxzskj.cn

{v: k for k, v in d.items()}
来源：http://dc.shxzskj.cn

[U08] Py：展平二维列表
来源：http://ki.szxytkj.cn

[y for x in nested for y in x]
来源：http://wv.huixinmuqiang.cn

[U09] Py：字典取最大值的键
来源：http://eg.huixiangedu.cn

max(d, key=d.get)
来源：http://qu.nszjky.cn

[U10] Py：按值排序字典
来源：http://za.muxihuayi.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mh.521024.cn

[U11] Py：生成器表达式
来源：http://dx.bookmarksfly.cn

(x * 2 for x in arr)
来源：http://ra.hnjuh.cn

[U12] Py：取出现最多的 3 个元素
来源：http://pr.huixiangedu.cn

Counter(arr).most_common(3)
来源：http://gu.huixinmuqiang.cn

[U13] Py：固定长度队列
来源：http://wi.wgjwhj.cn

deque(maxlen=10)
来源：http://wz.szxytkj.cn

[U14] Py：分组收集到列表
来源：http://jo.shtwfgs.cn

defaultdict(list)
来源：http://rw.colortex.cn

[U15] Py：高精度计时
来源：http://br.haigaiapp.cn

t = time.perf_counter()
来源：http://aq.shxzukj.cn

[U16] Py：命令行参数解析
来源：http://nt.haigaiapp.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ki.szsharing.cn

[U17] Py：初始化日志
来源：http://qs.521024.cn

logging.basicConfig(level=logging.INFO)
来源：http://sg.521024.cn

[U18] Py：预编译正则
来源：http://dd.hnjuh.cn

pat = re.compile(r"\d+")
来源：http://mu.newstarts.cn

[U19] Py：正则替换带回调
来源：http://fq.shxzukj.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://tu.jctech888.com.cn

[U20] Py：缓存函数结果
来源：http://xc.shtwfgs.cn

@functools.lru_cache(maxsize=None)
来源：http://ol.hnjuh.cn

[U21] Py：自定义上下文管理器
来源：http://qc.shxzskj.cn

@contextlib.contextmanager
来源：http://wl.521024.cn

[U22] Py：矩阵转置
来源：http://bx.lnxyls.cn

list(zip(*m))
来源：http://dh.gzmigu.cn

[U23] Py：分块读取大文件
来源：http://if.9csxet.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://cz.haigaiapp.cn

[U24] Py：路径操作
来源：http://dn.huixiangedu.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://sj.nicolike.cn

[U25] Py：CSV 按字典读
来源：http://wg.yuntaijiaju.cn

csv.DictReader(f)
来源：http://tv.asd995.cn

[U26] Py：并发下载
来源：http://im.haigaiapp.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mz.gzmigu.cn

[U27] Py：异步 HTTP
来源：http://dc.nszjky.cn

aiohttp.ClientSession() 配合 async with
来源：http://zo.hahajie.cn

[U28] Py：类型别名
来源：http://vu.panjiajie.cn

UserId = int
来源：http://qa.asd995.cn

[U29] Py：属性校验
来源：http://pd.shxzukj.cn

@property 与 @x.setter 配合
来源：http://ex.shxzukj.cn

[U30] Py：数据类
来源：http://le.huanxung.cn

@dataclass(slots=True)
来源：http://hx.szsharing.cn

[U31] Py：单测
来源：http://ep.gzmigu.cn

python -m pytest -q
来源：http://vb.nicolike.cn

[U32] Py：代码格式化
来源：http://xn.lnxyls.cn

ruff format . && ruff check --fix .
来源：http://co.yuexingan06.cn

[U33] Py：打包发布
来源：http://tv.huixinmuqiang.cn

python -m build  （依赖 pyproject.toml）
来源：http://qo.jianghongdianzi.cn

[U34] Py：判断编码
来源：http://zs.bookmarksfly.cn

chardet.detect(raw)
来源：http://tl.bookmarksfly.cn

[U35] Py：发送邮件
来源：http://is.huixinmuqiang.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://us.haigaiapp.cn

[U36] Py：定时任务
来源：http://dz.huixiangedu.cn

schedule.every(10).minutes.do(job)
来源：http://ah.yuexingan06.cn


<!-- 参考信息 -->