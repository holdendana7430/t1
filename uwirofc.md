代发 wailian999

int x; scanf("%d", &x);
来源：http://nh.szsharing.cn

[S04] C：字符串复制
来源：http://iz.huanxung.cn

char dst[32]; strcpy(dst, "hi");
来源：http://rv.szxytkj.cn

[S05] C：字符串长度
来源：http://cd.bookmarksfly.cn

strlen(s)
来源：http://fz.521024.cn

[S06] C：字符串比较
来源：http://kg.hnjuh.cn

strcmp(a, b) == 0
来源：http://rf.yuexingan06.cn

[S07] C：数组遍历求和
来源：http://es.shxzskj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ww.huixiangedu.cn

[S08] C：动态内存分配与释放
来源：http://ez.bjjhwx.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://vi.9csxet.cn

[S09] C：结构体定义与初始化
来源：http://bx.huixinmuqiang.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://pc.jctech888.com.cn

[S10] C：指针与解引用
来源：http://sr.gzmigu.cn

int *p = &a;  *p = 5;
来源：http://fq.521024.cn

[S11] C：逐行读文件
来源：http://sq.asd995.cn

FILE *f = fopen("a.txt", "r");
来源：http://ap.jianghongdianzi.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://se.szsharing.cn

fclose(f);
来源：http://ma.shxzukj.cn

[S12] C：写文件
来源：http://ow.asd995.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://kp.chemitech.net.cn

[S13] C：宏定义
来源：http://kg.shxzukj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ou.hahajie.cn

[S14] C：枚举
来源：http://ul.bookmarksfly.cn

enum Color { RED, GREEN, BLUE };
来源：http://di.shxzukj.cn

[S15] C：类型转换
来源：http://an.huixiangedu.cn

(double) a / b
来源：http://cc.wgjwhj.cn

[S16] C：位操作置位
来源：http://kp.colortex.cn

x |= (1 << 3);
来源：http://ge.shxzskj.cn

[S17] C：安全拼接字符串
来源：http://mt.muxihuayi.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hj.chemitech.net.cn

[S18] C：命令行参数
来源：http://jj.newstarts.cn

int main(int argc, char **argv)
来源：http://eq.huixinmuqiang.cn

[S19] C：快速排序
来源：http://gp.huixiangedu.cn

qsort(a, n, sizeof(int), cmp);
来源：http://mf.haigaiapp.cn

[S20] C：二分查找
来源：http://yc.shxzskj.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://md.huixiangedu.cn

[S21] C：字符类别判断
来源：http://nr.hnjuh.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://jt.gzmigu.cn

[S22] C：字符串转数字
来源：http://iv.wgjwhj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://mr.bookmarksfly.cn

[S23] C：随机数
来源：http://ig.huixinmuqiang.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://he.gzmigu.cn

[S24] C：获取本地时间
来源：http://ab.yuntaijiaju.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://tn.yuntaijiaju.cn

[S25] C：内存拷贝
来源：http://gq.yuntaijiaju.cn

memcpy(dst, src, n);
来源：http://av.yuexingan06.cn

[S26] C：内存清零
来源：http://jt.lnxyls.cn

memset(a, 0, sizeof a);
来源：http://iu.bjjhwx.cn

[S27] C：定义常量
来源：http://ad.hahajie.cn

const double PI = 3.14159;
来源：http://kw.szxytkj.cn

[S28] C：静态变量
来源：http://sq.yuexingan06.cn

static int counter = 0;
来源：http://uc.haigaiapp.cn

[S29] C：变参函数
来源：http://ya.huixinmuqiang.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://iz.bjjhwx.cn

[S30] C：头文件保护
来源：http://wo.gzmigu.cn

#ifndef X_H
来源：http://xi.hnjuh.cn

#define X_H
来源：http://ox.nicolike.cn

#endif
来源：http://bm.huanxung.cn

[S31] C++：Hello World
来源：http://xz.huanxung.cn

#include <iostream>
来源：http://rl.hnjuh.cn

int main() { std::cout << "Hello\n"; }
来源：http://xo.nicolike.cn

[S32] C++：字符串
来源：http://ep.9csxet.cn

