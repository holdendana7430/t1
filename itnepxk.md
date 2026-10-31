代发 wailian999

atoi("42");  strtod("3.14", NULL);
来源：http://cl.bjjhwx.cn

[S23] C：随机数
来源：http://tm.haigaiapp.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://bo.chemitech.net.cn

[S24] C：获取本地时间
来源：http://ow.hahajie.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://sz.lnxyls.cn

[S25] C：内存拷贝
来源：http://uk.colortex.cn

memcpy(dst, src, n);
来源：http://nv.nicolike.cn

[S26] C：内存清零
来源：http://ht.lnxyls.cn

memset(a, 0, sizeof a);
来源：http://ug.wgjwhj.cn

[S27] C：定义常量
来源：http://hr.gzmigu.cn

const double PI = 3.14159;
来源：http://hp.lnxyls.cn

[S28] C：静态变量
来源：http://sh.shxzskj.cn

static int counter = 0;
来源：http://dp.bjjhwx.cn

[S29] C：变参函数
来源：http://oe.shxzukj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ol.jianghongdianzi.cn

[S30] C：头文件保护
来源：http://mu.huixiangedu.cn

#ifndef X_H
来源：http://wl.szxytkj.cn

#define X_H
来源：http://rj.bjjhwx.cn

#endif
来源：http://rb.nicolike.cn

[S31] C++：Hello World
来源：http://ps.yuexingan06.cn

#include <iostream>
来源：http://eh.panjiajie.cn

int main() { std::cout << "Hello\n"; }
来源：http://tp.huixinmuqiang.cn

[S32] C++：字符串
来源：http://vl.jianghongdianzi.cn

std::string s = "hi";  s += "!";
来源：http://tx.bookmarksfly.cn

[S33] C++：vector 增删
来源：http://hf.chemitech.net.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://rd.haigaiapp.cn

[S34] C++：遍历 vector
来源：http://fx.hnjuh.cn

for (auto &x : v) { std::cout << x; }
来源：http://yv.bjjhwx.cn

[S35] C++：map
来源：http://kv.jctech888.com.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://uz.chemitech.net.cn

[S36] C++：unordered_map
来源：http://bi.huixiangedu.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://io.yuexingan06.cn

[S37] C++：set
来源：http://ip.asd995.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ok.bjjhwx.cn

[S38] C++：排序
来源：http://ug.521024.cn

std::sort(v.begin(), v.end());
来源：http://at.panjiajie.cn

[S39] C++：自定义比较器排序
来源：http://kz.chemitech.net.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://dt.szxytkj.cn

[S40] C++：查找元素
来源：http://ub.asd995.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ez.nicolike.cn

[S41] C++：类与构造函数
来源：http://xs.szsharing.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://rt.jctech888.com.cn

[S42] C++：继承与虚函数
来源：http://km.hnjuh.cn

class B : public Base { public: void f() override {} };
来源：http://jx.panjiajie.cn

[S43] C++：智能指针
来源：http://gu.nszjky.cn

auto p = std::make_unique<int>(5);
来源：http://gk.huanxung.cn

[S44] C++：引用传参
来源：http://ki.shxzukj.cn

void inc(int &x) { ++x; }
来源：http://ry.lnxyls.cn

[S45] C++：lambda
来源：http://ek.yuntaijiaju.cn

auto add = [](int a, int b) { return a + b; };
来源：http://bo.chemitech.net.cn

[S46] C++：函数模板
来源：http://mk.9csxet.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hd.wgjwhj.cn

[S47] C++：结构化绑定遍历
来源：http://is.muxihuayi.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://xw.yuntaijiaju.cn

[S48] C++：逐行读文件
来源：http://yy.szsharing.cn

std::ifstream in("a.txt");  std::string line;
来源：http://kj.huixinmuqiang.cn

while (std::getline(in, line)) { }
来源：http://kb.muxihuayi.cn

[S49] C++：写文件
来源：http://hp.panjiajie.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://uj.huanxung.cn

[S50] C++：格式化数字
来源：http://qe.chemitech.net.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ne.gzmigu.cn

