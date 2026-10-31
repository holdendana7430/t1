代发 wailian999

atoi("42");  strtod("3.14", NULL);
来源：http://kg.9csxet.cn

[S23] C：随机数
来源：http://bv.nicolike.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://kb.shtwfgs.cn

[S24] C：获取本地时间
来源：http://se.szsharing.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://tk.bjjhwx.cn

[S25] C：内存拷贝
来源：http://oh.jctech888.com.cn

memcpy(dst, src, n);
来源：http://ld.shxzskj.cn

[S26] C：内存清零
来源：http://yj.wgjwhj.cn

memset(a, 0, sizeof a);
来源：http://fa.chemitech.net.cn

[S27] C：定义常量
来源：http://nj.muxihuayi.cn

const double PI = 3.14159;
来源：http://jo.bookmarksfly.cn

[S28] C：静态变量
来源：http://ae.jctech888.com.cn

static int counter = 0;
来源：http://fv.nszjky.cn

[S29] C：变参函数
来源：http://in.521024.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://zt.wgjwhj.cn

[S30] C：头文件保护
来源：http://qr.huanxung.cn

#ifndef X_H
来源：http://ag.nszjky.cn

#define X_H
来源：http://yp.yuexingan06.cn

#endif
来源：http://dc.bookmarksfly.cn

[S31] C++：Hello World
来源：http://qf.9csxet.cn

#include <iostream>
来源：http://wo.bjjhwx.cn

int main() { std::cout << "Hello\n"; }
来源：http://wb.jctech888.com.cn

[S32] C++：字符串
来源：http://ar.newstarts.cn

std::string s = "hi";  s += "!";
来源：http://ka.haigaiapp.cn

[S33] C++：vector 增删
来源：http://ue.szxytkj.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://mh.asd995.cn

[S34] C++：遍历 vector
来源：http://sz.newstarts.cn

for (auto &x : v) { std::cout << x; }
来源：http://qh.9csxet.cn

[S35] C++：map
来源：http://vh.lnxyls.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://we.chemitech.net.cn

[S36] C++：unordered_map
来源：http://hl.nszjky.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://bn.hahajie.cn

[S37] C++：set
来源：http://su.521024.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://lo.yuntaijiaju.cn

[S38] C++：排序
来源：http://po.bjjhwx.cn

std::sort(v.begin(), v.end());
来源：http://lx.yuntaijiaju.cn

[S39] C++：自定义比较器排序
来源：http://xq.jianghongdianzi.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://oq.shxzukj.cn

[S40] C++：查找元素
来源：http://kb.huanxung.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mo.newstarts.cn

[S41] C++：类与构造函数
来源：http://px.yuexingan06.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://hk.panjiajie.cn

[S42] C++：继承与虚函数
来源：http://ok.hnjuh.cn

class B : public Base { public: void f() override {} };
来源：http://bp.haigaiapp.cn

[S43] C++：智能指针
来源：http://jh.nicolike.cn

auto p = std::make_unique<int>(5);
来源：http://qd.nicolike.cn

[S44] C++：引用传参
来源：http://jt.shxzukj.cn

void inc(int &x) { ++x; }
来源：http://ae.shxzskj.cn

[S45] C++：lambda
来源：http://kc.shxzskj.cn

auto add = [](int a, int b) { return a + b; };
来源：http://wk.huanxung.cn

[S46] C++：函数模板
来源：http://wl.jctech888.com.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://cc.jctech888.com.cn

[S47] C++：结构化绑定遍历
来源：http://rh.szsharing.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://rl.nszjky.cn

[S48] C++：逐行读文件
来源：http://cm.asd995.cn

std::ifstream in("a.txt");  std::string line;
来源：http://wk.huixiangedu.cn

while (std::getline(in, line)) { }
来源：http://nw.panjiajie.cn

[S49] C++：写文件
来源：http://ts.muxihuayi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://bc.muxihuayi.cn

[S50] C++：格式化数字
来源：http://si.yuntaijiaju.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ex.nicolike.cn

[S51] C++：显式类型转换
来源：http://fg.bookmarksfly.cn

