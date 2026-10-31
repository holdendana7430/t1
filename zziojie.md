代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ka.9csxet.cn

[S25] C：内存拷贝
来源：http://gz.panjiajie.cn

memcpy(dst, src, n);
来源：http://kf.jctech888.com.cn

[S26] C：内存清零
来源：http://bz.hnjuh.cn

memset(a, 0, sizeof a);
来源：http://vn.521024.cn

[S27] C：定义常量
来源：http://zq.huixiangedu.cn

const double PI = 3.14159;
来源：http://ep.huixinmuqiang.cn

[S28] C：静态变量
来源：http://hl.nicolike.cn

static int counter = 0;
来源：http://wq.chemitech.net.cn

[S29] C：变参函数
来源：http://hd.chemitech.net.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://up.shxzukj.cn

[S30] C：头文件保护
来源：http://eb.jianghongdianzi.cn

#ifndef X_H
来源：http://vw.hahajie.cn

#define X_H
来源：http://pa.jctech888.com.cn

#endif
来源：http://qg.lnxyls.cn

[S31] C++：Hello World
来源：http://wa.huanxung.cn

#include <iostream>
来源：http://ru.wgjwhj.cn

int main() { std::cout << "Hello\n"; }
来源：http://tp.bjjhwx.cn

[S32] C++：字符串
来源：http://bk.szxytkj.cn

std::string s = "hi";  s += "!";
来源：http://ib.jianghongdianzi.cn

[S33] C++：vector 增删
来源：http://nu.lnxyls.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ep.jctech888.com.cn

[S34] C++：遍历 vector
来源：http://do.gzmigu.cn

for (auto &x : v) { std::cout << x; }
来源：http://uo.bjjhwx.cn

[S35] C++：map
来源：http://xt.gzmigu.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://fx.gzmigu.cn

[S36] C++：unordered_map
来源：http://jp.jctech888.com.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://fq.hnjuh.cn

[S37] C++：set
来源：http://mx.nicolike.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://dx.gzmigu.cn

[S38] C++：排序
来源：http://cm.szsharing.cn

std::sort(v.begin(), v.end());
来源：http://ju.asd995.cn

[S39] C++：自定义比较器排序
来源：http://qc.nszjky.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://uo.bookmarksfly.cn

[S40] C++：查找元素
来源：http://ar.bjjhwx.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ly.bjjhwx.cn

[S41] C++：类与构造函数
来源：http://nu.521024.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://jh.hnjuh.cn

[S42] C++：继承与虚函数
来源：http://uc.nszjky.cn

class B : public Base { public: void f() override {} };
来源：http://iv.szxytkj.cn

[S43] C++：智能指针
来源：http://by.colortex.cn

auto p = std::make_unique<int>(5);
来源：http://ox.nicolike.cn

[S44] C++：引用传参
来源：http://du.huixiangedu.cn

void inc(int &x) { ++x; }
来源：http://bp.nicolike.cn

[S45] C++：lambda
来源：http://tn.shtwfgs.cn

auto add = [](int a, int b) { return a + b; };
来源：http://by.hnjuh.cn

[S46] C++：函数模板
来源：http://hk.szsharing.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://oo.bookmarksfly.cn

[S47] C++：结构化绑定遍历
来源：http://ry.muxihuayi.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ls.huixinmuqiang.cn

[S48] C++：逐行读文件
来源：http://cc.panjiajie.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ez.bjjhwx.cn

while (std::getline(in, line)) { }
来源：http://sc.huanxung.cn

[S49] C++：写文件
来源：http://kz.shxzukj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://sl.szxytkj.cn

[S50] C++：格式化数字
来源：http://id.newstarts.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://df.huixinmuqiang.cn

[S51] C++：显式类型转换
来源：http://bd.shtwfgs.cn

static_cast<double>(a) / b
来源：http://df.huixinmuqiang.cn

[S52] C++：const 与 noexcept
来源：http://kj.bjjhwx.cn

int size() const noexcept { return n_; }
来源：http://dj.wgjwhj.cn

[S53] C++：移动语义
来源：http://mh.colortex.cn