std::string s = "hi";  s += "!";
来源：http://rz.shtwfgs.cn

[S33] C++：vector 增删
来源：http://pt.asd995.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ml.huixiangedu.cn

[S34] C++：遍历 vector
来源：http://pf.jctech888.com.cn

for (auto &x : v) { std::cout << x; }
来源：http://zp.nszjky.cn

[S35] C++：map
来源：http://to.szsharing.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://tn.nszjky.cn

[S36] C++：unordered_map
来源：http://ye.szsharing.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://br.wgjwhj.cn

[S37] C++：set
来源：http://wc.jianghongdianzi.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://zn.hnjuh.cn

[S38] C++：排序
来源：http://jm.jianghongdianzi.cn

std::sort(v.begin(), v.end());
来源：http://aa.9csxet.cn

[S39] C++：自定义比较器排序
来源：http://he.jianghongdianzi.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://es.haigaiapp.cn

[S40] C++：查找元素
来源：http://ic.shxzskj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://kf.haigaiapp.cn

[S41] C++：类与构造函数
来源：http://bm.lnxyls.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ix.huixiangedu.cn

[S42] C++：继承与虚函数
来源：http://sz.gzmigu.cn

class B : public Base { public: void f() override {} };
来源：http://kn.jianghongdianzi.cn

[S43] C++：智能指针
来源：http://oy.yuexingan06.cn

auto p = std::make_unique<int>(5);
来源：http://rc.nicolike.cn

[S44] C++：引用传参
来源：http://dt.nicolike.cn

void inc(int &x) { ++x; }
来源：http://sc.gzmigu.cn

[S45] C++：lambda
来源：http://rp.gzmigu.cn

auto add = [](int a, int b) { return a + b; };
来源：http://zd.shtwfgs.cn

[S46] C++：函数模板
来源：http://hs.nszjky.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xa.huixinmuqiang.cn

[S47] C++：结构化绑定遍历
来源：http://bz.chemitech.net.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wj.lnxyls.cn

[S48] C++：逐行读文件
来源：http://ya.huixiangedu.cn

std::ifstream in("a.txt");  std::string line;
来源：http://sn.shxzskj.cn

while (std::getline(in, line)) { }
来源：http://lc.bookmarksfly.cn

[S49] C++：写文件
来源：http://cq.lnxyls.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://eg.hahajie.cn

[S50] C++：格式化数字
来源：http://hs.521024.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://kk.jianghongdianzi.cn

[S51] C++：显式类型转换
来源：http://ap.newstarts.cn

static_cast<double>(a) / b
来源：http://va.gzmigu.cn

[S52] C++：const 与 noexcept
来源：http://bw.jctech888.com.cn

int size() const noexcept { return n_; }
来源：http://zx.haigaiapp.cn

[S53] C++：移动语义
来源：http://pt.yuntaijiaju.cn

std::vector<int> w = std::move(v);
来源：http://fi.colortex.cn

[S54] C++：异常处理
来源：http://vp.haigaiapp.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://au.nicolike.cn

[S55] C++：结构化绑定
来源：http://yr.muxihuayi.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://od.yuexingan06.cn

[S56] C++：optional
来源：http://af.bjjhwx.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://yp.wgjwhj.cn

[S57] C++：编译期常量
来源：http://pd.colortex.cn

constexpr int N = 10;
来源：http://hp.newstarts.cn

[S58] C++：命名空间
来源：http://lp.521024.cn

namespace ns { int f() { return 1; } }
来源：http://yv.shxzskj.cn

[S59] C++：静态断言
来源：http://pj.shtwfgs.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ey.jianghongdianzi.cn

[S60] C++：遍历并删除元素
来源：http://up.nicolike.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ej.jianghongdianzi.cn

================================================================================
来源：http://io.chemitech.net.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://de.bjjhwx.cn

================================================================================
来源：http://hl.panjiajie.cn

[T01] Kotlin：Hello World
来源：http://vw.gzmigu.cn

println("Hello")
来源：http://ge.wgjwhj.cn

[T02] Kotlin：变量
来源：http://ac.muxihuayi.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ew.hnjuh.cn

