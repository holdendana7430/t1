代发 wailian999

memset(a, 0, sizeof a);
来源：http://hz.9csxet.cn

[S27] C：定义常量
来源：http://vl.nicolike.cn

const double PI = 3.14159;
来源：http://ez.huixiangedu.cn

[S28] C：静态变量
来源：http://qm.szsharing.cn

static int counter = 0;
来源：http://nl.nszjky.cn

[S29] C：变参函数
来源：http://fd.shxzskj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ou.521024.cn

[S30] C：头文件保护
来源：http://qe.shxzukj.cn

#ifndef X_H
来源：http://jv.hnjuh.cn

#define X_H
来源：http://gi.haigaiapp.cn

#endif
来源：http://ws.521024.cn

[S31] C++：Hello World
来源：http://hm.szxytkj.cn

#include <iostream>
来源：http://md.colortex.cn

int main() { std::cout << "Hello\n"; }
来源：http://qz.nszjky.cn

[S32] C++：字符串
来源：http://gk.jctech888.com.cn

std::string s = "hi";  s += "!";
来源：http://xe.szsharing.cn

[S33] C++：vector 增删
来源：http://mc.gzmigu.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://kr.szsharing.cn

[S34] C++：遍历 vector
来源：http://sp.hahajie.cn

for (auto &x : v) { std::cout << x; }
来源：http://mw.huanxung.cn

[S35] C++：map
来源：http://rl.muxihuayi.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ax.gzmigu.cn

[S36] C++：unordered_map
来源：http://ll.panjiajie.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ns.9csxet.cn

[S37] C++：set
来源：http://la.colortex.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://nn.9csxet.cn

[S38] C++：排序
来源：http://mx.panjiajie.cn

std::sort(v.begin(), v.end());
来源：http://pj.huixinmuqiang.cn

[S39] C++：自定义比较器排序
来源：http://ws.nicolike.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ou.huixiangedu.cn

[S40] C++：查找元素
来源：http://uj.asd995.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://jv.asd995.cn

[S41] C++：类与构造函数
来源：http://au.shxzukj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ev.lnxyls.cn

[S42] C++：继承与虚函数
来源：http://ns.lnxyls.cn

class B : public Base { public: void f() override {} };
来源：http://kp.hnjuh.cn

[S43] C++：智能指针
来源：http://vs.yuexingan06.cn

auto p = std::make_unique<int>(5);
来源：http://cd.9csxet.cn

[S44] C++：引用传参
来源：http://kq.shtwfgs.cn

void inc(int &x) { ++x; }
来源：http://vr.huixinmuqiang.cn

[S45] C++：lambda
来源：http://vr.szxytkj.cn

auto add = [](int a, int b) { return a + b; };
来源：http://rm.lnxyls.cn

[S46] C++：函数模板
来源：http://pk.bjjhwx.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://zk.newstarts.cn

[S47] C++：结构化绑定遍历
来源：http://ep.huixiangedu.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://zh.gzmigu.cn

[S48] C++：逐行读文件
来源：http://dx.huixinmuqiang.cn

std::ifstream in("a.txt");  std::string line;
来源：http://qd.lnxyls.cn

while (std::getline(in, line)) { }
来源：http://hf.szxytkj.cn

[S49] C++：写文件
来源：http://sx.muxihuayi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://je.nszjky.cn

[S50] C++：格式化数字
来源：http://vy.lnxyls.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://rc.yuexingan06.cn

[S51] C++：显式类型转换
来源：http://yv.gzmigu.cn

static_cast<double>(a) / b
来源：http://pk.nszjky.cn

[S52] C++：const 与 noexcept
来源：http://ld.szsharing.cn

int size() const noexcept { return n_; }
来源：http://zu.yuntaijiaju.cn

[S53] C++：移动语义
来源：http://tf.bookmarksfly.cn

std::vector<int> w = std::move(v);
来源：http://pl.szsharing.cn

[S54] C++：异常处理
来源：http://og.huixiangedu.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://nv.bjjhwx.cn

[S55] C++：结构化绑定
来源：http://ow.hahajie.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://kp.chemitech.net.cn

