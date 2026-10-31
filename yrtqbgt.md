代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://yh.huixiangedu.cn

[S25] C：内存拷贝
来源：http://fh.shxzskj.cn

memcpy(dst, src, n);
来源：http://kv.chemitech.net.cn

[S26] C：内存清零
来源：http://av.nicolike.cn

memset(a, 0, sizeof a);
来源：http://ml.nszjky.cn

[S27] C：定义常量
来源：http://wb.szsharing.cn

const double PI = 3.14159;
来源：http://kf.yuntaijiaju.cn

[S28] C：静态变量
来源：http://tk.szxytkj.cn

static int counter = 0;
来源：http://ww.bookmarksfly.cn

[S29] C：变参函数
来源：http://ad.wgjwhj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://sd.szxytkj.cn

[S30] C：头文件保护
来源：http://dc.shxzskj.cn

#ifndef X_H
来源：http://pn.panjiajie.cn

#define X_H
来源：http://xn.szsharing.cn

#endif
来源：http://ke.panjiajie.cn

[S31] C++：Hello World
来源：http://ts.panjiajie.cn

#include <iostream>
来源：http://ji.jianghongdianzi.cn

int main() { std::cout << "Hello\n"; }
来源：http://fl.521024.cn

[S32] C++：字符串
来源：http://wy.shtwfgs.cn

std::string s = "hi";  s += "!";
来源：http://lr.huanxung.cn

[S33] C++：vector 增删
来源：http://ai.nicolike.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://km.521024.cn

[S34] C++：遍历 vector
来源：http://of.nicolike.cn

for (auto &x : v) { std::cout << x; }
来源：http://ld.asd995.cn

[S35] C++：map
来源：http://ff.yuexingan06.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ig.hahajie.cn

[S36] C++：unordered_map
来源：http://mx.asd995.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ao.nicolike.cn

[S37] C++：set
来源：http://it.panjiajie.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://yx.bookmarksfly.cn

[S38] C++：排序
来源：http://ve.lnxyls.cn

std::sort(v.begin(), v.end());
来源：http://iq.szsharing.cn

[S39] C++：自定义比较器排序
来源：http://ip.wgjwhj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ho.nicolike.cn

[S40] C++：查找元素
来源：http://lb.chemitech.net.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://fs.huixiangedu.cn

[S41] C++：类与构造函数
来源：http://sk.hnjuh.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://al.lnxyls.cn

[S42] C++：继承与虚函数
来源：http://ie.shtwfgs.cn

class B : public Base { public: void f() override {} };
来源：http://jd.yuexingan06.cn

[S43] C++：智能指针
来源：http://nk.nszjky.cn

auto p = std::make_unique<int>(5);
来源：http://bn.huixiangedu.cn

[S44] C++：引用传参
来源：http://fc.huanxung.cn

void inc(int &x) { ++x; }
来源：http://xk.newstarts.cn

[S45] C++：lambda
来源：http://qu.jianghongdianzi.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ws.yuntaijiaju.cn

[S46] C++：函数模板
来源：http://tr.yuntaijiaju.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ob.szsharing.cn

[S47] C++：结构化绑定遍历
来源：http://ej.huixinmuqiang.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://nk.jianghongdianzi.cn

[S48] C++：逐行读文件
来源：http://kn.yuexingan06.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ab.szsharing.cn

while (std::getline(in, line)) { }
来源：http://fq.gzmigu.cn

[S49] C++：写文件
来源：http://ab.wgjwhj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://do.nicolike.cn

[S50] C++：格式化数字
来源：http://iw.colortex.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ri.gzmigu.cn

[S51] C++：显式类型转换
来源：http://wn.haigaiapp.cn

static_cast<double>(a) / b
来源：http://dn.haigaiapp.cn

[S52] C++：const 与 noexcept
来源：http://dd.521024.cn

int size() const noexcept { return n_; }
来源：http://jx.huixinmuqiang.cn

[S53] C++：移动语义
来源：http://ls.shtwfgs.cn

std::vector<int> w = std::move(v);
来源：http://bt.asd995.cn

