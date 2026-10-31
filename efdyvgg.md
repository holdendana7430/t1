代发 wailian999

atoi("42");  strtod("3.14", NULL);
来源：http://rl.shxzukj.cn

[S23] C：随机数
来源：http://ym.shxzskj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ai.chemitech.net.cn

[S24] C：获取本地时间
来源：http://qy.haigaiapp.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ni.muxihuayi.cn

[S25] C：内存拷贝
来源：http://it.shxzskj.cn

memcpy(dst, src, n);
来源：http://jn.newstarts.cn

[S26] C：内存清零
来源：http://fc.shxzskj.cn

memset(a, 0, sizeof a);
来源：http://jt.panjiajie.cn

[S27] C：定义常量
来源：http://lj.yuexingan06.cn

const double PI = 3.14159;
来源：http://lm.jctech888.com.cn

[S28] C：静态变量
来源：http://rs.yuntaijiaju.cn

static int counter = 0;
来源：http://iy.shxzskj.cn

[S29] C：变参函数
来源：http://ze.wgjwhj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://kh.shxzukj.cn

[S30] C：头文件保护
来源：http://sk.shxzukj.cn

#ifndef X_H
来源：http://oq.wgjwhj.cn

#define X_H
来源：http://jb.lnxyls.cn

#endif
来源：http://py.bjjhwx.cn

[S31] C++：Hello World
来源：http://du.asd995.cn

#include <iostream>
来源：http://ez.bookmarksfly.cn

int main() { std::cout << "Hello\n"; }
来源：http://hq.huanxung.cn

[S32] C++：字符串
来源：http://yk.szxytkj.cn

std::string s = "hi";  s += "!";
来源：http://ow.huixinmuqiang.cn

[S33] C++：vector 增删
来源：http://gd.shxzukj.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://uu.yuntaijiaju.cn

[S34] C++：遍历 vector
来源：http://gs.yuexingan06.cn

for (auto &x : v) { std::cout << x; }
来源：http://dp.yuntaijiaju.cn

[S35] C++：map
来源：http://ee.nszjky.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://uy.wgjwhj.cn

[S36] C++：unordered_map
来源：http://mf.jctech888.com.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ya.newstarts.cn

[S37] C++：set
来源：http://sp.asd995.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://pw.yuexingan06.cn

[S38] C++：排序
来源：http://bw.wgjwhj.cn

std::sort(v.begin(), v.end());
来源：http://vm.shxzukj.cn

[S39] C++：自定义比较器排序
来源：http://cl.lnxyls.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://zf.szsharing.cn

[S40] C++：查找元素
来源：http://qo.yuntaijiaju.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ob.huixiangedu.cn

[S41] C++：类与构造函数
来源：http://ep.huixiangedu.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://xh.haigaiapp.cn

[S42] C++：继承与虚函数
来源：http://lw.9csxet.cn

class B : public Base { public: void f() override {} };
来源：http://ak.jianghongdianzi.cn

[S43] C++：智能指针
来源：http://zn.nszjky.cn

auto p = std::make_unique<int>(5);
来源：http://vi.bookmarksfly.cn

[S44] C++：引用传参
来源：http://gx.9csxet.cn

void inc(int &x) { ++x; }
来源：http://cn.asd995.cn

[S45] C++：lambda
来源：http://py.shxzskj.cn

auto add = [](int a, int b) { return a + b; };
来源：http://op.wgjwhj.cn

[S46] C++：函数模板
来源：http://wl.nicolike.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hh.shxzskj.cn

[S47] C++：结构化绑定遍历
来源：http://nq.nszjky.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://vf.huixinmuqiang.cn

[S48] C++：逐行读文件
来源：http://to.hahajie.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ng.lnxyls.cn

while (std::getline(in, line)) { }
来源：http://xx.asd995.cn

[S49] C++：写文件
来源：http://xn.bjjhwx.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://dh.lnxyls.cn

[S50] C++：格式化数字
来源：http://mo.muxihuayi.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ku.panjiajie.cn

[S51] C++：显式类型转换
来源：http://ok.haigaiapp.cn

