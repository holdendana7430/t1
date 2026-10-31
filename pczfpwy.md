代发 wailian999

atoi("42");  strtod("3.14", NULL);
来源：http://ru.muxihuayi.cn

[S23] C：随机数
来源：http://sp.yuntaijiaju.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://da.9csxet.cn

[S24] C：获取本地时间
来源：http://om.hahajie.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://nu.jianghongdianzi.cn

[S25] C：内存拷贝
来源：http://vu.huixiangedu.cn

memcpy(dst, src, n);
来源：http://kz.bookmarksfly.cn

[S26] C：内存清零
来源：http://rd.bjjhwx.cn

memset(a, 0, sizeof a);
来源：http://gq.lnxyls.cn

[S27] C：定义常量
来源：http://hm.huixinmuqiang.cn

const double PI = 3.14159;
来源：http://jj.hnjuh.cn

[S28] C：静态变量
来源：http://fh.yuexingan06.cn

static int counter = 0;
来源：http://az.huixinmuqiang.cn

[S29] C：变参函数
来源：http://ff.hnjuh.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://bx.nicolike.cn

[S30] C：头文件保护
来源：http://pq.chemitech.net.cn

#ifndef X_H
来源：http://ra.newstarts.cn

#define X_H
来源：http://vj.wgjwhj.cn

#endif
来源：http://vo.521024.cn

[S31] C++：Hello World
来源：http://bg.muxihuayi.cn

#include <iostream>
来源：http://ut.shxzskj.cn

int main() { std::cout << "Hello\n"; }
来源：http://tt.shtwfgs.cn

[S32] C++：字符串
来源：http://vs.colortex.cn

std::string s = "hi";  s += "!";
来源：http://er.shtwfgs.cn

[S33] C++：vector 增删
来源：http://tm.yuexingan06.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ae.haigaiapp.cn

[S34] C++：遍历 vector
来源：http://xb.asd995.cn

for (auto &x : v) { std::cout << x; }
来源：http://mu.muxihuayi.cn

[S35] C++：map
来源：http://gw.huixinmuqiang.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wd.hahajie.cn

[S36] C++：unordered_map
来源：http://pz.haigaiapp.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://zm.asd995.cn

[S37] C++：set
来源：http://pw.hnjuh.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://qf.shtwfgs.cn

[S38] C++：排序
来源：http://ji.wgjwhj.cn

std::sort(v.begin(), v.end());
来源：http://he.newstarts.cn

[S39] C++：自定义比较器排序
来源：http://uw.wgjwhj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ln.shxzukj.cn

[S40] C++：查找元素
来源：http://fu.hahajie.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ve.521024.cn

[S41] C++：类与构造函数
来源：http://qt.asd995.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://do.shxzskj.cn

[S42] C++：继承与虚函数
来源：http://iw.asd995.cn

class B : public Base { public: void f() override {} };
来源：http://hn.haigaiapp.cn

[S43] C++：智能指针
来源：http://bt.bookmarksfly.cn

auto p = std::make_unique<int>(5);
来源：http://ct.szsharing.cn

[S44] C++：引用传参
来源：http://vt.lnxyls.cn

void inc(int &x) { ++x; }
来源：http://qf.shxzukj.cn

[S45] C++：lambda
来源：http://fy.colortex.cn

auto add = [](int a, int b) { return a + b; };
来源：http://xa.huixinmuqiang.cn

[S46] C++：函数模板
来源：http://no.muxihuayi.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://cs.hahajie.cn

[S47] C++：结构化绑定遍历
来源：http://oc.jctech888.com.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qu.muxihuayi.cn

[S48] C++：逐行读文件
来源：http://rr.colortex.cn

std::ifstream in("a.txt");  std::string line;
来源：http://fr.9csxet.cn

while (std::getline(in, line)) { }
来源：http://ng.szsharing.cn

[S49] C++：写文件
来源：http://fp.lnxyls.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://yy.panjiajie.cn

[S50] C++：格式化数字
来源：http://sx.9csxet.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://zz.muxihuayi.cn

[S51] C++：显式类型转换
来源：http://xp.yuexingan06.cn

