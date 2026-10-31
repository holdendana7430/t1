代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://qa.huixiangedu.cn

[S25] C：内存拷贝
来源：http://el.colortex.cn

memcpy(dst, src, n);
来源：http://hy.newstarts.cn

[S26] C：内存清零
来源：http://mj.muxihuayi.cn

memset(a, 0, sizeof a);
来源：http://wx.hnjuh.cn

[S27] C：定义常量
来源：http://dv.hahajie.cn

const double PI = 3.14159;
来源：http://eg.nicolike.cn

[S28] C：静态变量
来源：http://zb.szxytkj.cn

static int counter = 0;
来源：http://ic.huixiangedu.cn

[S29] C：变参函数
来源：http://mn.bjjhwx.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ib.nicolike.cn

[S30] C：头文件保护
来源：http://ht.yuntaijiaju.cn

#ifndef X_H
来源：http://wb.nszjky.cn

#define X_H
来源：http://pm.szxytkj.cn

#endif
来源：http://wq.lnxyls.cn

[S31] C++：Hello World
来源：http://ex.huixinmuqiang.cn

#include <iostream>
来源：http://fa.gzmigu.cn

int main() { std::cout << "Hello\n"; }
来源：http://tj.huixiangedu.cn

[S32] C++：字符串
来源：http://yt.yuexingan06.cn

std::string s = "hi";  s += "!";
来源：http://vh.huixinmuqiang.cn

[S33] C++：vector 增删
来源：http://ut.newstarts.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://cy.9csxet.cn

[S34] C++：遍历 vector
来源：http://ug.lnxyls.cn

for (auto &x : v) { std::cout << x; }
来源：http://fu.panjiajie.cn

[S35] C++：map
来源：http://no.shxzukj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://qj.colortex.cn

[S36] C++：unordered_map
来源：http://dn.yuexingan06.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://gc.nszjky.cn

[S37] C++：set
来源：http://nu.haigaiapp.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://um.shxzukj.cn

[S38] C++：排序
来源：http://zq.shxzskj.cn

std::sort(v.begin(), v.end());
来源：http://sa.521024.cn

[S39] C++：自定义比较器排序
来源：http://pp.shxzukj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://eu.nicolike.cn

[S40] C++：查找元素
来源：http://df.szsharing.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://og.nicolike.cn

[S41] C++：类与构造函数
来源：http://uz.haigaiapp.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ia.gzmigu.cn

[S42] C++：继承与虚函数
来源：http://mk.colortex.cn

class B : public Base { public: void f() override {} };
来源：http://bp.jianghongdianzi.cn

[S43] C++：智能指针
来源：http://uu.shxzskj.cn

auto p = std::make_unique<int>(5);
来源：http://lf.huixiangedu.cn

[S44] C++：引用传参
来源：http://nh.shtwfgs.cn

void inc(int &x) { ++x; }
来源：http://wm.muxihuayi.cn

[S45] C++：lambda
来源：http://wh.jctech888.com.cn

auto add = [](int a, int b) { return a + b; };
来源：http://qx.nicolike.cn

[S46] C++：函数模板
来源：http://vx.shxzskj.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://lu.shtwfgs.cn

[S47] C++：结构化绑定遍历
来源：http://wt.panjiajie.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hf.shxzukj.cn

[S48] C++：逐行读文件
来源：http://qj.yuntaijiaju.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ff.nicolike.cn

while (std::getline(in, line)) { }
来源：http://zq.9csxet.cn

[S49] C++：写文件
来源：http://yx.shxzskj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://xs.huixiangedu.cn

[S50] C++：格式化数字
来源：http://vx.szsharing.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://rl.asd995.cn

[S51] C++：显式类型转换
来源：http://fv.szsharing.cn

static_cast<double>(a) / b
来源：http://lx.nicolike.cn

[S52] C++：const 与 noexcept
来源：http://yu.hnjuh.cn

int size() const noexcept { return n_; }
来源：http://so.gzmigu.cn

[S53] C++：移动语义
来源：http://yk.panjiajie.cn

