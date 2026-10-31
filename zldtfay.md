代发 wailian999

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ij.muxihuayi.cn

[S21] C：字符类别判断
来源：http://rq.bookmarksfly.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://vg.jianghongdianzi.cn

[S22] C：字符串转数字
来源：http://us.bjjhwx.cn

atoi("42");  strtod("3.14", NULL);
来源：http://nd.jianghongdianzi.cn

[S23] C：随机数
来源：http://hg.nicolike.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://vs.gzmigu.cn

[S24] C：获取本地时间
来源：http://zq.panjiajie.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://vb.jctech888.com.cn

[S25] C：内存拷贝
来源：http://bj.wgjwhj.cn

memcpy(dst, src, n);
来源：http://rv.hnjuh.cn

[S26] C：内存清零
来源：http://gp.asd995.cn

memset(a, 0, sizeof a);
来源：http://dq.huixiangedu.cn

[S27] C：定义常量
来源：http://fg.bookmarksfly.cn

const double PI = 3.14159;
来源：http://ll.nicolike.cn

[S28] C：静态变量
来源：http://mw.colortex.cn

static int counter = 0;
来源：http://pu.colortex.cn

[S29] C：变参函数
来源：http://ig.shtwfgs.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://co.shxzskj.cn

[S30] C：头文件保护
来源：http://gm.yuexingan06.cn

#ifndef X_H
来源：http://rt.521024.cn

#define X_H
来源：http://aw.colortex.cn

#endif
来源：http://ah.szsharing.cn

[S31] C++：Hello World
来源：http://vh.nicolike.cn

#include <iostream>
来源：http://iy.haigaiapp.cn

int main() { std::cout << "Hello\n"; }
来源：http://ts.haigaiapp.cn

[S32] C++：字符串
来源：http://lw.szsharing.cn

std::string s = "hi";  s += "!";
来源：http://hw.shxzskj.cn

[S33] C++：vector 增删
来源：http://lu.9csxet.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://jp.colortex.cn

[S34] C++：遍历 vector
来源：http://ic.bjjhwx.cn

for (auto &x : v) { std::cout << x; }
来源：http://ts.9csxet.cn

[S35] C++：map
来源：http://mp.gzmigu.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://bq.jianghongdianzi.cn

[S36] C++：unordered_map
来源：http://ml.nicolike.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ef.wgjwhj.cn

[S37] C++：set
来源：http://or.haigaiapp.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://pg.newstarts.cn

[S38] C++：排序
来源：http://ws.szsharing.cn

std::sort(v.begin(), v.end());
来源：http://eb.shxzukj.cn

[S39] C++：自定义比较器排序
来源：http://em.nicolike.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://am.lnxyls.cn

[S40] C++：查找元素
来源：http://zy.shxzskj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://lo.gzmigu.cn

[S41] C++：类与构造函数
来源：http://da.haigaiapp.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://rw.9csxet.cn

[S42] C++：继承与虚函数
来源：http://bs.521024.cn

class B : public Base { public: void f() override {} };
来源：http://jc.yuexingan06.cn

[S43] C++：智能指针
来源：http://jq.nicolike.cn

auto p = std::make_unique<int>(5);
来源：http://ms.huixiangedu.cn

[S44] C++：引用传参
来源：http://sx.huixinmuqiang.cn

void inc(int &x) { ++x; }
来源：http://di.yuntaijiaju.cn

[S45] C++：lambda
来源：http://va.bjjhwx.cn

auto add = [](int a, int b) { return a + b; };
来源：http://qj.shxzskj.cn

[S46] C++：函数模板
来源：http://js.panjiajie.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://lt.huixiangedu.cn

[S47] C++：结构化绑定遍历
来源：http://uu.yuntaijiaju.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ha.chemitech.net.cn

[S48] C++：逐行读文件
来源：http://gc.jctech888.com.cn

std::ifstream in("a.txt");  std::string line;
来源：http://pi.huixinmuqiang.cn

while (std::getline(in, line)) { }
来源：http://px.9csxet.cn

[S49] C++：写文件
来源：http://ux.muxihuayi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ly.bjjhwx.cn

