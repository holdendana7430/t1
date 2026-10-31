代发 wailian999

#ifndef X_H
来源：http://jb.huanxung.cn

#define X_H
来源：http://ub.wgjwhj.cn

#endif
来源：http://bl.521024.cn

[S31] C++：Hello World
来源：http://cg.jianghongdianzi.cn

#include <iostream>
来源：http://im.huixinmuqiang.cn

int main() { std::cout << "Hello\n"; }
来源：http://qv.bookmarksfly.cn

[S32] C++：字符串
来源：http://yf.wgjwhj.cn

std::string s = "hi";  s += "!";
来源：http://uy.panjiajie.cn

[S33] C++：vector 增删
来源：http://tn.asd995.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ob.gzmigu.cn

[S34] C++：遍历 vector
来源：http://wt.szsharing.cn

for (auto &x : v) { std::cout << x; }
来源：http://hz.huixiangedu.cn

[S35] C++：map
来源：http://lj.asd995.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://pz.chemitech.net.cn

[S36] C++：unordered_map
来源：http://li.wgjwhj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ag.521024.cn

[S37] C++：set
来源：http://uy.huanxung.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://zk.huanxung.cn

[S38] C++：排序
来源：http://ie.hnjuh.cn

std::sort(v.begin(), v.end());
来源：http://ef.huixiangedu.cn

[S39] C++：自定义比较器排序
来源：http://ip.shtwfgs.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://yg.yuntaijiaju.cn

[S40] C++：查找元素
来源：http://ny.huixiangedu.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ni.9csxet.cn

[S41] C++：类与构造函数
来源：http://hn.521024.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://re.szxytkj.cn

[S42] C++：继承与虚函数
来源：http://tv.huixinmuqiang.cn

class B : public Base { public: void f() override {} };
来源：http://ls.bjjhwx.cn

[S43] C++：智能指针
来源：http://xr.haigaiapp.cn

auto p = std::make_unique<int>(5);
来源：http://op.shtwfgs.cn

[S44] C++：引用传参
来源：http://bo.bjjhwx.cn

void inc(int &x) { ++x; }
来源：http://ka.jctech888.com.cn

[S45] C++：lambda
来源：http://of.lnxyls.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ng.huixinmuqiang.cn

[S46] C++：函数模板
来源：http://bn.szxytkj.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://wy.hahajie.cn

[S47] C++：结构化绑定遍历
来源：http://ru.jianghongdianzi.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://xv.huixinmuqiang.cn

[S48] C++：逐行读文件
来源：http://js.nszjky.cn

std::ifstream in("a.txt");  std::string line;
来源：http://vq.gzmigu.cn

while (std::getline(in, line)) { }
来源：http://ni.shxzskj.cn

[S49] C++：写文件
来源：http://zl.bookmarksfly.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://be.yuexingan06.cn

[S50] C++：格式化数字
来源：http://zm.jctech888.com.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://di.jctech888.com.cn

[S51] C++：显式类型转换
来源：http://qf.shxzukj.cn

static_cast<double>(a) / b
来源：http://pb.jctech888.com.cn

[S52] C++：const 与 noexcept
来源：http://sh.jctech888.com.cn

int size() const noexcept { return n_; }
来源：http://cd.panjiajie.cn

[S53] C++：移动语义
来源：http://yd.yuntaijiaju.cn

std::vector<int> w = std::move(v);
来源：http://ix.szxytkj.cn

[S54] C++：异常处理
来源：http://mi.newstarts.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://dz.shxzskj.cn

[S55] C++：结构化绑定
来源：http://aa.lnxyls.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://pa.hahajie.cn

[S56] C++：optional
来源：http://js.wgjwhj.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ge.lnxyls.cn

[S57] C++：编译期常量
来源：http://il.panjiajie.cn

constexpr int N = 10;
来源：http://gk.jianghongdianzi.cn

[S58] C++：命名空间
来源：http://bd.521024.cn

namespace ns { int f() { return 1; } }
来源：http://lw.nicolike.cn

