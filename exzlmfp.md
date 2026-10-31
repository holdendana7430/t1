代发 wailian999

memset(a, 0, sizeof a);
来源：http://qt.wgjwhj.cn

[S27] C：定义常量
来源：http://qa.wgjwhj.cn

const double PI = 3.14159;
来源：http://sf.hnjuh.cn

[S28] C：静态变量
来源：http://ge.shxzskj.cn

static int counter = 0;
来源：http://pe.shtwfgs.cn

[S29] C：变参函数
来源：http://ht.bookmarksfly.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ta.nicolike.cn

[S30] C：头文件保护
来源：http://eq.9csxet.cn

#ifndef X_H
来源：http://ng.nszjky.cn

#define X_H
来源：http://zu.haigaiapp.cn

#endif
来源：http://af.jianghongdianzi.cn

[S31] C++：Hello World
来源：http://yu.9csxet.cn

#include <iostream>
来源：http://uw.hnjuh.cn

int main() { std::cout << "Hello\n"; }
来源：http://jm.muxihuayi.cn

[S32] C++：字符串
来源：http://tg.newstarts.cn

std::string s = "hi";  s += "!";
来源：http://zb.huanxung.cn

[S33] C++：vector 增删
来源：http://zh.panjiajie.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://go.shxzskj.cn

[S34] C++：遍历 vector
来源：http://ps.wgjwhj.cn

for (auto &x : v) { std::cout << x; }
来源：http://pc.shtwfgs.cn

[S35] C++：map
来源：http://oc.gzmigu.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://nh.szxytkj.cn

[S36] C++：unordered_map
来源：http://uo.hnjuh.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hr.521024.cn

[S37] C++：set
来源：http://ur.wgjwhj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://vy.shxzukj.cn

[S38] C++：排序
来源：http://dr.nicolike.cn

std::sort(v.begin(), v.end());
来源：http://ii.szxytkj.cn

[S39] C++：自定义比较器排序
来源：http://it.bookmarksfly.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ez.bjjhwx.cn

[S40] C++：查找元素
来源：http://ac.nszjky.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://uq.yuntaijiaju.cn

[S41] C++：类与构造函数
来源：http://hp.yuntaijiaju.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://gw.shxzskj.cn

[S42] C++：继承与虚函数
来源：http://st.asd995.cn

class B : public Base { public: void f() override {} };
来源：http://xb.shtwfgs.cn

[S43] C++：智能指针
来源：http://tm.colortex.cn

auto p = std::make_unique<int>(5);
来源：http://zy.nicolike.cn

[S44] C++：引用传参
来源：http://ff.huanxung.cn

void inc(int &x) { ++x; }
来源：http://ai.haigaiapp.cn

[S45] C++：lambda
来源：http://yj.muxihuayi.cn

auto add = [](int a, int b) { return a + b; };
来源：http://rx.jctech888.com.cn

[S46] C++：函数模板
来源：http://zv.yuexingan06.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://np.asd995.cn

[S47] C++：结构化绑定遍历
来源：http://tl.szsharing.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://cu.hahajie.cn

[S48] C++：逐行读文件
来源：http://ku.huixiangedu.cn

std::ifstream in("a.txt");  std::string line;
来源：http://yw.jctech888.com.cn

while (std::getline(in, line)) { }
来源：http://aq.szxytkj.cn

[S49] C++：写文件
来源：http://qs.hnjuh.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://xq.asd995.cn

[S50] C++：格式化数字
来源：http://mk.521024.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://yh.jianghongdianzi.cn

[S51] C++：显式类型转换
来源：http://qg.nicolike.cn

static_cast<double>(a) / b
来源：http://wu.colortex.cn

[S52] C++：const 与 noexcept
来源：http://mr.hnjuh.cn

int size() const noexcept { return n_; }
来源：http://mv.huixiangedu.cn

[S53] C++：移动语义
来源：http://ir.jctech888.com.cn

std::vector<int> w = std::move(v);
来源：http://bz.hnjuh.cn

[S54] C++：异常处理
来源：http://kl.bjjhwx.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ey.huixiangedu.cn