[S56] C++：optional
来源：http://xr.bjjhwx.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://dd.shtwfgs.cn

[S57] C++：编译期常量
来源：http://ig.jctech888.com.cn

constexpr int N = 10;
来源：http://jq.wgjwhj.cn

[S58] C++：命名空间
来源：http://uc.szxytkj.cn

namespace ns { int f() { return 1; } }
来源：http://eb.newstarts.cn

[S59] C++：静态断言
来源：http://zd.nicolike.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://yh.shxzukj.cn

[S60] C++：遍历并删除元素
来源：http://wq.nszjky.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://nc.wgjwhj.cn

================================================================================
来源：http://pb.shtwfgs.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://jz.huanxung.cn

================================================================================
来源：http://br.9csxet.cn

[T01] Kotlin：Hello World
来源：http://ih.szxytkj.cn

println("Hello")
来源：http://gq.jctech888.com.cn

[T02] Kotlin：变量
来源：http://lo.huixinmuqiang.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://pu.newstarts.cn

[T03] Kotlin：字符串模板
来源：http://xu.9csxet.cn

"值: $b"
来源：http://qh.nszjky.cn

[T04] Kotlin：空安全
来源：http://qu.asd995.cn

val n: String? = null;  n?.length
来源：http://ph.9csxet.cn

[T05] Kotlin：when 表达式
来源：http://vn.chemitech.net.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://si.yuntaijiaju.cn

[T06] Kotlin：集合映射
来源：http://dt.szsharing.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://wb.shxzukj.cn

[T07] Kotlin：集合过滤
来源：http://jc.shxzskj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://vz.chemitech.net.cn

[T08] Kotlin：数据类
来源：http://mm.huixiangedu.cn

data class User(val name: String, val age: Int)
来源：http://rw.yuexingan06.cn

[T09] Kotlin：扩展函数
来源：http://ev.panjiajie.cn

fun String.exclaim() = this + "!"
来源：http://sf.huixiangedu.cn

[T10] Kotlin：默认参数
来源：http://qp.huixinmuqiang.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://lm.huanxung.cn

[T11] Kotlin：协程
来源：http://yn.hahajie.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://am.haigaiapp.cn

[T12] Kotlin：解构声明
来源：http://ox.szsharing.cn

val (a, b) = Pair(1, 2)
来源：http://mm.shtwfgs.cn

[T13] Kotlin：只读 Map
来源：http://sn.shxzskj.cn

val m = mapOf("a" to 1)
来源：http://ps.bjjhwx.cn

[T14] Kotlin：循环
来源：http://uh.szsharing.cn

for (i in 1..10) println(i)
来源：http://wx.haigaiapp.cn

[T15] Kotlin：接口
来源：http://is.colortex.cn

interface Shape { fun area(): Double }
来源：http://ri.yuexingan06.cn

[T16] Swift：Hello World
来源：http://ja.bjjhwx.cn

print("Hello")
来源：http://ki.lnxyls.cn

[T17] Swift：变量与常量
来源：http://us.jianghongdianzi.cn

var a = 1;  let b = 2
来源：http://ls.muxihuayi.cn

[T18] Swift：字符串插值
来源：http://am.chemitech.net.cn

"值: \(b)"
来源：http://vf.chemitech.net.cn

[T19] Swift：可选绑定
来源：http://qg.shxzskj.cn

if let n = opt { print(n) }
来源：http://ex.shtwfgs.cn

[T20] Swift：数组操作
来源：http://ma.9csxet.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ec.huixiangedu.cn

[T21] Swift：遍历
来源：http://gz.newstarts.cn

for x in a { print(x) }
来源：http://gp.huixiangedu.cn

[T22] Swift：字典
来源：http://lt.asd995.cn

var d = ["a": 1];  d["b"] = 2
来源：http://yk.bookmarksfly.cn

[T23] Swift：函数
来源：http://gz.shtwfgs.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://pt.gzmigu.cn

[T24] Swift：闭包
来源：http://nz.chemitech.net.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ly.wgjwhj.cn

[T25] Swift：结构体
来源：http://hu.jianghongdianzi.cn

