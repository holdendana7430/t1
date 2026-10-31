代发 wailian999

int main(int argc, char **argv)
来源：http://dw.hnjuh.cn

[S19] C：快速排序
来源：http://xn.szsharing.cn

qsort(a, n, sizeof(int), cmp);
来源：http://cv.bjjhwx.cn

[S20] C：二分查找
来源：http://wv.newstarts.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://xf.bjjhwx.cn

[S21] C：字符类别判断
来源：http://yl.huixiangedu.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://lw.huixinmuqiang.cn

[S22] C：字符串转数字
来源：http://ux.lnxyls.cn

atoi("42");  strtod("3.14", NULL);
来源：http://bc.shxzukj.cn

[S23] C：随机数
来源：http://ix.nszjky.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://gi.huixiangedu.cn

[S24] C：获取本地时间
来源：http://xn.gzmigu.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://dy.521024.cn

[S25] C：内存拷贝
来源：http://hn.huixiangedu.cn

memcpy(dst, src, n);
来源：http://mf.nicolike.cn

[S26] C：内存清零
来源：http://uz.shxzskj.cn

memset(a, 0, sizeof a);
来源：http://fe.haigaiapp.cn

[S27] C：定义常量
来源：http://ms.gzmigu.cn

const double PI = 3.14159;
来源：http://no.shxzukj.cn

[S28] C：静态变量
来源：http://kv.shxzskj.cn

static int counter = 0;
来源：http://so.hahajie.cn

[S29] C：变参函数
来源：http://du.szxytkj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ls.newstarts.cn

[S30] C：头文件保护
来源：http://mi.shtwfgs.cn

#ifndef X_H
来源：http://jc.haigaiapp.cn

#define X_H
来源：http://wh.muxihuayi.cn

#endif
来源：http://fb.bookmarksfly.cn

[S31] C++：Hello World
来源：http://qb.gzmigu.cn

#include <iostream>
来源：http://mz.szsharing.cn

int main() { std::cout << "Hello\n"; }
来源：http://lp.wgjwhj.cn

[S32] C++：字符串
来源：http://qg.hnjuh.cn

std::string s = "hi";  s += "!";
来源：http://dg.haigaiapp.cn

[S33] C++：vector 增删
来源：http://ic.szxytkj.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hy.huixinmuqiang.cn

[S34] C++：遍历 vector
来源：http://qk.jianghongdianzi.cn

for (auto &x : v) { std::cout << x; }
来源：http://vy.muxihuayi.cn

[S35] C++：map
来源：http://mn.yuexingan06.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://lo.521024.cn

[S36] C++：unordered_map
来源：http://ae.huixiangedu.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ha.bookmarksfly.cn

[S37] C++：set
来源：http://jd.szxytkj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://wr.hnjuh.cn

[S38] C++：排序
来源：http://lq.gzmigu.cn

std::sort(v.begin(), v.end());
来源：http://ux.yuexingan06.cn

[S39] C++：自定义比较器排序
来源：http://uv.jctech888.com.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://zt.hnjuh.cn

[S40] C++：查找元素
来源：http://pk.shtwfgs.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://tz.jianghongdianzi.cn

[S41] C++：类与构造函数
来源：http://mo.gzmigu.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ju.gzmigu.cn

[S42] C++：继承与虚函数
来源：http://sj.bjjhwx.cn

class B : public Base { public: void f() override {} };
来源：http://rc.521024.cn

[S43] C++：智能指针
来源：http://md.newstarts.cn

auto p = std::make_unique<int>(5);
来源：http://ma.szxytkj.cn

[S44] C++：引用传参
来源：http://dy.nszjky.cn

void inc(int &x) { ++x; }
来源：http://ji.szxytkj.cn

[S45] C++：lambda
来源：http://an.szxytkj.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ph.szxytkj.cn

[S46] C++：函数模板
来源：http://yd.wgjwhj.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://mo.huixiangedu.cn

[S47] C++：结构化绑定遍历
来源：http://id.shxzukj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://oy.shxzskj.cn

[S48] C++：逐行读文件
来源：http://oy.shxzskj.cn

