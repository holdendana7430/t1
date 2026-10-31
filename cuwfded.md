代发 wailian999

df -h;  du -sh *
来源：http://tb.huanxung.cn

[R62] 找最占空间的文件
来源：http://sp.haigaiapp.cn

du -ah . | sort -rh | head -10
来源：http://nh.newstarts.cn

[R63] 内存与进程
来源：http://ya.gzmigu.cn

free -h;  ps aux | grep nginx
来源：http://mh.521024.cn

[R64] 结束进程
来源：http://ai.newstarts.cn

kill -9 $(pgrep -f app.py)
来源：http://kk.yuntaijiaju.cn

[R65] 查看端口占用
来源：http://em.yuexingan06.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://bv.nicolike.cn

[R66] 定时任务
来源：http://ar.yuntaijiaju.cn

crontab -e;  crontab -l
来源：http://mn.newstarts.cn

[R67] 生成随机十六进制串
来源：http://zz.nszjky.cn

openssl rand -hex 16
来源：http://uq.huixiangedu.cn

[R68] 计算文件校验值
来源：http://fx.haigaiapp.cn

sha256sum a.txt;  md5sum a.txt
来源：http://wh.haigaiapp.cn

[R69] 生成随机密码
来源：http://im.panjiajie.cn

head -c 16 /dev/urandom | base64
来源：http://yn.bjjhwx.cn

[R70] 时间戳与互转
来源：http://jy.bjjhwx.cn

date +%s;  date -d @1700000000
来源：http://hm.nicolike.cn

[R71] 日期格式化
来源：http://dx.newstarts.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://gy.huixinmuqiang.cn

[R72] 等待端口就绪
来源：http://kd.huanxung.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ze.asd995.cn

[R73] 分割大日志
来源：http://pr.jctech888.com.cn

split -l 1000 big.log part_
来源：http://fa.nicolike.cn

[R74] 批量重命名
来源：http://da.newstarts.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://gn.jianghongdianzi.cn

[R75] 导出环境变量
来源：http://qe.bjjhwx.cn

export PATH="$HOME/bin:$PATH"
来源：http://yp.521024.cn

[R76] 使用临时文件
来源：http://im.jctech888.com.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ns.huanxung.cn

[R77] 读取用户输入
来源：http://bn.lnxyls.cn

read -rp "请输入: " ans
来源：http://nw.hahajie.cn

[R78] 交互式菜单
来源：http://oc.bjjhwx.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://bx.gzmigu.cn

[R79] 解析命令行选项
来源：http://uy.shxzukj.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://yu.lnxyls.cn

[R80] 查看脚本执行耗时
来源：http://qs.szsharing.cn

time ./run.sh
来源：http://fa.huixinmuqiang.cn

================================================================================
来源：http://ua.bookmarksfly.cn

S. C / C++ 专题
来源：http://qc.hahajie.cn

================================================================================
来源：http://wq.yuntaijiaju.cn

[S01] C：Hello World
来源：http://we.haigaiapp.cn

#include <stdio.h>
来源：http://kn.szxytkj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://yf.wgjwhj.cn

[S02] C：变量与格式化输出
来源：http://ij.haigaiapp.cn

int a = 10; printf("%d\n", a);
来源：http://vt.huanxung.cn

[S03] C：读入整数
来源：http://iy.nszjky.cn

int x; scanf("%d", &x);
来源：http://by.asd995.cn

[S04] C：字符串复制
来源：http://ol.shxzskj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://uo.colortex.cn

[S05] C：字符串长度
来源：http://ja.panjiajie.cn

strlen(s)
来源：http://ch.yuntaijiaju.cn

[S06] C：字符串比较
来源：http://li.jctech888.com.cn

strcmp(a, b) == 0
来源：http://mw.asd995.cn

[S07] C：数组遍历求和
来源：http://lw.huanxung.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://dv.nszjky.cn

[S08] C：动态内存分配与释放
来源：http://cg.hahajie.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hf.asd995.cn

