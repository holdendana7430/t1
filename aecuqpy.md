代发 wailian999

enum Color { RED, GREEN, BLUE };
来源：http://pk.muxihuayi.cn

[S15] C：类型转换
来源：http://kj.jianghongdianzi.cn

(double) a / b
来源：http://un.hahajie.cn

[S16] C：位操作置位
来源：http://tq.jianghongdianzi.cn

x |= (1 << 3);
来源：http://hg.shxzukj.cn

[S17] C：安全拼接字符串
来源：http://bv.muxihuayi.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ht.newstarts.cn

[S18] C：命令行参数
来源：http://xl.huixinmuqiang.cn

int main(int argc, char **argv)
来源：http://sb.nicolike.cn

[S19] C：快速排序
来源：http://sw.huixiangedu.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ao.hnjuh.cn

[S20] C：二分查找
来源：http://lu.szsharing.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://vb.huixinmuqiang.cn

[S21] C：字符类别判断
来源：http://wv.colortex.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://py.muxihuayi.cn

[S22] C：字符串转数字
来源：http://qp.muxihuayi.cn

atoi("42");  strtod("3.14", NULL);
来源：http://bk.newstarts.cn

[S23] C：随机数
来源：http://ux.nicolike.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://on.lnxyls.cn

[S24] C：获取本地时间
来源：http://pg.shtwfgs.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://cg.newstarts.cn

[S25] C：内存拷贝
来源：http://pm.shtwfgs.cn

memcpy(dst, src, n);
来源：http://tv.lnxyls.cn

[S26] C：内存清零
来源：http://yr.haigaiapp.cn

memset(a, 0, sizeof a);
来源：http://ej.panjiajie.cn

[S27] C：定义常量
来源：http://ta.asd995.cn

const double PI = 3.14159;
来源：http://zh.bookmarksfly.cn

[S28] C：静态变量
来源：http://wv.yuntaijiaju.cn

static int counter = 0;
来源：http://cz.hnjuh.cn

[S29] C：变参函数
来源：http://kq.chemitech.net.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ge.nszjky.cn

[S30] C：头文件保护
来源：http://bw.szxytkj.cn

#ifndef X_H
来源：http://xm.huixiangedu.cn

#define X_H
来源：http://li.nicolike.cn

#endif
来源：http://pt.gzmigu.cn

[S31] C++：Hello World
来源：http://kn.yuexingan06.cn

#include <iostream>
来源：http://ds.shtwfgs.cn

int main() { std::cout << "Hello\n"; }
来源：http://wt.nszjky.cn

[S32] C++：字符串
来源：http://kz.haigaiapp.cn

std::string s = "hi";  s += "!";
来源：http://sp.gzmigu.cn

[S33] C++：vector 增删
来源：http://xq.521024.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hf.shtwfgs.cn

[S34] C++：遍历 vector
来源：http://lv.bjjhwx.cn

for (auto &x : v) { std::cout << x; }
来源：http://jv.nicolike.cn

[S35] C++：map
来源：http://mg.wgjwhj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://bt.nszjky.cn

[S36] C++：unordered_map
来源：http://av.yuntaijiaju.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://rq.bjjhwx.cn

[S37] C++：set
来源：http://fl.szxytkj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://vq.521024.cn

[S38] C++：排序
来源：http://st.nszjky.cn

std::sort(v.begin(), v.end());
来源：http://tx.szxytkj.cn

[S39] C++：自定义比较器排序
来源：http://lr.lnxyls.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://js.chemitech.net.cn

[S40] C++：查找元素
来源：http://ns.wgjwhj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://xf.yuexingan06.cn

[S41] C++：类与构造函数
来源：http://sy.521024.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://px.bookmarksfly.cn

[S42] C++：继承与虚函数
来源：http://fu.bjjhwx.cn

class B : public Base { public: void f() override {} };
来源：http://ps.haigaiapp.cn

[S43] C++：智能指针
来源：http://pv.bjjhwx.cn

auto p = std::make_unique<int>(5);
来源：http://fm.panjiajie.cn

