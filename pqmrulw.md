代发 wailian999

x |= (1 << 3);
来源：http://id.521024.cn

[S17] C：安全拼接字符串
来源：http://rh.szxytkj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ka.nszjky.cn

[S18] C：命令行参数
来源：http://fq.9csxet.cn

int main(int argc, char **argv)
来源：http://gx.szxytkj.cn

[S19] C：快速排序
来源：http://xl.wgjwhj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ri.haigaiapp.cn

[S20] C：二分查找
来源：http://hc.jctech888.com.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://lw.bookmarksfly.cn

[S21] C：字符类别判断
来源：http://ag.hahajie.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://oy.bookmarksfly.cn

[S22] C：字符串转数字
来源：http://mv.jctech888.com.cn

atoi("42");  strtod("3.14", NULL);
来源：http://np.nszjky.cn

[S23] C：随机数
来源：http://ff.huixinmuqiang.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://lb.yuntaijiaju.cn

[S24] C：获取本地时间
来源：http://ul.jctech888.com.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://gg.huixinmuqiang.cn

[S25] C：内存拷贝
来源：http://ik.shxzskj.cn

memcpy(dst, src, n);
来源：http://jk.jctech888.com.cn

[S26] C：内存清零
来源：http://uf.yuntaijiaju.cn

memset(a, 0, sizeof a);
来源：http://qo.nszjky.cn

[S27] C：定义常量
来源：http://av.yuntaijiaju.cn

const double PI = 3.14159;
来源：http://yu.newstarts.cn

[S28] C：静态变量
来源：http://an.asd995.cn

static int counter = 0;
来源：http://df.yuntaijiaju.cn

[S29] C：变参函数
来源：http://zk.huanxung.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ab.haigaiapp.cn

[S30] C：头文件保护
来源：http://dt.521024.cn

#ifndef X_H
来源：http://tl.szsharing.cn

#define X_H
来源：http://rs.huanxung.cn

#endif
来源：http://hp.521024.cn

[S31] C++：Hello World
来源：http://eu.newstarts.cn

#include <iostream>
来源：http://ud.newstarts.cn

int main() { std::cout << "Hello\n"; }
来源：http://ow.haigaiapp.cn

[S32] C++：字符串
来源：http://kv.shxzukj.cn

std::string s = "hi";  s += "!";
来源：http://ma.colortex.cn

[S33] C++：vector 增删
来源：http://kq.lnxyls.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ud.newstarts.cn

[S34] C++：遍历 vector
来源：http://wt.huixiangedu.cn

for (auto &x : v) { std::cout << x; }
来源：http://ax.jianghongdianzi.cn

[S35] C++：map
来源：http://jz.shxzskj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://zg.9csxet.cn

[S36] C++：unordered_map
来源：http://rn.shxzskj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://sm.bookmarksfly.cn

[S37] C++：set
来源：http://df.huixiangedu.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ar.shxzskj.cn

[S38] C++：排序
来源：http://lc.huixinmuqiang.cn

std::sort(v.begin(), v.end());
来源：http://py.szsharing.cn

[S39] C++：自定义比较器排序
来源：http://bb.bjjhwx.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://bl.huanxung.cn

[S40] C++：查找元素
来源：http://cm.shtwfgs.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://cc.9csxet.cn

[S41] C++：类与构造函数
来源：http://sl.wgjwhj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://xp.lnxyls.cn

[S42] C++：继承与虚函数
来源：http://qw.haigaiapp.cn

class B : public Base { public: void f() override {} };
来源：http://of.shxzskj.cn

[S43] C++：智能指针
来源：http://uh.haigaiapp.cn

auto p = std::make_unique<int>(5);
来源：http://al.huixiangedu.cn

[S44] C++：引用传参
来源：http://gg.newstarts.cn

void inc(int &x) { ++x; }
来源：http://yv.521024.cn

[S45] C++：lambda
来源：http://qh.muxihuayi.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ds.muxihuayi.cn

[S46] C++：函数模板
来源：http://mn.hahajie.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://pn.szsharing.cn

