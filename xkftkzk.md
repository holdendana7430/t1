代发 wailian999

atoi("42");  strtod("3.14", NULL);
来源：http://om.muxihuayi.cn

[S23] C：随机数
来源：http://tb.szxytkj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ne.9csxet.cn

[S24] C：获取本地时间
来源：http://df.gzmigu.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://iy.yuntaijiaju.cn

[S25] C：内存拷贝
来源：http://ky.bjjhwx.cn

memcpy(dst, src, n);
来源：http://zw.bookmarksfly.cn

[S26] C：内存清零
来源：http://ry.szsharing.cn

memset(a, 0, sizeof a);
来源：http://gh.nicolike.cn

[S27] C：定义常量
来源：http://ja.huanxung.cn

const double PI = 3.14159;
来源：http://fr.huixinmuqiang.cn

[S28] C：静态变量
来源：http://rr.9csxet.cn

static int counter = 0;
来源：http://ky.shxzskj.cn

[S29] C：变参函数
来源：http://we.nszjky.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://zf.hnjuh.cn

[S30] C：头文件保护
来源：http://fh.bookmarksfly.cn

#ifndef X_H
来源：http://bn.huixinmuqiang.cn

#define X_H
来源：http://kl.szxytkj.cn

#endif
来源：http://kz.shtwfgs.cn

[S31] C++：Hello World
来源：http://nj.colortex.cn

#include <iostream>
来源：http://ev.yuntaijiaju.cn

int main() { std::cout << "Hello\n"; }
来源：http://cd.bjjhwx.cn

[S32] C++：字符串
来源：http://cv.asd995.cn

std::string s = "hi";  s += "!";
来源：http://ar.521024.cn

[S33] C++：vector 增删
来源：http://cs.panjiajie.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://gy.colortex.cn

[S34] C++：遍历 vector
来源：http://bl.huanxung.cn

for (auto &x : v) { std::cout << x; }
来源：http://fk.lnxyls.cn

[S35] C++：map
来源：http://tt.lnxyls.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://lc.shxzukj.cn

[S36] C++：unordered_map
来源：http://cn.bookmarksfly.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://nw.haigaiapp.cn

[S37] C++：set
来源：http://dt.9csxet.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://sy.hahajie.cn

[S38] C++：排序
来源：http://wd.muxihuayi.cn

std::sort(v.begin(), v.end());
来源：http://ou.huixiangedu.cn

[S39] C++：自定义比较器排序
来源：http://ye.gzmigu.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://jj.yuexingan06.cn

[S40] C++：查找元素
来源：http://ix.szxytkj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wi.yuexingan06.cn

[S41] C++：类与构造函数
来源：http://tk.newstarts.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://dy.hnjuh.cn

[S42] C++：继承与虚函数
来源：http://oj.shtwfgs.cn

class B : public Base { public: void f() override {} };
来源：http://bt.shxzskj.cn

[S43] C++：智能指针
来源：http://ou.shxzskj.cn

auto p = std::make_unique<int>(5);
来源：http://hz.lnxyls.cn

[S44] C++：引用传参
来源：http://eu.bjjhwx.cn

void inc(int &x) { ++x; }
来源：http://ss.yuexingan06.cn

[S45] C++：lambda
来源：http://ed.521024.cn

auto add = [](int a, int b) { return a + b; };
来源：http://bq.szxytkj.cn

[S46] C++：函数模板
来源：http://ei.nicolike.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ae.nszjky.cn

[S47] C++：结构化绑定遍历
来源：http://qn.newstarts.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://uq.panjiajie.cn

[S48] C++：逐行读文件
来源：http://px.muxihuayi.cn

std::ifstream in("a.txt");  std::string line;
来源：http://nz.hnjuh.cn

while (std::getline(in, line)) { }
来源：http://pa.jctech888.com.cn

[S49] C++：写文件
来源：http://gj.521024.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ph.huixiangedu.cn

[S50] C++：格式化数字
来源：http://ju.nicolike.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://yr.jctech888.com.cn

[S51] C++：显式类型转换
来源：http://cu.shtwfgs.cn

