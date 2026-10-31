代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ix.nszjky.cn

[S25] C：内存拷贝
来源：http://zo.colortex.cn

memcpy(dst, src, n);
来源：http://be.shxzskj.cn

[S26] C：内存清零
来源：http://jy.nicolike.cn

memset(a, 0, sizeof a);
来源：http://oy.yuexingan06.cn

[S27] C：定义常量
来源：http://pz.hahajie.cn

const double PI = 3.14159;
来源：http://in.panjiajie.cn

[S28] C：静态变量
来源：http://jy.nicolike.cn

static int counter = 0;
来源：http://vl.huixiangedu.cn

[S29] C：变参函数
来源：http://mt.lnxyls.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ly.shxzukj.cn

[S30] C：头文件保护
来源：http://tf.bjjhwx.cn

#ifndef X_H
来源：http://lr.lnxyls.cn

#define X_H
来源：http://ku.huixinmuqiang.cn

#endif
来源：http://id.wgjwhj.cn

[S31] C++：Hello World
来源：http://eb.9csxet.cn

#include <iostream>
来源：http://qc.521024.cn

int main() { std::cout << "Hello\n"; }
来源：http://mg.521024.cn

[S32] C++：字符串
来源：http://uh.szsharing.cn

std::string s = "hi";  s += "!";
来源：http://wc.shxzukj.cn

[S33] C++：vector 增删
来源：http://tc.wgjwhj.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://jg.gzmigu.cn

[S34] C++：遍历 vector
来源：http://pu.colortex.cn

for (auto &x : v) { std::cout << x; }
来源：http://cb.yuexingan06.cn

[S35] C++：map
来源：http://hg.asd995.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://oo.521024.cn

[S36] C++：unordered_map
来源：http://op.lnxyls.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ko.nszjky.cn

[S37] C++：set
来源：http://po.colortex.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://bi.gzmigu.cn

[S38] C++：排序
来源：http://tj.colortex.cn

std::sort(v.begin(), v.end());
来源：http://ua.huixinmuqiang.cn

[S39] C++：自定义比较器排序
来源：http://of.newstarts.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://qt.shtwfgs.cn

[S40] C++：查找元素
来源：http://so.yuexingan06.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://gs.lnxyls.cn

[S41] C++：类与构造函数
来源：http://hy.nszjky.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ps.yuexingan06.cn

[S42] C++：继承与虚函数
来源：http://ng.bookmarksfly.cn

class B : public Base { public: void f() override {} };
来源：http://bh.yuexingan06.cn

[S43] C++：智能指针
来源：http://mw.asd995.cn

auto p = std::make_unique<int>(5);
来源：http://jf.9csxet.cn

[S44] C++：引用传参
来源：http://vf.shtwfgs.cn

void inc(int &x) { ++x; }
来源：http://dy.muxihuayi.cn

[S45] C++：lambda
来源：http://yh.bjjhwx.cn

auto add = [](int a, int b) { return a + b; };
来源：http://oi.huixiangedu.cn

[S46] C++：函数模板
来源：http://es.huixiangedu.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://pu.nicolike.cn

[S47] C++：结构化绑定遍历
来源：http://ob.gzmigu.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://by.huanxung.cn

[S48] C++：逐行读文件
来源：http://bi.bjjhwx.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ma.muxihuayi.cn

while (std::getline(in, line)) { }
来源：http://kl.521024.cn

[S49] C++：写文件
来源：http://fi.huixiangedu.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://gm.521024.cn

[S50] C++：格式化数字
来源：http://cy.yuexingan06.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://so.colortex.cn

[S51] C++：显式类型转换
来源：http://ny.nszjky.cn

static_cast<double>(a) / b
来源：http://ly.haigaiapp.cn

[S52] C++：const 与 noexcept
来源：http://yb.9csxet.cn

int size() const noexcept { return n_; }
来源：http://zl.huixinmuqiang.cn

[S53] C++：移动语义
来源：http://ty.jianghongdianzi.cn

std::vector<int> w = std::move(v);
来源：http://mz.521024.cn

