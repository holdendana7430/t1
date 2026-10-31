代发 wailian999

openssl rand -hex 16
来源：http://sy.yuexingan06.cn

[R68] 计算文件校验值
来源：http://bi.chemitech.net.cn

sha256sum a.txt;  md5sum a.txt
来源：http://sm.gzmigu.cn

[R69] 生成随机密码
来源：http://bf.colortex.cn

head -c 16 /dev/urandom | base64
来源：http://qp.shxzukj.cn

[R70] 时间戳与互转
来源：http://hs.bjjhwx.cn

date +%s;  date -d @1700000000
来源：http://hv.asd995.cn

[R71] 日期格式化
来源：http://ug.asd995.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://qn.hahajie.cn

[R72] 等待端口就绪
来源：http://kc.shtwfgs.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://qg.jctech888.com.cn

[R73] 分割大日志
来源：http://vb.hahajie.cn

split -l 1000 big.log part_
来源：http://gx.nicolike.cn

[R74] 批量重命名
来源：http://hc.muxihuayi.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://fi.nszjky.cn

[R75] 导出环境变量
来源：http://sy.hahajie.cn

export PATH="$HOME/bin:$PATH"
来源：http://nl.lnxyls.cn

[R76] 使用临时文件
来源：http://ni.chemitech.net.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://il.huixinmuqiang.cn

[R77] 读取用户输入
来源：http://lt.newstarts.cn

read -rp "请输入: " ans
来源：http://ce.bookmarksfly.cn

[R78] 交互式菜单
来源：http://im.yuntaijiaju.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://oq.hahajie.cn

[R79] 解析命令行选项
来源：http://yb.jctech888.com.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://qa.huixinmuqiang.cn

[R80] 查看脚本执行耗时
来源：http://ma.bookmarksfly.cn

time ./run.sh
来源：http://je.521024.cn

================================================================================
来源：http://lk.gzmigu.cn

S. C / C++ 专题
来源：http://hn.yuntaijiaju.cn

================================================================================
来源：http://du.lnxyls.cn

[S01] C：Hello World
来源：http://pk.9csxet.cn

#include <stdio.h>
来源：http://nu.colortex.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://se.jctech888.com.cn

[S02] C：变量与格式化输出
来源：http://hm.shtwfgs.cn

int a = 10; printf("%d\n", a);
来源：http://wy.521024.cn

[S03] C：读入整数
来源：http://ir.yuntaijiaju.cn

int x; scanf("%d", &x);
来源：http://bw.wgjwhj.cn

[S04] C：字符串复制
来源：http://vg.shxzskj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://kf.nszjky.cn

[S05] C：字符串长度
来源：http://zb.shtwfgs.cn

strlen(s)
来源：http://kp.nszjky.cn

[S06] C：字符串比较
来源：http://qs.panjiajie.cn

strcmp(a, b) == 0
来源：http://ae.colortex.cn

[S07] C：数组遍历求和
来源：http://rn.newstarts.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://yy.szxytkj.cn

[S08] C：动态内存分配与释放
来源：http://ow.huixiangedu.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://zf.muxihuayi.cn

[S09] C：结构体定义与初始化
来源：http://sg.jctech888.com.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://iv.huixinmuqiang.cn

[S10] C：指针与解引用
来源：http://mk.lnxyls.cn

int *p = &a;  *p = 5;
来源：http://kn.colortex.cn

[S11] C：逐行读文件
来源：http://du.asd995.cn

FILE *f = fopen("a.txt", "r");
来源：http://br.haigaiapp.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ae.9csxet.cn

fclose(f);
来源：http://mw.jianghongdianzi.cn

[S12] C：写文件
来源：http://xz.shtwfgs.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wg.muxihuayi.cn

[S13] C：宏定义
来源：http://wf.colortex.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qm.hnjuh.cn

[S14] C：枚举
来源：http://ja.haigaiapp.cn

enum Color { RED, GREEN, BLUE };
来源：http://ji.nicolike.cn

