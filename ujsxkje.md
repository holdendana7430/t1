代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://px.huixinmuqiang.cn

[S21] C：字符类别判断
来源：http://nt.gzmigu.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://sk.521024.cn

[S22] C：字符串转数字
来源：http://ov.haigaiapp.cn

atoi("42");  strtod("3.14", NULL);
来源：http://vc.9csxet.cn

[S23] C：随机数
来源：http://ea.chemitech.net.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://nf.colortex.cn

[S24] C：获取本地时间
来源：http://wc.haigaiapp.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ma.wgjwhj.cn

[S25] C：内存拷贝
来源：http://sy.521024.cn

memcpy(dst, src, n);
来源：http://rz.asd995.cn

[S26] C：内存清零
来源：http://hp.nszjky.cn

memset(a, 0, sizeof a);
来源：http://qj.szsharing.cn

[S27] C：定义常量
来源：http://mw.newstarts.cn

const double PI = 3.14159;
来源：http://dh.huanxung.cn

[S28] C：静态变量
来源：http://gv.shtwfgs.cn

static int counter = 0;
来源：http://wo.hnjuh.cn

[S29] C：变参函数
来源：http://gl.bookmarksfly.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ub.panjiajie.cn

[S30] C：头文件保护
来源：http://ba.lnxyls.cn

#ifndef X_H
来源：http://mn.yuntaijiaju.cn

#define X_H
来源：http://ov.huixinmuqiang.cn

#endif
来源：http://ym.bjjhwx.cn

[S31] C++：Hello World
来源：http://hy.huanxung.cn

#include <iostream>
来源：http://rq.shtwfgs.cn

int main() { std::cout << "Hello\n"; }
来源：http://ju.hnjuh.cn

[S32] C++：字符串
来源：http://bz.shtwfgs.cn

std::string s = "hi";  s += "!";
来源：http://jb.gzmigu.cn

[S33] C++：vector 增删
来源：http://mi.nicolike.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ot.hahajie.cn

[S34] C++：遍历 vector
来源：http://wm.jctech888.com.cn

for (auto &x : v) { std::cout << x; }
来源：http://qf.huixiangedu.cn

[S35] C++：map
来源：http://lv.bookmarksfly.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ms.muxihuayi.cn

[S36] C++：unordered_map
来源：http://bo.huixinmuqiang.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ia.chemitech.net.cn

[S37] C++：set
来源：http://op.hnjuh.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ox.lnxyls.cn

[S38] C++：排序
来源：http://fq.jianghongdianzi.cn

std::sort(v.begin(), v.end());
来源：http://yf.hnjuh.cn

[S39] C++：自定义比较器排序
来源：http://vv.9csxet.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://qi.bookmarksfly.cn

[S40] C++：查找元素
来源：http://tl.huixinmuqiang.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://tg.huixinmuqiang.cn

[S41] C++：类与构造函数
来源：http://zd.huanxung.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wa.bjjhwx.cn

[S42] C++：继承与虚函数
来源：http://os.gzmigu.cn

class B : public Base { public: void f() override {} };
来源：http://ug.jctech888.com.cn

[S43] C++：智能指针
来源：http://jn.chemitech.net.cn

auto p = std::make_unique<int>(5);
来源：http://mz.asd995.cn

[S44] C++：引用传参
来源：http://ug.bookmarksfly.cn

void inc(int &x) { ++x; }
来源：http://oe.muxihuayi.cn

[S45] C++：lambda
来源：http://cw.szsharing.cn

auto add = [](int a, int b) { return a + b; };
来源：http://qs.shxzskj.cn

[S46] C++：函数模板
来源：http://tx.nicolike.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://zv.szsharing.cn

[S47] C++：结构化绑定遍历
来源：http://vw.huixiangedu.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ix.yuntaijiaju.cn

[S48] C++：逐行读文件
来源：http://sf.yuexingan06.cn

std::ifstream in("a.txt");  std::string line;
来源：http://sj.newstarts.cn

while (std::getline(in, line)) { }
来源：http://rj.jianghongdianzi.cn

[S49] C++：写文件
来源：http://fq.bookmarksfly.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ra.hnjuh.cn