[S54] C++：异常处理
来源：http://lp.shxzskj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ej.nicolike.cn

[S55] C++：结构化绑定
来源：http://pg.hahajie.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://uz.nicolike.cn

[S56] C++：optional
来源：http://ll.panjiajie.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://zl.lnxyls.cn

[S57] C++：编译期常量
来源：http://fi.bookmarksfly.cn

constexpr int N = 10;
来源：http://db.newstarts.cn

[S58] C++：命名空间
来源：http://fw.hahajie.cn

namespace ns { int f() { return 1; } }
来源：http://vi.521024.cn

[S59] C++：静态断言
来源：http://pi.huixinmuqiang.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qv.hahajie.cn

[S60] C++：遍历并删除元素
来源：http://gy.huixiangedu.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://uo.huanxung.cn

================================================================================
来源：http://pi.shtwfgs.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://yr.shtwfgs.cn

================================================================================
来源：http://gd.panjiajie.cn

[T01] Kotlin：Hello World
来源：http://hl.jctech888.com.cn

println("Hello")
来源：http://yi.shxzukj.cn

[T02] Kotlin：变量
来源：http://vx.yuntaijiaju.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://xx.chemitech.net.cn

[T03] Kotlin：字符串模板
来源：http://up.shxzskj.cn

"值: $b"
来源：http://yw.hnjuh.cn

[T04] Kotlin：空安全
来源：http://di.gzmigu.cn

val n: String? = null;  n?.length
来源：http://wl.jctech888.com.cn

[T05] Kotlin：when 表达式
来源：http://bw.shxzukj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://lf.bjjhwx.cn

[T06] Kotlin：集合映射
来源：http://gj.lnxyls.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ag.yuexingan06.cn

[T07] Kotlin：集合过滤
来源：http://nb.shxzskj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://nb.shtwfgs.cn

[T08] Kotlin：数据类
来源：http://gv.yuexingan06.cn

data class User(val name: String, val age: Int)
来源：http://yh.wgjwhj.cn

[T09] Kotlin：扩展函数
来源：http://mj.huanxung.cn

fun String.exclaim() = this + "!"
来源：http://vk.lnxyls.cn

[T10] Kotlin：默认参数
来源：http://xj.bookmarksfly.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://la.huanxung.cn

[T11] Kotlin：协程
来源：http://cq.szsharing.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://zm.shtwfgs.cn

[T12] Kotlin：解构声明
来源：http://gm.bjjhwx.cn

val (a, b) = Pair(1, 2)
来源：http://jw.colortex.cn

[T13] Kotlin：只读 Map
来源：http://hy.szsharing.cn

val m = mapOf("a" to 1)
来源：http://fs.521024.cn

[T14] Kotlin：循环
来源：http://da.shtwfgs.cn

for (i in 1..10) println(i)
来源：http://tg.hnjuh.cn

[T15] Kotlin：接口
来源：http://ir.asd995.cn

interface Shape { fun area(): Double }
来源：http://pb.haigaiapp.cn

[T16] Swift：Hello World
来源：http://cv.huanxung.cn

print("Hello")
来源：http://zd.jianghongdianzi.cn

[T17] Swift：变量与常量
来源：http://si.nszjky.cn

var a = 1;  let b = 2
来源：http://yd.haigaiapp.cn

[T18] Swift：字符串插值
来源：http://gh.bjjhwx.cn

"值: \(b)"
来源：http://qf.szsharing.cn

[T19] Swift：可选绑定
来源：http://pp.9csxet.cn

if let n = opt { print(n) }
来源：http://gs.szsharing.cn

[T20] Swift：数组操作
来源：http://ik.chemitech.net.cn

var a = [1, 2, 3];  a.append(4)
来源：http://zy.bjjhwx.cn

[T21] Swift：遍历
来源：http://ju.wgjwhj.cn

for x in a { print(x) }
来源：http://xi.huixiangedu.cn

[T22] Swift：字典
来源：http://ed.szxytkj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://nn.hahajie.cn