[S15] C：类型转换
来源：http://ky.huixinmuqiang.cn

(double) a / b
来源：http://ab.yuexingan06.cn

[S16] C：位操作置位
来源：http://wi.szxytkj.cn

x |= (1 << 3);
来源：http://bd.newstarts.cn

[S17] C：安全拼接字符串
来源：http://ci.hnjuh.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://pc.hnjuh.cn

[S18] C：命令行参数
来源：http://co.lnxyls.cn

int main(int argc, char **argv)
来源：http://pw.huixiangedu.cn

[S19] C：快速排序
来源：http://ou.haigaiapp.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ve.szsharing.cn

[S20] C：二分查找
来源：http://kb.hnjuh.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ts.haigaiapp.cn

[S21] C：字符类别判断
来源：http://lh.szxytkj.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ni.yuntaijiaju.cn

[S22] C：字符串转数字
来源：http://gi.hnjuh.cn

atoi("42");  strtod("3.14", NULL);
来源：http://yj.521024.cn

[S23] C：随机数
来源：http://sk.bjjhwx.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://av.shtwfgs.cn

[S24] C：获取本地时间
来源：http://mv.hahajie.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://zj.bookmarksfly.cn

[S25] C：内存拷贝
来源：http://wf.colortex.cn

memcpy(dst, src, n);
来源：http://hy.lnxyls.cn

[S26] C：内存清零
来源：http://lc.haigaiapp.cn

memset(a, 0, sizeof a);
来源：http://sv.bjjhwx.cn

[S27] C：定义常量
来源：http://rk.asd995.cn

const double PI = 3.14159;
来源：http://am.hahajie.cn

[S28] C：静态变量
来源：http://rc.lnxyls.cn

static int counter = 0;
来源：http://db.9csxet.cn

[S29] C：变参函数
来源：http://db.gzmigu.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wt.9csxet.cn

[S30] C：头文件保护
来源：http://ah.bookmarksfly.cn

#ifndef X_H
来源：http://ks.nszjky.cn

#define X_H
来源：http://hb.bookmarksfly.cn

#endif
来源：http://px.yuntaijiaju.cn

[S31] C++：Hello World
来源：http://by.huixiangedu.cn

#include <iostream>
来源：http://da.newstarts.cn

int main() { std::cout << "Hello\n"; }
来源：http://zc.shxzukj.cn

[S32] C++：字符串
来源：http://ab.hnjuh.cn

std::string s = "hi";  s += "!";
来源：http://cv.nszjky.cn

[S33] C++：vector 增删
来源：http://uq.muxihuayi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://th.yuntaijiaju.cn

[S34] C++：遍历 vector
来源：http://kz.shxzukj.cn

for (auto &x : v) { std::cout << x; }
来源：http://hz.huanxung.cn

[S35] C++：map
来源：http://ex.szxytkj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://vt.wgjwhj.cn

[S36] C++：unordered_map
来源：http://vl.szxytkj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ht.haigaiapp.cn

[S37] C++：set
来源：http://ds.wgjwhj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://co.shxzskj.cn

[S38] C++：排序
来源：http://uk.colortex.cn

std::sort(v.begin(), v.end());
来源：http://hb.haigaiapp.cn

[S39] C++：自定义比较器排序
来源：http://op.panjiajie.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://pm.huixiangedu.cn

[S40] C++：查找元素
来源：http://bm.panjiajie.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://yr.haigaiapp.cn

[S41] C++：类与构造函数
来源：http://av.colortex.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ji.huanxung.cn

[S42] C++：继承与虚函数
来源：http://tf.asd995.cn

class B : public Base { public: void f() override {} };
来源：http://sx.huanxung.cn

[S43] C++：智能指针
来源：http://nk.521024.cn

auto p = std::make_unique<int>(5);
来源：http://jo.yuexingan06.cn

[S44] C++：引用传参
来源：http://bp.muxihuayi.cn

void inc(int &x) { ++x; }
来源：http://bu.huixinmuqiang.cn