[S50] C++：格式化数字
来源：http://xz.jctech888.com.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://dt.hnjuh.cn

[S51] C++：显式类型转换
来源：http://lr.yuexingan06.cn

static_cast<double>(a) / b
来源：http://kz.nszjky.cn

[S52] C++：const 与 noexcept
来源：http://vv.szxytkj.cn

int size() const noexcept { return n_; }
来源：http://km.bjjhwx.cn

[S53] C++：移动语义
来源：http://fc.szxytkj.cn

std::vector<int> w = std::move(v);
来源：http://kz.huanxung.cn

[S54] C++：异常处理
来源：http://zy.wgjwhj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://sa.shxzukj.cn

[S55] C++：结构化绑定
来源：http://fw.chemitech.net.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ba.nicolike.cn

[S56] C++：optional
来源：http://pv.huanxung.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://lq.asd995.cn

[S57] C++：编译期常量
来源：http://cq.muxihuayi.cn

constexpr int N = 10;
来源：http://qg.bjjhwx.cn

[S58] C++：命名空间
来源：http://qq.nszjky.cn

namespace ns { int f() { return 1; } }
来源：http://ko.huanxung.cn

[S59] C++：静态断言
来源：http://ko.nszjky.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://sf.bookmarksfly.cn

[S60] C++：遍历并删除元素
来源：http://ei.nicolike.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ug.panjiajie.cn

================================================================================
来源：http://hh.bookmarksfly.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://tt.9csxet.cn

================================================================================
来源：http://ed.yuexingan06.cn

[T01] Kotlin：Hello World
来源：http://sn.bookmarksfly.cn

println("Hello")
来源：http://xh.hahajie.cn

[T02] Kotlin：变量
来源：http://oq.9csxet.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ow.bjjhwx.cn

[T03] Kotlin：字符串模板
来源：http://we.shxzukj.cn

"值: $b"
来源：http://ll.bookmarksfly.cn

[T04] Kotlin：空安全
来源：http://cd.bookmarksfly.cn

val n: String? = null;  n?.length
来源：http://wn.haigaiapp.cn

[T05] Kotlin：when 表达式
来源：http://ol.shtwfgs.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://il.newstarts.cn

[T06] Kotlin：集合映射
来源：http://bd.muxihuayi.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://jx.lnxyls.cn

[T07] Kotlin：集合过滤
来源：http://gx.bjjhwx.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://kb.shxzukj.cn

[T08] Kotlin：数据类
来源：http://et.shtwfgs.cn

data class User(val name: String, val age: Int)
来源：http://jw.colortex.cn

[T09] Kotlin：扩展函数
来源：http://ar.shxzskj.cn

fun String.exclaim() = this + "!"
来源：http://ns.nszjky.cn

[T10] Kotlin：默认参数
来源：http://ms.haigaiapp.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://pl.yuntaijiaju.cn

[T11] Kotlin：协程
来源：http://da.colortex.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ka.muxihuayi.cn

[T12] Kotlin：解构声明
来源：http://up.huixinmuqiang.cn

val (a, b) = Pair(1, 2)
来源：http://sh.huanxung.cn

[T13] Kotlin：只读 Map
来源：http://mp.yuexingan06.cn

val m = mapOf("a" to 1)
来源：http://rg.hahajie.cn

[T14] Kotlin：循环
来源：http://nl.521024.cn

for (i in 1..10) println(i)
来源：http://cf.yuexingan06.cn

[T15] Kotlin：接口
来源：http://gf.chemitech.net.cn

interface Shape { fun area(): Double }
来源：http://ll.nszjky.cn

[T16] Swift：Hello World
来源：http://mz.panjiajie.cn

print("Hello")
来源：http://ng.hahajie.cn

[T17] Swift：变量与常量
来源：http://ky.haigaiapp.cn

var a = 1;  let b = 2
来源：http://xa.shtwfgs.cn

[T18] Swift：字符串插值
来源：http://xz.yuntaijiaju.cn

"值: \(b)"
来源：http://rs.hahajie.cn

[T19] Swift：可选绑定
来源：http://ee.newstarts.cn