[S51] C++：显式类型转换
来源：http://bs.huanxung.cn

static_cast<double>(a) / b
来源：http://tb.szsharing.cn

[S52] C++：const 与 noexcept
来源：http://dr.jianghongdianzi.cn

int size() const noexcept { return n_; }
来源：http://nn.colortex.cn

[S53] C++：移动语义
来源：http://ju.hnjuh.cn

std::vector<int> w = std::move(v);
来源：http://wx.newstarts.cn

[S54] C++：异常处理
来源：http://oa.bookmarksfly.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://of.nszjky.cn

[S55] C++：结构化绑定
来源：http://eb.shtwfgs.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://jd.hnjuh.cn

[S56] C++：optional
来源：http://bx.bjjhwx.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://rv.huanxung.cn

[S57] C++：编译期常量
来源：http://jx.bookmarksfly.cn

constexpr int N = 10;
来源：http://ib.muxihuayi.cn

[S58] C++：命名空间
来源：http://xi.shtwfgs.cn

namespace ns { int f() { return 1; } }
来源：http://es.wgjwhj.cn

[S59] C++：静态断言
来源：http://cg.newstarts.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://tw.jianghongdianzi.cn

[S60] C++：遍历并删除元素
来源：http://uh.huixiangedu.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://sn.haigaiapp.cn

================================================================================
来源：http://cr.hahajie.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://de.yuexingan06.cn

================================================================================
来源：http://vx.haigaiapp.cn

[T01] Kotlin：Hello World
来源：http://nv.hnjuh.cn

println("Hello")
来源：http://qq.hnjuh.cn

[T02] Kotlin：变量
来源：http://gp.gzmigu.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://cj.hahajie.cn

[T03] Kotlin：字符串模板
来源：http://up.nicolike.cn

"值: $b"
来源：http://lu.shxzukj.cn

[T04] Kotlin：空安全
来源：http://ji.shxzskj.cn

val n: String? = null;  n?.length
来源：http://qx.szsharing.cn

[T05] Kotlin：when 表达式
来源：http://rp.szxytkj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://yz.yuexingan06.cn

[T06] Kotlin：集合映射
来源：http://uz.shxzskj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://uy.jctech888.com.cn

[T07] Kotlin：集合过滤
来源：http://rz.yuntaijiaju.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://xc.wgjwhj.cn

[T08] Kotlin：数据类
来源：http://rj.nicolike.cn

data class User(val name: String, val age: Int)
来源：http://tx.bookmarksfly.cn

[T09] Kotlin：扩展函数
来源：http://rm.szxytkj.cn

fun String.exclaim() = this + "!"
来源：http://ij.521024.cn

[T10] Kotlin：默认参数
来源：http://gh.haigaiapp.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://nj.haigaiapp.cn

[T11] Kotlin：协程
来源：http://vx.jctech888.com.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://kh.jianghongdianzi.cn

[T12] Kotlin：解构声明
来源：http://fs.newstarts.cn

val (a, b) = Pair(1, 2)
来源：http://zs.jianghongdianzi.cn

[T13] Kotlin：只读 Map
来源：http://jh.chemitech.net.cn

val m = mapOf("a" to 1)
来源：http://bo.huanxung.cn

[T14] Kotlin：循环
来源：http://uw.nicolike.cn

for (i in 1..10) println(i)
来源：http://qz.huixiangedu.cn

[T15] Kotlin：接口
来源：http://xb.nicolike.cn

interface Shape { fun area(): Double }
来源：http://vn.wgjwhj.cn

[T16] Swift：Hello World
来源：http://dc.9csxet.cn

print("Hello")
来源：http://vj.9csxet.cn

[T17] Swift：变量与常量
来源：http://us.huanxung.cn

var a = 1;  let b = 2
来源：http://hj.szxytkj.cn

[T18] Swift：字符串插值
来源：http://pf.hahajie.cn

"值: \(b)"
来源：http://kj.bookmarksfly.cn

[T19] Swift：可选绑定
来源：http://dt.yuexingan06.cn

if let n = opt { print(n) }
来源：http://nm.haigaiapp.cn

