代发 wailian999

static int counter = 0;
来源：http://zu.yuexingan06.cn

[S29] C：变参函数
来源：http://bh.asd995.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://fj.huixinmuqiang.cn

[S30] C：头文件保护
来源：http://ku.gzmigu.cn

#ifndef X_H
来源：http://as.hahajie.cn

#define X_H
来源：http://ht.wgjwhj.cn

#endif
来源：http://fw.huixinmuqiang.cn

[S31] C++：Hello World
来源：http://lx.hahajie.cn

#include <iostream>
来源：http://no.jianghongdianzi.cn

int main() { std::cout << "Hello\n"; }
来源：http://bd.yuexingan06.cn

[S32] C++：字符串
来源：http://cy.bookmarksfly.cn

std::string s = "hi";  s += "!";
来源：http://el.huixiangedu.cn

[S33] C++：vector 增删
来源：http://gi.shxzskj.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://up.9csxet.cn

[S34] C++：遍历 vector
来源：http://th.yuexingan06.cn

for (auto &x : v) { std::cout << x; }
来源：http://cq.hnjuh.cn

[S35] C++：map
来源：http://nq.jianghongdianzi.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://kz.bookmarksfly.cn

[S36] C++：unordered_map
来源：http://mw.shxzukj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://vn.asd995.cn

[S37] C++：set
来源：http://mp.huixiangedu.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://cv.shtwfgs.cn

[S38] C++：排序
来源：http://kp.huanxung.cn

std::sort(v.begin(), v.end());
来源：http://mj.asd995.cn

[S39] C++：自定义比较器排序
来源：http://cg.hahajie.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://hn.panjiajie.cn

[S40] C++：查找元素
来源：http://jf.haigaiapp.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://tj.hahajie.cn

[S41] C++：类与构造函数
来源：http://fh.jianghongdianzi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://op.shtwfgs.cn

[S42] C++：继承与虚函数
来源：http://jj.chemitech.net.cn

class B : public Base { public: void f() override {} };
来源：http://pf.muxihuayi.cn

[S43] C++：智能指针
来源：http://ff.huixinmuqiang.cn

auto p = std::make_unique<int>(5);
来源：http://yq.shtwfgs.cn

[S44] C++：引用传参
来源：http://jo.hahajie.cn

void inc(int &x) { ++x; }
来源：http://ma.nicolike.cn

[S45] C++：lambda
来源：http://nr.asd995.cn

auto add = [](int a, int b) { return a + b; };
来源：http://xb.szxytkj.cn

[S46] C++：函数模板
来源：http://bx.panjiajie.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://jn.521024.cn

[S47] C++：结构化绑定遍历
来源：http://ao.nszjky.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://lm.asd995.cn

[S48] C++：逐行读文件
来源：http://bm.bookmarksfly.cn

std::ifstream in("a.txt");  std::string line;
来源：http://jx.muxihuayi.cn

while (std::getline(in, line)) { }
来源：http://nx.szsharing.cn

[S49] C++：写文件
来源：http://kk.muxihuayi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://gs.panjiajie.cn

[S50] C++：格式化数字
来源：http://xc.shxzukj.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://pa.bookmarksfly.cn

[S51] C++：显式类型转换
来源：http://yb.haigaiapp.cn

static_cast<double>(a) / b
来源：http://fu.jctech888.com.cn

[S52] C++：const 与 noexcept
来源：http://vb.jctech888.com.cn

int size() const noexcept { return n_; }
来源：http://do.jctech888.com.cn

[S53] C++：移动语义
来源：http://bl.bookmarksfly.cn

std::vector<int> w = std::move(v);
来源：http://xs.szxytkj.cn

[S54] C++：异常处理
来源：http://cw.9csxet.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://bh.shtwfgs.cn

[S55] C++：结构化绑定
来源：http://zb.nszjky.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://zp.panjiajie.cn

[S56] C++：optional
来源：http://dq.yuexingan06.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wr.yuntaijiaju.cn

[S57] C++：编译期常量
来源：http://sd.shxzskj.cn

constexpr int N = 10;
来源：http://jt.huixiangedu.cn

