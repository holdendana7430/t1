代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ou.colortex.cn

[S25] C：内存拷贝
来源：http://ri.huanxung.cn

memcpy(dst, src, n);
来源：http://ge.huanxung.cn

[S26] C：内存清零
来源：http://lz.shtwfgs.cn

memset(a, 0, sizeof a);
来源：http://kr.yuexingan06.cn

[S27] C：定义常量
来源：http://ev.lnxyls.cn

const double PI = 3.14159;
来源：http://xy.bookmarksfly.cn

[S28] C：静态变量
来源：http://lz.chemitech.net.cn

static int counter = 0;
来源：http://bs.szxytkj.cn

[S29] C：变参函数
来源：http://el.shxzukj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://sp.shtwfgs.cn

[S30] C：头文件保护
来源：http://ek.chemitech.net.cn

#ifndef X_H
来源：http://co.huanxung.cn

#define X_H
来源：http://lz.colortex.cn

#endif
来源：http://qr.shxzskj.cn

[S31] C++：Hello World
来源：http://kh.asd995.cn

#include <iostream>
来源：http://wj.muxihuayi.cn

int main() { std::cout << "Hello\n"; }
来源：http://vu.shxzskj.cn

[S32] C++：字符串
来源：http://ct.shxzskj.cn

std::string s = "hi";  s += "!";
来源：http://mc.colortex.cn

[S33] C++：vector 增删
来源：http://lh.hnjuh.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://tr.jianghongdianzi.cn

[S34] C++：遍历 vector
来源：http://vc.shxzskj.cn

for (auto &x : v) { std::cout << x; }
来源：http://cc.jctech888.com.cn

[S35] C++：map
来源：http://ir.shtwfgs.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://bl.chemitech.net.cn

[S36] C++：unordered_map
来源：http://fc.huixiangedu.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://bb.chemitech.net.cn

[S37] C++：set
来源：http://uc.wgjwhj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://is.huixiangedu.cn

[S38] C++：排序
来源：http://uy.panjiajie.cn

std::sort(v.begin(), v.end());
来源：http://rz.huixiangedu.cn

[S39] C++：自定义比较器排序
来源：http://gk.huanxung.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://cu.panjiajie.cn

[S40] C++：查找元素
来源：http://ma.bjjhwx.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://tn.bookmarksfly.cn

[S41] C++：类与构造函数
来源：http://rd.muxihuayi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ls.wgjwhj.cn

[S42] C++：继承与虚函数
来源：http://dm.shxzukj.cn

class B : public Base { public: void f() override {} };
来源：http://gl.shtwfgs.cn

[S43] C++：智能指针
来源：http://ve.asd995.cn

auto p = std::make_unique<int>(5);
来源：http://ne.yuexingan06.cn

[S44] C++：引用传参
来源：http://wg.lnxyls.cn

void inc(int &x) { ++x; }
来源：http://zb.nicolike.cn

[S45] C++：lambda
来源：http://mk.haigaiapp.cn

auto add = [](int a, int b) { return a + b; };
来源：http://co.chemitech.net.cn

[S46] C++：函数模板
来源：http://lp.newstarts.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://cu.521024.cn

[S47] C++：结构化绑定遍历
来源：http://li.jctech888.com.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://fh.nszjky.cn

[S48] C++：逐行读文件
来源：http://jc.lnxyls.cn

std::ifstream in("a.txt");  std::string line;
来源：http://pf.wgjwhj.cn

while (std::getline(in, line)) { }
来源：http://co.huanxung.cn

[S49] C++：写文件
来源：http://ur.lnxyls.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://so.yuexingan06.cn

[S50] C++：格式化数字
来源：http://ny.yuntaijiaju.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ju.hnjuh.cn

[S51] C++：显式类型转换
来源：http://yc.gzmigu.cn

static_cast<double>(a) / b
来源：http://bg.9csxet.cn

[S52] C++：const 与 noexcept
来源：http://yx.hnjuh.cn

int size() const noexcept { return n_; }
来源：http://ir.panjiajie.cn

[S53] C++：移动语义
来源：http://qv.hnjuh.cn

