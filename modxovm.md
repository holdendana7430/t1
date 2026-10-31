代发 wailian999

openssl rand -hex 16
来源：http://yt.huixinmuqiang.cn

[R68] 计算文件校验值
来源：http://pb.jianghongdianzi.cn

sha256sum a.txt;  md5sum a.txt
来源：http://bx.huanxung.cn

[R69] 生成随机密码
来源：http://qw.shxzukj.cn

head -c 16 /dev/urandom | base64
来源：http://zh.yuexingan06.cn

[R70] 时间戳与互转
来源：http://zf.panjiajie.cn

date +%s;  date -d @1700000000
来源：http://dg.jctech888.com.cn

[R71] 日期格式化
来源：http://sp.nszjky.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ci.shxzukj.cn

[R72] 等待端口就绪
来源：http://hr.gzmigu.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://hn.shxzskj.cn

[R73] 分割大日志
来源：http://lx.asd995.cn

split -l 1000 big.log part_
来源：http://yg.panjiajie.cn

[R74] 批量重命名
来源：http://yk.asd995.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://vo.nszjky.cn

[R75] 导出环境变量
来源：http://ch.shxzukj.cn

export PATH="$HOME/bin:$PATH"
来源：http://vw.hahajie.cn

[R76] 使用临时文件
来源：http://ui.wgjwhj.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://un.521024.cn

[R77] 读取用户输入
来源：http://hv.shxzukj.cn

read -rp "请输入: " ans
来源：http://pm.newstarts.cn

[R78] 交互式菜单
来源：http://zj.shtwfgs.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ym.panjiajie.cn

[R79] 解析命令行选项
来源：http://zk.yuexingan06.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://hw.huixiangedu.cn

[R80] 查看脚本执行耗时
来源：http://bu.jianghongdianzi.cn

time ./run.sh
来源：http://dk.gzmigu.cn

================================================================================
来源：http://ob.gzmigu.cn

S. C / C++ 专题
来源：http://uw.huixiangedu.cn

================================================================================
来源：http://uf.jianghongdianzi.cn

[S01] C：Hello World
来源：http://yr.nszjky.cn

#include <stdio.h>
来源：http://pp.colortex.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ga.szxytkj.cn

[S02] C：变量与格式化输出
来源：http://pl.hnjuh.cn

int a = 10; printf("%d\n", a);
来源：http://nw.nszjky.cn

[S03] C：读入整数
来源：http://af.shxzskj.cn

int x; scanf("%d", &x);
来源：http://hd.huixiangedu.cn

[S04] C：字符串复制
来源：http://re.shxzukj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://vd.jctech888.com.cn

[S05] C：字符串长度
来源：http://hn.shxzukj.cn

strlen(s)
来源：http://vt.hnjuh.cn

[S06] C：字符串比较
来源：http://wc.muxihuayi.cn

strcmp(a, b) == 0
来源：http://sb.521024.cn

[S07] C：数组遍历求和
来源：http://ag.bookmarksfly.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://kr.yuntaijiaju.cn

[S08] C：动态内存分配与释放
来源：http://do.panjiajie.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://iv.huanxung.cn

[S09] C：结构体定义与初始化
来源：http://ae.chemitech.net.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://fs.lnxyls.cn

[S10] C：指针与解引用
来源：http://st.hnjuh.cn

int *p = &a;  *p = 5;
来源：http://jn.colortex.cn

[S11] C：逐行读文件
来源：http://ye.shxzskj.cn

FILE *f = fopen("a.txt", "r");
来源：http://xm.huanxung.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://nj.szxytkj.cn

fclose(f);
来源：http://bm.hahajie.cn

[S12] C：写文件
来源：http://rj.bookmarksfly.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xj.huixiangedu.cn

[S13] C：宏定义
来源：http://ud.bookmarksfly.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://qh.jctech888.com.cn

[S14] C：枚举
来源：http://fc.shxzukj.cn

enum Color { RED, GREEN, BLUE };
来源：http://kw.lnxyls.cn