[S58] C++：命名空间
来源：http://fr.newstarts.cn

namespace ns { int f() { return 1; } }
来源：http://ot.yuexingan06.cn

[S59] C++：静态断言
来源：http://vy.panjiajie.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://cc.newstarts.cn

[S60] C++：遍历并删除元素
来源：http://vv.muxihuayi.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://zx.521024.cn

================================================================================
来源：http://pp.panjiajie.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://az.shtwfgs.cn

================================================================================
来源：http://yh.haigaiapp.cn

[T01] Kotlin：Hello World
来源：http://ke.nszjky.cn

println("Hello")
来源：http://hi.521024.cn

[T02] Kotlin：变量
来源：http://ys.haigaiapp.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://uj.haigaiapp.cn

[T03] Kotlin：字符串模板
来源：http://fv.shxzukj.cn

"值: $b"
来源：http://re.nszjky.cn

[T04] Kotlin：空安全
来源：http://na.muxihuayi.cn

val n: String? = null;  n?.length
来源：http://dw.521024.cn

[T05] Kotlin：when 表达式
来源：http://fr.9csxet.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://tg.jianghongdianzi.cn

[T06] Kotlin：集合映射
来源：http://te.szxytkj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ts.jctech888.com.cn

[T07] Kotlin：集合过滤
来源：http://wx.hnjuh.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ge.bookmarksfly.cn

[T08] Kotlin：数据类
来源：http://av.shtwfgs.cn

data class User(val name: String, val age: Int)
来源：http://or.hahajie.cn

[T09] Kotlin：扩展函数
来源：http://nj.shtwfgs.cn

fun String.exclaim() = this + "!"
来源：http://zy.jctech888.com.cn

[T10] Kotlin：默认参数
来源：http://hr.shxzskj.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://iw.gzmigu.cn

[T11] Kotlin：协程
来源：http://wn.hnjuh.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ot.lnxyls.cn

[T12] Kotlin：解构声明
来源：http://ie.shxzskj.cn

val (a, b) = Pair(1, 2)
来源：http://aw.lnxyls.cn

[T13] Kotlin：只读 Map
来源：http://sf.asd995.cn

val m = mapOf("a" to 1)
来源：http://qq.bjjhwx.cn

[T14] Kotlin：循环
来源：http://rk.szsharing.cn

for (i in 1..10) println(i)
来源：http://nm.panjiajie.cn

[T15] Kotlin：接口
来源：http://hj.nicolike.cn

interface Shape { fun area(): Double }
来源：http://fy.huixiangedu.cn

[T16] Swift：Hello World
来源：http://qw.huixinmuqiang.cn

print("Hello")
来源：http://hf.panjiajie.cn

[T17] Swift：变量与常量
来源：http://tc.bjjhwx.cn

var a = 1;  let b = 2
来源：http://nb.colortex.cn

[T18] Swift：字符串插值
来源：http://ts.huixinmuqiang.cn

"值: \(b)"
来源：http://jo.shxzskj.cn

[T19] Swift：可选绑定
来源：http://vd.newstarts.cn

if let n = opt { print(n) }
来源：http://zf.huixiangedu.cn

[T20] Swift：数组操作
来源：http://wo.nszjky.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ni.gzmigu.cn

[T21] Swift：遍历
来源：http://zk.panjiajie.cn

for x in a { print(x) }
来源：http://gx.bjjhwx.cn

[T22] Swift：字典
来源：http://mk.shtwfgs.cn

var d = ["a": 1];  d["b"] = 2
来源：http://xv.colortex.cn

[T23] Swift：函数
来源：http://si.colortex.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://yd.nicolike.cn

[T24] Swift：闭包
来源：http://uz.colortex.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://qv.521024.cn

[T25] Swift：结构体
来源：http://rj.szxytkj.cn

struct P { var x: Int }
来源：http://tg.yuntaijiaju.cn

[T26] Swift：类与重写
来源：http://zr.bjjhwx.cn

class A: Base { override func f() {} }
来源：http://xk.hnjuh.cn

[T27] Swift：错误处理
来源：http://kf.hnjuh.cn

