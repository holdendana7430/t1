代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qg.521024.cn

[S21] C：字符类别判断
来源：http://nt.bookmarksfly.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wg.hnjuh.cn

[S22] C：字符串转数字
来源：http://am.huixiangedu.cn

atoi("42");  strtod("3.14", NULL);
来源：http://wc.huixinmuqiang.cn

[S23] C：随机数
来源：http://hv.muxihuayi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://qt.muxihuayi.cn

[S24] C：获取本地时间
来源：http://vk.hnjuh.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://op.szsharing.cn

[S25] C：内存拷贝
来源：http://po.muxihuayi.cn

memcpy(dst, src, n);
来源：http://ml.huixinmuqiang.cn

[S26] C：内存清零
来源：http://ch.jctech888.com.cn

memset(a, 0, sizeof a);
来源：http://my.lnxyls.cn

[S27] C：定义常量
来源：http://lj.bookmarksfly.cn

const double PI = 3.14159;
来源：http://cm.chemitech.net.cn

[S28] C：静态变量
来源：http://ak.521024.cn

static int counter = 0;
来源：http://rv.521024.cn

[S29] C：变参函数
来源：http://jb.newstarts.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://gg.muxihuayi.cn

[S30] C：头文件保护
来源：http://gl.521024.cn

#ifndef X_H
来源：http://kt.huixinmuqiang.cn

#define X_H
来源：http://js.yuntaijiaju.cn

#endif
来源：http://mf.gzmigu.cn

[S31] C++：Hello World
来源：http://od.haigaiapp.cn

#include <iostream>
来源：http://lg.lnxyls.cn

int main() { std::cout << "Hello\n"; }
来源：http://vm.huixinmuqiang.cn

[S32] C++：字符串
来源：http://lc.lnxyls.cn

std::string s = "hi";  s += "!";
来源：http://vi.wgjwhj.cn

[S33] C++：vector 增删
来源：http://ju.shxzukj.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://dw.jctech888.com.cn

[S34] C++：遍历 vector
来源：http://hn.bookmarksfly.cn

for (auto &x : v) { std::cout << x; }
来源：http://ro.bjjhwx.cn

[S35] C++：map
来源：http://tf.colortex.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://gq.jianghongdianzi.cn

[S36] C++：unordered_map
来源：http://yr.huixiangedu.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hg.shxzskj.cn

[S37] C++：set
来源：http://hw.shxzskj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://vc.szxytkj.cn

[S38] C++：排序
来源：http://mb.521024.cn

std::sort(v.begin(), v.end());
来源：http://zm.jianghongdianzi.cn

[S39] C++：自定义比较器排序
来源：http://bf.yuntaijiaju.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ee.colortex.cn

[S40] C++：查找元素
来源：http://je.panjiajie.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ng.panjiajie.cn

[S41] C++：类与构造函数
来源：http://kz.yuexingan06.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hb.bookmarksfly.cn

[S42] C++：继承与虚函数
来源：http://mv.jianghongdianzi.cn

class B : public Base { public: void f() override {} };
来源：http://sg.huixinmuqiang.cn

[S43] C++：智能指针
来源：http://fs.huanxung.cn

auto p = std::make_unique<int>(5);
来源：http://yb.huixinmuqiang.cn

[S44] C++：引用传参
来源：http://jx.yuntaijiaju.cn

void inc(int &x) { ++x; }
来源：http://rb.shxzskj.cn

[S45] C++：lambda
来源：http://ly.9csxet.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ug.shtwfgs.cn

[S46] C++：函数模板
来源：http://nh.hahajie.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://tm.szxytkj.cn

[S47] C++：结构化绑定遍历
来源：http://nf.gzmigu.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ri.jianghongdianzi.cn

[S48] C++：逐行读文件
来源：http://pk.bjjhwx.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ck.panjiajie.cn

while (std::getline(in, line)) { }
来源：http://gj.szxytkj.cn

[S49] C++：写文件
来源：http://wd.hahajie.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://kl.asd995.cn

