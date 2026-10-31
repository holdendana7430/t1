代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://zq.hahajie.cn

[S21] C：字符类别判断
来源：http://vq.yuntaijiaju.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ei.huixinmuqiang.cn

[S22] C：字符串转数字
来源：http://pr.newstarts.cn

atoi("42");  strtod("3.14", NULL);
来源：http://lg.newstarts.cn

[S23] C：随机数
来源：http://vb.wgjwhj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://fw.shtwfgs.cn

[S24] C：获取本地时间
来源：http://ie.shxzukj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ki.lnxyls.cn

[S25] C：内存拷贝
来源：http://wm.bjjhwx.cn

memcpy(dst, src, n);
来源：http://bg.huixiangedu.cn

[S26] C：内存清零
来源：http://aj.panjiajie.cn

memset(a, 0, sizeof a);
来源：http://ty.huixinmuqiang.cn

[S27] C：定义常量
来源：http://us.hahajie.cn

const double PI = 3.14159;
来源：http://yy.jianghongdianzi.cn

[S28] C：静态变量
来源：http://tr.szsharing.cn

static int counter = 0;
来源：http://qj.huixinmuqiang.cn

[S29] C：变参函数
来源：http://sv.nszjky.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ch.yuexingan06.cn

[S30] C：头文件保护
来源：http://ym.521024.cn

#ifndef X_H
来源：http://ih.nszjky.cn

#define X_H
来源：http://fp.jctech888.com.cn

#endif
来源：http://qh.shxzskj.cn

[S31] C++：Hello World
来源：http://dr.hahajie.cn

#include <iostream>
来源：http://ep.hahajie.cn

int main() { std::cout << "Hello\n"; }
来源：http://im.nszjky.cn

[S32] C++：字符串
来源：http://rt.yuexingan06.cn

std::string s = "hi";  s += "!";
来源：http://fj.chemitech.net.cn

[S33] C++：vector 增删
来源：http://xx.jianghongdianzi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://vi.hnjuh.cn

[S34] C++：遍历 vector
来源：http://fa.hnjuh.cn

for (auto &x : v) { std::cout << x; }
来源：http://rf.panjiajie.cn

[S35] C++：map
来源：http://ke.huixiangedu.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://oj.huixinmuqiang.cn

[S36] C++：unordered_map
来源：http://bq.bjjhwx.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ly.nicolike.cn

[S37] C++：set
来源：http://ix.hnjuh.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://dg.colortex.cn

[S38] C++：排序
来源：http://si.huixiangedu.cn

std::sort(v.begin(), v.end());
来源：http://ni.asd995.cn

[S39] C++：自定义比较器排序
来源：http://sk.huixinmuqiang.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://vo.muxihuayi.cn

[S40] C++：查找元素
来源：http://ep.shxzskj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ch.szxytkj.cn

[S41] C++：类与构造函数
来源：http://cw.shxzukj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://sx.szsharing.cn

[S42] C++：继承与虚函数
来源：http://ew.shxzskj.cn

class B : public Base { public: void f() override {} };
来源：http://gg.9csxet.cn

[S43] C++：智能指针
来源：http://iz.lnxyls.cn

auto p = std::make_unique<int>(5);
来源：http://kb.huanxung.cn

[S44] C++：引用传参
来源：http://qw.nicolike.cn

void inc(int &x) { ++x; }
来源：http://cp.panjiajie.cn

[S45] C++：lambda
来源：http://fc.lnxyls.cn

auto add = [](int a, int b) { return a + b; };
来源：http://cd.lnxyls.cn

[S46] C++：函数模板
来源：http://ca.lnxyls.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ws.jianghongdianzi.cn

[S47] C++：结构化绑定遍历
来源：http://fq.9csxet.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://gr.shtwfgs.cn

[S48] C++：逐行读文件
来源：http://cl.wgjwhj.cn

std::ifstream in("a.txt");  std::string line;
来源：http://dv.yuntaijiaju.cn

while (std::getline(in, line)) { }
来源：http://na.bookmarksfly.cn

[S49] C++：写文件
来源：http://yl.newstarts.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://xb.huanxung.cn