[S54] C++：异常处理
来源：http://ve.gzmigu.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://rg.panjiajie.cn

[S55] C++：结构化绑定
来源：http://pn.nicolike.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://rb.jctech888.com.cn

[S56] C++：optional
来源：http://mn.yuexingan06.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ae.haigaiapp.cn

[S57] C++：编译期常量
来源：http://kq.lnxyls.cn

constexpr int N = 10;
来源：http://ef.bjjhwx.cn

[S58] C++：命名空间
来源：http://du.bookmarksfly.cn

namespace ns { int f() { return 1; } }
来源：http://pl.shxzukj.cn

[S59] C++：静态断言
来源：http://uo.colortex.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://bo.nszjky.cn

[S60] C++：遍历并删除元素
来源：http://fm.hnjuh.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ov.chemitech.net.cn

================================================================================
来源：http://um.newstarts.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://kj.huanxung.cn

================================================================================
来源：http://um.521024.cn

[T01] Kotlin：Hello World
来源：http://vf.hnjuh.cn

println("Hello")
来源：http://fb.nicolike.cn

[T02] Kotlin：变量
来源：http://ib.huanxung.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://nw.szxytkj.cn

[T03] Kotlin：字符串模板
来源：http://ak.yuntaijiaju.cn

"值: $b"
来源：http://nw.panjiajie.cn

[T04] Kotlin：空安全
来源：http://vn.szxytkj.cn

val n: String? = null;  n?.length
来源：http://hm.9csxet.cn

[T05] Kotlin：when 表达式
来源：http://ea.jctech888.com.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://pm.wgjwhj.cn

[T06] Kotlin：集合映射
来源：http://py.yuntaijiaju.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ph.9csxet.cn

[T07] Kotlin：集合过滤
来源：http://bv.521024.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://nu.haigaiapp.cn

[T08] Kotlin：数据类
来源：http://yf.huixinmuqiang.cn

data class User(val name: String, val age: Int)
来源：http://rk.shtwfgs.cn

[T09] Kotlin：扩展函数
来源：http://rt.huixiangedu.cn

fun String.exclaim() = this + "!"
来源：http://da.szsharing.cn

[T10] Kotlin：默认参数
来源：http://pg.muxihuayi.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://wo.colortex.cn

[T11] Kotlin：协程
来源：http://er.colortex.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://og.yuntaijiaju.cn

[T12] Kotlin：解构声明
来源：http://rc.wgjwhj.cn

val (a, b) = Pair(1, 2)
来源：http://bo.wgjwhj.cn

[T13] Kotlin：只读 Map
来源：http://ek.hahajie.cn

val m = mapOf("a" to 1)
来源：http://yx.muxihuayi.cn

[T14] Kotlin：循环
来源：http://dw.jianghongdianzi.cn

for (i in 1..10) println(i)
来源：http://ts.jianghongdianzi.cn

[T15] Kotlin：接口
来源：http://nk.huixiangedu.cn

interface Shape { fun area(): Double }
来源：http://ah.nszjky.cn

[T16] Swift：Hello World
来源：http://gl.yuexingan06.cn

print("Hello")
来源：http://ph.521024.cn

[T17] Swift：变量与常量
来源：http://fg.colortex.cn

var a = 1;  let b = 2
来源：http://qb.chemitech.net.cn

[T18] Swift：字符串插值
来源：http://ul.hnjuh.cn

"值: \(b)"
来源：http://vc.shtwfgs.cn

[T19] Swift：可选绑定
来源：http://zc.nszjky.cn

if let n = opt { print(n) }
来源：http://wf.shtwfgs.cn

[T20] Swift：数组操作
来源：http://do.huixinmuqiang.cn

var a = [1, 2, 3];  a.append(4)
来源：http://tc.wgjwhj.cn

[T21] Swift：遍历
来源：http://ol.szxytkj.cn

for x in a { print(x) }
来源：http://oz.521024.cn

[T22] Swift：字典
来源：http://jc.bookmarksfly.cn

var d = ["a": 1];  d["b"] = 2
来源：http://lk.huixinmuqiang.cn

