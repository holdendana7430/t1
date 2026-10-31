代发 wailian999

openssl rand -hex 16
来源：http://lq.shtwfgs.cn

[R68] 计算文件校验值
来源：http://qp.hahajie.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ml.huixiangedu.cn

[R69] 生成随机密码
来源：http://vz.szxytkj.cn

head -c 16 /dev/urandom | base64
来源：http://jg.521024.cn

[R70] 时间戳与互转
来源：http://fa.wgjwhj.cn

date +%s;  date -d @1700000000
来源：http://df.hnjuh.cn

[R71] 日期格式化
来源：http://zb.huixiangedu.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://vi.nszjky.cn

[R72] 等待端口就绪
来源：http://vh.bjjhwx.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://dj.chemitech.net.cn

[R73] 分割大日志
来源：http://sa.lnxyls.cn

split -l 1000 big.log part_
来源：http://bl.yuntaijiaju.cn

[R74] 批量重命名
来源：http://pw.huanxung.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hy.asd995.cn

[R75] 导出环境变量
来源：http://vp.shxzukj.cn

export PATH="$HOME/bin:$PATH"
来源：http://fy.nicolike.cn

[R76] 使用临时文件
来源：http://tk.shxzukj.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://dh.yuntaijiaju.cn

[R77] 读取用户输入
来源：http://gt.chemitech.net.cn

read -rp "请输入: " ans
来源：http://hr.hnjuh.cn

[R78] 交互式菜单
来源：http://rp.shxzskj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ys.huanxung.cn

[R79] 解析命令行选项
来源：http://mp.lnxyls.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://yf.shtwfgs.cn

[R80] 查看脚本执行耗时
来源：http://ul.yuntaijiaju.cn

time ./run.sh
来源：http://mm.jctech888.com.cn

================================================================================
来源：http://el.panjiajie.cn

S. C / C++ 专题
来源：http://tc.shxzukj.cn

================================================================================
来源：http://gh.szxytkj.cn

[S01] C：Hello World
来源：http://xa.haigaiapp.cn

#include <stdio.h>
来源：http://op.hahajie.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://og.nszjky.cn

[S02] C：变量与格式化输出
来源：http://zh.lnxyls.cn

int a = 10; printf("%d\n", a);
来源：http://ql.bookmarksfly.cn

[S03] C：读入整数
来源：http://ml.chemitech.net.cn

int x; scanf("%d", &x);
来源：http://ru.521024.cn

[S04] C：字符串复制
来源：http://yl.bjjhwx.cn

char dst[32]; strcpy(dst, "hi");
来源：http://kf.521024.cn

[S05] C：字符串长度
来源：http://te.9csxet.cn

strlen(s)
来源：http://hm.huixinmuqiang.cn

[S06] C：字符串比较
来源：http://ik.szxytkj.cn

strcmp(a, b) == 0
来源：http://ax.muxihuayi.cn

[S07] C：数组遍历求和
来源：http://um.asd995.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://tf.bookmarksfly.cn

[S08] C：动态内存分配与释放
来源：http://hd.shtwfgs.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://dw.haigaiapp.cn

[S09] C：结构体定义与初始化
来源：http://wt.colortex.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://cq.jianghongdianzi.cn

[S10] C：指针与解引用
来源：http://sy.nicolike.cn

int *p = &a;  *p = 5;
来源：http://jg.wgjwhj.cn

[S11] C：逐行读文件
来源：http://ne.huanxung.cn

FILE *f = fopen("a.txt", "r");
来源：http://ud.9csxet.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://bu.bookmarksfly.cn

fclose(f);
来源：http://ny.nszjky.cn

[S12] C：写文件
来源：http://lr.9csxet.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://sm.shtwfgs.cn

[S13] C：宏定义
来源：http://dy.shxzskj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://vr.newstarts.cn

[S14] C：枚举
来源：http://tn.hahajie.cn

enum Color { RED, GREEN, BLUE };
来源：http://ul.yuntaijiaju.cn

