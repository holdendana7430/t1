代发 wailian999

openssl rand -hex 16
来源：http://nm.521024.cn

[R68] 计算文件校验值
来源：http://kn.9csxet.cn

sha256sum a.txt;  md5sum a.txt
来源：http://xe.szsharing.cn

[R69] 生成随机密码
来源：http://vl.yuntaijiaju.cn

head -c 16 /dev/urandom | base64
来源：http://ix.hahajie.cn

[R70] 时间戳与互转
来源：http://vp.jianghongdianzi.cn

date +%s;  date -d @1700000000
来源：http://po.shxzukj.cn

[R71] 日期格式化
来源：http://tx.521024.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://fl.lnxyls.cn

[R72] 等待端口就绪
来源：http://lr.hahajie.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://cp.gzmigu.cn

[R73] 分割大日志
来源：http://zq.szsharing.cn

split -l 1000 big.log part_
来源：http://hr.yuntaijiaju.cn

[R74] 批量重命名
来源：http://si.haigaiapp.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mo.bjjhwx.cn

[R75] 导出环境变量
来源：http://rz.shxzukj.cn

export PATH="$HOME/bin:$PATH"
来源：http://fn.shxzukj.cn

[R76] 使用临时文件
来源：http://lj.wgjwhj.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://gt.hnjuh.cn

[R77] 读取用户输入
来源：http://au.shxzskj.cn

read -rp "请输入: " ans
来源：http://kv.newstarts.cn

[R78] 交互式菜单
来源：http://rb.yuexingan06.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://xo.colortex.cn

[R79] 解析命令行选项
来源：http://bf.jianghongdianzi.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ry.colortex.cn

[R80] 查看脚本执行耗时
来源：http://jn.shxzskj.cn

time ./run.sh
来源：http://hk.szsharing.cn

================================================================================
来源：http://gt.nicolike.cn

S. C / C++ 专题
来源：http://hp.szxytkj.cn

================================================================================
来源：http://pb.jctech888.com.cn

[S01] C：Hello World
来源：http://ae.jctech888.com.cn

#include <stdio.h>
来源：http://mn.bookmarksfly.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://cd.shxzukj.cn

[S02] C：变量与格式化输出
来源：http://qi.gzmigu.cn

int a = 10; printf("%d\n", a);
来源：http://hx.chemitech.net.cn

[S03] C：读入整数
来源：http://ct.hahajie.cn

int x; scanf("%d", &x);
来源：http://fh.huixiangedu.cn

[S04] C：字符串复制
来源：http://qw.jianghongdianzi.cn

char dst[32]; strcpy(dst, "hi");
来源：http://wa.chemitech.net.cn

[S05] C：字符串长度
来源：http://os.panjiajie.cn

strlen(s)
来源：http://gv.nszjky.cn

[S06] C：字符串比较
来源：http://hu.521024.cn

strcmp(a, b) == 0
来源：http://nk.hnjuh.cn

[S07] C：数组遍历求和
来源：http://wh.shtwfgs.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ra.bjjhwx.cn

[S08] C：动态内存分配与释放
来源：http://sf.yuexingan06.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://yb.asd995.cn

[S09] C：结构体定义与初始化
来源：http://cl.521024.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://rr.huixinmuqiang.cn

[S10] C：指针与解引用
来源：http://km.9csxet.cn

int *p = &a;  *p = 5;
来源：http://gl.wgjwhj.cn

[S11] C：逐行读文件
来源：http://je.huanxung.cn

FILE *f = fopen("a.txt", "r");
来源：http://zz.nszjky.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://zx.hahajie.cn

fclose(f);
来源：http://rx.panjiajie.cn

[S12] C：写文件
来源：http://ej.shtwfgs.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://jc.hahajie.cn

[S13] C：宏定义
来源：http://dz.muxihuayi.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://vz.shxzukj.cn

[S14] C：枚举
来源：http://bz.shxzskj.cn

enum Color { RED, GREEN, BLUE };
来源：http://wr.muxihuayi.cn