[T03] Kotlin：字符串模板
来源：http://wb.gzmigu.cn

"值: $b"
来源：http://zj.nszjky.cn

[T04] Kotlin：空安全
来源：http://nk.shtwfgs.cn

val n: String? = null;  n?.length
来源：http://wj.bjjhwx.cn

[T05] Kotlin：when 表达式
来源：http://xx.huixinmuqiang.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://tp.newstarts.cn

[T06] Kotlin：集合映射
来源：http://zw.panjiajie.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://gk.newstarts.cn

[T07] Kotlin：集合过滤
来源：http://gp.shxzukj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ku.gzmigu.cn

[T08] Kotlin：数据类
来源：http://xm.muxihuayi.cn

data class User(val name: String, val age: Int)
来源：http://qc.shxzukj.cn

[T09] Kotlin：扩展函数
来源：http://ks.shtwfgs.cn

fun String.exclaim() = this + "!"
来源：http://da.haigaiapp.cn

[T10] Kotlin：默认参数
来源：http://xg.newstarts.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://nn.chemitech.net.cn

[T11] Kotlin：协程
来源：http://wp.yuntaijiaju.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://it.bookmarksfly.cn

[T12] Kotlin：解构声明
来源：http://ey.hahajie.cn

val (a, b) = Pair(1, 2)
来源：http://yq.newstarts.cn

[T13] Kotlin：只读 Map
来源：http://eo.lnxyls.cn

val m = mapOf("a" to 1)
来源：http://si.nszjky.cn

[T14] Kotlin：循环
来源：http://cw.nicolike.cn

for (i in 1..10) println(i)
来源：http://ch.nszjky.cn

[T15] Kotlin：接口
来源：http://bw.nicolike.cn

interface Shape { fun area(): Double }
来源：http://rl.nicolike.cn

[T16] Swift：Hello World
来源：http://wm.huixiangedu.cn

print("Hello")
来源：http://xg.szxytkj.cn

[T17] Swift：变量与常量
来源：http://ff.lnxyls.cn

var a = 1;  let b = 2
来源：http://ik.yuexingan06.cn

[T18] Swift：字符串插值
来源：http://jf.chemitech.net.cn

"值: \(b)"
来源：http://yg.yuntaijiaju.cn

[T19] Swift：可选绑定
来源：http://fs.nicolike.cn

if let n = opt { print(n) }
来源：http://sj.wgjwhj.cn

[T20] Swift：数组操作
来源：http://fu.gzmigu.cn

var a = [1, 2, 3];  a.append(4)
来源：http://mr.shtwfgs.cn

[T21] Swift：遍历
来源：http://hh.bookmarksfly.cn

for x in a { print(x) }
来源：http://au.yuntaijiaju.cn

[T22] Swift：字典
来源：http://us.lnxyls.cn

var d = ["a": 1];  d["b"] = 2
来源：http://zr.shtwfgs.cn

[T23] Swift：函数
来源：http://hs.chemitech.net.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ow.wgjwhj.cn

[T24] Swift：闭包
来源：http://xj.jctech888.com.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://el.9csxet.cn

[T25] Swift：结构体
来源：http://dp.wgjwhj.cn

struct P { var x: Int }
来源：http://az.newstarts.cn

[T26] Swift：类与重写
来源：http://xh.wgjwhj.cn

class A: Base { override func f() {} }
来源：http://it.szsharing.cn

[T27] Swift：错误处理
来源：http://ff.jianghongdianzi.cn

do { try f() } catch { print(error) }
来源：http://tj.colortex.cn

[T28] Swift：枚举
来源：http://xb.hahajie.cn

enum Color { case red, green }
来源：http://mb.chemitech.net.cn

[T29] Swift：guard 提前返回
来源：http://si.newstarts.cn

guard let x = opt else { return }
来源：http://cn.shxzskj.cn

[T30] Swift：协议
来源：http://bu.shxzukj.cn

protocol Shape { func area() -> Double }
来源：http://ry.bookmarksfly.cn

[T31] Lua：Hello World
来源：http://wh.hahajie.cn

print("Hello")
来源：http://kr.yuexingan06.cn