[S50] C++：格式化数字
来源：http://sd.yuntaijiaju.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://py.nszjky.cn

[S51] C++：显式类型转换
来源：http://es.panjiajie.cn

static_cast<double>(a) / b
来源：http://ub.gzmigu.cn

[S52] C++：const 与 noexcept
来源：http://oh.shxzukj.cn

int size() const noexcept { return n_; }
来源：http://pf.asd995.cn

[S53] C++：移动语义
来源：http://em.gzmigu.cn

std::vector<int> w = std::move(v);
来源：http://kt.bjjhwx.cn

[S54] C++：异常处理
来源：http://af.newstarts.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://je.muxihuayi.cn

[S55] C++：结构化绑定
来源：http://wi.jctech888.com.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://tg.szsharing.cn

[S56] C++：optional
来源：http://yu.panjiajie.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://lu.521024.cn

[S57] C++：编译期常量
来源：http://tl.shtwfgs.cn

constexpr int N = 10;
来源：http://id.panjiajie.cn

[S58] C++：命名空间
来源：http://aa.asd995.cn

namespace ns { int f() { return 1; } }
来源：http://hb.jianghongdianzi.cn

[S59] C++：静态断言
来源：http://ia.9csxet.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://gl.shxzukj.cn

[S60] C++：遍历并删除元素
来源：http://kr.hnjuh.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://vr.nicolike.cn

================================================================================
来源：http://ff.yuntaijiaju.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://eo.bookmarksfly.cn

================================================================================
来源：http://ae.shxzukj.cn

[T01] Kotlin：Hello World
来源：http://kh.asd995.cn

println("Hello")
来源：http://ei.jctech888.com.cn

[T02] Kotlin：变量
来源：http://ix.jianghongdianzi.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://xo.huanxung.cn

[T03] Kotlin：字符串模板
来源：http://eg.haigaiapp.cn

"值: $b"
来源：http://fd.huixiangedu.cn

[T04] Kotlin：空安全
来源：http://ic.shxzskj.cn

val n: String? = null;  n?.length
来源：http://my.muxihuayi.cn

[T05] Kotlin：when 表达式
来源：http://ev.hnjuh.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://sv.bjjhwx.cn

[T06] Kotlin：集合映射
来源：http://sk.shxzukj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://cz.asd995.cn

[T07] Kotlin：集合过滤
来源：http://oj.shtwfgs.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://wo.chemitech.net.cn

[T08] Kotlin：数据类
来源：http://np.haigaiapp.cn

data class User(val name: String, val age: Int)
来源：http://bj.bookmarksfly.cn

[T09] Kotlin：扩展函数
来源：http://bl.bjjhwx.cn

fun String.exclaim() = this + "!"
来源：http://zd.huanxung.cn

[T10] Kotlin：默认参数
来源：http://rm.chemitech.net.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ee.bookmarksfly.cn

[T11] Kotlin：协程
来源：http://xz.colortex.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://zf.shxzskj.cn

[T12] Kotlin：解构声明
来源：http://ed.huanxung.cn

val (a, b) = Pair(1, 2)
来源：http://rb.jctech888.com.cn

[T13] Kotlin：只读 Map
来源：http://dq.bookmarksfly.cn

val m = mapOf("a" to 1)
来源：http://gh.521024.cn

[T14] Kotlin：循环
来源：http://ru.hnjuh.cn

for (i in 1..10) println(i)
来源：http://vh.shtwfgs.cn

[T15] Kotlin：接口
来源：http://uo.haigaiapp.cn

interface Shape { fun area(): Double }
来源：http://vd.nicolike.cn

[T16] Swift：Hello World
来源：http://uu.hahajie.cn

print("Hello")
来源：http://ci.chemitech.net.cn

[T17] Swift：变量与常量
来源：http://te.wgjwhj.cn

var a = 1;  let b = 2
来源：http://nj.yuntaijiaju.cn

[T18] Swift：字符串插值
来源：http://em.yuntaijiaju.cn

"值: \(b)"
来源：http://so.szsharing.cn