[S50] C++：格式化数字
来源：http://ai.9csxet.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wa.bjjhwx.cn

[S51] C++：显式类型转换
来源：http://eg.newstarts.cn

static_cast<double>(a) / b
来源：http://pp.lnxyls.cn

[S52] C++：const 与 noexcept
来源：http://is.jianghongdianzi.cn

int size() const noexcept { return n_; }
来源：http://gx.muxihuayi.cn

[S53] C++：移动语义
来源：http://vz.hahajie.cn

std::vector<int> w = std::move(v);
来源：http://od.huixiangedu.cn

[S54] C++：异常处理
来源：http://dk.panjiajie.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://sl.shxzskj.cn

[S55] C++：结构化绑定
来源：http://qg.szxytkj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://az.newstarts.cn

[S56] C++：optional
来源：http://qn.lnxyls.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://so.huixinmuqiang.cn

[S57] C++：编译期常量
来源：http://tr.haigaiapp.cn

constexpr int N = 10;
来源：http://od.huixinmuqiang.cn

[S58] C++：命名空间
来源：http://rz.jctech888.com.cn

namespace ns { int f() { return 1; } }
来源：http://nt.521024.cn

[S59] C++：静态断言
来源：http://yk.521024.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ds.huixiangedu.cn

[S60] C++：遍历并删除元素
来源：http://cu.521024.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://se.hahajie.cn

================================================================================
来源：http://sh.shxzskj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://jg.9csxet.cn

================================================================================
来源：http://ty.shtwfgs.cn

[T01] Kotlin：Hello World
来源：http://vu.yuntaijiaju.cn

println("Hello")
来源：http://kf.shxzskj.cn

[T02] Kotlin：变量
来源：http://gr.jctech888.com.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://pf.wgjwhj.cn

[T03] Kotlin：字符串模板
来源：http://jw.huixinmuqiang.cn

"值: $b"
来源：http://hi.muxihuayi.cn

[T04] Kotlin：空安全
来源：http://fq.muxihuayi.cn

val n: String? = null;  n?.length
来源：http://pi.szxytkj.cn

[T05] Kotlin：when 表达式
来源：http://ol.szsharing.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ci.asd995.cn

[T06] Kotlin：集合映射
来源：http://rs.haigaiapp.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://rq.wgjwhj.cn

[T07] Kotlin：集合过滤
来源：http://xw.huixinmuqiang.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ad.lnxyls.cn

[T08] Kotlin：数据类
来源：http://zi.jctech888.com.cn

data class User(val name: String, val age: Int)
来源：http://ia.gzmigu.cn

[T09] Kotlin：扩展函数
来源：http://zc.panjiajie.cn

fun String.exclaim() = this + "!"
来源：http://ik.chemitech.net.cn

[T10] Kotlin：默认参数
来源：http://yb.jctech888.com.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://mm.szsharing.cn

[T11] Kotlin：协程
来源：http://xb.szsharing.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ak.nicolike.cn

[T12] Kotlin：解构声明
来源：http://yy.shtwfgs.cn

val (a, b) = Pair(1, 2)
来源：http://tv.huanxung.cn

[T13] Kotlin：只读 Map
来源：http://sy.gzmigu.cn

val m = mapOf("a" to 1)
来源：http://mv.newstarts.cn

[T14] Kotlin：循环
来源：http://nv.lnxyls.cn

for (i in 1..10) println(i)
来源：http://ot.szsharing.cn

[T15] Kotlin：接口
来源：http://nm.nszjky.cn

interface Shape { fun area(): Double }
来源：http://vp.newstarts.cn

[T16] Swift：Hello World
来源：http://jl.lnxyls.cn

print("Hello")
来源：http://fx.lnxyls.cn

[T17] Swift：变量与常量
来源：http://rl.shtwfgs.cn

var a = 1;  let b = 2
来源：http://wu.hahajie.cn

[T18] Swift：字符串插值
来源：http://tm.hahajie.cn

"值: \(b)"
来源：http://yj.jctech888.com.cn

[T19] Swift：可选绑定
来源：http://hb.newstarts.cn