[S55] C++：结构化绑定
来源：http://uw.gzmigu.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://xn.shxzukj.cn

[S56] C++：optional
来源：http://kj.gzmigu.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://qs.yuexingan06.cn

[S57] C++：编译期常量
来源：http://qy.asd995.cn

constexpr int N = 10;
来源：http://ge.wgjwhj.cn

[S58] C++：命名空间
来源：http://zp.bjjhwx.cn

namespace ns { int f() { return 1; } }
来源：http://kr.hnjuh.cn

[S59] C++：静态断言
来源：http://hl.muxihuayi.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ya.yuexingan06.cn

[S60] C++：遍历并删除元素
来源：http://wp.nicolike.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ij.jctech888.com.cn

================================================================================
来源：http://vi.9csxet.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://bt.yuntaijiaju.cn

================================================================================
来源：http://cm.huanxung.cn

[T01] Kotlin：Hello World
来源：http://xt.hnjuh.cn

println("Hello")
来源：http://jo.szxytkj.cn

[T02] Kotlin：变量
来源：http://hh.szxytkj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://cd.hahajie.cn

[T03] Kotlin：字符串模板
来源：http://bt.nicolike.cn

"值: $b"
来源：http://fv.haigaiapp.cn

[T04] Kotlin：空安全
来源：http://qz.nszjky.cn

val n: String? = null;  n?.length
来源：http://ok.huixiangedu.cn

[T05] Kotlin：when 表达式
来源：http://vx.huixiangedu.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://bo.wgjwhj.cn

[T06] Kotlin：集合映射
来源：http://on.jctech888.com.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ia.gzmigu.cn

[T07] Kotlin：集合过滤
来源：http://ms.jctech888.com.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://no.521024.cn

[T08] Kotlin：数据类
来源：http://hb.shtwfgs.cn

data class User(val name: String, val age: Int)
来源：http://mn.521024.cn

[T09] Kotlin：扩展函数
来源：http://yl.shxzukj.cn

fun String.exclaim() = this + "!"
来源：http://rc.huixiangedu.cn

[T10] Kotlin：默认参数
来源：http://fq.chemitech.net.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://wy.jctech888.com.cn

[T11] Kotlin：协程
来源：http://ty.huixinmuqiang.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://fr.bookmarksfly.cn

[T12] Kotlin：解构声明
来源：http://cv.hnjuh.cn

val (a, b) = Pair(1, 2)
来源：http://cs.nszjky.cn

[T13] Kotlin：只读 Map
来源：http://db.521024.cn

val m = mapOf("a" to 1)
来源：http://lw.shxzukj.cn

[T14] Kotlin：循环
来源：http://wp.hahajie.cn

for (i in 1..10) println(i)
来源：http://xk.szsharing.cn

[T15] Kotlin：接口
来源：http://rh.yuntaijiaju.cn

interface Shape { fun area(): Double }
来源：http://ju.szsharing.cn

[T16] Swift：Hello World
来源：http://tv.bjjhwx.cn

print("Hello")
来源：http://nt.huixiangedu.cn

[T17] Swift：变量与常量
来源：http://hg.bjjhwx.cn

var a = 1;  let b = 2
来源：http://ls.nszjky.cn

[T18] Swift：字符串插值
来源：http://ox.szsharing.cn

"值: \(b)"
来源：http://xs.panjiajie.cn

[T19] Swift：可选绑定
来源：http://el.nszjky.cn

if let n = opt { print(n) }
来源：http://fs.bookmarksfly.cn

[T20] Swift：数组操作
来源：http://tq.hnjuh.cn

var a = [1, 2, 3];  a.append(4)
来源：http://be.nicolike.cn

[T21] Swift：遍历
来源：http://bh.jctech888.com.cn

for x in a { print(x) }
来源：http://wr.colortex.cn

[T22] Swift：字典
来源：http://sx.hahajie.cn

var d = ["a": 1];  d["b"] = 2
来源：http://vu.yuexingan06.cn

[T23] Swift：函数
来源：http://ry.bjjhwx.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://pb.jianghongdianzi.cn

