代发 wailian999

openssl rand -hex 16
来源：http://ow.lnxyls.cn

[R68] 计算文件校验值
来源：http://zz.szxytkj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://jr.huixinmuqiang.cn

[R69] 生成随机密码
来源：http://tf.newstarts.cn

head -c 16 /dev/urandom | base64
来源：http://fr.nicolike.cn

[R70] 时间戳与互转
来源：http://ma.szsharing.cn

date +%s;  date -d @1700000000
来源：http://lw.shtwfgs.cn

[R71] 日期格式化
来源：http://ve.jianghongdianzi.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://rw.wgjwhj.cn

[R72] 等待端口就绪
来源：http://zk.yuexingan06.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://dx.jctech888.com.cn

[R73] 分割大日志
来源：http://xw.huixinmuqiang.cn

split -l 1000 big.log part_
来源：http://vs.jctech888.com.cn

[R74] 批量重命名
来源：http://on.szsharing.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://sm.yuntaijiaju.cn

[R75] 导出环境变量
来源：http://ia.gzmigu.cn

export PATH="$HOME/bin:$PATH"
来源：http://lh.wgjwhj.cn

[R76] 使用临时文件
来源：http://wr.bookmarksfly.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://fr.huixinmuqiang.cn

[R77] 读取用户输入
来源：http://uh.jianghongdianzi.cn

read -rp "请输入: " ans
来源：http://hn.huanxung.cn

[R78] 交互式菜单
来源：http://xm.wgjwhj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://yb.panjiajie.cn

[R79] 解析命令行选项
来源：http://ot.hnjuh.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ur.shxzukj.cn

[R80] 查看脚本执行耗时
来源：http://fp.huanxung.cn

time ./run.sh
来源：http://tn.shxzskj.cn

================================================================================
来源：http://vv.huanxung.cn

S. C / C++ 专题
来源：http://cx.haigaiapp.cn

================================================================================
来源：http://to.hnjuh.cn

[S01] C：Hello World
来源：http://eb.asd995.cn

#include <stdio.h>
来源：http://db.yuntaijiaju.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://eb.yuexingan06.cn

[S02] C：变量与格式化输出
来源：http://mo.muxihuayi.cn

int a = 10; printf("%d\n", a);
来源：http://uu.shxzskj.cn

[S03] C：读入整数
来源：http://cn.huixinmuqiang.cn

int x; scanf("%d", &x);
来源：http://uq.jianghongdianzi.cn

[S04] C：字符串复制
来源：http://id.huixiangedu.cn

char dst[32]; strcpy(dst, "hi");
来源：http://yg.haigaiapp.cn

[S05] C：字符串长度
来源：http://ti.newstarts.cn

strlen(s)
来源：http://ej.asd995.cn

[S06] C：字符串比较
来源：http://iz.bjjhwx.cn

strcmp(a, b) == 0
来源：http://ac.bjjhwx.cn

[S07] C：数组遍历求和
来源：http://po.shtwfgs.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://av.huixinmuqiang.cn

[S08] C：动态内存分配与释放
来源：http://ol.huixiangedu.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://uq.521024.cn

[S09] C：结构体定义与初始化
来源：http://hw.szxytkj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://jh.521024.cn

[S10] C：指针与解引用
来源：http://xw.szxytkj.cn

int *p = &a;  *p = 5;
来源：http://bh.asd995.cn

[S11] C：逐行读文件
来源：http://ib.521024.cn

FILE *f = fopen("a.txt", "r");
来源：http://mu.huixiangedu.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://kr.szxytkj.cn

fclose(f);
来源：http://se.colortex.cn

[S12] C：写文件
来源：http://jj.shtwfgs.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://dx.shxzukj.cn

[S13] C：宏定义
来源：http://rd.nszjky.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ez.9csxet.cn

[S14] C：枚举
来源：http://wx.szxytkj.cn

enum Color { RED, GREEN, BLUE };
来源：http://fh.bookmarksfly.cn