[S15] C：类型转换
来源：http://bb.521024.cn

(double) a / b
来源：http://gk.haigaiapp.cn

[S16] C：位操作置位
来源：http://fm.haigaiapp.cn

x |= (1 << 3);
来源：http://ti.nszjky.cn

[S17] C：安全拼接字符串
来源：http://cy.szsharing.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://qo.asd995.cn

[S18] C：命令行参数
来源：http://nu.bookmarksfly.cn

int main(int argc, char **argv)
来源：http://ze.521024.cn

[S19] C：快速排序
来源：http://fk.nicolike.cn

qsort(a, n, sizeof(int), cmp);
来源：http://qr.chemitech.net.cn

[S20] C：二分查找
来源：http://ce.lnxyls.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://dw.huixiangedu.cn

[S21] C：字符类别判断
来源：http://wy.huanxung.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://yg.lnxyls.cn

[S22] C：字符串转数字
来源：http://kw.hnjuh.cn

atoi("42");  strtod("3.14", NULL);
来源：http://uf.colortex.cn

[S23] C：随机数
来源：http://sn.521024.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://uf.panjiajie.cn

[S24] C：获取本地时间
来源：http://if.9csxet.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://sx.wgjwhj.cn

[S25] C：内存拷贝
来源：http://iz.9csxet.cn

memcpy(dst, src, n);
来源：http://ou.nicolike.cn

[S26] C：内存清零
来源：http://ej.szsharing.cn

memset(a, 0, sizeof a);
来源：http://df.jianghongdianzi.cn

[S27] C：定义常量
来源：http://lq.chemitech.net.cn

const double PI = 3.14159;
来源：http://zh.shxzskj.cn

[S28] C：静态变量
来源：http://ta.chemitech.net.cn

static int counter = 0;
来源：http://vr.lnxyls.cn

[S29] C：变参函数
来源：http://fc.newstarts.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://au.hahajie.cn

[S30] C：头文件保护
来源：http://kz.shxzskj.cn

#ifndef X_H
来源：http://jh.panjiajie.cn

#define X_H
来源：http://gi.szsharing.cn

#endif
来源：http://dr.newstarts.cn

[S31] C++：Hello World
来源：http://ln.newstarts.cn

#include <iostream>
来源：http://cz.szxytkj.cn

int main() { std::cout << "Hello\n"; }
来源：http://jb.asd995.cn

[S32] C++：字符串
来源：http://lf.asd995.cn

std::string s = "hi";  s += "!";
来源：http://pb.haigaiapp.cn

[S33] C++：vector 增删
来源：http://sb.yuexingan06.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://cd.chemitech.net.cn

[S34] C++：遍历 vector
来源：http://kj.bookmarksfly.cn

for (auto &x : v) { std::cout << x; }
来源：http://je.szsharing.cn

[S35] C++：map
来源：http://xd.huixiangedu.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://jk.jctech888.com.cn

[S36] C++：unordered_map
来源：http://cp.521024.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://xs.szxytkj.cn

[S37] C++：set
来源：http://uh.huixinmuqiang.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://zz.haigaiapp.cn

[S38] C++：排序
来源：http://sw.panjiajie.cn

std::sort(v.begin(), v.end());
来源：http://xf.bookmarksfly.cn

[S39] C++：自定义比较器排序
来源：http://fy.huanxung.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://uw.szxytkj.cn

[S40] C++：查找元素
来源：http://gt.szsharing.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://lx.nicolike.cn

[S41] C++：类与构造函数
来源：http://tj.panjiajie.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://yl.asd995.cn

[S42] C++：继承与虚函数
来源：http://xw.bjjhwx.cn

class B : public Base { public: void f() override {} };
来源：http://eb.shxzukj.cn

[S43] C++：智能指针
来源：http://pu.newstarts.cn

auto p = std::make_unique<int>(5);
来源：http://oe.shtwfgs.cn

[S44] C++：引用传参
来源：http://jj.panjiajie.cn