static_cast<double>(a) / b
来源：http://mk.wgjwhj.cn

[S52] C++：const 与 noexcept
来源：http://dn.nicolike.cn

int size() const noexcept { return n_; }
来源：http://kq.newstarts.cn

[S53] C++：移动语义
来源：http://au.nicolike.cn

std::vector<int> w = std::move(v);
来源：http://nh.shtwfgs.cn

[S54] C++：异常处理
来源：http://qe.colortex.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://dz.muxihuayi.cn

[S55] C++：结构化绑定
来源：http://ug.jianghongdianzi.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://er.huanxung.cn

[S56] C++：optional
来源：http://dq.nszjky.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://lk.shxzskj.cn

[S57] C++：编译期常量
来源：http://wj.colortex.cn

constexpr int N = 10;
来源：http://ne.yuexingan06.cn

[S58] C++：命名空间
来源：http://nb.lnxyls.cn

namespace ns { int f() { return 1; } }
来源：http://gn.jianghongdianzi.cn

[S59] C++：静态断言
来源：http://mm.nicolike.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://gr.szxytkj.cn

[S60] C++：遍历并删除元素
来源：http://yv.haigaiapp.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ve.shxzukj.cn

================================================================================
来源：http://dp.yuexingan06.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://iv.wgjwhj.cn

================================================================================
来源：http://lp.yuntaijiaju.cn

[T01] Kotlin：Hello World
来源：http://fj.hahajie.cn

println("Hello")
来源：http://bp.panjiajie.cn

[T02] Kotlin：变量
来源：http://zu.shxzukj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ad.nszjky.cn

[T03] Kotlin：字符串模板
来源：http://uo.wgjwhj.cn

"值: $b"
来源：http://wf.asd995.cn

[T04] Kotlin：空安全
来源：http://if.muxihuayi.cn

val n: String? = null;  n?.length
来源：http://we.newstarts.cn

[T05] Kotlin：when 表达式
来源：http://fh.panjiajie.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://fk.nszjky.cn

[T06] Kotlin：集合映射
来源：http://yb.hahajie.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://je.hahajie.cn

[T07] Kotlin：集合过滤
来源：http://vd.yuexingan06.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://st.panjiajie.cn

[T08] Kotlin：数据类
来源：http://za.asd995.cn

data class User(val name: String, val age: Int)
来源：http://bo.newstarts.cn

[T09] Kotlin：扩展函数
来源：http://pk.asd995.cn

fun String.exclaim() = this + "!"
来源：http://mk.szxytkj.cn

[T10] Kotlin：默认参数
来源：http://fn.szxytkj.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://mu.yuntaijiaju.cn

[T11] Kotlin：协程
来源：http://ax.huixinmuqiang.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://bf.szxytkj.cn

[T12] Kotlin：解构声明
来源：http://rn.bookmarksfly.cn

val (a, b) = Pair(1, 2)
来源：http://ir.nszjky.cn

[T13] Kotlin：只读 Map
来源：http://yb.haigaiapp.cn

val m = mapOf("a" to 1)
来源：http://md.jctech888.com.cn

[T14] Kotlin：循环
来源：http://dv.shtwfgs.cn

for (i in 1..10) println(i)
来源：http://ya.haigaiapp.cn

[T15] Kotlin：接口
来源：http://op.bjjhwx.cn

interface Shape { fun area(): Double }
来源：http://sy.szsharing.cn

[T16] Swift：Hello World
来源：http://gw.huanxung.cn

print("Hello")
来源：http://ow.colortex.cn

[T17] Swift：变量与常量
来源：http://pi.huixiangedu.cn

var a = 1;  let b = 2
来源：http://rx.hnjuh.cn

[T18] Swift：字符串插值
来源：http://by.521024.cn

"值: \(b)"
来源：http://vp.hnjuh.cn

[T19] Swift：可选绑定
来源：http://dv.9csxet.cn

if let n = opt { print(n) }
来源：http://kg.lnxyls.cn

[T20] Swift：数组操作
来源：http://wi.nszjky.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ug.muxihuayi.cn

