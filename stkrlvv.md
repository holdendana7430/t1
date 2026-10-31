代发 wailian999

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ln.muxihuayi.cn

[S25] C：内存拷贝
来源：http://oh.yuntaijiaju.cn

memcpy(dst, src, n);
来源：http://ne.colortex.cn

[S26] C：内存清零
来源：http://ss.huixiangedu.cn

memset(a, 0, sizeof a);
来源：http://sg.hahajie.cn

[S27] C：定义常量
来源：http://rr.panjiajie.cn

const double PI = 3.14159;
来源：http://an.9csxet.cn

[S28] C：静态变量
来源：http://cd.haigaiapp.cn

static int counter = 0;
来源：http://yl.jianghongdianzi.cn

[S29] C：变参函数
来源：http://eu.chemitech.net.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://nx.muxihuayi.cn

[S30] C：头文件保护
来源：http://dk.bookmarksfly.cn

#ifndef X_H
来源：http://xi.jianghongdianzi.cn

#define X_H
来源：http://ky.521024.cn

#endif
来源：http://dq.gzmigu.cn

[S31] C++：Hello World
来源：http://ss.haigaiapp.cn

#include <iostream>
来源：http://bz.huanxung.cn

int main() { std::cout << "Hello\n"; }
来源：http://sf.9csxet.cn

[S32] C++：字符串
来源：http://vo.huanxung.cn

std::string s = "hi";  s += "!";
来源：http://gt.asd995.cn

[S33] C++：vector 增删
来源：http://ns.szsharing.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ah.hahajie.cn

[S34] C++：遍历 vector
来源：http://mg.hnjuh.cn

for (auto &x : v) { std::cout << x; }
来源：http://rr.nicolike.cn

[S35] C++：map
来源：http://rp.huixiangedu.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://bv.yuntaijiaju.cn

[S36] C++：unordered_map
来源：http://ev.newstarts.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ma.muxihuayi.cn

[S37] C++：set
来源：http://ci.yuntaijiaju.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ur.yuexingan06.cn

[S38] C++：排序
来源：http://dk.shxzskj.cn

std::sort(v.begin(), v.end());
来源：http://uc.panjiajie.cn

[S39] C++：自定义比较器排序
来源：http://ke.yuexingan06.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://uk.szxytkj.cn

[S40] C++：查找元素
来源：http://ch.huanxung.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://jl.wgjwhj.cn

[S41] C++：类与构造函数
来源：http://jg.bookmarksfly.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://al.bjjhwx.cn

[S42] C++：继承与虚函数
来源：http://ks.wgjwhj.cn

class B : public Base { public: void f() override {} };
来源：http://ek.shxzukj.cn

[S43] C++：智能指针
来源：http://aa.shtwfgs.cn

auto p = std::make_unique<int>(5);
来源：http://em.nszjky.cn

[S44] C++：引用传参
来源：http://ia.hnjuh.cn

void inc(int &x) { ++x; }
来源：http://yw.szxytkj.cn

[S45] C++：lambda
来源：http://os.huixinmuqiang.cn

auto add = [](int a, int b) { return a + b; };
来源：http://cx.gzmigu.cn

[S46] C++：函数模板
来源：http://yn.nszjky.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://bk.szxytkj.cn

[S47] C++：结构化绑定遍历
来源：http://wp.szxytkj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mv.huanxung.cn

[S48] C++：逐行读文件
来源：http://mn.muxihuayi.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ln.lnxyls.cn

while (std::getline(in, line)) { }
来源：http://yg.muxihuayi.cn

[S49] C++：写文件
来源：http://ue.nicolike.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://mk.gzmigu.cn

[S50] C++：格式化数字
来源：http://ky.yuntaijiaju.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://yz.shtwfgs.cn

[S51] C++：显式类型转换
来源：http://pn.hahajie.cn

static_cast<double>(a) / b
来源：http://ea.huixinmuqiang.cn

[S52] C++：const 与 noexcept
来源：http://jk.yuexingan06.cn

int size() const noexcept { return n_; }
来源：http://yz.szsharing.cn