[T19] Swift：可选绑定
来源：http://sc.haigaiapp.cn

if let n = opt { print(n) }
来源：http://jo.asd995.cn

[T20] Swift：数组操作
来源：http://qz.szxytkj.cn

var a = [1, 2, 3];  a.append(4)
来源：http://rv.huixiangedu.cn

[T21] Swift：遍历
来源：http://fp.jianghongdianzi.cn

for x in a { print(x) }
来源：http://cj.haigaiapp.cn

[T22] Swift：字典
来源：http://nc.wgjwhj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://yg.shxzskj.cn

[T23] Swift：函数
来源：http://ew.chemitech.net.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://qq.nszjky.cn

[T24] Swift：闭包
来源：http://xn.hahajie.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://yx.bookmarksfly.cn

[T25] Swift：结构体
来源：http://xk.lnxyls.cn

struct P { var x: Int }
来源：http://ts.nicolike.cn

[T26] Swift：类与重写
来源：http://uc.chemitech.net.cn

class A: Base { override func f() {} }
来源：http://wi.hahajie.cn

[T27] Swift：错误处理
来源：http://kp.9csxet.cn

do { try f() } catch { print(error) }
来源：http://lp.asd995.cn

[T28] Swift：枚举
来源：http://uf.nszjky.cn

enum Color { case red, green }
来源：http://gr.yuntaijiaju.cn

[T29] Swift：guard 提前返回
来源：http://rd.bookmarksfly.cn

guard let x = opt else { return }
来源：http://uz.panjiajie.cn

[T30] Swift：协议
来源：http://oz.panjiajie.cn

protocol Shape { func area() -> Double }
来源：http://bf.bookmarksfly.cn

[T31] Lua：Hello World
来源：http://xw.chemitech.net.cn

print("Hello")
来源：http://dz.gzmigu.cn

[T32] Lua：局部变量
来源：http://gv.bjjhwx.cn

local a = 1
来源：http://ho.colortex.cn

[T33] Lua：表（数组）
来源：http://sc.szsharing.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://pz.newstarts.cn

[T34] Lua：遍历表
来源：http://jj.lnxyls.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ho.wgjwhj.cn

[T35] Lua：字典表
来源：http://iv.huanxung.cn

local d = { a = 1 };  d.b = 2
来源：http://bc.bjjhwx.cn

[T36] Lua：函数
来源：http://rh.haigaiapp.cn

function add(a, b) return a + b end
来源：http://bp.bookmarksfly.cn

[T37] Lua：字符串拼接
来源：http://sl.huixinmuqiang.cn

"a" .. "b"
来源：http://vz.haigaiapp.cn

[T38] Lua：条件
来源：http://tt.colortex.cn

if x > 0 then print("正") end
来源：http://ho.colortex.cn

[T39] Lua：模式匹配
来源：http://ij.9csxet.cn

string.find(s, "%d+")
来源：http://is.9csxet.cn

[T40] Lua：元表
来源：http://io.gzmigu.cn

setmetatable({}, { __index = base })
来源：http://vn.bookmarksfly.cn

[T41] Perl：Hello World
来源：http://gc.colortex.cn

print "Hello\n";
来源：http://ne.asd995.cn

[T42] Perl：变量类型
来源：http://nd.newstarts.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://fa.jianghongdianzi.cn

[T43] Perl：字符串插值
来源：http://yt.colortex.cn

"值: $a"
来源：http://iq.haigaiapp.cn

[T44] Perl：条件
来源：http://my.jctech888.com.cn

if ($a > 0) { print "正"; }
来源：http://wj.huanxung.cn

[T45] Perl：数组遍历
来源：http://kk.yuntaijiaju.cn

for my $x (@arr) { print $x; }
来源：http://mh.jctech888.com.cn

[T46] Perl：哈希操作
来源：http://ea.shxzskj.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://xp.nszjky.cn

[T47] Perl：正则捕获
来源：http://sw.szxytkj.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ji.nicolike.cn

[T48] Perl：正则替换
来源：http://xb.nicolike.cn

$s =~ s/old/new/g;
来源：http://kk.nszjky.cn

