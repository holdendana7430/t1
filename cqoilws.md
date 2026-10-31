代发 wailian999

int main(int argc, char **argv)
来源：http://fb.huixiangedu.cn

[S19] C：快速排序
来源：http://wy.asd995.cn

qsort(a, n, sizeof(int), cmp);
来源：http://yg.nszjky.cn

[S20] C：二分查找
来源：http://cq.jctech888.com.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wz.shxzskj.cn

[S21] C：字符类别判断
来源：http://wc.huixinmuqiang.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ky.bookmarksfly.cn

[S22] C：字符串转数字
来源：http://vm.yuntaijiaju.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ye.521024.cn

[S23] C：随机数
来源：http://qy.hnjuh.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://vj.nicolike.cn

[S24] C：获取本地时间
来源：http://cw.lnxyls.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://vi.yuntaijiaju.cn

[S25] C：内存拷贝
来源：http://nx.521024.cn

memcpy(dst, src, n);
来源：http://qu.nicolike.cn

[S26] C：内存清零
来源：http://te.colortex.cn

memset(a, 0, sizeof a);
来源：http://ig.jctech888.com.cn

[S27] C：定义常量
来源：http://fo.szsharing.cn

const double PI = 3.14159;
来源：http://tu.chemitech.net.cn

[S28] C：静态变量
来源：http://xm.jianghongdianzi.cn

static int counter = 0;
来源：http://gd.yuexingan06.cn

[S29] C：变参函数
来源：http://dd.jctech888.com.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://rs.jianghongdianzi.cn

[S30] C：头文件保护
来源：http://vo.hahajie.cn

#ifndef X_H
来源：http://sv.jianghongdianzi.cn

#define X_H
来源：http://sg.yuntaijiaju.cn

#endif
来源：http://qb.bjjhwx.cn

[S31] C++：Hello World
来源：http://ll.panjiajie.cn

#include <iostream>
来源：http://et.bjjhwx.cn

int main() { std::cout << "Hello\n"; }
来源：http://xg.szsharing.cn

[S32] C++：字符串
来源：http://dg.bookmarksfly.cn

std::string s = "hi";  s += "!";
来源：http://og.panjiajie.cn

[S33] C++：vector 增删
来源：http://hp.shxzskj.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ed.lnxyls.cn

[S34] C++：遍历 vector
来源：http://is.wgjwhj.cn

for (auto &x : v) { std::cout << x; }
来源：http://an.haigaiapp.cn

[S35] C++：map
来源：http://lf.huixinmuqiang.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ft.lnxyls.cn

[S36] C++：unordered_map
来源：http://ff.bjjhwx.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mu.yuexingan06.cn

[S37] C++：set
来源：http://en.9csxet.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://xn.asd995.cn

[S38] C++：排序
来源：http://ad.newstarts.cn

std::sort(v.begin(), v.end());
来源：http://pb.bookmarksfly.cn

[S39] C++：自定义比较器排序
来源：http://ao.yuexingan06.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://lt.9csxet.cn

[S40] C++：查找元素
来源：http://kt.chemitech.net.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://iy.nicolike.cn

[S41] C++：类与构造函数
来源：http://kw.9csxet.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ot.huixiangedu.cn

[S42] C++：继承与虚函数
来源：http://em.muxihuayi.cn

class B : public Base { public: void f() override {} };
来源：http://ag.huixinmuqiang.cn

[S43] C++：智能指针
来源：http://gb.9csxet.cn

auto p = std::make_unique<int>(5);
来源：http://fc.asd995.cn

[S44] C++：引用传参
来源：http://bz.521024.cn

void inc(int &x) { ++x; }
来源：http://df.huixinmuqiang.cn

[S45] C++：lambda
来源：http://fd.hahajie.cn

auto add = [](int a, int b) { return a + b; };
来源：http://zv.521024.cn

[S46] C++：函数模板
来源：http://ha.yuntaijiaju.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ya.shxzukj.cn

[S47] C++：结构化绑定遍历
来源：http://zo.jianghongdianzi.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://fa.lnxyls.cn

