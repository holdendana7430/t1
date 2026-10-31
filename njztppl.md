代发 wailian999

free -h;  ps aux | grep nginx
来源：http://lp.muxihuayi.cn

[R64] 结束进程
来源：http://qc.jctech888.com.cn

kill -9 $(pgrep -f app.py)
来源：http://li.nszjky.cn

[R65] 查看端口占用
来源：http://cj.szsharing.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://st.panjiajie.cn

[R66] 定时任务
来源：http://zv.haigaiapp.cn

crontab -e;  crontab -l
来源：http://rs.bjjhwx.cn

[R67] 生成随机十六进制串
来源：http://vf.9csxet.cn

openssl rand -hex 16
来源：http://oz.gzmigu.cn

[R68] 计算文件校验值
来源：http://zi.huixiangedu.cn

sha256sum a.txt;  md5sum a.txt
来源：http://xs.bjjhwx.cn

[R69] 生成随机密码
来源：http://lf.shxzukj.cn

head -c 16 /dev/urandom | base64
来源：http://nr.bjjhwx.cn

[R70] 时间戳与互转
来源：http://nu.yuexingan06.cn

date +%s;  date -d @1700000000
来源：http://sz.panjiajie.cn

[R71] 日期格式化
来源：http://xj.muxihuayi.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ju.nicolike.cn

[R72] 等待端口就绪
来源：http://ke.huixiangedu.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://jz.newstarts.cn

[R73] 分割大日志
来源：http://lk.nszjky.cn

split -l 1000 big.log part_
来源：http://rv.chemitech.net.cn

[R74] 批量重命名
来源：http://fp.panjiajie.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://xq.yuntaijiaju.cn

[R75] 导出环境变量
来源：http://vp.szxytkj.cn

export PATH="$HOME/bin:$PATH"
来源：http://ox.shxzskj.cn

[R76] 使用临时文件
来源：http://ds.lnxyls.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://la.panjiajie.cn

[R77] 读取用户输入
来源：http://mn.haigaiapp.cn

read -rp "请输入: " ans
来源：http://gx.haigaiapp.cn

[R78] 交互式菜单
来源：http://bj.nszjky.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://jk.hnjuh.cn

[R79] 解析命令行选项
来源：http://by.muxihuayi.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://se.bookmarksfly.cn

[R80] 查看脚本执行耗时
来源：http://fe.bookmarksfly.cn

time ./run.sh
来源：http://xy.nicolike.cn

================================================================================
来源：http://so.521024.cn

S. C / C++ 专题
来源：http://pi.9csxet.cn

================================================================================
来源：http://cx.jctech888.com.cn

[S01] C：Hello World
来源：http://jb.hnjuh.cn

#include <stdio.h>
来源：http://do.bjjhwx.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://wo.jctech888.com.cn

[S02] C：变量与格式化输出
来源：http://fv.hnjuh.cn

int a = 10; printf("%d\n", a);
来源：http://xm.yuexingan06.cn

[S03] C：读入整数
来源：http://sf.hahajie.cn

int x; scanf("%d", &x);
来源：http://wz.yuexingan06.cn

[S04] C：字符串复制
来源：http://ep.chemitech.net.cn

char dst[32]; strcpy(dst, "hi");
来源：http://sm.hahajie.cn

[S05] C：字符串长度
来源：http://an.521024.cn

strlen(s)
来源：http://dw.colortex.cn

[S06] C：字符串比较
来源：http://ji.szsharing.cn

strcmp(a, b) == 0
来源：http://qs.haigaiapp.cn

[S07] C：数组遍历求和
来源：http://hf.muxihuayi.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ts.chemitech.net.cn

[S08] C：动态内存分配与释放
来源：http://jk.bookmarksfly.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://kl.colortex.cn

[S09] C：结构体定义与初始化
来源：http://ut.shxzskj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://cx.bookmarksfly.cn

[S10] C：指针与解引用
来源：http://gs.szsharing.cn

int *p = &a;  *p = 5;
来源：http://fn.bookmarksfly.cn