[S47] C++：结构化绑定遍历
来源：http://wa.nszjky.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ha.nszjky.cn

[S48] C++：逐行读文件
来源：http://cv.shxzukj.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ro.shxzukj.cn

while (std::getline(in, line)) { }
来源：http://fv.panjiajie.cn

[S49] C++：写文件
来源：http://kn.haigaiapp.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mg.szsharing.cn

[S50] C++：格式化数字
来源：http://fk.hahajie.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://vj.huanxung.cn

[S51] C++：显式类型转换
来源：http://mm.gzmigu.cn

static_cast<double>(a) / b
来源：http://qv.hahajie.cn

[S52] C++：const 与 noexcept
来源：http://es.yuexingan06.cn

int size() const noexcept { return n_; }
来源：http://dy.shxzskj.cn

[S53] C++：移动语义
来源：http://tt.jianghongdianzi.cn

std::vector<int> w = std::move(v);
来源：http://xg.jianghongdianzi.cn

[S54] C++：异常处理
来源：http://qk.newstarts.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://go.jianghongdianzi.cn

[S55] C++：结构化绑定
来源：http://pu.shxzukj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://nt.lnxyls.cn

[S56] C++：optional
来源：http://jz.hnjuh.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://it.asd995.cn

[S57] C++：编译期常量
来源：http://pm.wgjwhj.cn

constexpr int N = 10;
来源：http://mw.nszjky.cn

[S58] C++：命名空间
来源：http://eg.hnjuh.cn

namespace ns { int f() { return 1; } }
来源：http://hr.shtwfgs.cn

[S59] C++：静态断言
来源：http://fz.bookmarksfly.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://mh.szsharing.cn

[S60] C++：遍历并删除元素
来源：http://pc.bookmarksfly.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ze.huixinmuqiang.cn

================================================================================
来源：http://bc.szxytkj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://es.yuexingan06.cn

================================================================================
来源：http://wj.jianghongdianzi.cn

[T01] Kotlin：Hello World
来源：http://lh.panjiajie.cn

println("Hello")
来源：http://ib.szsharing.cn

[T02] Kotlin：变量
来源：http://zk.colortex.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://bt.colortex.cn

[T03] Kotlin：字符串模板
来源：http://sh.szxytkj.cn

"值: $b"
来源：http://zy.asd995.cn

[T04] Kotlin：空安全
来源：http://cz.bjjhwx.cn

val n: String? = null;  n?.length
来源：http://nt.yuexingan06.cn

[T05] Kotlin：when 表达式
来源：http://oq.szsharing.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://fv.nicolike.cn

[T06] Kotlin：集合映射
来源：http://iw.haigaiapp.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://nr.bookmarksfly.cn

[T07] Kotlin：集合过滤
来源：http://my.hahajie.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ii.gzmigu.cn

[T08] Kotlin：数据类
来源：http://ki.huanxung.cn

data class User(val name: String, val age: Int)
来源：http://ds.521024.cn

[T09] Kotlin：扩展函数
来源：http://ji.nicolike.cn

fun String.exclaim() = this + "!"
来源：http://zl.bjjhwx.cn

[T10] Kotlin：默认参数
来源：http://hr.gzmigu.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://dn.muxihuayi.cn

[T11] Kotlin：协程
来源：http://yt.muxihuayi.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://th.jianghongdianzi.cn

[T12] Kotlin：解构声明
来源：http://al.huixiangedu.cn

val (a, b) = Pair(1, 2)
来源：http://ey.szxytkj.cn

[T13] Kotlin：只读 Map
来源：http://ko.jctech888.com.cn

val m = mapOf("a" to 1)
来源：http://vn.chemitech.net.cn

[T14] Kotlin：循环
来源：http://ou.521024.cn

for (i in 1..10) println(i)
来源：http://ud.521024.cn

[T15] Kotlin：接口
来源：http://eu.hahajie.cn

interface Shape { fun area(): Double }
来源：http://vp.asd995.cn

[T16] Swift：Hello World
来源：http://iw.bjjhwx.cn

