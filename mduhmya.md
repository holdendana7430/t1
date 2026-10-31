代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://cs.521024.cn

[S25] C：内存拷贝
来源：http://nl.hahajie.cn

memcpy(dst, src, n);
来源：http://ym.chemitech.net.cn

[S26] C：内存清零
来源：http://vh.chemitech.net.cn

memset(a, 0, sizeof a);
来源：http://ff.wgjwhj.cn

[S27] C：定义常量
来源：http://tk.muxihuayi.cn

const double PI = 3.14159;
来源：http://xn.shtwfgs.cn

[S28] C：静态变量
来源：http://qq.asd995.cn

static int counter = 0;
来源：http://mq.jianghongdianzi.cn

[S29] C：变参函数
来源：http://pa.jctech888.com.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://lx.chemitech.net.cn

[S30] C：头文件保护
来源：http://zt.shxzskj.cn

#ifndef X_H
来源：http://xc.wgjwhj.cn

#define X_H
来源：http://by.chemitech.net.cn

#endif
来源：http://ha.newstarts.cn

[S31] C++：Hello World
来源：http://dt.huixiangedu.cn

#include <iostream>
来源：http://id.bjjhwx.cn

int main() { std::cout << "Hello\n"; }
来源：http://yl.panjiajie.cn

[S32] C++：字符串
来源：http://pv.521024.cn

std::string s = "hi";  s += "!";
来源：http://nz.yuntaijiaju.cn

[S33] C++：vector 增删
来源：http://gp.asd995.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qa.bookmarksfly.cn

[S34] C++：遍历 vector
来源：http://ir.panjiajie.cn

for (auto &x : v) { std::cout << x; }
来源：http://tu.haigaiapp.cn

[S35] C++：map
来源：http://si.nicolike.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://xd.hahajie.cn

[S36] C++：unordered_map
来源：http://ci.huixinmuqiang.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://mz.szsharing.cn

[S37] C++：set
来源：http://tz.shtwfgs.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://pg.szsharing.cn

[S38] C++：排序
来源：http://cz.haigaiapp.cn

std::sort(v.begin(), v.end());
来源：http://zl.wgjwhj.cn

[S39] C++：自定义比较器排序
来源：http://lo.asd995.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://kl.jctech888.com.cn

[S40] C++：查找元素
来源：http://ro.chemitech.net.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://bm.hahajie.cn

[S41] C++：类与构造函数
来源：http://aw.szxytkj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://jc.yuntaijiaju.cn

[S42] C++：继承与虚函数
来源：http://im.muxihuayi.cn

class B : public Base { public: void f() override {} };
来源：http://sq.nicolike.cn

[S43] C++：智能指针
来源：http://ds.jctech888.com.cn

auto p = std::make_unique<int>(5);
来源：http://qn.panjiajie.cn

[S44] C++：引用传参
来源：http://ks.nicolike.cn

void inc(int &x) { ++x; }
来源：http://yl.bjjhwx.cn

[S45] C++：lambda
来源：http://fs.newstarts.cn

auto add = [](int a, int b) { return a + b; };
来源：http://yl.bjjhwx.cn

[S46] C++：函数模板
来源：http://je.hahajie.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hu.huanxung.cn

[S47] C++：结构化绑定遍历
来源：http://aa.bjjhwx.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ae.shxzskj.cn

[S48] C++：逐行读文件
来源：http://kq.nicolike.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ak.jctech888.com.cn

while (std::getline(in, line)) { }
来源：http://mb.huixinmuqiang.cn

[S49] C++：写文件
来源：http://ws.hahajie.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hi.szxytkj.cn

[S50] C++：格式化数字
来源：http://cb.colortex.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://dq.521024.cn

[S51] C++：显式类型转换
来源：http://ge.nicolike.cn

static_cast<double>(a) / b
来源：http://tl.lnxyls.cn

[S52] C++：const 与 noexcept
来源：http://yu.newstarts.cn

int size() const noexcept { return n_; }
来源：http://dv.huixiangedu.cn

[S53] C++：移动语义
来源：http://ui.nicolike.cn