static_cast<double>(a) / b
来源：http://sn.colortex.cn

[S52] C++：const 与 noexcept
来源：http://kk.shxzskj.cn

int size() const noexcept { return n_; }
来源：http://ws.lnxyls.cn

[S53] C++：移动语义
来源：http://qd.szxytkj.cn

std::vector<int> w = std::move(v);
来源：http://cl.jctech888.com.cn

[S54] C++：异常处理
来源：http://ks.bookmarksfly.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://gm.asd995.cn

[S55] C++：结构化绑定
来源：http://gp.huanxung.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ys.nszjky.cn

[S56] C++：optional
来源：http://oo.szxytkj.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ux.nicolike.cn

[S57] C++：编译期常量
来源：http://yz.huanxung.cn

constexpr int N = 10;
来源：http://gc.shtwfgs.cn

[S58] C++：命名空间
来源：http://dk.shxzukj.cn

namespace ns { int f() { return 1; } }
来源：http://gy.shxzskj.cn

[S59] C++：静态断言
来源：http://ld.yuexingan06.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://bj.asd995.cn

[S60] C++：遍历并删除元素
来源：http://il.szsharing.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://pg.panjiajie.cn

================================================================================
来源：http://qb.hnjuh.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ga.yuntaijiaju.cn

================================================================================
来源：http://ti.chemitech.net.cn

[T01] Kotlin：Hello World
来源：http://pt.gzmigu.cn

println("Hello")
来源：http://ic.shtwfgs.cn

[T02] Kotlin：变量
来源：http://lh.521024.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wp.gzmigu.cn

[T03] Kotlin：字符串模板
来源：http://zs.hahajie.cn

"值: $b"
来源：http://if.colortex.cn

[T04] Kotlin：空安全
来源：http://jl.gzmigu.cn

val n: String? = null;  n?.length
来源：http://xh.bookmarksfly.cn

[T05] Kotlin：when 表达式
来源：http://fw.hnjuh.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://zh.shxzskj.cn

[T06] Kotlin：集合映射
来源：http://hl.yuntaijiaju.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://xo.yuntaijiaju.cn

[T07] Kotlin：集合过滤
来源：http://yv.newstarts.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://er.nicolike.cn

[T08] Kotlin：数据类
来源：http://xh.lnxyls.cn

data class User(val name: String, val age: Int)
来源：http://ym.huixiangedu.cn

[T09] Kotlin：扩展函数
来源：http://wa.jianghongdianzi.cn

fun String.exclaim() = this + "!"
来源：http://hv.colortex.cn

[T10] Kotlin：默认参数
来源：http://oi.colortex.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://lr.bookmarksfly.cn

[T11] Kotlin：协程
来源：http://hs.yuntaijiaju.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://oy.huixinmuqiang.cn

[T12] Kotlin：解构声明
来源：http://ej.bjjhwx.cn

val (a, b) = Pair(1, 2)
来源：http://ko.huixinmuqiang.cn

[T13] Kotlin：只读 Map
来源：http://sv.asd995.cn

val m = mapOf("a" to 1)
来源：http://py.jctech888.com.cn

[T14] Kotlin：循环
来源：http://iy.chemitech.net.cn

for (i in 1..10) println(i)
来源：http://gp.shtwfgs.cn

[T15] Kotlin：接口
来源：http://ir.gzmigu.cn

interface Shape { fun area(): Double }
来源：http://qe.shxzukj.cn

[T16] Swift：Hello World
来源：http://qh.hahajie.cn

print("Hello")
来源：http://tq.shxzskj.cn

[T17] Swift：变量与常量
来源：http://ru.hahajie.cn

var a = 1;  let b = 2
来源：http://bt.nicolike.cn

[T18] Swift：字符串插值
来源：http://qk.yuntaijiaju.cn

"值: \(b)"
来源：http://yq.muxihuayi.cn

[T19] Swift：可选绑定
来源：http://si.huanxung.cn

if let n = opt { print(n) }
来源：http://wo.panjiajie.cn

[T20] Swift：数组操作
来源：http://eq.haigaiapp.cn