[T24] Swift：闭包
来源：http://dq.wgjwhj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://sh.yuexingan06.cn

[T25] Swift：结构体
来源：http://bq.bjjhwx.cn

struct P { var x: Int }
来源：http://iy.bookmarksfly.cn

[T26] Swift：类与重写
来源：http://ys.haigaiapp.cn

class A: Base { override func f() {} }
来源：http://uj.huanxung.cn

[T27] Swift：错误处理
来源：http://sd.szsharing.cn

do { try f() } catch { print(error) }
来源：http://dm.szxytkj.cn

[T28] Swift：枚举
来源：http://nv.521024.cn

enum Color { case red, green }
来源：http://wj.9csxet.cn

[T29] Swift：guard 提前返回
来源：http://dc.huixiangedu.cn

guard let x = opt else { return }
来源：http://bo.newstarts.cn

[T30] Swift：协议
来源：http://zh.chemitech.net.cn

protocol Shape { func area() -> Double }
来源：http://gc.szxytkj.cn

[T31] Lua：Hello World
来源：http://nu.bookmarksfly.cn

print("Hello")
来源：http://xu.shxzukj.cn

[T32] Lua：局部变量
来源：http://yj.wgjwhj.cn

local a = 1
来源：http://ex.jctech888.com.cn

[T33] Lua：表（数组）
来源：http://cp.bookmarksfly.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://xj.bookmarksfly.cn

[T34] Lua：遍历表
来源：http://ev.yuexingan06.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://pi.shxzukj.cn

[T35] Lua：字典表
来源：http://zz.bjjhwx.cn

local d = { a = 1 };  d.b = 2
来源：http://xf.huixiangedu.cn

[T36] Lua：函数
来源：http://fj.panjiajie.cn

function add(a, b) return a + b end
来源：http://oa.shxzskj.cn

[T37] Lua：字符串拼接
来源：http://ct.colortex.cn

"a" .. "b"
来源：http://et.szsharing.cn

[T38] Lua：条件
来源：http://hc.colortex.cn

if x > 0 then print("正") end
来源：http://ct.521024.cn

[T39] Lua：模式匹配
来源：http://gp.hnjuh.cn

string.find(s, "%d+")
来源：http://tg.bjjhwx.cn

[T40] Lua：元表
来源：http://fr.szsharing.cn

setmetatable({}, { __index = base })
来源：http://ht.colortex.cn

[T41] Perl：Hello World
来源：http://hu.muxihuayi.cn

print "Hello\n";
来源：http://jo.lnxyls.cn

[T42] Perl：变量类型
来源：http://qb.521024.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://oj.nszjky.cn

[T43] Perl：字符串插值
来源：http://jd.bookmarksfly.cn

"值: $a"
来源：http://bx.shtwfgs.cn

[T44] Perl：条件
来源：http://sv.bookmarksfly.cn

if ($a > 0) { print "正"; }
来源：http://pg.wgjwhj.cn

[T45] Perl：数组遍历
来源：http://ib.hahajie.cn

for my $x (@arr) { print $x; }
来源：http://im.hahajie.cn

[T46] Perl：哈希操作
来源：http://ja.colortex.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wk.jctech888.com.cn

[T47] Perl：正则捕获
来源：http://wr.panjiajie.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ho.shtwfgs.cn

[T48] Perl：正则替换
来源：http://lf.newstarts.cn

$s =~ s/old/new/g;
来源：http://zk.colortex.cn

[T49] Perl：函数
来源：http://py.newstarts.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://rl.szxytkj.cn

[T50] Perl：逐行读文件
来源：http://da.bjjhwx.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ks.shxzukj.cn

while (my $line = <$fh>) { print $line; }
来源：http://mk.hnjuh.cn

[T51] Scala：Hello World
来源：http://yb.shtwfgs.cn

println("Hello")
来源：http://mc.huixiangedu.cn

[T52] Scala：变量
来源：http://cb.shxzskj.cn

val a = 1;  var b = 2
来源：http://kx.nicolike.cn

[T53] Scala：字符串插值
来源：http://ke.bjjhwx.cn