print("Hello")
来源：http://fi.haigaiapp.cn

[T17] Swift：变量与常量
来源：http://pt.9csxet.cn

var a = 1;  let b = 2
来源：http://ig.nicolike.cn

[T18] Swift：字符串插值
来源：http://xi.jctech888.com.cn

"值: \(b)"
来源：http://ib.huixinmuqiang.cn

[T19] Swift：可选绑定
来源：http://ox.shxzskj.cn

if let n = opt { print(n) }
来源：http://qw.wgjwhj.cn

[T20] Swift：数组操作
来源：http://ut.lnxyls.cn

var a = [1, 2, 3];  a.append(4)
来源：http://lu.asd995.cn

[T21] Swift：遍历
来源：http://wt.colortex.cn

for x in a { print(x) }
来源：http://aj.colortex.cn

[T22] Swift：字典
来源：http://lz.521024.cn

var d = ["a": 1];  d["b"] = 2
来源：http://nr.9csxet.cn

[T23] Swift：函数
来源：http://ae.shxzukj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://dr.szxytkj.cn

[T24] Swift：闭包
来源：http://gw.hahajie.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://zh.nszjky.cn

[T25] Swift：结构体
来源：http://hk.huixiangedu.cn

struct P { var x: Int }
来源：http://ad.521024.cn

[T26] Swift：类与重写
来源：http://lv.colortex.cn

class A: Base { override func f() {} }
来源：http://ol.gzmigu.cn

[T27] Swift：错误处理
来源：http://ad.yuntaijiaju.cn

do { try f() } catch { print(error) }
来源：http://ao.chemitech.net.cn

[T28] Swift：枚举
来源：http://vh.shxzskj.cn

enum Color { case red, green }
来源：http://mz.huixiangedu.cn

[T29] Swift：guard 提前返回
来源：http://tu.muxihuayi.cn

guard let x = opt else { return }
来源：http://ne.bookmarksfly.cn

[T30] Swift：协议
来源：http://lb.haigaiapp.cn

protocol Shape { func area() -> Double }
来源：http://la.bjjhwx.cn

[T31] Lua：Hello World
来源：http://sr.shxzskj.cn

print("Hello")
来源：http://if.szxytkj.cn

[T32] Lua：局部变量
来源：http://bu.colortex.cn

local a = 1
来源：http://qe.jctech888.com.cn

[T33] Lua：表（数组）
来源：http://tn.lnxyls.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://na.hnjuh.cn

[T34] Lua：遍历表
来源：http://sy.hahajie.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://kf.shxzskj.cn

[T35] Lua：字典表
来源：http://je.yuntaijiaju.cn

local d = { a = 1 };  d.b = 2
来源：http://rg.shxzskj.cn

[T36] Lua：函数
来源：http://th.bjjhwx.cn

function add(a, b) return a + b end
来源：http://at.yuntaijiaju.cn

[T37] Lua：字符串拼接
来源：http://eq.yuexingan06.cn

"a" .. "b"
来源：http://tk.newstarts.cn

[T38] Lua：条件
来源：http://de.panjiajie.cn

if x > 0 then print("正") end
来源：http://rz.521024.cn

[T39] Lua：模式匹配
来源：http://kb.hahajie.cn

string.find(s, "%d+")
来源：http://ac.shxzukj.cn

[T40] Lua：元表
来源：http://ho.shxzukj.cn

setmetatable({}, { __index = base })
来源：http://ze.hnjuh.cn

[T41] Perl：Hello World
来源：http://lw.bjjhwx.cn

print "Hello\n";
来源：http://tf.jctech888.com.cn

[T42] Perl：变量类型
来源：http://zd.lnxyls.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://jo.yuntaijiaju.cn

[T43] Perl：字符串插值
来源：http://jb.yuntaijiaju.cn

"值: $a"
来源：http://oh.chemitech.net.cn

[T44] Perl：条件
来源：http://if.yuexingan06.cn

if ($a > 0) { print "正"; }
来源：http://if.muxihuayi.cn

[T45] Perl：数组遍历
来源：http://fl.szsharing.cn