std::vector<int> w = std::move(v);
来源：http://jw.lnxyls.cn

[S54] C++：异常处理
来源：http://kl.szxytkj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://av.gzmigu.cn

[S55] C++：结构化绑定
来源：http://to.9csxet.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://jq.shxzskj.cn

[S56] C++：optional
来源：http://re.szxytkj.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://yj.shtwfgs.cn

[S57] C++：编译期常量
来源：http://ld.shxzukj.cn

constexpr int N = 10;
来源：http://nu.bjjhwx.cn

[S58] C++：命名空间
来源：http://kz.bookmarksfly.cn

namespace ns { int f() { return 1; } }
来源：http://jg.huixiangedu.cn

[S59] C++：静态断言
来源：http://cl.jctech888.com.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ne.shxzukj.cn

[S60] C++：遍历并删除元素
来源：http://rq.nicolike.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ik.muxihuayi.cn

================================================================================
来源：http://po.szxytkj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://fr.asd995.cn

================================================================================
来源：http://oh.huixiangedu.cn

[T01] Kotlin：Hello World
来源：http://hz.nicolike.cn

println("Hello")
来源：http://fw.wgjwhj.cn

[T02] Kotlin：变量
来源：http://ye.wgjwhj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ap.nszjky.cn

[T03] Kotlin：字符串模板
来源：http://wf.panjiajie.cn

"值: $b"
来源：http://hy.jctech888.com.cn

[T04] Kotlin：空安全
来源：http://lu.wgjwhj.cn

val n: String? = null;  n?.length
来源：http://tw.asd995.cn

[T05] Kotlin：when 表达式
来源：http://bj.haigaiapp.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ui.521024.cn

[T06] Kotlin：集合映射
来源：http://xg.newstarts.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://px.nicolike.cn

[T07] Kotlin：集合过滤
来源：http://ut.nicolike.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://jp.yuexingan06.cn

[T08] Kotlin：数据类
来源：http://tn.wgjwhj.cn

data class User(val name: String, val age: Int)
来源：http://mw.shtwfgs.cn

[T09] Kotlin：扩展函数
来源：http://lg.bjjhwx.cn

fun String.exclaim() = this + "!"
来源：http://pa.huanxung.cn

[T10] Kotlin：默认参数
来源：http://th.9csxet.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://pr.panjiajie.cn

[T11] Kotlin：协程
来源：http://kz.bjjhwx.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://bg.szsharing.cn

[T12] Kotlin：解构声明
来源：http://ap.shtwfgs.cn

val (a, b) = Pair(1, 2)
来源：http://ge.panjiajie.cn

[T13] Kotlin：只读 Map
来源：http://yi.hnjuh.cn

val m = mapOf("a" to 1)
来源：http://dj.shtwfgs.cn

[T14] Kotlin：循环
来源：http://lm.yuexingan06.cn

for (i in 1..10) println(i)
来源：http://tt.shxzukj.cn

[T15] Kotlin：接口
来源：http://bz.bookmarksfly.cn

interface Shape { fun area(): Double }
来源：http://uk.asd995.cn

[T16] Swift：Hello World
来源：http://lt.shtwfgs.cn

print("Hello")
来源：http://yi.asd995.cn

[T17] Swift：变量与常量
来源：http://rz.colortex.cn

var a = 1;  let b = 2
来源：http://mt.gzmigu.cn

[T18] Swift：字符串插值
来源：http://pl.nszjky.cn

"值: \(b)"
来源：http://px.colortex.cn

[T19] Swift：可选绑定
来源：http://dc.hnjuh.cn

if let n = opt { print(n) }
来源：http://dl.wgjwhj.cn

[T20] Swift：数组操作
来源：http://pp.jianghongdianzi.cn

var a = [1, 2, 3];  a.append(4)
来源：http://gy.asd995.cn

[T21] Swift：遍历
来源：http://yb.lnxyls.cn

for x in a { print(x) }
来源：http://is.9csxet.cn