var a = [1, 2, 3];  a.append(4)
来源：http://iq.nicolike.cn

[T21] Swift：遍历
来源：http://uc.jctech888.com.cn

for x in a { print(x) }
来源：http://cr.colortex.cn

[T22] Swift：字典
来源：http://rg.nszjky.cn

var d = ["a": 1];  d["b"] = 2
来源：http://sa.hnjuh.cn

[T23] Swift：函数
来源：http://pv.gzmigu.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://vn.huixinmuqiang.cn

[T24] Swift：闭包
来源：http://fa.chemitech.net.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://rb.haigaiapp.cn

[T25] Swift：结构体
来源：http://sz.panjiajie.cn

struct P { var x: Int }
来源：http://ix.yuntaijiaju.cn

[T26] Swift：类与重写
来源：http://tu.hnjuh.cn

class A: Base { override func f() {} }
来源：http://hz.9csxet.cn

[T27] Swift：错误处理
来源：http://te.bookmarksfly.cn

do { try f() } catch { print(error) }
来源：http://vg.yuntaijiaju.cn

[T28] Swift：枚举
来源：http://vk.nszjky.cn

enum Color { case red, green }
来源：http://tm.szxytkj.cn

[T29] Swift：guard 提前返回
来源：http://ts.gzmigu.cn

guard let x = opt else { return }
来源：http://jr.lnxyls.cn

[T30] Swift：协议
来源：http://de.panjiajie.cn

protocol Shape { func area() -> Double }
来源：http://si.hnjuh.cn

[T31] Lua：Hello World
来源：http://ue.shxzskj.cn

print("Hello")
来源：http://ck.szsharing.cn

[T32] Lua：局部变量
来源：http://ry.hnjuh.cn

local a = 1
来源：http://nd.muxihuayi.cn

[T33] Lua：表（数组）
来源：http://gs.colortex.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://wb.shxzskj.cn

[T34] Lua：遍历表
来源：http://ik.lnxyls.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ri.521024.cn

[T35] Lua：字典表
来源：http://tk.colortex.cn

local d = { a = 1 };  d.b = 2
来源：http://wx.nicolike.cn

[T36] Lua：函数
来源：http://un.colortex.cn

function add(a, b) return a + b end
来源：http://zw.yuntaijiaju.cn

[T37] Lua：字符串拼接
来源：http://mp.haigaiapp.cn

"a" .. "b"
来源：http://up.hnjuh.cn

[T38] Lua：条件
来源：http://mi.hnjuh.cn

if x > 0 then print("正") end
来源：http://bs.chemitech.net.cn

[T39] Lua：模式匹配
来源：http://px.hnjuh.cn

string.find(s, "%d+")
来源：http://ej.chemitech.net.cn

[T40] Lua：元表
来源：http://qs.haigaiapp.cn

setmetatable({}, { __index = base })
来源：http://xy.bjjhwx.cn

[T41] Perl：Hello World
来源：http://dt.jianghongdianzi.cn

print "Hello\n";
来源：http://mc.colortex.cn

[T42] Perl：变量类型
来源：http://pq.nszjky.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://vs.chemitech.net.cn

[T43] Perl：字符串插值
来源：http://kx.szsharing.cn

"值: $a"
来源：http://mo.huixiangedu.cn

[T44] Perl：条件
来源：http://pm.huixinmuqiang.cn

if ($a > 0) { print "正"; }
来源：http://sb.bookmarksfly.cn

[T45] Perl：数组遍历
来源：http://mc.lnxyls.cn

for my $x (@arr) { print $x; }
来源：http://rh.shtwfgs.cn

[T46] Perl：哈希操作
来源：http://vm.yuntaijiaju.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://te.bjjhwx.cn

[T47] Perl：正则捕获
来源：http://oh.panjiajie.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ny.hnjuh.cn

[T48] Perl：正则替换
来源：http://kz.szxytkj.cn

$s =~ s/old/new/g;
来源：http://du.jctech888.com.cn

[T49] Perl：函数
来源：http://dh.szxytkj.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://zm.jianghongdianzi.cn

