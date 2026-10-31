代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://nz.yuntaijiaju.cn

[S21] C：字符类别判断
来源：http://tr.hnjuh.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://pn.shtwfgs.cn

[S22] C：字符串转数字
来源：http://qq.huanxung.cn

atoi("42");  strtod("3.14", NULL);
来源：http://kd.shxzskj.cn

[S23] C：随机数
来源：http://zf.newstarts.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://vi.hnjuh.cn

[S24] C：获取本地时间
来源：http://ez.huixinmuqiang.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://rn.shxzukj.cn

[S25] C：内存拷贝
来源：http://on.9csxet.cn

memcpy(dst, src, n);
来源：http://gu.muxihuayi.cn

[S26] C：内存清零
来源：http://nc.wgjwhj.cn

memset(a, 0, sizeof a);
来源：http://km.muxihuayi.cn

[S27] C：定义常量
来源：http://kn.jianghongdianzi.cn

const double PI = 3.14159;
来源：http://pg.hahajie.cn

[S28] C：静态变量
来源：http://yq.haigaiapp.cn

static int counter = 0;
来源：http://qq.szsharing.cn

[S29] C：变参函数
来源：http://ej.jianghongdianzi.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://rx.szsharing.cn

[S30] C：头文件保护
来源：http://ya.nicolike.cn

#ifndef X_H
来源：http://en.shtwfgs.cn

#define X_H
来源：http://ku.asd995.cn

#endif
来源：http://aq.shxzukj.cn

[S31] C++：Hello World
来源：http://kc.yuexingan06.cn

#include <iostream>
来源：http://xk.szxytkj.cn

int main() { std::cout << "Hello\n"; }
来源：http://ba.huixinmuqiang.cn

[S32] C++：字符串
来源：http://xa.chemitech.net.cn

std::string s = "hi";  s += "!";
来源：http://jh.colortex.cn

[S33] C++：vector 增删
来源：http://tq.shxzskj.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://wp.shxzskj.cn

[S34] C++：遍历 vector
来源：http://du.chemitech.net.cn

for (auto &x : v) { std::cout << x; }
来源：http://on.huixinmuqiang.cn

[S35] C++：map
来源：http://hp.wgjwhj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://vb.lnxyls.cn

[S36] C++：unordered_map
来源：http://ii.nszjky.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://em.szsharing.cn

[S37] C++：set
来源：http://sg.hahajie.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://dn.lnxyls.cn

[S38] C++：排序
来源：http://ms.jctech888.com.cn

std::sort(v.begin(), v.end());
来源：http://ld.huixiangedu.cn

[S39] C++：自定义比较器排序
来源：http://ma.chemitech.net.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://df.hnjuh.cn

[S40] C++：查找元素
来源：http://tr.panjiajie.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hv.chemitech.net.cn

[S41] C++：类与构造函数
来源：http://jv.shxzskj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://oi.9csxet.cn

[S42] C++：继承与虚函数
来源：http://qt.bookmarksfly.cn

class B : public Base { public: void f() override {} };
来源：http://ye.szsharing.cn

[S43] C++：智能指针
来源：http://mv.asd995.cn

auto p = std::make_unique<int>(5);
来源：http://sx.shxzskj.cn

[S44] C++：引用传参
来源：http://ot.colortex.cn

void inc(int &x) { ++x; }
来源：http://ny.newstarts.cn

[S45] C++：lambda
来源：http://ta.bjjhwx.cn

auto add = [](int a, int b) { return a + b; };
来源：http://af.hahajie.cn

[S46] C++：函数模板
来源：http://th.jctech888.com.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://vc.newstarts.cn

[S47] C++：结构化绑定遍历
来源：http://ed.yuexingan06.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ly.jctech888.com.cn

[S48] C++：逐行读文件
来源：http://qi.szxytkj.cn

std::ifstream in("a.txt");  std::string line;
来源：http://zv.huixinmuqiang.cn

while (std::getline(in, line)) { }
来源：http://he.nicolike.cn

[S49] C++：写文件
来源：http://fw.shxzukj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://lf.shxzukj.cn