[S50] C++：格式化数字
来源：http://ei.nicolike.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://go.huixinmuqiang.cn

[S51] C++：显式类型转换
来源：http://nq.bjjhwx.cn

static_cast<double>(a) / b
来源：http://te.szxytkj.cn

[S52] C++：const 与 noexcept
来源：http://yh.521024.cn

int size() const noexcept { return n_; }
来源：http://uj.newstarts.cn

[S53] C++：移动语义
来源：http://va.hahajie.cn

std::vector<int> w = std::move(v);
来源：http://dk.9csxet.cn

[S54] C++：异常处理
来源：http://ci.yuntaijiaju.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mo.panjiajie.cn

[S55] C++：结构化绑定
来源：http://qf.yuexingan06.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://wh.huanxung.cn

[S56] C++：optional
来源：http://qc.szxytkj.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://gu.nicolike.cn

[S57] C++：编译期常量
来源：http://uk.bookmarksfly.cn

constexpr int N = 10;
来源：http://je.bookmarksfly.cn

[S58] C++：命名空间
来源：http://hf.szxytkj.cn

namespace ns { int f() { return 1; } }
来源：http://nl.bjjhwx.cn

[S59] C++：静态断言
来源：http://hn.521024.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://vj.chemitech.net.cn

[S60] C++：遍历并删除元素
来源：http://if.yuntaijiaju.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hu.9csxet.cn

================================================================================
来源：http://ov.521024.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://qn.521024.cn

================================================================================
来源：http://bw.huixiangedu.cn

[T01] Kotlin：Hello World
来源：http://pj.chemitech.net.cn

println("Hello")
来源：http://xc.yuntaijiaju.cn

[T02] Kotlin：变量
来源：http://xc.jianghongdianzi.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://go.yuexingan06.cn

[T03] Kotlin：字符串模板
来源：http://mb.shxzskj.cn

"值: $b"
来源：http://mv.shxzskj.cn

[T04] Kotlin：空安全
来源：http://zc.panjiajie.cn

val n: String? = null;  n?.length
来源：http://ib.yuexingan06.cn

[T05] Kotlin：when 表达式
来源：http://ra.szsharing.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://at.bjjhwx.cn

[T06] Kotlin：集合映射
来源：http://vw.wgjwhj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://rl.yuexingan06.cn

[T07] Kotlin：集合过滤
来源：http://vp.nszjky.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://mh.nicolike.cn

[T08] Kotlin：数据类
来源：http://cs.gzmigu.cn

data class User(val name: String, val age: Int)
来源：http://qg.asd995.cn

[T09] Kotlin：扩展函数
来源：http://hy.jctech888.com.cn

fun String.exclaim() = this + "!"
来源：http://wj.huixiangedu.cn

[T10] Kotlin：默认参数
来源：http://bn.asd995.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://bz.nicolike.cn

[T11] Kotlin：协程
来源：http://xk.huixinmuqiang.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://yj.huixinmuqiang.cn

[T12] Kotlin：解构声明
来源：http://zp.521024.cn

val (a, b) = Pair(1, 2)
来源：http://sa.huixinmuqiang.cn

[T13] Kotlin：只读 Map
来源：http://rc.haigaiapp.cn

val m = mapOf("a" to 1)
来源：http://hb.hnjuh.cn

[T14] Kotlin：循环
来源：http://de.szxytkj.cn

for (i in 1..10) println(i)
来源：http://dt.521024.cn

[T15] Kotlin：接口
来源：http://vh.jctech888.com.cn

interface Shape { fun area(): Double }
来源：http://qp.newstarts.cn

[T16] Swift：Hello World
来源：http://ni.yuntaijiaju.cn

print("Hello")
来源：http://fu.chemitech.net.cn

[T17] Swift：变量与常量
来源：http://zo.jctech888.com.cn

var a = 1;  let b = 2
来源：http://hy.jctech888.com.cn

[T18] Swift：字符串插值
来源：http://jl.9csxet.cn

"值: \(b)"
来源：http://mg.szsharing.cn

[T19] Swift：可选绑定
来源：http://uu.yuexingan06.cn