[T32] Lua：局部变量
来源：http://lm.huanxung.cn

local a = 1
来源：http://gs.newstarts.cn

[T33] Lua：表（数组）
来源：http://ah.jianghongdianzi.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://kc.9csxet.cn

[T34] Lua：遍历表
来源：http://su.wgjwhj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://xf.muxihuayi.cn

[T35] Lua：字典表
来源：http://oc.huanxung.cn

local d = { a = 1 };  d.b = 2
来源：http://hp.muxihuayi.cn

[T36] Lua：函数
来源：http://lf.colortex.cn

function add(a, b) return a + b end
来源：http://ek.newstarts.cn

[T37] Lua：字符串拼接
来源：http://nm.yuntaijiaju.cn

"a" .. "b"
来源：http://pk.hahajie.cn

[T38] Lua：条件
来源：http://td.huixiangedu.cn

if x > 0 then print("正") end
来源：http://lg.nicolike.cn

[T39] Lua：模式匹配
来源：http://ws.szsharing.cn

string.find(s, "%d+")
来源：http://bi.yuntaijiaju.cn

[T40] Lua：元表
来源：http://ac.wgjwhj.cn

setmetatable({}, { __index = base })
来源：http://zr.gzmigu.cn

[T41] Perl：Hello World
来源：http://dd.521024.cn

print "Hello\n";
来源：http://cr.huixinmuqiang.cn

[T42] Perl：变量类型
来源：http://os.haigaiapp.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://wq.bjjhwx.cn

[T43] Perl：字符串插值
来源：http://bm.hnjuh.cn

"值: $a"
来源：http://oi.jctech888.com.cn

[T44] Perl：条件
来源：http://jh.szsharing.cn

if ($a > 0) { print "正"; }
来源：http://ch.newstarts.cn

[T45] Perl：数组遍历
来源：http://wz.521024.cn

for my $x (@arr) { print $x; }
来源：http://tp.gzmigu.cn

[T46] Perl：哈希操作
来源：http://id.yuexingan06.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://jt.shxzukj.cn

[T47] Perl：正则捕获
来源：http://ac.muxihuayi.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://oe.shxzukj.cn

[T48] Perl：正则替换
来源：http://vv.shtwfgs.cn

$s =~ s/old/new/g;
来源：http://ym.panjiajie.cn

[T49] Perl：函数
来源：http://pr.gzmigu.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://pl.szsharing.cn

[T50] Perl：逐行读文件
来源：http://tu.jctech888.com.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ud.szxytkj.cn

while (my $line = <$fh>) { print $line; }
来源：http://vm.hnjuh.cn

[T51] Scala：Hello World
来源：http://mj.shxzskj.cn

println("Hello")
来源：http://sd.shtwfgs.cn

[T52] Scala：变量
来源：http://ye.hahajie.cn

val a = 1;  var b = 2
来源：http://xx.lnxyls.cn

[T53] Scala：字符串插值
来源：http://qf.shxzukj.cn

s"值: $b"
来源：http://lk.huixinmuqiang.cn

[T54] Scala：集合映射
来源：http://uu.jianghongdianzi.cn

List(1, 2, 3).map(_ * 2)
来源：http://ao.huixiangedu.cn

[T55] Scala：集合过滤
来源：http://fw.asd995.cn

List(1, 2, 3).filter(_ > 1)
来源：http://kx.szxytkj.cn

[T56] Scala：样例类
来源：http://ld.newstarts.cn

case class User(name: String, age: Int)
来源：http://kd.muxihuayi.cn

[T57] Scala：模式匹配
来源：http://ap.bjjhwx.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ba.asd995.cn

[T58] Scala：函数定义
来源：http://gr.shtwfgs.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ki.huanxung.cn

[T59] Scala：循环
来源：http://qk.asd995.cn

for (i <- 1 to 10) println(i)
来源：http://oh.521024.cn

[T60] Scala：折叠
来源：http://ar.shxzukj.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://an.szsharing.cn

================================================================================
来源：http://zm.panjiajie.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://os.gzmigu.cn

================================================================================
来源：http://kp.521024.cn