[S50] C++：格式化数字
来源：http://so.muxihuayi.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://se.nszjky.cn

[S51] C++：显式类型转换
来源：http://lj.bjjhwx.cn

static_cast<double>(a) / b
来源：http://tu.shtwfgs.cn

[S52] C++：const 与 noexcept
来源：http://lz.panjiajie.cn

int size() const noexcept { return n_; }
来源：http://pu.wgjwhj.cn

[S53] C++：移动语义
来源：http://vr.haigaiapp.cn

std::vector<int> w = std::move(v);
来源：http://zt.yuntaijiaju.cn

[S54] C++：异常处理
来源：http://im.shxzskj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hc.bookmarksfly.cn

[S55] C++：结构化绑定
来源：http://me.bookmarksfly.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://vo.panjiajie.cn

[S56] C++：optional
来源：http://eq.shxzskj.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://gg.chemitech.net.cn

[S57] C++：编译期常量
来源：http://fo.jianghongdianzi.cn

constexpr int N = 10;
来源：http://eb.newstarts.cn

[S58] C++：命名空间
来源：http://si.shxzskj.cn

namespace ns { int f() { return 1; } }
来源：http://xz.asd995.cn

[S59] C++：静态断言
来源：http://jw.asd995.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://kf.9csxet.cn

[S60] C++：遍历并删除元素
来源：http://qn.hahajie.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ra.chemitech.net.cn

================================================================================
来源：http://rp.chemitech.net.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://rw.bjjhwx.cn

================================================================================
来源：http://fp.jianghongdianzi.cn

[T01] Kotlin：Hello World
来源：http://um.bjjhwx.cn

println("Hello")
来源：http://rk.nszjky.cn

[T02] Kotlin：变量
来源：http://wa.huixinmuqiang.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://kx.bookmarksfly.cn

[T03] Kotlin：字符串模板
来源：http://an.shxzskj.cn

"值: $b"
来源：http://ep.wgjwhj.cn

[T04] Kotlin：空安全
来源：http://qa.colortex.cn

val n: String? = null;  n?.length
来源：http://tg.lnxyls.cn

[T05] Kotlin：when 表达式
来源：http://ho.shtwfgs.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://vt.chemitech.net.cn

[T06] Kotlin：集合映射
来源：http://dv.chemitech.net.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://nd.szxytkj.cn

[T07] Kotlin：集合过滤
来源：http://iz.bjjhwx.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://bx.lnxyls.cn

[T08] Kotlin：数据类
来源：http://ap.shxzukj.cn

data class User(val name: String, val age: Int)
来源：http://fk.nszjky.cn

[T09] Kotlin：扩展函数
来源：http://zp.newstarts.cn

fun String.exclaim() = this + "!"
来源：http://gw.chemitech.net.cn

[T10] Kotlin：默认参数
来源：http://ig.lnxyls.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://eg.jctech888.com.cn

[T11] Kotlin：协程
来源：http://cp.colortex.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://zn.521024.cn

[T12] Kotlin：解构声明
来源：http://qu.nszjky.cn

val (a, b) = Pair(1, 2)
来源：http://kj.newstarts.cn

[T13] Kotlin：只读 Map
来源：http://hm.szxytkj.cn

val m = mapOf("a" to 1)
来源：http://hl.huanxung.cn

[T14] Kotlin：循环
来源：http://ox.huixinmuqiang.cn

for (i in 1..10) println(i)
来源：http://le.muxihuayi.cn

[T15] Kotlin：接口
来源：http://fm.lnxyls.cn

interface Shape { fun area(): Double }
来源：http://ip.lnxyls.cn

[T16] Swift：Hello World
来源：http://cz.bjjhwx.cn

print("Hello")
来源：http://zu.shtwfgs.cn

[T17] Swift：变量与常量
来源：http://aw.hahajie.cn

var a = 1;  let b = 2
来源：http://ww.shtwfgs.cn

[T18] Swift：字符串插值
来源：http://my.huanxung.cn

"值: \(b)"
来源：http://uu.shxzskj.cn

[T19] Swift：可选绑定
来源：http://gc.huixiangedu.cn