[T22] Swift：字典
来源：http://hq.szxytkj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ou.shxzukj.cn

[T23] Swift：函数
来源：http://rm.gzmigu.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://cv.nicolike.cn

[T24] Swift：闭包
来源：http://kl.muxihuayi.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://hu.hnjuh.cn

[T25] Swift：结构体
来源：http://np.nicolike.cn

struct P { var x: Int }
来源：http://qc.bjjhwx.cn

[T26] Swift：类与重写
来源：http://sg.colortex.cn

class A: Base { override func f() {} }
来源：http://fy.szxytkj.cn

[T27] Swift：错误处理
来源：http://sq.nicolike.cn

do { try f() } catch { print(error) }
来源：http://th.chemitech.net.cn

[T28] Swift：枚举
来源：http://uj.huixiangedu.cn

enum Color { case red, green }
来源：http://lg.bookmarksfly.cn

[T29] Swift：guard 提前返回
来源：http://mm.asd995.cn

guard let x = opt else { return }
来源：http://qt.bjjhwx.cn

[T30] Swift：协议
来源：http://ey.szxytkj.cn

protocol Shape { func area() -> Double }
来源：http://ya.lnxyls.cn

[T31] Lua：Hello World
来源：http://wd.gzmigu.cn

print("Hello")
来源：http://si.shtwfgs.cn

[T32] Lua：局部变量
来源：http://vw.szsharing.cn

local a = 1
来源：http://ws.chemitech.net.cn

[T33] Lua：表（数组）
来源：http://zt.chemitech.net.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://vq.521024.cn

[T34] Lua：遍历表
来源：http://bn.521024.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ba.huanxung.cn

[T35] Lua：字典表
来源：http://ub.gzmigu.cn

local d = { a = 1 };  d.b = 2
来源：http://kl.haigaiapp.cn

[T36] Lua：函数
来源：http://hm.shtwfgs.cn

function add(a, b) return a + b end
来源：http://as.nicolike.cn

[T37] Lua：字符串拼接
来源：http://cn.yuntaijiaju.cn

"a" .. "b"
来源：http://mm.asd995.cn

[T38] Lua：条件
来源：http://fp.shxzskj.cn

if x > 0 then print("正") end
来源：http://wr.wgjwhj.cn

[T39] Lua：模式匹配
来源：http://wf.gzmigu.cn

string.find(s, "%d+")
来源：http://ly.lnxyls.cn

[T40] Lua：元表
来源：http://fe.huixiangedu.cn

setmetatable({}, { __index = base })
来源：http://qm.huixiangedu.cn

[T41] Perl：Hello World
来源：http://nw.hahajie.cn

print "Hello\n";
来源：http://gc.huixiangedu.cn

[T42] Perl：变量类型
来源：http://dd.yuexingan06.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mu.lnxyls.cn

[T43] Perl：字符串插值
来源：http://gh.lnxyls.cn

"值: $a"
来源：http://qt.asd995.cn

[T44] Perl：条件
来源：http://ei.bjjhwx.cn

if ($a > 0) { print "正"; }
来源：http://yt.szsharing.cn

[T45] Perl：数组遍历
来源：http://nj.huanxung.cn

for my $x (@arr) { print $x; }
来源：http://mw.nicolike.cn

[T46] Perl：哈希操作
来源：http://es.newstarts.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://bx.szxytkj.cn

[T47] Perl：正则捕获
来源：http://bm.shtwfgs.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://zi.gzmigu.cn

[T48] Perl：正则替换
来源：http://op.huixinmuqiang.cn

$s =~ s/old/new/g;
来源：http://lx.muxihuayi.cn

[T49] Perl：函数
来源：http://fe.hnjuh.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mm.9csxet.cn

[T50] Perl：逐行读文件
来源：http://uo.szsharing.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://pp.bookmarksfly.cn

while (my $line = <$fh>) { print $line; }
来源：http://bs.colortex.cn

[T51] Scala：Hello World
来源：http://gi.wgjwhj.cn

println("Hello")
来源：http://gh.colortex.cn