std::vector<int> w = std::move(v);
来源：http://mv.521024.cn

[S54] C++：异常处理
来源：http://mj.szsharing.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://gl.huanxung.cn

[S55] C++：结构化绑定
来源：http://mn.521024.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ix.muxihuayi.cn

[S56] C++：optional
来源：http://oj.bookmarksfly.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://vl.bjjhwx.cn

[S57] C++：编译期常量
来源：http://dr.hahajie.cn

constexpr int N = 10;
来源：http://qc.szsharing.cn

[S58] C++：命名空间
来源：http://ix.muxihuayi.cn

namespace ns { int f() { return 1; } }
来源：http://jx.bookmarksfly.cn

[S59] C++：静态断言
来源：http://rk.jianghongdianzi.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://wi.shxzskj.cn

[S60] C++：遍历并删除元素
来源：http://cm.haigaiapp.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wd.jctech888.com.cn

================================================================================
来源：http://vd.szxytkj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://pm.asd995.cn

================================================================================
来源：http://no.szxytkj.cn

[T01] Kotlin：Hello World
来源：http://af.haigaiapp.cn

println("Hello")
来源：http://bz.nszjky.cn

[T02] Kotlin：变量
来源：http://su.huanxung.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://kb.9csxet.cn

[T03] Kotlin：字符串模板
来源：http://pr.shtwfgs.cn

"值: $b"
来源：http://io.szsharing.cn

[T04] Kotlin：空安全
来源：http://id.hnjuh.cn

val n: String? = null;  n?.length
来源：http://fc.nicolike.cn

[T05] Kotlin：when 表达式
来源：http://qs.chemitech.net.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://me.muxihuayi.cn

[T06] Kotlin：集合映射
来源：http://up.huanxung.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://zp.bookmarksfly.cn

[T07] Kotlin：集合过滤
来源：http://lb.shxzskj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://tl.newstarts.cn

[T08] Kotlin：数据类
来源：http://uh.chemitech.net.cn

data class User(val name: String, val age: Int)
来源：http://gn.jianghongdianzi.cn

[T09] Kotlin：扩展函数
来源：http://bl.yuexingan06.cn

fun String.exclaim() = this + "!"
来源：http://rc.hnjuh.cn

[T10] Kotlin：默认参数
来源：http://dr.jianghongdianzi.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://nj.huixinmuqiang.cn

[T11] Kotlin：协程
来源：http://vg.bjjhwx.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://zp.gzmigu.cn

[T12] Kotlin：解构声明
来源：http://oc.yuntaijiaju.cn

val (a, b) = Pair(1, 2)
来源：http://vy.nszjky.cn

[T13] Kotlin：只读 Map
来源：http://th.hahajie.cn

val m = mapOf("a" to 1)
来源：http://gj.szxytkj.cn

[T14] Kotlin：循环
来源：http://dj.hnjuh.cn

for (i in 1..10) println(i)
来源：http://xl.wgjwhj.cn

[T15] Kotlin：接口
来源：http://pg.chemitech.net.cn

interface Shape { fun area(): Double }
来源：http://ol.huixiangedu.cn

[T16] Swift：Hello World
来源：http://fv.jianghongdianzi.cn

print("Hello")
来源：http://xh.jianghongdianzi.cn

[T17] Swift：变量与常量
来源：http://ql.chemitech.net.cn

var a = 1;  let b = 2
来源：http://vl.9csxet.cn

[T18] Swift：字符串插值
来源：http://ho.yuexingan06.cn

"值: \(b)"
来源：http://vp.lnxyls.cn

[T19] Swift：可选绑定
来源：http://vh.huixiangedu.cn

if let n = opt { print(n) }
来源：http://vx.bjjhwx.cn

[T20] Swift：数组操作
来源：http://em.huanxung.cn

var a = [1, 2, 3];  a.append(4)
来源：http://gq.jctech888.com.cn

[T21] Swift：遍历
来源：http://pd.gzmigu.cn

for x in a { print(x) }
来源：http://kq.szxytkj.cn