[T49] Perl：函数
来源：http://cd.yuexingan06.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ed.nszjky.cn

[T50] Perl：逐行读文件
来源：http://um.huixiangedu.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://hh.jianghongdianzi.cn

while (my $line = <$fh>) { print $line; }
来源：http://ns.lnxyls.cn

[T51] Scala：Hello World
来源：http://qc.hnjuh.cn

println("Hello")
来源：http://vy.huixiangedu.cn

[T52] Scala：变量
来源：http://fa.huixinmuqiang.cn

val a = 1;  var b = 2
来源：http://el.huanxung.cn

[T53] Scala：字符串插值
来源：http://wj.chemitech.net.cn

s"值: $b"
来源：http://py.huixinmuqiang.cn

[T54] Scala：集合映射
来源：http://fk.nicolike.cn

List(1, 2, 3).map(_ * 2)
来源：http://gj.huanxung.cn

[T55] Scala：集合过滤
来源：http://vu.hnjuh.cn

List(1, 2, 3).filter(_ > 1)
来源：http://cv.chemitech.net.cn

[T56] Scala：样例类
来源：http://hx.wgjwhj.cn

case class User(name: String, age: Int)
来源：http://az.szxytkj.cn

[T57] Scala：模式匹配
来源：http://ul.bookmarksfly.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://xm.jianghongdianzi.cn

[T58] Scala：函数定义
来源：http://nz.lnxyls.cn

def add(a: Int, b: Int): Int = a + b
来源：http://pv.nszjky.cn

[T59] Scala：循环
来源：http://ko.wgjwhj.cn

for (i <- 1 to 10) println(i)
来源：http://jh.gzmigu.cn

[T60] Scala：折叠
来源：http://iy.bjjhwx.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://qv.newstarts.cn

================================================================================
来源：http://al.asd995.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://lt.szxytkj.cn

================================================================================
来源：http://xo.jianghongdianzi.cn

[U01] Py：创建虚拟环境
来源：http://db.huixiangedu.cn

python -m venv .venv && source .venv/bin/activate
来源：http://uj.szsharing.cn

[U02] Py：导出 / 安装依赖
来源：http://wn.lnxyls.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://rw.jianghongdianzi.cn

[U03] Py：加载 .env 配置
来源：http://jx.bjjhwx.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://rc.asd995.cn

[U04] Py：变量调试打印
来源：http://ww.huixiangedu.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://wr.huanxung.cn

[U05] Py：列表去重且保序
来源：http://dv.shxzukj.cn

list(dict.fromkeys(arr))
来源：http://ae.nszjky.cn

[U06] Py：合并两个字典
来源：http://mq.chemitech.net.cn

{**a, **b}
来源：http://hb.shxzukj.cn

[U07] Py：反转字典键值
来源：http://pr.muxihuayi.cn

{v: k for k, v in d.items()}
来源：http://am.wgjwhj.cn

[U08] Py：展平二维列表
来源：http://jj.jianghongdianzi.cn

[y for x in nested for y in x]
来源：http://ag.huanxung.cn

[U09] Py：字典取最大值的键
来源：http://qw.haigaiapp.cn

max(d, key=d.get)
来源：http://iu.asd995.cn

[U10] Py：按值排序字典
来源：http://kl.gzmigu.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://to.9csxet.cn

[U11] Py：生成器表达式
来源：http://fx.newstarts.cn

(x * 2 for x in arr)
来源：http://iz.colortex.cn

[U12] Py：取出现最多的 3 个元素
来源：http://dg.newstarts.cn

Counter(arr).most_common(3)
来源：http://hp.hnjuh.cn

[U13] Py：固定长度队列
来源：http://ib.hnjuh.cn

deque(maxlen=10)
来源：http://hm.wgjwhj.cn

[U14] Py：分组收集到列表
来源：http://tv.huanxung.cn

defaultdict(list)
来源：http://pj.huixinmuqiang.cn

[U15] Py：高精度计时
来源：http://eu.nicolike.cn

t = time.perf_counter()
来源：http://vq.hnjuh.cn

[U16] Py：命令行参数解析
来源：http://xu.nicolike.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://wc.panjiajie.cn