if let n = opt { print(n) }
来源：http://be.bookmarksfly.cn

[T20] Swift：数组操作
来源：http://ld.haigaiapp.cn

var a = [1, 2, 3];  a.append(4)
来源：http://on.gzmigu.cn

[T21] Swift：遍历
来源：http://iu.lnxyls.cn

for x in a { print(x) }
来源：http://eh.lnxyls.cn

[T22] Swift：字典
来源：http://ua.huixiangedu.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ik.bookmarksfly.cn

[T23] Swift：函数
来源：http://ws.huanxung.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://rr.huixinmuqiang.cn

[T24] Swift：闭包
来源：http://tg.shxzskj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://tr.shtwfgs.cn

[T25] Swift：结构体
来源：http://ze.haigaiapp.cn

struct P { var x: Int }
来源：http://eu.haigaiapp.cn

[T26] Swift：类与重写
来源：http://hy.haigaiapp.cn

class A: Base { override func f() {} }
来源：http://pq.chemitech.net.cn

[T27] Swift：错误处理
来源：http://pb.bookmarksfly.cn

do { try f() } catch { print(error) }
来源：http://od.nszjky.cn

[T28] Swift：枚举
来源：http://hl.muxihuayi.cn

enum Color { case red, green }
来源：http://an.huixinmuqiang.cn

[T29] Swift：guard 提前返回
来源：http://xv.shxzskj.cn

guard let x = opt else { return }
来源：http://aa.chemitech.net.cn

[T30] Swift：协议
来源：http://mz.huixinmuqiang.cn

protocol Shape { func area() -> Double }
来源：http://dm.shxzskj.cn

[T31] Lua：Hello World
来源：http://pz.gzmigu.cn

print("Hello")
来源：http://tc.hnjuh.cn

[T32] Lua：局部变量
来源：http://sa.hahajie.cn

local a = 1
来源：http://yo.shtwfgs.cn

[T33] Lua：表（数组）
来源：http://ic.huixiangedu.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://wn.colortex.cn

[T34] Lua：遍历表
来源：http://sy.hahajie.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://qv.nicolike.cn

[T35] Lua：字典表
来源：http://jw.lnxyls.cn

local d = { a = 1 };  d.b = 2
来源：http://fx.newstarts.cn

[T36] Lua：函数
来源：http://ba.huixinmuqiang.cn

function add(a, b) return a + b end
来源：http://tp.huixiangedu.cn

[T37] Lua：字符串拼接
来源：http://yw.szsharing.cn

"a" .. "b"
来源：http://gc.shxzukj.cn

[T38] Lua：条件
来源：http://tk.shxzukj.cn

if x > 0 then print("正") end
来源：http://tf.9csxet.cn

[T39] Lua：模式匹配
来源：http://cq.huixiangedu.cn

string.find(s, "%d+")
来源：http://ko.jianghongdianzi.cn

[T40] Lua：元表
来源：http://ea.haigaiapp.cn

setmetatable({}, { __index = base })
来源：http://kt.panjiajie.cn

[T41] Perl：Hello World
来源：http://my.lnxyls.cn

print "Hello\n";
来源：http://km.huixiangedu.cn

[T42] Perl：变量类型
来源：http://bw.bjjhwx.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://tj.gzmigu.cn

[T43] Perl：字符串插值
来源：http://gc.chemitech.net.cn

"值: $a"
来源：http://ij.huixinmuqiang.cn

[T44] Perl：条件
来源：http://ao.shxzskj.cn

if ($a > 0) { print "正"; }
来源：http://xi.newstarts.cn

[T45] Perl：数组遍历
来源：http://ve.shxzskj.cn

for my $x (@arr) { print $x; }
来源：http://pn.521024.cn

[T46] Perl：哈希操作
来源：http://rg.shtwfgs.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ll.huanxung.cn

[T47] Perl：正则捕获
来源：http://km.huixinmuqiang.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://sq.bjjhwx.cn

[T48] Perl：正则替换
来源：http://zk.shxzskj.cn

$s =~ s/old/new/g;
来源：http://nq.szsharing.cn