[S09] C：结构体定义与初始化
来源：http://bt.wgjwhj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://bk.bookmarksfly.cn

[S10] C：指针与解引用
来源：http://jf.asd995.cn

int *p = &a;  *p = 5;
来源：http://bt.huanxung.cn

[S11] C：逐行读文件
来源：http://pf.wgjwhj.cn

FILE *f = fopen("a.txt", "r");
来源：http://ur.muxihuayi.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ei.szsharing.cn

fclose(f);
来源：http://wu.nszjky.cn

[S12] C：写文件
来源：http://py.muxihuayi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://gm.muxihuayi.cn

[S13] C：宏定义
来源：http://oe.szxytkj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://id.huixiangedu.cn

[S14] C：枚举
来源：http://pq.521024.cn

enum Color { RED, GREEN, BLUE };
来源：http://ia.hahajie.cn

[S15] C：类型转换
来源：http://vm.yuexingan06.cn

(double) a / b
来源：http://hh.9csxet.cn

[S16] C：位操作置位
来源：http://yc.gzmigu.cn

x |= (1 << 3);
来源：http://zt.bookmarksfly.cn

[S17] C：安全拼接字符串
来源：http://do.hahajie.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wh.panjiajie.cn

[S18] C：命令行参数
来源：http://co.shxzskj.cn

int main(int argc, char **argv)
来源：http://cd.lnxyls.cn

[S19] C：快速排序
来源：http://km.9csxet.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ir.chemitech.net.cn

[S20] C：二分查找
来源：http://rz.nszjky.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://xs.huanxung.cn

[S21] C：字符类别判断
来源：http://ie.asd995.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://lj.9csxet.cn

[S22] C：字符串转数字
来源：http://ip.shxzukj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://km.colortex.cn

[S23] C：随机数
来源：http://yb.yuexingan06.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://mk.huixiangedu.cn

[S24] C：获取本地时间
来源：http://fm.9csxet.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://cr.haigaiapp.cn

[S25] C：内存拷贝
来源：http://qz.panjiajie.cn

memcpy(dst, src, n);
来源：http://rr.521024.cn

[S26] C：内存清零
来源：http://bb.nszjky.cn

memset(a, 0, sizeof a);
来源：http://cw.bookmarksfly.cn

[S27] C：定义常量
来源：http://rf.jianghongdianzi.cn

const double PI = 3.14159;
来源：http://tq.szsharing.cn

[S28] C：静态变量
来源：http://rn.chemitech.net.cn

static int counter = 0;
来源：http://hh.chemitech.net.cn

[S29] C：变参函数
来源：http://mj.shtwfgs.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://gc.asd995.cn

[S30] C：头文件保护
来源：http://kf.521024.cn

#ifndef X_H
来源：http://zr.nicolike.cn

#define X_H
来源：http://ac.shxzskj.cn

#endif
来源：http://hs.huixinmuqiang.cn

[S31] C++：Hello World
来源：http://pf.gzmigu.cn

#include <iostream>
来源：http://zx.szsharing.cn

int main() { std::cout << "Hello\n"; }
来源：http://ix.shxzskj.cn

[S32] C++：字符串
来源：http://st.shxzskj.cn

std::string s = "hi";  s += "!";
来源：http://ws.yuexingan06.cn

[S33] C++：vector 增删
来源：http://li.muxihuayi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ne.jctech888.com.cn

[S34] C++：遍历 vector
来源：http://cf.chemitech.net.cn

for (auto &x : v) { std::cout << x; }
来源：http://oj.szxytkj.cn

[S35] C++：map
来源：http://nw.wgjwhj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ss.521024.cn

[S36] C++：unordered_map
来源：http://ey.szsharing.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://kn.shxzukj.cn

[S37] C++：set
来源：http://wy.yuntaijiaju.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://so.colortex.cn

[S38] C++：排序
来源：http://xi.shxzukj.cn

std::sort(v.begin(), v.end());
来源：http://fg.panjiajie.cn