static_cast<double>(a) / b
来源：http://ah.nicolike.cn

[S52] C++：const 与 noexcept
来源：http://mx.jianghongdianzi.cn

int size() const noexcept { return n_; }
来源：http://nn.bookmarksfly.cn

[S53] C++：移动语义
来源：http://yu.shxzskj.cn

std::vector<int> w = std::move(v);
来源：http://jz.haigaiapp.cn

[S54] C++：异常处理
来源：http://lt.yuexingan06.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://nn.hahajie.cn

[S55] C++：结构化绑定
来源：http://np.lnxyls.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://bl.shxzukj.cn

[S56] C++：optional
来源：http://gi.hahajie.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://uw.bookmarksfly.cn

[S57] C++：编译期常量
来源：http://aj.huanxung.cn

constexpr int N = 10;
来源：http://ih.wgjwhj.cn

[S58] C++：命名空间
来源：http://uv.hnjuh.cn

namespace ns { int f() { return 1; } }
来源：http://zc.huixinmuqiang.cn

[S59] C++：静态断言
来源：http://kg.haigaiapp.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://qs.huanxung.cn

[S60] C++：遍历并删除元素
来源：http://bg.szxytkj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://xo.bookmarksfly.cn

================================================================================
来源：http://in.nicolike.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ko.jianghongdianzi.cn

================================================================================
来源：http://jj.9csxet.cn

[T01] Kotlin：Hello World
来源：http://dg.newstarts.cn

println("Hello")
来源：http://pd.shxzukj.cn

[T02] Kotlin：变量
来源：http://ty.chemitech.net.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mq.shtwfgs.cn

[T03] Kotlin：字符串模板
来源：http://rk.haigaiapp.cn

"值: $b"
来源：http://us.shxzukj.cn

[T04] Kotlin：空安全
来源：http://wk.hahajie.cn

val n: String? = null;  n?.length
来源：http://hg.yuntaijiaju.cn

[T05] Kotlin：when 表达式
来源：http://fb.szxytkj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://dl.hnjuh.cn

[T06] Kotlin：集合映射
来源：http://sz.bjjhwx.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://mz.nszjky.cn

[T07] Kotlin：集合过滤
来源：http://el.lnxyls.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://xu.panjiajie.cn

[T08] Kotlin：数据类
来源：http://el.chemitech.net.cn

data class User(val name: String, val age: Int)
来源：http://pl.haigaiapp.cn

[T09] Kotlin：扩展函数
来源：http://wg.nszjky.cn

fun String.exclaim() = this + "!"
来源：http://li.hahajie.cn

[T10] Kotlin：默认参数
来源：http://ll.hnjuh.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://nd.hahajie.cn

[T11] Kotlin：协程
来源：http://kh.shxzukj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://xu.jctech888.com.cn

[T12] Kotlin：解构声明
来源：http://hu.bookmarksfly.cn

val (a, b) = Pair(1, 2)
来源：http://qz.shxzukj.cn

[T13] Kotlin：只读 Map
来源：http://jc.jctech888.com.cn

val m = mapOf("a" to 1)
来源：http://gt.yuexingan06.cn

[T14] Kotlin：循环
来源：http://us.nicolike.cn

for (i in 1..10) println(i)
来源：http://wy.haigaiapp.cn

[T15] Kotlin：接口
来源：http://tg.wgjwhj.cn

interface Shape { fun area(): Double }
来源：http://vg.bjjhwx.cn

[T16] Swift：Hello World
来源：http://wx.newstarts.cn

print("Hello")
来源：http://bl.szsharing.cn

[T17] Swift：变量与常量
来源：http://ij.nszjky.cn

var a = 1;  let b = 2
来源：http://il.szsharing.cn

[T18] Swift：字符串插值
来源：http://md.bjjhwx.cn

"值: \(b)"
来源：http://ic.szxytkj.cn

[T19] Swift：可选绑定
来源：http://xm.huanxung.cn

if let n = opt { print(n) }
来源：http://dl.haigaiapp.cn