s"值: $b"
来源：http://ch.bjjhwx.cn

[T54] Scala：集合映射
来源：http://st.muxihuayi.cn

List(1, 2, 3).map(_ * 2)
来源：http://xi.chemitech.net.cn

[T55] Scala：集合过滤
来源：http://zv.panjiajie.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ru.asd995.cn

[T56] Scala：样例类
来源：http://tw.jctech888.com.cn

case class User(name: String, age: Int)
来源：http://xt.panjiajie.cn

[T57] Scala：模式匹配
来源：http://hl.newstarts.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ec.lnxyls.cn

[T58] Scala：函数定义
来源：http://ix.colortex.cn

def add(a: Int, b: Int): Int = a + b
来源：http://kn.shxzukj.cn

[T59] Scala：循环
来源：http://kk.huixiangedu.cn

for (i <- 1 to 10) println(i)
来源：http://wp.panjiajie.cn

[T60] Scala：折叠
来源：http://ff.bookmarksfly.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://wx.huanxung.cn

================================================================================
来源：http://be.colortex.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://im.yuntaijiaju.cn

================================================================================
来源：http://ja.jctech888.com.cn

[U01] Py：创建虚拟环境
来源：http://wf.yuntaijiaju.cn

python -m venv .venv && source .venv/bin/activate
来源：http://uq.jctech888.com.cn

[U02] Py：导出 / 安装依赖
来源：http://vg.colortex.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://zc.huanxung.cn

[U03] Py：加载 .env 配置
来源：http://fi.huanxung.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://oy.nszjky.cn

[U04] Py：变量调试打印
来源：http://qn.shtwfgs.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://li.shtwfgs.cn

[U05] Py：列表去重且保序
来源：http://fw.shxzskj.cn

list(dict.fromkeys(arr))
来源：http://jl.huixinmuqiang.cn

[U06] Py：合并两个字典
来源：http://su.huanxung.cn

{**a, **b}
来源：http://bq.huixiangedu.cn

[U07] Py：反转字典键值
来源：http://fd.colortex.cn

{v: k for k, v in d.items()}
来源：http://cc.nicolike.cn

[U08] Py：展平二维列表
来源：http://ow.gzmigu.cn

[y for x in nested for y in x]
来源：http://ca.yuexingan06.cn

[U09] Py：字典取最大值的键
来源：http://on.jianghongdianzi.cn

max(d, key=d.get)
来源：http://qx.haigaiapp.cn

[U10] Py：按值排序字典
来源：http://pc.huixiangedu.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://qu.huixinmuqiang.cn

[U11] Py：生成器表达式
来源：http://zs.shxzukj.cn

(x * 2 for x in arr)
来源：http://tx.nszjky.cn

[U12] Py：取出现最多的 3 个元素
来源：http://mw.hahajie.cn

Counter(arr).most_common(3)
来源：http://sn.huanxung.cn

[U13] Py：固定长度队列
来源：http://if.haigaiapp.cn

deque(maxlen=10)
来源：http://vu.huanxung.cn

[U14] Py：分组收集到列表
来源：http://wh.huanxung.cn

defaultdict(list)
来源：http://om.huanxung.cn

[U15] Py：高精度计时
来源：http://su.bookmarksfly.cn

t = time.perf_counter()
来源：http://uh.asd995.cn

[U16] Py：命令行参数解析
来源：http://le.colortex.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://np.muxihuayi.cn

[U17] Py：初始化日志
来源：http://uu.shxzskj.cn

logging.basicConfig(level=logging.INFO)
来源：http://st.nicolike.cn

[U18] Py：预编译正则
来源：http://dd.huixinmuqiang.cn

pat = re.compile(r"\d+")
来源：http://va.lnxyls.cn

[U19] Py：正则替换带回调
来源：http://jh.shxzskj.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://or.asd995.cn

[U20] Py：缓存函数结果
来源：http://vn.hnjuh.cn

@functools.lru_cache(maxsize=None)
来源：http://jm.gzmigu.cn

[U21] Py：自定义上下文管理器
来源：http://st.yuexingan06.cn