[S11] C：逐行读文件
来源：http://cr.newstarts.cn

FILE *f = fopen("a.txt", "r");
来源：http://pe.asd995.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://cs.bookmarksfly.cn

fclose(f);
来源：http://rx.colortex.cn

[S12] C：写文件
来源：http://sn.gzmigu.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://rx.9csxet.cn

[S13] C：宏定义
来源：http://ge.wgjwhj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://hd.huanxung.cn

[S14] C：枚举
来源：http://nf.chemitech.net.cn

enum Color { RED, GREEN, BLUE };
来源：http://le.haigaiapp.cn

[S15] C：类型转换
来源：http://nq.hahajie.cn

(double) a / b
来源：http://xa.shxzukj.cn

[S16] C：位操作置位
来源：http://hj.yuexingan06.cn

x |= (1 << 3);
来源：http://ml.huanxung.cn

[S17] C：安全拼接字符串
来源：http://fs.colortex.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://jv.lnxyls.cn

[S18] C：命令行参数
来源：http://yi.asd995.cn

int main(int argc, char **argv)
来源：http://hn.shtwfgs.cn

[S19] C：快速排序
来源：http://zv.hnjuh.cn

qsort(a, n, sizeof(int), cmp);
来源：http://go.nszjky.cn

[S20] C：二分查找
来源：http://sw.muxihuayi.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://is.lnxyls.cn

[S21] C：字符类别判断
来源：http://zv.bookmarksfly.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://jd.521024.cn

[S22] C：字符串转数字
来源：http://uv.huanxung.cn

atoi("42");  strtod("3.14", NULL);
来源：http://vy.muxihuayi.cn

[S23] C：随机数
来源：http://wt.gzmigu.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://dk.bookmarksfly.cn

[S24] C：获取本地时间
来源：http://ul.shxzskj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://qn.yuntaijiaju.cn

[S25] C：内存拷贝
来源：http://fm.szxytkj.cn

memcpy(dst, src, n);
来源：http://ze.yuexingan06.cn

[S26] C：内存清零
来源：http://it.szxytkj.cn

memset(a, 0, sizeof a);
来源：http://ql.szsharing.cn

[S27] C：定义常量
来源：http://ij.szxytkj.cn

const double PI = 3.14159;
来源：http://el.jianghongdianzi.cn

[S28] C：静态变量
来源：http://xk.huixinmuqiang.cn

static int counter = 0;
来源：http://it.chemitech.net.cn

[S29] C：变参函数
来源：http://hn.bookmarksfly.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://tf.shtwfgs.cn

[S30] C：头文件保护
来源：http://an.colortex.cn

#ifndef X_H
来源：http://va.nszjky.cn

#define X_H
来源：http://si.lnxyls.cn

#endif
来源：http://nh.shxzskj.cn

[S31] C++：Hello World
来源：http://za.shxzukj.cn

#include <iostream>
来源：http://jj.newstarts.cn

int main() { std::cout << "Hello\n"; }
来源：http://lz.jctech888.com.cn

[S32] C++：字符串
来源：http://kn.jianghongdianzi.cn

std::string s = "hi";  s += "!";
来源：http://fy.huixinmuqiang.cn

[S33] C++：vector 增删
来源：http://pt.gzmigu.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://gg.chemitech.net.cn

[S34] C++：遍历 vector
来源：http://rg.shxzskj.cn

for (auto &x : v) { std::cout << x; }
来源：http://rq.hahajie.cn

[S35] C++：map
来源：http://on.huanxung.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://am.asd995.cn

[S36] C++：unordered_map
来源：http://tj.shxzskj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://zy.huixiangedu.cn

[S37] C++：set
来源：http://xt.hnjuh.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://vi.bookmarksfly.cn

[S38] C++：排序
来源：http://oh.colortex.cn

std::sort(v.begin(), v.end());
来源：http://kh.lnxyls.cn

[S39] C++：自定义比较器排序
来源：http://ye.newstarts.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://gt.bookmarksfly.cn