[T20] Swift：数组操作
来源：http://tg.huixinmuqiang.cn

var a = [1, 2, 3];  a.append(4)
来源：http://hc.jctech888.com.cn

[T21] Swift：遍历
来源：http://hm.jctech888.com.cn

for x in a { print(x) }
来源：http://am.9csxet.cn

[T22] Swift：字典
来源：http://sc.huanxung.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ax.shxzskj.cn

[T23] Swift：函数
来源：http://vc.asd995.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://xu.haigaiapp.cn

[T24] Swift：闭包
来源：http://dm.shxzukj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://tc.gzmigu.cn

[T25] Swift：结构体
来源：http://wk.bookmarksfly.cn

struct P { var x: Int }
来源：http://tu.hahajie.cn

[T26] Swift：类与重写
来源：http://og.521024.cn

class A: Base { override func f() {} }
来源：http://aa.asd995.cn

[T27] Swift：错误处理
来源：http://em.nszjky.cn

do { try f() } catch { print(error) }
来源：http://zr.bjjhwx.cn

[T28] Swift：枚举
来源：http://hv.muxihuayi.cn

enum Color { case red, green }
来源：http://wl.muxihuayi.cn

[T29] Swift：guard 提前返回
来源：http://ku.hahajie.cn

guard let x = opt else { return }
来源：http://vx.nszjky.cn

[T30] Swift：协议
来源：http://ui.shtwfgs.cn

protocol Shape { func area() -> Double }
来源：http://jb.huanxung.cn

[T31] Lua：Hello World
来源：http://om.wgjwhj.cn

print("Hello")
来源：http://om.hahajie.cn

[T32] Lua：局部变量
来源：http://av.panjiajie.cn

local a = 1
来源：http://cz.panjiajie.cn

[T33] Lua：表（数组）
来源：http://ws.bjjhwx.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://nn.9csxet.cn

[T34] Lua：遍历表
来源：http://no.szxytkj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://rh.huixiangedu.cn

[T35] Lua：字典表
来源：http://vl.jctech888.com.cn

local d = { a = 1 };  d.b = 2
来源：http://qq.huixiangedu.cn

[T36] Lua：函数
来源：http://fq.shxzskj.cn

function add(a, b) return a + b end
来源：http://fo.shxzukj.cn

[T37] Lua：字符串拼接
来源：http://em.lnxyls.cn

"a" .. "b"
来源：http://qr.asd995.cn

[T38] Lua：条件
来源：http://zm.muxihuayi.cn

if x > 0 then print("正") end
来源：http://pw.nicolike.cn

[T39] Lua：模式匹配
来源：http://sd.szxytkj.cn

string.find(s, "%d+")
来源：http://hk.9csxet.cn

[T40] Lua：元表
来源：http://tf.jctech888.com.cn

setmetatable({}, { __index = base })
来源：http://qy.shxzskj.cn

[T41] Perl：Hello World
来源：http://kx.hahajie.cn

print "Hello\n";
来源：http://gd.bookmarksfly.cn

[T42] Perl：变量类型
来源：http://rt.bookmarksfly.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ga.hahajie.cn

[T43] Perl：字符串插值
来源：http://li.huanxung.cn

"值: $a"
来源：http://kk.huanxung.cn

[T44] Perl：条件
来源：http://lx.huanxung.cn

if ($a > 0) { print "正"; }
来源：http://oo.9csxet.cn

[T45] Perl：数组遍历
来源：http://nh.bookmarksfly.cn

for my $x (@arr) { print $x; }
来源：http://hn.nszjky.cn

[T46] Perl：哈希操作
来源：http://tm.wgjwhj.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://zl.szsharing.cn

[T47] Perl：正则捕获
来源：http://vo.asd995.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://du.szsharing.cn

[T48] Perl：正则替换
来源：http://do.colortex.cn

$s =~ s/old/new/g;
来源：http://sl.huixiangedu.cn

[T49] Perl：函数
来源：http://ra.newstarts.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://yp.lnxyls.cn

[T50] Perl：逐行读文件
来源：http://fo.9csxet.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://rs.huixiangedu.cn

