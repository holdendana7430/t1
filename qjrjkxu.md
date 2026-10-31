代发 wailian999

atoi("42");  strtod("3.14", NULL);
来源：http://yc.huixiangedu.cn

[S23] C：随机数
来源：http://bu.newstarts.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://wa.szxytkj.cn

[S24] C：获取本地时间
来源：http://jw.shxzskj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://wx.jianghongdianzi.cn

[S25] C：内存拷贝
来源：http://tf.bjjhwx.cn

memcpy(dst, src, n);
来源：http://hk.panjiajie.cn

[S26] C：内存清零
来源：http://px.nicolike.cn

memset(a, 0, sizeof a);
来源：http://mt.bookmarksfly.cn

[S27] C：定义常量
来源：http://ci.shxzskj.cn

const double PI = 3.14159;
来源：http://id.panjiajie.cn

[S28] C：静态变量
来源：http://bl.bookmarksfly.cn

static int counter = 0;
来源：http://ff.shxzukj.cn

[S29] C：变参函数
来源：http://uh.gzmigu.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://nf.panjiajie.cn

[S30] C：头文件保护
来源：http://kf.9csxet.cn

#ifndef X_H
来源：http://cl.521024.cn

#define X_H
来源：http://it.9csxet.cn

#endif
来源：http://bb.jianghongdianzi.cn

[S31] C++：Hello World
来源：http://qf.gzmigu.cn

#include <iostream>
来源：http://js.huixinmuqiang.cn

int main() { std::cout << "Hello\n"; }
来源：http://st.newstarts.cn

[S32] C++：字符串
来源：http://pl.jctech888.com.cn

std::string s = "hi";  s += "!";
来源：http://ws.huixinmuqiang.cn

[S33] C++：vector 增删
来源：http://my.newstarts.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qq.shxzukj.cn

[S34] C++：遍历 vector
来源：http://wi.wgjwhj.cn

for (auto &x : v) { std::cout << x; }
来源：http://hd.shxzskj.cn

[S35] C++：map
来源：http://vr.shxzukj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://rj.nszjky.cn

[S36] C++：unordered_map
来源：http://fe.chemitech.net.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://fo.yuntaijiaju.cn

[S37] C++：set
来源：http://gv.9csxet.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://gq.9csxet.cn

[S38] C++：排序
来源：http://pz.gzmigu.cn

std::sort(v.begin(), v.end());
来源：http://ip.yuexingan06.cn

[S39] C++：自定义比较器排序
来源：http://ss.bookmarksfly.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://lz.newstarts.cn

[S40] C++：查找元素
来源：http://xo.shxzukj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://sw.chemitech.net.cn

[S41] C++：类与构造函数
来源：http://yc.szxytkj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://nd.newstarts.cn

[S42] C++：继承与虚函数
来源：http://pc.wgjwhj.cn

class B : public Base { public: void f() override {} };
来源：http://lc.bookmarksfly.cn

[S43] C++：智能指针
来源：http://zq.newstarts.cn

auto p = std::make_unique<int>(5);
来源：http://fq.jctech888.com.cn

[S44] C++：引用传参
来源：http://qp.panjiajie.cn

void inc(int &x) { ++x; }
来源：http://tw.yuntaijiaju.cn

[S45] C++：lambda
来源：http://os.newstarts.cn

auto add = [](int a, int b) { return a + b; };
来源：http://bq.chemitech.net.cn

[S46] C++：函数模板
来源：http://do.newstarts.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://js.nicolike.cn

[S47] C++：结构化绑定遍历
来源：http://tb.jctech888.com.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://og.wgjwhj.cn

[S48] C++：逐行读文件
来源：http://ww.jianghongdianzi.cn

std::ifstream in("a.txt");  std::string line;
来源：http://kg.hahajie.cn

while (std::getline(in, line)) { }
来源：http://yk.newstarts.cn

[S49] C++：写文件
来源：http://bb.lnxyls.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://vk.jctech888.com.cn

[S50] C++：格式化数字
来源：http://zb.newstarts.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://bh.bookmarksfly.cn

[S51] C++：显式类型转换
来源：http://sm.haigaiapp.cn