[S15] C：类型转换
来源：http://ds.newstarts.cn

(double) a / b
来源：http://co.hahajie.cn

[S16] C：位操作置位
来源：http://ko.hnjuh.cn

x |= (1 << 3);
来源：http://we.shxzskj.cn

[S17] C：安全拼接字符串
来源：http://ei.asd995.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://vn.hahajie.cn

[S18] C：命令行参数
来源：http://at.muxihuayi.cn

int main(int argc, char **argv)
来源：http://ka.newstarts.cn

[S19] C：快速排序
来源：http://pw.jctech888.com.cn

qsort(a, n, sizeof(int), cmp);
来源：http://nq.shxzukj.cn

[S20] C：二分查找
来源：http://gc.hnjuh.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://cn.newstarts.cn

[S21] C：字符类别判断
来源：http://cy.521024.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://kn.shxzukj.cn

[S22] C：字符串转数字
来源：http://in.hnjuh.cn

atoi("42");  strtod("3.14", NULL);
来源：http://xw.haigaiapp.cn

[S23] C：随机数
来源：http://ys.colortex.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://hk.asd995.cn

[S24] C：获取本地时间
来源：http://ue.muxihuayi.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ef.panjiajie.cn

[S25] C：内存拷贝
来源：http://eo.bookmarksfly.cn

memcpy(dst, src, n);
来源：http://js.jianghongdianzi.cn

[S26] C：内存清零
来源：http://si.asd995.cn

memset(a, 0, sizeof a);
来源：http://by.gzmigu.cn

[S27] C：定义常量
来源：http://lu.szsharing.cn

const double PI = 3.14159;
来源：http://bi.huixinmuqiang.cn

[S28] C：静态变量
来源：http://lm.muxihuayi.cn

static int counter = 0;
来源：http://wk.asd995.cn

[S29] C：变参函数
来源：http://mm.bjjhwx.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ns.huixiangedu.cn

[S30] C：头文件保护
来源：http://nr.shxzukj.cn

#ifndef X_H
来源：http://jb.521024.cn

#define X_H
来源：http://ww.newstarts.cn

#endif
来源：http://rl.nicolike.cn

[S31] C++：Hello World
来源：http://lf.bjjhwx.cn

#include <iostream>
来源：http://ab.bjjhwx.cn

int main() { std::cout << "Hello\n"; }
来源：http://qf.shxzukj.cn

[S32] C++：字符串
来源：http://dm.bjjhwx.cn

std::string s = "hi";  s += "!";
来源：http://mi.muxihuayi.cn

[S33] C++：vector 增删
来源：http://si.chemitech.net.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://sm.shtwfgs.cn

[S34] C++：遍历 vector
来源：http://ns.newstarts.cn

for (auto &x : v) { std::cout << x; }
来源：http://op.bjjhwx.cn

[S35] C++：map
来源：http://sm.panjiajie.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://nq.nicolike.cn

[S36] C++：unordered_map
来源：http://rf.szsharing.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://em.szxytkj.cn

[S37] C++：set
来源：http://aw.hahajie.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://xi.szsharing.cn

[S38] C++：排序
来源：http://ug.newstarts.cn

std::sort(v.begin(), v.end());
来源：http://ee.newstarts.cn

[S39] C++：自定义比较器排序
来源：http://xu.nicolike.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://jb.szxytkj.cn

[S40] C++：查找元素
来源：http://tl.nszjky.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ge.yuntaijiaju.cn

[S41] C++：类与构造函数
来源：http://tk.panjiajie.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://xx.lnxyls.cn

[S42] C++：继承与虚函数
来源：http://so.panjiajie.cn

class B : public Base { public: void f() override {} };
来源：http://wz.521024.cn

[S43] C++：智能指针
来源：http://mt.hahajie.cn

auto p = std::make_unique<int>(5);
来源：http://au.huixiangedu.cn

[S44] C++：引用传参
来源：http://xc.nicolike.cn