[S39] C++：自定义比较器排序
来源：http://hq.hnjuh.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://im.wgjwhj.cn

[S40] C++：查找元素
来源：http://fk.gzmigu.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mm.haigaiapp.cn

[S41] C++：类与构造函数
来源：http://pt.colortex.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://pa.shxzukj.cn

[S42] C++：继承与虚函数
来源：http://yi.muxihuayi.cn

class B : public Base { public: void f() override {} };
来源：http://wn.huanxung.cn

[S43] C++：智能指针
来源：http://xd.jianghongdianzi.cn

auto p = std::make_unique<int>(5);
来源：http://wm.9csxet.cn

[S44] C++：引用传参
来源：http://sf.szxytkj.cn

void inc(int &x) { ++x; }
来源：http://bf.szxytkj.cn

[S45] C++：lambda
来源：http://ii.panjiajie.cn

auto add = [](int a, int b) { return a + b; };
来源：http://yn.jctech888.com.cn

[S46] C++：函数模板
来源：http://bh.nszjky.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://yg.newstarts.cn

[S47] C++：结构化绑定遍历
来源：http://po.521024.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://bd.hahajie.cn

[S48] C++：逐行读文件
来源：http://ea.gzmigu.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ex.szxytkj.cn

while (std::getline(in, line)) { }
来源：http://jl.wgjwhj.cn

[S49] C++：写文件
来源：http://rd.newstarts.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://if.bookmarksfly.cn

[S50] C++：格式化数字
来源：http://yi.jctech888.com.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://vf.newstarts.cn

[S51] C++：显式类型转换
来源：http://nd.chemitech.net.cn

static_cast<double>(a) / b
来源：http://tj.lnxyls.cn

[S52] C++：const 与 noexcept
来源：http://qt.colortex.cn

int size() const noexcept { return n_; }
来源：http://bq.szsharing.cn

[S53] C++：移动语义
来源：http://dl.bookmarksfly.cn

std::vector<int> w = std::move(v);
来源：http://ck.huixinmuqiang.cn

[S54] C++：异常处理
来源：http://nv.nicolike.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://fd.lnxyls.cn

[S55] C++：结构化绑定
来源：http://pe.szsharing.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://vg.asd995.cn

[S56] C++：optional
来源：http://cx.9csxet.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://gz.shxzskj.cn

[S57] C++：编译期常量
来源：http://jq.panjiajie.cn

constexpr int N = 10;
来源：http://lk.shtwfgs.cn

[S58] C++：命名空间
来源：http://lr.muxihuayi.cn

namespace ns { int f() { return 1; } }
来源：http://tb.szxytkj.cn

[S59] C++：静态断言
来源：http://kz.huanxung.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://kz.yuexingan06.cn

[S60] C++：遍历并删除元素
来源：http://qg.nicolike.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hn.huixinmuqiang.cn

================================================================================
来源：http://qk.newstarts.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://nx.huixinmuqiang.cn

================================================================================
来源：http://xd.bookmarksfly.cn

[T01] Kotlin：Hello World
来源：http://ly.haigaiapp.cn

println("Hello")
来源：http://vp.hnjuh.cn

[T02] Kotlin：变量
来源：http://it.huixiangedu.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://dn.panjiajie.cn

[T03] Kotlin：字符串模板
来源：http://np.jianghongdianzi.cn

"值: $b"
来源：http://iy.szsharing.cn

[T04] Kotlin：空安全
来源：http://dv.haigaiapp.cn

val n: String? = null;  n?.length
来源：http://pv.bjjhwx.cn

[T05] Kotlin：when 表达式
来源：http://uk.newstarts.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://wm.shxzskj.cn

[T06] Kotlin：集合映射
来源：http://gp.9csxet.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://rm.asd995.cn

[T07] Kotlin：集合过滤
来源：http://ff.521024.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://kr.wgjwhj.cn

[T08] Kotlin：数据类
来源：http://us.bjjhwx.cn