static_cast<double>(a) / b
来源：http://ki.nszjky.cn

[S52] C++：const 与 noexcept
来源：http://ta.huixinmuqiang.cn

int size() const noexcept { return n_; }
来源：http://ke.jctech888.com.cn

[S53] C++：移动语义
来源：http://ce.bjjhwx.cn

std::vector<int> w = std::move(v);
来源：http://rd.haigaiapp.cn

[S54] C++：异常处理
来源：http://kx.521024.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://qg.chemitech.net.cn

[S55] C++：结构化绑定
来源：http://ww.szxytkj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://bo.shxzukj.cn

[S56] C++：optional
来源：http://wh.huixinmuqiang.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://am.bjjhwx.cn

[S57] C++：编译期常量
来源：http://dd.jianghongdianzi.cn

constexpr int N = 10;
来源：http://ns.colortex.cn

[S58] C++：命名空间
来源：http://qc.muxihuayi.cn

namespace ns { int f() { return 1; } }
来源：http://lw.9csxet.cn

[S59] C++：静态断言
来源：http://tv.newstarts.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://tn.colortex.cn

[S60] C++：遍历并删除元素
来源：http://ln.nicolike.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://qc.nszjky.cn

================================================================================
来源：http://vd.lnxyls.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xr.hahajie.cn

================================================================================
来源：http://vz.hahajie.cn

[T01] Kotlin：Hello World
来源：http://ag.shxzukj.cn

println("Hello")
来源：http://vt.szxytkj.cn

[T02] Kotlin：变量
来源：http://tr.jianghongdianzi.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mw.9csxet.cn

[T03] Kotlin：字符串模板
来源：http://sx.hnjuh.cn

"值: $b"
来源：http://px.chemitech.net.cn

[T04] Kotlin：空安全
来源：http://cw.shxzskj.cn

val n: String? = null;  n?.length
来源：http://ms.bjjhwx.cn

[T05] Kotlin：when 表达式
来源：http://ei.colortex.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://pj.bookmarksfly.cn

[T06] Kotlin：集合映射
来源：http://ng.asd995.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://cq.gzmigu.cn

[T07] Kotlin：集合过滤
来源：http://qg.bookmarksfly.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ey.muxihuayi.cn

[T08] Kotlin：数据类
来源：http://wq.bjjhwx.cn

data class User(val name: String, val age: Int)
来源：http://fb.jianghongdianzi.cn

[T09] Kotlin：扩展函数
来源：http://aq.lnxyls.cn

fun String.exclaim() = this + "!"
来源：http://ys.haigaiapp.cn

[T10] Kotlin：默认参数
来源：http://yy.yuntaijiaju.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://dy.shxzukj.cn

[T11] Kotlin：协程
来源：http://dz.jctech888.com.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://vs.yuexingan06.cn

[T12] Kotlin：解构声明
来源：http://uk.521024.cn

val (a, b) = Pair(1, 2)
来源：http://gs.521024.cn

[T13] Kotlin：只读 Map
来源：http://ss.haigaiapp.cn

val m = mapOf("a" to 1)
来源：http://ga.muxihuayi.cn

[T14] Kotlin：循环
来源：http://pa.colortex.cn

for (i in 1..10) println(i)
来源：http://oq.panjiajie.cn

[T15] Kotlin：接口
来源：http://gc.jianghongdianzi.cn

interface Shape { fun area(): Double }
来源：http://fn.lnxyls.cn

[T16] Swift：Hello World
来源：http://sk.szsharing.cn

print("Hello")
来源：http://rr.huanxung.cn

[T17] Swift：变量与常量
来源：http://ir.yuntaijiaju.cn

var a = 1;  let b = 2
来源：http://zl.jianghongdianzi.cn

[T18] Swift：字符串插值
来源：http://jt.bookmarksfly.cn

"值: \(b)"
来源：http://sh.bjjhwx.cn

[T19] Swift：可选绑定
来源：http://jv.hnjuh.cn

if let n = opt { print(n) }
来源：http://nd.haigaiapp.cn

[T20] Swift：数组操作
来源：http://tr.shxzukj.cn