[T49] Perl：函数
来源：http://vt.yuntaijiaju.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wr.shxzukj.cn

[T50] Perl：逐行读文件
来源：http://bw.chemitech.net.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ov.bjjhwx.cn

while (my $line = <$fh>) { print $line; }
来源：http://ba.hahajie.cn

[T51] Scala：Hello World
来源：http://yg.nszjky.cn

println("Hello")
来源：http://ip.wgjwhj.cn

[T52] Scala：变量
来源：http://sy.asd995.cn

val a = 1;  var b = 2
来源：http://px.jctech888.com.cn

[T53] Scala：字符串插值
来源：http://jq.haigaiapp.cn

s"值: $b"
来源：http://ho.shxzukj.cn

[T54] Scala：集合映射
来源：http://jb.shxzukj.cn

List(1, 2, 3).map(_ * 2)
来源：http://qq.shtwfgs.cn

[T55] Scala：集合过滤
来源：http://vq.wgjwhj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://gb.haigaiapp.cn

[T56] Scala：样例类
来源：http://mv.wgjwhj.cn

case class User(name: String, age: Int)
来源：http://dh.panjiajie.cn

[T57] Scala：模式匹配
来源：http://mw.newstarts.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://sj.nszjky.cn

[T58] Scala：函数定义
来源：http://de.shxzskj.cn

def add(a: Int, b: Int): Int = a + b
来源：http://uu.yuntaijiaju.cn

[T59] Scala：循环
来源：http://vb.wgjwhj.cn

for (i <- 1 to 10) println(i)
来源：http://hq.shxzukj.cn

[T60] Scala：折叠
来源：http://pj.yuntaijiaju.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://xl.muxihuayi.cn

================================================================================
来源：http://fb.szsharing.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://xr.hnjuh.cn

================================================================================
来源：http://xj.bjjhwx.cn

[U01] Py：创建虚拟环境
来源：http://pv.nszjky.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ow.lnxyls.cn

[U02] Py：导出 / 安装依赖
来源：http://tg.wgjwhj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://qn.huixiangedu.cn

[U03] Py：加载 .env 配置
来源：http://cu.9csxet.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ne.haigaiapp.cn

[U04] Py：变量调试打印
来源：http://uk.panjiajie.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://cw.hahajie.cn

[U05] Py：列表去重且保序
来源：http://jg.bjjhwx.cn

list(dict.fromkeys(arr))
来源：http://pd.shxzukj.cn

[U06] Py：合并两个字典
来源：http://xu.asd995.cn

{**a, **b}
来源：http://le.shtwfgs.cn

[U07] Py：反转字典键值
来源：http://kv.nszjky.cn

{v: k for k, v in d.items()}
来源：http://as.9csxet.cn

[U08] Py：展平二维列表
来源：http://pe.521024.cn

[y for x in nested for y in x]
来源：http://hq.colortex.cn

[U09] Py：字典取最大值的键
来源：http://vq.bookmarksfly.cn

max(d, key=d.get)
来源：http://es.colortex.cn

[U10] Py：按值排序字典
来源：http://yk.hnjuh.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://yv.muxihuayi.cn

[U11] Py：生成器表达式
来源：http://rp.521024.cn

(x * 2 for x in arr)
来源：http://xe.szsharing.cn

[U12] Py：取出现最多的 3 个元素
来源：http://lx.panjiajie.cn

Counter(arr).most_common(3)
来源：http://qi.chemitech.net.cn

[U13] Py：固定长度队列
来源：http://db.asd995.cn

deque(maxlen=10)
来源：http://ed.yuexingan06.cn

[U14] Py：分组收集到列表
来源：http://am.haigaiapp.cn

defaultdict(list)
来源：http://jo.panjiajie.cn

[U15] Py：高精度计时
来源：http://vg.huixinmuqiang.cn

t = time.perf_counter()
来源：http://mt.asd995.cn

[U16] Py：命令行参数解析
来源：http://jd.521024.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://dw.yuexingan06.cn

[U17] Py：初始化日志
来源：http://ni.huixinmuqiang.cn

logging.basicConfig(level=logging.INFO)
来源：http://fc.haigaiapp.cn