void inc(int &x) { ++x; }
来源：http://qk.gzmigu.cn

[S45] C++：lambda
来源：http://fs.shxzukj.cn

auto add = [](int a, int b) { return a + b; };
来源：http://xs.hahajie.cn

[S46] C++：函数模板
来源：http://di.yuexingan06.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ed.colortex.cn

[S47] C++：结构化绑定遍历
来源：http://bm.haigaiapp.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://yf.yuexingan06.cn

[S48] C++：逐行读文件
来源：http://no.szsharing.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ha.haigaiapp.cn

while (std::getline(in, line)) { }
来源：http://af.szsharing.cn

[S49] C++：写文件
来源：http://lx.haigaiapp.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://sj.huixiangedu.cn

[S50] C++：格式化数字
来源：http://xu.jianghongdianzi.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://qg.panjiajie.cn

[S51] C++：显式类型转换
来源：http://ke.muxihuayi.cn

static_cast<double>(a) / b
来源：http://xf.hnjuh.cn

[S52] C++：const 与 noexcept
来源：http://bo.haigaiapp.cn

int size() const noexcept { return n_; }
来源：http://yt.panjiajie.cn

[S53] C++：移动语义
来源：http://bg.bookmarksfly.cn

std::vector<int> w = std::move(v);
来源：http://pr.hnjuh.cn

[S54] C++：异常处理
来源：http://wv.newstarts.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://jc.nszjky.cn

[S55] C++：结构化绑定
来源：http://eg.szxytkj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://dv.gzmigu.cn

[S56] C++：optional
来源：http://rn.huanxung.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://od.shxzukj.cn

[S57] C++：编译期常量
来源：http://fn.shxzukj.cn

constexpr int N = 10;
来源：http://bh.newstarts.cn

[S58] C++：命名空间
来源：http://nd.bjjhwx.cn

namespace ns { int f() { return 1; } }
来源：http://zj.chemitech.net.cn

[S59] C++：静态断言
来源：http://lu.huixiangedu.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://si.shxzukj.cn

[S60] C++：遍历并删除元素
来源：http://ik.shxzskj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://rf.yuntaijiaju.cn

================================================================================
来源：http://ug.bjjhwx.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xu.hahajie.cn

================================================================================
来源：http://gu.huixinmuqiang.cn

[T01] Kotlin：Hello World
来源：http://yj.asd995.cn

println("Hello")
来源：http://au.shxzukj.cn

[T02] Kotlin：变量
来源：http://nk.jctech888.com.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ue.hnjuh.cn

[T03] Kotlin：字符串模板
来源：http://es.muxihuayi.cn

"值: $b"
来源：http://uc.panjiajie.cn

[T04] Kotlin：空安全
来源：http://ia.huixinmuqiang.cn

val n: String? = null;  n?.length
来源：http://vv.panjiajie.cn

[T05] Kotlin：when 表达式
来源：http://wq.hahajie.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://lo.jianghongdianzi.cn

[T06] Kotlin：集合映射
来源：http://yg.521024.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://gt.shxzskj.cn

[T07] Kotlin：集合过滤
来源：http://td.shxzukj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://lr.shxzskj.cn

[T08] Kotlin：数据类
来源：http://gf.szsharing.cn

data class User(val name: String, val age: Int)
来源：http://ak.newstarts.cn

[T09] Kotlin：扩展函数
来源：http://qm.wgjwhj.cn

fun String.exclaim() = this + "!"
来源：http://ti.huixinmuqiang.cn

[T10] Kotlin：默认参数
来源：http://cg.colortex.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ea.shxzukj.cn

[T11] Kotlin：协程
来源：http://yd.huixinmuqiang.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://qb.chemitech.net.cn

[T12] Kotlin：解构声明
来源：http://id.shxzskj.cn

val (a, b) = Pair(1, 2)
来源：http://dr.szsharing.cn

[T13] Kotlin：只读 Map
来源：http://du.9csxet.cn

val m = mapOf("a" to 1)
来源：http://pl.jctech888.com.cn