[T22] Swift：字典
来源：http://gd.szxytkj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://wq.panjiajie.cn

[T23] Swift：函数
来源：http://dm.hnjuh.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://od.huixinmuqiang.cn

[T24] Swift：闭包
来源：http://pm.newstarts.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://kk.szxytkj.cn

[T25] Swift：结构体
来源：http://ir.szxytkj.cn

struct P { var x: Int }
来源：http://dx.huixiangedu.cn

[T26] Swift：类与重写
来源：http://jq.9csxet.cn

class A: Base { override func f() {} }
来源：http://uv.chemitech.net.cn

[T27] Swift：错误处理
来源：http://dn.hnjuh.cn

do { try f() } catch { print(error) }
来源：http://qf.nicolike.cn

[T28] Swift：枚举
来源：http://so.9csxet.cn

enum Color { case red, green }
来源：http://nm.9csxet.cn

[T29] Swift：guard 提前返回
来源：http://wo.newstarts.cn

guard let x = opt else { return }
来源：http://xz.wgjwhj.cn

[T30] Swift：协议
来源：http://jl.huixiangedu.cn

protocol Shape { func area() -> Double }
来源：http://je.huixinmuqiang.cn

[T31] Lua：Hello World
来源：http://iq.newstarts.cn

print("Hello")
来源：http://fl.nicolike.cn

[T32] Lua：局部变量
来源：http://xg.lnxyls.cn

local a = 1
来源：http://fa.colortex.cn

[T33] Lua：表（数组）
来源：http://vr.chemitech.net.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://cm.szxytkj.cn

[T34] Lua：遍历表
来源：http://zz.panjiajie.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://pc.huixiangedu.cn

[T35] Lua：字典表
来源：http://zm.nszjky.cn

local d = { a = 1 };  d.b = 2
来源：http://jj.chemitech.net.cn

[T36] Lua：函数
来源：http://jd.huixinmuqiang.cn

function add(a, b) return a + b end
来源：http://st.panjiajie.cn

[T37] Lua：字符串拼接
来源：http://im.szxytkj.cn

"a" .. "b"
来源：http://eo.jianghongdianzi.cn

[T38] Lua：条件
来源：http://pz.jctech888.com.cn

if x > 0 then print("正") end
来源：http://jr.jctech888.com.cn

[T39] Lua：模式匹配
来源：http://wl.huixiangedu.cn

string.find(s, "%d+")
来源：http://pi.521024.cn

[T40] Lua：元表
来源：http://pr.chemitech.net.cn

setmetatable({}, { __index = base })
来源：http://bc.muxihuayi.cn

[T41] Perl：Hello World
来源：http://mq.nicolike.cn

print "Hello\n";
来源：http://sa.521024.cn

[T42] Perl：变量类型
来源：http://td.bjjhwx.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://cc.9csxet.cn

[T43] Perl：字符串插值
来源：http://ok.lnxyls.cn

"值: $a"
来源：http://cn.shxzskj.cn

[T44] Perl：条件
来源：http://fu.gzmigu.cn

if ($a > 0) { print "正"; }
来源：http://aw.asd995.cn

[T45] Perl：数组遍历
来源：http://ah.panjiajie.cn

for my $x (@arr) { print $x; }
来源：http://cr.nszjky.cn

[T46] Perl：哈希操作
来源：http://xh.panjiajie.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://rz.shtwfgs.cn

[T47] Perl：正则捕获
来源：http://lt.wgjwhj.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://es.jianghongdianzi.cn

[T48] Perl：正则替换
来源：http://cf.521024.cn

$s =~ s/old/new/g;
来源：http://vu.bjjhwx.cn

[T49] Perl：函数
来源：http://ji.bjjhwx.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://uj.asd995.cn

[T50] Perl：逐行读文件
来源：http://zz.bjjhwx.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://kw.nicolike.cn

while (my $line = <$fh>) { print $line; }
来源：http://yu.shtwfgs.cn

[T51] Scala：Hello World
来源：http://ig.szxytkj.cn

println("Hello")
来源：http://qt.wgjwhj.cn

[T52] Scala：变量
来源：http://rp.lnxyls.cn