std::vector<int> w = std::move(v);
来源：http://ph.521024.cn

[S54] C++：异常处理
来源：http://in.panjiajie.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://rp.hnjuh.cn

[S55] C++：结构化绑定
来源：http://kl.hnjuh.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ia.asd995.cn

[S56] C++：optional
来源：http://fi.9csxet.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://zy.asd995.cn

[S57] C++：编译期常量
来源：http://hs.wgjwhj.cn

constexpr int N = 10;
来源：http://ho.szxytkj.cn

[S58] C++：命名空间
来源：http://xc.wgjwhj.cn

namespace ns { int f() { return 1; } }
来源：http://yw.panjiajie.cn

[S59] C++：静态断言
来源：http://gn.asd995.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://yz.asd995.cn

[S60] C++：遍历并删除元素
来源：http://lq.yuexingan06.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://jk.huixinmuqiang.cn

================================================================================
来源：http://xe.shxzukj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://yf.szxytkj.cn

================================================================================
来源：http://xx.bookmarksfly.cn

[T01] Kotlin：Hello World
来源：http://dm.szxytkj.cn

println("Hello")
来源：http://fq.bjjhwx.cn

[T02] Kotlin：变量
来源：http://eh.panjiajie.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://qk.nszjky.cn

[T03] Kotlin：字符串模板
来源：http://pb.hnjuh.cn

"值: $b"
来源：http://gq.shtwfgs.cn

[T04] Kotlin：空安全
来源：http://rq.jianghongdianzi.cn

val n: String? = null;  n?.length
来源：http://yw.bookmarksfly.cn

[T05] Kotlin：when 表达式
来源：http://kd.newstarts.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ra.panjiajie.cn

[T06] Kotlin：集合映射
来源：http://dh.nszjky.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://sc.shtwfgs.cn

[T07] Kotlin：集合过滤
来源：http://hr.huixiangedu.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ms.shtwfgs.cn

[T08] Kotlin：数据类
来源：http://hv.yuntaijiaju.cn

data class User(val name: String, val age: Int)
来源：http://ji.newstarts.cn

[T09] Kotlin：扩展函数
来源：http://ca.shxzukj.cn

fun String.exclaim() = this + "!"
来源：http://lo.nicolike.cn

[T10] Kotlin：默认参数
来源：http://il.jctech888.com.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ve.jianghongdianzi.cn

[T11] Kotlin：协程
来源：http://yx.hnjuh.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://lt.bjjhwx.cn

[T12] Kotlin：解构声明
来源：http://wd.muxihuayi.cn

val (a, b) = Pair(1, 2)
来源：http://za.huanxung.cn

[T13] Kotlin：只读 Map
来源：http://ih.nszjky.cn

val m = mapOf("a" to 1)
来源：http://gq.haigaiapp.cn

[T14] Kotlin：循环
来源：http://nu.bookmarksfly.cn

for (i in 1..10) println(i)
来源：http://vh.shxzskj.cn

[T15] Kotlin：接口
来源：http://wz.jianghongdianzi.cn

interface Shape { fun area(): Double }
来源：http://mh.jctech888.com.cn

[T16] Swift：Hello World
来源：http://pj.yuntaijiaju.cn

print("Hello")
来源：http://gi.521024.cn

[T17] Swift：变量与常量
来源：http://hu.huixiangedu.cn

var a = 1;  let b = 2
来源：http://ql.chemitech.net.cn

[T18] Swift：字符串插值
来源：http://tn.bookmarksfly.cn

"值: \(b)"
来源：http://on.nszjky.cn

[T19] Swift：可选绑定
来源：http://gz.huanxung.cn

if let n = opt { print(n) }
来源：http://bc.huanxung.cn

[T20] Swift：数组操作
来源：http://ny.huixiangedu.cn

var a = [1, 2, 3];  a.append(4)
来源：http://dp.huixiangedu.cn

[T21] Swift：遍历
来源：http://jm.bjjhwx.cn

for x in a { print(x) }
来源：http://qf.yuexingan06.cn