std::vector<int> w = std::move(v);
来源：http://za.yuexingan06.cn

[S54] C++：异常处理
来源：http://km.asd995.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://dz.szxytkj.cn

[S55] C++：结构化绑定
来源：http://nm.jianghongdianzi.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ta.newstarts.cn

[S56] C++：optional
来源：http://ky.yuexingan06.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mh.gzmigu.cn

[S57] C++：编译期常量
来源：http://iv.szsharing.cn

constexpr int N = 10;
来源：http://rc.jctech888.com.cn

[S58] C++：命名空间
来源：http://hm.shtwfgs.cn

namespace ns { int f() { return 1; } }
来源：http://ff.gzmigu.cn

[S59] C++：静态断言
来源：http://uz.huixinmuqiang.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://eo.huixiangedu.cn

[S60] C++：遍历并删除元素
来源：http://nw.newstarts.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hj.haigaiapp.cn

================================================================================
来源：http://ai.yuexingan06.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hr.9csxet.cn

================================================================================
来源：http://rk.huanxung.cn

[T01] Kotlin：Hello World
来源：http://uu.yuntaijiaju.cn

println("Hello")
来源：http://dy.colortex.cn

[T02] Kotlin：变量
来源：http://fx.haigaiapp.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://px.wgjwhj.cn

[T03] Kotlin：字符串模板
来源：http://kn.huanxung.cn

"值: $b"
来源：http://au.jianghongdianzi.cn

[T04] Kotlin：空安全
来源：http://xj.jctech888.com.cn

val n: String? = null;  n?.length
来源：http://rd.panjiajie.cn

[T05] Kotlin：when 表达式
来源：http://xi.haigaiapp.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ao.jianghongdianzi.cn

[T06] Kotlin：集合映射
来源：http://ys.nszjky.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://kj.colortex.cn

[T07] Kotlin：集合过滤
来源：http://gk.chemitech.net.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://cu.shtwfgs.cn

[T08] Kotlin：数据类
来源：http://vc.asd995.cn

data class User(val name: String, val age: Int)
来源：http://lt.haigaiapp.cn

[T09] Kotlin：扩展函数
来源：http://nd.panjiajie.cn

fun String.exclaim() = this + "!"
来源：http://rb.yuntaijiaju.cn

[T10] Kotlin：默认参数
来源：http://de.huanxung.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://um.huanxung.cn

[T11] Kotlin：协程
来源：http://zx.shxzskj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ig.wgjwhj.cn

[T12] Kotlin：解构声明
来源：http://qw.nszjky.cn

val (a, b) = Pair(1, 2)
来源：http://ys.bookmarksfly.cn

[T13] Kotlin：只读 Map
来源：http://ip.colortex.cn

val m = mapOf("a" to 1)
来源：http://ac.huanxung.cn

[T14] Kotlin：循环
来源：http://jo.bookmarksfly.cn

for (i in 1..10) println(i)
来源：http://ag.bjjhwx.cn

[T15] Kotlin：接口
来源：http://uj.nicolike.cn

interface Shape { fun area(): Double }
来源：http://xy.colortex.cn

[T16] Swift：Hello World
来源：http://nu.jianghongdianzi.cn

print("Hello")
来源：http://wt.jianghongdianzi.cn

[T17] Swift：变量与常量
来源：http://rw.shxzskj.cn

var a = 1;  let b = 2
来源：http://nu.muxihuayi.cn

[T18] Swift：字符串插值
来源：http://jj.521024.cn

"值: \(b)"
来源：http://oh.colortex.cn

[T19] Swift：可选绑定
来源：http://sg.lnxyls.cn

if let n = opt { print(n) }
来源：http://mv.muxihuayi.cn

[T20] Swift：数组操作
来源：http://du.hnjuh.cn

var a = [1, 2, 3];  a.append(4)
来源：http://se.jianghongdianzi.cn

[T21] Swift：遍历
来源：http://rh.yuntaijiaju.cn

for x in a { print(x) }
来源：http://mx.huanxung.cn