struct P { var x: Int }
来源：http://ma.521024.cn

[T26] Swift：类与重写
来源：http://yv.shtwfgs.cn

class A: Base { override func f() {} }
来源：http://mj.huanxung.cn

[T27] Swift：错误处理
来源：http://gl.asd995.cn

do { try f() } catch { print(error) }
来源：http://ot.shtwfgs.cn

[T28] Swift：枚举
来源：http://jr.huixiangedu.cn

enum Color { case red, green }
来源：http://cm.colortex.cn

[T29] Swift：guard 提前返回
来源：http://vg.bookmarksfly.cn

guard let x = opt else { return }
来源：http://tx.wgjwhj.cn

[T30] Swift：协议
来源：http://fw.gzmigu.cn

protocol Shape { func area() -> Double }
来源：http://fu.huanxung.cn

[T31] Lua：Hello World
来源：http://ah.yuntaijiaju.cn

print("Hello")
来源：http://lp.panjiajie.cn

[T32] Lua：局部变量
来源：http://wj.yuexingan06.cn

local a = 1
来源：http://ja.9csxet.cn

[T33] Lua：表（数组）
来源：http://oh.jctech888.com.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ht.jianghongdianzi.cn

[T34] Lua：遍历表
来源：http://ja.9csxet.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://xw.haigaiapp.cn

[T35] Lua：字典表
来源：http://bk.shxzskj.cn

local d = { a = 1 };  d.b = 2
来源：http://xr.jianghongdianzi.cn

[T36] Lua：函数
来源：http://mb.hnjuh.cn

function add(a, b) return a + b end
来源：http://th.bookmarksfly.cn

[T37] Lua：字符串拼接
来源：http://ey.hnjuh.cn

"a" .. "b"
来源：http://gu.bjjhwx.cn

[T38] Lua：条件
来源：http://ki.panjiajie.cn

if x > 0 then print("正") end
来源：http://yz.hnjuh.cn

[T39] Lua：模式匹配
来源：http://cl.shxzukj.cn

string.find(s, "%d+")
来源：http://az.yuexingan06.cn

[T40] Lua：元表
来源：http://zx.colortex.cn

setmetatable({}, { __index = base })
来源：http://qa.huixiangedu.cn

[T41] Perl：Hello World
来源：http://ig.shxzskj.cn

print "Hello\n";
来源：http://rh.shxzukj.cn

[T42] Perl：变量类型
来源：http://bu.shxzukj.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://nc.huixinmuqiang.cn

[T43] Perl：字符串插值
来源：http://yb.hnjuh.cn

"值: $a"
来源：http://sa.colortex.cn

[T44] Perl：条件
来源：http://ca.shxzukj.cn

if ($a > 0) { print "正"; }
来源：http://az.szsharing.cn

[T45] Perl：数组遍历
来源：http://dh.yuexingan06.cn

for my $x (@arr) { print $x; }
来源：http://up.521024.cn

[T46] Perl：哈希操作
来源：http://ae.shtwfgs.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://fa.shxzskj.cn

[T47] Perl：正则捕获
来源：http://dt.shxzukj.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ij.521024.cn

[T48] Perl：正则替换
来源：http://yb.nszjky.cn

$s =~ s/old/new/g;
来源：http://ll.bookmarksfly.cn

[T49] Perl：函数
来源：http://lm.colortex.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ay.hahajie.cn

[T50] Perl：逐行读文件
来源：http://ll.newstarts.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://jb.newstarts.cn

while (my $line = <$fh>) { print $line; }
来源：http://gb.hnjuh.cn

[T51] Scala：Hello World
来源：http://fz.jianghongdianzi.cn

println("Hello")
来源：http://ud.huixinmuqiang.cn

[T52] Scala：变量
来源：http://xa.muxihuayi.cn

val a = 1;  var b = 2
来源：http://py.muxihuayi.cn

[T53] Scala：字符串插值
来源：http://oa.yuexingan06.cn

s"值: $b"
来源：http://wz.9csxet.cn

[T54] Scala：集合映射
来源：http://tv.shxzukj.cn