[T22] Swift：字典
来源：http://zv.bookmarksfly.cn

var d = ["a": 1];  d["b"] = 2
来源：http://py.jctech888.com.cn

[T23] Swift：函数
来源：http://um.newstarts.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ty.yuntaijiaju.cn

[T24] Swift：闭包
来源：http://rv.bookmarksfly.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://nk.huixinmuqiang.cn

[T25] Swift：结构体
来源：http://la.9csxet.cn

struct P { var x: Int }
来源：http://jc.huanxung.cn

[T26] Swift：类与重写
来源：http://fi.szsharing.cn

class A: Base { override func f() {} }
来源：http://kn.lnxyls.cn

[T27] Swift：错误处理
来源：http://ym.muxihuayi.cn

do { try f() } catch { print(error) }
来源：http://uj.huanxung.cn

[T28] Swift：枚举
来源：http://jw.gzmigu.cn

enum Color { case red, green }
来源：http://ot.hahajie.cn

[T29] Swift：guard 提前返回
来源：http://ip.huixinmuqiang.cn

guard let x = opt else { return }
来源：http://vc.asd995.cn

[T30] Swift：协议
来源：http://cv.yuexingan06.cn

protocol Shape { func area() -> Double }
来源：http://ou.hnjuh.cn

[T31] Lua：Hello World
来源：http://up.huixinmuqiang.cn

print("Hello")
来源：http://bj.hahajie.cn

[T32] Lua：局部变量
来源：http://yy.szxytkj.cn

local a = 1
来源：http://gc.9csxet.cn

[T33] Lua：表（数组）
来源：http://jo.panjiajie.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://kf.huanxung.cn

[T34] Lua：遍历表
来源：http://cj.nicolike.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://zp.lnxyls.cn

[T35] Lua：字典表
来源：http://vv.bookmarksfly.cn

local d = { a = 1 };  d.b = 2
来源：http://lp.colortex.cn

[T36] Lua：函数
来源：http://ye.nicolike.cn

function add(a, b) return a + b end
来源：http://wi.9csxet.cn

[T37] Lua：字符串拼接
来源：http://nq.9csxet.cn

"a" .. "b"
来源：http://eo.szsharing.cn

[T38] Lua：条件
来源：http://hn.9csxet.cn

if x > 0 then print("正") end
来源：http://ns.colortex.cn

[T39] Lua：模式匹配
来源：http://kd.jianghongdianzi.cn

string.find(s, "%d+")
来源：http://zj.lnxyls.cn

[T40] Lua：元表
来源：http://yo.asd995.cn

setmetatable({}, { __index = base })
来源：http://ue.panjiajie.cn

[T41] Perl：Hello World
来源：http://bc.szsharing.cn

print "Hello\n";
来源：http://uw.shxzukj.cn

[T42] Perl：变量类型
来源：http://jo.yuexingan06.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://qe.panjiajie.cn

[T43] Perl：字符串插值
来源：http://ga.nicolike.cn

"值: $a"
来源：http://hx.muxihuayi.cn

[T44] Perl：条件
来源：http://rb.szxytkj.cn

if ($a > 0) { print "正"; }
来源：http://tj.nszjky.cn

[T45] Perl：数组遍历
来源：http://sr.yuntaijiaju.cn

for my $x (@arr) { print $x; }
来源：http://ga.shtwfgs.cn

[T46] Perl：哈希操作
来源：http://fj.muxihuayi.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://tj.nicolike.cn

[T47] Perl：正则捕获
来源：http://li.9csxet.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://hs.9csxet.cn

[T48] Perl：正则替换
来源：http://lr.wgjwhj.cn

$s =~ s/old/new/g;
来源：http://rn.shtwfgs.cn

[T49] Perl：函数
来源：http://xd.asd995.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://xc.bookmarksfly.cn

[T50] Perl：逐行读文件
来源：http://sz.szxytkj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://oj.hnjuh.cn

while (my $line = <$fh>) { print $line; }
来源：http://vd.jctech888.com.cn

[T51] Scala：Hello World
来源：http://dr.jctech888.com.cn