[S48] C++：逐行读文件
来源：http://pe.huixinmuqiang.cn

std::ifstream in("a.txt");  std::string line;
来源：http://uw.nszjky.cn

while (std::getline(in, line)) { }
来源：http://xa.szxytkj.cn

[S49] C++：写文件
来源：http://xo.jctech888.com.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://jk.shxzukj.cn

[S50] C++：格式化数字
来源：http://cn.jctech888.com.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://fr.shtwfgs.cn

[S51] C++：显式类型转换
来源：http://vz.huanxung.cn

static_cast<double>(a) / b
来源：http://sp.hnjuh.cn

[S52] C++：const 与 noexcept
来源：http://mf.9csxet.cn

int size() const noexcept { return n_; }
来源：http://ce.521024.cn

[S53] C++：移动语义
来源：http://nv.gzmigu.cn

std::vector<int> w = std::move(v);
来源：http://zq.shxzskj.cn

[S54] C++：异常处理
来源：http://ax.muxihuayi.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mq.jianghongdianzi.cn

[S55] C++：结构化绑定
来源：http://uz.huixinmuqiang.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://lb.jianghongdianzi.cn

[S56] C++：optional
来源：http://ju.nszjky.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://be.lnxyls.cn

[S57] C++：编译期常量
来源：http://qv.jctech888.com.cn

constexpr int N = 10;
来源：http://zz.shxzukj.cn

[S58] C++：命名空间
来源：http://jn.huixinmuqiang.cn

namespace ns { int f() { return 1; } }
来源：http://pl.gzmigu.cn

[S59] C++：静态断言
来源：http://vb.9csxet.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://pf.wgjwhj.cn

[S60] C++：遍历并删除元素
来源：http://lb.huixinmuqiang.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://zb.gzmigu.cn

================================================================================
来源：http://kk.colortex.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://gz.9csxet.cn

================================================================================
来源：http://st.huixiangedu.cn

[T01] Kotlin：Hello World
来源：http://se.yuexingan06.cn

println("Hello")
来源：http://dj.newstarts.cn

[T02] Kotlin：变量
来源：http://zv.colortex.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://tx.shxzukj.cn

[T03] Kotlin：字符串模板
来源：http://uu.jianghongdianzi.cn

"值: $b"
来源：http://yl.9csxet.cn

[T04] Kotlin：空安全
来源：http://fk.shxzukj.cn

val n: String? = null;  n?.length
来源：http://en.newstarts.cn

[T05] Kotlin：when 表达式
来源：http://lo.newstarts.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hg.gzmigu.cn

[T06] Kotlin：集合映射
来源：http://tp.9csxet.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ss.wgjwhj.cn

[T07] Kotlin：集合过滤
来源：http://dm.szsharing.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://lx.shxzukj.cn

[T08] Kotlin：数据类
来源：http://sk.muxihuayi.cn

data class User(val name: String, val age: Int)
来源：http://zo.shxzukj.cn

[T09] Kotlin：扩展函数
来源：http://om.colortex.cn

fun String.exclaim() = this + "!"
来源：http://iq.gzmigu.cn

[T10] Kotlin：默认参数
来源：http://xy.shtwfgs.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://px.gzmigu.cn

[T11] Kotlin：协程
来源：http://ze.huanxung.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://xz.shxzskj.cn

[T12] Kotlin：解构声明
来源：http://nb.wgjwhj.cn

val (a, b) = Pair(1, 2)
来源：http://jh.haigaiapp.cn

[T13] Kotlin：只读 Map
来源：http://ri.nszjky.cn

val m = mapOf("a" to 1)
来源：http://sv.panjiajie.cn

[T14] Kotlin：循环
来源：http://as.bookmarksfly.cn

for (i in 1..10) println(i)
来源：http://rc.shxzukj.cn

[T15] Kotlin：接口
来源：http://lk.szsharing.cn

interface Shape { fun area(): Double }
来源：http://xm.huixiangedu.cn

[T16] Swift：Hello World
来源：http://ql.shtwfgs.cn