while (my $line = <$fh>) { print $line; }
来源：http://ko.chemitech.net.cn

[T51] Scala：Hello World
来源：http://bw.hnjuh.cn

println("Hello")
来源：http://ns.hahajie.cn

[T52] Scala：变量
来源：http://us.huixiangedu.cn

val a = 1;  var b = 2
来源：http://mb.521024.cn

[T53] Scala：字符串插值
来源：http://fg.chemitech.net.cn

s"值: $b"
来源：http://dq.hahajie.cn

[T54] Scala：集合映射
来源：http://tx.jctech888.com.cn

List(1, 2, 3).map(_ * 2)
来源：http://nm.jctech888.com.cn

[T55] Scala：集合过滤
来源：http://cv.huanxung.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ju.9csxet.cn

[T56] Scala：样例类
来源：http://wv.haigaiapp.cn

case class User(name: String, age: Int)
来源：http://lq.shxzukj.cn

[T57] Scala：模式匹配
来源：http://ox.gzmigu.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://cs.colortex.cn

[T58] Scala：函数定义
来源：http://uo.szxytkj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://gs.huanxung.cn

[T59] Scala：循环
来源：http://va.colortex.cn

for (i <- 1 to 10) println(i)
来源：http://ev.muxihuayi.cn

[T60] Scala：折叠
来源：http://pu.wgjwhj.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ul.szsharing.cn

================================================================================
来源：http://un.yuntaijiaju.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://vr.shxzukj.cn

================================================================================
来源：http://oe.szsharing.cn

[U01] Py：创建虚拟环境
来源：http://mv.yuexingan06.cn

python -m venv .venv && source .venv/bin/activate
来源：http://qo.muxihuayi.cn

[U02] Py：导出 / 安装依赖
来源：http://yx.huanxung.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://dq.newstarts.cn

[U03] Py：加载 .env 配置
来源：http://lc.asd995.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://nh.yuntaijiaju.cn

[U04] Py：变量调试打印
来源：http://pl.shtwfgs.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://gt.szxytkj.cn

[U05] Py：列表去重且保序
来源：http://xb.muxihuayi.cn

list(dict.fromkeys(arr))
来源：http://zt.9csxet.cn

[U06] Py：合并两个字典
来源：http://fy.bookmarksfly.cn

{**a, **b}
来源：http://fv.yuntaijiaju.cn

[U07] Py：反转字典键值
来源：http://nb.9csxet.cn

{v: k for k, v in d.items()}
来源：http://hb.gzmigu.cn

[U08] Py：展平二维列表
来源：http://pm.shxzukj.cn

[y for x in nested for y in x]
来源：http://hs.gzmigu.cn

[U09] Py：字典取最大值的键
来源：http://qi.gzmigu.cn

max(d, key=d.get)
来源：http://jn.jctech888.com.cn

[U10] Py：按值排序字典
来源：http://bx.nicolike.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://os.asd995.cn

[U11] Py：生成器表达式
来源：http://fx.huixinmuqiang.cn

(x * 2 for x in arr)
来源：http://gr.muxihuayi.cn

[U12] Py：取出现最多的 3 个元素
来源：http://sw.hnjuh.cn

Counter(arr).most_common(3)
来源：http://lj.huanxung.cn

[U13] Py：固定长度队列
来源：http://xm.wgjwhj.cn

deque(maxlen=10)
来源：http://hj.hahajie.cn

[U14] Py：分组收集到列表
来源：http://ah.szxytkj.cn

defaultdict(list)
来源：http://zs.bjjhwx.cn

[U15] Py：高精度计时
来源：http://mh.yuexingan06.cn

t = time.perf_counter()
来源：http://cc.521024.cn

[U16] Py：命令行参数解析
来源：http://co.9csxet.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://ww.huanxung.cn

[U17] Py：初始化日志
来源：http://wm.yuexingan06.cn

logging.basicConfig(level=logging.INFO)
来源：http://bj.nicolike.cn

[U18] Py：预编译正则
来源：http://ry.yuntaijiaju.cn

pat = re.compile(r"\d+")
来源：http://ux.asd995.cn