[T22] Swift：字典
来源：http://oh.shxzskj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://oc.shxzskj.cn

[T23] Swift：函数
来源：http://yv.hnjuh.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://xs.huixiangedu.cn

[T24] Swift：闭包
来源：http://ih.muxihuayi.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://dc.huixinmuqiang.cn

[T25] Swift：结构体
来源：http://ak.nszjky.cn

struct P { var x: Int }
来源：http://kc.bookmarksfly.cn

[T26] Swift：类与重写
来源：http://up.shxzskj.cn

class A: Base { override func f() {} }
来源：http://yc.jctech888.com.cn

[T27] Swift：错误处理
来源：http://by.jctech888.com.cn

do { try f() } catch { print(error) }
来源：http://pj.nszjky.cn

[T28] Swift：枚举
来源：http://gi.huixinmuqiang.cn

enum Color { case red, green }
来源：http://be.panjiajie.cn

[T29] Swift：guard 提前返回
来源：http://op.bookmarksfly.cn

guard let x = opt else { return }
来源：http://bw.hahajie.cn

[T30] Swift：协议
来源：http://vz.shxzukj.cn

protocol Shape { func area() -> Double }
来源：http://oo.chemitech.net.cn

[T31] Lua：Hello World
来源：http://pu.yuntaijiaju.cn

print("Hello")
来源：http://rn.jctech888.com.cn

[T32] Lua：局部变量
来源：http://yk.wgjwhj.cn

local a = 1
来源：http://qg.newstarts.cn

[T33] Lua：表（数组）
来源：http://qm.huanxung.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://qi.huanxung.cn

[T34] Lua：遍历表
来源：http://jq.bookmarksfly.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://yt.huanxung.cn

[T35] Lua：字典表
来源：http://wh.lnxyls.cn

local d = { a = 1 };  d.b = 2
来源：http://nw.bookmarksfly.cn

[T36] Lua：函数
来源：http://td.nszjky.cn

function add(a, b) return a + b end
来源：http://fj.colortex.cn

[T37] Lua：字符串拼接
来源：http://uz.wgjwhj.cn

"a" .. "b"
来源：http://bh.szxytkj.cn

[T38] Lua：条件
来源：http://ap.hnjuh.cn

if x > 0 then print("正") end
来源：http://ew.jianghongdianzi.cn

[T39] Lua：模式匹配
来源：http://wt.huixiangedu.cn

string.find(s, "%d+")
来源：http://qr.hahajie.cn

[T40] Lua：元表
来源：http://gs.hahajie.cn

setmetatable({}, { __index = base })
来源：http://hm.haigaiapp.cn

[T41] Perl：Hello World
来源：http://ct.colortex.cn

print "Hello\n";
来源：http://nb.haigaiapp.cn

[T42] Perl：变量类型
来源：http://xr.szxytkj.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://oc.nicolike.cn

[T43] Perl：字符串插值
来源：http://hi.nicolike.cn

"值: $a"
来源：http://vk.haigaiapp.cn

[T44] Perl：条件
来源：http://vx.yuexingan06.cn

if ($a > 0) { print "正"; }
来源：http://ra.huixiangedu.cn

[T45] Perl：数组遍历
来源：http://og.huixiangedu.cn

for my $x (@arr) { print $x; }
来源：http://xk.9csxet.cn

[T46] Perl：哈希操作
来源：http://oa.nicolike.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://yp.bjjhwx.cn

[T47] Perl：正则捕获
来源：http://ct.colortex.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://hq.521024.cn

[T48] Perl：正则替换
来源：http://un.hnjuh.cn

$s =~ s/old/new/g;
来源：http://no.nicolike.cn

[T49] Perl：函数
来源：http://mt.colortex.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://gs.colortex.cn

[T50] Perl：逐行读文件
来源：http://jn.huanxung.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://eq.shtwfgs.cn

while (my $line = <$fh>) { print $line; }
来源：http://wr.jctech888.com.cn

[T51] Scala：Hello World
来源：http://pn.shxzukj.cn

println("Hello")
来源：http://cy.lnxyls.cn