[S53] C++：移动语义
来源：http://xl.szxytkj.cn

std::vector<int> w = std::move(v);
来源：http://fa.nszjky.cn

[S54] C++：异常处理
来源：http://sq.9csxet.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://dj.panjiajie.cn

[S55] C++：结构化绑定
来源：http://ht.nicolike.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ud.panjiajie.cn

[S56] C++：optional
来源：http://dr.jianghongdianzi.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://un.wgjwhj.cn

[S57] C++：编译期常量
来源：http://ix.521024.cn

constexpr int N = 10;
来源：http://fp.panjiajie.cn

[S58] C++：命名空间
来源：http://lr.lnxyls.cn

namespace ns { int f() { return 1; } }
来源：http://gb.hahajie.cn

[S59] C++：静态断言
来源：http://wg.wgjwhj.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fl.huixiangedu.cn

[S60] C++：遍历并删除元素
来源：http://ow.chemitech.net.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://cv.wgjwhj.cn

================================================================================
来源：http://tb.colortex.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://vj.chemitech.net.cn

================================================================================
来源：http://xs.hahajie.cn

[T01] Kotlin：Hello World
来源：http://zb.wgjwhj.cn

println("Hello")
来源：http://cg.9csxet.cn

[T02] Kotlin：变量
来源：http://vz.shtwfgs.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wf.yuntaijiaju.cn

[T03] Kotlin：字符串模板
来源：http://zk.asd995.cn

"值: $b"
来源：http://us.shtwfgs.cn

[T04] Kotlin：空安全
来源：http://fy.newstarts.cn

val n: String? = null;  n?.length
来源：http://wm.huanxung.cn

[T05] Kotlin：when 表达式
来源：http://hn.huixiangedu.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://yk.panjiajie.cn

[T06] Kotlin：集合映射
来源：http://lv.haigaiapp.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://zm.huanxung.cn

[T07] Kotlin：集合过滤
来源：http://db.bjjhwx.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://zo.nicolike.cn

[T08] Kotlin：数据类
来源：http://mw.gzmigu.cn

data class User(val name: String, val age: Int)
来源：http://za.hnjuh.cn

[T09] Kotlin：扩展函数
来源：http://ns.shxzukj.cn

fun String.exclaim() = this + "!"
来源：http://cu.bookmarksfly.cn

[T10] Kotlin：默认参数
来源：http://jp.shxzskj.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://up.huixinmuqiang.cn

[T11] Kotlin：协程
来源：http://hq.jianghongdianzi.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://bc.yuntaijiaju.cn

[T12] Kotlin：解构声明
来源：http://ei.huanxung.cn

val (a, b) = Pair(1, 2)
来源：http://xh.szxytkj.cn

[T13] Kotlin：只读 Map
来源：http://go.shxzskj.cn

val m = mapOf("a" to 1)
来源：http://wl.panjiajie.cn

[T14] Kotlin：循环
来源：http://bd.panjiajie.cn

for (i in 1..10) println(i)
来源：http://da.shxzukj.cn

[T15] Kotlin：接口
来源：http://pv.shxzukj.cn

interface Shape { fun area(): Double }
来源：http://eu.nszjky.cn

[T16] Swift：Hello World
来源：http://bh.muxihuayi.cn

print("Hello")
来源：http://ew.huanxung.cn

[T17] Swift：变量与常量
来源：http://vf.wgjwhj.cn

var a = 1;  let b = 2
来源：http://ax.yuntaijiaju.cn

[T18] Swift：字符串插值
来源：http://kp.lnxyls.cn

"值: \(b)"
来源：http://km.jianghongdianzi.cn

[T19] Swift：可选绑定
来源：http://nc.colortex.cn

if let n = opt { print(n) }
来源：http://zw.panjiajie.cn

[T20] Swift：数组操作
来源：http://ya.shxzskj.cn

var a = [1, 2, 3];  a.append(4)
来源：http://qz.huanxung.cn

[T21] Swift：遍历
来源：http://qg.huixiangedu.cn

for x in a { print(x) }
来源：http://la.9csxet.cn