[T50] Perl：逐行读文件
来源：http://xw.szxytkj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://cd.521024.cn

while (my $line = <$fh>) { print $line; }
来源：http://qe.bookmarksfly.cn

[T51] Scala：Hello World
来源：http://dp.shxzukj.cn

println("Hello")
来源：http://ha.hnjuh.cn

[T52] Scala：变量
来源：http://ww.huanxung.cn

val a = 1;  var b = 2
来源：http://zt.szsharing.cn

[T53] Scala：字符串插值
来源：http://fr.huixiangedu.cn

s"值: $b"
来源：http://rw.nicolike.cn

[T54] Scala：集合映射
来源：http://nj.bookmarksfly.cn

List(1, 2, 3).map(_ * 2)
来源：http://hk.shtwfgs.cn

[T55] Scala：集合过滤
来源：http://hf.521024.cn

List(1, 2, 3).filter(_ > 1)
来源：http://co.szxytkj.cn

[T56] Scala：样例类
来源：http://kh.chemitech.net.cn

case class User(name: String, age: Int)
来源：http://hq.szsharing.cn

[T57] Scala：模式匹配
来源：http://xk.bookmarksfly.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ek.yuexingan06.cn

[T58] Scala：函数定义
来源：http://dc.muxihuayi.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ly.muxihuayi.cn

[T59] Scala：循环
来源：http://jq.521024.cn

for (i <- 1 to 10) println(i)
来源：http://rx.bookmarksfly.cn

[T60] Scala：折叠
来源：http://hh.hnjuh.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://vd.newstarts.cn

================================================================================
来源：http://gd.szxytkj.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://bt.muxihuayi.cn

================================================================================
来源：http://eb.bjjhwx.cn

[U01] Py：创建虚拟环境
来源：http://aa.hahajie.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ny.huixiangedu.cn

[U02] Py：导出 / 安装依赖
来源：http://er.szsharing.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://br.szxytkj.cn

[U03] Py：加载 .env 配置
来源：http://dz.wgjwhj.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://jb.nicolike.cn

[U04] Py：变量调试打印
来源：http://gs.hnjuh.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://iq.nszjky.cn

[U05] Py：列表去重且保序
来源：http://bz.shxzskj.cn

list(dict.fromkeys(arr))
来源：http://oi.gzmigu.cn

[U06] Py：合并两个字典
来源：http://wv.panjiajie.cn

{**a, **b}
来源：http://ij.jctech888.com.cn

[U07] Py：反转字典键值
来源：http://lz.nszjky.cn

{v: k for k, v in d.items()}
来源：http://fr.chemitech.net.cn

[U08] Py：展平二维列表
来源：http://qj.wgjwhj.cn

[y for x in nested for y in x]
来源：http://qs.hahajie.cn

[U09] Py：字典取最大值的键
来源：http://we.nszjky.cn

max(d, key=d.get)
来源：http://vf.jianghongdianzi.cn

[U10] Py：按值排序字典
来源：http://xl.nicolike.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://zr.huixinmuqiang.cn

[U11] Py：生成器表达式
来源：http://cn.hahajie.cn

(x * 2 for x in arr)
来源：http://ds.szxytkj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://jj.nicolike.cn

Counter(arr).most_common(3)
来源：http://dq.gzmigu.cn

[U13] Py：固定长度队列
来源：http://kz.shtwfgs.cn

deque(maxlen=10)
来源：http://vd.nicolike.cn

[U14] Py：分组收集到列表
来源：http://uu.nszjky.cn

defaultdict(list)
来源：http://gn.colortex.cn

[U15] Py：高精度计时
来源：http://ua.gzmigu.cn

t = time.perf_counter()
来源：http://pm.hnjuh.cn

[U16] Py：命令行参数解析
来源：http://vn.yuexingan06.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://qh.gzmigu.cn

[U17] Py：初始化日志
来源：http://kv.szsharing.cn

logging.basicConfig(level=logging.INFO)
来源：http://wu.yuexingan06.cn

[U18] Py：预编译正则
来源：http://he.bookmarksfly.cn