[S45] C++：lambda
来源：http://px.shxzukj.cn

auto add = [](int a, int b) { return a + b; };
来源：http://fl.hahajie.cn

[S46] C++：函数模板
来源：http://ey.lnxyls.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ps.szsharing.cn

[S47] C++：结构化绑定遍历
来源：http://if.shxzskj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://cq.yuntaijiaju.cn

[S48] C++：逐行读文件
来源：http://fy.yuntaijiaju.cn

std::ifstream in("a.txt");  std::string line;
来源：http://nf.newstarts.cn

while (std::getline(in, line)) { }
来源：http://zr.panjiajie.cn

[S49] C++：写文件
来源：http://lh.szsharing.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://qt.panjiajie.cn

[S50] C++：格式化数字
来源：http://mf.jctech888.com.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wu.nicolike.cn

[S51] C++：显式类型转换
来源：http://ww.nicolike.cn

static_cast<double>(a) / b
来源：http://nn.panjiajie.cn

[S52] C++：const 与 noexcept
来源：http://pf.nszjky.cn

int size() const noexcept { return n_; }
来源：http://el.chemitech.net.cn

[S53] C++：移动语义
来源：http://zw.hahajie.cn

std::vector<int> w = std::move(v);
来源：http://ie.wgjwhj.cn

[S54] C++：异常处理
来源：http://ap.jianghongdianzi.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ut.shtwfgs.cn

[S55] C++：结构化绑定
来源：http://zj.huixiangedu.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://iw.wgjwhj.cn

[S56] C++：optional
来源：http://vp.newstarts.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mi.yuexingan06.cn

[S57] C++：编译期常量
来源：http://ml.jianghongdianzi.cn

constexpr int N = 10;
来源：http://de.haigaiapp.cn

[S58] C++：命名空间
来源：http://nc.newstarts.cn

namespace ns { int f() { return 1; } }
来源：http://od.shxzskj.cn

[S59] C++：静态断言
来源：http://hu.nszjky.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://sn.huixiangedu.cn

[S60] C++：遍历并删除元素
来源：http://zs.shxzukj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://wk.huixinmuqiang.cn

================================================================================
来源：http://mn.shxzskj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://wg.huixinmuqiang.cn

================================================================================
来源：http://be.shxzukj.cn

[T01] Kotlin：Hello World
来源：http://ui.newstarts.cn

println("Hello")
来源：http://it.huixiangedu.cn

[T02] Kotlin：变量
来源：http://co.wgjwhj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://in.shxzskj.cn

[T03] Kotlin：字符串模板
来源：http://kk.yuexingan06.cn

"值: $b"
来源：http://lf.521024.cn

[T04] Kotlin：空安全
来源：http://ri.yuexingan06.cn

val n: String? = null;  n?.length
来源：http://by.chemitech.net.cn

[T05] Kotlin：when 表达式
来源：http://ep.yuexingan06.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://tu.521024.cn

[T06] Kotlin：集合映射
来源：http://jk.huixiangedu.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ml.gzmigu.cn

[T07] Kotlin：集合过滤
来源：http://ko.haigaiapp.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://zu.muxihuayi.cn

[T08] Kotlin：数据类
来源：http://xo.muxihuayi.cn

data class User(val name: String, val age: Int)
来源：http://gd.521024.cn

[T09] Kotlin：扩展函数
来源：http://fa.yuexingan06.cn

fun String.exclaim() = this + "!"
来源：http://rd.nicolike.cn

[T10] Kotlin：默认参数
来源：http://rc.huixinmuqiang.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://yd.9csxet.cn

[T11] Kotlin：协程
来源：http://cw.shtwfgs.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://iv.jctech888.com.cn

[T12] Kotlin：解构声明
来源：http://wm.nszjky.cn

val (a, b) = Pair(1, 2)
来源：http://mn.nszjky.cn

[T13] Kotlin：只读 Map
来源：http://ek.wgjwhj.cn