void inc(int &x) { ++x; }
来源：http://rp.asd995.cn

[S45] C++：lambda
来源：http://yp.yuexingan06.cn

auto add = [](int a, int b) { return a + b; };
来源：http://tj.yuntaijiaju.cn

[S46] C++：函数模板
来源：http://qq.chemitech.net.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://zt.gzmigu.cn

[S47] C++：结构化绑定遍历
来源：http://xr.bookmarksfly.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://re.shxzskj.cn

[S48] C++：逐行读文件
来源：http://kw.colortex.cn

std::ifstream in("a.txt");  std::string line;
来源：http://gv.chemitech.net.cn

while (std::getline(in, line)) { }
来源：http://oq.jianghongdianzi.cn

[S49] C++：写文件
来源：http://de.shxzukj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://km.shxzukj.cn

[S50] C++：格式化数字
来源：http://jl.nszjky.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://dy.nicolike.cn

[S51] C++：显式类型转换
来源：http://lf.shxzukj.cn

static_cast<double>(a) / b
来源：http://rm.colortex.cn

[S52] C++：const 与 noexcept
来源：http://bx.lnxyls.cn

int size() const noexcept { return n_; }
来源：http://jn.colortex.cn

[S53] C++：移动语义
来源：http://oy.gzmigu.cn

std::vector<int> w = std::move(v);
来源：http://up.nicolike.cn

[S54] C++：异常处理
来源：http://xd.chemitech.net.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://xw.yuexingan06.cn

[S55] C++：结构化绑定
来源：http://zz.shxzskj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ab.asd995.cn

[S56] C++：optional
来源：http://ns.huixinmuqiang.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://bm.shxzukj.cn

[S57] C++：编译期常量
来源：http://jt.newstarts.cn

constexpr int N = 10;
来源：http://bn.szsharing.cn

[S58] C++：命名空间
来源：http://wt.newstarts.cn

namespace ns { int f() { return 1; } }
来源：http://rj.521024.cn

[S59] C++：静态断言
来源：http://ht.wgjwhj.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://pi.yuexingan06.cn

[S60] C++：遍历并删除元素
来源：http://be.9csxet.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://eb.nszjky.cn

================================================================================
来源：http://xp.asd995.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ve.huixiangedu.cn

================================================================================
来源：http://ce.shxzskj.cn

[T01] Kotlin：Hello World
来源：http://or.asd995.cn

println("Hello")
来源：http://ra.panjiajie.cn

[T02] Kotlin：变量
来源：http://yo.nszjky.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://bk.huanxung.cn

[T03] Kotlin：字符串模板
来源：http://rz.hahajie.cn

"值: $b"
来源：http://oj.yuntaijiaju.cn

[T04] Kotlin：空安全
来源：http://zr.huanxung.cn

val n: String? = null;  n?.length
来源：http://xv.colortex.cn

[T05] Kotlin：when 表达式
来源：http://bl.szxytkj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://iw.gzmigu.cn

[T06] Kotlin：集合映射
来源：http://wb.nicolike.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://uy.yuntaijiaju.cn

[T07] Kotlin：集合过滤
来源：http://rv.wgjwhj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://pn.huixiangedu.cn

[T08] Kotlin：数据类
来源：http://nv.521024.cn

data class User(val name: String, val age: Int)
来源：http://px.jianghongdianzi.cn

[T09] Kotlin：扩展函数
来源：http://gx.huixiangedu.cn

fun String.exclaim() = this + "!"
来源：http://io.huixiangedu.cn

[T10] Kotlin：默认参数
来源：http://xb.nicolike.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://gj.asd995.cn

[T11] Kotlin：协程
来源：http://um.wgjwhj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ti.bjjhwx.cn

[T12] Kotlin：解构声明
来源：http://gc.yuntaijiaju.cn

val (a, b) = Pair(1, 2)
来源：http://yy.521024.cn

[T13] Kotlin：只读 Map
来源：http://rg.jctech888.com.cn