do { try f() } catch { print(error) }
来源：http://eb.colortex.cn

[T28] Swift：枚举
来源：http://es.chemitech.net.cn

enum Color { case red, green }
来源：http://rf.colortex.cn

[T29] Swift：guard 提前返回
来源：http://le.muxihuayi.cn

guard let x = opt else { return }
来源：http://wa.jianghongdianzi.cn

[T30] Swift：协议
来源：http://zz.jctech888.com.cn

protocol Shape { func area() -> Double }
来源：http://ne.wgjwhj.cn

[T31] Lua：Hello World
来源：http://mn.hnjuh.cn

print("Hello")
来源：http://xc.huixiangedu.cn

[T32] Lua：局部变量
来源：http://nc.szsharing.cn

local a = 1
来源：http://nj.panjiajie.cn

[T33] Lua：表（数组）
来源：http://ih.huixiangedu.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://uk.asd995.cn

[T34] Lua：遍历表
来源：http://dx.jctech888.com.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://je.nszjky.cn

[T35] Lua：字典表
来源：http://li.muxihuayi.cn

local d = { a = 1 };  d.b = 2
来源：http://cc.haigaiapp.cn

[T36] Lua：函数
来源：http://xr.muxihuayi.cn

function add(a, b) return a + b end
来源：http://vj.521024.cn

[T37] Lua：字符串拼接
来源：http://lg.hahajie.cn

"a" .. "b"
来源：http://on.muxihuayi.cn

[T38] Lua：条件
来源：http://dm.panjiajie.cn

if x > 0 then print("正") end
来源：http://om.yuexingan06.cn

[T39] Lua：模式匹配
来源：http://yy.hnjuh.cn

string.find(s, "%d+")
来源：http://vh.szxytkj.cn

[T40] Lua：元表
来源：http://pv.bookmarksfly.cn

setmetatable({}, { __index = base })
来源：http://ax.shtwfgs.cn

[T41] Perl：Hello World
来源：http://ng.jianghongdianzi.cn

print "Hello\n";
来源：http://ba.haigaiapp.cn

[T42] Perl：变量类型
来源：http://we.haigaiapp.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://gt.asd995.cn

[T43] Perl：字符串插值
来源：http://oh.shxzskj.cn

"值: $a"
来源：http://vl.hnjuh.cn

[T44] Perl：条件
来源：http://ds.muxihuayi.cn

if ($a > 0) { print "正"; }
来源：http://gi.huixiangedu.cn

[T45] Perl：数组遍历
来源：http://nz.asd995.cn

for my $x (@arr) { print $x; }
来源：http://rg.shtwfgs.cn

[T46] Perl：哈希操作
来源：http://sh.asd995.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://xf.jctech888.com.cn

[T47] Perl：正则捕获
来源：http://nd.bjjhwx.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://vz.chemitech.net.cn

[T48] Perl：正则替换
来源：http://xy.shxzskj.cn

$s =~ s/old/new/g;
来源：http://yo.muxihuayi.cn

[T49] Perl：函数
来源：http://aq.muxihuayi.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://fq.huixinmuqiang.cn

[T50] Perl：逐行读文件
来源：http://uh.szsharing.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://gf.panjiajie.cn

while (my $line = <$fh>) { print $line; }
来源：http://im.wgjwhj.cn

[T51] Scala：Hello World
来源：http://wi.yuexingan06.cn

println("Hello")
来源：http://so.jianghongdianzi.cn

[T52] Scala：变量
来源：http://yz.huanxung.cn

val a = 1;  var b = 2
来源：http://te.muxihuayi.cn

[T53] Scala：字符串插值
来源：http://or.muxihuayi.cn

s"值: $b"
来源：http://kx.yuntaijiaju.cn

[T54] Scala：集合映射
来源：http://yn.gzmigu.cn

List(1, 2, 3).map(_ * 2)
来源：http://uy.jianghongdianzi.cn

[T55] Scala：集合过滤
来源：http://rg.szsharing.cn

List(1, 2, 3).filter(_ > 1)
来源：http://um.wgjwhj.cn

[T56] Scala：样例类
来源：http://mh.huixinmuqiang.cn