if let n = opt { print(n) }
来源：http://am.nicolike.cn

[T20] Swift：数组操作
来源：http://aw.521024.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ey.shtwfgs.cn

[T21] Swift：遍历
来源：http://gx.szxytkj.cn

for x in a { print(x) }
来源：http://pa.yuexingan06.cn

[T22] Swift：字典
来源：http://lg.521024.cn

var d = ["a": 1];  d["b"] = 2
来源：http://jf.asd995.cn

[T23] Swift：函数
来源：http://dx.szsharing.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://fx.muxihuayi.cn

[T24] Swift：闭包
来源：http://ox.wgjwhj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://wx.hahajie.cn

[T25] Swift：结构体
来源：http://ou.yuntaijiaju.cn

struct P { var x: Int }
来源：http://tv.521024.cn

[T26] Swift：类与重写
来源：http://we.huanxung.cn

class A: Base { override func f() {} }
来源：http://ne.szxytkj.cn

[T27] Swift：错误处理
来源：http://no.colortex.cn

do { try f() } catch { print(error) }
来源：http://ml.jianghongdianzi.cn

[T28] Swift：枚举
来源：http://uh.lnxyls.cn

enum Color { case red, green }
来源：http://tb.gzmigu.cn

[T29] Swift：guard 提前返回
来源：http://qm.shxzskj.cn

guard let x = opt else { return }
来源：http://oo.haigaiapp.cn

[T30] Swift：协议
来源：http://dt.gzmigu.cn

protocol Shape { func area() -> Double }
来源：http://mz.szxytkj.cn

[T31] Lua：Hello World
来源：http://dg.huixinmuqiang.cn

print("Hello")
来源：http://wk.huanxung.cn

[T32] Lua：局部变量
来源：http://rq.huixiangedu.cn

local a = 1
来源：http://dn.newstarts.cn

[T33] Lua：表（数组）
来源：http://it.colortex.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://mn.szsharing.cn

[T34] Lua：遍历表
来源：http://cq.hnjuh.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://br.panjiajie.cn

[T35] Lua：字典表
来源：http://ys.asd995.cn

local d = { a = 1 };  d.b = 2
来源：http://gs.chemitech.net.cn

[T36] Lua：函数
来源：http://dc.newstarts.cn

function add(a, b) return a + b end
来源：http://yt.huixiangedu.cn

[T37] Lua：字符串拼接
来源：http://kg.szxytkj.cn

"a" .. "b"
来源：http://ah.hnjuh.cn

[T38] Lua：条件
来源：http://ef.szsharing.cn

if x > 0 then print("正") end
来源：http://yo.nicolike.cn

[T39] Lua：模式匹配
来源：http://ee.yuntaijiaju.cn

string.find(s, "%d+")
来源：http://lu.panjiajie.cn

[T40] Lua：元表
来源：http://vu.yuntaijiaju.cn

setmetatable({}, { __index = base })
来源：http://of.huixiangedu.cn

[T41] Perl：Hello World
来源：http://rx.haigaiapp.cn

print "Hello\n";
来源：http://gt.bjjhwx.cn

[T42] Perl：变量类型
来源：http://rz.gzmigu.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://nr.hahajie.cn

[T43] Perl：字符串插值
来源：http://vj.muxihuayi.cn

"值: $a"
来源：http://xi.muxihuayi.cn

[T44] Perl：条件
来源：http://cn.chemitech.net.cn

if ($a > 0) { print "正"; }
来源：http://nl.521024.cn

[T45] Perl：数组遍历
来源：http://dr.haigaiapp.cn

for my $x (@arr) { print $x; }
来源：http://lj.nicolike.cn

[T46] Perl：哈希操作
来源：http://de.muxihuayi.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://oh.521024.cn

[T47] Perl：正则捕获
来源：http://dm.wgjwhj.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://tn.colortex.cn

[T48] Perl：正则替换
来源：http://kl.wgjwhj.cn

$s =~ s/old/new/g;
来源：http://qa.chemitech.net.cn