var a = [1, 2, 3];  a.append(4)
来源：http://sy.lnxyls.cn

[T21] Swift：遍历
来源：http://oe.521024.cn

for x in a { print(x) }
来源：http://ow.yuntaijiaju.cn

[T22] Swift：字典
来源：http://xl.szsharing.cn

var d = ["a": 1];  d["b"] = 2
来源：http://bg.shtwfgs.cn

[T23] Swift：函数
来源：http://kz.jianghongdianzi.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://cm.huixinmuqiang.cn

[T24] Swift：闭包
来源：http://vq.huixinmuqiang.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://kr.gzmigu.cn

[T25] Swift：结构体
来源：http://ht.hahajie.cn

struct P { var x: Int }
来源：http://fd.nszjky.cn

[T26] Swift：类与重写
来源：http://zs.shxzskj.cn

class A: Base { override func f() {} }
来源：http://jv.shxzukj.cn

[T27] Swift：错误处理
来源：http://fj.colortex.cn

do { try f() } catch { print(error) }
来源：http://zm.huixinmuqiang.cn

[T28] Swift：枚举
来源：http://mg.shtwfgs.cn

enum Color { case red, green }
来源：http://ke.huixiangedu.cn

[T29] Swift：guard 提前返回
来源：http://pi.jianghongdianzi.cn

guard let x = opt else { return }
来源：http://zy.szsharing.cn

[T30] Swift：协议
来源：http://rw.shxzukj.cn

protocol Shape { func area() -> Double }
来源：http://lw.szxytkj.cn

[T31] Lua：Hello World
来源：http://gy.huixiangedu.cn

print("Hello")
来源：http://re.hahajie.cn

[T32] Lua：局部变量
来源：http://ag.shxzskj.cn

local a = 1
来源：http://dg.szxytkj.cn

[T33] Lua：表（数组）
来源：http://kb.huixiangedu.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://gv.hahajie.cn

[T34] Lua：遍历表
来源：http://vo.nszjky.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://kt.gzmigu.cn

[T35] Lua：字典表
来源：http://li.panjiajie.cn

local d = { a = 1 };  d.b = 2
来源：http://yb.jctech888.com.cn

[T36] Lua：函数
来源：http://zj.asd995.cn

function add(a, b) return a + b end
来源：http://tt.521024.cn

[T37] Lua：字符串拼接
来源：http://vg.lnxyls.cn

"a" .. "b"
来源：http://og.lnxyls.cn

[T38] Lua：条件
来源：http://gl.szxytkj.cn

if x > 0 then print("正") end
来源：http://bt.yuntaijiaju.cn

[T39] Lua：模式匹配
来源：http://rs.hahajie.cn

string.find(s, "%d+")
来源：http://ir.9csxet.cn

[T40] Lua：元表
来源：http://kk.newstarts.cn

setmetatable({}, { __index = base })
来源：http://uo.szxytkj.cn

[T41] Perl：Hello World
来源：http://jk.huixinmuqiang.cn

print "Hello\n";
来源：http://at.jianghongdianzi.cn

[T42] Perl：变量类型
来源：http://mp.wgjwhj.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://og.wgjwhj.cn

[T43] Perl：字符串插值
来源：http://cp.hnjuh.cn

"值: $a"
来源：http://ng.nszjky.cn

[T44] Perl：条件
来源：http://xh.lnxyls.cn

if ($a > 0) { print "正"; }
来源：http://ap.hahajie.cn

[T45] Perl：数组遍历
来源：http://wk.haigaiapp.cn

for my $x (@arr) { print $x; }
来源：http://jo.hahajie.cn

[T46] Perl：哈希操作
来源：http://uh.9csxet.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://gb.haigaiapp.cn

[T47] Perl：正则捕获
来源：http://oa.muxihuayi.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ki.szsharing.cn

[T48] Perl：正则替换
来源：http://wh.colortex.cn

$s =~ s/old/new/g;
来源：http://ab.shxzukj.cn

[T49] Perl：函数
来源：http://st.hnjuh.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ep.haigaiapp.cn

[T50] Perl：逐行读文件
来源：http://zk.jianghongdianzi.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://fn.haigaiapp.cn