print("Hello")
来源：http://zl.yuntaijiaju.cn

[T17] Swift：变量与常量
来源：http://ng.bjjhwx.cn

var a = 1;  let b = 2
来源：http://vn.nicolike.cn

[T18] Swift：字符串插值
来源：http://xq.521024.cn

"值: \(b)"
来源：http://he.gzmigu.cn

[T19] Swift：可选绑定
来源：http://jt.shxzukj.cn

if let n = opt { print(n) }
来源：http://ix.jianghongdianzi.cn

[T20] Swift：数组操作
来源：http://rh.shxzskj.cn

var a = [1, 2, 3];  a.append(4)
来源：http://bs.muxihuayi.cn

[T21] Swift：遍历
来源：http://im.colortex.cn

for x in a { print(x) }
来源：http://bs.szxytkj.cn

[T22] Swift：字典
来源：http://ha.huanxung.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ln.huanxung.cn

[T23] Swift：函数
来源：http://ml.huixiangedu.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ah.bookmarksfly.cn

[T24] Swift：闭包
来源：http://fo.muxihuayi.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://zg.huanxung.cn

[T25] Swift：结构体
来源：http://ar.newstarts.cn

struct P { var x: Int }
来源：http://qu.shxzukj.cn

[T26] Swift：类与重写
来源：http://jv.haigaiapp.cn

class A: Base { override func f() {} }
来源：http://mq.bjjhwx.cn

[T27] Swift：错误处理
来源：http://lh.jianghongdianzi.cn

do { try f() } catch { print(error) }
来源：http://ne.hnjuh.cn

[T28] Swift：枚举
来源：http://cv.chemitech.net.cn

enum Color { case red, green }
来源：http://um.bjjhwx.cn

[T29] Swift：guard 提前返回
来源：http://qw.shxzskj.cn

guard let x = opt else { return }
来源：http://cr.shxzukj.cn

[T30] Swift：协议
来源：http://kj.nszjky.cn

protocol Shape { func area() -> Double }
来源：http://za.huixinmuqiang.cn

[T31] Lua：Hello World
来源：http://kh.nszjky.cn

print("Hello")
来源：http://mm.chemitech.net.cn

[T32] Lua：局部变量
来源：http://nv.yuexingan06.cn

local a = 1
来源：http://uf.hahajie.cn

[T33] Lua：表（数组）
来源：http://ng.szxytkj.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://st.huanxung.cn

[T34] Lua：遍历表
来源：http://ax.hahajie.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://lm.shxzskj.cn

[T35] Lua：字典表
来源：http://sq.haigaiapp.cn

local d = { a = 1 };  d.b = 2
来源：http://yx.szxytkj.cn

[T36] Lua：函数
来源：http://kz.hahajie.cn

function add(a, b) return a + b end
来源：http://lr.wgjwhj.cn

[T37] Lua：字符串拼接
来源：http://qs.newstarts.cn

"a" .. "b"
来源：http://rp.panjiajie.cn

[T38] Lua：条件
来源：http://bx.asd995.cn

if x > 0 then print("正") end
来源：http://qy.wgjwhj.cn

[T39] Lua：模式匹配
来源：http://uu.521024.cn

string.find(s, "%d+")
来源：http://xl.huixiangedu.cn

[T40] Lua：元表
来源：http://xf.asd995.cn

setmetatable({}, { __index = base })
来源：http://cs.shxzskj.cn

[T41] Perl：Hello World
来源：http://zp.521024.cn

print "Hello\n";
来源：http://ee.huixiangedu.cn

[T42] Perl：变量类型
来源：http://us.shtwfgs.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://pi.shxzskj.cn

[T43] Perl：字符串插值
来源：http://co.huixinmuqiang.cn

"值: $a"
来源：http://hm.colortex.cn

[T44] Perl：条件
来源：http://zk.panjiajie.cn

if ($a > 0) { print "正"; }
来源：http://lc.muxihuayi.cn

[T45] Perl：数组遍历
来源：http://hm.panjiajie.cn

for my $x (@arr) { print $x; }
来源：http://yf.asd995.cn