[T52] Scala：变量
来源：http://tp.huanxung.cn

val a = 1;  var b = 2
来源：http://kr.nicolike.cn

[T53] Scala：字符串插值
来源：http://uz.bjjhwx.cn

s"值: $b"
来源：http://ug.wgjwhj.cn

[T54] Scala：集合映射
来源：http://eg.9csxet.cn

List(1, 2, 3).map(_ * 2)
来源：http://iv.jianghongdianzi.cn

[T55] Scala：集合过滤
来源：http://mm.lnxyls.cn

List(1, 2, 3).filter(_ > 1)
来源：http://tl.gzmigu.cn

[T56] Scala：样例类
来源：http://ja.nicolike.cn

case class User(name: String, age: Int)
来源：http://kk.shxzskj.cn

[T57] Scala：模式匹配
来源：http://lp.nicolike.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://tf.huanxung.cn

[T58] Scala：函数定义
来源：http://zl.colortex.cn

def add(a: Int, b: Int): Int = a + b
来源：http://tl.newstarts.cn

[T59] Scala：循环
来源：http://mp.jctech888.com.cn

for (i <- 1 to 10) println(i)
来源：http://wh.chemitech.net.cn

[T60] Scala：折叠
来源：http://hf.colortex.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://qx.panjiajie.cn

================================================================================
来源：http://us.bjjhwx.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://uj.shxzskj.cn

================================================================================
来源：http://fm.chemitech.net.cn

[U01] Py：创建虚拟环境
来源：http://qf.shxzukj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://of.jctech888.com.cn

[U02] Py：导出 / 安装依赖
来源：http://tt.muxihuayi.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://ue.panjiajie.cn

[U03] Py：加载 .env 配置
来源：http://ud.panjiajie.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://dg.bookmarksfly.cn

[U04] Py：变量调试打印
来源：http://ok.shtwfgs.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://zf.wgjwhj.cn

[U05] Py：列表去重且保序
来源：http://gu.chemitech.net.cn

list(dict.fromkeys(arr))
来源：http://iu.521024.cn

[U06] Py：合并两个字典
来源：http://lv.huanxung.cn

{**a, **b}
来源：http://lr.huixiangedu.cn

[U07] Py：反转字典键值
来源：http://od.shxzskj.cn

{v: k for k, v in d.items()}
来源：http://cq.521024.cn

[U08] Py：展平二维列表
来源：http://hj.chemitech.net.cn

[y for x in nested for y in x]
来源：http://gw.wgjwhj.cn

[U09] Py：字典取最大值的键
来源：http://md.521024.cn

max(d, key=d.get)
来源：http://ou.panjiajie.cn

[U10] Py：按值排序字典
来源：http://ab.shtwfgs.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://kd.shxzukj.cn

[U11] Py：生成器表达式
来源：http://qv.bookmarksfly.cn

(x * 2 for x in arr)
来源：http://ge.bookmarksfly.cn

[U12] Py：取出现最多的 3 个元素
来源：http://ub.newstarts.cn

Counter(arr).most_common(3)
来源：http://wt.huanxung.cn

[U13] Py：固定长度队列
来源：http://il.hnjuh.cn

deque(maxlen=10)
来源：http://qo.shxzskj.cn

[U14] Py：分组收集到列表
来源：http://hx.szxytkj.cn

defaultdict(list)
来源：http://qw.huixiangedu.cn

[U15] Py：高精度计时
来源：http://ke.bookmarksfly.cn

t = time.perf_counter()
来源：http://do.chemitech.net.cn

[U16] Py：命令行参数解析
来源：http://hn.bjjhwx.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://de.hahajie.cn

[U17] Py：初始化日志
来源：http://vp.wgjwhj.cn

logging.basicConfig(level=logging.INFO)
来源：http://mc.wgjwhj.cn

[U18] Py：预编译正则
来源：http://tp.szsharing.cn

pat = re.compile(r"\d+")
来源：http://gp.panjiajie.cn

[U19] Py：正则替换带回调
来源：http://eh.lnxyls.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://dp.szsharing.cn