[T23] Swift：函数
来源：http://wu.nicolike.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://lf.yuexingan06.cn

[T24] Swift：闭包
来源：http://im.chemitech.net.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ok.jianghongdianzi.cn

[T25] Swift：结构体
来源：http://ob.jianghongdianzi.cn

struct P { var x: Int }
来源：http://kh.9csxet.cn

[T26] Swift：类与重写
来源：http://he.haigaiapp.cn

class A: Base { override func f() {} }
来源：http://rj.nicolike.cn

[T27] Swift：错误处理
来源：http://ny.521024.cn

do { try f() } catch { print(error) }
来源：http://dg.huanxung.cn

[T28] Swift：枚举
来源：http://gt.521024.cn

enum Color { case red, green }
来源：http://te.haigaiapp.cn

[T29] Swift：guard 提前返回
来源：http://ea.bookmarksfly.cn

guard let x = opt else { return }
来源：http://nb.szsharing.cn

[T30] Swift：协议
来源：http://nm.muxihuayi.cn

protocol Shape { func area() -> Double }
来源：http://lq.jianghongdianzi.cn

[T31] Lua：Hello World
来源：http://fk.huixiangedu.cn

print("Hello")
来源：http://tp.shxzskj.cn

[T32] Lua：局部变量
来源：http://bl.newstarts.cn

local a = 1
来源：http://hd.jianghongdianzi.cn

[T33] Lua：表（数组）
来源：http://bk.huixinmuqiang.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://rl.hnjuh.cn

[T34] Lua：遍历表
来源：http://xd.huixinmuqiang.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://aw.szsharing.cn

[T35] Lua：字典表
来源：http://qy.jianghongdianzi.cn

local d = { a = 1 };  d.b = 2
来源：http://mb.szsharing.cn

[T36] Lua：函数
来源：http://ve.haigaiapp.cn

function add(a, b) return a + b end
来源：http://hn.jctech888.com.cn

[T37] Lua：字符串拼接
来源：http://ni.huixinmuqiang.cn

"a" .. "b"
来源：http://rr.lnxyls.cn

[T38] Lua：条件
来源：http://yy.bookmarksfly.cn

if x > 0 then print("正") end
来源：http://kk.shxzukj.cn

[T39] Lua：模式匹配
来源：http://lq.shxzskj.cn

string.find(s, "%d+")
来源：http://zt.muxihuayi.cn

[T40] Lua：元表
来源：http://ta.szsharing.cn

setmetatable({}, { __index = base })
来源：http://jl.haigaiapp.cn

[T41] Perl：Hello World
来源：http://jr.panjiajie.cn

print "Hello\n";
来源：http://qg.szsharing.cn

[T42] Perl：变量类型
来源：http://zp.hahajie.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ag.521024.cn

[T43] Perl：字符串插值
来源：http://tu.huanxung.cn

"值: $a"
来源：http://hi.muxihuayi.cn

[T44] Perl：条件
来源：http://gq.nicolike.cn

if ($a > 0) { print "正"; }
来源：http://aw.bookmarksfly.cn

[T45] Perl：数组遍历
来源：http://vo.hnjuh.cn

for my $x (@arr) { print $x; }
来源：http://rb.haigaiapp.cn

[T46] Perl：哈希操作
来源：http://ru.gzmigu.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://bb.521024.cn

[T47] Perl：正则捕获
来源：http://uj.panjiajie.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://je.bookmarksfly.cn

[T48] Perl：正则替换
来源：http://vs.wgjwhj.cn

$s =~ s/old/new/g;
来源：http://is.shxzskj.cn

[T49] Perl：函数
来源：http://pj.hnjuh.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://db.lnxyls.cn

[T50] Perl：逐行读文件
来源：http://zq.hahajie.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://he.jctech888.com.cn

while (my $line = <$fh>) { print $line; }
来源：http://ev.newstarts.cn

[T51] Scala：Hello World
来源：http://mc.haigaiapp.cn

println("Hello")
来源：http://ju.chemitech.net.cn