static_cast<double>(a) / b
来源：http://as.huixiangedu.cn

[S52] C++：const 与 noexcept
来源：http://xv.newstarts.cn

int size() const noexcept { return n_; }
来源：http://me.gzmigu.cn

[S53] C++：移动语义
来源：http://va.jctech888.com.cn

std::vector<int> w = std::move(v);
来源：http://si.panjiajie.cn

[S54] C++：异常处理
来源：http://jt.chemitech.net.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://lh.521024.cn

[S55] C++：结构化绑定
来源：http://yn.hahajie.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://bz.szsharing.cn

[S56] C++：optional
来源：http://ob.shxzskj.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://lv.yuexingan06.cn

[S57] C++：编译期常量
来源：http://ux.panjiajie.cn

constexpr int N = 10;
来源：http://th.bookmarksfly.cn

[S58] C++：命名空间
来源：http://eb.colortex.cn

namespace ns { int f() { return 1; } }
来源：http://kz.newstarts.cn

[S59] C++：静态断言
来源：http://rf.colortex.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://nr.colortex.cn

[S60] C++：遍历并删除元素
来源：http://hm.nicolike.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://kb.szxytkj.cn

================================================================================
来源：http://ya.nicolike.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://za.muxihuayi.cn

================================================================================
来源：http://fo.wgjwhj.cn

[T01] Kotlin：Hello World
来源：http://ep.gzmigu.cn

println("Hello")
来源：http://hq.bjjhwx.cn

[T02] Kotlin：变量
来源：http://xh.nszjky.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://iw.panjiajie.cn

[T03] Kotlin：字符串模板
来源：http://qg.bookmarksfly.cn

"值: $b"
来源：http://eq.haigaiapp.cn

[T04] Kotlin：空安全
来源：http://bu.szsharing.cn

val n: String? = null;  n?.length
来源：http://eb.9csxet.cn

[T05] Kotlin：when 表达式
来源：http://pi.yuexingan06.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://yd.chemitech.net.cn

[T06] Kotlin：集合映射
来源：http://ub.yuntaijiaju.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://pm.nicolike.cn

[T07] Kotlin：集合过滤
来源：http://xk.newstarts.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ai.hnjuh.cn

[T08] Kotlin：数据类
来源：http://kt.nszjky.cn

data class User(val name: String, val age: Int)
来源：http://ld.huixinmuqiang.cn

[T09] Kotlin：扩展函数
来源：http://re.bookmarksfly.cn

fun String.exclaim() = this + "!"
来源：http://re.huanxung.cn

[T10] Kotlin：默认参数
来源：http://ms.huixiangedu.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://mf.chemitech.net.cn

[T11] Kotlin：协程
来源：http://ap.newstarts.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://lq.gzmigu.cn

[T12] Kotlin：解构声明
来源：http://zn.nicolike.cn

val (a, b) = Pair(1, 2)
来源：http://vs.gzmigu.cn

[T13] Kotlin：只读 Map
来源：http://tc.yuexingan06.cn

val m = mapOf("a" to 1)
来源：http://pf.nicolike.cn

[T14] Kotlin：循环
来源：http://wa.yuntaijiaju.cn

for (i in 1..10) println(i)
来源：http://dr.nicolike.cn

[T15] Kotlin：接口
来源：http://bo.shtwfgs.cn

interface Shape { fun area(): Double }
来源：http://xg.yuntaijiaju.cn

[T16] Swift：Hello World
来源：http://bk.colortex.cn

print("Hello")
来源：http://ie.lnxyls.cn

[T17] Swift：变量与常量
来源：http://ib.nszjky.cn

var a = 1;  let b = 2
来源：http://jk.huixiangedu.cn

[T18] Swift：字符串插值
来源：http://ux.haigaiapp.cn

"值: \(b)"
来源：http://oe.szxytkj.cn

[T19] Swift：可选绑定
来源：http://zw.jianghongdianzi.cn

if let n = opt { print(n) }
来源：http://ct.newstarts.cn

[T20] Swift：数组操作
来源：http://zp.colortex.cn

var a = [1, 2, 3];  a.append(4)
来源：http://wi.szxytkj.cn

