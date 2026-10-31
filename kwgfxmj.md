代发 wailian999

atoi("42");  strtod("3.14", NULL);
来源：http://bn.shtwfgs.cn

[S23] C：随机数
来源：http://tw.szsharing.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ab.521024.cn

[S24] C：获取本地时间
来源：http://bm.shxzskj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://sa.szxytkj.cn

[S25] C：内存拷贝
来源：http://vs.jctech888.com.cn

memcpy(dst, src, n);
来源：http://tu.newstarts.cn

[S26] C：内存清零
来源：http://vg.szsharing.cn

memset(a, 0, sizeof a);
来源：http://se.shtwfgs.cn

[S27] C：定义常量
来源：http://xy.jctech888.com.cn

const double PI = 3.14159;
来源：http://rn.shtwfgs.cn

[S28] C：静态变量
来源：http://bw.gzmigu.cn

static int counter = 0;
来源：http://rs.gzmigu.cn

[S29] C：变参函数
来源：http://dg.colortex.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ku.haigaiapp.cn

[S30] C：头文件保护
来源：http://ny.muxihuayi.cn

#ifndef X_H
来源：http://qs.newstarts.cn

#define X_H
来源：http://nv.bjjhwx.cn

#endif
来源：http://lz.jianghongdianzi.cn

[S31] C++：Hello World
来源：http://jm.nicolike.cn

#include <iostream>
来源：http://yj.huixiangedu.cn

int main() { std::cout << "Hello\n"; }
来源：http://lj.yuexingan06.cn

[S32] C++：字符串
来源：http://bw.yuntaijiaju.cn

std::string s = "hi";  s += "!";
来源：http://gn.521024.cn

[S33] C++：vector 增删
来源：http://jn.haigaiapp.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ay.gzmigu.cn

[S34] C++：遍历 vector
来源：http://zn.jianghongdianzi.cn

for (auto &x : v) { std::cout << x; }
来源：http://vn.bjjhwx.cn

[S35] C++：map
来源：http://gl.521024.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://qn.jianghongdianzi.cn

[S36] C++：unordered_map
来源：http://ax.lnxyls.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://fd.nszjky.cn

[S37] C++：set
来源：http://os.shtwfgs.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://sl.shxzukj.cn

[S38] C++：排序
来源：http://bc.nicolike.cn

std::sort(v.begin(), v.end());
来源：http://tu.yuexingan06.cn

[S39] C++：自定义比较器排序
来源：http://nb.szxytkj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://wh.bookmarksfly.cn

[S40] C++：查找元素
来源：http://jh.gzmigu.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://lk.shtwfgs.cn

[S41] C++：类与构造函数
来源：http://gs.huanxung.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://av.gzmigu.cn

[S42] C++：继承与虚函数
来源：http://tt.huixiangedu.cn

class B : public Base { public: void f() override {} };
来源：http://sa.asd995.cn

[S43] C++：智能指针
来源：http://pr.wgjwhj.cn

auto p = std::make_unique<int>(5);
来源：http://dc.521024.cn

[S44] C++：引用传参
来源：http://sf.wgjwhj.cn

void inc(int &x) { ++x; }
来源：http://do.521024.cn

[S45] C++：lambda
来源：http://ez.chemitech.net.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ef.521024.cn

[S46] C++：函数模板
来源：http://vl.shxzskj.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://bl.shxzukj.cn

[S47] C++：结构化绑定遍历
来源：http://fy.nicolike.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://jy.lnxyls.cn

[S48] C++：逐行读文件
来源：http://mm.szxytkj.cn

std::ifstream in("a.txt");  std::string line;
来源：http://yw.colortex.cn

while (std::getline(in, line)) { }
来源：http://ta.muxihuayi.cn

[S49] C++：写文件
来源：http://hn.huixinmuqiang.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://id.nszjky.cn

[S50] C++：格式化数字
来源：http://hf.9csxet.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hv.yuexingan06.cn

[S51] C++：显式类型转换
来源：http://ww.nicolike.cn