[S44] C++：引用传参
来源：http://hj.huixiangedu.cn

void inc(int &x) { ++x; }
来源：http://lt.shxzskj.cn

[S45] C++：lambda
来源：http://oc.521024.cn

auto add = [](int a, int b) { return a + b; };
来源：http://wp.muxihuayi.cn

[S46] C++：函数模板
来源：http://ha.521024.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://pv.colortex.cn

[S47] C++：结构化绑定遍历
来源：http://ua.hnjuh.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ky.hahajie.cn

[S48] C++：逐行读文件
来源：http://wi.lnxyls.cn

std::ifstream in("a.txt");  std::string line;
来源：http://kv.nicolike.cn

while (std::getline(in, line)) { }
来源：http://ie.haigaiapp.cn

[S49] C++：写文件
来源：http://nu.bjjhwx.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://gb.jctech888.com.cn

[S50] C++：格式化数字
来源：http://fg.jctech888.com.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ru.shxzukj.cn

[S51] C++：显式类型转换
来源：http://dq.szsharing.cn

static_cast<double>(a) / b
来源：http://vb.gzmigu.cn

[S52] C++：const 与 noexcept
来源：http://hn.hnjuh.cn

int size() const noexcept { return n_; }
来源：http://dm.huixiangedu.cn

[S53] C++：移动语义
来源：http://an.chemitech.net.cn

std::vector<int> w = std::move(v);
来源：http://yf.9csxet.cn

[S54] C++：异常处理
来源：http://lq.shxzskj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://vo.muxihuayi.cn

[S55] C++：结构化绑定
来源：http://wd.hnjuh.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://to.huixinmuqiang.cn

[S56] C++：optional
来源：http://zl.yuntaijiaju.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ph.muxihuayi.cn

[S57] C++：编译期常量
来源：http://ac.lnxyls.cn

constexpr int N = 10;
来源：http://ct.9csxet.cn

[S58] C++：命名空间
来源：http://ho.yuntaijiaju.cn

namespace ns { int f() { return 1; } }
来源：http://bt.szsharing.cn

[S59] C++：静态断言
来源：http://hs.bookmarksfly.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ke.hnjuh.cn

[S60] C++：遍历并删除元素
来源：http://fh.huanxung.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://jf.bjjhwx.cn

================================================================================
来源：http://li.yuexingan06.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://yn.yuntaijiaju.cn

================================================================================
来源：http://av.nszjky.cn

[T01] Kotlin：Hello World
来源：http://it.yuntaijiaju.cn

println("Hello")
来源：http://ht.shtwfgs.cn

[T02] Kotlin：变量
来源：http://rm.panjiajie.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mu.bookmarksfly.cn

[T03] Kotlin：字符串模板
来源：http://db.asd995.cn

"值: $b"
来源：http://iq.yuntaijiaju.cn

[T04] Kotlin：空安全
来源：http://kt.asd995.cn

val n: String? = null;  n?.length
来源：http://qg.szsharing.cn

[T05] Kotlin：when 表达式
来源：http://tu.yuntaijiaju.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://rm.yuntaijiaju.cn

[T06] Kotlin：集合映射
来源：http://xo.chemitech.net.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ul.wgjwhj.cn

[T07] Kotlin：集合过滤
来源：http://jv.hahajie.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://sy.bjjhwx.cn

[T08] Kotlin：数据类
来源：http://hq.asd995.cn

data class User(val name: String, val age: Int)
来源：http://nx.bjjhwx.cn

[T09] Kotlin：扩展函数
来源：http://yz.gzmigu.cn

fun String.exclaim() = this + "!"
来源：http://bz.huixinmuqiang.cn

[T10] Kotlin：默认参数
来源：http://bm.jctech888.com.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://fp.9csxet.cn

[T11] Kotlin：协程
来源：http://kc.huixinmuqiang.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://wd.jianghongdianzi.cn

[T12] Kotlin：解构声明
来源：http://py.shtwfgs.cn

val (a, b) = Pair(1, 2)
来源：http://rr.hnjuh.cn

[T13] Kotlin：只读 Map
来源：http://vj.panjiajie.cn