@contextlib.contextmanager
来源：http://zr.shxzskj.cn

[U22] Py：矩阵转置
来源：http://yp.haigaiapp.cn

list(zip(*m))
来源：http://pq.hahajie.cn

[U23] Py：分块读取大文件
来源：http://eh.szxytkj.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://gr.nicolike.cn

[U24] Py：路径操作
来源：http://ew.521024.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://yc.colortex.cn

[U25] Py：CSV 按字典读
来源：http://wn.huixinmuqiang.cn

csv.DictReader(f)
来源：http://fj.huanxung.cn

[U26] Py：并发下载
来源：http://um.nszjky.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://vn.jctech888.com.cn

[U27] Py：异步 HTTP
来源：http://qa.hnjuh.cn

aiohttp.ClientSession() 配合 async with
来源：http://ul.9csxet.cn

[U28] Py：类型别名
来源：http://et.colortex.cn

UserId = int
来源：http://pl.shtwfgs.cn

[U29] Py：属性校验
来源：http://ub.shtwfgs.cn

@property 与 @x.setter 配合
来源：http://tc.hahajie.cn

[U30] Py：数据类
来源：http://qf.wgjwhj.cn

@dataclass(slots=True)
来源：http://pb.panjiajie.cn

[U31] Py：单测
来源：http://jw.jianghongdianzi.cn

python -m pytest -q
来源：http://uc.yuntaijiaju.cn

[U32] Py：代码格式化
来源：http://zw.yuexingan06.cn

ruff format . && ruff check --fix .
来源：http://xt.9csxet.cn

[U33] Py：打包发布
来源：http://yk.shtwfgs.cn

python -m build  （依赖 pyproject.toml）
来源：http://ap.chemitech.net.cn

[U34] Py：判断编码
来源：http://xv.gzmigu.cn

chardet.detect(raw)
来源：http://js.shxzukj.cn

[U35] Py：发送邮件
来源：http://tr.colortex.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ml.huixinmuqiang.cn

[U36] Py：定时任务
来源：http://ua.yuntaijiaju.cn

schedule.every(10).minutes.do(job)
来源：http://dq.9csxet.cn

[U37] Py：读写 Excel
来源：http://qo.hahajie.cn

pandas.read_excel / DataFrame.to_excel
来源：http://qx.szsharing.cn

[U38] Py：获取脚本所在目录
来源：http://wg.9csxet.cn

Path(__file__).resolve().parent
来源：http://ab.szsharing.cn

[U39] Py：判断是否在交互环境
来源：http://lh.shxzskj.cn

sys.stdout.isatty()
来源：http://zf.jctech888.com.cn

[U40] Py：打印到标准错误
来源：http://ns.9csxet.cn

print("err", file=sys.stderr)
来源：http://kq.yuntaijiaju.cn

[U41] PHP：初始化 Composer 项目
来源：http://kl.lnxyls.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://fq.521024.cn

[U42] PHP：PSR-4 自动加载
来源：http://bo.bjjhwx.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://zk.shxzukj.cn

[U43] PHP：声明命名空间
来源：http://jz.huixinmuqiang.cn

namespace App\Http;
来源：http://rx.huixiangedu.cn

[U44] PHP：开启严格类型
来源：http://bl.521024.cn

declare(strict_types=1);
来源：http://jj.hnjuh.cn

[U45] PHP：类型声明与返回类型
来源：http://uc.521024.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://db.lnxyls.cn

[U46] PHP：可空类型
来源：http://jb.nszjky.cn

?string $name = null
来源：http://zy.lnxyls.cn

[U47] PHP：联合类型
来源：http://co.szxytkj.cn

int|string $id
来源：http://mc.chemitech.net.cn

[U48] PHP：纯枚举
来源：http://tz.hahajie.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://my.newstarts.cn

[U49] PHP：只读属性
来源：http://dk.yuntaijiaju.cn

public readonly string $name
来源：http://at.huixiangedu.cn

[U50] PHP：构造器属性提升
来源：http://fw.shxzukj.cn

public function __construct(private int $id) {}
来源：http://nu.shxzukj.cn


<!-- 参考信息 -->