case class User(name: String, age: Int)
来源：http://fq.chemitech.net.cn

[T57] Scala：模式匹配
来源：http://vh.huixinmuqiang.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://zq.9csxet.cn

[T58] Scala：函数定义
来源：http://sp.nszjky.cn

def add(a: Int, b: Int): Int = a + b
来源：http://gn.shxzukj.cn

[T59] Scala：循环
来源：http://ct.shxzskj.cn

for (i <- 1 to 10) println(i)
来源：http://xn.wgjwhj.cn

[T60] Scala：折叠
来源：http://fa.colortex.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://vu.lnxyls.cn

================================================================================
来源：http://sg.521024.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://mb.huixinmuqiang.cn

================================================================================
来源：http://jt.haigaiapp.cn

[U01] Py：创建虚拟环境
来源：http://bb.wgjwhj.cn

python -m venv .venv && source .venv/bin/activate
来源：http://pm.yuexingan06.cn

[U02] Py：导出 / 安装依赖
来源：http://tx.huanxung.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://zg.jianghongdianzi.cn

[U03] Py：加载 .env 配置
来源：http://qj.lnxyls.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://zu.jianghongdianzi.cn

[U04] Py：变量调试打印
来源：http://sv.wgjwhj.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://zi.szxytkj.cn

[U05] Py：列表去重且保序
来源：http://lr.huixiangedu.cn

list(dict.fromkeys(arr))
来源：http://mz.nszjky.cn

[U06] Py：合并两个字典
来源：http://lk.haigaiapp.cn

{**a, **b}
来源：http://ux.gzmigu.cn

[U07] Py：反转字典键值
来源：http://ql.szsharing.cn

{v: k for k, v in d.items()}
来源：http://kl.shxzskj.cn

[U08] Py：展平二维列表
来源：http://mg.huanxung.cn

[y for x in nested for y in x]
来源：http://ng.panjiajie.cn

[U09] Py：字典取最大值的键
来源：http://mb.shxzskj.cn

max(d, key=d.get)
来源：http://ti.shxzukj.cn

[U10] Py：按值排序字典
来源：http://rb.lnxyls.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://et.jctech888.com.cn

[U11] Py：生成器表达式
来源：http://hp.szxytkj.cn

(x * 2 for x in arr)
来源：http://uz.yuntaijiaju.cn

[U12] Py：取出现最多的 3 个元素
来源：http://oa.gzmigu.cn

Counter(arr).most_common(3)
来源：http://bk.muxihuayi.cn

[U13] Py：固定长度队列
来源：http://jz.shtwfgs.cn

deque(maxlen=10)
来源：http://du.wgjwhj.cn

[U14] Py：分组收集到列表
来源：http://ey.shxzskj.cn

defaultdict(list)
来源：http://cm.haigaiapp.cn

[U15] Py：高精度计时
来源：http://cp.asd995.cn

t = time.perf_counter()
来源：http://lq.bjjhwx.cn

[U16] Py：命令行参数解析
来源：http://xr.szxytkj.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://md.521024.cn

[U17] Py：初始化日志
来源：http://xa.huixinmuqiang.cn

logging.basicConfig(level=logging.INFO)
来源：http://gr.yuntaijiaju.cn

[U18] Py：预编译正则
来源：http://dz.huanxung.cn

pat = re.compile(r"\d+")
来源：http://yq.shxzukj.cn

[U19] Py：正则替换带回调
来源：http://lh.hahajie.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://xa.szsharing.cn

[U20] Py：缓存函数结果
来源：http://uf.bjjhwx.cn

@functools.lru_cache(maxsize=None)
来源：http://ks.chemitech.net.cn

[U21] Py：自定义上下文管理器
来源：http://kb.hnjuh.cn

@contextlib.contextmanager
来源：http://ag.asd995.cn

[U22] Py：矩阵转置
来源：http://po.nszjky.cn

list(zip(*m))
来源：http://kz.9csxet.cn

[U23] Py：分块读取大文件
来源：http://yy.panjiajie.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://nu.shxzukj.cn

[U24] Py：路径操作
来源：http://wo.shtwfgs.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://ek.colortex.cn