[T52] Scala：变量
来源：http://mt.521024.cn

val a = 1;  var b = 2
来源：http://pk.hnjuh.cn

[T53] Scala：字符串插值
来源：http://oj.szsharing.cn

s"值: $b"
来源：http://mo.huanxung.cn

[T54] Scala：集合映射
来源：http://bl.shtwfgs.cn

List(1, 2, 3).map(_ * 2)
来源：http://by.shxzskj.cn

[T55] Scala：集合过滤
来源：http://zu.nicolike.cn

List(1, 2, 3).filter(_ > 1)
来源：http://oa.colortex.cn

[T56] Scala：样例类
来源：http://nj.jianghongdianzi.cn

case class User(name: String, age: Int)
来源：http://wb.shtwfgs.cn

[T57] Scala：模式匹配
来源：http://qe.jianghongdianzi.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://er.hahajie.cn

[T58] Scala：函数定义
来源：http://ep.lnxyls.cn

def add(a: Int, b: Int): Int = a + b
来源：http://pe.huanxung.cn

[T59] Scala：循环
来源：http://tv.9csxet.cn

for (i <- 1 to 10) println(i)
来源：http://uv.jianghongdianzi.cn

[T60] Scala：折叠
来源：http://fd.jctech888.com.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://rc.shxzskj.cn

================================================================================
来源：http://tz.shxzskj.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ch.nszjky.cn

================================================================================
来源：http://lj.shxzukj.cn

[U01] Py：创建虚拟环境
来源：http://mu.wgjwhj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://hg.huixinmuqiang.cn

[U02] Py：导出 / 安装依赖
来源：http://fz.wgjwhj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ro.521024.cn

[U03] Py：加载 .env 配置
来源：http://ea.szsharing.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://eb.newstarts.cn

[U04] Py：变量调试打印
来源：http://xy.muxihuayi.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://kd.nszjky.cn

[U05] Py：列表去重且保序
来源：http://vd.bjjhwx.cn

list(dict.fromkeys(arr))
来源：http://jq.szsharing.cn

[U06] Py：合并两个字典
来源：http://eb.nszjky.cn

{**a, **b}
来源：http://pc.colortex.cn

[U07] Py：反转字典键值
来源：http://er.colortex.cn

{v: k for k, v in d.items()}
来源：http://mg.lnxyls.cn

[U08] Py：展平二维列表
来源：http://ai.muxihuayi.cn

[y for x in nested for y in x]
来源：http://hq.bjjhwx.cn

[U09] Py：字典取最大值的键
来源：http://fn.jianghongdianzi.cn

max(d, key=d.get)
来源：http://dt.hahajie.cn

[U10] Py：按值排序字典
来源：http://bk.shtwfgs.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ca.szsharing.cn

[U11] Py：生成器表达式
来源：http://yt.jianghongdianzi.cn

(x * 2 for x in arr)
来源：http://ws.asd995.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ui.muxihuayi.cn

Counter(arr).most_common(3)
来源：http://qx.szsharing.cn

[U13] Py：固定长度队列
来源：http://br.yuntaijiaju.cn

deque(maxlen=10)
来源：http://wd.muxihuayi.cn

[U14] Py：分组收集到列表
来源：http://ze.colortex.cn

defaultdict(list)
来源：http://fv.chemitech.net.cn

[U15] Py：高精度计时
来源：http://bo.colortex.cn

t = time.perf_counter()
来源：http://im.szxytkj.cn

[U16] Py：命令行参数解析
来源：http://gt.haigaiapp.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://yf.panjiajie.cn

[U17] Py：初始化日志
来源：http://vx.panjiajie.cn

logging.basicConfig(level=logging.INFO)
来源：http://rc.huanxung.cn

[U18] Py：预编译正则
来源：http://hz.muxihuayi.cn

pat = re.compile(r"\d+")
来源：http://eu.yuntaijiaju.cn

[U19] Py：正则替换带回调
来源：http://bc.panjiajie.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://na.nszjky.cn