[U19] Py：正则替换带回调
来源：http://pj.lnxyls.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://oc.hnjuh.cn

[U20] Py：缓存函数结果
来源：http://so.haigaiapp.cn

@functools.lru_cache(maxsize=None)
来源：http://oc.yuexingan06.cn

[U21] Py：自定义上下文管理器
来源：http://oz.panjiajie.cn

@contextlib.contextmanager
来源：http://rg.muxihuayi.cn

[U22] Py：矩阵转置
来源：http://zh.szsharing.cn

list(zip(*m))
来源：http://ff.huixiangedu.cn

[U23] Py：分块读取大文件
来源：http://kw.lnxyls.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://qv.nicolike.cn

[U24] Py：路径操作
来源：http://xu.jianghongdianzi.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mw.nszjky.cn

[U25] Py：CSV 按字典读
来源：http://be.panjiajie.cn

csv.DictReader(f)
来源：http://tc.asd995.cn

[U26] Py：并发下载
来源：http://ai.jctech888.com.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://mi.huixiangedu.cn

[U27] Py：异步 HTTP
来源：http://sn.521024.cn

aiohttp.ClientSession() 配合 async with
来源：http://wo.jianghongdianzi.cn

[U28] Py：类型别名
来源：http://un.nicolike.cn

UserId = int
来源：http://hj.hnjuh.cn

[U29] Py：属性校验
来源：http://ux.huixiangedu.cn

@property 与 @x.setter 配合
来源：http://qa.jctech888.com.cn

[U30] Py：数据类
来源：http://wc.shtwfgs.cn

@dataclass(slots=True)
来源：http://th.muxihuayi.cn

[U31] Py：单测
来源：http://dn.haigaiapp.cn

python -m pytest -q
来源：http://jv.panjiajie.cn

[U32] Py：代码格式化
来源：http://jc.lnxyls.cn

ruff format . && ruff check --fix .
来源：http://ld.wgjwhj.cn

[U33] Py：打包发布
来源：http://vu.muxihuayi.cn

python -m build  （依赖 pyproject.toml）
来源：http://qh.9csxet.cn

[U34] Py：判断编码
来源：http://cg.szxytkj.cn

chardet.detect(raw)
来源：http://hd.hahajie.cn

[U35] Py：发送邮件
来源：http://rd.bjjhwx.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://ms.panjiajie.cn

[U36] Py：定时任务
来源：http://ja.gzmigu.cn

schedule.every(10).minutes.do(job)
来源：http://vq.hahajie.cn

[U37] Py：读写 Excel
来源：http://zn.shxzskj.cn

pandas.read_excel / DataFrame.to_excel
来源：http://ay.hnjuh.cn

[U38] Py：获取脚本所在目录
来源：http://il.nszjky.cn

Path(__file__).resolve().parent
来源：http://io.jianghongdianzi.cn

[U39] Py：判断是否在交互环境
来源：http://ze.bjjhwx.cn

sys.stdout.isatty()
来源：http://vf.shtwfgs.cn

[U40] Py：打印到标准错误
来源：http://uj.jianghongdianzi.cn

print("err", file=sys.stderr)
来源：http://ib.jianghongdianzi.cn

[U41] PHP：初始化 Composer 项目
来源：http://de.haigaiapp.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://tf.huanxung.cn

[U42] PHP：PSR-4 自动加载
来源：http://ws.nszjky.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://rj.yuntaijiaju.cn

[U43] PHP：声明命名空间
来源：http://ot.muxihuayi.cn

namespace App\Http;
来源：http://lp.newstarts.cn

[U44] PHP：开启严格类型
来源：http://cl.huanxung.cn

declare(strict_types=1);
来源：http://cg.shtwfgs.cn

[U45] PHP：类型声明与返回类型
来源：http://zb.shxzskj.cn

function add(int $a, int $b): int { return $a + $b; }
来源：http://sn.asd995.cn

[U46] PHP：可空类型
来源：http://uh.yuexingan06.cn

?string $name = null
来源：http://vz.jianghongdianzi.cn


<!-- 参考信息 -->