[S15] C：类型转换
来源：http://sn.hnjuh.cn

(double) a / b
来源：http://gw.shtwfgs.cn

[S16] C：位操作置位
来源：http://qe.9csxet.cn

x |= (1 << 3);
来源：http://sx.shtwfgs.cn

[S17] C：安全拼接字符串
来源：http://um.nicolike.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://fz.haigaiapp.cn

[S18] C：命令行参数
来源：http://qc.wgjwhj.cn

int main(int argc, char **argv)
来源：http://ls.huixiangedu.cn

[S19] C：快速排序
来源：http://wy.hnjuh.cn

qsort(a, n, sizeof(int), cmp);
来源：http://vy.szxytkj.cn

[S20] C：二分查找
来源：http://ts.jctech888.com.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://gp.muxihuayi.cn

[S21] C：字符类别判断
来源：http://oq.521024.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ci.gzmigu.cn

[S22] C：字符串转数字
来源：http://oh.hnjuh.cn

atoi("42");  strtod("3.14", NULL);
来源：http://du.panjiajie.cn

[S23] C：随机数
来源：http://if.huanxung.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://fa.szsharing.cn

[S24] C：获取本地时间
来源：http://nt.hahajie.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://lp.shtwfgs.cn

[S25] C：内存拷贝
来源：http://og.shxzskj.cn

memcpy(dst, src, n);
来源：http://un.haigaiapp.cn

[S26] C：内存清零
来源：http://km.huixiangedu.cn

memset(a, 0, sizeof a);
来源：http://hy.huixiangedu.cn

[S27] C：定义常量
来源：http://uh.huixiangedu.cn

const double PI = 3.14159;
来源：http://as.panjiajie.cn

[S28] C：静态变量
来源：http://nx.asd995.cn

static int counter = 0;
来源：http://mn.wgjwhj.cn

[S29] C：变参函数
来源：http://wq.bookmarksfly.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ip.nszjky.cn

[S30] C：头文件保护
来源：http://fy.shxzukj.cn

#ifndef X_H
来源：http://kv.521024.cn

#define X_H
来源：http://hq.521024.cn

#endif
来源：http://jr.bjjhwx.cn

[S31] C++：Hello World
来源：http://ib.huanxung.cn

#include <iostream>
来源：http://md.nicolike.cn

int main() { std::cout << "Hello\n"; }
来源：http://vk.colortex.cn

[S32] C++：字符串
来源：http://oh.newstarts.cn

std::string s = "hi";  s += "!";
来源：http://fn.wgjwhj.cn

[S33] C++：vector 增删
来源：http://ak.shxzukj.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ou.huixinmuqiang.cn

[S34] C++：遍历 vector
来源：http://dy.hnjuh.cn

for (auto &x : v) { std::cout << x; }
来源：http://ur.newstarts.cn

[S35] C++：map
来源：http://ru.yuexingan06.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://fb.9csxet.cn

[S36] C++：unordered_map
来源：http://pq.nicolike.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://pc.wgjwhj.cn

[S37] C++：set
来源：http://mf.jianghongdianzi.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://jf.9csxet.cn

[S38] C++：排序
来源：http://xo.shxzukj.cn

std::sort(v.begin(), v.end());
来源：http://bg.jctech888.com.cn

[S39] C++：自定义比较器排序
来源：http://jg.haigaiapp.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ap.yuntaijiaju.cn

[S40] C++：查找元素
来源：http://ph.huixinmuqiang.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://pz.hnjuh.cn

[S41] C++：类与构造函数
来源：http://os.9csxet.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://iq.jianghongdianzi.cn

[S42] C++：继承与虚函数
来源：http://zx.nszjky.cn

class B : public Base { public: void f() override {} };
来源：http://va.nszjky.cn

[S43] C++：智能指针
来源：http://kz.hnjuh.cn

auto p = std::make_unique<int>(5);
来源：http://xu.nicolike.cn

[S44] C++：引用传参
来源：http://pd.bjjhwx.cn