[T46] Perl：哈希操作
来源：http://gq.asd995.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://qi.huixiangedu.cn

[T47] Perl：正则捕获
来源：http://hd.hnjuh.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://bb.lnxyls.cn

[T48] Perl：正则替换
来源：http://qz.hnjuh.cn

$s =~ s/old/new/g;
来源：http://kk.wgjwhj.cn

[T49] Perl：函数
来源：http://jv.huanxung.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://vl.newstarts.cn

[T50] Perl：逐行读文件
来源：http://ke.huixiangedu.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://eb.szxytkj.cn

while (my $line = <$fh>) { print $line; }
来源：http://vj.hahajie.cn

[T51] Scala：Hello World
来源：http://nt.nicolike.cn

println("Hello")
来源：http://ha.bookmarksfly.cn

[T52] Scala：变量
来源：http://ox.yuexingan06.cn

val a = 1;  var b = 2
来源：http://qw.shtwfgs.cn

[T53] Scala：字符串插值
来源：http://sp.chemitech.net.cn

s"值: $b"
来源：http://as.wgjwhj.cn

[T54] Scala：集合映射
来源：http://un.shxzskj.cn

List(1, 2, 3).map(_ * 2)
来源：http://iz.szsharing.cn

[T55] Scala：集合过滤
来源：http://cy.panjiajie.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ks.haigaiapp.cn

[T56] Scala：样例类
来源：http://rg.szsharing.cn

case class User(name: String, age: Int)
来源：http://ya.yuntaijiaju.cn

[T57] Scala：模式匹配
来源：http://di.yuexingan06.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://lw.hnjuh.cn

[T58] Scala：函数定义
来源：http://yu.shxzskj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://gj.chemitech.net.cn

[T59] Scala：循环
来源：http://vs.lnxyls.cn

for (i <- 1 to 10) println(i)
来源：http://og.yuntaijiaju.cn

[T60] Scala：折叠
来源：http://ir.bookmarksfly.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://bd.szsharing.cn

================================================================================
来源：http://fk.muxihuayi.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://nq.panjiajie.cn

================================================================================
来源：http://wj.szxytkj.cn

[U01] Py：创建虚拟环境
来源：http://ke.9csxet.cn

python -m venv .venv && source .venv/bin/activate
来源：http://mr.szxytkj.cn

[U02] Py：导出 / 安装依赖
来源：http://gd.newstarts.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://qn.wgjwhj.cn

[U03] Py：加载 .env 配置
来源：http://xd.bjjhwx.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ud.shtwfgs.cn

[U04] Py：变量调试打印
来源：http://na.9csxet.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ht.muxihuayi.cn

[U05] Py：列表去重且保序
来源：http://yn.huixinmuqiang.cn

list(dict.fromkeys(arr))
来源：http://cj.shxzskj.cn

[U06] Py：合并两个字典
来源：http://dv.panjiajie.cn

{**a, **b}
来源：http://pd.shxzukj.cn

[U07] Py：反转字典键值
来源：http://cn.nszjky.cn

{v: k for k, v in d.items()}
来源：http://pg.shxzskj.cn

[U08] Py：展平二维列表
来源：http://ql.hnjuh.cn

[y for x in nested for y in x]
来源：http://bf.newstarts.cn

[U09] Py：字典取最大值的键
来源：http://wt.szxytkj.cn

max(d, key=d.get)
来源：http://ah.shxzskj.cn

[U10] Py：按值排序字典
来源：http://dg.521024.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://dl.shtwfgs.cn

[U11] Py：生成器表达式
来源：http://tr.panjiajie.cn

(x * 2 for x in arr)
来源：http://cu.newstarts.cn

[U12] Py：取出现最多的 3 个元素
来源：http://km.jctech888.com.cn

Counter(arr).most_common(3)
来源：http://nw.lnxyls.cn

[U13] Py：固定长度队列
来源：http://gl.bookmarksfly.cn

deque(maxlen=10)
来源：http://wb.huixinmuqiang.cn

[U14] Py：分组收集到列表
来源：http://hr.nszjky.cn