List(1, 2, 3).map(_ * 2)
来源：http://ic.521024.cn

[T55] Scala：集合过滤
来源：http://hk.lnxyls.cn

List(1, 2, 3).filter(_ > 1)
来源：http://cd.shxzukj.cn

[T56] Scala：样例类
来源：http://bj.hahajie.cn

case class User(name: String, age: Int)
来源：http://em.shxzukj.cn

[T57] Scala：模式匹配
来源：http://pj.yuntaijiaju.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://eb.asd995.cn

[T58] Scala：函数定义
来源：http://km.asd995.cn

def add(a: Int, b: Int): Int = a + b
来源：http://uq.9csxet.cn

[T59] Scala：循环
来源：http://zw.huixiangedu.cn

for (i <- 1 to 10) println(i)
来源：http://xf.bookmarksfly.cn

[T60] Scala：折叠
来源：http://oe.yuexingan06.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://io.nszjky.cn

================================================================================
来源：http://lf.yuexingan06.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wk.huanxung.cn

================================================================================
来源：http://ud.yuntaijiaju.cn

[U01] Py：创建虚拟环境
来源：http://ey.hnjuh.cn

python -m venv .venv && source .venv/bin/activate
来源：http://zq.hahajie.cn

[U02] Py：导出 / 安装依赖
来源：http://xa.nszjky.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://sg.szsharing.cn

[U03] Py：加载 .env 配置
来源：http://mx.yuexingan06.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://yj.haigaiapp.cn

[U04] Py：变量调试打印
来源：http://ty.huixinmuqiang.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://dm.gzmigu.cn

[U05] Py：列表去重且保序
来源：http://hf.shxzukj.cn

list(dict.fromkeys(arr))
来源：http://me.yuntaijiaju.cn

[U06] Py：合并两个字典
来源：http://zz.shxzskj.cn

{**a, **b}
来源：http://ty.haigaiapp.cn

[U07] Py：反转字典键值
来源：http://nh.huanxung.cn

{v: k for k, v in d.items()}
来源：http://gm.shxzskj.cn

[U08] Py：展平二维列表
来源：http://us.haigaiapp.cn

[y for x in nested for y in x]
来源：http://wk.haigaiapp.cn

[U09] Py：字典取最大值的键
来源：http://bt.yuntaijiaju.cn

max(d, key=d.get)
来源：http://qy.shtwfgs.cn

[U10] Py：按值排序字典
来源：http://gd.panjiajie.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://mh.wgjwhj.cn

[U11] Py：生成器表达式
来源：http://ja.newstarts.cn

(x * 2 for x in arr)
来源：http://hz.shxzskj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://pt.wgjwhj.cn

Counter(arr).most_common(3)
来源：http://sa.muxihuayi.cn

[U13] Py：固定长度队列
来源：http://hr.hnjuh.cn

deque(maxlen=10)
来源：http://wz.shxzskj.cn

[U14] Py：分组收集到列表
来源：http://wg.bjjhwx.cn

defaultdict(list)
来源：http://qi.hnjuh.cn

[U15] Py：高精度计时
来源：http://bq.huixinmuqiang.cn

t = time.perf_counter()
来源：http://bt.chemitech.net.cn

[U16] Py：命令行参数解析
来源：http://kp.521024.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://gw.nicolike.cn

[U17] Py：初始化日志
来源：http://gl.szsharing.cn

logging.basicConfig(level=logging.INFO)
来源：http://el.wgjwhj.cn

[U18] Py：预编译正则
来源：http://kv.yuexingan06.cn

pat = re.compile(r"\d+")
来源：http://dr.hahajie.cn

[U19] Py：正则替换带回调
来源：http://cc.yuntaijiaju.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://do.bookmarksfly.cn

[U20] Py：缓存函数结果
来源：http://ee.huixinmuqiang.cn

@functools.lru_cache(maxsize=None)
来源：http://pg.lnxyls.cn

[U21] Py：自定义上下文管理器
来源：http://bo.lnxyls.cn

@contextlib.contextmanager
来源：http://ro.haigaiapp.cn