void inc(int &x) { ++x; }
来源：http://oo.shtwfgs.cn

[S45] C++：lambda
来源：http://oj.nicolike.cn

auto add = [](int a, int b) { return a + b; };
来源：http://vg.hnjuh.cn

[S46] C++：函数模板
来源：http://fn.gzmigu.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ow.lnxyls.cn

[S47] C++：结构化绑定遍历
来源：http://mg.shxzskj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wd.lnxyls.cn

[S48] C++：逐行读文件
来源：http://dt.szxytkj.cn

std::ifstream in("a.txt");  std::string line;
来源：http://qk.nszjky.cn

while (std::getline(in, line)) { }
来源：http://io.shxzukj.cn

[S49] C++：写文件
来源：http://ro.shtwfgs.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://iz.huixinmuqiang.cn

[S50] C++：格式化数字
来源：http://da.jctech888.com.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://se.bjjhwx.cn

[S51] C++：显式类型转换
来源：http://wj.shxzukj.cn

static_cast<double>(a) / b
来源：http://vr.wgjwhj.cn

[S52] C++：const 与 noexcept
来源：http://du.huixiangedu.cn

int size() const noexcept { return n_; }
来源：http://rw.panjiajie.cn

[S53] C++：移动语义
来源：http://ay.nicolike.cn

std::vector<int> w = std::move(v);
来源：http://gb.hahajie.cn

[S54] C++：异常处理
来源：http://eu.asd995.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ql.9csxet.cn

[S55] C++：结构化绑定
来源：http://rg.huanxung.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ib.hahajie.cn

[S56] C++：optional
来源：http://pt.jctech888.com.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://il.jctech888.com.cn

[S57] C++：编译期常量
来源：http://kj.lnxyls.cn

constexpr int N = 10;
来源：http://gf.muxihuayi.cn

[S58] C++：命名空间
来源：http://fc.huanxung.cn

namespace ns { int f() { return 1; } }
来源：http://nh.jctech888.com.cn

[S59] C++：静态断言
来源：http://op.yuntaijiaju.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://sq.haigaiapp.cn

[S60] C++：遍历并删除元素
来源：http://wn.szxytkj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://em.shxzskj.cn

================================================================================
来源：http://at.yuntaijiaju.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://qj.chemitech.net.cn

================================================================================
来源：http://hm.chemitech.net.cn

[T01] Kotlin：Hello World
来源：http://vk.521024.cn

println("Hello")
来源：http://ct.gzmigu.cn

[T02] Kotlin：变量
来源：http://ie.521024.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://nd.gzmigu.cn

[T03] Kotlin：字符串模板
来源：http://ny.chemitech.net.cn

"值: $b"
来源：http://fz.jianghongdianzi.cn

[T04] Kotlin：空安全
来源：http://ub.huixiangedu.cn

val n: String? = null;  n?.length
来源：http://ei.huixiangedu.cn

[T05] Kotlin：when 表达式
来源：http://lj.9csxet.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://lk.9csxet.cn

[T06] Kotlin：集合映射
来源：http://wm.huixiangedu.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://gm.yuntaijiaju.cn

[T07] Kotlin：集合过滤
来源：http://io.wgjwhj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://qc.wgjwhj.cn

[T08] Kotlin：数据类
来源：http://jc.jianghongdianzi.cn

data class User(val name: String, val age: Int)
来源：http://ro.jianghongdianzi.cn

[T09] Kotlin：扩展函数
来源：http://qt.szsharing.cn

fun String.exclaim() = this + "!"
来源：http://gt.yuexingan06.cn

[T10] Kotlin：默认参数
来源：http://st.szxytkj.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://pa.521024.cn

[T11] Kotlin：协程
来源：http://ls.nicolike.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://em.asd995.cn

[T12] Kotlin：解构声明
来源：http://gg.asd995.cn

val (a, b) = Pair(1, 2)
来源：http://sn.521024.cn