for my $x (@arr) { print $x; }
来源：http://bh.huixiangedu.cn

[T46] Perl：哈希操作
来源：http://hd.yuexingan06.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://fv.newstarts.cn

[T47] Perl：正则捕获
来源：http://hn.yuexingan06.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://aj.shxzukj.cn

[T48] Perl：正则替换
来源：http://tc.shxzskj.cn

$s =~ s/old/new/g;
来源：http://uf.muxihuayi.cn

[T49] Perl：函数
来源：http://jr.521024.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://vc.jianghongdianzi.cn

[T50] Perl：逐行读文件
来源：http://gm.szsharing.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://uc.chemitech.net.cn

while (my $line = <$fh>) { print $line; }
来源：http://tb.szsharing.cn

[T51] Scala：Hello World
来源：http://lm.haigaiapp.cn

println("Hello")
来源：http://kr.shxzskj.cn

[T52] Scala：变量
来源：http://ps.nicolike.cn

val a = 1;  var b = 2
来源：http://qt.yuntaijiaju.cn

[T53] Scala：字符串插值
来源：http://qj.gzmigu.cn

s"值: $b"
来源：http://kw.shxzukj.cn

[T54] Scala：集合映射
来源：http://jx.haigaiapp.cn

List(1, 2, 3).map(_ * 2)
来源：http://tg.panjiajie.cn

[T55] Scala：集合过滤
来源：http://ie.nszjky.cn

List(1, 2, 3).filter(_ > 1)
来源：http://nx.hahajie.cn

[T56] Scala：样例类
来源：http://ri.hnjuh.cn

case class User(name: String, age: Int)
来源：http://na.shxzukj.cn

[T57] Scala：模式匹配
来源：http://ve.9csxet.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://hn.huixinmuqiang.cn

[T58] Scala：函数定义
来源：http://xo.szsharing.cn

def add(a: Int, b: Int): Int = a + b
来源：http://cn.shxzukj.cn

[T59] Scala：循环
来源：http://bh.9csxet.cn

for (i <- 1 to 10) println(i)
来源：http://uh.bookmarksfly.cn

[T60] Scala：折叠
来源：http://fy.9csxet.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wh.huanxung.cn

================================================================================
来源：http://vd.9csxet.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://yo.haigaiapp.cn

================================================================================
来源：http://bj.nicolike.cn

[U01] Py：创建虚拟环境
来源：http://rb.521024.cn

python -m venv .venv && source .venv/bin/activate
来源：http://wb.9csxet.cn

[U02] Py：导出 / 安装依赖
来源：http://gz.muxihuayi.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ex.shxzukj.cn

[U03] Py：加载 .env 配置
来源：http://yu.bjjhwx.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://oz.panjiajie.cn

[U04] Py：变量调试打印
来源：http://sv.bookmarksfly.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ne.newstarts.cn

[U05] Py：列表去重且保序
来源：http://xv.521024.cn

list(dict.fromkeys(arr))
来源：http://jv.jianghongdianzi.cn

[U06] Py：合并两个字典
来源：http://br.shxzukj.cn

{**a, **b}
来源：http://fb.521024.cn

[U07] Py：反转字典键值
来源：http://lb.huixinmuqiang.cn

{v: k for k, v in d.items()}
来源：http://zn.9csxet.cn

[U08] Py：展平二维列表
来源：http://uz.szsharing.cn

[y for x in nested for y in x]
来源：http://an.9csxet.cn

[U09] Py：字典取最大值的键
来源：http://hm.lnxyls.cn

max(d, key=d.get)
来源：http://jc.huanxung.cn

[U10] Py：按值排序字典
来源：http://qi.panjiajie.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://fk.muxihuayi.cn

[U11] Py：生成器表达式
来源：http://kq.muxihuayi.cn

(x * 2 for x in arr)
来源：http://gl.haigaiapp.cn

[U12] Py：取出现最多的 3 个元素
来源：http://es.szsharing.cn

Counter(arr).most_common(3)
来源：http://jj.yuntaijiaju.cn