[S59] C++：静态断言
来源：http://lb.szxytkj.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hf.hnjuh.cn

[S60] C++：遍历并删除元素
来源：http://sk.nicolike.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hk.wgjwhj.cn

================================================================================
来源：http://my.szsharing.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://yv.nicolike.cn

================================================================================
来源：http://te.colortex.cn

[T01] Kotlin：Hello World
来源：http://jb.jctech888.com.cn

println("Hello")
来源：http://ux.521024.cn

[T02] Kotlin：变量
来源：http://zf.chemitech.net.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://bb.huanxung.cn

[T03] Kotlin：字符串模板
来源：http://eh.gzmigu.cn

"值: $b"
来源：http://kr.huanxung.cn

[T04] Kotlin：空安全
来源：http://wk.wgjwhj.cn

val n: String? = null;  n?.length
来源：http://nv.newstarts.cn

[T05] Kotlin：when 表达式
来源：http://cy.huanxung.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://or.nicolike.cn

[T06] Kotlin：集合映射
来源：http://oa.haigaiapp.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://pe.nszjky.cn

[T07] Kotlin：集合过滤
来源：http://ho.bjjhwx.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ur.szxytkj.cn

[T08] Kotlin：数据类
来源：http://yc.lnxyls.cn

data class User(val name: String, val age: Int)
来源：http://xr.521024.cn

[T09] Kotlin：扩展函数
来源：http://tj.shxzskj.cn

fun String.exclaim() = this + "!"
来源：http://ym.lnxyls.cn

[T10] Kotlin：默认参数
来源：http://fw.asd995.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://cj.nicolike.cn

[T11] Kotlin：协程
来源：http://yb.jianghongdianzi.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://yr.newstarts.cn

[T12] Kotlin：解构声明
来源：http://qm.shtwfgs.cn

val (a, b) = Pair(1, 2)
来源：http://aw.jianghongdianzi.cn

[T13] Kotlin：只读 Map
来源：http://qp.gzmigu.cn

val m = mapOf("a" to 1)
来源：http://we.szsharing.cn

[T14] Kotlin：循环
来源：http://eg.hnjuh.cn

for (i in 1..10) println(i)
来源：http://rn.szxytkj.cn

[T15] Kotlin：接口
来源：http://qz.bookmarksfly.cn

interface Shape { fun area(): Double }
来源：http://va.nicolike.cn

[T16] Swift：Hello World
来源：http://kr.asd995.cn

print("Hello")
来源：http://qm.yuntaijiaju.cn

[T17] Swift：变量与常量
来源：http://px.lnxyls.cn

var a = 1;  let b = 2
来源：http://mr.nszjky.cn

[T18] Swift：字符串插值
来源：http://wa.szsharing.cn

"值: \(b)"
来源：http://gh.nicolike.cn

[T19] Swift：可选绑定
来源：http://do.hnjuh.cn

if let n = opt { print(n) }
来源：http://oe.chemitech.net.cn

[T20] Swift：数组操作
来源：http://us.bjjhwx.cn

var a = [1, 2, 3];  a.append(4)
来源：http://fb.shxzukj.cn

[T21] Swift：遍历
来源：http://ry.wgjwhj.cn

for x in a { print(x) }
来源：http://jk.huixinmuqiang.cn

[T22] Swift：字典
来源：http://at.bjjhwx.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ea.lnxyls.cn

[T23] Swift：函数
来源：http://zg.colortex.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://al.bookmarksfly.cn

[T24] Swift：闭包
来源：http://az.shxzukj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://vw.colortex.cn

[T25] Swift：结构体
来源：http://ho.yuexingan06.cn

struct P { var x: Int }
来源：http://qi.asd995.cn

[T26] Swift：类与重写
来源：http://rr.shxzukj.cn

class A: Base { override func f() {} }
来源：http://os.gzmigu.cn

[T27] Swift：错误处理
来源：http://wf.9csxet.cn

do { try f() } catch { print(error) }
来源：http://ms.lnxyls.cn

[T28] Swift：枚举
来源：http://rr.yuexingan06.cn