[T13] Kotlin：只读 Map
来源：http://cv.gzmigu.cn

val m = mapOf("a" to 1)
来源：http://sd.nicolike.cn

[T14] Kotlin：循环
来源：http://xd.chemitech.net.cn

for (i in 1..10) println(i)
来源：http://vt.gzmigu.cn

[T15] Kotlin：接口
来源：http://sn.shtwfgs.cn

interface Shape { fun area(): Double }
来源：http://wn.gzmigu.cn

[T16] Swift：Hello World
来源：http://rp.shxzukj.cn

print("Hello")
来源：http://oq.bookmarksfly.cn

[T17] Swift：变量与常量
来源：http://wh.nszjky.cn

var a = 1;  let b = 2
来源：http://ne.jianghongdianzi.cn

[T18] Swift：字符串插值
来源：http://un.nicolike.cn

"值: \(b)"
来源：http://lq.lnxyls.cn

[T19] Swift：可选绑定
来源：http://um.wgjwhj.cn

if let n = opt { print(n) }
来源：http://cy.asd995.cn

[T20] Swift：数组操作
来源：http://uh.bookmarksfly.cn

var a = [1, 2, 3];  a.append(4)
来源：http://em.521024.cn

[T21] Swift：遍历
来源：http://ra.jctech888.com.cn

for x in a { print(x) }
来源：http://sd.colortex.cn

[T22] Swift：字典
来源：http://iu.shxzskj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://do.huixiangedu.cn

[T23] Swift：函数
来源：http://ce.bookmarksfly.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://vt.colortex.cn

[T24] Swift：闭包
来源：http://kw.szxytkj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://xh.panjiajie.cn

[T25] Swift：结构体
来源：http://yx.9csxet.cn

struct P { var x: Int }
来源：http://xq.bookmarksfly.cn

[T26] Swift：类与重写
来源：http://tz.jianghongdianzi.cn

class A: Base { override func f() {} }
来源：http://sa.yuexingan06.cn

[T27] Swift：错误处理
来源：http://dl.gzmigu.cn

do { try f() } catch { print(error) }
来源：http://yt.yuexingan06.cn

[T28] Swift：枚举
来源：http://cc.asd995.cn

enum Color { case red, green }
来源：http://nj.shxzskj.cn

[T29] Swift：guard 提前返回
来源：http://yc.asd995.cn

guard let x = opt else { return }
来源：http://bg.hnjuh.cn

[T30] Swift：协议
来源：http://sp.huanxung.cn

protocol Shape { func area() -> Double }
来源：http://ye.shxzukj.cn

[T31] Lua：Hello World
来源：http://ij.521024.cn

print("Hello")
来源：http://xd.newstarts.cn

[T32] Lua：局部变量
来源：http://yq.szxytkj.cn

local a = 1
来源：http://ny.panjiajie.cn

[T33] Lua：表（数组）
来源：http://tt.hahajie.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ei.jianghongdianzi.cn

[T34] Lua：遍历表
来源：http://ho.hnjuh.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://fk.wgjwhj.cn

[T35] Lua：字典表
来源：http://cc.haigaiapp.cn

local d = { a = 1 };  d.b = 2
来源：http://bv.gzmigu.cn

[T36] Lua：函数
来源：http://yo.521024.cn

function add(a, b) return a + b end
来源：http://qf.jianghongdianzi.cn

[T37] Lua：字符串拼接
来源：http://ib.panjiajie.cn

"a" .. "b"
来源：http://gz.chemitech.net.cn

[T38] Lua：条件
来源：http://zm.haigaiapp.cn

if x > 0 then print("正") end
来源：http://iw.521024.cn

[T39] Lua：模式匹配
来源：http://zj.521024.cn

string.find(s, "%d+")
来源：http://us.muxihuayi.cn

[T40] Lua：元表
来源：http://hz.bookmarksfly.cn

setmetatable({}, { __index = base })
来源：http://nc.nicolike.cn