[T20] Swift：数组操作
来源：http://oy.jianghongdianzi.cn

var a = [1, 2, 3];  a.append(4)
来源：http://fp.huixiangedu.cn

[T21] Swift：遍历
来源：http://la.asd995.cn

for x in a { print(x) }
来源：http://jk.newstarts.cn

[T22] Swift：字典
来源：http://af.shtwfgs.cn

var d = ["a": 1];  d["b"] = 2
来源：http://gx.asd995.cn

[T23] Swift：函数
来源：http://gi.panjiajie.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://lf.haigaiapp.cn

[T24] Swift：闭包
来源：http://lz.521024.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://xb.shxzukj.cn

[T25] Swift：结构体
来源：http://mh.szsharing.cn

struct P { var x: Int }
来源：http://cl.huanxung.cn

[T26] Swift：类与重写
来源：http://yb.panjiajie.cn

class A: Base { override func f() {} }
来源：http://ni.gzmigu.cn

[T27] Swift：错误处理
来源：http://zt.yuexingan06.cn

do { try f() } catch { print(error) }
来源：http://mf.panjiajie.cn

[T28] Swift：枚举
来源：http://xf.huixinmuqiang.cn

enum Color { case red, green }
来源：http://oi.jianghongdianzi.cn

[T29] Swift：guard 提前返回
来源：http://ex.muxihuayi.cn

guard let x = opt else { return }
来源：http://yu.nicolike.cn

[T30] Swift：协议
来源：http://eo.yuntaijiaju.cn

protocol Shape { func area() -> Double }
来源：http://sw.nszjky.cn

[T31] Lua：Hello World
来源：http://be.huixiangedu.cn

print("Hello")
来源：http://ha.wgjwhj.cn

[T32] Lua：局部变量
来源：http://xk.panjiajie.cn

local a = 1
来源：http://ng.yuntaijiaju.cn

[T33] Lua：表（数组）
来源：http://ix.9csxet.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://nr.jctech888.com.cn

[T34] Lua：遍历表
来源：http://vl.szxytkj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://on.szsharing.cn

[T35] Lua：字典表
来源：http://fu.jctech888.com.cn

local d = { a = 1 };  d.b = 2
来源：http://wd.521024.cn

[T36] Lua：函数
来源：http://mi.lnxyls.cn

function add(a, b) return a + b end
来源：http://ds.wgjwhj.cn

[T37] Lua：字符串拼接
来源：http://jy.shxzukj.cn

"a" .. "b"
来源：http://fv.chemitech.net.cn

[T38] Lua：条件
来源：http://os.jctech888.com.cn

if x > 0 then print("正") end
来源：http://ha.jctech888.com.cn

[T39] Lua：模式匹配
来源：http://uy.bookmarksfly.cn

string.find(s, "%d+")
来源：http://sp.bjjhwx.cn

[T40] Lua：元表
来源：http://iv.521024.cn

setmetatable({}, { __index = base })
来源：http://gk.521024.cn

[T41] Perl：Hello World
来源：http://ha.huanxung.cn

print "Hello\n";
来源：http://ss.wgjwhj.cn

[T42] Perl：变量类型
来源：http://qh.9csxet.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ho.haigaiapp.cn

[T43] Perl：字符串插值
来源：http://gr.shxzukj.cn

"值: $a"
来源：http://hp.jctech888.com.cn

[T44] Perl：条件
来源：http://jp.haigaiapp.cn

if ($a > 0) { print "正"; }
来源：http://gj.szxytkj.cn

[T45] Perl：数组遍历
来源：http://sk.bookmarksfly.cn

for my $x (@arr) { print $x; }
来源：http://cq.shxzskj.cn

[T46] Perl：哈希操作
来源：http://zb.yuexingan06.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://fg.jianghongdianzi.cn

[T47] Perl：正则捕获
来源：http://zk.jctech888.com.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ts.huixiangedu.cn

[T48] Perl：正则替换
来源：http://hi.lnxyls.cn

$s =~ s/old/new/g;
来源：http://bu.asd995.cn