val m = mapOf("a" to 1)
来源：http://ay.521024.cn

[T14] Kotlin：循环
来源：http://mf.newstarts.cn

for (i in 1..10) println(i)
来源：http://tc.newstarts.cn

[T15] Kotlin：接口
来源：http://up.shxzukj.cn

interface Shape { fun area(): Double }
来源：http://ok.szxytkj.cn

[T16] Swift：Hello World
来源：http://qs.huixinmuqiang.cn

print("Hello")
来源：http://yb.huixinmuqiang.cn

[T17] Swift：变量与常量
来源：http://ln.haigaiapp.cn

var a = 1;  let b = 2
来源：http://vk.muxihuayi.cn

[T18] Swift：字符串插值
来源：http://ct.bookmarksfly.cn

"值: \(b)"
来源：http://ut.muxihuayi.cn

[T19] Swift：可选绑定
来源：http://zz.haigaiapp.cn

if let n = opt { print(n) }
来源：http://yw.9csxet.cn

[T20] Swift：数组操作
来源：http://ry.muxihuayi.cn

var a = [1, 2, 3];  a.append(4)
来源：http://mo.521024.cn

[T21] Swift：遍历
来源：http://rz.muxihuayi.cn

for x in a { print(x) }
来源：http://yr.521024.cn

[T22] Swift：字典
来源：http://qf.szxytkj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://vu.yuexingan06.cn

[T23] Swift：函数
来源：http://zf.shtwfgs.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ja.jianghongdianzi.cn

[T24] Swift：闭包
来源：http://vg.hnjuh.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://cs.panjiajie.cn

[T25] Swift：结构体
来源：http://dn.huanxung.cn

struct P { var x: Int }
来源：http://hz.huixiangedu.cn

[T26] Swift：类与重写
来源：http://rc.jianghongdianzi.cn

class A: Base { override func f() {} }
来源：http://ik.nszjky.cn

[T27] Swift：错误处理
来源：http://at.9csxet.cn

do { try f() } catch { print(error) }
来源：http://ii.521024.cn

[T28] Swift：枚举
来源：http://yw.shxzukj.cn

enum Color { case red, green }
来源：http://bk.szxytkj.cn

[T29] Swift：guard 提前返回
来源：http://gh.wgjwhj.cn

guard let x = opt else { return }
来源：http://bs.chemitech.net.cn

[T30] Swift：协议
来源：http://uo.muxihuayi.cn

protocol Shape { func area() -> Double }
来源：http://so.jianghongdianzi.cn

[T31] Lua：Hello World
来源：http://pn.hahajie.cn

print("Hello")
来源：http://yk.huixiangedu.cn

[T32] Lua：局部变量
来源：http://me.jianghongdianzi.cn

local a = 1
来源：http://oh.asd995.cn

[T33] Lua：表（数组）
来源：http://zo.hnjuh.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://bx.nszjky.cn

[T34] Lua：遍历表
来源：http://vz.shtwfgs.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ib.muxihuayi.cn

[T35] Lua：字典表
来源：http://fc.521024.cn

local d = { a = 1 };  d.b = 2
来源：http://ys.jctech888.com.cn

[T36] Lua：函数
来源：http://jp.panjiajie.cn

function add(a, b) return a + b end
来源：http://jh.chemitech.net.cn

[T37] Lua：字符串拼接
来源：http://gz.hahajie.cn

"a" .. "b"
来源：http://hb.521024.cn

[T38] Lua：条件
来源：http://ni.shxzskj.cn

if x > 0 then print("正") end
来源：http://mz.9csxet.cn

[T39] Lua：模式匹配
来源：http://li.huanxung.cn

string.find(s, "%d+")
来源：http://vw.shxzukj.cn

[T40] Lua：元表
来源：http://mr.szxytkj.cn

setmetatable({}, { __index = base })
来源：http://kz.colortex.cn

[T41] Perl：Hello World
来源：http://kd.shxzskj.cn

print "Hello\n";
来源：http://ow.panjiajie.cn