enum Color { case red, green }
来源：http://jz.shtwfgs.cn

[T29] Swift：guard 提前返回
来源：http://ef.szxytkj.cn

guard let x = opt else { return }
来源：http://gs.colortex.cn

[T30] Swift：协议
来源：http://fp.bjjhwx.cn

protocol Shape { func area() -> Double }
来源：http://wu.shxzukj.cn

[T31] Lua：Hello World
来源：http://rh.bookmarksfly.cn

print("Hello")
来源：http://ll.hnjuh.cn

[T32] Lua：局部变量
来源：http://mm.chemitech.net.cn

local a = 1
来源：http://bk.yuntaijiaju.cn

[T33] Lua：表（数组）
来源：http://ii.huanxung.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://cq.chemitech.net.cn

[T34] Lua：遍历表
来源：http://af.newstarts.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ud.521024.cn

[T35] Lua：字典表
来源：http://or.huixiangedu.cn

local d = { a = 1 };  d.b = 2
来源：http://bb.huixiangedu.cn

[T36] Lua：函数
来源：http://to.nicolike.cn

function add(a, b) return a + b end
来源：http://cp.muxihuayi.cn

[T37] Lua：字符串拼接
来源：http://vi.nicolike.cn

"a" .. "b"
来源：http://ff.szsharing.cn

[T38] Lua：条件
来源：http://xj.nszjky.cn

if x > 0 then print("正") end
来源：http://vu.huixiangedu.cn

[T39] Lua：模式匹配
来源：http://ax.shxzskj.cn

string.find(s, "%d+")
来源：http://qh.521024.cn

[T40] Lua：元表
来源：http://io.bjjhwx.cn

setmetatable({}, { __index = base })
来源：http://cv.yuexingan06.cn

[T41] Perl：Hello World
来源：http://xd.9csxet.cn

print "Hello\n";
来源：http://er.wgjwhj.cn

[T42] Perl：变量类型
来源：http://xp.hahajie.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://fz.shtwfgs.cn

[T43] Perl：字符串插值
来源：http://tp.hnjuh.cn

"值: $a"
来源：http://hl.hahajie.cn

[T44] Perl：条件
来源：http://oi.nicolike.cn

if ($a > 0) { print "正"; }
来源：http://bk.colortex.cn

[T45] Perl：数组遍历
来源：http://ha.hahajie.cn

for my $x (@arr) { print $x; }
来源：http://en.muxihuayi.cn

[T46] Perl：哈希操作
来源：http://sv.521024.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://aj.szxytkj.cn

[T47] Perl：正则捕获
来源：http://sz.shxzukj.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ya.huanxung.cn

[T48] Perl：正则替换
来源：http://ow.haigaiapp.cn

$s =~ s/old/new/g;
来源：http://qu.9csxet.cn

[T49] Perl：函数
来源：http://of.huanxung.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://jt.huanxung.cn

[T50] Perl：逐行读文件
来源：http://tc.bjjhwx.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://lg.shxzukj.cn

while (my $line = <$fh>) { print $line; }
来源：http://ug.wgjwhj.cn

[T51] Scala：Hello World
来源：http://jt.shxzskj.cn

println("Hello")
来源：http://rj.521024.cn

[T52] Scala：变量
来源：http://hf.jianghongdianzi.cn

val a = 1;  var b = 2
来源：http://ri.asd995.cn

[T53] Scala：字符串插值
来源：http://wl.521024.cn

s"值: $b"
来源：http://sb.jianghongdianzi.cn

[T54] Scala：集合映射
来源：http://na.hnjuh.cn

List(1, 2, 3).map(_ * 2)
来源：http://zz.yuexingan06.cn

[T55] Scala：集合过滤
来源：http://ld.szxytkj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://dw.huixinmuqiang.cn

[T56] Scala：样例类
来源：http://jo.haigaiapp.cn

case class User(name: String, age: Int)
来源：http://qe.jianghongdianzi.cn

[T57] Scala：模式匹配
来源：http://bm.huanxung.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://tt.bookmarksfly.cn