if let n = opt { print(n) }
来源：http://vu.jianghongdianzi.cn

[T20] Swift：数组操作
来源：http://li.jianghongdianzi.cn

var a = [1, 2, 3];  a.append(4)
来源：http://pr.gzmigu.cn

[T21] Swift：遍历
来源：http://la.shxzskj.cn

for x in a { print(x) }
来源：http://sj.szsharing.cn

[T22] Swift：字典
来源：http://rs.521024.cn

var d = ["a": 1];  d["b"] = 2
来源：http://sy.huixiangedu.cn

[T23] Swift：函数
来源：http://ku.szxytkj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hn.chemitech.net.cn

[T24] Swift：闭包
来源：http://pf.newstarts.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://bv.huixiangedu.cn

[T25] Swift：结构体
来源：http://vu.huixinmuqiang.cn

struct P { var x: Int }
来源：http://ey.lnxyls.cn

[T26] Swift：类与重写
来源：http://ip.yuexingan06.cn

class A: Base { override func f() {} }
来源：http://yk.szxytkj.cn

[T27] Swift：错误处理
来源：http://fr.shxzukj.cn

do { try f() } catch { print(error) }
来源：http://dx.wgjwhj.cn

[T28] Swift：枚举
来源：http://eq.shxzukj.cn

enum Color { case red, green }
来源：http://wv.asd995.cn

[T29] Swift：guard 提前返回
来源：http://la.bookmarksfly.cn

guard let x = opt else { return }
来源：http://de.panjiajie.cn

[T30] Swift：协议
来源：http://ir.asd995.cn

protocol Shape { func area() -> Double }
来源：http://rx.huixinmuqiang.cn

[T31] Lua：Hello World
来源：http://rg.huixinmuqiang.cn

print("Hello")
来源：http://jo.haigaiapp.cn

[T32] Lua：局部变量
来源：http://zp.shxzskj.cn

local a = 1
来源：http://qq.hnjuh.cn

[T33] Lua：表（数组）
来源：http://lj.bookmarksfly.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://or.bjjhwx.cn

[T34] Lua：遍历表
来源：http://ov.asd995.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://eo.yuexingan06.cn

[T35] Lua：字典表
来源：http://fh.huanxung.cn

local d = { a = 1 };  d.b = 2
来源：http://ta.huixinmuqiang.cn

[T36] Lua：函数
来源：http://lb.wgjwhj.cn

function add(a, b) return a + b end
来源：http://yj.yuexingan06.cn

[T37] Lua：字符串拼接
来源：http://ib.yuexingan06.cn

"a" .. "b"
来源：http://ru.shxzukj.cn

[T38] Lua：条件
来源：http://xh.jianghongdianzi.cn

if x > 0 then print("正") end
来源：http://tn.bjjhwx.cn

[T39] Lua：模式匹配
来源：http://mn.hnjuh.cn

string.find(s, "%d+")
来源：http://vh.shxzskj.cn

[T40] Lua：元表
来源：http://ya.jctech888.com.cn

setmetatable({}, { __index = base })
来源：http://rk.huanxung.cn

[T41] Perl：Hello World
来源：http://dm.asd995.cn

print "Hello\n";
来源：http://jj.bookmarksfly.cn

[T42] Perl：变量类型
来源：http://dd.yuntaijiaju.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ww.bjjhwx.cn

[T43] Perl：字符串插值
来源：http://kr.wgjwhj.cn

"值: $a"
来源：http://bw.jctech888.com.cn

[T44] Perl：条件
来源：http://vy.huixiangedu.cn

if ($a > 0) { print "正"; }
来源：http://cv.asd995.cn

[T45] Perl：数组遍历
来源：http://ne.panjiajie.cn

for my $x (@arr) { print $x; }
来源：http://sv.panjiajie.cn

[T46] Perl：哈希操作
来源：http://zk.huixiangedu.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hu.asd995.cn

[T47] Perl：正则捕获
来源：http://lf.yuntaijiaju.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://wr.bookmarksfly.cn

[T48] Perl：正则替换
来源：http://jl.huanxung.cn