std::ifstream in("a.txt");  std::string line;
来源：http://jo.wgjwhj.cn

while (std::getline(in, line)) { }
来源：http://gn.nszjky.cn

[S49] C++：写文件
来源：http://rh.asd995.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://te.yuexingan06.cn

[S50] C++：格式化数字
来源：http://fu.newstarts.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ng.panjiajie.cn

[S51] C++：显式类型转换
来源：http://yx.haigaiapp.cn

static_cast<double>(a) / b
来源：http://bs.jianghongdianzi.cn

[S52] C++：const 与 noexcept
来源：http://bl.jctech888.com.cn

int size() const noexcept { return n_; }
来源：http://kt.521024.cn

[S53] C++：移动语义
来源：http://ci.jianghongdianzi.cn

std::vector<int> w = std::move(v);
来源：http://op.hnjuh.cn

[S54] C++：异常处理
来源：http://we.9csxet.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://tb.panjiajie.cn

[S55] C++：结构化绑定
来源：http://fh.huanxung.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://xi.chemitech.net.cn

[S56] C++：optional
来源：http://tv.szsharing.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wx.lnxyls.cn

[S57] C++：编译期常量
来源：http://zx.haigaiapp.cn

constexpr int N = 10;
来源：http://hb.lnxyls.cn

[S58] C++：命名空间
来源：http://kq.jianghongdianzi.cn

namespace ns { int f() { return 1; } }
来源：http://tz.szxytkj.cn

[S59] C++：静态断言
来源：http://en.hahajie.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fr.muxihuayi.cn

[S60] C++：遍历并删除元素
来源：http://kr.jianghongdianzi.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://en.bookmarksfly.cn

================================================================================
来源：http://yp.shxzukj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://yq.jianghongdianzi.cn

================================================================================
来源：http://mz.jctech888.com.cn

[T01] Kotlin：Hello World
来源：http://yz.asd995.cn

println("Hello")
来源：http://tc.chemitech.net.cn

[T02] Kotlin：变量
来源：http://ed.bookmarksfly.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://zd.9csxet.cn

[T03] Kotlin：字符串模板
来源：http://vm.nicolike.cn

"值: $b"
来源：http://av.shxzukj.cn

[T04] Kotlin：空安全
来源：http://hn.shtwfgs.cn

val n: String? = null;  n?.length
来源：http://gv.jianghongdianzi.cn

[T05] Kotlin：when 表达式
来源：http://ev.jianghongdianzi.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ei.bjjhwx.cn

[T06] Kotlin：集合映射
来源：http://hp.shxzskj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://tn.jianghongdianzi.cn

[T07] Kotlin：集合过滤
来源：http://rq.nicolike.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://fz.szxytkj.cn

[T08] Kotlin：数据类
来源：http://wb.huixiangedu.cn

data class User(val name: String, val age: Int)
来源：http://vd.nszjky.cn

[T09] Kotlin：扩展函数
来源：http://im.shxzukj.cn

fun String.exclaim() = this + "!"
来源：http://wd.newstarts.cn

[T10] Kotlin：默认参数
来源：http://gs.haigaiapp.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://yk.szxytkj.cn

[T11] Kotlin：协程
来源：http://om.shxzskj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://wd.lnxyls.cn

[T12] Kotlin：解构声明
来源：http://th.nszjky.cn

val (a, b) = Pair(1, 2)
来源：http://ta.yuntaijiaju.cn

[T13] Kotlin：只读 Map
来源：http://qm.chemitech.net.cn

val m = mapOf("a" to 1)
来源：http://sm.huanxung.cn

[T14] Kotlin：循环
来源：http://kl.521024.cn

for (i in 1..10) println(i)
来源：http://co.hnjuh.cn

[T15] Kotlin：接口
来源：http://lo.haigaiapp.cn

interface Shape { fun area(): Double }
来源：http://as.gzmigu.cn

[T16] Swift：Hello World
来源：http://bf.hnjuh.cn

print("Hello")
来源：http://sj.huixinmuqiang.cn

[T17] Swift：变量与常量
来源：http://ps.gzmigu.cn