[U22] Py：矩阵转置
来源：http://dp.bjjhwx.cn

list(zip(*m))
来源：http://sw.hahajie.cn

[U23] Py：分块读取大文件
来源：http://ht.nicolike.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://qh.bookmarksfly.cn

[U24] Py：路径操作
来源：http://hn.chemitech.net.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://bh.wgjwhj.cn

[U25] Py：CSV 按字典读
来源：http://su.shtwfgs.cn

csv.DictReader(f)
来源：http://dd.yuntaijiaju.cn

[U26] Py：并发下载
来源：http://hb.shxzskj.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://df.yuexingan06.cn

[U27] Py：异步 HTTP
来源：http://re.huixinmuqiang.cn

aiohttp.ClientSession() 配合 async with
来源：http://si.jctech888.com.cn

[U28] Py：类型别名
来源：http://qp.haigaiapp.cn

UserId = int
来源：http://co.shtwfgs.cn

[U29] Py：属性校验
来源：http://rf.colortex.cn

@property 与 @x.setter 配合
来源：http://fo.yuntaijiaju.cn

[U30] Py：数据类
来源：http://uh.bjjhwx.cn

@dataclass(slots=True)
来源：http://sc.chemitech.net.cn

[U31] Py：单测
来源：http://qy.chemitech.net.cn

python -m pytest -q
来源：http://ai.hnjuh.cn

[U32] Py：代码格式化
来源：http://jz.shxzskj.cn

ruff format . && ruff check --fix .
来源：http://fl.yuntaijiaju.cn

[U33] Py：打包发布
来源：http://cj.hnjuh.cn

python -m build  （依赖 pyproject.toml）
来源：http://ky.huixinmuqiang.cn

[U34] Py：判断编码
来源：http://og.bjjhwx.cn

chardet.detect(raw)
来源：http://ou.shtwfgs.cn

[U35] Py：发送邮件
来源：http://so.bjjhwx.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://nv.haigaiapp.cn

[U36] Py：定时任务
来源：http://cw.huanxung.cn

schedule.every(10).minutes.do(job)
来源：http://xl.shtwfgs.cn

[U37] Py：读写 Excel
来源：http://tc.hahajie.cn

pandas.read_excel / DataFrame.to_excel
来源：http://sc.muxihuayi.cn

[U38] Py：获取脚本所在目录
来源：http://bc.colortex.cn

Path(__file__).resolve().parent
来源：http://fy.wgjwhj.cn

[U39] Py：判断是否在交互环境
来源：http://lu.521024.cn

sys.stdout.isatty()
来源：http://mg.nszjky.cn

[U40] Py：打印到标准错误
来源：http://ut.szxytkj.cn

print("err", file=sys.stderr)
来源：http://jy.lnxyls.cn

[U41] PHP：初始化 Composer 项目
来源：http://xk.nszjky.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://qa.panjiajie.cn

[U42] PHP：PSR-4 自动加载
来源：http://bo.newstarts.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://dy.yuexingan06.cn

[U43] PHP：声明命名空间
来源：http://en.haigaiapp.cn

namespace App\Http;
来源：http://jt.asd995.cn

[U44] PHP：开启严格类型
来源：http://ik.huixinmuqiang.cn

declare(strict_types=1);
来源：http://no.huanxung.cn

[U45] PHP：类型声明与返回类型
来源：http://ei.9csxet.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://iv.asd995.cn

[U46] PHP：可空类型
来源：http://iu.haigaiapp.cn

?string $name = null
来源：http://ep.szsharing.cn

[U47] PHP：联合类型
来源：http://ok.hahajie.cn

int|string $id
来源：http://ba.colortex.cn

[U48] PHP：纯枚举
来源：http://bi.colortex.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://gx.yuntaijiaju.cn

[U49] PHP：只读属性
来源：http://be.colortex.cn

public readonly string $name
来源：http://kj.9csxet.cn

[U50] PHP：构造器属性提升
来源：http://gg.szxytkj.cn

public function __construct(private int $id) {}
来源：http://uz.yuntaijiaju.cn


<!-- 参考信息 -->