println("Hello")
来源：http://vw.shtwfgs.cn

[T52] Scala：变量
来源：http://xi.colortex.cn

val a = 1;  var b = 2
来源：http://qc.nicolike.cn

[T53] Scala：字符串插值
来源：http://sc.chemitech.net.cn

s"值: $b"
来源：http://wq.muxihuayi.cn

[T54] Scala：集合映射
来源：http://qk.bjjhwx.cn

List(1, 2, 3).map(_ * 2)
来源：http://vr.hnjuh.cn

[T55] Scala：集合过滤
来源：http://zr.shxzukj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://iw.jianghongdianzi.cn

[T56] Scala：样例类
来源：http://hs.asd995.cn

case class User(name: String, age: Int)
来源：http://fo.521024.cn

[T57] Scala：模式匹配
来源：http://oz.hahajie.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://sp.gzmigu.cn

[T58] Scala：函数定义
来源：http://rp.521024.cn

def add(a: Int, b: Int): Int = a + b
来源：http://wp.muxihuayi.cn

[T59] Scala：循环
来源：http://re.9csxet.cn

for (i <- 1 to 10) println(i)
来源：http://bl.chemitech.net.cn

[T60] Scala：折叠
来源：http://xs.hahajie.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://uv.chemitech.net.cn

================================================================================
来源：http://yo.nicolike.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://sf.gzmigu.cn

================================================================================
来源：http://tt.gzmigu.cn

[U01] Py：创建虚拟环境
来源：http://tu.shxzukj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://rq.huixinmuqiang.cn

[U02] Py：导出 / 安装依赖
来源：http://yv.hnjuh.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://qi.chemitech.net.cn

[U03] Py：加载 .env 配置
来源：http://en.panjiajie.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://vd.chemitech.net.cn

[U04] Py：变量调试打印
来源：http://kr.szsharing.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://nf.jctech888.com.cn

[U05] Py：列表去重且保序
来源：http://rp.jctech888.com.cn

list(dict.fromkeys(arr))
来源：http://rc.yuntaijiaju.cn

[U06] Py：合并两个字典
来源：http://ok.wgjwhj.cn

{**a, **b}
来源：http://wd.huanxung.cn

[U07] Py：反转字典键值
来源：http://uh.hahajie.cn

{v: k for k, v in d.items()}
来源：http://hc.hahajie.cn

[U08] Py：展平二维列表
来源：http://ex.szxytkj.cn

[y for x in nested for y in x]
来源：http://ej.colortex.cn

[U09] Py：字典取最大值的键
来源：http://fd.lnxyls.cn

max(d, key=d.get)
来源：http://hk.asd995.cn

[U10] Py：按值排序字典
来源：http://vm.jctech888.com.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://rb.hahajie.cn

[U11] Py：生成器表达式
来源：http://kh.yuexingan06.cn

(x * 2 for x in arr)
来源：http://gr.shxzukj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://dr.haigaiapp.cn

Counter(arr).most_common(3)
来源：http://zy.wgjwhj.cn

[U13] Py：固定长度队列
来源：http://fc.lnxyls.cn

deque(maxlen=10)
来源：http://er.jianghongdianzi.cn

[U14] Py：分组收集到列表
来源：http://ot.yuexingan06.cn

defaultdict(list)
来源：http://xw.shxzukj.cn

[U15] Py：高精度计时
来源：http://lf.shtwfgs.cn

t = time.perf_counter()
来源：http://qa.hnjuh.cn

[U16] Py：命令行参数解析
来源：http://uf.haigaiapp.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ak.huixinmuqiang.cn

[U17] Py：初始化日志
来源：http://gc.huixiangedu.cn

logging.basicConfig(level=logging.INFO)
来源：http://ot.muxihuayi.cn

[U18] Py：预编译正则
来源：http://fn.newstarts.cn

pat = re.compile(r"\d+")
来源：http://sx.huixinmuqiang.cn

[U19] Py：正则替换带回调
来源：http://kg.szsharing.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://bz.9csxet.cn

[U20] Py：缓存函数结果
来源：http://ve.nicolike.cn