[U17] Py：初始化日志
来源：http://fu.newstarts.cn

logging.basicConfig(level=logging.INFO)
来源：http://wi.lnxyls.cn

[U18] Py：预编译正则
来源：http://rh.nszjky.cn

pat = re.compile(r"\d+")
来源：http://wb.szsharing.cn

[U19] Py：正则替换带回调
来源：http://wx.yuexingan06.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://rv.muxihuayi.cn

[U20] Py：缓存函数结果
来源：http://cm.shxzukj.cn

@functools.lru_cache(maxsize=None)
来源：http://vw.szxytkj.cn

[U21] Py：自定义上下文管理器
来源：http://so.wgjwhj.cn

@contextlib.contextmanager
来源：http://ye.asd995.cn

[U22] Py：矩阵转置
来源：http://xb.nicolike.cn

list(zip(*m))
来源：http://le.bjjhwx.cn

[U23] Py：分块读取大文件
来源：http://qq.nicolike.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://yq.szxytkj.cn

[U24] Py：路径操作
来源：http://sa.chemitech.net.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://cc.shxzukj.cn

[U25] Py：CSV 按字典读
来源：http://ef.panjiajie.cn

csv.DictReader(f)
来源：http://al.gzmigu.cn

[U26] Py：并发下载
来源：http://bf.yuntaijiaju.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://wj.bookmarksfly.cn

[U27] Py：异步 HTTP
来源：http://fc.jctech888.com.cn

aiohttp.ClientSession() 配合 async with
来源：http://ou.bjjhwx.cn

[U28] Py：类型别名
来源：http://xw.shtwfgs.cn

UserId = int
来源：http://aj.colortex.cn

[U29] Py：属性校验
来源：http://rt.huixinmuqiang.cn

@property 与 @x.setter 配合
来源：http://hw.wgjwhj.cn

[U30] Py：数据类
来源：http://zc.huanxung.cn

@dataclass(slots=True)
来源：http://as.yuntaijiaju.cn

[U31] Py：单测
来源：http://vs.colortex.cn

python -m pytest -q
来源：http://tf.bookmarksfly.cn

[U32] Py：代码格式化
来源：http://gr.lnxyls.cn

ruff format . && ruff check --fix .
来源：http://ay.521024.cn

[U33] Py：打包发布
来源：http://dg.hnjuh.cn

python -m build  （依赖 pyproject.toml）
来源：http://vu.shtwfgs.cn

[U34] Py：判断编码
来源：http://xr.521024.cn

chardet.detect(raw)
来源：http://gv.shxzskj.cn

[U35] Py：发送邮件
来源：http://mn.jctech888.com.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://gx.yuntaijiaju.cn

[U36] Py：定时任务
来源：http://ql.nszjky.cn

schedule.every(10).minutes.do(job)
来源：http://dw.nszjky.cn

[U37] Py：读写 Excel
来源：http://qk.9csxet.cn

pandas.read_excel / DataFrame.to_excel
来源：http://hg.haigaiapp.cn

[U38] Py：获取脚本所在目录
来源：http://rh.yuntaijiaju.cn

Path(__file__).resolve().parent
来源：http://tv.newstarts.cn

[U39] Py：判断是否在交互环境
来源：http://te.shxzukj.cn

sys.stdout.isatty()
来源：http://zl.szxytkj.cn

[U40] Py：打印到标准错误
来源：http://vk.jianghongdianzi.cn

print("err", file=sys.stderr)
来源：http://lw.521024.cn

[U41] PHP：初始化 Composer 项目
来源：http://ty.bjjhwx.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://cv.yuntaijiaju.cn

[U42] PHP：PSR-4 自动加载
来源：http://hc.nicolike.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://hf.yuntaijiaju.cn

[U43] PHP：声明命名空间
来源：http://fl.shxzukj.cn

namespace App\Http;
来源：http://dp.shxzskj.cn

[U44] PHP：开启严格类型
来源：http://vm.gzmigu.cn

declare(strict_types=1);
来源：http://sq.521024.cn


<!-- 参考信息 -->