[S15] C：类型转换
来源：http://hy.nicolike.cn

(double) a / b
来源：http://wm.521024.cn

[S16] C：位操作置位
来源：http://yr.chemitech.net.cn

x |= (1 << 3);
来源：http://gv.huanxung.cn

[S17] C：安全拼接字符串
来源：http://bb.shtwfgs.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://rj.panjiajie.cn

[S18] C：命令行参数
来源：http://zw.shtwfgs.cn

int main(int argc, char **argv)
来源：http://sb.lnxyls.cn

[S19] C：快速排序
来源：http://ln.bookmarksfly.cn

qsort(a, n, sizeof(int), cmp);
来源：http://zz.jianghongdianzi.cn

[S20] C：二分查找
来源：http://zt.bjjhwx.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://rq.muxihuayi.cn

[S21] C：字符类别判断
来源：http://ww.newstarts.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://oq.shxzukj.cn

[S22] C：字符串转数字
来源：http://rj.szxytkj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://we.chemitech.net.cn

[S23] C：随机数
来源：http://bu.shtwfgs.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ah.colortex.cn

[S24] C：获取本地时间
来源：http://st.newstarts.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ud.shxzukj.cn

[S25] C：内存拷贝
来源：http://kg.hnjuh.cn

memcpy(dst, src, n);
来源：http://hw.hnjuh.cn

[S26] C：内存清零
来源：http://rp.shxzskj.cn

memset(a, 0, sizeof a);
来源：http://gf.chemitech.net.cn

[S27] C：定义常量
来源：http://jx.shtwfgs.cn

const double PI = 3.14159;
来源：http://ca.gzmigu.cn

[S28] C：静态变量
来源：http://kw.jctech888.com.cn

static int counter = 0;
来源：http://vv.colortex.cn

[S29] C：变参函数
来源：http://vk.yuntaijiaju.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://tc.shxzskj.cn

[S30] C：头文件保护
来源：http://bs.yuexingan06.cn

#ifndef X_H
来源：http://ih.hahajie.cn

#define X_H
来源：http://em.yuntaijiaju.cn

#endif
来源：http://wm.chemitech.net.cn

[S31] C++：Hello World
来源：http://jq.shtwfgs.cn

#include <iostream>
来源：http://hy.yuntaijiaju.cn

int main() { std::cout << "Hello\n"; }
来源：http://mi.hahajie.cn

[S32] C++：字符串
来源：http://pd.shxzskj.cn

std::string s = "hi";  s += "!";
来源：http://zk.jctech888.com.cn

[S33] C++：vector 增删
来源：http://gb.bjjhwx.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://fb.szxytkj.cn

[S34] C++：遍历 vector
来源：http://bo.lnxyls.cn

for (auto &x : v) { std::cout << x; }
来源：http://et.szsharing.cn

[S35] C++：map
来源：http://lf.hnjuh.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://oq.wgjwhj.cn

[S36] C++：unordered_map
来源：http://vw.huixiangedu.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://un.asd995.cn

[S37] C++：set
来源：http://ld.gzmigu.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://fk.haigaiapp.cn

[S38] C++：排序
来源：http://iv.gzmigu.cn

std::sort(v.begin(), v.end());
来源：http://zh.chemitech.net.cn

[S39] C++：自定义比较器排序
来源：http://ij.yuexingan06.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://km.chemitech.net.cn

[S40] C++：查找元素
来源：http://hb.muxihuayi.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://bn.huixiangedu.cn

[S41] C++：类与构造函数
来源：http://vd.huixinmuqiang.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://tl.shxzskj.cn

[S42] C++：继承与虚函数
来源：http://rj.haigaiapp.cn

class B : public Base { public: void f() override {} };
来源：http://wt.yuntaijiaju.cn

[S43] C++：智能指针
来源：http://lz.huanxung.cn

auto p = std::make_unique<int>(5);
来源：http://el.shxzukj.cn

[S44] C++：引用传参
来源：http://tz.shxzskj.cn