[T52] Scala：变量
来源：http://xt.szsharing.cn

val a = 1;  var b = 2
来源：http://hj.hnjuh.cn

[T53] Scala：字符串插值
来源：http://dx.yuexingan06.cn

s"值: $b"
来源：http://os.hnjuh.cn

[T54] Scala：集合映射
来源：http://oo.colortex.cn

List(1, 2, 3).map(_ * 2)
来源：http://bn.muxihuayi.cn

[T55] Scala：集合过滤
来源：http://vk.szxytkj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://bf.hahajie.cn

[T56] Scala：样例类
来源：http://et.gzmigu.cn

case class User(name: String, age: Int)
来源：http://hj.hnjuh.cn

[T57] Scala：模式匹配
来源：http://dw.bjjhwx.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://jq.szsharing.cn

[T58] Scala：函数定义
来源：http://za.colortex.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ey.bookmarksfly.cn

[T59] Scala：循环
来源：http://uj.jianghongdianzi.cn

for (i <- 1 to 10) println(i)
来源：http://of.huixiangedu.cn

[T60] Scala：折叠
来源：http://us.lnxyls.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://vn.lnxyls.cn

================================================================================
来源：http://eo.szxytkj.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://cy.9csxet.cn

================================================================================
来源：http://ra.yuntaijiaju.cn

[U01] Py：创建虚拟环境
来源：http://wp.asd995.cn

python -m venv .venv && source .venv/bin/activate
来源：http://zw.yuntaijiaju.cn

[U02] Py：导出 / 安装依赖
来源：http://nu.lnxyls.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://mx.newstarts.cn

[U03] Py：加载 .env 配置
来源：http://rt.muxihuayi.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://xn.huixinmuqiang.cn

[U04] Py：变量调试打印
来源：http://zz.huixiangedu.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://qn.szxytkj.cn

[U05] Py：列表去重且保序
来源：http://dd.nszjky.cn

list(dict.fromkeys(arr))
来源：http://mi.panjiajie.cn

[U06] Py：合并两个字典
来源：http://gq.huixinmuqiang.cn

{**a, **b}
来源：http://xw.shxzskj.cn

[U07] Py：反转字典键值
来源：http://ao.bjjhwx.cn

{v: k for k, v in d.items()}
来源：http://ye.huixiangedu.cn

[U08] Py：展平二维列表
来源：http://bf.huanxung.cn

[y for x in nested for y in x]
来源：http://yu.newstarts.cn

[U09] Py：字典取最大值的键
来源：http://og.huixinmuqiang.cn

max(d, key=d.get)
来源：http://mm.gzmigu.cn

[U10] Py：按值排序字典
来源：http://or.huixinmuqiang.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ed.bjjhwx.cn

[U11] Py：生成器表达式
来源：http://va.panjiajie.cn

(x * 2 for x in arr)
来源：http://qc.shxzukj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ln.huanxung.cn

Counter(arr).most_common(3)
来源：http://va.szsharing.cn

[U13] Py：固定长度队列
来源：http://dc.shtwfgs.cn

deque(maxlen=10)
来源：http://dh.jianghongdianzi.cn

[U14] Py：分组收集到列表
来源：http://cs.lnxyls.cn

defaultdict(list)
来源：http://nn.huixinmuqiang.cn

[U15] Py：高精度计时
来源：http://id.shxzukj.cn

t = time.perf_counter()
来源：http://ue.shtwfgs.cn

[U16] Py：命令行参数解析
来源：http://nh.yuntaijiaju.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ak.huixiangedu.cn

[U17] Py：初始化日志
来源：http://sh.wgjwhj.cn

logging.basicConfig(level=logging.INFO)
来源：http://xz.521024.cn

[U18] Py：预编译正则
来源：http://fq.lnxyls.cn

pat = re.compile(r"\d+")
来源：http://bj.nicolike.cn

[U19] Py：正则替换带回调
来源：http://jz.wgjwhj.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://sr.newstarts.cn

[U20] Py：缓存函数结果
来源：http://hn.9csxet.cn