val m = mapOf("a" to 1)
来源：http://ug.bjjhwx.cn

[T14] Kotlin：循环
来源：http://to.bookmarksfly.cn

for (i in 1..10) println(i)
来源：http://yl.hahajie.cn

[T15] Kotlin：接口
来源：http://sp.shtwfgs.cn

interface Shape { fun area(): Double }
来源：http://ge.szsharing.cn

[T16] Swift：Hello World
来源：http://bl.jctech888.com.cn

print("Hello")
来源：http://pa.chemitech.net.cn

[T17] Swift：变量与常量
来源：http://hp.hahajie.cn

var a = 1;  let b = 2
来源：http://mx.szxytkj.cn

[T18] Swift：字符串插值
来源：http://oc.gzmigu.cn

"值: \(b)"
来源：http://dc.shxzskj.cn

[T19] Swift：可选绑定
来源：http://ms.nszjky.cn

if let n = opt { print(n) }
来源：http://so.9csxet.cn

[T20] Swift：数组操作
来源：http://ck.muxihuayi.cn

var a = [1, 2, 3];  a.append(4)
来源：http://zi.chemitech.net.cn

[T21] Swift：遍历
来源：http://yy.gzmigu.cn

for x in a { print(x) }
来源：http://hz.newstarts.cn

[T22] Swift：字典
来源：http://cn.bjjhwx.cn

var d = ["a": 1];  d["b"] = 2
来源：http://su.hnjuh.cn

[T23] Swift：函数
来源：http://ns.nicolike.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://fm.yuexingan06.cn

[T24] Swift：闭包
来源：http://xi.szxytkj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ex.shxzskj.cn

[T25] Swift：结构体
来源：http://fs.9csxet.cn

struct P { var x: Int }
来源：http://hx.muxihuayi.cn

[T26] Swift：类与重写
来源：http://bd.chemitech.net.cn

class A: Base { override func f() {} }
来源：http://tt.wgjwhj.cn

[T27] Swift：错误处理
来源：http://nl.szsharing.cn

do { try f() } catch { print(error) }
来源：http://ac.bjjhwx.cn

[T28] Swift：枚举
来源：http://bm.hahajie.cn

enum Color { case red, green }
来源：http://mk.nszjky.cn

[T29] Swift：guard 提前返回
来源：http://oi.asd995.cn

guard let x = opt else { return }
来源：http://ij.muxihuayi.cn

[T30] Swift：协议
来源：http://cw.newstarts.cn

protocol Shape { func area() -> Double }
来源：http://os.muxihuayi.cn

[T31] Lua：Hello World
来源：http://ao.newstarts.cn

print("Hello")
来源：http://bl.chemitech.net.cn

[T32] Lua：局部变量
来源：http://bg.muxihuayi.cn

local a = 1
来源：http://vn.bjjhwx.cn

[T33] Lua：表（数组）
来源：http://cs.colortex.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://vp.szsharing.cn

[T34] Lua：遍历表
来源：http://bp.jianghongdianzi.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://hh.panjiajie.cn

[T35] Lua：字典表
来源：http://ib.huixiangedu.cn

local d = { a = 1 };  d.b = 2
来源：http://jz.521024.cn

[T36] Lua：函数
来源：http://zl.nszjky.cn

function add(a, b) return a + b end
来源：http://wy.shxzskj.cn

[T37] Lua：字符串拼接
来源：http://ak.shxzskj.cn

"a" .. "b"
来源：http://oi.yuexingan06.cn

[T38] Lua：条件
来源：http://ag.jctech888.com.cn

if x > 0 then print("正") end
来源：http://do.wgjwhj.cn

[T39] Lua：模式匹配
来源：http://hy.bookmarksfly.cn

string.find(s, "%d+")
来源：http://xg.haigaiapp.cn

[T40] Lua：元表
来源：http://ja.hahajie.cn

setmetatable({}, { __index = base })
来源：http://px.bjjhwx.cn