[T49] Perl：函数
来源：http://lv.hahajie.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://vc.bjjhwx.cn

[T50] Perl：逐行读文件
来源：http://il.nszjky.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://qn.521024.cn

while (my $line = <$fh>) { print $line; }
来源：http://qr.muxihuayi.cn

[T51] Scala：Hello World
来源：http://rl.huanxung.cn

println("Hello")
来源：http://kd.hnjuh.cn

[T52] Scala：变量
来源：http://nb.bookmarksfly.cn

val a = 1;  var b = 2
来源：http://fl.newstarts.cn

[T53] Scala：字符串插值
来源：http://ib.521024.cn

s"值: $b"
来源：http://lu.szsharing.cn

[T54] Scala：集合映射
来源：http://hw.asd995.cn

List(1, 2, 3).map(_ * 2)
来源：http://rn.huixinmuqiang.cn

[T55] Scala：集合过滤
来源：http://ue.colortex.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ay.lnxyls.cn

[T56] Scala：样例类
来源：http://qq.bjjhwx.cn

case class User(name: String, age: Int)
来源：http://cv.hahajie.cn

[T57] Scala：模式匹配
来源：http://yi.jianghongdianzi.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ej.nszjky.cn

[T58] Scala：函数定义
来源：http://qy.newstarts.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ff.bookmarksfly.cn

[T59] Scala：循环
来源：http://wn.szsharing.cn

for (i <- 1 to 10) println(i)
来源：http://zm.shtwfgs.cn

[T60] Scala：折叠
来源：http://se.muxihuayi.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://fq.newstarts.cn

================================================================================
来源：http://ad.yuexingan06.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://cu.wgjwhj.cn

================================================================================
来源：http://bd.haigaiapp.cn

[U01] Py：创建虚拟环境
来源：http://gg.colortex.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ml.haigaiapp.cn

[U02] Py：导出 / 安装依赖
来源：http://mv.muxihuayi.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://kh.wgjwhj.cn

[U03] Py：加载 .env 配置
来源：http://yw.asd995.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://br.colortex.cn

[U04] Py：变量调试打印
来源：http://ft.9csxet.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://en.lnxyls.cn

[U05] Py：列表去重且保序
来源：http://qa.newstarts.cn

list(dict.fromkeys(arr))
来源：http://hk.hnjuh.cn

[U06] Py：合并两个字典
来源：http://mi.asd995.cn

{**a, **b}
来源：http://ru.shxzukj.cn

[U07] Py：反转字典键值
来源：http://je.nicolike.cn

{v: k for k, v in d.items()}
来源：http://il.jianghongdianzi.cn

[U08] Py：展平二维列表
来源：http://oi.nicolike.cn

[y for x in nested for y in x]
来源：http://dl.bookmarksfly.cn

[U09] Py：字典取最大值的键
来源：http://md.szxytkj.cn

max(d, key=d.get)
来源：http://uz.huanxung.cn

[U10] Py：按值排序字典
来源：http://fk.shxzukj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ad.shxzskj.cn

[U11] Py：生成器表达式
来源：http://uh.hahajie.cn

(x * 2 for x in arr)
来源：http://yi.hahajie.cn

[U12] Py：取出现最多的 3 个元素
来源：http://km.asd995.cn

Counter(arr).most_common(3)
来源：http://bf.jctech888.com.cn

[U13] Py：固定长度队列
来源：http://lg.huanxung.cn

deque(maxlen=10)
来源：http://ln.newstarts.cn

[U14] Py：分组收集到列表
来源：http://eb.hahajie.cn

defaultdict(list)
来源：http://dy.panjiajie.cn

[U15] Py：高精度计时
来源：http://rh.jctech888.com.cn

t = time.perf_counter()
来源：http://ag.hnjuh.cn

[U16] Py：命令行参数解析
来源：http://zm.shtwfgs.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://dt.shxzskj.cn

[U17] Py：初始化日志
来源：http://wd.szxytkj.cn

logging.basicConfig(level=logging.INFO)
来源：http://gz.hahajie.cn

[U18] Py：预编译正则
来源：http://db.nszjky.cn