if let n = opt { print(n) }
来源：http://fh.asd995.cn

[T20] Swift：数组操作
来源：http://pu.jianghongdianzi.cn

var a = [1, 2, 3];  a.append(4)
来源：http://qj.521024.cn

[T21] Swift：遍历
来源：http://sa.asd995.cn

for x in a { print(x) }
来源：http://um.szxytkj.cn

[T22] Swift：字典
来源：http://vr.gzmigu.cn

var d = ["a": 1];  d["b"] = 2
来源：http://su.shxzskj.cn

[T23] Swift：函数
来源：http://mb.hnjuh.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://cs.huixiangedu.cn

[T24] Swift：闭包
来源：http://me.szxytkj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://bc.huixiangedu.cn

[T25] Swift：结构体
来源：http://oe.chemitech.net.cn

struct P { var x: Int }
来源：http://gc.chemitech.net.cn

[T26] Swift：类与重写
来源：http://lu.haigaiapp.cn

class A: Base { override func f() {} }
来源：http://dy.lnxyls.cn

[T27] Swift：错误处理
来源：http://ce.9csxet.cn

do { try f() } catch { print(error) }
来源：http://jn.yuexingan06.cn

[T28] Swift：枚举
来源：http://ye.bjjhwx.cn

enum Color { case red, green }
来源：http://gc.yuntaijiaju.cn

[T29] Swift：guard 提前返回
来源：http://wg.asd995.cn

guard let x = opt else { return }
来源：http://hm.chemitech.net.cn

[T30] Swift：协议
来源：http://wb.wgjwhj.cn

protocol Shape { func area() -> Double }
来源：http://kr.szxytkj.cn

[T31] Lua：Hello World
来源：http://ab.jianghongdianzi.cn

print("Hello")
来源：http://xi.9csxet.cn

[T32] Lua：局部变量
来源：http://fb.panjiajie.cn

local a = 1
来源：http://ww.yuntaijiaju.cn

[T33] Lua：表（数组）
来源：http://dp.yuntaijiaju.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://tf.asd995.cn

[T34] Lua：遍历表
来源：http://tb.nicolike.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://zo.jctech888.com.cn

[T35] Lua：字典表
来源：http://aa.asd995.cn

local d = { a = 1 };  d.b = 2
来源：http://bw.yuntaijiaju.cn

[T36] Lua：函数
来源：http://kw.panjiajie.cn

function add(a, b) return a + b end
来源：http://zx.chemitech.net.cn

[T37] Lua：字符串拼接
来源：http://yr.shtwfgs.cn

"a" .. "b"
来源：http://mo.huixinmuqiang.cn

[T38] Lua：条件
来源：http://la.huixiangedu.cn

if x > 0 then print("正") end
来源：http://gu.bjjhwx.cn

[T39] Lua：模式匹配
来源：http://fu.hahajie.cn

string.find(s, "%d+")
来源：http://rn.jctech888.com.cn

[T40] Lua：元表
来源：http://hd.hahajie.cn

setmetatable({}, { __index = base })
来源：http://yj.muxihuayi.cn

[T41] Perl：Hello World
来源：http://ce.yuexingan06.cn

print "Hello\n";
来源：http://dx.panjiajie.cn

[T42] Perl：变量类型
来源：http://wn.jianghongdianzi.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://yr.shxzukj.cn

[T43] Perl：字符串插值
来源：http://ej.521024.cn

"值: $a"
来源：http://kn.hahajie.cn

[T44] Perl：条件
来源：http://mw.panjiajie.cn

if ($a > 0) { print "正"; }
来源：http://ui.shxzukj.cn

[T45] Perl：数组遍历
来源：http://kl.nszjky.cn

for my $x (@arr) { print $x; }
来源：http://me.shxzskj.cn

[T46] Perl：哈希操作
来源：http://sa.shxzskj.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ka.yuntaijiaju.cn

[T47] Perl：正则捕获
来源：http://qx.muxihuayi.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://uo.panjiajie.cn

[T48] Perl：正则替换
来源：http://ed.shxzskj.cn