[S40] C++：查找元素
来源：http://wk.shxzukj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ss.muxihuayi.cn

[S41] C++：类与构造函数
来源：http://aj.nszjky.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://pw.huanxung.cn

[S42] C++：继承与虚函数
来源：http://wd.bookmarksfly.cn

class B : public Base { public: void f() override {} };
来源：http://ez.shxzukj.cn

[S43] C++：智能指针
来源：http://tw.shxzskj.cn

auto p = std::make_unique<int>(5);
来源：http://ut.newstarts.cn

[S44] C++：引用传参
来源：http://vm.huixinmuqiang.cn

void inc(int &x) { ++x; }
来源：http://ih.nszjky.cn

[S45] C++：lambda
来源：http://ve.chemitech.net.cn

auto add = [](int a, int b) { return a + b; };
来源：http://se.newstarts.cn

[S46] C++：函数模板
来源：http://bx.colortex.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://uc.nicolike.cn

[S47] C++：结构化绑定遍历
来源：http://un.haigaiapp.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://lv.huixinmuqiang.cn

[S48] C++：逐行读文件
来源：http://cc.nszjky.cn

std::ifstream in("a.txt");  std::string line;
来源：http://hc.nszjky.cn

while (std::getline(in, line)) { }
来源：http://nm.nszjky.cn

[S49] C++：写文件
来源：http://rr.yuntaijiaju.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://pf.szsharing.cn

[S50] C++：格式化数字
来源：http://sp.szsharing.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://if.gzmigu.cn

[S51] C++：显式类型转换
来源：http://ra.huanxung.cn

static_cast<double>(a) / b
来源：http://dy.chemitech.net.cn

[S52] C++：const 与 noexcept
来源：http://mb.chemitech.net.cn

int size() const noexcept { return n_; }
来源：http://pp.lnxyls.cn

[S53] C++：移动语义
来源：http://ts.yuntaijiaju.cn

std::vector<int> w = std::move(v);
来源：http://zx.colortex.cn

[S54] C++：异常处理
来源：http://hl.asd995.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://rp.newstarts.cn

[S55] C++：结构化绑定
来源：http://xo.hnjuh.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ua.yuntaijiaju.cn

[S56] C++：optional
来源：http://oq.lnxyls.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://cq.shtwfgs.cn

[S57] C++：编译期常量
来源：http://lb.shxzukj.cn

constexpr int N = 10;
来源：http://br.muxihuayi.cn

[S58] C++：命名空间
来源：http://gw.yuntaijiaju.cn

namespace ns { int f() { return 1; } }
来源：http://xs.colortex.cn

[S59] C++：静态断言
来源：http://sz.haigaiapp.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://iu.newstarts.cn

[S60] C++：遍历并删除元素
来源：http://vk.gzmigu.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://it.9csxet.cn

================================================================================
来源：http://xz.521024.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://co.yuntaijiaju.cn

================================================================================
来源：http://gl.shxzukj.cn

[T01] Kotlin：Hello World
来源：http://wm.hahajie.cn

println("Hello")
来源：http://jh.bjjhwx.cn

[T02] Kotlin：变量
来源：http://lh.521024.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://je.szsharing.cn

[T03] Kotlin：字符串模板
来源：http://yn.hahajie.cn

"值: $b"
来源：http://zx.nicolike.cn

[T04] Kotlin：空安全
来源：http://jf.hnjuh.cn

val n: String? = null;  n?.length
来源：http://tl.chemitech.net.cn

[T05] Kotlin：when 表达式
来源：http://wq.shtwfgs.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://bo.newstarts.cn

[T06] Kotlin：集合映射
来源：http://mn.chemitech.net.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://sv.jianghongdianzi.cn

[T07] Kotlin：集合过滤
来源：http://rs.shtwfgs.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://iy.hnjuh.cn

[T08] Kotlin：数据类
来源：http://at.huixinmuqiang.cn

data class User(val name: String, val age: Int)
来源：http://ko.huixiangedu.cn