[T21] Swift：遍历
来源：http://nf.wgjwhj.cn

for x in a { print(x) }
来源：http://sz.szsharing.cn

[T22] Swift：字典
来源：http://vg.asd995.cn

var d = ["a": 1];  d["b"] = 2
来源：http://cy.newstarts.cn

[T23] Swift：函数
来源：http://ie.hnjuh.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hc.yuexingan06.cn

[T24] Swift：闭包
来源：http://fq.shxzukj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://to.szxytkj.cn

[T25] Swift：结构体
来源：http://lh.jianghongdianzi.cn

struct P { var x: Int }
来源：http://kq.gzmigu.cn

[T26] Swift：类与重写
来源：http://jh.gzmigu.cn

class A: Base { override func f() {} }
来源：http://zr.hnjuh.cn

[T27] Swift：错误处理
来源：http://sa.panjiajie.cn

do { try f() } catch { print(error) }
来源：http://yy.muxihuayi.cn

[T28] Swift：枚举
来源：http://ym.muxihuayi.cn

enum Color { case red, green }
来源：http://yq.chemitech.net.cn

[T29] Swift：guard 提前返回
来源：http://oc.yuntaijiaju.cn

guard let x = opt else { return }
来源：http://no.bookmarksfly.cn

[T30] Swift：协议
来源：http://hs.szxytkj.cn

protocol Shape { func area() -> Double }
来源：http://sr.shxzskj.cn

[T31] Lua：Hello World
来源：http://dv.panjiajie.cn

print("Hello")
来源：http://dz.newstarts.cn

[T32] Lua：局部变量
来源：http://nb.yuntaijiaju.cn

local a = 1
来源：http://kv.bookmarksfly.cn

[T33] Lua：表（数组）
来源：http://xd.asd995.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://vk.nszjky.cn

[T34] Lua：遍历表
来源：http://cb.szsharing.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://pn.9csxet.cn

[T35] Lua：字典表
来源：http://xl.haigaiapp.cn

local d = { a = 1 };  d.b = 2
来源：http://kl.shxzukj.cn

[T36] Lua：函数
来源：http://ci.lnxyls.cn

function add(a, b) return a + b end
来源：http://ka.asd995.cn

[T37] Lua：字符串拼接
来源：http://ic.hahajie.cn

"a" .. "b"
来源：http://tg.huixinmuqiang.cn

[T38] Lua：条件
来源：http://wr.jianghongdianzi.cn

if x > 0 then print("正") end
来源：http://uk.huixiangedu.cn

[T39] Lua：模式匹配
来源：http://mr.panjiajie.cn

string.find(s, "%d+")
来源：http://qj.newstarts.cn

[T40] Lua：元表
来源：http://rd.colortex.cn

setmetatable({}, { __index = base })
来源：http://df.chemitech.net.cn

[T41] Perl：Hello World
来源：http://yh.nszjky.cn

print "Hello\n";
来源：http://kw.9csxet.cn

[T42] Perl：变量类型
来源：http://kh.chemitech.net.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://on.yuntaijiaju.cn

[T43] Perl：字符串插值
来源：http://wg.szsharing.cn

"值: $a"
来源：http://vg.jctech888.com.cn

[T44] Perl：条件
来源：http://ob.hahajie.cn

if ($a > 0) { print "正"; }
来源：http://wd.9csxet.cn

[T45] Perl：数组遍历
来源：http://kr.521024.cn

for my $x (@arr) { print $x; }
来源：http://nf.bookmarksfly.cn

[T46] Perl：哈希操作
来源：http://pt.newstarts.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://kt.bookmarksfly.cn

[T47] Perl：正则捕获
来源：http://fi.shtwfgs.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://lh.wgjwhj.cn

[T48] Perl：正则替换
来源：http://jm.shxzukj.cn

$s =~ s/old/new/g;
来源：http://ak.bjjhwx.cn

[T49] Perl：函数
来源：http://dj.yuntaijiaju.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ia.chemitech.net.cn

[T50] Perl：逐行读文件
来源：http://hv.szsharing.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://pp.muxihuayi.cn