$s =~ s/old/new/g;
来源：http://yn.panjiajie.cn

[T49] Perl：函数
来源：http://lw.9csxet.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ue.haigaiapp.cn

[T50] Perl：逐行读文件
来源：http://jb.asd995.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ht.bjjhwx.cn

while (my $line = <$fh>) { print $line; }
来源：http://ke.shxzskj.cn

[T51] Scala：Hello World
来源：http://wo.521024.cn

println("Hello")
来源：http://gt.hahajie.cn

[T52] Scala：变量
来源：http://ge.jianghongdianzi.cn

val a = 1;  var b = 2
来源：http://uk.yuntaijiaju.cn

[T53] Scala：字符串插值
来源：http://ae.9csxet.cn

s"值: $b"
来源：http://iw.huixinmuqiang.cn

[T54] Scala：集合映射
来源：http://rr.muxihuayi.cn

List(1, 2, 3).map(_ * 2)
来源：http://ka.panjiajie.cn

[T55] Scala：集合过滤
来源：http://pf.lnxyls.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ia.huixiangedu.cn

[T56] Scala：样例类
来源：http://gs.muxihuayi.cn

case class User(name: String, age: Int)
来源：http://nf.lnxyls.cn

[T57] Scala：模式匹配
来源：http://bd.gzmigu.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://vx.wgjwhj.cn

[T58] Scala：函数定义
来源：http://xp.bjjhwx.cn

def add(a: Int, b: Int): Int = a + b
来源：http://gl.shxzskj.cn

[T59] Scala：循环
来源：http://en.jianghongdianzi.cn

for (i <- 1 to 10) println(i)
来源：http://jm.hnjuh.cn

[T60] Scala：折叠
来源：http://hp.szsharing.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://rs.szsharing.cn

================================================================================
来源：http://dn.hahajie.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://qi.chemitech.net.cn

================================================================================
来源：http://ul.nicolike.cn

[U01] Py：创建虚拟环境
来源：http://yz.muxihuayi.cn

python -m venv .venv && source .venv/bin/activate
来源：http://kq.bookmarksfly.cn

[U02] Py：导出 / 安装依赖
来源：http://eg.bjjhwx.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://un.shxzskj.cn

[U03] Py：加载 .env 配置
来源：http://er.shtwfgs.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://at.shxzskj.cn

[U04] Py：变量调试打印
来源：http://lc.jianghongdianzi.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ez.hahajie.cn

[U05] Py：列表去重且保序
来源：http://gh.nicolike.cn

list(dict.fromkeys(arr))
来源：http://qx.muxihuayi.cn

[U06] Py：合并两个字典
来源：http://kk.colortex.cn

{**a, **b}
来源：http://qw.huixinmuqiang.cn

[U07] Py：反转字典键值
来源：http://nx.shxzskj.cn

{v: k for k, v in d.items()}
来源：http://dr.muxihuayi.cn

[U08] Py：展平二维列表
来源：http://ut.huanxung.cn

[y for x in nested for y in x]
来源：http://oy.hnjuh.cn

[U09] Py：字典取最大值的键
来源：http://kt.muxihuayi.cn

max(d, key=d.get)
来源：http://qp.bookmarksfly.cn

[U10] Py：按值排序字典
来源：http://se.jianghongdianzi.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://gz.jianghongdianzi.cn

[U11] Py：生成器表达式
来源：http://jd.shxzskj.cn

(x * 2 for x in arr)
来源：http://uc.bookmarksfly.cn

[U12] Py：取出现最多的 3 个元素
来源：http://vb.szxytkj.cn

Counter(arr).most_common(3)
来源：http://dc.huanxung.cn

[U13] Py：固定长度队列
来源：http://qu.wgjwhj.cn

deque(maxlen=10)
来源：http://vf.haigaiapp.cn

[U14] Py：分组收集到列表
来源：http://jv.gzmigu.cn

defaultdict(list)
来源：http://im.muxihuayi.cn

[U15] Py：高精度计时
来源：http://cq.haigaiapp.cn

t = time.perf_counter()
来源：http://sl.9csxet.cn