pat = re.compile(r"\d+")
来源：http://vm.huixinmuqiang.cn

[U19] Py：正则替换带回调
来源：http://jl.hahajie.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://lj.nszjky.cn

[U20] Py：缓存函数结果
来源：http://fu.hahajie.cn

@functools.lru_cache(maxsize=None)
来源：http://qq.panjiajie.cn

[U21] Py：自定义上下文管理器
来源：http://me.bjjhwx.cn

@contextlib.contextmanager
来源：http://ou.9csxet.cn

[U22] Py：矩阵转置
来源：http://sh.haigaiapp.cn

list(zip(*m))
来源：http://jr.chemitech.net.cn

[U23] Py：分块读取大文件
来源：http://wo.hnjuh.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://ti.yuntaijiaju.cn

[U24] Py：路径操作
来源：http://gx.hahajie.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://cy.521024.cn

[U25] Py：CSV 按字典读
来源：http://uf.muxihuayi.cn

csv.DictReader(f)
来源：http://hk.gzmigu.cn

[U26] Py：并发下载
来源：http://fm.shxzukj.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://dy.colortex.cn

[U27] Py：异步 HTTP
来源：http://ou.shxzukj.cn

aiohttp.ClientSession() 配合 async with
来源：http://lp.muxihuayi.cn

[U28] Py：类型别名
来源：http://dz.521024.cn

UserId = int
来源：http://jk.nicolike.cn

[U29] Py：属性校验
来源：http://vg.jctech888.com.cn

@property 与 @x.setter 配合
来源：http://wp.shtwfgs.cn

[U30] Py：数据类
来源：http://vd.9csxet.cn

@dataclass(slots=True)
来源：http://pi.panjiajie.cn

[U31] Py：单测
来源：http://ai.haigaiapp.cn

python -m pytest -q
来源：http://ss.hahajie.cn

[U32] Py：代码格式化
来源：http://wo.haigaiapp.cn

ruff format . && ruff check --fix .
来源：http://ut.hnjuh.cn

[U33] Py：打包发布
来源：http://kg.newstarts.cn

python -m build  （依赖 pyproject.toml）
来源：http://wa.9csxet.cn

[U34] Py：判断编码
来源：http://mx.yuexingan06.cn

chardet.detect(raw)
来源：http://rz.huanxung.cn

[U35] Py：发送邮件
来源：http://bh.yuntaijiaju.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://pz.panjiajie.cn

[U36] Py：定时任务
来源：http://cg.yuntaijiaju.cn

schedule.every(10).minutes.do(job)
来源：http://ld.asd995.cn

[U37] Py：读写 Excel
来源：http://rf.shtwfgs.cn

pandas.read_excel / DataFrame.to_excel
来源：http://fo.jctech888.com.cn

[U38] Py：获取脚本所在目录
来源：http://cc.nszjky.cn

Path(__file__).resolve().parent
来源：http://nt.hahajie.cn

[U39] Py：判断是否在交互环境
来源：http://oa.yuexingan06.cn

sys.stdout.isatty()
来源：http://df.huanxung.cn

[U40] Py：打印到标准错误
来源：http://up.hnjuh.cn

print("err", file=sys.stderr)
来源：http://dy.521024.cn

[U41] PHP：初始化 Composer 项目
来源：http://za.nicolike.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://wr.lnxyls.cn

[U42] PHP：PSR-4 自动加载
来源：http://se.shxzukj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://tb.muxihuayi.cn

[U43] PHP：声明命名空间
来源：http://di.huixiangedu.cn

namespace App\Http;
来源：http://qd.shtwfgs.cn

[U44] PHP：开启严格类型
来源：http://rx.hnjuh.cn

declare(strict_types=1);
来源：http://bo.jianghongdianzi.cn

[U45] PHP：类型声明与返回类型
来源：http://qr.szsharing.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://zl.bookmarksfly.cn

[U46] PHP：可空类型
来源：http://cv.huixiangedu.cn

?string $name = null
来源：http://lm.521024.cn


<!-- 参考信息 -->