while (my $line = <$fh>) { print $line; }
来源：http://eb.521024.cn

[T51] Scala：Hello World
来源：http://wv.jctech888.com.cn

println("Hello")
来源：http://sb.shtwfgs.cn

[T52] Scala：变量
来源：http://yk.yuntaijiaju.cn

val a = 1;  var b = 2
来源：http://wc.haigaiapp.cn

[T53] Scala：字符串插值
来源：http://bs.yuexingan06.cn

s"值: $b"
来源：http://im.chemitech.net.cn

[T54] Scala：集合映射
来源：http://ci.9csxet.cn

List(1, 2, 3).map(_ * 2)
来源：http://lt.szxytkj.cn

[T55] Scala：集合过滤
来源：http://ed.szsharing.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ye.asd995.cn

[T56] Scala：样例类
来源：http://br.newstarts.cn

case class User(name: String, age: Int)
来源：http://qt.jctech888.com.cn

[T57] Scala：模式匹配
来源：http://rf.bookmarksfly.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ts.bookmarksfly.cn

[T58] Scala：函数定义
来源：http://il.haigaiapp.cn

def add(a: Int, b: Int): Int = a + b
来源：http://bb.521024.cn

[T59] Scala：循环
来源：http://lc.huanxung.cn

for (i <- 1 to 10) println(i)
来源：http://xo.shtwfgs.cn

[T60] Scala：折叠
来源：http://aa.bjjhwx.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://yx.huixinmuqiang.cn

================================================================================
来源：http://mh.jctech888.com.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://vt.jianghongdianzi.cn

================================================================================
来源：http://rj.wgjwhj.cn

[U01] Py：创建虚拟环境
来源：http://wo.newstarts.cn

python -m venv .venv && source .venv/bin/activate
来源：http://eb.gzmigu.cn

[U02] Py：导出 / 安装依赖
来源：http://wv.jctech888.com.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://fx.bjjhwx.cn

[U03] Py：加载 .env 配置
来源：http://hw.panjiajie.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://lu.huixiangedu.cn

[U04] Py：变量调试打印
来源：http://jk.gzmigu.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://rr.huixiangedu.cn

[U05] Py：列表去重且保序
来源：http://sw.9csxet.cn

list(dict.fromkeys(arr))
来源：http://yg.huixinmuqiang.cn

[U06] Py：合并两个字典
来源：http://su.huixinmuqiang.cn

{**a, **b}
来源：http://ah.panjiajie.cn

[U07] Py：反转字典键值
来源：http://cr.nszjky.cn

{v: k for k, v in d.items()}
来源：http://it.yuexingan06.cn

[U08] Py：展平二维列表
来源：http://ti.yuexingan06.cn

[y for x in nested for y in x]
来源：http://cb.szsharing.cn

[U09] Py：字典取最大值的键
来源：http://pv.gzmigu.cn

max(d, key=d.get)
来源：http://ig.wgjwhj.cn

[U10] Py：按值排序字典
来源：http://om.bjjhwx.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://in.huixinmuqiang.cn

[U11] Py：生成器表达式
来源：http://eu.wgjwhj.cn

(x * 2 for x in arr)
来源：http://oo.yuntaijiaju.cn

[U12] Py：取出现最多的 3 个元素
来源：http://iy.jctech888.com.cn

Counter(arr).most_common(3)
来源：http://ct.shxzukj.cn

[U13] Py：固定长度队列
来源：http://kg.panjiajie.cn

deque(maxlen=10)
来源：http://gq.huanxung.cn

[U14] Py：分组收集到列表
来源：http://ms.huixiangedu.cn

defaultdict(list)
来源：http://xo.chemitech.net.cn

[U15] Py：高精度计时
来源：http://nr.hahajie.cn

t = time.perf_counter()
来源：http://ta.shxzukj.cn

[U16] Py：命令行参数解析
来源：http://ob.nicolike.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://qp.bookmarksfly.cn

[U17] Py：初始化日志
来源：http://ho.521024.cn

logging.basicConfig(level=logging.INFO)
来源：http://zg.szsharing.cn