[T21] Swift：遍历
来源：http://hr.szxytkj.cn

for x in a { print(x) }
来源：http://ov.shxzskj.cn

[T22] Swift：字典
来源：http://wb.jianghongdianzi.cn

var d = ["a": 1];  d["b"] = 2
来源：http://hn.shxzskj.cn

[T23] Swift：函数
来源：http://gv.yuntaijiaju.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://vv.nszjky.cn

[T24] Swift：闭包
来源：http://ay.szsharing.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ve.panjiajie.cn

[T25] Swift：结构体
来源：http://je.shtwfgs.cn

struct P { var x: Int }
来源：http://rx.asd995.cn

[T26] Swift：类与重写
来源：http://bp.shxzukj.cn

class A: Base { override func f() {} }
来源：http://vh.jianghongdianzi.cn

[T27] Swift：错误处理
来源：http://rp.asd995.cn

do { try f() } catch { print(error) }
来源：http://kj.shxzskj.cn

[T28] Swift：枚举
来源：http://yi.szsharing.cn

enum Color { case red, green }
来源：http://xq.shxzskj.cn

[T29] Swift：guard 提前返回
来源：http://wb.shxzukj.cn

guard let x = opt else { return }
来源：http://ls.shxzskj.cn

[T30] Swift：协议
来源：http://mv.haigaiapp.cn

protocol Shape { func area() -> Double }
来源：http://zw.haigaiapp.cn

[T31] Lua：Hello World
来源：http://re.huixinmuqiang.cn

print("Hello")
来源：http://eq.haigaiapp.cn

[T32] Lua：局部变量
来源：http://tc.szxytkj.cn

local a = 1
来源：http://uq.521024.cn

[T33] Lua：表（数组）
来源：http://qw.huanxung.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://qh.szsharing.cn

[T34] Lua：遍历表
来源：http://qa.wgjwhj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ts.lnxyls.cn

[T35] Lua：字典表
来源：http://dg.haigaiapp.cn

local d = { a = 1 };  d.b = 2
来源：http://jm.nszjky.cn

[T36] Lua：函数
来源：http://ss.haigaiapp.cn

function add(a, b) return a + b end
来源：http://yh.jctech888.com.cn

[T37] Lua：字符串拼接
来源：http://ky.wgjwhj.cn

"a" .. "b"
来源：http://vm.huixiangedu.cn

[T38] Lua：条件
来源：http://pv.shtwfgs.cn

if x > 0 then print("正") end
来源：http://nx.haigaiapp.cn

[T39] Lua：模式匹配
来源：http://ke.bookmarksfly.cn

string.find(s, "%d+")
来源：http://nd.shtwfgs.cn

[T40] Lua：元表
来源：http://zk.bjjhwx.cn

setmetatable({}, { __index = base })
来源：http://fy.colortex.cn

[T41] Perl：Hello World
来源：http://nf.9csxet.cn

print "Hello\n";
来源：http://ve.shxzukj.cn

[T42] Perl：变量类型
来源：http://lb.chemitech.net.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://iy.shxzukj.cn

[T43] Perl：字符串插值
来源：http://su.gzmigu.cn

"值: $a"
来源：http://ec.jctech888.com.cn

[T44] Perl：条件
来源：http://cx.yuntaijiaju.cn

if ($a > 0) { print "正"; }
来源：http://kn.shxzukj.cn

[T45] Perl：数组遍历
来源：http://og.hahajie.cn

for my $x (@arr) { print $x; }
来源：http://ou.9csxet.cn

[T46] Perl：哈希操作
来源：http://ju.jctech888.com.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://oj.bookmarksfly.cn

[T47] Perl：正则捕获
来源：http://qz.jctech888.com.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ds.huixiangedu.cn

[T48] Perl：正则替换
来源：http://rl.huixinmuqiang.cn

$s =~ s/old/new/g;
来源：http://aj.colortex.cn

[T49] Perl：函数
来源：http://cf.jianghongdianzi.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ni.panjiajie.cn

[T50] Perl：逐行读文件
来源：http://qu.szsharing.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://sj.shtwfgs.cn