static_cast<double>(a) / b
来源：http://qs.shxzskj.cn

[S52] C++：const 与 noexcept
来源：http://oy.wgjwhj.cn

int size() const noexcept { return n_; }
来源：http://qz.panjiajie.cn

[S53] C++：移动语义
来源：http://nv.szxytkj.cn

std::vector<int> w = std::move(v);
来源：http://sd.chemitech.net.cn

[S54] C++：异常处理
来源：http://fk.nszjky.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://cp.shtwfgs.cn

[S55] C++：结构化绑定
来源：http://uk.asd995.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://qv.hnjuh.cn

[S56] C++：optional
来源：http://xw.newstarts.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://gk.wgjwhj.cn

[S57] C++：编译期常量
来源：http://fv.bjjhwx.cn

constexpr int N = 10;
来源：http://yj.gzmigu.cn

[S58] C++：命名空间
来源：http://gt.szxytkj.cn

namespace ns { int f() { return 1; } }
来源：http://tc.panjiajie.cn

[S59] C++：静态断言
来源：http://dg.newstarts.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ul.haigaiapp.cn

[S60] C++：遍历并删除元素
来源：http://of.shtwfgs.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://yv.asd995.cn

================================================================================
来源：http://mh.szxytkj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ks.521024.cn

================================================================================
来源：http://rl.asd995.cn

[T01] Kotlin：Hello World
来源：http://hj.colortex.cn

println("Hello")
来源：http://eo.huanxung.cn

[T02] Kotlin：变量
来源：http://wo.huixiangedu.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://tr.wgjwhj.cn

[T03] Kotlin：字符串模板
来源：http://wn.panjiajie.cn

"值: $b"
来源：http://hg.szxytkj.cn

[T04] Kotlin：空安全
来源：http://ha.hnjuh.cn

val n: String? = null;  n?.length
来源：http://ie.shxzukj.cn

[T05] Kotlin：when 表达式
来源：http://py.shxzukj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://kb.yuexingan06.cn

[T06] Kotlin：集合映射
来源：http://zm.huanxung.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://fp.hahajie.cn

[T07] Kotlin：集合过滤
来源：http://fk.bookmarksfly.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ns.hahajie.cn

[T08] Kotlin：数据类
来源：http://ux.nicolike.cn

data class User(val name: String, val age: Int)
来源：http://ol.hnjuh.cn

[T09] Kotlin：扩展函数
来源：http://eu.9csxet.cn

fun String.exclaim() = this + "!"
来源：http://ya.chemitech.net.cn

[T10] Kotlin：默认参数
来源：http://to.jianghongdianzi.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://hc.chemitech.net.cn

[T11] Kotlin：协程
来源：http://pl.nicolike.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ij.szxytkj.cn

[T12] Kotlin：解构声明
来源：http://nd.nicolike.cn

val (a, b) = Pair(1, 2)
来源：http://qa.panjiajie.cn

[T13] Kotlin：只读 Map
来源：http://sp.szsharing.cn

val m = mapOf("a" to 1)
来源：http://zp.hahajie.cn

[T14] Kotlin：循环
来源：http://or.shtwfgs.cn

for (i in 1..10) println(i)
来源：http://ck.szsharing.cn

[T15] Kotlin：接口
来源：http://up.colortex.cn

interface Shape { fun area(): Double }
来源：http://nb.nszjky.cn

[T16] Swift：Hello World
来源：http://ad.huixiangedu.cn

print("Hello")
来源：http://gp.colortex.cn

[T17] Swift：变量与常量
来源：http://mr.shxzukj.cn

var a = 1;  let b = 2
来源：http://mj.szxytkj.cn

[T18] Swift：字符串插值
来源：http://hh.521024.cn

"值: \(b)"
来源：http://yh.gzmigu.cn

[T19] Swift：可选绑定
来源：http://qa.haigaiapp.cn

if let n = opt { print(n) }
来源：http://lx.yuntaijiaju.cn

[T20] Swift：数组操作
来源：http://uq.wgjwhj.cn