[T58] Scala：函数定义
来源：http://yu.lnxyls.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ft.colortex.cn

[T59] Scala：循环
来源：http://bl.colortex.cn

for (i <- 1 to 10) println(i)
来源：http://og.521024.cn

[T60] Scala：折叠
来源：http://dn.bjjhwx.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://lz.muxihuayi.cn

================================================================================
来源：http://ik.panjiajie.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://fq.asd995.cn

================================================================================
来源：http://cn.lnxyls.cn

[U01] Py：创建虚拟环境
来源：http://tr.jctech888.com.cn

python -m venv .venv && source .venv/bin/activate
来源：http://cw.colortex.cn

[U02] Py：导出 / 安装依赖
来源：http://yo.yuntaijiaju.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://js.haigaiapp.cn

[U03] Py：加载 .env 配置
来源：http://zb.szsharing.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://rx.colortex.cn

[U04] Py：变量调试打印
来源：http://dq.jctech888.com.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://vj.shxzskj.cn

[U05] Py：列表去重且保序
来源：http://bl.shtwfgs.cn

list(dict.fromkeys(arr))
来源：http://dy.9csxet.cn

[U06] Py：合并两个字典
来源：http://gt.huixiangedu.cn

{**a, **b}
来源：http://rk.shxzskj.cn

[U07] Py：反转字典键值
来源：http://dm.jianghongdianzi.cn

{v: k for k, v in d.items()}
来源：http://wr.nicolike.cn

[U08] Py：展平二维列表
来源：http://qs.shxzukj.cn

[y for x in nested for y in x]
来源：http://th.haigaiapp.cn

[U09] Py：字典取最大值的键
来源：http://az.szsharing.cn

max(d, key=d.get)
来源：http://is.shxzskj.cn

[U10] Py：按值排序字典
来源：http://rk.wgjwhj.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://ua.9csxet.cn

[U11] Py：生成器表达式
来源：http://mb.panjiajie.cn

(x * 2 for x in arr)
来源：http://pk.asd995.cn

[U12] Py：取出现最多的 3 个元素
来源：http://lc.nicolike.cn

Counter(arr).most_common(3)
来源：http://kv.newstarts.cn

[U13] Py：固定长度队列
来源：http://hg.szxytkj.cn

deque(maxlen=10)
来源：http://rf.jianghongdianzi.cn

[U14] Py：分组收集到列表
来源：http://wg.shtwfgs.cn

defaultdict(list)
来源：http://om.shtwfgs.cn

[U15] Py：高精度计时
来源：http://nm.szsharing.cn

t = time.perf_counter()
来源：http://ig.panjiajie.cn

[U16] Py：命令行参数解析
来源：http://hq.yuexingan06.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://qw.shxzskj.cn

[U17] Py：初始化日志
来源：http://af.szxytkj.cn

logging.basicConfig(level=logging.INFO)
来源：http://nk.521024.cn

[U18] Py：预编译正则
来源：http://ze.hnjuh.cn

pat = re.compile(r"\d+")
来源：http://nl.yuntaijiaju.cn

[U19] Py：正则替换带回调
来源：http://ot.shtwfgs.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://it.nicolike.cn

[U20] Py：缓存函数结果
来源：http://iv.colortex.cn

@functools.lru_cache(maxsize=None)
来源：http://ki.jctech888.com.cn

[U21] Py：自定义上下文管理器
来源：http://lr.521024.cn

@contextlib.contextmanager
来源：http://wj.nicolike.cn

[U22] Py：矩阵转置
来源：http://cf.jianghongdianzi.cn

list(zip(*m))
来源：http://by.9csxet.cn

[U23] Py：分块读取大文件
来源：http://pv.shxzskj.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://zz.shxzukj.cn

[U24] Py：路径操作
来源：http://ib.shxzskj.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://sw.lnxyls.cn

[U25] Py：CSV 按字典读
来源：http://um.asd995.cn

csv.DictReader(f)
来源：http://sx.szsharing.cn

[U26] Py：并发下载
来源：http://al.hnjuh.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://kc.newstarts.cn