[T23] Swift：函数
来源：http://cb.szsharing.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://yg.colortex.cn

[T24] Swift：闭包
来源：http://rf.colortex.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://up.hnjuh.cn

[T25] Swift：结构体
来源：http://en.huanxung.cn

struct P { var x: Int }
来源：http://nm.hnjuh.cn

[T26] Swift：类与重写
来源：http://nj.jianghongdianzi.cn

class A: Base { override func f() {} }
来源：http://tp.yuexingan06.cn

[T27] Swift：错误处理
来源：http://ny.bookmarksfly.cn

do { try f() } catch { print(error) }
来源：http://dy.jctech888.com.cn

[T28] Swift：枚举
来源：http://ko.nicolike.cn

enum Color { case red, green }
来源：http://bf.asd995.cn

[T29] Swift：guard 提前返回
来源：http://oc.huanxung.cn

guard let x = opt else { return }
来源：http://kl.asd995.cn

[T30] Swift：协议
来源：http://xb.szxytkj.cn

protocol Shape { func area() -> Double }
来源：http://ww.newstarts.cn

[T31] Lua：Hello World
来源：http://rv.yuexingan06.cn

print("Hello")
来源：http://pi.huixinmuqiang.cn

[T32] Lua：局部变量
来源：http://jr.nszjky.cn

local a = 1
来源：http://dn.asd995.cn

[T33] Lua：表（数组）
来源：http://lo.nicolike.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://id.nszjky.cn

[T34] Lua：遍历表
来源：http://il.521024.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://bi.bookmarksfly.cn

[T35] Lua：字典表
来源：http://du.hahajie.cn

local d = { a = 1 };  d.b = 2
来源：http://bi.9csxet.cn

[T36] Lua：函数
来源：http://of.huixinmuqiang.cn

function add(a, b) return a + b end
来源：http://ip.colortex.cn

[T37] Lua：字符串拼接
来源：http://la.asd995.cn

"a" .. "b"
来源：http://fm.jianghongdianzi.cn

[T38] Lua：条件
来源：http://yk.haigaiapp.cn

if x > 0 then print("正") end
来源：http://lw.haigaiapp.cn

[T39] Lua：模式匹配
来源：http://qt.bookmarksfly.cn

string.find(s, "%d+")
来源：http://cm.newstarts.cn

[T40] Lua：元表
来源：http://ev.newstarts.cn

setmetatable({}, { __index = base })
来源：http://vt.lnxyls.cn

[T41] Perl：Hello World
来源：http://fw.yuexingan06.cn

print "Hello\n";
来源：http://li.hnjuh.cn

[T42] Perl：变量类型
来源：http://yr.shxzukj.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://kx.yuexingan06.cn

[T43] Perl：字符串插值
来源：http://hf.szxytkj.cn

"值: $a"
来源：http://du.muxihuayi.cn

[T44] Perl：条件
来源：http://wg.muxihuayi.cn

if ($a > 0) { print "正"; }
来源：http://ln.bookmarksfly.cn

[T45] Perl：数组遍历
来源：http://iv.newstarts.cn

for my $x (@arr) { print $x; }
来源：http://uc.szxytkj.cn

[T46] Perl：哈希操作
来源：http://nv.yuexingan06.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://fn.szxytkj.cn

[T47] Perl：正则捕获
来源：http://wb.huixinmuqiang.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://te.lnxyls.cn

[T48] Perl：正则替换
来源：http://ye.haigaiapp.cn

$s =~ s/old/new/g;
来源：http://qi.yuntaijiaju.cn

[T49] Perl：函数
来源：http://im.shxzskj.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ib.shtwfgs.cn

[T50] Perl：逐行读文件
来源：http://me.lnxyls.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://el.wgjwhj.cn

while (my $line = <$fh>) { print $line; }
来源：http://wu.wgjwhj.cn

[T51] Scala：Hello World
来源：http://av.shxzukj.cn

println("Hello")
来源：http://vp.hnjuh.cn

[T52] Scala：变量
来源：http://xz.bjjhwx.cn