var a = [1, 2, 3];  a.append(4)
来源：http://cz.shxzskj.cn

[T21] Swift：遍历
来源：http://bs.shtwfgs.cn

for x in a { print(x) }
来源：http://dp.521024.cn

[T22] Swift：字典
来源：http://xn.9csxet.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ix.panjiajie.cn

[T23] Swift：函数
来源：http://dv.521024.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://sq.haigaiapp.cn

[T24] Swift：闭包
来源：http://xr.colortex.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://rs.shxzskj.cn

[T25] Swift：结构体
来源：http://ns.lnxyls.cn

struct P { var x: Int }
来源：http://em.hahajie.cn

[T26] Swift：类与重写
来源：http://iz.jianghongdianzi.cn

class A: Base { override func f() {} }
来源：http://jn.newstarts.cn

[T27] Swift：错误处理
来源：http://db.shtwfgs.cn

do { try f() } catch { print(error) }
来源：http://fv.szxytkj.cn

[T28] Swift：枚举
来源：http://mp.colortex.cn

enum Color { case red, green }
来源：http://pd.huixiangedu.cn

[T29] Swift：guard 提前返回
来源：http://fc.jianghongdianzi.cn

guard let x = opt else { return }
来源：http://fk.jctech888.com.cn

[T30] Swift：协议
来源：http://kb.shxzskj.cn

protocol Shape { func area() -> Double }
来源：http://bo.huanxung.cn

[T31] Lua：Hello World
来源：http://jt.chemitech.net.cn

print("Hello")
来源：http://hp.newstarts.cn

[T32] Lua：局部变量
来源：http://nb.jctech888.com.cn

local a = 1
来源：http://ow.szxytkj.cn

[T33] Lua：表（数组）
来源：http://eu.colortex.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://vm.newstarts.cn

[T34] Lua：遍历表
来源：http://ri.newstarts.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://fg.9csxet.cn

[T35] Lua：字典表
来源：http://vb.huixinmuqiang.cn

local d = { a = 1 };  d.b = 2
来源：http://ei.hnjuh.cn

[T36] Lua：函数
来源：http://ih.hnjuh.cn

function add(a, b) return a + b end
来源：http://km.huanxung.cn

[T37] Lua：字符串拼接
来源：http://xm.haigaiapp.cn

"a" .. "b"
来源：http://qi.shxzukj.cn

[T38] Lua：条件
来源：http://pi.asd995.cn

if x > 0 then print("正") end
来源：http://pz.haigaiapp.cn

[T39] Lua：模式匹配
来源：http://dr.huanxung.cn

string.find(s, "%d+")
来源：http://jc.nicolike.cn

[T40] Lua：元表
来源：http://xu.muxihuayi.cn

setmetatable({}, { __index = base })
来源：http://pq.huixinmuqiang.cn

[T41] Perl：Hello World
来源：http://af.muxihuayi.cn

print "Hello\n";
来源：http://ea.szxytkj.cn

[T42] Perl：变量类型
来源：http://st.shxzukj.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://yk.huanxung.cn

[T43] Perl：字符串插值
来源：http://ri.haigaiapp.cn

"值: $a"
来源：http://th.bookmarksfly.cn

[T44] Perl：条件
来源：http://xn.colortex.cn

if ($a > 0) { print "正"; }
来源：http://pu.jctech888.com.cn

[T45] Perl：数组遍历
来源：http://yw.panjiajie.cn

for my $x (@arr) { print $x; }
来源：http://ei.nszjky.cn

[T46] Perl：哈希操作
来源：http://eo.muxihuayi.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://at.nicolike.cn

[T47] Perl：正则捕获
来源：http://pp.chemitech.net.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ji.colortex.cn

[T48] Perl：正则替换
来源：http://ax.asd995.cn

$s =~ s/old/new/g;
来源：http://te.asd995.cn

[T49] Perl：函数
来源：http://gk.huanxung.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://vb.szxytkj.cn

[T50] Perl：逐行读文件
来源：http://vd.szsharing.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://bb.szxytkj.cn