while (my $line = <$fh>) { print $line; }
来源：http://gx.nicolike.cn

[T51] Scala：Hello World
来源：http://wg.yuexingan06.cn

println("Hello")
来源：http://vv.shtwfgs.cn

[T52] Scala：变量
来源：http://mb.yuexingan06.cn

val a = 1;  var b = 2
来源：http://ck.hahajie.cn

[T53] Scala：字符串插值
来源：http://rw.panjiajie.cn

s"值: $b"
来源：http://cu.hahajie.cn

[T54] Scala：集合映射
来源：http://zh.yuntaijiaju.cn

List(1, 2, 3).map(_ * 2)
来源：http://ux.shxzukj.cn

[T55] Scala：集合过滤
来源：http://dn.szsharing.cn

List(1, 2, 3).filter(_ > 1)
来源：http://pw.hnjuh.cn

[T56] Scala：样例类
来源：http://fd.gzmigu.cn

case class User(name: String, age: Int)
来源：http://gj.haigaiapp.cn

[T57] Scala：模式匹配
来源：http://gq.bookmarksfly.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://iy.shtwfgs.cn

[T58] Scala：函数定义
来源：http://on.panjiajie.cn

def add(a: Int, b: Int): Int = a + b
来源：http://jp.huanxung.cn

[T59] Scala：循环
来源：http://pu.shxzukj.cn

for (i <- 1 to 10) println(i)
来源：http://ku.huixinmuqiang.cn

[T60] Scala：折叠
来源：http://gp.muxihuayi.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://gc.panjiajie.cn

================================================================================
来源：http://pu.huixinmuqiang.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ht.panjiajie.cn

================================================================================
来源：http://bn.chemitech.net.cn

[U01] Py：创建虚拟环境
来源：http://eh.newstarts.cn

python -m venv .venv && source .venv/bin/activate
来源：http://sn.yuntaijiaju.cn

[U02] Py：导出 / 安装依赖
来源：http://mn.huanxung.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://vh.jctech888.com.cn

[U03] Py：加载 .env 配置
来源：http://on.newstarts.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://uq.521024.cn

[U04] Py：变量调试打印
来源：http://js.huixiangedu.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ay.szsharing.cn

[U05] Py：列表去重且保序
来源：http://gp.newstarts.cn

list(dict.fromkeys(arr))
来源：http://ij.9csxet.cn

[U06] Py：合并两个字典
来源：http://bv.hnjuh.cn

{**a, **b}
来源：http://jw.panjiajie.cn

[U07] Py：反转字典键值
来源：http://sy.hahajie.cn

{v: k for k, v in d.items()}
来源：http://wa.asd995.cn

[U08] Py：展平二维列表
来源：http://vi.szxytkj.cn

[y for x in nested for y in x]
来源：http://yv.newstarts.cn

[U09] Py：字典取最大值的键
来源：http://uy.asd995.cn

max(d, key=d.get)
来源：http://fm.chemitech.net.cn

[U10] Py：按值排序字典
来源：http://qn.shtwfgs.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://kx.szxytkj.cn

[U11] Py：生成器表达式
来源：http://ck.huixinmuqiang.cn

(x * 2 for x in arr)
来源：http://qv.shxzukj.cn

[U12] Py：取出现最多的 3 个元素
来源：http://uc.bjjhwx.cn

Counter(arr).most_common(3)
来源：http://fo.szxytkj.cn

[U13] Py：固定长度队列
来源：http://wx.newstarts.cn

deque(maxlen=10)
来源：http://vp.asd995.cn

[U14] Py：分组收集到列表
来源：http://sk.nicolike.cn

defaultdict(list)
来源：http://hr.bookmarksfly.cn

[U15] Py：高精度计时
来源：http://jq.hnjuh.cn

t = time.perf_counter()
来源：http://qh.nicolike.cn

[U16] Py：命令行参数解析
来源：http://ih.asd995.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://vg.shxzukj.cn

[U17] Py：初始化日志
来源：http://nl.shtwfgs.cn

logging.basicConfig(level=logging.INFO)
来源：http://sh.hnjuh.cn

[U18] Py：预编译正则
来源：http://my.hnjuh.cn