[T41] Perl：Hello World
来源：http://ka.bookmarksfly.cn

print "Hello\n";
来源：http://tp.gzmigu.cn

[T42] Perl：变量类型
来源：http://lh.huixiangedu.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://fz.shtwfgs.cn

[T43] Perl：字符串插值
来源：http://ba.gzmigu.cn

"值: $a"
来源：http://uq.shxzskj.cn

[T44] Perl：条件
来源：http://rz.521024.cn

if ($a > 0) { print "正"; }
来源：http://nr.haigaiapp.cn

[T45] Perl：数组遍历
来源：http://kx.hnjuh.cn

for my $x (@arr) { print $x; }
来源：http://dr.hahajie.cn

[T46] Perl：哈希操作
来源：http://et.shxzukj.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://xs.wgjwhj.cn

[T47] Perl：正则捕获
来源：http://qh.haigaiapp.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://qg.521024.cn

[T48] Perl：正则替换
来源：http://yj.yuexingan06.cn

$s =~ s/old/new/g;
来源：http://fx.panjiajie.cn

[T49] Perl：函数
来源：http://ce.bjjhwx.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ps.shxzukj.cn

[T50] Perl：逐行读文件
来源：http://wv.shtwfgs.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ch.hnjuh.cn

while (my $line = <$fh>) { print $line; }
来源：http://ht.nszjky.cn

[T51] Scala：Hello World
来源：http://oy.hahajie.cn

println("Hello")
来源：http://rr.521024.cn

[T52] Scala：变量
来源：http://nw.asd995.cn

val a = 1;  var b = 2
来源：http://lr.szsharing.cn

[T53] Scala：字符串插值
来源：http://eh.bookmarksfly.cn

s"值: $b"
来源：http://di.yuntaijiaju.cn

[T54] Scala：集合映射
来源：http://km.yuexingan06.cn

List(1, 2, 3).map(_ * 2)
来源：http://je.lnxyls.cn

[T55] Scala：集合过滤
来源：http://wy.szxytkj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ut.haigaiapp.cn

[T56] Scala：样例类
来源：http://uc.shtwfgs.cn

case class User(name: String, age: Int)
来源：http://xe.jctech888.com.cn

[T57] Scala：模式匹配
来源：http://xs.hahajie.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://mw.lnxyls.cn

[T58] Scala：函数定义
来源：http://ts.hnjuh.cn

def add(a: Int, b: Int): Int = a + b
来源：http://rw.521024.cn

[T59] Scala：循环
来源：http://vp.bookmarksfly.cn

for (i <- 1 to 10) println(i)
来源：http://ny.panjiajie.cn

[T60] Scala：折叠
来源：http://cq.colortex.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://im.muxihuayi.cn

================================================================================
来源：http://oc.szsharing.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://sz.asd995.cn

================================================================================
来源：http://sd.jctech888.com.cn

[U01] Py：创建虚拟环境
来源：http://mj.hahajie.cn

python -m venv .venv && source .venv/bin/activate
来源：http://xo.hahajie.cn

[U02] Py：导出 / 安装依赖
来源：http://bm.bjjhwx.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://td.nszjky.cn

[U03] Py：加载 .env 配置
来源：http://vs.bookmarksfly.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://cg.lnxyls.cn

[U04] Py：变量调试打印
来源：http://mm.521024.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ej.lnxyls.cn

[U05] Py：列表去重且保序
来源：http://tj.nszjky.cn

list(dict.fromkeys(arr))
来源：http://un.colortex.cn

[U06] Py：合并两个字典
来源：http://ce.shxzukj.cn

{**a, **b}
来源：http://wc.panjiajie.cn

[U07] Py：反转字典键值
来源：http://ff.huixinmuqiang.cn

{v: k for k, v in d.items()}
来源：http://xp.hahajie.cn

[U08] Py：展平二维列表
来源：http://yt.hahajie.cn

[y for x in nested for y in x]
来源：http://ud.jianghongdianzi.cn


<!-- 参考信息 -->