[T22] Swift：字典
来源：http://zd.bookmarksfly.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ke.9csxet.cn

[T23] Swift：函数
来源：http://gg.gzmigu.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://dg.yuexingan06.cn

[T24] Swift：闭包
来源：http://zk.szxytkj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://zd.9csxet.cn

[T25] Swift：结构体
来源：http://tn.gzmigu.cn

struct P { var x: Int }
来源：http://ml.asd995.cn

[T26] Swift：类与重写
来源：http://bl.shtwfgs.cn

class A: Base { override func f() {} }
来源：http://qj.haigaiapp.cn

[T27] Swift：错误处理
来源：http://vv.chemitech.net.cn

do { try f() } catch { print(error) }
来源：http://ep.lnxyls.cn

[T28] Swift：枚举
来源：http://xm.yuntaijiaju.cn

enum Color { case red, green }
来源：http://sm.yuexingan06.cn

[T29] Swift：guard 提前返回
来源：http://ru.bookmarksfly.cn

guard let x = opt else { return }
来源：http://xx.hahajie.cn

[T30] Swift：协议
来源：http://cy.bookmarksfly.cn

protocol Shape { func area() -> Double }
来源：http://gg.yuntaijiaju.cn

[T31] Lua：Hello World
来源：http://co.huixiangedu.cn

print("Hello")
来源：http://br.bookmarksfly.cn

[T32] Lua：局部变量
来源：http://dk.521024.cn

local a = 1
来源：http://qd.asd995.cn

[T33] Lua：表（数组）
来源：http://fa.hnjuh.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://lo.chemitech.net.cn

[T34] Lua：遍历表
来源：http://sm.panjiajie.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://sv.huixinmuqiang.cn

[T35] Lua：字典表
来源：http://se.chemitech.net.cn

local d = { a = 1 };  d.b = 2
来源：http://ie.jianghongdianzi.cn

[T36] Lua：函数
来源：http://cq.shxzukj.cn

function add(a, b) return a + b end
来源：http://hs.colortex.cn

[T37] Lua：字符串拼接
来源：http://is.colortex.cn

"a" .. "b"
来源：http://fa.nszjky.cn

[T38] Lua：条件
来源：http://yj.lnxyls.cn

if x > 0 then print("正") end
来源：http://ju.shxzskj.cn

[T39] Lua：模式匹配
来源：http://sq.colortex.cn

string.find(s, "%d+")
来源：http://de.nicolike.cn

[T40] Lua：元表
来源：http://hi.shxzukj.cn

setmetatable({}, { __index = base })
来源：http://rw.huixiangedu.cn

[T41] Perl：Hello World
来源：http://sb.yuntaijiaju.cn

print "Hello\n";
来源：http://da.wgjwhj.cn

[T42] Perl：变量类型
来源：http://wk.colortex.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://be.szxytkj.cn

[T43] Perl：字符串插值
来源：http://dk.yuntaijiaju.cn

"值: $a"
来源：http://sr.shxzukj.cn

[T44] Perl：条件
来源：http://le.jianghongdianzi.cn

if ($a > 0) { print "正"; }
来源：http://za.hahajie.cn

[T45] Perl：数组遍历
来源：http://qm.nicolike.cn

for my $x (@arr) { print $x; }
来源：http://cz.szsharing.cn

[T46] Perl：哈希操作
来源：http://er.hnjuh.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://xo.huanxung.cn

[T47] Perl：正则捕获
来源：http://xw.szxytkj.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ij.gzmigu.cn

[T48] Perl：正则替换
来源：http://em.lnxyls.cn

$s =~ s/old/new/g;
来源：http://lr.hahajie.cn

[T49] Perl：函数
来源：http://vi.colortex.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hg.gzmigu.cn

[T50] Perl：逐行读文件
来源：http://fv.bookmarksfly.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ai.9csxet.cn

while (my $line = <$fh>) { print $line; }
来源：http://mj.szxytkj.cn

[T51] Scala：Hello World
来源：http://mz.jianghongdianzi.cn

println("Hello")
来源：http://as.panjiajie.cn