[T42] Perl：变量类型
来源：http://cv.szxytkj.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ri.szsharing.cn

[T43] Perl：字符串插值
来源：http://aq.shxzukj.cn

"值: $a"
来源：http://va.huixiangedu.cn

[T44] Perl：条件
来源：http://ck.gzmigu.cn

if ($a > 0) { print "正"; }
来源：http://yz.huanxung.cn

[T45] Perl：数组遍历
来源：http://xx.hahajie.cn

for my $x (@arr) { print $x; }
来源：http://ss.jctech888.com.cn

[T46] Perl：哈希操作
来源：http://yl.gzmigu.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://no.bjjhwx.cn

[T47] Perl：正则捕获
来源：http://ua.newstarts.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://cv.hahajie.cn

[T48] Perl：正则替换
来源：http://hm.jctech888.com.cn

$s =~ s/old/new/g;
来源：http://qv.huanxung.cn

[T49] Perl：函数
来源：http://kr.newstarts.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://fw.jctech888.com.cn

[T50] Perl：逐行读文件
来源：http://ra.yuexingan06.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://vw.colortex.cn

while (my $line = <$fh>) { print $line; }
来源：http://ox.huixiangedu.cn

[T51] Scala：Hello World
来源：http://gu.huanxung.cn

println("Hello")
来源：http://uj.huixiangedu.cn

[T52] Scala：变量
来源：http://kr.lnxyls.cn

val a = 1;  var b = 2
来源：http://xk.newstarts.cn

[T53] Scala：字符串插值
来源：http://jv.chemitech.net.cn

s"值: $b"
来源：http://dz.panjiajie.cn

[T54] Scala：集合映射
来源：http://lr.wgjwhj.cn

List(1, 2, 3).map(_ * 2)
来源：http://vy.lnxyls.cn

[T55] Scala：集合过滤
来源：http://ah.newstarts.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ff.gzmigu.cn

[T56] Scala：样例类
来源：http://kp.huixinmuqiang.cn

case class User(name: String, age: Int)
来源：http://sc.haigaiapp.cn

[T57] Scala：模式匹配
来源：http://sa.muxihuayi.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://xw.nicolike.cn

[T58] Scala：函数定义
来源：http://pq.9csxet.cn

def add(a: Int, b: Int): Int = a + b
来源：http://oo.9csxet.cn

[T59] Scala：循环
来源：http://uf.gzmigu.cn

for (i <- 1 to 10) println(i)
来源：http://ao.szxytkj.cn

[T60] Scala：折叠
来源：http://xs.newstarts.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://tf.huixiangedu.cn

================================================================================
来源：http://st.muxihuayi.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hu.szxytkj.cn

================================================================================
来源：http://ot.muxihuayi.cn

[U01] Py：创建虚拟环境
来源：http://xo.shxzukj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://cu.huixiangedu.cn

[U02] Py：导出 / 安装依赖
来源：http://dm.colortex.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://jf.haigaiapp.cn

[U03] Py：加载 .env 配置
来源：http://vm.shxzskj.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://lp.bookmarksfly.cn

[U04] Py：变量调试打印
来源：http://ee.huixiangedu.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://je.shxzskj.cn

[U05] Py：列表去重且保序
来源：http://mi.wgjwhj.cn

list(dict.fromkeys(arr))
来源：http://co.asd995.cn

[U06] Py：合并两个字典
来源：http://dj.huixiangedu.cn

{**a, **b}
来源：http://uq.jctech888.com.cn

[U07] Py：反转字典键值
来源：http://dy.chemitech.net.cn

{v: k for k, v in d.items()}
来源：http://td.shtwfgs.cn

[U08] Py：展平二维列表
来源：http://ps.newstarts.cn

[y for x in nested for y in x]
来源：http://lz.bookmarksfly.cn

[U09] Py：字典取最大值的键
来源：http://uj.haigaiapp.cn

max(d, key=d.get)
来源：http://rw.hahajie.cn

[U10] Py：按值排序字典
来源：http://xb.shxzukj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://dr.lnxyls.cn