while (my $line = <$fh>) { print $line; }
来源：http://aw.jctech888.com.cn

[T51] Scala：Hello World
来源：http://ct.yuntaijiaju.cn

println("Hello")
来源：http://mz.shxzukj.cn

[T52] Scala：变量
来源：http://hz.huanxung.cn

val a = 1;  var b = 2
来源：http://ip.lnxyls.cn

[T53] Scala：字符串插值
来源：http://yj.wgjwhj.cn

s"值: $b"
来源：http://pt.szsharing.cn

[T54] Scala：集合映射
来源：http://kn.haigaiapp.cn

List(1, 2, 3).map(_ * 2)
来源：http://pi.muxihuayi.cn

[T55] Scala：集合过滤
来源：http://kq.shxzskj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ra.newstarts.cn

[T56] Scala：样例类
来源：http://ls.yuntaijiaju.cn

case class User(name: String, age: Int)
来源：http://xn.9csxet.cn

[T57] Scala：模式匹配
来源：http://es.muxihuayi.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://fw.muxihuayi.cn

[T58] Scala：函数定义
来源：http://no.huixinmuqiang.cn

def add(a: Int, b: Int): Int = a + b
来源：http://dd.shxzukj.cn

[T59] Scala：循环
来源：http://wk.szsharing.cn

for (i <- 1 to 10) println(i)
来源：http://pa.haigaiapp.cn

[T60] Scala：折叠
来源：http://uw.9csxet.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://yq.jctech888.com.cn

================================================================================
来源：http://nn.hahajie.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://vo.gzmigu.cn

================================================================================
来源：http://xk.nszjky.cn

[U01] Py：创建虚拟环境
来源：http://fn.521024.cn

python -m venv .venv && source .venv/bin/activate
来源：http://by.521024.cn

[U02] Py：导出 / 安装依赖
来源：http://an.huanxung.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://vk.wgjwhj.cn

[U03] Py：加载 .env 配置
来源：http://dn.bjjhwx.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://hr.gzmigu.cn

[U04] Py：变量调试打印
来源：http://nf.shxzskj.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://uz.newstarts.cn

[U05] Py：列表去重且保序
来源：http://nz.muxihuayi.cn

list(dict.fromkeys(arr))
来源：http://ai.jctech888.com.cn

[U06] Py：合并两个字典
来源：http://jd.yuntaijiaju.cn

{**a, **b}
来源：http://ej.hnjuh.cn

[U07] Py：反转字典键值
来源：http://dz.jctech888.com.cn

{v: k for k, v in d.items()}
来源：http://zw.nszjky.cn

[U08] Py：展平二维列表
来源：http://wt.huanxung.cn

[y for x in nested for y in x]
来源：http://ig.lnxyls.cn

[U09] Py：字典取最大值的键
来源：http://lr.bjjhwx.cn

max(d, key=d.get)
来源：http://cw.lnxyls.cn

[U10] Py：按值排序字典
来源：http://yb.gzmigu.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://un.huixiangedu.cn

[U11] Py：生成器表达式
来源：http://pg.wgjwhj.cn

(x * 2 for x in arr)
来源：http://qv.9csxet.cn

[U12] Py：取出现最多的 3 个元素
来源：http://rg.szxytkj.cn

Counter(arr).most_common(3)
来源：http://sm.shxzukj.cn

[U13] Py：固定长度队列
来源：http://sq.shtwfgs.cn

deque(maxlen=10)
来源：http://wc.shtwfgs.cn

[U14] Py：分组收集到列表
来源：http://lq.chemitech.net.cn

defaultdict(list)
来源：http://hr.szsharing.cn

[U15] Py：高精度计时
来源：http://yh.yuntaijiaju.cn

t = time.perf_counter()
来源：http://vy.shtwfgs.cn

[U16] Py：命令行参数解析
来源：http://bm.yuexingan06.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://dc.chemitech.net.cn

[U17] Py：初始化日志
来源：http://mx.shtwfgs.cn

logging.basicConfig(level=logging.INFO)
来源：http://wd.asd995.cn