void inc(int &x) { ++x; }
来源：http://ad.haigaiapp.cn

[S45] C++：lambda
来源：http://ni.bookmarksfly.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ok.huixinmuqiang.cn

[S46] C++：函数模板
来源：http://wp.yuexingan06.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://aj.bjjhwx.cn

[S47] C++：结构化绑定遍历
来源：http://ay.yuntaijiaju.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://bl.jctech888.com.cn

[S48] C++：逐行读文件
来源：http://qw.huixinmuqiang.cn

std::ifstream in("a.txt");  std::string line;
来源：http://sg.bookmarksfly.cn

while (std::getline(in, line)) { }
来源：http://nb.yuntaijiaju.cn

[S49] C++：写文件
来源：http://qm.szsharing.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ke.shxzukj.cn

[S50] C++：格式化数字
来源：http://ly.huixinmuqiang.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wt.chemitech.net.cn

[S51] C++：显式类型转换
来源：http://au.shxzskj.cn

static_cast<double>(a) / b
来源：http://xt.521024.cn

[S52] C++：const 与 noexcept
来源：http://rm.asd995.cn

int size() const noexcept { return n_; }
来源：http://pl.huixinmuqiang.cn

[S53] C++：移动语义
来源：http://nv.newstarts.cn

std::vector<int> w = std::move(v);
来源：http://zx.hnjuh.cn

[S54] C++：异常处理
来源：http://es.yuexingan06.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ps.shxzskj.cn

[S55] C++：结构化绑定
来源：http://vm.shxzukj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ws.9csxet.cn

[S56] C++：optional
来源：http://tv.szsharing.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mh.huixinmuqiang.cn

[S57] C++：编译期常量
来源：http://us.hahajie.cn

constexpr int N = 10;
来源：http://ll.yuexingan06.cn

[S58] C++：命名空间
来源：http://bb.bjjhwx.cn

namespace ns { int f() { return 1; } }
来源：http://ys.yuexingan06.cn

[S59] C++：静态断言
来源：http://kj.lnxyls.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://cb.shtwfgs.cn

[S60] C++：遍历并删除元素
来源：http://ny.bookmarksfly.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://rw.bjjhwx.cn

================================================================================
来源：http://qt.lnxyls.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://pd.9csxet.cn

================================================================================
来源：http://ew.huixiangedu.cn

[T01] Kotlin：Hello World
来源：http://kr.szsharing.cn

println("Hello")
来源：http://wt.asd995.cn

[T02] Kotlin：变量
来源：http://rd.huanxung.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://mu.huixiangedu.cn

[T03] Kotlin：字符串模板
来源：http://wq.521024.cn

"值: $b"
来源：http://tg.9csxet.cn

[T04] Kotlin：空安全
来源：http://xf.colortex.cn

val n: String? = null;  n?.length
来源：http://ls.colortex.cn

[T05] Kotlin：when 表达式
来源：http://pr.muxihuayi.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ib.huanxung.cn

[T06] Kotlin：集合映射
来源：http://wp.yuntaijiaju.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://fo.huixinmuqiang.cn

[T07] Kotlin：集合过滤
来源：http://om.shxzukj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://dr.shxzukj.cn

[T08] Kotlin：数据类
来源：http://gu.yuntaijiaju.cn

data class User(val name: String, val age: Int)
来源：http://qz.panjiajie.cn

[T09] Kotlin：扩展函数
来源：http://va.nicolike.cn

fun String.exclaim() = this + "!"
来源：http://tb.yuexingan06.cn

[T10] Kotlin：默认参数
来源：http://yw.newstarts.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ra.panjiajie.cn

[T11] Kotlin：协程
来源：http://fy.jctech888.com.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://qb.shxzskj.cn

[T12] Kotlin：解构声明
来源：http://cd.hahajie.cn

val (a, b) = Pair(1, 2)
来源：http://gh.szxytkj.cn

[T13] Kotlin：只读 Map
来源：http://yx.shxzukj.cn