[U16] Py：命令行参数解析
来源：http://mi.huixinmuqiang.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://bv.haigaiapp.cn

[U17] Py：初始化日志
来源：http://hv.jianghongdianzi.cn

logging.basicConfig(level=logging.INFO)
来源：http://nr.newstarts.cn

[U18] Py：预编译正则
来源：http://yq.szxytkj.cn

pat = re.compile(r"\d+")
来源：http://ek.nicolike.cn

[U19] Py：正则替换带回调
来源：http://sx.shxzukj.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://ta.huixinmuqiang.cn

[U20] Py：缓存函数结果
来源：http://sl.jctech888.com.cn

@functools.lru_cache(maxsize=None)
来源：http://gb.chemitech.net.cn

[U21] Py：自定义上下文管理器
来源：http://yc.yuexingan06.cn

@contextlib.contextmanager
来源：http://rl.szxytkj.cn

[U22] Py：矩阵转置
来源：http://ki.colortex.cn

list(zip(*m))
来源：http://za.hahajie.cn

[U23] Py：分块读取大文件
来源：http://kc.hnjuh.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://bn.wgjwhj.cn

[U24] Py：路径操作
来源：http://fp.yuntaijiaju.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://bf.muxihuayi.cn

[U25] Py：CSV 按字典读
来源：http://vn.huanxung.cn

csv.DictReader(f)
来源：http://jl.nicolike.cn

[U26] Py：并发下载
来源：http://fq.bjjhwx.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://fo.nicolike.cn

[U27] Py：异步 HTTP
来源：http://yz.bjjhwx.cn

aiohttp.ClientSession() 配合 async with
来源：http://uy.colortex.cn

[U28] Py：类型别名
来源：http://lj.hahajie.cn

UserId = int
来源：http://ir.shtwfgs.cn

[U29] Py：属性校验
来源：http://zp.newstarts.cn

@property 与 @x.setter 配合
来源：http://pw.nszjky.cn

[U30] Py：数据类
来源：http://bp.9csxet.cn

@dataclass(slots=True)
来源：http://ve.shxzukj.cn

[U31] Py：单测
来源：http://si.huanxung.cn

python -m pytest -q
来源：http://uo.shxzukj.cn

[U32] Py：代码格式化
来源：http://zj.szxytkj.cn

ruff format . && ruff check --fix .
来源：http://cz.9csxet.cn

[U33] Py：打包发布
来源：http://it.panjiajie.cn

python -m build  （依赖 pyproject.toml）
来源：http://xv.wgjwhj.cn

[U34] Py：判断编码
来源：http://pg.huanxung.cn

chardet.detect(raw)
来源：http://gx.shxzukj.cn

[U35] Py：发送邮件
来源：http://xa.hahajie.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://cj.haigaiapp.cn

[U36] Py：定时任务
来源：http://qd.521024.cn

schedule.every(10).minutes.do(job)
来源：http://bk.hnjuh.cn

[U37] Py：读写 Excel
来源：http://ep.huixinmuqiang.cn

pandas.read_excel / DataFrame.to_excel
来源：http://oj.chemitech.net.cn

[U38] Py：获取脚本所在目录
来源：http://yp.bjjhwx.cn

Path(__file__).resolve().parent
来源：http://mx.9csxet.cn

[U39] Py：判断是否在交互环境
来源：http://ly.jianghongdianzi.cn

sys.stdout.isatty()
来源：http://ba.colortex.cn

[U40] Py：打印到标准错误
来源：http://qb.huanxung.cn

print("err", file=sys.stderr)
来源：http://eg.lnxyls.cn

[U41] PHP：初始化 Composer 项目
来源：http://jf.shtwfgs.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://gd.nicolike.cn

[U42] PHP：PSR-4 自动加载
来源：http://xx.huixinmuqiang.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://kw.hnjuh.cn

[U43] PHP：声明命名空间
来源：http://ma.haigaiapp.cn

namespace App\Http;
来源：http://rm.colortex.cn

[U44] PHP：开启严格类型
来源：http://je.nszjky.cn

declare(strict_types=1);
来源：http://yl.haigaiapp.cn


<!-- 参考信息 -->