val a = 1;  var b = 2
来源：http://ri.newstarts.cn

[T53] Scala：字符串插值
来源：http://gy.muxihuayi.cn

s"值: $b"
来源：http://bh.gzmigu.cn

[T54] Scala：集合映射
来源：http://fc.muxihuayi.cn

List(1, 2, 3).map(_ * 2)
来源：http://ma.lnxyls.cn

[T55] Scala：集合过滤
来源：http://or.newstarts.cn

List(1, 2, 3).filter(_ > 1)
来源：http://he.shtwfgs.cn

[T56] Scala：样例类
来源：http://mr.muxihuayi.cn

case class User(name: String, age: Int)
来源：http://sj.panjiajie.cn

[T57] Scala：模式匹配
来源：http://oz.nszjky.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://if.colortex.cn

[T58] Scala：函数定义
来源：http://xc.newstarts.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ww.jctech888.com.cn

[T59] Scala：循环
来源：http://fc.chemitech.net.cn

for (i <- 1 to 10) println(i)
来源：http://wv.nicolike.cn

[T60] Scala：折叠
来源：http://xq.huanxung.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://sy.gzmigu.cn

================================================================================
来源：http://mq.lnxyls.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://yn.newstarts.cn

================================================================================
来源：http://ql.chemitech.net.cn

[U01] Py：创建虚拟环境
来源：http://kb.panjiajie.cn

python -m venv .venv && source .venv/bin/activate
来源：http://bg.newstarts.cn

[U02] Py：导出 / 安装依赖
来源：http://fa.bookmarksfly.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://bp.shxzukj.cn

[U03] Py：加载 .env 配置
来源：http://zc.szxytkj.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://bn.gzmigu.cn

[U04] Py：变量调试打印
来源：http://ul.bjjhwx.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://jo.chemitech.net.cn

[U05] Py：列表去重且保序
来源：http://jv.yuntaijiaju.cn

list(dict.fromkeys(arr))
来源：http://oc.bookmarksfly.cn

[U06] Py：合并两个字典
来源：http://xt.hnjuh.cn

{**a, **b}
来源：http://pe.muxihuayi.cn

[U07] Py：反转字典键值
来源：http://lz.szxytkj.cn

{v: k for k, v in d.items()}
来源：http://pt.yuexingan06.cn

[U08] Py：展平二维列表
来源：http://cd.newstarts.cn

[y for x in nested for y in x]
来源：http://os.lnxyls.cn

[U09] Py：字典取最大值的键
来源：http://zk.nszjky.cn

max(d, key=d.get)
来源：http://gm.yuntaijiaju.cn

[U10] Py：按值排序字典
来源：http://gr.muxihuayi.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://lm.lnxyls.cn

[U11] Py：生成器表达式
来源：http://hg.shxzskj.cn

(x * 2 for x in arr)
来源：http://ys.shxzukj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://et.panjiajie.cn

Counter(arr).most_common(3)
来源：http://hi.wgjwhj.cn

[U13] Py：固定长度队列
来源：http://ro.colortex.cn

deque(maxlen=10)
来源：http://rq.hnjuh.cn

[U14] Py：分组收集到列表
来源：http://va.huixiangedu.cn

defaultdict(list)
来源：http://pt.chemitech.net.cn

[U15] Py：高精度计时
来源：http://gs.hnjuh.cn

t = time.perf_counter()
来源：http://ii.shtwfgs.cn

[U16] Py：命令行参数解析
来源：http://ky.bjjhwx.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://jo.yuntaijiaju.cn

[U17] Py：初始化日志
来源：http://fz.nszjky.cn

logging.basicConfig(level=logging.INFO)
来源：http://yb.chemitech.net.cn

[U18] Py：预编译正则
来源：http://xm.haigaiapp.cn

pat = re.compile(r"\d+")
来源：http://dm.bookmarksfly.cn

[U19] Py：正则替换带回调
来源：http://zw.hnjuh.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://su.muxihuayi.cn

[U20] Py：缓存函数结果
来源：http://to.hahajie.cn