[T09] Kotlin：扩展函数
来源：http://yq.newstarts.cn

fun String.exclaim() = this + "!"
来源：http://fe.szsharing.cn

[T10] Kotlin：默认参数
来源：http://ia.panjiajie.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://sx.szxytkj.cn

[T11] Kotlin：协程
来源：http://bw.lnxyls.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://bc.shtwfgs.cn

[T12] Kotlin：解构声明
来源：http://yn.huanxung.cn

val (a, b) = Pair(1, 2)
来源：http://yy.wgjwhj.cn

[T13] Kotlin：只读 Map
来源：http://pk.jctech888.com.cn

val m = mapOf("a" to 1)
来源：http://vz.newstarts.cn

[T14] Kotlin：循环
来源：http://nx.hnjuh.cn

for (i in 1..10) println(i)
来源：http://sc.lnxyls.cn

[T15] Kotlin：接口
来源：http://az.huixiangedu.cn

interface Shape { fun area(): Double }
来源：http://bn.yuntaijiaju.cn

[T16] Swift：Hello World
来源：http://on.szxytkj.cn

print("Hello")
来源：http://jt.yuntaijiaju.cn

[T17] Swift：变量与常量
来源：http://zg.haigaiapp.cn

var a = 1;  let b = 2
来源：http://pm.shtwfgs.cn

[T18] Swift：字符串插值
来源：http://hn.huanxung.cn

"值: \(b)"
来源：http://sm.lnxyls.cn

[T19] Swift：可选绑定
来源：http://oo.9csxet.cn

if let n = opt { print(n) }
来源：http://ir.wgjwhj.cn

[T20] Swift：数组操作
来源：http://lz.haigaiapp.cn

var a = [1, 2, 3];  a.append(4)
来源：http://aw.wgjwhj.cn

[T21] Swift：遍历
来源：http://dz.nicolike.cn

for x in a { print(x) }
来源：http://wd.szsharing.cn

[T22] Swift：字典
来源：http://ns.521024.cn

var d = ["a": 1];  d["b"] = 2
来源：http://lp.muxihuayi.cn

[T23] Swift：函数
来源：http://yz.shtwfgs.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ir.hahajie.cn

[T24] Swift：闭包
来源：http://kz.muxihuayi.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://yi.huixinmuqiang.cn

[T25] Swift：结构体
来源：http://yk.asd995.cn

struct P { var x: Int }
来源：http://qd.jctech888.com.cn

[T26] Swift：类与重写
来源：http://dc.shxzskj.cn

class A: Base { override func f() {} }
来源：http://sw.colortex.cn

[T27] Swift：错误处理
来源：http://lz.muxihuayi.cn

do { try f() } catch { print(error) }
来源：http://ns.hnjuh.cn

[T28] Swift：枚举
来源：http://xw.nszjky.cn

enum Color { case red, green }
来源：http://fr.newstarts.cn

[T29] Swift：guard 提前返回
来源：http://ov.521024.cn

guard let x = opt else { return }
来源：http://as.yuexingan06.cn

[T30] Swift：协议
来源：http://pd.shxzskj.cn

protocol Shape { func area() -> Double }
来源：http://lh.gzmigu.cn

[T31] Lua：Hello World
来源：http://il.shxzukj.cn

print("Hello")
来源：http://pt.lnxyls.cn

[T32] Lua：局部变量
来源：http://uj.szxytkj.cn

local a = 1
来源：http://uh.huixiangedu.cn

[T33] Lua：表（数组）
来源：http://vz.panjiajie.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://jc.gzmigu.cn

[T34] Lua：遍历表
来源：http://ex.bookmarksfly.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://in.jianghongdianzi.cn

[T35] Lua：字典表
来源：http://fm.newstarts.cn

local d = { a = 1 };  d.b = 2
来源：http://vi.huixinmuqiang.cn

[T36] Lua：函数
来源：http://lp.hahajie.cn

function add(a, b) return a + b end
来源：http://ix.521024.cn