[T52] Scala：变量
来源：http://jp.muxihuayi.cn

val a = 1;  var b = 2
来源：http://vv.asd995.cn

[T53] Scala：字符串插值
来源：http://qk.9csxet.cn

s"值: $b"
来源：http://tt.9csxet.cn

[T54] Scala：集合映射
来源：http://dd.jianghongdianzi.cn

List(1, 2, 3).map(_ * 2)
来源：http://yi.shtwfgs.cn

[T55] Scala：集合过滤
来源：http://qw.521024.cn

List(1, 2, 3).filter(_ > 1)
来源：http://fm.wgjwhj.cn

[T56] Scala：样例类
来源：http://lp.shtwfgs.cn

case class User(name: String, age: Int)
来源：http://yw.huanxung.cn

[T57] Scala：模式匹配
来源：http://bm.bjjhwx.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ox.szsharing.cn

[T58] Scala：函数定义
来源：http://gn.shxzskj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://sg.bookmarksfly.cn

[T59] Scala：循环
来源：http://yy.wgjwhj.cn

for (i <- 1 to 10) println(i)
来源：http://yz.nszjky.cn

[T60] Scala：折叠
来源：http://re.yuntaijiaju.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://fw.521024.cn

================================================================================
来源：http://qg.chemitech.net.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://dw.huanxung.cn

================================================================================
来源：http://di.newstarts.cn

[U01] Py：创建虚拟环境
来源：http://ak.huanxung.cn

python -m venv .venv && source .venv/bin/activate
来源：http://je.panjiajie.cn

[U02] Py：导出 / 安装依赖
来源：http://fc.huanxung.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://nb.huixinmuqiang.cn

[U03] Py：加载 .env 配置
来源：http://uz.colortex.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://jh.hahajie.cn

[U04] Py：变量调试打印
来源：http://hf.huixiangedu.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://os.gzmigu.cn

[U05] Py：列表去重且保序
来源：http://rx.521024.cn

list(dict.fromkeys(arr))
来源：http://nh.hahajie.cn

[U06] Py：合并两个字典
来源：http://tk.shxzskj.cn

{**a, **b}
来源：http://ea.wgjwhj.cn

[U07] Py：反转字典键值
来源：http://is.colortex.cn

{v: k for k, v in d.items()}
来源：http://uv.colortex.cn

[U08] Py：展平二维列表
来源：http://dg.chemitech.net.cn

[y for x in nested for y in x]
来源：http://hs.szxytkj.cn

[U09] Py：字典取最大值的键
来源：http://sk.huanxung.cn

max(d, key=d.get)
来源：http://re.huixiangedu.cn

[U10] Py：按值排序字典
来源：http://xy.yuexingan06.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://qd.jianghongdianzi.cn

[U11] Py：生成器表达式
来源：http://bu.wgjwhj.cn

(x * 2 for x in arr)
来源：http://se.chemitech.net.cn

[U12] Py：取出现最多的 3 个元素
来源：http://hq.huixiangedu.cn

Counter(arr).most_common(3)
来源：http://mk.shxzskj.cn

[U13] Py：固定长度队列
来源：http://uc.muxihuayi.cn

deque(maxlen=10)
来源：http://kh.hnjuh.cn

[U14] Py：分组收集到列表
来源：http://zf.9csxet.cn

defaultdict(list)
来源：http://rd.hnjuh.cn

[U15] Py：高精度计时
来源：http://ls.newstarts.cn

t = time.perf_counter()
来源：http://mm.521024.cn

[U16] Py：命令行参数解析
来源：http://ay.hahajie.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://mf.shxzskj.cn

[U17] Py：初始化日志
来源：http://kp.jctech888.com.cn

logging.basicConfig(level=logging.INFO)
来源：http://ub.chemitech.net.cn

[U18] Py：预编译正则
来源：http://it.newstarts.cn

pat = re.compile(r"\d+")
来源：http://mq.shxzukj.cn

[U19] Py：正则替换带回调
来源：http://wm.gzmigu.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://fd.nszjky.cn