[T49] Perl：函数
来源：http://ag.nicolike.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://nt.bjjhwx.cn

[T50] Perl：逐行读文件
来源：http://kv.huixiangedu.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://gf.9csxet.cn

while (my $line = <$fh>) { print $line; }
来源：http://rg.wgjwhj.cn

[T51] Scala：Hello World
来源：http://pd.muxihuayi.cn

println("Hello")
来源：http://og.colortex.cn

[T52] Scala：变量
来源：http://zx.bookmarksfly.cn

val a = 1;  var b = 2
来源：http://nj.haigaiapp.cn

[T53] Scala：字符串插值
来源：http://dx.szxytkj.cn

s"值: $b"
来源：http://at.asd995.cn

[T54] Scala：集合映射
来源：http://ac.hnjuh.cn

List(1, 2, 3).map(_ * 2)
来源：http://av.newstarts.cn

[T55] Scala：集合过滤
来源：http://vd.jctech888.com.cn

List(1, 2, 3).filter(_ > 1)
来源：http://fy.huixiangedu.cn

[T56] Scala：样例类
来源：http://br.wgjwhj.cn

case class User(name: String, age: Int)
来源：http://zr.jctech888.com.cn

[T57] Scala：模式匹配
来源：http://cg.jctech888.com.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://tn.wgjwhj.cn

[T58] Scala：函数定义
来源：http://sh.huixiangedu.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ot.hahajie.cn

[T59] Scala：循环
来源：http://ls.huanxung.cn

for (i <- 1 to 10) println(i)
来源：http://ny.jianghongdianzi.cn

[T60] Scala：折叠
来源：http://yx.colortex.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://nl.521024.cn

================================================================================
来源：http://wm.hnjuh.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ns.lnxyls.cn

================================================================================
来源：http://ie.colortex.cn

[U01] Py：创建虚拟环境
来源：http://ua.nicolike.cn

python -m venv .venv && source .venv/bin/activate
来源：http://gb.asd995.cn

[U02] Py：导出 / 安装依赖
来源：http://ln.huixiangedu.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://by.huixinmuqiang.cn

[U03] Py：加载 .env 配置
来源：http://ii.huanxung.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://my.nszjky.cn

[U04] Py：变量调试打印
来源：http://oc.chemitech.net.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://cp.bjjhwx.cn

[U05] Py：列表去重且保序
来源：http://gt.huanxung.cn

list(dict.fromkeys(arr))
来源：http://zv.haigaiapp.cn

[U06] Py：合并两个字典
来源：http://qv.lnxyls.cn

{**a, **b}
来源：http://uk.szsharing.cn

[U07] Py：反转字典键值
来源：http://vg.jctech888.com.cn

{v: k for k, v in d.items()}
来源：http://jk.jctech888.com.cn

[U08] Py：展平二维列表
来源：http://yf.jctech888.com.cn

[y for x in nested for y in x]
来源：http://bt.huixiangedu.cn

[U09] Py：字典取最大值的键
来源：http://do.huixinmuqiang.cn

max(d, key=d.get)
来源：http://nz.huanxung.cn

[U10] Py：按值排序字典
来源：http://nc.hahajie.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://jm.huanxung.cn

[U11] Py：生成器表达式
来源：http://nb.yuexingan06.cn

(x * 2 for x in arr)
来源：http://uo.newstarts.cn

[U12] Py：取出现最多的 3 个元素
来源：http://uh.szsharing.cn

Counter(arr).most_common(3)
来源：http://cr.shtwfgs.cn

[U13] Py：固定长度队列
来源：http://db.nicolike.cn

deque(maxlen=10)
来源：http://pa.shxzukj.cn

[U14] Py：分组收集到列表
来源：http://lz.jctech888.com.cn

defaultdict(list)
来源：http://zj.newstarts.cn

[U15] Py：高精度计时
来源：http://dx.gzmigu.cn

t = time.perf_counter()
来源：http://xo.nicolike.cn

[U16] Py：命令行参数解析
来源：http://it.muxihuayi.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://gh.wgjwhj.cn