[T37] Lua：字符串拼接
来源：http://ma.haigaiapp.cn

"a" .. "b"
来源：http://lu.huixiangedu.cn

[T38] Lua：条件
来源：http://eq.szsharing.cn

if x > 0 then print("正") end
来源：http://kl.asd995.cn

[T39] Lua：模式匹配
来源：http://dm.asd995.cn

string.find(s, "%d+")
来源：http://ve.bookmarksfly.cn

[T40] Lua：元表
来源：http://ae.huixinmuqiang.cn

setmetatable({}, { __index = base })
来源：http://ml.521024.cn

[T41] Perl：Hello World
来源：http://ig.huixiangedu.cn

print "Hello\n";
来源：http://wk.521024.cn

[T42] Perl：变量类型
来源：http://ri.muxihuayi.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://un.szxytkj.cn

[T43] Perl：字符串插值
来源：http://vr.huanxung.cn

"值: $a"
来源：http://rq.yuexingan06.cn

[T44] Perl：条件
来源：http://dl.hnjuh.cn

if ($a > 0) { print "正"; }
来源：http://sa.shtwfgs.cn

[T45] Perl：数组遍历
来源：http://lp.jctech888.com.cn

for my $x (@arr) { print $x; }
来源：http://tg.wgjwhj.cn

[T46] Perl：哈希操作
来源：http://jh.hnjuh.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://dq.colortex.cn

[T47] Perl：正则捕获
来源：http://vs.huanxung.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://bk.chemitech.net.cn

[T48] Perl：正则替换
来源：http://hh.wgjwhj.cn

$s =~ s/old/new/g;
来源：http://yn.hnjuh.cn

[T49] Perl：函数
来源：http://sk.lnxyls.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://bj.jctech888.com.cn

[T50] Perl：逐行读文件
来源：http://cj.lnxyls.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ux.nszjky.cn

while (my $line = <$fh>) { print $line; }
来源：http://dc.jianghongdianzi.cn

[T51] Scala：Hello World
来源：http://ec.hnjuh.cn

println("Hello")
来源：http://zr.shxzukj.cn

[T52] Scala：变量
来源：http://lq.nicolike.cn

val a = 1;  var b = 2
来源：http://ri.huixinmuqiang.cn

[T53] Scala：字符串插值
来源：http://js.jctech888.com.cn

s"值: $b"
来源：http://hs.shxzskj.cn

[T54] Scala：集合映射
来源：http://br.huixinmuqiang.cn

List(1, 2, 3).map(_ * 2)
来源：http://tk.wgjwhj.cn

[T55] Scala：集合过滤
来源：http://bb.hahajie.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ci.shtwfgs.cn

[T56] Scala：样例类
来源：http://nh.gzmigu.cn

case class User(name: String, age: Int)
来源：http://ey.szxytkj.cn

[T57] Scala：模式匹配
来源：http://fl.jctech888.com.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://oe.9csxet.cn

[T58] Scala：函数定义
来源：http://nz.szsharing.cn

def add(a: Int, b: Int): Int = a + b
来源：http://bw.jianghongdianzi.cn

[T59] Scala：循环
来源：http://ye.yuntaijiaju.cn

for (i <- 1 to 10) println(i)
来源：http://yv.szsharing.cn

[T60] Scala：折叠
来源：http://wh.asd995.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://me.chemitech.net.cn

================================================================================
来源：http://lo.jctech888.com.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wn.yuntaijiaju.cn

================================================================================
来源：http://ll.wgjwhj.cn

[U01] Py：创建虚拟环境
来源：http://ns.lnxyls.cn

python -m venv .venv && source .venv/bin/activate
来源：http://qa.521024.cn

[U02] Py：导出 / 安装依赖
来源：http://ri.hnjuh.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://wy.bookmarksfly.cn

[U03] Py：加载 .env 配置
来源：http://xf.szsharing.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://wg.hahajie.cn

[U04] Py：变量调试打印
来源：http://zn.nicolike.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://vm.nicolike.cn


<!-- 参考信息 -->