val m = mapOf("a" to 1)
来源：http://mv.lnxyls.cn

[T14] Kotlin：循环
来源：http://iw.nicolike.cn

for (i in 1..10) println(i)
来源：http://ax.wgjwhj.cn

[T15] Kotlin：接口
来源：http://jz.huixiangedu.cn

interface Shape { fun area(): Double }
来源：http://ik.wgjwhj.cn

[T16] Swift：Hello World
来源：http://zj.shxzukj.cn

print("Hello")
来源：http://te.colortex.cn

[T17] Swift：变量与常量
来源：http://zz.huixiangedu.cn

var a = 1;  let b = 2
来源：http://fo.muxihuayi.cn

[T18] Swift：字符串插值
来源：http://vf.colortex.cn

"值: \(b)"
来源：http://ae.nszjky.cn

[T19] Swift：可选绑定
来源：http://px.shtwfgs.cn

if let n = opt { print(n) }
来源：http://hj.jianghongdianzi.cn

[T20] Swift：数组操作
来源：http://vs.szsharing.cn

var a = [1, 2, 3];  a.append(4)
来源：http://yz.shxzskj.cn

[T21] Swift：遍历
来源：http://vm.huanxung.cn

for x in a { print(x) }
来源：http://jb.asd995.cn

[T22] Swift：字典
来源：http://fz.521024.cn

var d = ["a": 1];  d["b"] = 2
来源：http://fe.lnxyls.cn

[T23] Swift：函数
来源：http://jj.9csxet.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://av.yuexingan06.cn

[T24] Swift：闭包
来源：http://qs.huanxung.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://fu.colortex.cn

[T25] Swift：结构体
来源：http://xy.9csxet.cn

struct P { var x: Int }
来源：http://lv.wgjwhj.cn

[T26] Swift：类与重写
来源：http://vb.hahajie.cn

class A: Base { override func f() {} }
来源：http://ux.yuntaijiaju.cn

[T27] Swift：错误处理
来源：http://qy.wgjwhj.cn

do { try f() } catch { print(error) }
来源：http://gp.9csxet.cn

[T28] Swift：枚举
来源：http://cm.colortex.cn

enum Color { case red, green }
来源：http://sc.wgjwhj.cn

[T29] Swift：guard 提前返回
来源：http://nw.hnjuh.cn

guard let x = opt else { return }
来源：http://su.jianghongdianzi.cn

[T30] Swift：协议
来源：http://ke.nszjky.cn

protocol Shape { func area() -> Double }
来源：http://xt.huixiangedu.cn

[T31] Lua：Hello World
来源：http://qm.521024.cn

print("Hello")
来源：http://ai.nicolike.cn

[T32] Lua：局部变量
来源：http://bv.huixinmuqiang.cn

local a = 1
来源：http://el.jianghongdianzi.cn

[T33] Lua：表（数组）
来源：http://ho.nszjky.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://cw.gzmigu.cn

[T34] Lua：遍历表
来源：http://jh.bjjhwx.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://io.521024.cn

[T35] Lua：字典表
来源：http://fw.szsharing.cn

local d = { a = 1 };  d.b = 2
来源：http://ma.jianghongdianzi.cn

[T36] Lua：函数
来源：http://fz.muxihuayi.cn

function add(a, b) return a + b end
来源：http://ib.huixinmuqiang.cn

[T37] Lua：字符串拼接
来源：http://oe.shtwfgs.cn

"a" .. "b"
来源：http://zc.huixiangedu.cn

[T38] Lua：条件
来源：http://wz.muxihuayi.cn

if x > 0 then print("正") end
来源：http://tq.newstarts.cn

[T39] Lua：模式匹配
来源：http://zz.nicolike.cn

string.find(s, "%d+")
来源：http://oh.chemitech.net.cn

[T40] Lua：元表
来源：http://sd.wgjwhj.cn

setmetatable({}, { __index = base })
来源：http://zn.huixinmuqiang.cn

[T41] Perl：Hello World
来源：http://xc.bookmarksfly.cn