val a = 1;  var b = 2
来源：http://dp.chemitech.net.cn

[T53] Scala：字符串插值
来源：http://li.jianghongdianzi.cn

s"值: $b"
来源：http://vg.colortex.cn

[T54] Scala：集合映射
来源：http://ws.yuntaijiaju.cn

List(1, 2, 3).map(_ * 2)
来源：http://fx.haigaiapp.cn

[T55] Scala：集合过滤
来源：http://pv.lnxyls.cn

List(1, 2, 3).filter(_ > 1)
来源：http://lr.hnjuh.cn

[T56] Scala：样例类
来源：http://mw.colortex.cn

case class User(name: String, age: Int)
来源：http://jt.colortex.cn

[T57] Scala：模式匹配
来源：http://bs.szsharing.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://qc.bjjhwx.cn

[T58] Scala：函数定义
来源：http://za.9csxet.cn

def add(a: Int, b: Int): Int = a + b
来源：http://zx.yuntaijiaju.cn

[T59] Scala：循环
来源：http://af.muxihuayi.cn

for (i <- 1 to 10) println(i)
来源：http://xg.haigaiapp.cn

[T60] Scala：折叠
来源：http://gb.bjjhwx.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://xj.colortex.cn

================================================================================
来源：http://rr.bookmarksfly.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wg.colortex.cn

================================================================================
来源：http://ic.521024.cn

[U01] Py：创建虚拟环境
来源：http://bk.yuntaijiaju.cn

python -m venv .venv && source .venv/bin/activate
来源：http://xj.jianghongdianzi.cn

[U02] Py：导出 / 安装依赖
来源：http://dn.szxytkj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://at.jianghongdianzi.cn

[U03] Py：加载 .env 配置
来源：http://ar.muxihuayi.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://sa.colortex.cn

[U04] Py：变量调试打印
来源：http://at.huixiangedu.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://eg.gzmigu.cn

[U05] Py：列表去重且保序
来源：http://za.szxytkj.cn

list(dict.fromkeys(arr))
来源：http://pa.haigaiapp.cn

[U06] Py：合并两个字典
来源：http://ku.gzmigu.cn

{**a, **b}
来源：http://xz.newstarts.cn

[U07] Py：反转字典键值
来源：http://me.nszjky.cn

{v: k for k, v in d.items()}
来源：http://ao.yuntaijiaju.cn

[U08] Py：展平二维列表
来源：http://ux.gzmigu.cn

[y for x in nested for y in x]
来源：http://as.gzmigu.cn

[U09] Py：字典取最大值的键
来源：http://tj.hahajie.cn

max(d, key=d.get)
来源：http://bp.szxytkj.cn

[U10] Py：按值排序字典
来源：http://qp.huixiangedu.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://lf.nszjky.cn

[U11] Py：生成器表达式
来源：http://vm.nszjky.cn

(x * 2 for x in arr)
来源：http://us.lnxyls.cn

[U12] Py：取出现最多的 3 个元素
来源：http://xd.muxihuayi.cn

Counter(arr).most_common(3)
来源：http://zr.huixinmuqiang.cn

[U13] Py：固定长度队列
来源：http://ab.newstarts.cn

deque(maxlen=10)
来源：http://uz.panjiajie.cn

[U14] Py：分组收集到列表
来源：http://ik.hahajie.cn

defaultdict(list)
来源：http://es.newstarts.cn

[U15] Py：高精度计时
来源：http://jf.newstarts.cn

t = time.perf_counter()
来源：http://nm.wgjwhj.cn

[U16] Py：命令行参数解析
来源：http://gy.colortex.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://pl.9csxet.cn

[U17] Py：初始化日志
来源：http://ti.huanxung.cn

logging.basicConfig(level=logging.INFO)
来源：http://ep.gzmigu.cn

[U18] Py：预编译正则
来源：http://ty.newstarts.cn

pat = re.compile(r"\d+")
来源：http://ic.newstarts.cn

[U19] Py：正则替换带回调
来源：http://rc.9csxet.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://so.jctech888.com.cn

[U20] Py：缓存函数结果
来源：http://hz.panjiajie.cn