var a = 1;  let b = 2
来源：http://pt.asd995.cn

[T18] Swift：字符串插值
来源：http://jr.521024.cn

"值: \(b)"
来源：http://vf.hnjuh.cn

[T19] Swift：可选绑定
来源：http://ug.colortex.cn

if let n = opt { print(n) }
来源：http://bn.huixiangedu.cn

[T20] Swift：数组操作
来源：http://qr.huixinmuqiang.cn

var a = [1, 2, 3];  a.append(4)
来源：http://hl.yuntaijiaju.cn

[T21] Swift：遍历
来源：http://cz.huixiangedu.cn

for x in a { print(x) }
来源：http://rr.bookmarksfly.cn

[T22] Swift：字典
来源：http://gw.colortex.cn

var d = ["a": 1];  d["b"] = 2
来源：http://kq.newstarts.cn

[T23] Swift：函数
来源：http://ee.jctech888.com.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://aj.bjjhwx.cn

[T24] Swift：闭包
来源：http://qe.bjjhwx.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://pf.yuntaijiaju.cn

[T25] Swift：结构体
来源：http://mf.521024.cn

struct P { var x: Int }
来源：http://ba.szsharing.cn

[T26] Swift：类与重写
来源：http://qs.huanxung.cn

class A: Base { override func f() {} }
来源：http://oa.yuntaijiaju.cn

[T27] Swift：错误处理
来源：http://kl.asd995.cn

do { try f() } catch { print(error) }
来源：http://qo.hahajie.cn

[T28] Swift：枚举
来源：http://bx.huixinmuqiang.cn

enum Color { case red, green }
来源：http://ir.bjjhwx.cn

[T29] Swift：guard 提前返回
来源：http://gj.wgjwhj.cn

guard let x = opt else { return }
来源：http://nq.newstarts.cn

[T30] Swift：协议
来源：http://nr.nszjky.cn

protocol Shape { func area() -> Double }
来源：http://nn.shxzukj.cn

[T31] Lua：Hello World
来源：http://od.jianghongdianzi.cn

print("Hello")
来源：http://bt.shtwfgs.cn

[T32] Lua：局部变量
来源：http://fx.yuexingan06.cn

local a = 1
来源：http://fb.huanxung.cn

[T33] Lua：表（数组）
来源：http://iz.haigaiapp.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://vl.jianghongdianzi.cn

[T34] Lua：遍历表
来源：http://ox.nicolike.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ln.szxytkj.cn

[T35] Lua：字典表
来源：http://cw.colortex.cn

local d = { a = 1 };  d.b = 2
来源：http://lk.bookmarksfly.cn

[T36] Lua：函数
来源：http://df.gzmigu.cn

function add(a, b) return a + b end
来源：http://em.huixiangedu.cn

[T37] Lua：字符串拼接
来源：http://te.bookmarksfly.cn

"a" .. "b"
来源：http://pu.panjiajie.cn

[T38] Lua：条件
来源：http://ni.huanxung.cn

if x > 0 then print("正") end
来源：http://oe.panjiajie.cn

[T39] Lua：模式匹配
来源：http://pp.huanxung.cn

string.find(s, "%d+")
来源：http://fg.gzmigu.cn

[T40] Lua：元表
来源：http://sq.bookmarksfly.cn

setmetatable({}, { __index = base })
来源：http://tl.haigaiapp.cn

[T41] Perl：Hello World
来源：http://uz.521024.cn

print "Hello\n";
来源：http://nj.nicolike.cn

[T42] Perl：变量类型
来源：http://rr.jctech888.com.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://qe.muxihuayi.cn

[T43] Perl：字符串插值
来源：http://qo.chemitech.net.cn

"值: $a"
来源：http://qv.jctech888.com.cn

[T44] Perl：条件
来源：http://qe.haigaiapp.cn

if ($a > 0) { print "正"; }
来源：http://bs.wgjwhj.cn

[T45] Perl：数组遍历
来源：http://hf.hnjuh.cn

for my $x (@arr) { print $x; }
来源：http://wd.521024.cn

[T46] Perl：哈希操作
来源：http://th.bjjhwx.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://uc.nszjky.cn