defaultdict(list)
来源：http://ps.asd995.cn

[U15] Py：高精度计时
来源：http://mi.bookmarksfly.cn

t = time.perf_counter()
来源：http://ye.muxihuayi.cn

[U16] Py：命令行参数解析
来源：http://ed.nszjky.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mv.szsharing.cn

[U17] Py：初始化日志
来源：http://kc.huanxung.cn

logging.basicConfig(level=logging.INFO)
来源：http://tt.9csxet.cn

[U18] Py：预编译正则
来源：http://in.asd995.cn

pat = re.compile(r"\d+")
来源：http://vm.panjiajie.cn

[U19] Py：正则替换带回调
来源：http://dl.colortex.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://bd.nszjky.cn

[U20] Py：缓存函数结果
来源：http://ic.huixiangedu.cn

@functools.lru_cache(maxsize=None)
来源：http://bs.haigaiapp.cn

[U21] Py：自定义上下文管理器
来源：http://gw.jctech888.com.cn

@contextlib.contextmanager
来源：http://zz.muxihuayi.cn

[U22] Py：矩阵转置
来源：http://zp.huixiangedu.cn

list(zip(*m))
来源：http://dh.shtwfgs.cn

[U23] Py：分块读取大文件
来源：http://jg.szsharing.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://io.huixinmuqiang.cn

[U24] Py：路径操作
来源：http://yb.asd995.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ey.shxzskj.cn

[U25] Py：CSV 按字典读
来源：http://ud.huixiangedu.cn

csv.DictReader(f)
来源：http://ua.nicolike.cn

[U26] Py：并发下载
来源：http://ny.hnjuh.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wp.newstarts.cn

[U27] Py：异步 HTTP
来源：http://wn.haigaiapp.cn

aiohttp.ClientSession() 配合 async with
来源：http://sh.newstarts.cn

[U28] Py：类型别名
来源：http://tz.szsharing.cn

UserId = int
来源：http://za.shtwfgs.cn

[U29] Py：属性校验
来源：http://fk.wgjwhj.cn

@property 与 @x.setter 配合
来源：http://id.panjiajie.cn

[U30] Py：数据类
来源：http://mi.jianghongdianzi.cn

@dataclass(slots=True)
来源：http://mw.wgjwhj.cn

[U31] Py：单测
来源：http://gg.colortex.cn

python -m pytest -q
来源：http://lh.521024.cn

[U32] Py：代码格式化
来源：http://qt.jctech888.com.cn

ruff format . && ruff check --fix .
来源：http://rm.hnjuh.cn

[U33] Py：打包发布
来源：http://sp.bjjhwx.cn

python -m build  （依赖 pyproject.toml）
来源：http://ol.jctech888.com.cn

[U34] Py：判断编码
来源：http://mz.yuntaijiaju.cn

chardet.detect(raw)
来源：http://pn.asd995.cn

[U35] Py：发送邮件
来源：http://uo.colortex.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://mz.huixiangedu.cn

[U36] Py：定时任务
来源：http://gb.shxzskj.cn

schedule.every(10).minutes.do(job)
来源：http://jk.panjiajie.cn

[U37] Py：读写 Excel
来源：http://by.huixinmuqiang.cn

pandas.read_excel / DataFrame.to_excel
来源：http://je.colortex.cn

[U38] Py：获取脚本所在目录
来源：http://mo.huanxung.cn

Path(__file__).resolve().parent
来源：http://fs.yuexingan06.cn

[U39] Py：判断是否在交互环境
来源：http://so.huixinmuqiang.cn

sys.stdout.isatty()
来源：http://wo.lnxyls.cn

[U40] Py：打印到标准错误
来源：http://ml.szsharing.cn

print("err", file=sys.stderr)
来源：http://ns.hnjuh.cn

[U41] PHP：初始化 Composer 项目
来源：http://ev.szxytkj.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ml.9csxet.cn

[U42] PHP：PSR-4 自动加载
来源：http://en.hahajie.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://vj.shtwfgs.cn


<!-- 参考信息 -->