pat = re.compile(r"\d+")
来源：http://wu.nicolike.cn

[U19] Py：正则替换带回调
来源：http://vg.yuntaijiaju.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://yo.wgjwhj.cn

[U20] Py：缓存函数结果
来源：http://fa.nszjky.cn

@functools.lru_cache(maxsize=None)
来源：http://uf.muxihuayi.cn

[U21] Py：自定义上下文管理器
来源：http://gs.huanxung.cn

@contextlib.contextmanager
来源：http://zz.huixinmuqiang.cn

[U22] Py：矩阵转置
来源：http://yy.yuexingan06.cn

list(zip(*m))
来源：http://eq.yuntaijiaju.cn

[U23] Py：分块读取大文件
来源：http://qw.lnxyls.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://bi.haigaiapp.cn

[U24] Py：路径操作
来源：http://uj.yuntaijiaju.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://fm.yuexingan06.cn

[U25] Py：CSV 按字典读
来源：http://dq.nszjky.cn

csv.DictReader(f)
来源：http://rf.hahajie.cn

[U26] Py：并发下载
来源：http://bt.nszjky.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://ts.chemitech.net.cn

[U27] Py：异步 HTTP
来源：http://rh.haigaiapp.cn

aiohttp.ClientSession() 配合 async with
来源：http://rd.hnjuh.cn

[U28] Py：类型别名
来源：http://ah.nicolike.cn

UserId = int
来源：http://vz.nszjky.cn

[U29] Py：属性校验
来源：http://va.nicolike.cn

@property 与 @x.setter 配合
来源：http://jm.yuntaijiaju.cn

[U30] Py：数据类
来源：http://og.hahajie.cn

@dataclass(slots=True)
来源：http://nu.bjjhwx.cn

[U31] Py：单测
来源：http://vb.chemitech.net.cn

python -m pytest -q
来源：http://zv.hnjuh.cn

[U32] Py：代码格式化
来源：http://en.gzmigu.cn

ruff format . && ruff check --fix .
来源：http://ud.colortex.cn

[U33] Py：打包发布
来源：http://ht.lnxyls.cn

python -m build  （依赖 pyproject.toml）
来源：http://mn.panjiajie.cn

[U34] Py：判断编码
来源：http://zy.yuexingan06.cn

chardet.detect(raw)
来源：http://ed.yuexingan06.cn

[U35] Py：发送邮件
来源：http://pt.nszjky.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://sv.bookmarksfly.cn

[U36] Py：定时任务
来源：http://ld.huixinmuqiang.cn

schedule.every(10).minutes.do(job)
来源：http://jy.shtwfgs.cn

[U37] Py：读写 Excel
来源：http://wl.huixinmuqiang.cn

pandas.read_excel / DataFrame.to_excel
来源：http://eh.shxzskj.cn

[U38] Py：获取脚本所在目录
来源：http://ue.huanxung.cn

Path(__file__).resolve().parent
来源：http://bn.shxzukj.cn

[U39] Py：判断是否在交互环境
来源：http://dp.yuntaijiaju.cn

sys.stdout.isatty()
来源：http://ty.huanxung.cn

[U40] Py：打印到标准错误
来源：http://ej.shxzukj.cn

print("err", file=sys.stderr)
来源：http://wl.chemitech.net.cn

[U41] PHP：初始化 Composer 项目
来源：http://uj.shxzukj.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://dt.shxzukj.cn

[U42] PHP：PSR-4 自动加载
来源：http://bs.wgjwhj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://ri.hahajie.cn

[U43] PHP：声明命名空间
来源：http://lq.shxzskj.cn

namespace App\Http;
来源：http://mb.521024.cn

[U44] PHP：开启严格类型
来源：http://fe.colortex.cn

declare(strict_types=1);
来源：http://xu.bjjhwx.cn

[U45] PHP：类型声明与返回类型
来源：http://hi.newstarts.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://wn.shxzukj.cn

[U46] PHP：可空类型
来源：http://he.wgjwhj.cn

?string $name = null
来源：http://jd.bjjhwx.cn


<!-- 参考信息 -->