[U25] Py：CSV 按字典读
来源：http://yk.colortex.cn

csv.DictReader(f)
来源：http://nf.yuntaijiaju.cn

[U26] Py：并发下载
来源：http://kd.521024.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://bo.szxytkj.cn

[U27] Py：异步 HTTP
来源：http://pn.newstarts.cn

aiohttp.ClientSession() 配合 async with
来源：http://ro.szsharing.cn

[U28] Py：类型别名
来源：http://eg.521024.cn

UserId = int
来源：http://vz.muxihuayi.cn

[U29] Py：属性校验
来源：http://zg.asd995.cn

@property 与 @x.setter 配合
来源：http://zj.asd995.cn

[U30] Py：数据类
来源：http://nr.shtwfgs.cn

@dataclass(slots=True)
来源：http://rr.nszjky.cn

[U31] Py：单测
来源：http://sw.9csxet.cn

python -m pytest -q
来源：http://rp.lnxyls.cn

[U32] Py：代码格式化
来源：http://ua.shxzukj.cn

ruff format . && ruff check --fix .
来源：http://pa.asd995.cn

[U33] Py：打包发布
来源：http://sw.yuntaijiaju.cn

python -m build  （依赖 pyproject.toml）
来源：http://wu.szsharing.cn

[U34] Py：判断编码
来源：http://ig.huanxung.cn

chardet.detect(raw)
来源：http://ei.muxihuayi.cn

[U35] Py：发送邮件
来源：http://rj.colortex.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ef.jctech888.com.cn

[U36] Py：定时任务
来源：http://zu.nszjky.cn

schedule.every(10).minutes.do(job)
来源：http://ka.huixiangedu.cn

[U37] Py：读写 Excel
来源：http://jv.wgjwhj.cn

pandas.read_excel / DataFrame.to_excel
来源：http://pz.haigaiapp.cn

[U38] Py：获取脚本所在目录
来源：http://zk.panjiajie.cn

Path(__file__).resolve().parent
来源：http://hr.jianghongdianzi.cn

[U39] Py：判断是否在交互环境
来源：http://xb.hahajie.cn

sys.stdout.isatty()
来源：http://li.521024.cn

[U40] Py：打印到标准错误
来源：http://es.panjiajie.cn

print("err", file=sys.stderr)
来源：http://nm.yuexingan06.cn

[U41] PHP：初始化 Composer 项目
来源：http://ll.chemitech.net.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://ha.bjjhwx.cn

[U42] PHP：PSR-4 自动加载
来源：http://hd.newstarts.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://zc.chemitech.net.cn

[U43] PHP：声明命名空间
来源：http://dy.szxytkj.cn

namespace App\Http;
来源：http://ti.521024.cn

[U44] PHP：开启严格类型
来源：http://tr.521024.cn

declare(strict_types=1);
来源：http://fo.nszjky.cn

[U45] PHP：类型声明与返回类型
来源：http://pq.9csxet.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://pc.haigaiapp.cn

[U46] PHP：可空类型
来源：http://xk.huixiangedu.cn

?string $name = null
来源：http://wf.huixinmuqiang.cn

[U47] PHP：联合类型
来源：http://fl.muxihuayi.cn

int|string $id
来源：http://sp.bjjhwx.cn

[U48] PHP：纯枚举
来源：http://hb.muxihuayi.cn

enum Status: string { case Active = "active"; case Off = "off"; }
来源：http://wx.shtwfgs.cn

[U49] PHP：只读属性
来源：http://hq.hahajie.cn

public readonly string $name
来源：http://tm.huixinmuqiang.cn

[U50] PHP：构造器属性提升
来源：http://ct.jianghongdianzi.cn

public function __construct(private int $id) {}
来源：http://bj.szsharing.cn

[U51] PHP：数组解构
来源：http://vk.asd995.cn

[$a, $b] = $arr;
来源：http://pg.colortex.cn

[U52] PHP：箭头函数
来源：http://ev.huanxung.cn

$double = fn($x) => $x * 2;
来源：http://dh.panjiajie.cn


<!-- 参考信息 -->