[U11] Py：生成器表达式
来源：http://ka.muxihuayi.cn

(x * 2 for x in arr)
来源：http://dh.jctech888.com.cn

[U12] Py：取出现最多的 3 个元素
来源：http://iw.huixinmuqiang.cn

Counter(arr).most_common(3)
来源：http://ff.asd995.cn

[U13] Py：固定长度队列
来源：http://rb.9csxet.cn

deque(maxlen=10)
来源：http://hh.yuntaijiaju.cn

[U14] Py：分组收集到列表
来源：http://fz.panjiajie.cn

defaultdict(list)
来源：http://ed.bjjhwx.cn

[U15] Py：高精度计时
来源：http://gc.nicolike.cn

t = time.perf_counter()
来源：http://wf.huixinmuqiang.cn

[U16] Py：命令行参数解析
来源：http://du.gzmigu.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://zo.huixiangedu.cn

[U17] Py：初始化日志
来源：http://kw.szsharing.cn

logging.basicConfig(level=logging.INFO)
来源：http://lp.shxzskj.cn

[U18] Py：预编译正则
来源：http://yk.hahajie.cn

pat = re.compile(r"\d+")
来源：http://uw.lnxyls.cn

[U19] Py：正则替换带回调
来源：http://ib.shxzskj.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://rz.muxihuayi.cn

[U20] Py：缓存函数结果
来源：http://fw.jctech888.com.cn

@functools.lru_cache(maxsize=None)
来源：http://xp.huixiangedu.cn

[U21] Py：自定义上下文管理器
来源：http://hi.szsharing.cn

@contextlib.contextmanager
来源：http://xx.haigaiapp.cn

[U22] Py：矩阵转置
来源：http://zk.521024.cn

list(zip(*m))
来源：http://tn.nszjky.cn

[U23] Py：分块读取大文件
来源：http://hy.haigaiapp.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://eo.yuexingan06.cn

[U24] Py：路径操作
来源：http://kb.yuexingan06.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://hq.9csxet.cn

[U25] Py：CSV 按字典读
来源：http://sr.wgjwhj.cn

csv.DictReader(f)
来源：http://la.yuexingan06.cn

[U26] Py：并发下载
来源：http://iz.nicolike.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://gc.wgjwhj.cn

[U27] Py：异步 HTTP
来源：http://bo.huixiangedu.cn

aiohttp.ClientSession() 配合 async with
来源：http://gn.521024.cn

[U28] Py：类型别名
来源：http://uj.yuexingan06.cn

UserId = int
来源：http://sy.chemitech.net.cn

[U29] Py：属性校验
来源：http://cq.nszjky.cn

@property 与 @x.setter 配合
来源：http://ng.bookmarksfly.cn

[U30] Py：数据类
来源：http://or.haigaiapp.cn

@dataclass(slots=True)
来源：http://ne.panjiajie.cn

[U31] Py：单测
来源：http://ux.chemitech.net.cn

python -m pytest -q
来源：http://ha.lnxyls.cn

[U32] Py：代码格式化
来源：http://tw.hnjuh.cn

ruff format . && ruff check --fix .
来源：http://kc.huixinmuqiang.cn

[U33] Py：打包发布
来源：http://se.colortex.cn

python -m build  （依赖 pyproject.toml）
来源：http://ym.shxzukj.cn

[U34] Py：判断编码
来源：http://cr.lnxyls.cn

chardet.detect(raw)
来源：http://wy.nicolike.cn

[U35] Py：发送邮件
来源：http://pk.yuexingan06.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://zz.huixinmuqiang.cn

[U36] Py：定时任务
来源：http://gh.wgjwhj.cn

schedule.every(10).minutes.do(job)
来源：http://eh.wgjwhj.cn

[U37] Py：读写 Excel
来源：http://jr.hahajie.cn

pandas.read_excel / DataFrame.to_excel
来源：http://uc.bjjhwx.cn

[U38] Py：获取脚本所在目录
来源：http://yw.newstarts.cn

Path(__file__).resolve().parent
来源：http://vy.huixiangedu.cn


<!-- 参考信息 -->