data class User(val name: String, val age: Int)
来源：http://zh.huanxung.cn

[T09] Kotlin：扩展函数
来源：http://ym.panjiajie.cn

fun String.exclaim() = this + "!"
来源：http://lu.chemitech.net.cn

[T10] Kotlin：默认参数
来源：http://it.asd995.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://th.shtwfgs.cn

[T11] Kotlin：协程
来源：http://bt.szsharing.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ft.jianghongdianzi.cn

[T12] Kotlin：解构声明
来源：http://fp.shxzskj.cn

val (a, b) = Pair(1, 2)
来源：http://yx.newstarts.cn

[T13] Kotlin：只读 Map
来源：http://gs.szxytkj.cn

val m = mapOf("a" to 1)
来源：http://zq.colortex.cn

[T14] Kotlin：循环
来源：http://cd.shxzskj.cn

for (i in 1..10) println(i)
来源：http://dq.szsharing.cn

[T15] Kotlin：接口
来源：http://nx.wgjwhj.cn

interface Shape { fun area(): Double }
来源：http://nh.yuexingan06.cn

[T16] Swift：Hello World
来源：http://bl.panjiajie.cn

print("Hello")
来源：http://re.lnxyls.cn

[T17] Swift：变量与常量
来源：http://ss.panjiajie.cn

var a = 1;  let b = 2
来源：http://hz.yuexingan06.cn

[T18] Swift：字符串插值
来源：http://fb.jianghongdianzi.cn

"值: \(b)"
来源：http://sd.huixinmuqiang.cn

[T19] Swift：可选绑定
来源：http://ld.bjjhwx.cn

if let n = opt { print(n) }
来源：http://oz.haigaiapp.cn

[T20] Swift：数组操作
来源：http://wa.asd995.cn

var a = [1, 2, 3];  a.append(4)
来源：http://dy.shtwfgs.cn

[T21] Swift：遍历
来源：http://sm.muxihuayi.cn

for x in a { print(x) }
来源：http://ds.jctech888.com.cn

[T22] Swift：字典
来源：http://cd.hahajie.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ks.huanxung.cn

[T23] Swift：函数
来源：http://jt.huixiangedu.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://rc.chemitech.net.cn

[T24] Swift：闭包
来源：http://lx.nicolike.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://eb.nszjky.cn

[T25] Swift：结构体
来源：http://ke.wgjwhj.cn

struct P { var x: Int }
来源：http://ml.asd995.cn

[T26] Swift：类与重写
来源：http://vr.huixinmuqiang.cn

class A: Base { override func f() {} }
来源：http://vv.shxzukj.cn

[T27] Swift：错误处理
来源：http://ke.shxzukj.cn

do { try f() } catch { print(error) }
来源：http://bp.muxihuayi.cn

[T28] Swift：枚举
来源：http://nw.yuexingan06.cn

enum Color { case red, green }
来源：http://ka.huixiangedu.cn

[T29] Swift：guard 提前返回
来源：http://sg.shxzskj.cn

guard let x = opt else { return }
来源：http://fw.chemitech.net.cn

[T30] Swift：协议
来源：http://ia.bookmarksfly.cn

protocol Shape { func area() -> Double }
来源：http://ma.newstarts.cn

[T31] Lua：Hello World
来源：http://nm.asd995.cn

print("Hello")
来源：http://mx.jianghongdianzi.cn

[T32] Lua：局部变量
来源：http://fk.wgjwhj.cn

local a = 1
来源：http://vm.jianghongdianzi.cn

[T33] Lua：表（数组）
来源：http://tw.nszjky.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://yj.hnjuh.cn

[T34] Lua：遍历表
来源：http://dx.asd995.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://pw.asd995.cn

[T35] Lua：字典表
来源：http://mt.panjiajie.cn

local d = { a = 1 };  d.b = 2
来源：http://wp.bjjhwx.cn

[T36] Lua：函数
来源：http://at.szxytkj.cn