[U27] Py：异步 HTTP
来源：http://rn.huanxung.cn

aiohttp.ClientSession() 配合 async with
来源：http://th.huixiangedu.cn

[U28] Py：类型别名
来源：http://rv.wgjwhj.cn

UserId = int
来源：http://oz.jianghongdianzi.cn

[U29] Py：属性校验
来源：http://pm.gzmigu.cn

@property 与 @x.setter 配合
来源：http://iy.yuexingan06.cn

[U30] Py：数据类
来源：http://hb.muxihuayi.cn

@dataclass(slots=True)
来源：http://nk.yuexingan06.cn

[U31] Py：单测
来源：http://vd.jctech888.com.cn

python -m pytest -q
来源：http://hk.szxytkj.cn

[U32] Py：代码格式化
来源：http://kh.9csxet.cn

ruff format . && ruff check --fix .
来源：http://nf.shtwfgs.cn

[U33] Py：打包发布
来源：http://vv.huixiangedu.cn

python -m build  （依赖 pyproject.toml）
来源：http://lw.521024.cn

[U34] Py：判断编码
来源：http://wz.bjjhwx.cn

chardet.detect(raw)
来源：http://wn.asd995.cn

[U35] Py：发送邮件
来源：http://dz.asd995.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://gc.newstarts.cn

[U36] Py：定时任务
来源：http://sm.asd995.cn

schedule.every(10).minutes.do(job)
来源：http://ay.newstarts.cn

[U37] Py：读写 Excel
来源：http://mz.bookmarksfly.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ag.szxytkj.cn

[U38] Py：获取脚本所在目录
来源：http://uq.gzmigu.cn

Path(__file__).resolve().parent
来源：http://sa.521024.cn

[U39] Py：判断是否在交互环境
来源：http://cy.hahajie.cn

sys.stdout.isatty()
来源：http://hk.jctech888.com.cn

[U40] Py：打印到标准错误
来源：http://su.asd995.cn

print("err", file=sys.stderr)
来源：http://bu.hahajie.cn

[U41] PHP：初始化 Composer 项目
来源：http://cd.shtwfgs.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ur.panjiajie.cn

[U42] PHP：PSR-4 自动加载
来源：http://bz.nszjky.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://cs.shxzskj.cn

[U43] PHP：声明命名空间
来源：http://yi.huixinmuqiang.cn

namespace App\Http;
来源：http://va.hnjuh.cn

[U44] PHP：开启严格类型
来源：http://iy.yuntaijiaju.cn

declare(strict_types=1);
来源：http://dd.yuntaijiaju.cn

[U45] PHP：类型声明与返回类型
来源：http://jf.yuntaijiaju.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://po.muxihuayi.cn

[U46] PHP：可空类型
来源：http://mu.huixinmuqiang.cn

?string $name = null
来源：http://xo.nszjky.cn

[U47] PHP：联合类型
来源：http://mj.shtwfgs.cn

int|string $id
来源：http://hj.shtwfgs.cn

[U48] PHP：纯枚举
来源：http://ld.bjjhwx.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://ys.jianghongdianzi.cn

[U49] PHP：只读属性
来源：http://ly.jctech888.com.cn

public readonly string $name
来源：http://pz.gzmigu.cn

[U50] PHP：构造器属性提升
来源：http://lg.szxytkj.cn

public function __construct(private int $id) {}
来源：http://dc.lnxyls.cn

[U51] PHP：数组解构
来源：http://dn.panjiajie.cn

[$a, $b] = $arr;
来源：http://wz.shxzukj.cn

[U52] PHP：箭头函数
来源：http://hp.nszjky.cn

$double = fn($x) => $x * 2;
来源：http://ap.hahajie.cn

[U53] PHP：空合并运算符
来源：http://gr.bjjhwx.cn

$v = $a ?? $b ?? "default";
来源：http://xb.hahajie.cn

[U54] PHP：空安全调用
来源：http://zv.521024.cn

$obj?->method()
来源：http://dc.huixinmuqiang.cn


<!-- 参考信息 -->