val m = mapOf("a" to 1)
来源：http://tu.shxzskj.cn

[T14] Kotlin：循环
来源：http://nz.shxzskj.cn

for (i in 1..10) println(i)
来源：http://zl.shxzskj.cn

[T15] Kotlin：接口
来源：http://el.asd995.cn

interface Shape { fun area(): Double }
来源：http://tj.newstarts.cn

[T16] Swift：Hello World
来源：http://pd.jianghongdianzi.cn

print("Hello")
来源：http://py.jctech888.com.cn

[T17] Swift：变量与常量
来源：http://jl.hnjuh.cn

var a = 1;  let b = 2
来源：http://yp.shxzukj.cn

[T18] Swift：字符串插值
来源：http://pt.bookmarksfly.cn

"值: \(b)"
来源：http://zf.hahajie.cn

[T19] Swift：可选绑定
来源：http://rb.gzmigu.cn

if let n = opt { print(n) }
来源：http://eq.bjjhwx.cn

[T20] Swift：数组操作
来源：http://th.hnjuh.cn

var a = [1, 2, 3];  a.append(4)
来源：http://sv.yuexingan06.cn

[T21] Swift：遍历
来源：http://le.huixiangedu.cn

for x in a { print(x) }
来源：http://td.jianghongdianzi.cn

[T22] Swift：字典
来源：http://jr.gzmigu.cn

var d = ["a": 1];  d["b"] = 2
来源：http://hk.9csxet.cn

[T23] Swift：函数
来源：http://ee.jctech888.com.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://to.szsharing.cn

[T24] Swift：闭包
来源：http://jf.wgjwhj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://yh.9csxet.cn

[T25] Swift：结构体
来源：http://em.asd995.cn

struct P { var x: Int }
来源：http://js.huanxung.cn

[T26] Swift：类与重写
来源：http://tq.yuexingan06.cn

class A: Base { override func f() {} }
来源：http://io.yuntaijiaju.cn

[T27] Swift：错误处理
来源：http://sr.gzmigu.cn

do { try f() } catch { print(error) }
来源：http://cs.gzmigu.cn

[T28] Swift：枚举
来源：http://ud.bookmarksfly.cn

enum Color { case red, green }
来源：http://yp.wgjwhj.cn

[T29] Swift：guard 提前返回
来源：http://te.panjiajie.cn

guard let x = opt else { return }
来源：http://vd.szsharing.cn

[T30] Swift：协议
来源：http://qi.jianghongdianzi.cn

protocol Shape { func area() -> Double }
来源：http://qe.521024.cn

[T31] Lua：Hello World
来源：http://ps.chemitech.net.cn

print("Hello")
来源：http://aw.huixiangedu.cn

[T32] Lua：局部变量
来源：http://zy.muxihuayi.cn

local a = 1
来源：http://tu.jianghongdianzi.cn

[T33] Lua：表（数组）
来源：http://jt.nicolike.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ie.bjjhwx.cn

[T34] Lua：遍历表
来源：http://gy.muxihuayi.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ws.muxihuayi.cn

[T35] Lua：字典表
来源：http://tr.huixinmuqiang.cn

local d = { a = 1 };  d.b = 2
来源：http://sr.shxzskj.cn

[T36] Lua：函数
来源：http://lg.lnxyls.cn

function add(a, b) return a + b end
来源：http://dw.wgjwhj.cn

[T37] Lua：字符串拼接
来源：http://iv.gzmigu.cn

"a" .. "b"
来源：http://lt.nicolike.cn

[T38] Lua：条件
来源：http://qa.nszjky.cn

if x > 0 then print("正") end
来源：http://rm.bjjhwx.cn

[T39] Lua：模式匹配
来源：http://wn.shxzskj.cn

string.find(s, "%d+")
来源：http://ls.521024.cn

[T40] Lua：元表
来源：http://ia.jianghongdianzi.cn

setmetatable({}, { __index = base })
来源：http://mw.wgjwhj.cn