function add(a, b) return a + b end
来源：http://xg.wgjwhj.cn

[T37] Lua：字符串拼接
来源：http://mk.panjiajie.cn

"a" .. "b"
来源：http://sz.shxzskj.cn

[T38] Lua：条件
来源：http://os.muxihuayi.cn

if x > 0 then print("正") end
来源：http://oj.asd995.cn

[T39] Lua：模式匹配
来源：http://ad.521024.cn

string.find(s, "%d+")
来源：http://sf.nszjky.cn

[T40] Lua：元表
来源：http://fd.lnxyls.cn

setmetatable({}, { __index = base })
来源：http://qc.nicolike.cn

[T41] Perl：Hello World
来源：http://we.shxzskj.cn

print "Hello\n";
来源：http://ly.yuntaijiaju.cn

[T42] Perl：变量类型
来源：http://ov.muxihuayi.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://jc.huixiangedu.cn

[T43] Perl：字符串插值
来源：http://si.shxzukj.cn

"值: $a"
来源：http://em.panjiajie.cn

[T44] Perl：条件
来源：http://si.shtwfgs.cn

if ($a > 0) { print "正"; }
来源：http://qn.shtwfgs.cn

[T45] Perl：数组遍历
来源：http://vw.hnjuh.cn

for my $x (@arr) { print $x; }
来源：http://fr.newstarts.cn

[T46] Perl：哈希操作
来源：http://gz.yuntaijiaju.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://sa.hnjuh.cn

[T47] Perl：正则捕获
来源：http://tm.nszjky.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://xf.bjjhwx.cn

[T48] Perl：正则替换
来源：http://sh.hahajie.cn

$s =~ s/old/new/g;
来源：http://ym.panjiajie.cn

[T49] Perl：函数
来源：http://za.muxihuayi.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://gb.hnjuh.cn

[T50] Perl：逐行读文件
来源：http://lo.newstarts.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://xa.panjiajie.cn

while (my $line = <$fh>) { print $line; }
来源：http://jn.bjjhwx.cn

[T51] Scala：Hello World
来源：http://ym.shxzukj.cn

println("Hello")
来源：http://ru.huanxung.cn

[T52] Scala：变量
来源：http://yw.asd995.cn

val a = 1;  var b = 2
来源：http://zt.newstarts.cn

[T53] Scala：字符串插值
来源：http://nv.muxihuayi.cn

s"值: $b"
来源：http://pa.lnxyls.cn

[T54] Scala：集合映射
来源：http://qa.lnxyls.cn

List(1, 2, 3).map(_ * 2)
来源：http://gm.muxihuayi.cn

[T55] Scala：集合过滤
来源：http://kc.nszjky.cn

List(1, 2, 3).filter(_ > 1)
来源：http://vi.bjjhwx.cn

[T56] Scala：样例类
来源：http://al.huixiangedu.cn

case class User(name: String, age: Int)
来源：http://ea.panjiajie.cn

[T57] Scala：模式匹配
来源：http://vc.colortex.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://zr.haigaiapp.cn

[T58] Scala：函数定义
来源：http://rn.lnxyls.cn

def add(a: Int, b: Int): Int = a + b
来源：http://gb.hahajie.cn

[T59] Scala：循环
来源：http://ks.haigaiapp.cn

for (i <- 1 to 10) println(i)
来源：http://ct.jctech888.com.cn

[T60] Scala：折叠
来源：http://kk.chemitech.net.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://jr.huixinmuqiang.cn

================================================================================
来源：http://li.bookmarksfly.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://lr.muxihuayi.cn

================================================================================
来源：http://cd.wgjwhj.cn

[U01] Py：创建虚拟环境
来源：http://ab.asd995.cn

python -m venv .venv && source .venv/bin/activate
来源：http://uc.huanxung.cn

[U02] Py：导出 / 安装依赖
来源：http://ah.shxzskj.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://la.haigaiapp.cn


<!-- 参考信息 -->