pat = re.compile(r"\d+")
来源：http://ct.huixinmuqiang.cn

[U19] Py：正则替换带回调
来源：http://ls.muxihuayi.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ws.szxytkj.cn

[U20] Py：缓存函数结果
来源：http://tf.shxzskj.cn

@functools.lru_cache(maxsize=None)
来源：http://js.huixinmuqiang.cn

[U21] Py：自定义上下文管理器
来源：http://qn.wgjwhj.cn

@contextlib.contextmanager
来源：http://ce.panjiajie.cn

[U22] Py：矩阵转置
来源：http://wx.newstarts.cn

list(zip(*m))
来源：http://lg.yuntaijiaju.cn

[U23] Py：分块读取大文件
来源：http://wf.wgjwhj.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://cg.jianghongdianzi.cn

[U24] Py：路径操作
来源：http://cw.9csxet.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://yf.jianghongdianzi.cn

[U25] Py：CSV 按字典读
来源：http://kv.bookmarksfly.cn

csv.DictReader(f)
来源：http://ev.bookmarksfly.cn

[U26] Py：并发下载
来源：http://al.wgjwhj.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://tq.nszjky.cn

[U27] Py：异步 HTTP
来源：http://jh.jianghongdianzi.cn

aiohttp.ClientSession() 配合 async with
来源：http://af.521024.cn

[U28] Py：类型别名
来源：http://bk.szxytkj.cn

UserId = int
来源：http://sp.hnjuh.cn

[U29] Py：属性校验
来源：http://sp.panjiajie.cn

@property 与 @x.setter 配合
来源：http://wx.hahajie.cn

[U30] Py：数据类
来源：http://lw.hnjuh.cn

@dataclass(slots=True)
来源：http://dy.shxzukj.cn

[U31] Py：单测
来源：http://ax.jianghongdianzi.cn

python -m pytest -q
来源：http://mf.nszjky.cn

[U32] Py：代码格式化
来源：http://ke.szxytkj.cn

ruff format . && ruff check --fix .
来源：http://bw.yuexingan06.cn

[U33] Py：打包发布
来源：http://gi.shxzukj.cn

python -m build  （依赖 pyproject.toml）
来源：http://vn.wgjwhj.cn

[U34] Py：判断编码
来源：http://dz.521024.cn

chardet.detect(raw)
来源：http://tj.szsharing.cn

[U35] Py：发送邮件
来源：http://js.jctech888.com.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://io.newstarts.cn

[U36] Py：定时任务
来源：http://to.szxytkj.cn

schedule.every(10).minutes.do(job)
来源：http://zg.jctech888.com.cn

[U37] Py：读写 Excel
来源：http://ux.yuexingan06.cn

pandas.read_excel / DataFrame.to_excel
来源：http://oq.bookmarksfly.cn

[U38] Py：获取脚本所在目录
来源：http://ci.hahajie.cn

Path(__file__).resolve().parent
来源：http://sd.szsharing.cn

[U39] Py：判断是否在交互环境
来源：http://ki.huixiangedu.cn

sys.stdout.isatty()
来源：http://zo.yuntaijiaju.cn

[U40] Py：打印到标准错误
来源：http://ln.colortex.cn

print("err", file=sys.stderr)
来源：http://qg.newstarts.cn

[U41] PHP：初始化 Composer 项目
来源：http://ib.yuntaijiaju.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://qh.colortex.cn

[U42] PHP：PSR-4 自动加载
来源：http://sc.jctech888.com.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://yz.huixiangedu.cn

[U43] PHP：声明命名空间
来源：http://yt.shxzukj.cn

namespace App\Http;
来源：http://ac.bookmarksfly.cn

[U44] PHP：开启严格类型
来源：http://hr.huixinmuqiang.cn

declare(strict_types=1);
来源：http://hv.muxihuayi.cn

[U45] PHP：类型声明与返回类型
来源：http://hq.panjiajie.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://ys.szxytkj.cn

[U46] PHP：可空类型
来源：http://ms.yuntaijiaju.cn

?string $name = null
来源：http://lj.chemitech.net.cn


<!-- 参考信息 -->