$s =~ s/old/new/g;
来源：http://bl.huanxung.cn

[T49] Perl：函数
来源：http://fv.huanxung.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hb.colortex.cn

[T50] Perl：逐行读文件
来源：http://qq.yuntaijiaju.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://wr.haigaiapp.cn

while (my $line = <$fh>) { print $line; }
来源：http://wv.huanxung.cn

[T51] Scala：Hello World
来源：http://ph.szsharing.cn

println("Hello")
来源：http://kb.colortex.cn

[T52] Scala：变量
来源：http://yy.bjjhwx.cn

val a = 1;  var b = 2
来源：http://gm.yuexingan06.cn

[T53] Scala：字符串插值
来源：http://yk.521024.cn

s"值: $b"
来源：http://on.gzmigu.cn

[T54] Scala：集合映射
来源：http://nj.haigaiapp.cn

List(1, 2, 3).map(_ * 2)
来源：http://an.chemitech.net.cn

[T55] Scala：集合过滤
来源：http://dq.szxytkj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://mg.muxihuayi.cn

[T56] Scala：样例类
来源：http://zm.shxzukj.cn

case class User(name: String, age: Int)
来源：http://jk.9csxet.cn

[T57] Scala：模式匹配
来源：http://xg.jctech888.com.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://lf.huanxung.cn

[T58] Scala：函数定义
来源：http://wg.colortex.cn

def add(a: Int, b: Int): Int = a + b
来源：http://kn.haigaiapp.cn

[T59] Scala：循环
来源：http://ub.bookmarksfly.cn

for (i <- 1 to 10) println(i)
来源：http://uc.huixinmuqiang.cn

[T60] Scala：折叠
来源：http://id.yuntaijiaju.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ux.shxzukj.cn

================================================================================
来源：http://cp.shxzukj.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://kk.newstarts.cn

================================================================================
来源：http://ut.9csxet.cn

[U01] Py：创建虚拟环境
来源：http://ej.asd995.cn

python -m venv .venv && source .venv/bin/activate
来源：http://zo.yuntaijiaju.cn

[U02] Py：导出 / 安装依赖
来源：http://um.bookmarksfly.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://fa.huixinmuqiang.cn

[U03] Py：加载 .env 配置
来源：http://yf.asd995.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://rd.gzmigu.cn

[U04] Py：变量调试打印
来源：http://gj.chemitech.net.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://to.asd995.cn

[U05] Py：列表去重且保序
来源：http://hj.szsharing.cn

list(dict.fromkeys(arr))
来源：http://td.szsharing.cn

[U06] Py：合并两个字典
来源：http://yn.muxihuayi.cn

{**a, **b}
来源：http://hl.szsharing.cn

[U07] Py：反转字典键值
来源：http://en.panjiajie.cn

{v: k for k, v in d.items()}
来源：http://ag.jctech888.com.cn

[U08] Py：展平二维列表
来源：http://ke.yuexingan06.cn

[y for x in nested for y in x]
来源：http://ut.shxzskj.cn

[U09] Py：字典取最大值的键
来源：http://cp.panjiajie.cn

max(d, key=d.get)
来源：http://xi.muxihuayi.cn

[U10] Py：按值排序字典
来源：http://gn.huixinmuqiang.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ra.huixinmuqiang.cn

[U11] Py：生成器表达式
来源：http://zw.shxzskj.cn

(x * 2 for x in arr)
来源：http://sc.wgjwhj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://yn.haigaiapp.cn

Counter(arr).most_common(3)
来源：http://mp.hahajie.cn

[U13] Py：固定长度队列
来源：http://ba.huixiangedu.cn

deque(maxlen=10)
来源：http://qo.shtwfgs.cn

[U14] Py：分组收集到列表
来源：http://rb.panjiajie.cn

defaultdict(list)
来源：http://qk.nszjky.cn

[U15] Py：高精度计时
来源：http://zq.chemitech.net.cn

t = time.perf_counter()
来源：http://xr.huanxung.cn

[U16] Py：命令行参数解析
来源：http://ek.huanxung.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://uy.nszjky.cn