@functools.lru_cache(maxsize=None)
来源：http://vx.shxzskj.cn

[U21] Py：自定义上下文管理器
来源：http://iz.jctech888.com.cn

@contextlib.contextmanager
来源：http://uc.newstarts.cn

[U22] Py：矩阵转置
来源：http://ti.bjjhwx.cn

list(zip(*m))
来源：http://sc.szsharing.cn

[U23] Py：分块读取大文件
来源：http://du.9csxet.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://og.521024.cn

[U24] Py：路径操作
来源：http://gg.9csxet.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ed.asd995.cn

[U25] Py：CSV 按字典读
来源：http://zv.jianghongdianzi.cn

csv.DictReader(f)
来源：http://rc.nicolike.cn

[U26] Py：并发下载
来源：http://no.bookmarksfly.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://qh.nicolike.cn

[U27] Py：异步 HTTP
来源：http://fc.szxytkj.cn

aiohttp.ClientSession() 配合 async with
来源：http://aq.muxihuayi.cn

[U28] Py：类型别名
来源：http://gi.szsharing.cn

UserId = int
来源：http://yn.shtwfgs.cn

[U29] Py：属性校验
来源：http://hf.lnxyls.cn

@property 与 @x.setter 配合
来源：http://lw.chemitech.net.cn

[U30] Py：数据类
来源：http://zk.hnjuh.cn

@dataclass(slots=True)
来源：http://gw.huixinmuqiang.cn

[U31] Py：单测
来源：http://wm.lnxyls.cn

python -m pytest -q
来源：http://ie.szsharing.cn

[U32] Py：代码格式化
来源：http://uq.hahajie.cn

ruff format . && ruff check --fix .
来源：http://ga.hnjuh.cn

[U33] Py：打包发布
来源：http://em.gzmigu.cn

python -m build  （依赖 pyproject.toml）
来源：http://kh.nszjky.cn

[U34] Py：判断编码
来源：http://ji.shxzskj.cn

chardet.detect(raw)
来源：http://gy.shxzskj.cn

[U35] Py：发送邮件
来源：http://sd.yuntaijiaju.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://xk.asd995.cn

[U36] Py：定时任务
来源：http://ow.shxzskj.cn

schedule.every(10).minutes.do(job)
来源：http://su.huixinmuqiang.cn

[U37] Py：读写 Excel
来源：http://qi.newstarts.cn

pandas.read_excel / DataFrame.to_excel
来源：http://qs.hahajie.cn

[U38] Py：获取脚本所在目录
来源：http://fo.shtwfgs.cn

Path(__file__).resolve().parent
来源：http://pf.wgjwhj.cn

[U39] Py：判断是否在交互环境
来源：http://cn.newstarts.cn

sys.stdout.isatty()
来源：http://sm.yuntaijiaju.cn

[U40] Py：打印到标准错误
来源：http://lc.yuntaijiaju.cn

print("err", file=sys.stderr)
来源：http://xd.9csxet.cn

[U41] PHP：初始化 Composer 项目
来源：http://ey.asd995.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://le.lnxyls.cn

[U42] PHP：PSR-4 自动加载
来源：http://ff.panjiajie.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://jq.9csxet.cn

[U43] PHP：声明命名空间
来源：http://qz.muxihuayi.cn

namespace App\Http;
来源：http://pg.chemitech.net.cn

[U44] PHP：开启严格类型
来源：http://bs.huixiangedu.cn

declare(strict_types=1);
来源：http://ld.colortex.cn

[U45] PHP：类型声明与返回类型
来源：http://wg.szxytkj.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://zi.huixiangedu.cn

[U46] PHP：可空类型
来源：http://uz.9csxet.cn

?string $name = null
来源：http://iy.jctech888.com.cn

[U47] PHP：联合类型
来源：http://jy.hahajie.cn

int|string $id
来源：http://bw.muxihuayi.cn

[U48] PHP：纯枚举
来源：http://qm.bjjhwx.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://br.newstarts.cn


<!-- 参考信息 -->