[T47] Perl：正则捕获
来源：http://wx.bookmarksfly.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://gk.lnxyls.cn

[T48] Perl：正则替换
来源：http://xo.szxytkj.cn

$s =~ s/old/new/g;
来源：http://mz.lnxyls.cn

[T49] Perl：函数
来源：http://rr.shxzskj.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://jm.jianghongdianzi.cn

[T50] Perl：逐行读文件
来源：http://sy.colortex.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://xb.hahajie.cn

while (my $line = <$fh>) { print $line; }
来源：http://nt.yuntaijiaju.cn

[T51] Scala：Hello World
来源：http://ey.bookmarksfly.cn

println("Hello")
来源：http://df.muxihuayi.cn

[T52] Scala：变量
来源：http://ov.szsharing.cn

val a = 1;  var b = 2
来源：http://bv.huixinmuqiang.cn

[T53] Scala：字符串插值
来源：http://aw.huixinmuqiang.cn

s"值: $b"
来源：http://el.colortex.cn

[T54] Scala：集合映射
来源：http://mp.colortex.cn

List(1, 2, 3).map(_ * 2)
来源：http://od.szsharing.cn

[T55] Scala：集合过滤
来源：http://ma.huixinmuqiang.cn

List(1, 2, 3).filter(_ > 1)
来源：http://tc.wgjwhj.cn

[T56] Scala：样例类
来源：http://we.nszjky.cn

case class User(name: String, age: Int)
来源：http://ga.wgjwhj.cn

[T57] Scala：模式匹配
来源：http://je.muxihuayi.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://uy.jianghongdianzi.cn

[T58] Scala：函数定义
来源：http://hu.huixinmuqiang.cn

def add(a: Int, b: Int): Int = a + b
来源：http://cq.huixinmuqiang.cn

[T59] Scala：循环
来源：http://wm.yuntaijiaju.cn

for (i <- 1 to 10) println(i)
来源：http://kv.huixiangedu.cn

[T60] Scala：折叠
来源：http://ty.chemitech.net.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://sh.nicolike.cn

================================================================================
来源：http://tr.shxzskj.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://vv.shxzskj.cn

================================================================================
来源：http://bg.jianghongdianzi.cn

[U01] Py：创建虚拟环境
来源：http://oi.521024.cn

python -m venv .venv && source .venv/bin/activate
来源：http://qi.newstarts.cn

[U02] Py：导出 / 安装依赖
来源：http://ep.shxzukj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://nb.shtwfgs.cn

[U03] Py：加载 .env 配置
来源：http://ay.panjiajie.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://bh.hnjuh.cn

[U04] Py：变量调试打印
来源：http://bq.hnjuh.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://tz.hnjuh.cn

[U05] Py：列表去重且保序
来源：http://fq.yuntaijiaju.cn

list(dict.fromkeys(arr))
来源：http://qi.shxzukj.cn

[U06] Py：合并两个字典
来源：http://ll.hnjuh.cn

{**a, **b}
来源：http://fi.shtwfgs.cn

[U07] Py：反转字典键值
来源：http://lp.shtwfgs.cn

{v: k for k, v in d.items()}
来源：http://ok.9csxet.cn

[U08] Py：展平二维列表
来源：http://xz.521024.cn

[y for x in nested for y in x]
来源：http://hf.asd995.cn

[U09] Py：字典取最大值的键
来源：http://ol.szxytkj.cn

max(d, key=d.get)
来源：http://vf.lnxyls.cn

[U10] Py：按值排序字典
来源：http://fn.panjiajie.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://gt.lnxyls.cn

[U11] Py：生成器表达式
来源：http://ok.muxihuayi.cn

(x * 2 for x in arr)
来源：http://af.haigaiapp.cn

[U12] Py：取出现最多的 3 个元素
来源：http://tu.nszjky.cn

Counter(arr).most_common(3)
来源：http://qf.521024.cn

[U13] Py：固定长度队列
来源：http://xo.jctech888.com.cn

deque(maxlen=10)
来源：http://ft.muxihuayi.cn