[T41] Perl：Hello World
来源：http://up.huixiangedu.cn

print "Hello\n";
来源：http://hl.szsharing.cn

[T42] Perl：变量类型
来源：http://kn.9csxet.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hy.bookmarksfly.cn

[T43] Perl：字符串插值
来源：http://bo.colortex.cn

"值: $a"
来源：http://nt.colortex.cn

[T44] Perl：条件
来源：http://hj.9csxet.cn

if ($a > 0) { print "正"; }
来源：http://sd.huixinmuqiang.cn

[T45] Perl：数组遍历
来源：http://lo.shtwfgs.cn

for my $x (@arr) { print $x; }
来源：http://rk.shxzskj.cn

[T46] Perl：哈希操作
来源：http://ju.chemitech.net.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://lx.hnjuh.cn

[T47] Perl：正则捕获
来源：http://um.yuntaijiaju.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://lb.nicolike.cn

[T48] Perl：正则替换
来源：http://qk.nicolike.cn

$s =~ s/old/new/g;
来源：http://zv.hnjuh.cn

[T49] Perl：函数
来源：http://bh.yuntaijiaju.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://pp.muxihuayi.cn

[T50] Perl：逐行读文件
来源：http://gg.asd995.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://cm.bjjhwx.cn

while (my $line = <$fh>) { print $line; }
来源：http://vz.shtwfgs.cn

[T51] Scala：Hello World
来源：http://zb.szsharing.cn

println("Hello")
来源：http://ia.muxihuayi.cn

[T52] Scala：变量
来源：http://br.bookmarksfly.cn

val a = 1;  var b = 2
来源：http://ch.shxzskj.cn

[T53] Scala：字符串插值
来源：http://uz.huixinmuqiang.cn

s"值: $b"
来源：http://eh.haigaiapp.cn

[T54] Scala：集合映射
来源：http://me.szxytkj.cn

List(1, 2, 3).map(_ * 2)
来源：http://ji.yuexingan06.cn

[T55] Scala：集合过滤
来源：http://qh.wgjwhj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ah.hnjuh.cn

[T56] Scala：样例类
来源：http://id.szxytkj.cn

case class User(name: String, age: Int)
来源：http://ym.huanxung.cn

[T57] Scala：模式匹配
来源：http://iw.hnjuh.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://el.jctech888.com.cn

[T58] Scala：函数定义
来源：http://nr.nicolike.cn

def add(a: Int, b: Int): Int = a + b
来源：http://qx.shxzukj.cn

[T59] Scala：循环
来源：http://dp.panjiajie.cn

for (i <- 1 to 10) println(i)
来源：http://mr.bookmarksfly.cn

[T60] Scala：折叠
来源：http://cs.newstarts.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://uh.nszjky.cn

================================================================================
来源：http://ns.lnxyls.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://nx.lnxyls.cn

================================================================================
来源：http://wd.hnjuh.cn

[U01] Py：创建虚拟环境
来源：http://np.hahajie.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ny.shtwfgs.cn

[U02] Py：导出 / 安装依赖
来源：http://oz.shtwfgs.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://dl.9csxet.cn

[U03] Py：加载 .env 配置
来源：http://rw.shxzskj.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://ks.hahajie.cn

[U04] Py：变量调试打印
来源：http://yl.bookmarksfly.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://rv.hahajie.cn

[U05] Py：列表去重且保序
来源：http://bp.huixiangedu.cn

list(dict.fromkeys(arr))
来源：http://kt.jctech888.com.cn

[U06] Py：合并两个字典
来源：http://uj.chemitech.net.cn

{**a, **b}
来源：http://ur.newstarts.cn

[U07] Py：反转字典键值
来源：http://xw.nicolike.cn

{v: k for k, v in d.items()}
来源：http://gr.huixiangedu.cn

[U08] Py：展平二维列表
来源：http://ft.huanxung.cn

[y for x in nested for y in x]
来源：http://ew.wgjwhj.cn


<!-- 参考信息 -->