@functools.lru_cache(maxsize=None)
来源：http://sh.huixinmuqiang.cn

[U21] Py：自定义上下文管理器
来源：http://th.szxytkj.cn

@contextlib.contextmanager
来源：http://yh.jctech888.com.cn

[U22] Py：矩阵转置
来源：http://ft.gzmigu.cn

list(zip(*m))
来源：http://fu.huixinmuqiang.cn

[U23] Py：分块读取大文件
来源：http://gj.muxihuayi.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://eg.huixinmuqiang.cn

[U24] Py：路径操作
来源：http://sx.nszjky.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://bb.chemitech.net.cn

[U25] Py：CSV 按字典读
来源：http://cj.lnxyls.cn

csv.DictReader(f)
来源：http://xx.hahajie.cn

[U26] Py：并发下载
来源：http://zw.huixinmuqiang.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://np.nszjky.cn

[U27] Py：异步 HTTP
来源：http://en.huixinmuqiang.cn

aiohttp.ClientSession() 配合 async with
来源：http://kd.chemitech.net.cn

[U28] Py：类型别名
来源：http://fp.yuntaijiaju.cn

UserId = int
来源：http://yx.shtwfgs.cn

[U29] Py：属性校验
来源：http://ds.jianghongdianzi.cn

@property 与 @x.setter 配合
来源：http://zi.nicolike.cn

[U30] Py：数据类
来源：http://rz.wgjwhj.cn

@dataclass(slots=True)
来源：http://re.hahajie.cn

[U31] Py：单测
来源：http://gj.huixinmuqiang.cn

python -m pytest -q
来源：http://ce.yuntaijiaju.cn

[U32] Py：代码格式化
来源：http://cz.wgjwhj.cn

ruff format . && ruff check --fix .
来源：http://jl.shxzukj.cn

[U33] Py：打包发布
来源：http://kd.huixinmuqiang.cn

python -m build  （依赖 pyproject.toml）
来源：http://px.panjiajie.cn

[U34] Py：判断编码
来源：http://ux.jctech888.com.cn

chardet.detect(raw)
来源：http://qy.gzmigu.cn

[U35] Py：发送邮件
来源：http://xi.hnjuh.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://sr.hnjuh.cn

[U36] Py：定时任务
来源：http://yd.jctech888.com.cn

schedule.every(10).minutes.do(job)
来源：http://yr.bookmarksfly.cn

[U37] Py：读写 Excel
来源：http://dn.huixiangedu.cn

pandas.read_excel / DataFrame.to_excel
来源：http://xm.chemitech.net.cn

[U38] Py：获取脚本所在目录
来源：http://dx.lnxyls.cn

Path(__file__).resolve().parent
来源：http://zy.huixinmuqiang.cn

[U39] Py：判断是否在交互环境
来源：http://nv.bookmarksfly.cn

sys.stdout.isatty()
来源：http://di.521024.cn

[U40] Py：打印到标准错误
来源：http://on.colortex.cn

print("err", file=sys.stderr)
来源：http://if.bjjhwx.cn

[U41] PHP：初始化 Composer 项目
来源：http://jw.hnjuh.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://gg.jctech888.com.cn

[U42] PHP：PSR-4 自动加载
来源：http://hg.haigaiapp.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ph.shtwfgs.cn

[U43] PHP：声明命名空间
来源：http://hj.lnxyls.cn

namespace App\Http;
来源：http://bq.huixiangedu.cn

[U44] PHP：开启严格类型
来源：http://zh.huixinmuqiang.cn

declare(strict_types=1);
来源：http://ne.nicolike.cn

[U45] PHP：类型声明与返回类型
来源：http://wy.shxzukj.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://fl.yuexingan06.cn

[U46] PHP：可空类型
来源：http://sq.jctech888.com.cn

?string $name = null
来源：http://sz.huanxung.cn

[U47] PHP：联合类型
来源：http://yi.yuntaijiaju.cn

int|string $id
来源：http://sj.nszjky.cn

[U48] PHP：纯枚举
来源：http://bu.newstarts.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://fq.bookmarksfly.cn


<!-- 参考信息 -->