[U14] Py：分组收集到列表
来源：http://ye.521024.cn

defaultdict(list)
来源：http://nv.asd995.cn

[U15] Py：高精度计时
来源：http://fc.asd995.cn

t = time.perf_counter()
来源：http://ao.yuexingan06.cn

[U16] Py：命令行参数解析
来源：http://bm.asd995.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ll.bookmarksfly.cn

[U17] Py：初始化日志
来源：http://um.panjiajie.cn

logging.basicConfig(level=logging.INFO)
来源：http://cm.huanxung.cn

[U18] Py：预编译正则
来源：http://qs.huanxung.cn

pat = re.compile(r"\d+")
来源：http://tm.muxihuayi.cn

[U19] Py：正则替换带回调
来源：http://yq.nicolike.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://iw.newstarts.cn

[U20] Py：缓存函数结果
来源：http://tw.shxzskj.cn

@functools.lru_cache(maxsize=None)
来源：http://xi.muxihuayi.cn

[U21] Py：自定义上下文管理器
来源：http://sa.asd995.cn

@contextlib.contextmanager
来源：http://ab.bjjhwx.cn

[U22] Py：矩阵转置
来源：http://pt.jctech888.com.cn

list(zip(*m))
来源：http://ib.huanxung.cn

[U23] Py：分块读取大文件
来源：http://rf.521024.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://gj.colortex.cn

[U24] Py：路径操作
来源：http://fe.jianghongdianzi.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://np.yuexingan06.cn

[U25] Py：CSV 按字典读
来源：http://yi.wgjwhj.cn

csv.DictReader(f)
来源：http://hn.shxzskj.cn

[U26] Py：并发下载
来源：http://gq.haigaiapp.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://tp.nszjky.cn

[U27] Py：异步 HTTP
来源：http://wy.asd995.cn

aiohttp.ClientSession() 配合 async with
来源：http://vv.shtwfgs.cn

[U28] Py：类型别名
来源：http://yi.hnjuh.cn

UserId = int
来源：http://jc.yuntaijiaju.cn

[U29] Py：属性校验
来源：http://ht.newstarts.cn

@property 与 @x.setter 配合
来源：http://nw.huanxung.cn

[U30] Py：数据类
来源：http://wr.muxihuayi.cn

@dataclass(slots=True)
来源：http://nk.bjjhwx.cn

[U31] Py：单测
来源：http://pz.9csxet.cn

python -m pytest -q
来源：http://gt.huixinmuqiang.cn

[U32] Py：代码格式化
来源：http://lc.wgjwhj.cn

ruff format . && ruff check --fix .
来源：http://rq.wgjwhj.cn

[U33] Py：打包发布
来源：http://bq.hahajie.cn

python -m build  （依赖 pyproject.toml）
来源：http://je.jctech888.com.cn

[U34] Py：判断编码
来源：http://ut.lnxyls.cn

chardet.detect(raw)
来源：http://lx.shtwfgs.cn

[U35] Py：发送邮件
来源：http://ks.gzmigu.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ow.shxzskj.cn

[U36] Py：定时任务
来源：http://wj.muxihuayi.cn

schedule.every(10).minutes.do(job)
来源：http://nc.gzmigu.cn

[U37] Py：读写 Excel
来源：http://pd.bookmarksfly.cn

pandas.read_excel / DataFrame.to_excel
来源：http://zl.shxzskj.cn

[U38] Py：获取脚本所在目录
来源：http://ad.huanxung.cn

Path(__file__).resolve().parent
来源：http://bz.shtwfgs.cn

[U39] Py：判断是否在交互环境
来源：http://qx.szxytkj.cn

sys.stdout.isatty()
来源：http://rd.haigaiapp.cn

[U40] Py：打印到标准错误
来源：http://td.shxzukj.cn

print("err", file=sys.stderr)
来源：http://ke.hnjuh.cn

[U41] PHP：初始化 Composer 项目
来源：http://ce.jctech888.com.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://mu.hahajie.cn

[U42] PHP：PSR-4 自动加载
来源：http://wu.bjjhwx.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://fu.521024.cn


<!-- 参考信息 -->