[U17] Py：初始化日志
来源：http://id.yuntaijiaju.cn

logging.basicConfig(level=logging.INFO)
来源：http://oo.huixiangedu.cn

[U18] Py：预编译正则
来源：http://nz.shtwfgs.cn

pat = re.compile(r"\d+")
来源：http://yj.huanxung.cn

[U19] Py：正则替换带回调
来源：http://ay.shtwfgs.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://hv.jianghongdianzi.cn

[U20] Py：缓存函数结果
来源：http://dx.521024.cn

@functools.lru_cache(maxsize=None)
来源：http://jy.shxzukj.cn

[U21] Py：自定义上下文管理器
来源：http://ai.hnjuh.cn

@contextlib.contextmanager
来源：http://kw.newstarts.cn

[U22] Py：矩阵转置
来源：http://xo.panjiajie.cn

list(zip(*m))
来源：http://ab.huixiangedu.cn

[U23] Py：分块读取大文件
来源：http://cv.huanxung.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://lz.bjjhwx.cn

[U24] Py：路径操作
来源：http://ye.shxzskj.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://zt.wgjwhj.cn

[U25] Py：CSV 按字典读
来源：http://sf.wgjwhj.cn

csv.DictReader(f)
来源：http://hf.nicolike.cn

[U26] Py：并发下载
来源：http://nm.9csxet.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://tl.yuexingan06.cn

[U27] Py：异步 HTTP
来源：http://qs.yuexingan06.cn

aiohttp.ClientSession() 配合 async with
来源：http://pc.bookmarksfly.cn

[U28] Py：类型别名
来源：http://uc.nicolike.cn

UserId = int
来源：http://je.hahajie.cn

[U29] Py：属性校验
来源：http://fu.521024.cn

@property 与 @x.setter 配合
来源：http://zi.jianghongdianzi.cn

[U30] Py：数据类
来源：http://aa.nicolike.cn

@dataclass(slots=True)
来源：http://ma.muxihuayi.cn

[U31] Py：单测
来源：http://nr.huixiangedu.cn

python -m pytest -q
来源：http://yf.jctech888.com.cn

[U32] Py：代码格式化
来源：http://ua.shxzukj.cn

ruff format . && ruff check --fix .
来源：http://td.nicolike.cn

[U33] Py：打包发布
来源：http://uu.asd995.cn

python -m build  （依赖 pyproject.toml）
来源：http://le.colortex.cn

[U34] Py：判断编码
来源：http://hh.yuexingan06.cn

chardet.detect(raw)
来源：http://pb.panjiajie.cn

[U35] Py：发送邮件
来源：http://il.haigaiapp.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://rq.shtwfgs.cn

[U36] Py：定时任务
来源：http://sx.yuntaijiaju.cn

schedule.every(10).minutes.do(job)
来源：http://ni.shtwfgs.cn

[U37] Py：读写 Excel
来源：http://ra.9csxet.cn

pandas.read_excel / DataFrame.to_excel
来源：http://iv.haigaiapp.cn

[U38] Py：获取脚本所在目录
来源：http://na.chemitech.net.cn

Path(__file__).resolve().parent
来源：http://ex.muxihuayi.cn

[U39] Py：判断是否在交互环境
来源：http://kl.szxytkj.cn

sys.stdout.isatty()
来源：http://sm.huixinmuqiang.cn

[U40] Py：打印到标准错误
来源：http://qn.huanxung.cn

print("err", file=sys.stderr)
来源：http://aw.huanxung.cn

[U41] PHP：初始化 Composer 项目
来源：http://ag.colortex.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ls.yuexingan06.cn

[U42] PHP：PSR-4 自动加载
来源：http://ev.hnjuh.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://zz.521024.cn

[U43] PHP：声明命名空间
来源：http://hx.muxihuayi.cn

namespace App\Http;
来源：http://eh.shtwfgs.cn

[U44] PHP：开启严格类型
来源：http://me.jctech888.com.cn

declare(strict_types=1);
来源：http://tu.panjiajie.cn


<!-- 参考信息 -->