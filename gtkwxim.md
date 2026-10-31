代发 wailian999

int main(int argc, char **argv)
来源：http://fo.shtwfgs.cn

[S19] C：快速排序
来源：http://ar.gzmigu.cn

qsort(a, n, sizeof(int), cmp);
来源：http://wd.gzmigu.cn

[S20] C：二分查找
来源：http://dt.colortex.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://nj.muxihuayi.cn

[S21] C：字符类别判断
来源：http://ts.newstarts.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://vn.jianghongdianzi.cn

[S22] C：字符串转数字
来源：http://cm.haigaiapp.cn

atoi("42");  strtod("3.14", NULL);
来源：http://tu.yuntaijiaju.cn

[S23] C：随机数
来源：http://yo.szsharing.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ls.yuexingan06.cn

[S24] C：获取本地时间
来源：http://ey.lnxyls.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://di.haigaiapp.cn

[S25] C：内存拷贝
来源：http://vx.bookmarksfly.cn

memcpy(dst, src, n);
来源：http://ti.szsharing.cn

[S26] C：内存清零
来源：http://yv.yuexingan06.cn

memset(a, 0, sizeof a);
来源：http://jc.nicolike.cn

[S27] C：定义常量
来源：http://kh.szxytkj.cn

const double PI = 3.14159;
来源：http://xk.panjiajie.cn

[S28] C：静态变量
来源：http://vf.nszjky.cn

static int counter = 0;
来源：http://nl.chemitech.net.cn

[S29] C：变参函数
来源：http://nr.bjjhwx.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hx.shxzskj.cn

[S30] C：头文件保护
来源：http://nb.jctech888.com.cn

#ifndef X_H
来源：http://gj.shxzukj.cn

#define X_H
来源：http://jx.521024.cn

#endif
来源：http://ij.nicolike.cn

[S31] C++：Hello World
来源：http://bn.huixinmuqiang.cn

#include <iostream>
来源：http://pm.haigaiapp.cn

int main() { std::cout << "Hello\n"; }
来源：http://nq.bjjhwx.cn

[S32] C++：字符串
来源：http://ng.szxytkj.cn

std::string s = "hi";  s += "!";
来源：http://rn.chemitech.net.cn

[S33] C++：vector 增删
来源：http://jv.huixiangedu.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://xd.huixinmuqiang.cn

[S34] C++：遍历 vector
来源：http://by.yuntaijiaju.cn

for (auto &x : v) { std::cout << x; }
来源：http://lp.bjjhwx.cn

[S35] C++：map
来源：http://qi.jianghongdianzi.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://vl.lnxyls.cn

[S36] C++：unordered_map
来源：http://ye.yuexingan06.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://px.jctech888.com.cn

[S37] C++：set
来源：http://zx.shxzskj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://dg.gzmigu.cn

[S38] C++：排序
来源：http://eo.wgjwhj.cn

std::sort(v.begin(), v.end());
来源：http://mh.nszjky.cn

[S39] C++：自定义比较器排序
来源：http://ld.newstarts.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://yk.521024.cn

[S40] C++：查找元素
来源：http://yv.hnjuh.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://sb.hahajie.cn

[S41] C++：类与构造函数
来源：http://ud.huixiangedu.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://qa.haigaiapp.cn

[S42] C++：继承与虚函数
来源：http://cr.yuntaijiaju.cn

class B : public Base { public: void f() override {} };
来源：http://ha.yuntaijiaju.cn

[S43] C++：智能指针
来源：http://vq.huixinmuqiang.cn

auto p = std::make_unique<int>(5);
来源：http://tb.9csxet.cn

[S44] C++：引用传参
来源：http://qh.yuntaijiaju.cn

void inc(int &x) { ++x; }
来源：http://cr.huixiangedu.cn

[S45] C++：lambda
来源：http://jx.muxihuayi.cn

auto add = [](int a, int b) { return a + b; };
来源：http://rb.hahajie.cn

[S46] C++：函数模板
来源：http://ee.muxihuayi.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://en.haigaiapp.cn

[S47] C++：结构化绑定遍历
来源：http://bn.wgjwhj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qw.shxzskj.cn