[U20] Py：缓存函数结果
来源：http://dm.bjjhwx.cn

@functools.lru_cache(maxsize=None)
来源：http://em.hahajie.cn

[U21] Py：自定义上下文管理器
来源：http://qv.jctech888.com.cn

@contextlib.contextmanager
来源：http://nz.shxzskj.cn

[U22] Py：矩阵转置
来源：http://er.szsharing.cn

list(zip(*m))
来源：http://cy.521024.cn

[U23] Py：分块读取大文件
来源：http://xl.asd995.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://yn.hahajie.cn

[U24] Py：路径操作
来源：http://tq.shxzskj.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://vp.lnxyls.cn

[U25] Py：CSV 按字典读
来源：http://cu.huixinmuqiang.cn

csv.DictReader(f)
来源：http://ly.yuexingan06.cn

[U26] Py：并发下载
来源：http://ds.haigaiapp.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://gu.gzmigu.cn

[U27] Py：异步 HTTP
来源：http://fe.shxzskj.cn

aiohttp.ClientSession() 配合 async with
来源：http://lc.panjiajie.cn

[U28] Py：类型别名
来源：http://hl.huixiangedu.cn

UserId = int
来源：http://nb.9csxet.cn

[U29] Py：属性校验
来源：http://ov.szsharing.cn

@property 与 @x.setter 配合
来源：http://qa.nszjky.cn

[U30] Py：数据类
来源：http://ry.shxzukj.cn

@dataclass(slots=True)
来源：http://pe.newstarts.cn

[U31] Py：单测
来源：http://sp.bookmarksfly.cn

python -m pytest -q
来源：http://ir.huixinmuqiang.cn

[U32] Py：代码格式化
来源：http://av.shxzskj.cn

ruff format . && ruff check --fix .
来源：http://zs.bjjhwx.cn

[U33] Py：打包发布
来源：http://ed.521024.cn

python -m build  （依赖 pyproject.toml）
来源：http://ht.asd995.cn

[U34] Py：判断编码
来源：http://ys.haigaiapp.cn

chardet.detect(raw)
来源：http://qi.jianghongdianzi.cn

[U35] Py：发送邮件
来源：http://hd.jctech888.com.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://su.colortex.cn

[U36] Py：定时任务
来源：http://cs.colortex.cn

schedule.every(10).minutes.do(job)
来源：http://oq.bjjhwx.cn

[U37] Py：读写 Excel
来源：http://rd.yuntaijiaju.cn

pandas.read_excel / DataFrame.to_excel
来源：http://av.newstarts.cn

[U38] Py：获取脚本所在目录
来源：http://bs.hahajie.cn

Path(__file__).resolve().parent
来源：http://ip.shxzukj.cn

[U39] Py：判断是否在交互环境
来源：http://ii.haigaiapp.cn

sys.stdout.isatty()
来源：http://fb.hnjuh.cn

[U40] Py：打印到标准错误
来源：http://ym.521024.cn

print("err", file=sys.stderr)
来源：http://mc.yuexingan06.cn

[U41] PHP：初始化 Composer 项目
来源：http://qr.lnxyls.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://mx.gzmigu.cn

[U42] PHP：PSR-4 自动加载
来源：http://fi.jctech888.com.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://od.chemitech.net.cn

[U43] PHP：声明命名空间
来源：http://gn.9csxet.cn

namespace App\Http;
来源：http://ze.gzmigu.cn

[U44] PHP：开启严格类型
来源：http://ty.shxzskj.cn

declare(strict_types=1);
来源：http://zp.9csxet.cn

[U45] PHP：类型声明与返回类型
来源：http://la.huanxung.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://pb.shtwfgs.cn

[U46] PHP：可空类型
来源：http://nx.chemitech.net.cn

?string $name = null
来源：http://dy.panjiajie.cn

[U47] PHP：联合类型
来源：http://gc.panjiajie.cn

int|string $id
来源：http://fe.wgjwhj.cn

[U48] PHP：纯枚举
来源：http://fb.nszjky.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://cm.gzmigu.cn


<!-- 参考信息 -->