[T14] Kotlin：循环
来源：http://mb.lnxyls.cn

for (i in 1..10) println(i)
来源：http://et.jianghongdianzi.cn

[T15] Kotlin：接口
来源：http://hu.gzmigu.cn

interface Shape { fun area(): Double }
来源：http://ib.huixinmuqiang.cn

[T16] Swift：Hello World
来源：http://ti.szsharing.cn

print("Hello")
来源：http://ky.hnjuh.cn

[T17] Swift：变量与常量
来源：http://qk.yuexingan06.cn

var a = 1;  let b = 2
来源：http://qy.muxihuayi.cn

[T18] Swift：字符串插值
来源：http://oa.jianghongdianzi.cn

"值: \(b)"
来源：http://oj.chemitech.net.cn

[T19] Swift：可选绑定
来源：http://ae.muxihuayi.cn

if let n = opt { print(n) }
来源：http://ar.huanxung.cn

[T20] Swift：数组操作
来源：http://on.haigaiapp.cn

var a = [1, 2, 3];  a.append(4)
来源：http://kx.yuexingan06.cn

[T21] Swift：遍历
来源：http://ce.szxytkj.cn

for x in a { print(x) }
来源：http://xu.nszjky.cn

[T22] Swift：字典
来源：http://tk.bjjhwx.cn

var d = ["a": 1];  d["b"] = 2
来源：http://np.chemitech.net.cn

[T23] Swift：函数
来源：http://ud.muxihuayi.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mp.bookmarksfly.cn

[T24] Swift：闭包
来源：http://ya.521024.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ev.nszjky.cn

[T25] Swift：结构体
来源：http://us.asd995.cn

struct P { var x: Int }
来源：http://qd.yuntaijiaju.cn

[T26] Swift：类与重写
来源：http://xz.haigaiapp.cn

class A: Base { override func f() {} }
来源：http://pz.jianghongdianzi.cn

[T27] Swift：错误处理
来源：http://ls.shtwfgs.cn

do { try f() } catch { print(error) }
来源：http://ev.muxihuayi.cn

[T28] Swift：枚举
来源：http://qd.bjjhwx.cn

enum Color { case red, green }
来源：http://rs.colortex.cn

[T29] Swift：guard 提前返回
来源：http://ho.haigaiapp.cn

guard let x = opt else { return }
来源：http://yc.muxihuayi.cn

[T30] Swift：协议
来源：http://gj.lnxyls.cn

protocol Shape { func area() -> Double }
来源：http://yk.chemitech.net.cn

[T31] Lua：Hello World
来源：http://gk.nszjky.cn

print("Hello")
来源：http://ks.jianghongdianzi.cn

[T32] Lua：局部变量
来源：http://ws.colortex.cn

local a = 1
来源：http://il.newstarts.cn

[T33] Lua：表（数组）
来源：http://er.hnjuh.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://bx.9csxet.cn

[T34] Lua：遍历表
来源：http://ae.lnxyls.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://cv.chemitech.net.cn

[T35] Lua：字典表
来源：http://en.haigaiapp.cn

local d = { a = 1 };  d.b = 2
来源：http://yo.nszjky.cn

[T36] Lua：函数
来源：http://vo.shxzukj.cn

function add(a, b) return a + b end
来源：http://ev.hahajie.cn

[T37] Lua：字符串拼接
来源：http://xv.szxytkj.cn

"a" .. "b"
来源：http://sp.huanxung.cn

[T38] Lua：条件
来源：http://ev.hahajie.cn

if x > 0 then print("正") end
来源：http://gl.lnxyls.cn

[T39] Lua：模式匹配
来源：http://up.jianghongdianzi.cn

string.find(s, "%d+")
来源：http://wj.asd995.cn

[T40] Lua：元表
来源：http://ck.bookmarksfly.cn

setmetatable({}, { __index = base })
来源：http://fv.gzmigu.cn

[T41] Perl：Hello World
来源：http://wf.huixiangedu.cn