[S48] C++：逐行读文件
来源：http://qq.colortex.cn

std::ifstream in("a.txt");  std::string line;
来源：http://xz.nszjky.cn

while (std::getline(in, line)) { }
来源：http://pw.szxytkj.cn

[S49] C++：写文件
来源：http://eb.asd995.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mr.9csxet.cn

[S50] C++：格式化数字
来源：http://mt.huixinmuqiang.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://jw.szsharing.cn

[S51] C++：显式类型转换
来源：http://kb.haigaiapp.cn

static_cast<double>(a) / b
来源：http://pq.bookmarksfly.cn

[S52] C++：const 与 noexcept
来源：http://cu.shxzskj.cn

int size() const noexcept { return n_; }
来源：http://gb.szsharing.cn

[S53] C++：移动语义
来源：http://sv.jctech888.com.cn

std::vector<int> w = std::move(v);
来源：http://io.lnxyls.cn

[S54] C++：异常处理
来源：http://wf.shxzskj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://zp.521024.cn

[S55] C++：结构化绑定
来源：http://ww.chemitech.net.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://yl.huixiangedu.cn

[S56] C++：optional
来源：http://ki.gzmigu.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://qt.bjjhwx.cn

[S57] C++：编译期常量
来源：http://zy.chemitech.net.cn

constexpr int N = 10;
来源：http://of.jctech888.com.cn

[S58] C++：命名空间
来源：http://nq.shxzukj.cn

namespace ns { int f() { return 1; } }
来源：http://jl.lnxyls.cn

[S59] C++：静态断言
来源：http://sb.9csxet.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fd.nicolike.cn

[S60] C++：遍历并删除元素
来源：http://za.jianghongdianzi.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ne.muxihuayi.cn

================================================================================
来源：http://mx.panjiajie.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://eo.521024.cn

================================================================================
来源：http://xv.huixinmuqiang.cn

[T01] Kotlin：Hello World
来源：http://qt.lnxyls.cn

println("Hello")
来源：http://tj.yuntaijiaju.cn

[T02] Kotlin：变量
来源：http://be.wgjwhj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://dk.jctech888.com.cn

[T03] Kotlin：字符串模板
来源：http://ko.nszjky.cn

"值: $b"
来源：http://rv.colortex.cn

[T04] Kotlin：空安全
来源：http://oa.asd995.cn

val n: String? = null;  n?.length
来源：http://mh.shxzskj.cn

[T05] Kotlin：when 表达式
来源：http://rr.yuexingan06.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ko.yuntaijiaju.cn

[T06] Kotlin：集合映射
来源：http://kx.panjiajie.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://zv.9csxet.cn

[T07] Kotlin：集合过滤
来源：http://ny.panjiajie.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://nd.huanxung.cn

[T08] Kotlin：数据类
来源：http://fs.shtwfgs.cn

data class User(val name: String, val age: Int)
来源：http://lh.nszjky.cn

[T09] Kotlin：扩展函数
来源：http://ai.hahajie.cn

fun String.exclaim() = this + "!"
来源：http://pg.haigaiapp.cn

[T10] Kotlin：默认参数
来源：http://ag.shxzskj.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ks.haigaiapp.cn

[T11] Kotlin：协程
来源：http://no.huixiangedu.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://zw.huanxung.cn

[T12] Kotlin：解构声明
来源：http://vm.yuexingan06.cn

val (a, b) = Pair(1, 2)
来源：http://mq.haigaiapp.cn

[T13] Kotlin：只读 Map
来源：http://vp.shtwfgs.cn

val m = mapOf("a" to 1)
来源：http://zl.9csxet.cn

[T14] Kotlin：循环
来源：http://yp.haigaiapp.cn

for (i in 1..10) println(i)
来源：http://sy.shxzukj.cn

[T15] Kotlin：接口
来源：http://od.huanxung.cn

interface Shape { fun area(): Double }
来源：http://vn.colortex.cn

[T16] Swift：Hello World
来源：http://au.shtwfgs.cn

print("Hello")
来源：http://px.jianghongdianzi.cn