while (my $line = <$fh>) { print $line; }
来源：http://qk.521024.cn

[T51] Scala：Hello World
来源：http://xk.wgjwhj.cn

println("Hello")
来源：http://gm.shxzukj.cn

[T52] Scala：变量
来源：http://fc.szsharing.cn

val a = 1;  var b = 2
来源：http://ii.huixinmuqiang.cn

[T53] Scala：字符串插值
来源：http://yd.bjjhwx.cn

s"值: $b"
来源：http://ix.jctech888.com.cn

[T54] Scala：集合映射
来源：http://dz.lnxyls.cn

List(1, 2, 3).map(_ * 2)
来源：http://xm.yuntaijiaju.cn

[T55] Scala：集合过滤
来源：http://fn.lnxyls.cn

List(1, 2, 3).filter(_ > 1)
来源：http://bd.panjiajie.cn

[T56] Scala：样例类
来源：http://uh.szsharing.cn

case class User(name: String, age: Int)
来源：http://fe.chemitech.net.cn

[T57] Scala：模式匹配
来源：http://db.szxytkj.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://sr.shxzukj.cn

[T58] Scala：函数定义
来源：http://df.jianghongdianzi.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ra.bjjhwx.cn

[T59] Scala：循环
来源：http://oi.bookmarksfly.cn

for (i <- 1 to 10) println(i)
来源：http://ci.muxihuayi.cn

[T60] Scala：折叠
来源：http://pa.yuntaijiaju.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://nl.shxzskj.cn

================================================================================
来源：http://yj.shxzskj.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://hh.9csxet.cn

================================================================================
来源：http://rw.wgjwhj.cn

[U01] Py：创建虚拟环境
来源：http://lj.shxzukj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://mt.nicolike.cn

[U02] Py：导出 / 安装依赖
来源：http://ww.muxihuayi.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://lh.newstarts.cn

[U03] Py：加载 .env 配置
来源：http://pp.colortex.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://hw.hahajie.cn

[U04] Py：变量调试打印
来源：http://ts.jianghongdianzi.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://kg.szsharing.cn

[U05] Py：列表去重且保序
来源：http://vo.lnxyls.cn

list(dict.fromkeys(arr))
来源：http://bj.huanxung.cn

[U06] Py：合并两个字典
来源：http://ak.panjiajie.cn

{**a, **b}
来源：http://cb.lnxyls.cn

[U07] Py：反转字典键值
来源：http://ac.panjiajie.cn

{v: k for k, v in d.items()}
来源：http://at.yuexingan06.cn

[U08] Py：展平二维列表
来源：http://ru.bjjhwx.cn

[y for x in nested for y in x]
来源：http://tc.lnxyls.cn

[U09] Py：字典取最大值的键
来源：http://gx.jianghongdianzi.cn

max(d, key=d.get)
来源：http://na.chemitech.net.cn

[U10] Py：按值排序字典
来源：http://ma.shxzukj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://uz.lnxyls.cn

[U11] Py：生成器表达式
来源：http://ri.colortex.cn

(x * 2 for x in arr)
来源：http://yv.9csxet.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ws.gzmigu.cn

Counter(arr).most_common(3)
来源：http://ag.panjiajie.cn

[U13] Py：固定长度队列
来源：http://zc.nszjky.cn

deque(maxlen=10)
来源：http://vn.colortex.cn

[U14] Py：分组收集到列表
来源：http://md.newstarts.cn

defaultdict(list)
来源：http://jw.yuntaijiaju.cn

[U15] Py：高精度计时
来源：http://lp.huixiangedu.cn

t = time.perf_counter()
来源：http://we.9csxet.cn

[U16] Py：命令行参数解析
来源：http://fb.nszjky.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://qd.521024.cn

[U17] Py：初始化日志
来源：http://qw.bookmarksfly.cn

logging.basicConfig(level=logging.INFO)
来源：http://im.haigaiapp.cn

[U18] Py：预编译正则
来源：http://ch.jctech888.com.cn