[U18] Py：预编译正则
来源：http://qu.bookmarksfly.cn

pat = re.compile(r"\d+")
来源：http://px.szxytkj.cn

[U19] Py：正则替换带回调
来源：http://ek.szxytkj.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ov.hnjuh.cn

[U20] Py：缓存函数结果
来源：http://ut.szsharing.cn

@functools.lru_cache(maxsize=None)
来源：http://ox.colortex.cn

[U21] Py：自定义上下文管理器
来源：http://ej.hnjuh.cn

@contextlib.contextmanager
来源：http://xt.hahajie.cn

[U22] Py：矩阵转置
来源：http://gz.hnjuh.cn

list(zip(*m))
来源：http://ga.huixinmuqiang.cn

[U23] Py：分块读取大文件
来源：http://ri.huixinmuqiang.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://rr.asd995.cn

[U24] Py：路径操作
来源：http://dh.wgjwhj.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://rl.hnjuh.cn

[U25] Py：CSV 按字典读
来源：http://bo.asd995.cn

csv.DictReader(f)
来源：http://if.yuexingan06.cn

[U26] Py：并发下载
来源：http://uc.yuexingan06.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://bv.nszjky.cn

[U27] Py：异步 HTTP
来源：http://kx.shxzukj.cn

aiohttp.ClientSession() 配合 async with
来源：http://qg.szsharing.cn

[U28] Py：类型别名
来源：http://nw.huixinmuqiang.cn

UserId = int
来源：http://iv.yuexingan06.cn

[U29] Py：属性校验
来源：http://lb.bookmarksfly.cn

@property 与 @x.setter 配合
来源：http://no.huanxung.cn

[U30] Py：数据类
来源：http://bk.hahajie.cn

@dataclass(slots=True)
来源：http://ru.yuntaijiaju.cn

[U31] Py：单测
来源：http://tp.nicolike.cn

python -m pytest -q
来源：http://lz.bookmarksfly.cn

[U32] Py：代码格式化
来源：http://xy.gzmigu.cn

ruff format . && ruff check --fix .
来源：http://pe.panjiajie.cn

[U33] Py：打包发布
来源：http://wk.bookmarksfly.cn

python -m build  （依赖 pyproject.toml）
来源：http://nt.521024.cn

[U34] Py：判断编码
来源：http://bt.szsharing.cn

chardet.detect(raw)
来源：http://yn.newstarts.cn

[U35] Py：发送邮件
来源：http://hf.hnjuh.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://jd.huanxung.cn

[U36] Py：定时任务
来源：http://cl.bookmarksfly.cn

schedule.every(10).minutes.do(job)
来源：http://jd.yuntaijiaju.cn

[U37] Py：读写 Excel
来源：http://bv.hahajie.cn

pandas.read_excel / DataFrame.to_excel
来源：http://yl.nicolike.cn

[U38] Py：获取脚本所在目录
来源：http://fu.szxytkj.cn

Path(__file__).resolve().parent
来源：http://nv.shxzukj.cn

[U39] Py：判断是否在交互环境
来源：http://kf.huixiangedu.cn

sys.stdout.isatty()
来源：http://oa.szsharing.cn

[U40] Py：打印到标准错误
来源：http://dq.shtwfgs.cn

print("err", file=sys.stderr)
来源：http://au.asd995.cn

[U41] PHP：初始化 Composer 项目
来源：http://dd.muxihuayi.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ae.jctech888.com.cn

[U42] PHP：PSR-4 自动加载
来源：http://dg.muxihuayi.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://be.haigaiapp.cn

[U43] PHP：声明命名空间
来源：http://ye.nszjky.cn

namespace App\Http;
来源：http://dw.521024.cn

[U44] PHP：开启严格类型
来源：http://pc.nicolike.cn

declare(strict_types=1);
来源：http://ln.yuntaijiaju.cn

[U45] PHP：类型声明与返回类型
来源：http://cq.nicolike.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://rc.shxzukj.cn

[U46] PHP：可空类型
来源：http://xo.9csxet.cn

?string $name = null
来源：http://jb.huixinmuqiang.cn


<!-- 参考信息 -->