print "Hello\n";
来源：http://hx.asd995.cn

[T42] Perl：变量类型
来源：http://zr.9csxet.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ai.muxihuayi.cn

[T43] Perl：字符串插值
来源：http://mk.huixinmuqiang.cn

"值: $a"
来源：http://wv.521024.cn

[T44] Perl：条件
来源：http://cd.jianghongdianzi.cn

if ($a > 0) { print "正"; }
来源：http://hv.nicolike.cn

[T45] Perl：数组遍历
来源：http://bx.huanxung.cn

for my $x (@arr) { print $x; }
来源：http://lg.szxytkj.cn

[T46] Perl：哈希操作
来源：http://ha.haigaiapp.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://on.nicolike.cn

[T47] Perl：正则捕获
来源：http://se.huixiangedu.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://pq.panjiajie.cn

[T48] Perl：正则替换
来源：http://zl.huixinmuqiang.cn

$s =~ s/old/new/g;
来源：http://ky.shxzukj.cn

[T49] Perl：函数
来源：http://ob.shtwfgs.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://jr.yuexingan06.cn

[T50] Perl：逐行读文件
来源：http://os.hnjuh.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://mv.jctech888.com.cn

while (my $line = <$fh>) { print $line; }
来源：http://lf.muxihuayi.cn

[T51] Scala：Hello World
来源：http://iq.colortex.cn

println("Hello")
来源：http://hd.colortex.cn

[T52] Scala：变量
来源：http://df.521024.cn

val a = 1;  var b = 2
来源：http://gj.nicolike.cn

[T53] Scala：字符串插值
来源：http://cb.huixinmuqiang.cn

s"值: $b"
来源：http://gh.haigaiapp.cn

[T54] Scala：集合映射
来源：http://oe.bookmarksfly.cn

List(1, 2, 3).map(_ * 2)
来源：http://dm.asd995.cn

[T55] Scala：集合过滤
来源：http://dj.nicolike.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ek.chemitech.net.cn

[T56] Scala：样例类
来源：http://vs.colortex.cn

case class User(name: String, age: Int)
来源：http://to.muxihuayi.cn

[T57] Scala：模式匹配
来源：http://sh.shxzskj.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ba.nszjky.cn

[T58] Scala：函数定义
来源：http://xq.hnjuh.cn

def add(a: Int, b: Int): Int = a + b
来源：http://tk.yuntaijiaju.cn

[T59] Scala：循环
来源：http://qn.521024.cn

for (i <- 1 to 10) println(i)
来源：http://pj.shtwfgs.cn

[T60] Scala：折叠
来源：http://zk.jianghongdianzi.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://uz.shxzukj.cn

================================================================================
来源：http://sr.panjiajie.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ib.muxihuayi.cn

================================================================================
来源：http://ae.hahajie.cn

[U01] Py：创建虚拟环境
来源：http://om.hahajie.cn

python -m venv .venv && source .venv/bin/activate
来源：http://hm.jctech888.com.cn

[U02] Py：导出 / 安装依赖
来源：http://kg.bookmarksfly.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://da.asd995.cn

[U03] Py：加载 .env 配置
来源：http://cm.muxihuayi.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://rz.nszjky.cn

[U04] Py：变量调试打印
来源：http://ee.nszjky.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ec.huixinmuqiang.cn

[U05] Py：列表去重且保序
来源：http://os.newstarts.cn

list(dict.fromkeys(arr))
来源：http://ww.jianghongdianzi.cn

[U06] Py：合并两个字典
来源：http://jw.haigaiapp.cn

{**a, **b}
来源：http://fv.9csxet.cn

[U07] Py：反转字典键值
来源：http://vp.bookmarksfly.cn

{v: k for k, v in d.items()}
来源：http://wt.shtwfgs.cn

[U08] Py：展平二维列表
来源：http://bt.szsharing.cn

[y for x in nested for y in x]
来源：http://ju.jianghongdianzi.cn


<!-- 参考信息 -->