[U18] Py：预编译正则
来源：http://hd.colortex.cn

pat = re.compile(r"\d+")
来源：http://jq.chemitech.net.cn

[U19] Py：正则替换带回调
来源：http://tq.nszjky.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://zt.521024.cn

[U20] Py：缓存函数结果
来源：http://zf.szsharing.cn

@functools.lru_cache(maxsize=None)
来源：http://hl.shtwfgs.cn

[U21] Py：自定义上下文管理器
来源：http://jp.colortex.cn

@contextlib.contextmanager
来源：http://qb.bookmarksfly.cn

[U22] Py：矩阵转置
来源：http://xo.colortex.cn

list(zip(*m))
来源：http://fc.haigaiapp.cn

[U23] Py：分块读取大文件
来源：http://ep.jctech888.com.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://gy.haigaiapp.cn

[U24] Py：路径操作
来源：http://fm.haigaiapp.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://mf.bookmarksfly.cn

[U25] Py：CSV 按字典读
来源：http://fv.nszjky.cn

csv.DictReader(f)
来源：http://fv.9csxet.cn

[U26] Py：并发下载
来源：http://nv.hahajie.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://am.huixiangedu.cn

[U27] Py：异步 HTTP
来源：http://ff.shxzskj.cn

aiohttp.ClientSession() 配合 async with
来源：http://rw.jctech888.com.cn

[U28] Py：类型别名
来源：http://xg.chemitech.net.cn

UserId = int
来源：http://vh.shxzukj.cn

[U29] Py：属性校验
来源：http://kk.newstarts.cn

@property 与 @x.setter 配合
来源：http://xr.yuntaijiaju.cn

[U30] Py：数据类
来源：http://ko.hahajie.cn

@dataclass(slots=True)
来源：http://wo.szxytkj.cn

[U31] Py：单测
来源：http://lc.nszjky.cn

python -m pytest -q
来源：http://fb.shxzukj.cn

[U32] Py：代码格式化
来源：http://tu.gzmigu.cn

ruff format . && ruff check --fix .
来源：http://cz.shtwfgs.cn

[U33] Py：打包发布
来源：http://ru.wgjwhj.cn

python -m build  （依赖 pyproject.toml）
来源：http://gk.huixiangedu.cn

[U34] Py：判断编码
来源：http://pk.nicolike.cn

chardet.detect(raw)
来源：http://bb.colortex.cn

[U35] Py：发送邮件
来源：http://vy.gzmigu.cn

smtplib.SMTP_SSL(...).send_message(msg)
来源：http://bt.colortex.cn

[U36] Py：定时任务
来源：http://lc.huixiangedu.cn

schedule.every(10).minutes.do(job)
来源：http://dn.nszjky.cn

[U37] Py：读写 Excel
来源：http://ya.gzmigu.cn

pandas.read_excel / DataFrame.to_excel
来源：http://qu.panjiajie.cn

[U38] Py：获取脚本所在目录
来源：http://jc.hahajie.cn

Path(__file__).resolve().parent
来源：http://jj.colortex.cn

[U39] Py：判断是否在交互环境
来源：http://ey.huixiangedu.cn

sys.stdout.isatty()
来源：http://rw.yuexingan06.cn

[U40] Py：打印到标准错误
来源：http://zj.asd995.cn

print("err", file=sys.stderr)
来源：http://dd.shxzskj.cn

[U41] PHP：初始化 Composer 项目
来源：http://gj.hahajie.cn

composer init;  composer require guzzlehttp/guzzle
来源：http://vp.lnxyls.cn

[U42] PHP：PSR-4 自动加载
来源：http://mr.szxytkj.cn

"autoload": { "psr-4": { "App\\": "src/" } }
来源：http://le.wgjwhj.cn

[U43] PHP：声明命名空间
来源：http://bo.yuexingan06.cn

namespace App\Http;
来源：http://sc.asd995.cn

[U44] PHP：开启严格类型
来源：http://jc.hahajie.cn

declare(strict_types=1);
来源：http://rm.muxihuayi.cn


<!-- 参考信息 -->