print "Hello\n";
来源：http://rq.9csxet.cn

[T42] Perl：变量类型
来源：http://df.521024.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://hj.chemitech.net.cn

[T43] Perl：字符串插值
来源：http://go.521024.cn

"值: $a"
来源：http://yi.newstarts.cn

[T44] Perl：条件
来源：http://sq.yuexingan06.cn

if ($a > 0) { print "正"; }
来源：http://hk.muxihuayi.cn

[T45] Perl：数组遍历
来源：http://tw.521024.cn

for my $x (@arr) { print $x; }
来源：http://xs.huixinmuqiang.cn

[T46] Perl：哈希操作
来源：http://ua.shxzskj.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://sj.shxzukj.cn

[T47] Perl：正则捕获
来源：http://tz.hahajie.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://zs.shxzskj.cn

[T48] Perl：正则替换
来源：http://mt.hnjuh.cn

$s =~ s/old/new/g;
来源：http://he.panjiajie.cn

[T49] Perl：函数
来源：http://ap.bookmarksfly.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://fs.shxzukj.cn

[T50] Perl：逐行读文件
来源：http://ld.huixiangedu.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://co.panjiajie.cn

while (my $line = <$fh>) { print $line; }
来源：http://yh.nicolike.cn

[T51] Scala：Hello World
来源：http://sm.szsharing.cn

println("Hello")
来源：http://be.chemitech.net.cn

[T52] Scala：变量
来源：http://wj.bookmarksfly.cn

val a = 1;  var b = 2
来源：http://yu.muxihuayi.cn

[T53] Scala：字符串插值
来源：http://rn.hnjuh.cn

s"值: $b"
来源：http://hz.shxzukj.cn

[T54] Scala：集合映射
来源：http://kg.shxzskj.cn

List(1, 2, 3).map(_ * 2)
来源：http://fl.asd995.cn

[T55] Scala：集合过滤
来源：http://wr.gzmigu.cn

List(1, 2, 3).filter(_ > 1)
来源：http://eq.bjjhwx.cn

[T56] Scala：样例类
来源：http://wx.nszjky.cn

case class User(name: String, age: Int)
来源：http://kc.shxzskj.cn

[T57] Scala：模式匹配
来源：http://nv.jctech888.com.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://gz.jctech888.com.cn

[T58] Scala：函数定义
来源：http://fl.hahajie.cn

def add(a: Int, b: Int): Int = a + b
来源：http://nw.shxzukj.cn

[T59] Scala：循环
来源：http://xa.huixinmuqiang.cn

for (i <- 1 to 10) println(i)
来源：http://ow.bookmarksfly.cn

[T60] Scala：折叠
来源：http://kd.bookmarksfly.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ks.colortex.cn

================================================================================
来源：http://ok.gzmigu.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wr.jianghongdianzi.cn

================================================================================
来源：http://co.yuexingan06.cn

[U01] Py：创建虚拟环境
来源：http://uf.yuntaijiaju.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ny.shxzskj.cn

[U02] Py：导出 / 安装依赖
来源：http://fv.muxihuayi.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://vq.bookmarksfly.cn

[U03] Py：加载 .env 配置
来源：http://uf.panjiajie.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://wp.jctech888.com.cn

[U04] Py：变量调试打印
来源：http://xj.bookmarksfly.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://gq.gzmigu.cn

[U05] Py：列表去重且保序
来源：http://un.9csxet.cn

list(dict.fromkeys(arr))
来源：http://pa.yuntaijiaju.cn

[U06] Py：合并两个字典
来源：http://wl.jianghongdianzi.cn

{**a, **b}
来源：http://nn.521024.cn

[U07] Py：反转字典键值
来源：http://iw.shxzskj.cn

{v: k for k, v in d.items()}
来源：http://pa.bjjhwx.cn

[U08] Py：展平二维列表
来源：http://lp.shxzskj.cn

[y for x in nested for y in x]
来源：http://dl.muxihuayi.cn


<!-- 参考信息 -->