@functools.lru_cache(maxsize=None)
来源：http://da.shtwfgs.cn

[U21] Py：自定义上下文管理器
来源：http://ab.wgjwhj.cn

@contextlib.contextmanager
来源：http://nr.chemitech.net.cn

[U22] Py：矩阵转置
来源：http://iq.jctech888.com.cn

list(zip(*m))
来源：http://bw.newstarts.cn

[U23] Py：分块读取大文件
来源：http://hn.colortex.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://gk.bookmarksfly.cn

[U24] Py：路径操作
来源：http://ze.huixinmuqiang.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://pk.yuntaijiaju.cn

[U25] Py：CSV 按字典读
来源：http://sr.newstarts.cn

csv.DictReader(f)
来源：http://sw.shtwfgs.cn

[U26] Py：并发下载
来源：http://qr.huanxung.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://vx.bookmarksfly.cn

[U27] Py：异步 HTTP
来源：http://ix.wgjwhj.cn

aiohttp.ClientSession() 配合 async with
来源：http://dm.szxytkj.cn

[U28] Py：类型别名
来源：http://yq.panjiajie.cn

UserId = int
来源：http://mm.asd995.cn

[U29] Py：属性校验
来源：http://fk.jctech888.com.cn

@property 与 @x.setter 配合
来源：http://ui.muxihuayi.cn

[U30] Py：数据类
来源：http://pq.bjjhwx.cn

@dataclass(slots=True)
来源：http://pf.chemitech.net.cn

[U31] Py：单测
来源：http://lx.colortex.cn

python -m pytest -q
来源：http://ut.hahajie.cn

[U32] Py：代码格式化
来源：http://tb.9csxet.cn

ruff format . && ruff check --fix .
来源：http://co.gzmigu.cn

[U33] Py：打包发布
来源：http://pj.lnxyls.cn

python -m build  （依赖 pyproject.toml）
来源：http://wr.shxzukj.cn

[U34] Py：判断编码
来源：http://gt.bookmarksfly.cn

chardet.detect(raw)
来源：http://mw.yuntaijiaju.cn

[U35] Py：发送邮件
来源：http://oi.shtwfgs.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://zp.colortex.cn

[U36] Py：定时任务
来源：http://cv.nszjky.cn

schedule.every(10).minutes.do(job)
来源：http://wn.hahajie.cn

[U37] Py：读写 Excel
来源：http://tj.bjjhwx.cn

pandas.read_excel / DataFrame.to_excel
来源：http://fr.huixiangedu.cn

[U38] Py：获取脚本所在目录
来源：http://ih.szxytkj.cn

Path(__file__).resolve().parent
来源：http://me.panjiajie.cn

[U39] Py：判断是否在交互环境
来源：http://hy.hahajie.cn

sys.stdout.isatty()
来源：http://gf.lnxyls.cn

[U40] Py：打印到标准错误
来源：http://ym.szxytkj.cn

print("err", file=sys.stderr)
来源：http://nc.asd995.cn

[U41] PHP：初始化 Composer 项目
来源：http://hl.shxzukj.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ov.newstarts.cn

[U42] PHP：PSR-4 自动加载
来源：http://lb.lnxyls.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://vi.huixinmuqiang.cn

[U43] PHP：声明命名空间
来源：http://nk.jianghongdianzi.cn

namespace App\Http;
来源：http://bj.nicolike.cn

[U44] PHP：开启严格类型
来源：http://bd.lnxyls.cn

declare(strict_types=1);
来源：http://ea.chemitech.net.cn

[U45] PHP：类型声明与返回类型
来源：http://nb.jctech888.com.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://an.hahajie.cn

[U46] PHP：可空类型
来源：http://hm.huanxung.cn

?string $name = null
来源：http://vy.yuntaijiaju.cn

[U47] PHP：联合类型
来源：http://gz.jianghongdianzi.cn

int|string $id
来源：http://hr.panjiajie.cn

[U48] PHP：纯枚举
来源：http://up.yuexingan06.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://jy.muxihuayi.cn


<!-- 参考信息 -->