[T41] Perl：Hello World
来源：http://tl.nszjky.cn

print "Hello\n";
来源：http://up.gzmigu.cn

[T42] Perl：变量类型
来源：http://jz.bjjhwx.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://os.szxytkj.cn

[T43] Perl：字符串插值
来源：http://gq.521024.cn

"值: $a"
来源：http://wr.jctech888.com.cn

[T44] Perl：条件
来源：http://sn.szsharing.cn

if ($a > 0) { print "正"; }
来源：http://rs.hnjuh.cn

[T45] Perl：数组遍历
来源：http://ww.lnxyls.cn

for my $x (@arr) { print $x; }
来源：http://hb.yuexingan06.cn

[T46] Perl：哈希操作
来源：http://vn.jctech888.com.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://pp.huixinmuqiang.cn

[T47] Perl：正则捕获
来源：http://ag.hnjuh.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://zb.huanxung.cn

[T48] Perl：正则替换
来源：http://gb.521024.cn

$s =~ s/old/new/g;
来源：http://kt.hahajie.cn

[T49] Perl：函数
来源：http://hk.muxihuayi.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://pg.colortex.cn

[T50] Perl：逐行读文件
来源：http://ma.hnjuh.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://rx.shtwfgs.cn

while (my $line = <$fh>) { print $line; }
来源：http://xh.shtwfgs.cn

[T51] Scala：Hello World
来源：http://yu.huanxung.cn

println("Hello")
来源：http://bf.521024.cn

[T52] Scala：变量
来源：http://ot.gzmigu.cn

val a = 1;  var b = 2
来源：http://gv.jianghongdianzi.cn

[T53] Scala：字符串插值
来源：http://lw.newstarts.cn

s"值: $b"
来源：http://ak.panjiajie.cn

[T54] Scala：集合映射
来源：http://aq.muxihuayi.cn

List(1, 2, 3).map(_ * 2)
来源：http://mg.bjjhwx.cn

[T55] Scala：集合过滤
来源：http://jq.panjiajie.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ei.szsharing.cn

[T56] Scala：样例类
来源：http://zx.lnxyls.cn

case class User(name: String, age: Int)
来源：http://qt.asd995.cn

[T57] Scala：模式匹配
来源：http://zh.szsharing.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://tk.shxzukj.cn

[T58] Scala：函数定义
来源：http://aw.shtwfgs.cn

def add(a: Int, b: Int): Int = a + b
来源：http://qg.yuexingan06.cn

[T59] Scala：循环
来源：http://cp.521024.cn

for (i <- 1 to 10) println(i)
来源：http://xs.haigaiapp.cn

[T60] Scala：折叠
来源：http://kf.huanxung.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://sg.huixiangedu.cn

================================================================================
来源：http://dh.panjiajie.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://fd.nicolike.cn

================================================================================
来源：http://ck.nicolike.cn

[U01] Py：创建虚拟环境
来源：http://ow.shtwfgs.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ww.wgjwhj.cn

[U02] Py：导出 / 安装依赖
来源：http://nb.9csxet.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://vk.nicolike.cn

[U03] Py：加载 .env 配置
来源：http://pl.huixinmuqiang.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://gm.shtwfgs.cn

[U04] Py：变量调试打印
来源：http://rv.9csxet.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://hg.nszjky.cn

[U05] Py：列表去重且保序
来源：http://is.nszjky.cn

list(dict.fromkeys(arr))
来源：http://ff.chemitech.net.cn

[U06] Py：合并两个字典
来源：http://kd.hnjuh.cn

{**a, **b}
来源：http://lk.gzmigu.cn

[U07] Py：反转字典键值
来源：http://ey.bookmarksfly.cn

{v: k for k, v in d.items()}
来源：http://gq.shxzskj.cn

[U08] Py：展平二维列表
来源：http://yx.lnxyls.cn

[y for x in nested for y in x]
来源：http://pu.szsharing.cn


<!-- 参考信息 -->