[U18] Py：预编译正则
来源：http://kd.huixiangedu.cn

pat = re.compile(r"\d+")
来源：http://mr.bookmarksfly.cn

[U19] Py：正则替换带回调
来源：http://bw.chemitech.net.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://la.yuntaijiaju.cn

[U20] Py：缓存函数结果
来源：http://pp.newstarts.cn

@functools.lru_cache(maxsize=None)
来源：http://xp.nicolike.cn

[U21] Py：自定义上下文管理器
来源：http://qw.nicolike.cn

@contextlib.contextmanager
来源：http://ru.muxihuayi.cn

[U22] Py：矩阵转置
来源：http://ru.nszjky.cn

list(zip(*m))
来源：http://wq.gzmigu.cn

[U23] Py：分块读取大文件
来源：http://ul.panjiajie.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://lq.yuntaijiaju.cn

[U24] Py：路径操作
来源：http://ka.lnxyls.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://en.wgjwhj.cn

[U25] Py：CSV 按字典读
来源：http://ru.gzmigu.cn

csv.DictReader(f)
来源：http://lk.muxihuayi.cn

[U26] Py：并发下载
来源：http://yd.9csxet.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://pa.colortex.cn

[U27] Py：异步 HTTP
来源：http://ay.huixiangedu.cn

aiohttp.ClientSession() 配合 async with
来源：http://ou.shtwfgs.cn

[U28] Py：类型别名
来源：http://vw.yuexingan06.cn

UserId = int
来源：http://bc.panjiajie.cn

[U29] Py：属性校验
来源：http://mr.wgjwhj.cn

@property 与 @x.setter 配合
来源：http://fm.9csxet.cn

[U30] Py：数据类
来源：http://xq.huixiangedu.cn

@dataclass(slots=True)
来源：http://cv.asd995.cn

[U31] Py：单测
来源：http://gg.bookmarksfly.cn

python -m pytest -q
来源：http://eo.jianghongdianzi.cn

[U32] Py：代码格式化
来源：http://oq.lnxyls.cn

ruff format . && ruff check --fix .
来源：http://yy.huixiangedu.cn

[U33] Py：打包发布
来源：http://hd.szxytkj.cn

python -m build  （依赖 pyproject.toml）
来源：http://vy.wgjwhj.cn

[U34] Py：判断编码
来源：http://gh.nszjky.cn

chardet.detect(raw)
来源：http://yk.shxzskj.cn

[U35] Py：发送邮件
来源：http://ih.haigaiapp.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://rd.shxzukj.cn

[U36] Py：定时任务
来源：http://cc.shxzukj.cn

schedule.every(10).minutes.do(job)
来源：http://cs.lnxyls.cn

[U37] Py：读写 Excel
来源：http://bm.colortex.cn

pandas.read_excel / DataFrame.to_excel
来源：http://hi.hnjuh.cn

[U38] Py：获取脚本所在目录
来源：http://dm.huixinmuqiang.cn

Path(__file__).resolve().parent
来源：http://xg.jctech888.com.cn

[U39] Py：判断是否在交互环境
来源：http://wa.bookmarksfly.cn

sys.stdout.isatty()
来源：http://kn.szxytkj.cn

[U40] Py：打印到标准错误
来源：http://pv.nicolike.cn

print("err", file=sys.stderr)
来源：http://bp.wgjwhj.cn

[U41] PHP：初始化 Composer 项目
来源：http://xp.yuexingan06.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://av.nszjky.cn

[U42] PHP：PSR-4 自动加载
来源：http://zm.lnxyls.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://gv.yuntaijiaju.cn

[U43] PHP：声明命名空间
来源：http://pp.haigaiapp.cn

namespace App\Http;
来源：http://ux.colortex.cn

[U44] PHP：开启严格类型
来源：http://df.hnjuh.cn

declare(strict_types=1);
来源：http://ua.hnjuh.cn

[U45] PHP：类型声明与返回类型
来源：http://zz.yuntaijiaju.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://dt.9csxet.cn

[U46] PHP：可空类型
来源：http://wr.lnxyls.cn

?string $name = null
来源：http://wt.szsharing.cn


<!-- 参考信息 -->