[U20] Py：缓存函数结果
来源：http://jg.9csxet.cn

@functools.lru_cache(maxsize=None)
来源：http://cn.jianghongdianzi.cn

[U21] Py：自定义上下文管理器
来源：http://fg.hnjuh.cn

@contextlib.contextmanager
来源：http://bq.yuntaijiaju.cn

[U22] Py：矩阵转置
来源：http://hq.nszjky.cn

list(zip(*m))
来源：http://yd.newstarts.cn

[U23] Py：分块读取大文件
来源：http://zl.yuntaijiaju.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://qf.huixiangedu.cn

[U24] Py：路径操作
来源：http://id.521024.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://th.haigaiapp.cn

[U25] Py：CSV 按字典读
来源：http://aw.huanxung.cn

csv.DictReader(f)
来源：http://nr.shtwfgs.cn

[U26] Py：并发下载
来源：http://po.lnxyls.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://er.bjjhwx.cn

[U27] Py：异步 HTTP
来源：http://tw.huixiangedu.cn

aiohttp.ClientSession() 配合 async with
来源：http://yv.huanxung.cn

[U28] Py：类型别名
来源：http://vp.huixiangedu.cn

UserId = int
来源：http://ag.yuexingan06.cn

[U29] Py：属性校验
来源：http://fh.gzmigu.cn

@property 与 @x.setter 配合
来源：http://gw.9csxet.cn

[U30] Py：数据类
来源：http://sh.bookmarksfly.cn

@dataclass(slots=True)
来源：http://cd.chemitech.net.cn

[U31] Py：单测
来源：http://un.nszjky.cn

python -m pytest -q
来源：http://yh.asd995.cn

[U32] Py：代码格式化
来源：http://fo.szsharing.cn

ruff format . && ruff check --fix .
来源：http://it.szxytkj.cn

[U33] Py：打包发布
来源：http://yq.521024.cn

python -m build  （依赖 pyproject.toml）
来源：http://di.yuntaijiaju.cn

[U34] Py：判断编码
来源：http://jr.yuntaijiaju.cn

chardet.detect(raw)
来源：http://iy.bjjhwx.cn

[U35] Py：发送邮件
来源：http://oi.shtwfgs.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://cy.huixinmuqiang.cn

[U36] Py：定时任务
来源：http://gr.hahajie.cn

schedule.every(10).minutes.do(job)
来源：http://ut.shxzskj.cn

[U37] Py：读写 Excel
来源：http://tq.chemitech.net.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ce.asd995.cn

[U38] Py：获取脚本所在目录
来源：http://lt.muxihuayi.cn

Path(__file__).resolve().parent
来源：http://up.521024.cn

[U39] Py：判断是否在交互环境
来源：http://jv.hahajie.cn

sys.stdout.isatty()
来源：http://tk.huixiangedu.cn

[U40] Py：打印到标准错误
来源：http://np.shtwfgs.cn

print("err", file=sys.stderr)
来源：http://qd.hnjuh.cn

[U41] PHP：初始化 Composer 项目
来源：http://db.shxzukj.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://xy.huixinmuqiang.cn

[U42] PHP：PSR-4 自动加载
来源：http://ce.huixinmuqiang.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ip.panjiajie.cn

[U43] PHP：声明命名空间
来源：http://jq.hahajie.cn

namespace App\Http;
来源：http://jv.asd995.cn

[U44] PHP：开启严格类型
来源：http://tj.huanxung.cn

declare(strict_types=1);
来源：http://vm.nicolike.cn

[U45] PHP：类型声明与返回类型
来源：http://lc.gzmigu.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://fg.haigaiapp.cn

[U46] PHP：可空类型
来源：http://bc.yuntaijiaju.cn

?string $name = null
来源：http://hr.hnjuh.cn

[U47] PHP：联合类型
来源：http://mz.huixiangedu.cn

int|string $id
来源：http://ya.chemitech.net.cn

[U48] PHP：纯枚举
来源：http://tc.gzmigu.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://nu.521024.cn


<!-- 参考信息 -->