[U20] Py：缓存函数结果
来源：http://mp.hahajie.cn

@functools.lru_cache(maxsize=None)
来源：http://eg.lnxyls.cn

[U21] Py：自定义上下文管理器
来源：http://bk.chemitech.net.cn

@contextlib.contextmanager
来源：http://mm.colortex.cn

[U22] Py：矩阵转置
来源：http://mt.newstarts.cn

list(zip(*m))
来源：http://dh.nszjky.cn

[U23] Py：分块读取大文件
来源：http://js.yuexingan06.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://xp.newstarts.cn

[U24] Py：路径操作
来源：http://dn.shxzskj.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ns.hnjuh.cn

[U25] Py：CSV 按字典读
来源：http://jr.colortex.cn

csv.DictReader(f)
来源：http://rn.gzmigu.cn

[U26] Py：并发下载
来源：http://rv.nicolike.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://fc.521024.cn

[U27] Py：异步 HTTP
来源：http://yl.9csxet.cn

aiohttp.ClientSession() 配合 async with
来源：http://zz.jctech888.com.cn

[U28] Py：类型别名
来源：http://jt.yuexingan06.cn

UserId = int
来源：http://er.hnjuh.cn

[U29] Py：属性校验
来源：http://tr.nszjky.cn

@property 与 @x.setter 配合
来源：http://tp.hnjuh.cn

[U30] Py：数据类
来源：http://ja.shxzukj.cn

@dataclass(slots=True)
来源：http://su.gzmigu.cn

[U31] Py：单测
来源：http://oz.lnxyls.cn

python -m pytest -q
来源：http://uv.huixinmuqiang.cn

[U32] Py：代码格式化
来源：http://lh.wgjwhj.cn

ruff format . && ruff check --fix .
来源：http://tj.jianghongdianzi.cn

[U33] Py：打包发布
来源：http://uw.yuexingan06.cn

python -m build  （依赖 pyproject.toml）
来源：http://ti.hahajie.cn

[U34] Py：判断编码
来源：http://ow.jctech888.com.cn

chardet.detect(raw)
来源：http://pn.shxzskj.cn

[U35] Py：发送邮件
来源：http://fc.wgjwhj.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://sc.yuexingan06.cn

[U36] Py：定时任务
来源：http://eg.yuexingan06.cn

schedule.every(10).minutes.do(job)
来源：http://wr.huanxung.cn

[U37] Py：读写 Excel
来源：http://lp.521024.cn

pandas.read_excel / DataFrame.to_excel
来源：http://vf.asd995.cn

[U38] Py：获取脚本所在目录
来源：http://kx.521024.cn

Path(__file__).resolve().parent
来源：http://bu.bookmarksfly.cn

[U39] Py：判断是否在交互环境
来源：http://xg.jianghongdianzi.cn

sys.stdout.isatty()
来源：http://vq.lnxyls.cn

[U40] Py：打印到标准错误
来源：http://px.bjjhwx.cn

print("err", file=sys.stderr)
来源：http://um.jianghongdianzi.cn

[U41] PHP：初始化 Composer 项目
来源：http://cm.huixiangedu.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://el.huixinmuqiang.cn

[U42] PHP：PSR-4 自动加载
来源：http://po.huanxung.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://rg.huanxung.cn

[U43] PHP：声明命名空间
来源：http://uf.huixiangedu.cn

namespace App\Http;
来源：http://at.jctech888.com.cn

[U44] PHP：开启严格类型
来源：http://za.chemitech.net.cn

declare(strict_types=1);
来源：http://fh.newstarts.cn

[U45] PHP：类型声明与返回类型
来源：http://xp.jianghongdianzi.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://qg.haigaiapp.cn

[U46] PHP：可空类型
来源：http://wd.nicolike.cn

?string $name = null
来源：http://fs.huanxung.cn

[U47] PHP：联合类型
来源：http://ex.szxytkj.cn

int|string $id
来源：http://lq.hnjuh.cn

[U48] PHP：纯枚举
来源：http://xl.jctech888.com.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://yv.hnjuh.cn


<!-- 参考信息 -->