[T17] Swift：变量与常量
来源：http://qj.bjjhwx.cn

var a = 1;  let b = 2
来源：http://ew.nicolike.cn

[T18] Swift：字符串插值
来源：http://oj.521024.cn

"值: \(b)"
来源：http://vx.yuexingan06.cn

[T19] Swift：可选绑定
来源：http://vy.wgjwhj.cn

if let n = opt { print(n) }
来源：http://ax.huixinmuqiang.cn

[T20] Swift：数组操作
来源：http://ba.huixinmuqiang.cn

var a = [1, 2, 3];  a.append(4)
来源：http://pg.szxytkj.cn

[T21] Swift：遍历
来源：http://yk.hahajie.cn

for x in a { print(x) }
来源：http://bx.9csxet.cn

[T22] Swift：字典
来源：http://rb.wgjwhj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://vl.yuntaijiaju.cn

[T23] Swift：函数
来源：http://ei.huixinmuqiang.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ax.9csxet.cn

[T24] Swift：闭包
来源：http://fl.shxzukj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://cv.hnjuh.cn

[T25] Swift：结构体
来源：http://dg.yuntaijiaju.cn

struct P { var x: Int }
来源：http://hb.szxytkj.cn

[T26] Swift：类与重写
来源：http://ud.shxzukj.cn

class A: Base { override func f() {} }
来源：http://sl.jctech888.com.cn

[T27] Swift：错误处理
来源：http://xl.shtwfgs.cn

do { try f() } catch { print(error) }
来源：http://vb.haigaiapp.cn

[T28] Swift：枚举
来源：http://kf.shxzskj.cn

enum Color { case red, green }
来源：http://ht.chemitech.net.cn

[T29] Swift：guard 提前返回
来源：http://ev.521024.cn

guard let x = opt else { return }
来源：http://sp.szsharing.cn

[T30] Swift：协议
来源：http://zt.hahajie.cn

protocol Shape { func area() -> Double }
来源：http://an.shxzukj.cn

[T31] Lua：Hello World
来源：http://ts.szsharing.cn

print("Hello")
来源：http://jo.hahajie.cn

[T32] Lua：局部变量
来源：http://gz.gzmigu.cn

local a = 1
来源：http://vi.gzmigu.cn

[T33] Lua：表（数组）
来源：http://le.bjjhwx.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://fi.bookmarksfly.cn

[T34] Lua：遍历表
来源：http://ap.nszjky.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ah.hnjuh.cn

[T35] Lua：字典表
来源：http://xy.shxzukj.cn

local d = { a = 1 };  d.b = 2
来源：http://jp.bookmarksfly.cn

[T36] Lua：函数
来源：http://uh.bjjhwx.cn

function add(a, b) return a + b end
来源：http://kq.shtwfgs.cn

[T37] Lua：字符串拼接
来源：http://cl.521024.cn

"a" .. "b"
来源：http://up.haigaiapp.cn

[T38] Lua：条件
来源：http://ns.colortex.cn

if x > 0 then print("正") end
来源：http://fr.huixiangedu.cn

[T39] Lua：模式匹配
来源：http://oi.huixinmuqiang.cn

string.find(s, "%d+")
来源：http://yb.colortex.cn

[T40] Lua：元表
来源：http://td.haigaiapp.cn

setmetatable({}, { __index = base })
来源：http://dt.huanxung.cn

[T41] Perl：Hello World
来源：http://em.jctech888.com.cn

print "Hello\n";
来源：http://ss.9csxet.cn

[T42] Perl：变量类型
来源：http://mp.yuexingan06.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ja.huixinmuqiang.cn

[T43] Perl：字符串插值
来源：http://wd.panjiajie.cn

"值: $a"
来源：http://uv.haigaiapp.cn

[T44] Perl：条件
来源：http://ck.521024.cn

if ($a > 0) { print "正"; }
来源：http://cp.nszjky.cn

[T45] Perl：数组遍历
来源：http://tx.haigaiapp.cn

for my $x (@arr) { print $x; }
来源：http://lz.szsharing.cn

[T46] Perl：哈希操作
来源：http://zi.hnjuh.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://rp.panjiajie.cn