[U01] Py：创建虚拟环境
来源：http://qx.hnjuh.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ow.shxzukj.cn

[U02] Py：导出 / 安装依赖
来源：http://aw.haigaiapp.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://kd.hahajie.cn

[U03] Py：加载 .env 配置
来源：http://ht.asd995.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://cm.newstarts.cn

[U04] Py：变量调试打印
来源：http://ub.9csxet.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://yu.shtwfgs.cn

[U05] Py：列表去重且保序
来源：http://rm.jianghongdianzi.cn

list(dict.fromkeys(arr))
来源：http://wd.colortex.cn

[U06] Py：合并两个字典
来源：http://sj.hahajie.cn

{**a, **b}
来源：http://km.nicolike.cn

[U07] Py：反转字典键值
来源：http://tc.chemitech.net.cn

{v: k for k, v in d.items()}
来源：http://uf.bookmarksfly.cn

[U08] Py：展平二维列表
来源：http://eo.huanxung.cn

[y for x in nested for y in x]
来源：http://cq.huanxung.cn

[U09] Py：字典取最大值的键
来源：http://oz.szsharing.cn

max(d, key=d.get)
来源：http://wu.bookmarksfly.cn

[U10] Py：按值排序字典
来源：http://uf.jianghongdianzi.cn

dict(sorted(d.items(), key=lambda kv: kv[1]))
来源：http://db.bjjhwx.cn

[U11] Py：生成器表达式
来源：http://sl.521024.cn

(x * 2 for x in arr)
来源：http://fe.yuexingan06.cn

[U12] Py：取出现最多的 3 个元素
来源：http://xq.shxzskj.cn

Counter(arr).most_common(3)
来源：http://cr.szxytkj.cn

[U13] Py：固定长度队列
来源：http://or.yuntaijiaju.cn

deque(maxlen=10)
来源：http://rf.szxytkj.cn

[U14] Py：分组收集到列表
来源：http://sh.yuntaijiaju.cn

defaultdict(list)
来源：http://tq.9csxet.cn

[U15] Py：高精度计时
来源：http://cc.gzmigu.cn

t = time.perf_counter()
来源：http://uz.jianghongdianzi.cn

[U16] Py：命令行参数解析
来源：http://nq.yuntaijiaju.cn

ap = argparse.ArgumentParser();  ap.add_argument("--name");  args = ap.parse_args()
来源：http://cl.szsharing.cn

[U17] Py：初始化日志
来源：http://pf.nicolike.cn

logging.basicConfig(level=logging.INFO)
来源：http://tx.lnxyls.cn

[U18] Py：预编译正则
来源：http://gz.gzmigu.cn

pat = re.compile(r"\d+")
来源：http://lz.szxytkj.cn

[U19] Py：正则替换带回调
来源：http://ab.nszjky.cn

re.sub(r"\d+", lambda m: str(int(m.group()) * 2), s)
来源：http://zz.nszjky.cn

[U20] Py：缓存函数结果
来源：http://am.shtwfgs.cn

@functools.lru_cache(maxsize=None)
来源：http://ig.panjiajie.cn

[U21] Py：自定义上下文管理器
来源：http://jm.chemitech.net.cn

@contextlib.contextmanager
来源：http://xs.newstarts.cn

[U22] Py：矩阵转置
来源：http://ri.lnxyls.cn

list(zip(*m))
来源：http://ps.bjjhwx.cn

[U23] Py：分块读取大文件
来源：http://zx.newstarts.cn

for chunk in iter(lambda: f.read(8192), b""):
来源：http://tk.huanxung.cn

[U24] Py：路径操作
来源：http://ns.bjjhwx.cn

Path("a/b.txt").parent.mkdir(parents=True, exist_ok=True)
来源：http://rt.nicolike.cn

[U25] Py：CSV 按字典读
来源：http://su.huixinmuqiang.cn

csv.DictReader(f)
来源：http://za.muxihuayi.cn

[U26] Py：并发下载
来源：http://ot.nicolike.cn

ThreadPoolExecutor(max_workers=8).map(fetch, urls)
来源：http://lx.huixinmuqiang.cn


<!-- 参考信息 -->