@functools.lru_cache(maxsize=None)
来源：http://ha.nszjky.cn

[U21] Py：自定义上下文管理器
来源：http://lc.shtwfgs.cn

@contextlib.contextmanager
来源：http://nf.nicolike.cn

[U22] Py：矩阵转置
来源：http://cw.wgjwhj.cn

list(zip(*m))
来源：http://su.asd995.cn

[U23] Py：分块读取大文件
来源：http://is.chemitech.net.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://di.bookmarksfly.cn

[U24] Py：路径操作
来源：http://ck.hahajie.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://qe.chemitech.net.cn

[U25] Py：CSV 按字典读
来源：http://ih.asd995.cn

csv.DictReader(f)
来源：http://si.gzmigu.cn

[U26] Py：并发下载
来源：http://te.bjjhwx.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://gt.newstarts.cn

[U27] Py：异步 HTTP
来源：http://ql.521024.cn

aiohttp.ClientSession() 配合 async with
来源：http://zt.yuntaijiaju.cn

[U28] Py：类型别名
来源：http://hu.shtwfgs.cn

UserId = int
来源：http://vl.muxihuayi.cn

[U29] Py：属性校验
来源：http://ex.bookmarksfly.cn

@property 与 @x.setter 配合
来源：http://yc.haigaiapp.cn

[U30] Py：数据类
来源：http://yd.9csxet.cn

@dataclass(slots=True)
来源：http://iu.bjjhwx.cn

[U31] Py：单测
来源：http://bw.chemitech.net.cn

python -m pytest -q
来源：http://ct.chemitech.net.cn

[U32] Py：代码格式化
来源：http://hd.chemitech.net.cn

ruff format . && ruff check --fix .
来源：http://dy.newstarts.cn

[U33] Py：打包发布
来源：http://vs.huixiangedu.cn

python -m build  （依赖 pyproject.toml）
来源：http://nn.chemitech.net.cn

[U34] Py：判断编码
来源：http://lv.lnxyls.cn

chardet.detect(raw)
来源：http://cz.muxihuayi.cn

[U35] Py：发送邮件
来源：http://og.szsharing.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://fe.hnjuh.cn

[U36] Py：定时任务
来源：http://tn.shxzukj.cn

schedule.every(10).minutes.do(job)
来源：http://wf.yuexingan06.cn

[U37] Py：读写 Excel
来源：http://ay.chemitech.net.cn

pandas.read_excel / DataFrame.to_excel
来源：http://nn.521024.cn

[U38] Py：获取脚本所在目录
来源：http://xu.wgjwhj.cn

Path(__file__).resolve().parent
来源：http://ao.chemitech.net.cn

[U39] Py：判断是否在交互环境
来源：http://my.jianghongdianzi.cn

sys.stdout.isatty()
来源：http://bo.szxytkj.cn

[U40] Py：打印到标准错误
来源：http://vd.nicolike.cn

print("err", file=sys.stderr)
来源：http://ea.huanxung.cn

[U41] PHP：初始化 Composer 项目
来源：http://di.szxytkj.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://mi.hnjuh.cn

[U42] PHP：PSR-4 自动加载
来源：http://qq.asd995.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://jt.shxzukj.cn

[U43] PHP：声明命名空间
来源：http://rd.newstarts.cn

namespace App\Http;
来源：http://jx.huixinmuqiang.cn

[U44] PHP：开启严格类型
来源：http://pv.panjiajie.cn

declare(strict_types=1);
来源：http://ra.shxzskj.cn

[U45] PHP：类型声明与返回类型
来源：http://wd.colortex.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://lf.chemitech.net.cn

[U46] PHP：可空类型
来源：http://aa.huixinmuqiang.cn

?string $name = null
来源：http://kr.szxytkj.cn

[U47] PHP：联合类型
来源：http://zh.muxihuayi.cn

int|string $id
来源：http://ph.szsharing.cn

[U48] PHP：纯枚举
来源：http://cy.wgjwhj.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://dm.colortex.cn


<!-- 参考信息 -->