[U13] Py：固定长度队列
来源：http://ed.nszjky.cn

deque(maxlen=10)
来源：http://sj.szsharing.cn

[U14] Py：分组收集到列表
来源：http://uc.huanxung.cn

defaultdict(list)
来源：http://uc.haigaiapp.cn

[U15] Py：高精度计时
来源：http://hj.shxzskj.cn

t = time.perf_counter()
来源：http://fv.shxzskj.cn

[U16] Py：命令行参数解析
来源：http://td.huixinmuqiang.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://hl.shxzukj.cn

[U17] Py：初始化日志
来源：http://aq.wgjwhj.cn

logging.basicConfig(level=logging.INFO)
来源：http://tk.jctech888.com.cn

[U18] Py：预编译正则
来源：http://lv.jianghongdianzi.cn

pat = re.compile(r"\d+")
来源：http://jc.panjiajie.cn

[U19] Py：正则替换带回调
来源：http://fi.jctech888.com.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://wd.bjjhwx.cn

[U20] Py：缓存函数结果
来源：http://ox.gzmigu.cn

@functools.lru_cache(maxsize=None)
来源：http://ua.nszjky.cn

[U21] Py：自定义上下文管理器
来源：http://cs.shtwfgs.cn

@contextlib.contextmanager
来源：http://uk.521024.cn

[U22] Py：矩阵转置
来源：http://ij.521024.cn

list(zip(*m))
来源：http://om.nicolike.cn

[U23] Py：分块读取大文件
来源：http://iy.hnjuh.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://co.lnxyls.cn

[U24] Py：路径操作
来源：http://rj.wgjwhj.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ap.shtwfgs.cn

[U25] Py：CSV 按字典读
来源：http://vp.yuntaijiaju.cn

csv.DictReader(f)
来源：http://rx.shxzukj.cn

[U26] Py：并发下载
来源：http://no.gzmigu.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ev.hahajie.cn

[U27] Py：异步 HTTP
来源：http://gv.newstarts.cn

aiohttp.ClientSession() 配合 async with
来源：http://is.hnjuh.cn

[U28] Py：类型别名
来源：http://ic.hahajie.cn

UserId = int
来源：http://lj.panjiajie.cn

[U29] Py：属性校验
来源：http://pf.szsharing.cn

@property 与 @x.setter 配合
来源：http://na.hnjuh.cn

[U30] Py：数据类
来源：http://eu.lnxyls.cn

@dataclass(slots=True)
来源：http://ve.yuexingan06.cn

[U31] Py：单测
来源：http://pc.shxzukj.cn

python -m pytest -q
来源：http://aj.chemitech.net.cn

[U32] Py：代码格式化
来源：http://it.jctech888.com.cn

ruff format . && ruff check --fix .
来源：http://iw.521024.cn

[U33] Py：打包发布
来源：http://rz.haigaiapp.cn

python -m build  （依赖 pyproject.toml）
来源：http://bo.hnjuh.cn

[U34] Py：判断编码
来源：http://db.hahajie.cn

chardet.detect(raw)
来源：http://ri.gzmigu.cn

[U35] Py：发送邮件
来源：http://mw.bookmarksfly.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://xn.chemitech.net.cn

[U36] Py：定时任务
来源：http://bm.521024.cn

schedule.every(10).minutes.do(job)
来源：http://sb.chemitech.net.cn

[U37] Py：读写 Excel
来源：http://su.jctech888.com.cn

pandas.read_excel / DataFrame.to_excel
来源：http://kc.muxihuayi.cn

[U38] Py：获取脚本所在目录
来源：http://dd.newstarts.cn

Path(__file__).resolve().parent
来源：http://rq.hnjuh.cn

[U39] Py：判断是否在交互环境
来源：http://pz.colortex.cn

sys.stdout.isatty()
来源：http://ib.nicolike.cn

[U40] Py：打印到标准错误
来源：http://wu.hnjuh.cn

print("err", file=sys.stderr)
来源：http://ty.huixiangedu.cn


<!-- 参考信息 -->