pat = re.compile(r"\d+")
来源：http://xc.szxytkj.cn

[U19] Py：正则替换带回调
来源：http://fr.huixiangedu.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://fb.haigaiapp.cn

[U20] Py：缓存函数结果
来源：http://am.bjjhwx.cn

@functools.lru_cache(maxsize=None)
来源：http://mk.bookmarksfly.cn

[U21] Py：自定义上下文管理器
来源：http://kt.hnjuh.cn

@contextlib.contextmanager
来源：http://as.huixiangedu.cn

[U22] Py：矩阵转置
来源：http://xp.hahajie.cn

list(zip(*m))
来源：http://wu.shxzskj.cn

[U23] Py：分块读取大文件
来源：http://bw.haigaiapp.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://jw.521024.cn

[U24] Py：路径操作
来源：http://eq.9csxet.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://rq.jctech888.com.cn

[U25] Py：CSV 按字典读
来源：http://ty.szxytkj.cn

csv.DictReader(f)
来源：http://wp.shxzskj.cn

[U26] Py：并发下载
来源：http://qd.jianghongdianzi.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://og.shtwfgs.cn

[U27] Py：异步 HTTP
来源：http://ky.huixiangedu.cn

aiohttp.ClientSession() 配合 async with
来源：http://hs.bjjhwx.cn

[U28] Py：类型别名
来源：http://ck.yuexingan06.cn

UserId = int
来源：http://ff.gzmigu.cn

[U29] Py：属性校验
来源：http://vc.hahajie.cn

@property 与 @x.setter 配合
来源：http://gh.colortex.cn

[U30] Py：数据类
来源：http://to.hnjuh.cn

@dataclass(slots=True)
来源：http://qn.nszjky.cn

[U31] Py：单测
来源：http://uh.nicolike.cn

python -m pytest -q
来源：http://tt.muxihuayi.cn

[U32] Py：代码格式化
来源：http://qa.szsharing.cn

ruff format . && ruff check --fix .
来源：http://ud.shxzskj.cn

[U33] Py：打包发布
来源：http://vr.bookmarksfly.cn

python -m build  （依赖 pyproject.toml）
来源：http://vc.shxzukj.cn

[U34] Py：判断编码
来源：http://ez.muxihuayi.cn

chardet.detect(raw)
来源：http://jv.9csxet.cn

[U35] Py：发送邮件
来源：http://fr.panjiajie.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://bz.huixiangedu.cn

[U36] Py：定时任务
来源：http://nx.jctech888.com.cn

schedule.every(10).minutes.do(job)
来源：http://kk.jctech888.com.cn

[U37] Py：读写 Excel
来源：http://lz.shxzskj.cn

pandas.read_excel / DataFrame.to_excel
来源：http://xb.huixiangedu.cn

[U38] Py：获取脚本所在目录
来源：http://yw.bjjhwx.cn

Path(__file__).resolve().parent
来源：http://kw.szsharing.cn

[U39] Py：判断是否在交互环境
来源：http://vr.panjiajie.cn

sys.stdout.isatty()
来源：http://xr.szsharing.cn

[U40] Py：打印到标准错误
来源：http://lz.lnxyls.cn

print("err", file=sys.stderr)
来源：http://hf.huixiangedu.cn

[U41] PHP：初始化 Composer 项目
来源：http://jg.gzmigu.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://sd.nszjky.cn

[U42] PHP：PSR-4 自动加载
来源：http://hc.szxytkj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ap.hahajie.cn

[U43] PHP：声明命名空间
来源：http://yz.huixiangedu.cn

namespace App\Http;
来源：http://au.shxzskj.cn

[U44] PHP：开启严格类型
来源：http://kl.9csxet.cn

declare(strict_types=1);
来源：http://zc.nicolike.cn

[U45] PHP：类型声明与返回类型
来源：http://ba.haigaiapp.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://qh.nszjky.cn

[U46] PHP：可空类型
来源：http://hi.panjiajie.cn

?string $name = null
来源：http://bo.muxihuayi.cn


<!-- 参考信息 -->