[T47] Perl：正则捕获
来源：http://qn.hahajie.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://wu.yuexingan06.cn

[T48] Perl：正则替换
来源：http://hd.shtwfgs.cn

$s =~ s/old/new/g;
来源：http://ps.colortex.cn

[T49] Perl：函数
来源：http://au.haigaiapp.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://vw.yuntaijiaju.cn

[T50] Perl：逐行读文件
来源：http://qs.huixiangedu.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://mb.nszjky.cn

while (my $line = <$fh>) { print $line; }
来源：http://hl.jianghongdianzi.cn

[T51] Scala：Hello World
来源：http://mz.newstarts.cn

println("Hello")
来源：http://cp.haigaiapp.cn

[T52] Scala：变量
来源：http://lw.nszjky.cn

val a = 1;  var b = 2
来源：http://os.bookmarksfly.cn

[T53] Scala：字符串插值
来源：http://bi.nszjky.cn

s"值: $b"
来源：http://qv.wgjwhj.cn

[T54] Scala：集合映射
来源：http://fn.yuexingan06.cn

List(1, 2, 3).map(_ * 2)
来源：http://qf.bookmarksfly.cn

[T55] Scala：集合过滤
来源：http://aw.hnjuh.cn

List(1, 2, 3).filter(_ > 1)
来源：http://lw.shtwfgs.cn

[T56] Scala：样例类
来源：http://ge.shtwfgs.cn

case class User(name: String, age: Int)
来源：http://rr.yuexingan06.cn

[T57] Scala：模式匹配
来源：http://ib.panjiajie.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ct.asd995.cn

[T58] Scala：函数定义
来源：http://ij.muxihuayi.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ni.panjiajie.cn

[T59] Scala：循环
来源：http://wf.asd995.cn

for (i <- 1 to 10) println(i)
来源：http://jj.huanxung.cn

[T60] Scala：折叠
来源：http://dp.gzmigu.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://cf.haigaiapp.cn

================================================================================
来源：http://rd.lnxyls.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://em.szxytkj.cn

================================================================================
来源：http://bk.muxihuayi.cn

[U01] Py：创建虚拟环境
来源：http://lt.gzmigu.cn

python -m venv .venv && source .venv/bin/activate
来源：http://pd.szxytkj.cn

[U02] Py：导出 / 安装依赖
来源：http://oq.yuexingan06.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://tf.bookmarksfly.cn

[U03] Py：加载 .env 配置
来源：http://fp.shxzukj.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://jf.huanxung.cn

[U04] Py：变量调试打印
来源：http://jx.wgjwhj.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://tw.9csxet.cn

[U05] Py：列表去重且保序
来源：http://np.yuntaijiaju.cn

list(dict.fromkeys(arr))
来源：http://eb.huanxung.cn

[U06] Py：合并两个字典
来源：http://zb.bjjhwx.cn

{**a, **b}
来源：http://mj.hnjuh.cn

[U07] Py：反转字典键值
来源：http://ee.huixiangedu.cn

{v: k for k, v in d.items()}
来源：http://xu.wgjwhj.cn

[U08] Py：展平二维列表
来源：http://ba.shxzskj.cn

[y for x in nested for y in x]
来源：http://eq.gzmigu.cn

[U09] Py：字典取最大值的键
来源：http://qx.haigaiapp.cn

max(d, key=d.get)
来源：http://aw.yuntaijiaju.cn

[U10] Py：按值排序字典
来源：http://tl.yuexingan06.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ot.colortex.cn

[U11] Py：生成器表达式
来源：http://lp.jianghongdianzi.cn

(x * 2 for x in arr)
来源：http://fl.lnxyls.cn

[U12] Py：取出现最多的 3 个元素
来源：http://bm.jianghongdianzi.cn

Counter(arr).most_common(3)
来源：http://te.shxzukj.cn

[U13] Py：固定长度队列
来源：http://dz.jianghongdianzi.cn

deque(maxlen=10)
来源：http://tn.asd995.cn

[U14] Py：分组收集到列表
来源：http://tj.jianghongdianzi.cn