[U17] Py：初始化日志
来源：http://tu.jianghongdianzi.cn

logging.basicConfig(level=logging.INFO)
来源：http://dn.shtwfgs.cn

[U18] Py：预编译正则
来源：http://kw.shtwfgs.cn

pat = re.compile(r"\d+")
来源：http://ei.yuexingan06.cn

[U19] Py：正则替换带回调
来源：http://fr.chemitech.net.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://oq.hnjuh.cn

[U20] Py：缓存函数结果
来源：http://wm.newstarts.cn

@functools.lru_cache(maxsize=None)
来源：http://mt.szxytkj.cn

[U21] Py：自定义上下文管理器
来源：http://wz.wgjwhj.cn

@contextlib.contextmanager
来源：http://sg.shtwfgs.cn

[U22] Py：矩阵转置
来源：http://hh.huixiangedu.cn

list(zip(*m))
来源：http://tu.szxytkj.cn

[U23] Py：分块读取大文件
来源：http://so.jianghongdianzi.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://qs.shxzukj.cn

[U24] Py：路径操作
来源：http://sk.colortex.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://st.szxytkj.cn

[U25] Py：CSV 按字典读
来源：http://gr.jianghongdianzi.cn

csv.DictReader(f)
来源：http://pt.521024.cn

[U26] Py：并发下载
来源：http://dv.hnjuh.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://as.yuexingan06.cn

[U27] Py：异步 HTTP
来源：http://mr.shxzukj.cn

aiohttp.ClientSession() 配合 async with
来源：http://us.szxytkj.cn

[U28] Py：类型别名
来源：http://ww.haigaiapp.cn

UserId = int
来源：http://gj.lnxyls.cn

[U29] Py：属性校验
来源：http://oo.szsharing.cn

@property 与 @x.setter 配合
来源：http://nj.jctech888.com.cn

[U30] Py：数据类
来源：http://nn.jianghongdianzi.cn

@dataclass(slots=True)
来源：http://jv.shxzskj.cn

[U31] Py：单测
来源：http://oy.muxihuayi.cn

python -m pytest -q
来源：http://yu.shxzukj.cn

[U32] Py：代码格式化
来源：http://pv.jianghongdianzi.cn

ruff format . && ruff check --fix .
来源：http://sl.hahajie.cn

[U33] Py：打包发布
来源：http://xt.bjjhwx.cn

python -m build  （依赖 pyproject.toml）
来源：http://mu.bookmarksfly.cn

[U34] Py：判断编码
来源：http://aj.wgjwhj.cn

chardet.detect(raw)
来源：http://im.lnxyls.cn

[U35] Py：发送邮件
来源：http://vy.shxzukj.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://rk.yuntaijiaju.cn

[U36] Py：定时任务
来源：http://yf.newstarts.cn

schedule.every(10).minutes.do(job)
来源：http://in.bookmarksfly.cn

[U37] Py：读写 Excel
来源：http://mk.asd995.cn

pandas.read_excel / DataFrame.to_excel
来源：http://df.jctech888.com.cn

[U38] Py：获取脚本所在目录
来源：http://mb.jianghongdianzi.cn

Path(__file__).resolve().parent
来源：http://wz.chemitech.net.cn

[U39] Py：判断是否在交互环境
来源：http://jk.bookmarksfly.cn

sys.stdout.isatty()
来源：http://jz.asd995.cn

[U40] Py：打印到标准错误
来源：http://rt.9csxet.cn

print("err", file=sys.stderr)
来源：http://mm.jianghongdianzi.cn

[U41] PHP：初始化 Composer 项目
来源：http://cv.lnxyls.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ty.panjiajie.cn

[U42] PHP：PSR-4 自动加载
来源：http://xk.hnjuh.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://br.yuexingan06.cn

[U43] PHP：声明命名空间
来源：http://uy.jianghongdianzi.cn

namespace App\Http;
来源：http://oh.jctech888.com.cn

[U44] PHP：开启严格类型
来源：http://of.huanxung.cn

declare(strict_types=1);
来源：http://wz.gzmigu.cn


<!-- 参考信息 -->