defaultdict(list)
来源：http://un.huixiangedu.cn

[U15] Py：高精度计时
来源：http://gz.nszjky.cn

t = time.perf_counter()
来源：http://gz.521024.cn

[U16] Py：命令行参数解析
来源：http://qu.bjjhwx.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://me.chemitech.net.cn

[U17] Py：初始化日志
来源：http://ob.chemitech.net.cn

logging.basicConfig(level=logging.INFO)
来源：http://dy.bjjhwx.cn

[U18] Py：预编译正则
来源：http://dy.lnxyls.cn

pat = re.compile(r"\d+")
来源：http://dj.huanxung.cn

[U19] Py：正则替换带回调
来源：http://hk.9csxet.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://if.hahajie.cn

[U20] Py：缓存函数结果
来源：http://zs.yuntaijiaju.cn

@functools.lru_cache(maxsize=None)
来源：http://ao.huixiangedu.cn

[U21] Py：自定义上下文管理器
来源：http://gf.szsharing.cn

@contextlib.contextmanager
来源：http://ib.jctech888.com.cn

[U22] Py：矩阵转置
来源：http://ni.jianghongdianzi.cn

list(zip(*m))
来源：http://ch.nszjky.cn

[U23] Py：分块读取大文件
来源：http://je.szsharing.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ws.huanxung.cn

[U24] Py：路径操作
来源：http://eb.bookmarksfly.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://kp.muxihuayi.cn

[U25] Py：CSV 按字典读
来源：http://rp.jianghongdianzi.cn

csv.DictReader(f)
来源：http://es.bjjhwx.cn

[U26] Py：并发下载
来源：http://kf.colortex.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ef.nszjky.cn

[U27] Py：异步 HTTP
来源：http://mh.bookmarksfly.cn

aiohttp.ClientSession() 配合 async with
来源：http://vr.shxzukj.cn

[U28] Py：类型别名
来源：http://ei.hnjuh.cn

UserId = int
来源：http://pt.shxzskj.cn

[U29] Py：属性校验
来源：http://ob.bookmarksfly.cn

@property 与 @x.setter 配合
来源：http://sw.shxzskj.cn

[U30] Py：数据类
来源：http://sv.huixiangedu.cn

@dataclass(slots=True)
来源：http://wi.nszjky.cn

[U31] Py：单测
来源：http://ac.jianghongdianzi.cn

python -m pytest -q
来源：http://ev.huanxung.cn

[U32] Py：代码格式化
来源：http://gz.shxzskj.cn

ruff format . && ruff check --fix .
来源：http://ll.shxzskj.cn

[U33] Py：打包发布
来源：http://ly.nszjky.cn

python -m build  （依赖 pyproject.toml）
来源：http://hv.shtwfgs.cn

[U34] Py：判断编码
来源：http://cv.haigaiapp.cn

chardet.detect(raw)
来源：http://et.muxihuayi.cn

[U35] Py：发送邮件
来源：http://ym.yuexingan06.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ik.colortex.cn

[U36] Py：定时任务
来源：http://ue.muxihuayi.cn

schedule.every(10).minutes.do(job)
来源：http://of.bookmarksfly.cn

[U37] Py：读写 Excel
来源：http://nq.9csxet.cn

pandas.read_excel / DataFrame.to_excel
来源：http://yd.lnxyls.cn

[U38] Py：获取脚本所在目录
来源：http://df.lnxyls.cn

Path(__file__).resolve().parent
来源：http://yi.szxytkj.cn

[U39] Py：判断是否在交互环境
来源：http://mr.huixinmuqiang.cn

sys.stdout.isatty()
来源：http://wv.jctech888.com.cn

[U40] Py：打印到标准错误
来源：http://lg.szsharing.cn

print("err", file=sys.stderr)
来源：http://tu.yuntaijiaju.cn

[U41] PHP：初始化 Composer 项目
来源：http://mt.yuntaijiaju.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://sk.gzmigu.cn

[U42] PHP：PSR-4 自动加载
来源：http://dw.nszjky.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://qe.haigaiapp.cn


<!-- 参考信息 -->