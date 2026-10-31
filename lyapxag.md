代发 wailian999

df -h;  du -sh *
来源：http://li.muxihuayi.cn

[R62] 找最占空间的文件
来源：http://lm.bjjhwx.cn

du -ah . | sort -rh | head -10
来源：http://he.bjjhwx.cn

[R63] 内存与进程
来源：http://rp.huixinmuqiang.cn

free -h;  ps aux | grep nginx
来源：http://be.lnxyls.cn

[R64] 结束进程
来源：http://ds.hnjuh.cn

kill -9 $(pgrep -f app.py)
来源：http://vj.bjjhwx.cn

[R65] 查看端口占用
来源：http://ym.chemitech.net.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://dl.huixiangedu.cn

[R66] 定时任务
来源：http://sy.haigaiapp.cn

crontab -e;  crontab -l
来源：http://bf.lnxyls.cn

[R67] 生成随机十六进制串
来源：http://tz.521024.cn

openssl rand -hex 16
来源：http://gm.jianghongdianzi.cn

[R68] 计算文件校验值
来源：http://zs.asd995.cn

sha256sum a.txt;  md5sum a.txt
来源：http://vh.szsharing.cn

[R69] 生成随机密码
来源：http://pj.gzmigu.cn

head -c 16 /dev/urandom | base64
来源：http://um.haigaiapp.cn

[R70] 时间戳与互转
来源：http://sd.bookmarksfly.cn

date +%s;  date -d @1700000000
来源：http://pd.bookmarksfly.cn

[R71] 日期格式化
来源：http://nq.shtwfgs.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ow.yuexingan06.cn

[R72] 等待端口就绪
来源：http://cm.huanxung.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ku.nszjky.cn

[R73] 分割大日志
来源：http://nx.huixiangedu.cn

split -l 1000 big.log part_
来源：http://dm.bookmarksfly.cn

[R74] 批量重命名
来源：http://zj.colortex.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://iv.521024.cn

[R75] 导出环境变量
来源：http://dq.nicolike.cn

export PATH="$HOME/bin:$PATH"
来源：http://fk.bjjhwx.cn

[R76] 使用临时文件
来源：http://wp.nicolike.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ka.jctech888.com.cn

[R77] 读取用户输入
来源：http://bn.521024.cn

read -rp "请输入: " ans
来源：http://ak.bjjhwx.cn

[R78] 交互式菜单
来源：http://gh.lnxyls.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://yp.hahajie.cn

[R79] 解析命令行选项
来源：http://fb.gzmigu.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ei.nszjky.cn

[R80] 查看脚本执行耗时
来源：http://dp.colortex.cn

time ./run.sh
来源：http://bo.shxzskj.cn

================================================================================
来源：http://wx.szsharing.cn

S. C / C++ 专题
来源：http://jh.chemitech.net.cn

================================================================================
来源：http://ud.yuexingan06.cn

[S01] C：Hello World
来源：http://re.hnjuh.cn

#include <stdio.h>
来源：http://jv.panjiajie.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://kf.jianghongdianzi.cn

[S02] C：变量与格式化输出
来源：http://gd.lnxyls.cn

int a = 10; printf("%d\n", a);
来源：http://gc.nicolike.cn

[S03] C：读入整数
来源：http://ot.asd995.cn

int x; scanf("%d", &x);
来源：http://xy.shtwfgs.cn

[S04] C：字符串复制
来源：http://nq.shtwfgs.cn

char dst[32]; strcpy(dst, "hi");
来源：http://qo.yuexingan06.cn

[S05] C：字符串长度
来源：http://pt.jianghongdianzi.cn

strlen(s)
来源：http://he.colortex.cn

[S06] C：字符串比较
来源：http://ow.nszjky.cn

strcmp(a, b) == 0
来源：http://rf.yuntaijiaju.cn

[S07] C：数组遍历求和
来源：http://it.shxzskj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://eb.nszjky.cn

[S08] C：动态内存分配与释放
来源：http://mf.bjjhwx.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qn.nicolike.cn

[S09] C：结构体定义与初始化
来源：http://tp.yuexingan06.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://uw.haigaiapp.cn

[S10] C：指针与解引用
来源：http://zi.colortex.cn

int *p = &a;  *p = 5;
来源：http://ao.yuexingan06.cn

[S11] C：逐行读文件
来源：http://ux.newstarts.cn

FILE *f = fopen("a.txt", "r");
来源：http://ks.nicolike.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://yb.szxytkj.cn

fclose(f);
来源：http://jf.shxzukj.cn

[S12] C：写文件
来源：http://fp.huixinmuqiang.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://oe.lnxyls.cn

[S13] C：宏定义
来源：http://aa.szxytkj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://at.521024.cn

[S14] C：枚举
来源：http://mp.huixiangedu.cn

enum Color { RED, GREEN, BLUE };
来源：http://km.shxzskj.cn

[S15] C：类型转换
来源：http://ny.huixinmuqiang.cn

(double) a / b
来源：http://nc.huixiangedu.cn

[S16] C：位操作置位
来源：http://hf.jianghongdianzi.cn

x |= (1 << 3);
来源：http://ii.hnjuh.cn

[S17] C：安全拼接字符串
来源：http://zm.newstarts.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wl.jctech888.com.cn

[S18] C：命令行参数
来源：http://lv.bjjhwx.cn

int main(int argc, char **argv)
来源：http://oc.newstarts.cn

[S19] C：快速排序
来源：http://bj.panjiajie.cn

qsort(a, n, sizeof(int), cmp);
来源：http://op.chemitech.net.cn

[S20] C：二分查找
来源：http://rv.asd995.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://pm.jctech888.com.cn

[S21] C：字符类别判断
来源：http://kd.jctech888.com.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://zm.nicolike.cn

[S22] C：字符串转数字
来源：http://qf.shxzskj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://vp.huanxung.cn

[S23] C：随机数
来源：http://uk.szsharing.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://xt.szxytkj.cn

[S24] C：获取本地时间
来源：http://zn.bookmarksfly.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ku.huixiangedu.cn

[S25] C：内存拷贝
来源：http://ys.jctech888.com.cn

memcpy(dst, src, n);
来源：http://pj.jctech888.com.cn

[S26] C：内存清零
来源：http://zm.nszjky.cn

memset(a, 0, sizeof a);
来源：http://ht.jctech888.com.cn

[S27] C：定义常量
来源：http://lp.asd995.cn

const double PI = 3.14159;
来源：http://ab.chemitech.net.cn

[S28] C：静态变量
来源：http://al.jctech888.com.cn

static int counter = 0;
来源：http://uo.lnxyls.cn

[S29] C：变参函数
来源：http://sr.huixinmuqiang.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://sl.nicolike.cn

[S30] C：头文件保护
来源：http://oz.hahajie.cn

#ifndef X_H
来源：http://ge.asd995.cn

#define X_H
来源：http://sa.bjjhwx.cn

#endif
来源：http://yo.jctech888.com.cn

[S31] C++：Hello World
来源：http://xn.newstarts.cn

#include <iostream>
来源：http://ob.nicolike.cn

int main() { std::cout << "Hello\n"; }
来源：http://ia.lnxyls.cn

[S32] C++：字符串
来源：http://tw.bjjhwx.cn

std::string s = "hi";  s += "!";
来源：http://xw.jianghongdianzi.cn

[S33] C++：vector 增删
来源：http://es.huanxung.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ew.bjjhwx.cn

[S34] C++：遍历 vector
来源：http://fs.nicolike.cn

for (auto &x : v) { std::cout << x; }
来源：http://kc.jctech888.com.cn

[S35] C++：map
来源：http://ja.jctech888.com.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://gn.yuexingan06.cn

[S36] C++：unordered_map
来源：http://kr.yuntaijiaju.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ot.asd995.cn

[S37] C++：set
来源：http://os.nszjky.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://hm.yuntaijiaju.cn

[S38] C++：排序
来源：http://um.szxytkj.cn

std::sort(v.begin(), v.end());
来源：http://kn.jianghongdianzi.cn

[S39] C++：自定义比较器排序
来源：http://tf.nszjky.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ly.bookmarksfly.cn

[S40] C++：查找元素
来源：http://rf.huixiangedu.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ja.521024.cn

[S41] C++：类与构造函数
来源：http://dt.9csxet.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://dp.asd995.cn

[S42] C++：继承与虚函数
来源：http://st.bookmarksfly.cn

class B : public Base { public: void f() override {} };
来源：http://jq.panjiajie.cn

[S43] C++：智能指针
来源：http://pd.haigaiapp.cn

auto p = std::make_unique<int>(5);
来源：http://wl.yuexingan06.cn

[S44] C++：引用传参
来源：http://kr.bjjhwx.cn

void inc(int &x) { ++x; }
来源：http://zl.hahajie.cn

[S45] C++：lambda
来源：http://of.9csxet.cn

auto add = [](int a, int b) { return a + b; };
来源：http://qg.hahajie.cn

[S46] C++：函数模板
来源：http://ap.shtwfgs.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://jm.szsharing.cn

[S47] C++：结构化绑定遍历
来源：http://py.huanxung.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ad.huanxung.cn

[S48] C++：逐行读文件
来源：http://oo.hnjuh.cn

std::ifstream in("a.txt");  std::string line;
来源：http://vt.bjjhwx.cn

while (std::getline(in, line)) { }
来源：http://tk.chemitech.net.cn

[S49] C++：写文件
来源：http://xv.nicolike.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://pl.9csxet.cn

[S50] C++：格式化数字
来源：http://xz.chemitech.net.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://cn.chemitech.net.cn

[S51] C++：显式类型转换
来源：http://bd.shtwfgs.cn

static_cast<double>(a) / b
来源：http://vs.panjiajie.cn

[S52] C++：const 与 noexcept
来源：http://sb.gzmigu.cn

int size() const noexcept { return n_; }
来源：http://ra.huixiangedu.cn

[S53] C++：移动语义
来源：http://wz.newstarts.cn

std::vector<int> w = std::move(v);
来源：http://wk.haigaiapp.cn

[S54] C++：异常处理
来源：http://qp.colortex.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://cn.hahajie.cn

[S55] C++：结构化绑定
来源：http://im.yuntaijiaju.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://qa.huixinmuqiang.cn

[S56] C++：optional
来源：http://nb.9csxet.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://dw.wgjwhj.cn

[S57] C++：编译期常量
来源：http://qt.shxzskj.cn

constexpr int N = 10;
来源：http://sb.huixinmuqiang.cn

[S58] C++：命名空间
来源：http://uc.newstarts.cn

namespace ns { int f() { return 1; } }
来源：http://at.521024.cn

[S59] C++：静态断言
来源：http://di.huixinmuqiang.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://vp.hahajie.cn

[S60] C++：遍历并删除元素
来源：http://cw.yuntaijiaju.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://vr.bookmarksfly.cn

================================================================================
来源：http://pv.huanxung.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://sd.wgjwhj.cn

================================================================================
来源：http://gv.shtwfgs.cn

[T01] Kotlin：Hello World
来源：http://zy.521024.cn

println("Hello")
来源：http://kj.hnjuh.cn

[T02] Kotlin：变量
来源：http://aw.newstarts.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://bv.shtwfgs.cn

[T03] Kotlin：字符串模板
来源：http://lj.huanxung.cn

"值: $b"
来源：http://eg.huanxung.cn

[T04] Kotlin：空安全
来源：http://sk.jianghongdianzi.cn

val n: String? = null;  n?.length
来源：http://yr.lnxyls.cn

[T05] Kotlin：when 表达式
来源：http://zq.haigaiapp.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://zm.wgjwhj.cn

[T06] Kotlin：集合映射
来源：http://by.jctech888.com.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://uh.panjiajie.cn

[T07] Kotlin：集合过滤
来源：http://ol.shxzukj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://qf.szxytkj.cn

[T08] Kotlin：数据类
来源：http://pr.huixinmuqiang.cn

data class User(val name: String, val age: Int)
来源：http://me.szxytkj.cn

[T09] Kotlin：扩展函数
来源：http://gv.huixiangedu.cn

fun String.exclaim() = this + "!"
来源：http://ri.9csxet.cn

[T10] Kotlin：默认参数
来源：http://wr.wgjwhj.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://cn.szxytkj.cn

[T11] Kotlin：协程
来源：http://gn.shxzukj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://mw.shtwfgs.cn

[T12] Kotlin：解构声明
来源：http://yp.shxzukj.cn

val (a, b) = Pair(1, 2)
来源：http://pn.lnxyls.cn

[T13] Kotlin：只读 Map
来源：http://kx.hahajie.cn

val m = mapOf("a" to 1)
来源：http://ug.bjjhwx.cn

[T14] Kotlin：循环
来源：http://pp.szxytkj.cn

for (i in 1..10) println(i)
来源：http://di.newstarts.cn

[T15] Kotlin：接口
来源：http://ax.nszjky.cn

interface Shape { fun area(): Double }
来源：http://zl.bookmarksfly.cn

[T16] Swift：Hello World
来源：http://fv.bookmarksfly.cn

print("Hello")
来源：http://jt.wgjwhj.cn

[T17] Swift：变量与常量
来源：http://qn.jianghongdianzi.cn

var a = 1;  let b = 2
来源：http://xd.wgjwhj.cn

[T18] Swift：字符串插值
来源：http://ab.huixiangedu.cn

"值: \(b)"
来源：http://lt.yuexingan06.cn

[T19] Swift：可选绑定
来源：http://ks.asd995.cn

if let n = opt { print(n) }
来源：http://hj.colortex.cn

[T20] Swift：数组操作
来源：http://az.hnjuh.cn

var a = [1, 2, 3];  a.append(4)
来源：http://jl.wgjwhj.cn

[T21] Swift：遍历
来源：http://wo.jianghongdianzi.cn

for x in a { print(x) }
来源：http://ao.huixinmuqiang.cn

[T22] Swift：字典
来源：http://gz.yuexingan06.cn

var d = ["a": 1];  d["b"] = 2
来源：http://cw.huixinmuqiang.cn

[T23] Swift：函数
来源：http://uv.muxihuayi.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ld.shxzukj.cn

[T24] Swift：闭包
来源：http://ze.jianghongdianzi.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ni.gzmigu.cn

[T25] Swift：结构体
来源：http://xv.colortex.cn

struct P { var x: Int }
来源：http://if.colortex.cn

[T26] Swift：类与重写
来源：http://jv.wgjwhj.cn

class A: Base { override func f() {} }
来源：http://vc.nszjky.cn

[T27] Swift：错误处理
来源：http://mi.yuexingan06.cn

do { try f() } catch { print(error) }
来源：http://js.haigaiapp.cn

[T28] Swift：枚举
来源：http://uy.jianghongdianzi.cn

enum Color { case red, green }
来源：http://ay.bjjhwx.cn

[T29] Swift：guard 提前返回
来源：http://gb.hahajie.cn

guard let x = opt else { return }
来源：http://gm.huanxung.cn

[T30] Swift：协议
来源：http://lr.haigaiapp.cn

protocol Shape { func area() -> Double }
来源：http://gx.panjiajie.cn

[T31] Lua：Hello World
来源：http://mc.gzmigu.cn

print("Hello")
来源：http://jz.szsharing.cn

[T32] Lua：局部变量
来源：http://jg.jianghongdianzi.cn

local a = 1
来源：http://kb.gzmigu.cn

[T33] Lua：表（数组）
来源：http://ww.nicolike.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://qm.chemitech.net.cn

[T34] Lua：遍历表
来源：http://pr.9csxet.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://nt.hahajie.cn

[T35] Lua：字典表
来源：http://md.yuexingan06.cn

local d = { a = 1 };  d.b = 2
来源：http://ow.yuexingan06.cn

[T36] Lua：函数
来源：http://jr.hnjuh.cn

function add(a, b) return a + b end
来源：http://fp.lnxyls.cn

[T37] Lua：字符串拼接
来源：http://ec.shxzskj.cn

"a" .. "b"
来源：http://sd.nicolike.cn

[T38] Lua：条件
来源：http://tl.huixiangedu.cn

if x > 0 then print("正") end
来源：http://pr.wgjwhj.cn

[T39] Lua：模式匹配
来源：http://pq.chemitech.net.cn

string.find(s, "%d+")
来源：http://wz.muxihuayi.cn

[T40] Lua：元表
来源：http://lv.chemitech.net.cn

setmetatable({}, { __index = base })
来源：http://uk.newstarts.cn

[T41] Perl：Hello World
来源：http://kw.nszjky.cn

print "Hello\n";
来源：http://ig.szsharing.cn

[T42] Perl：变量类型
来源：http://jn.muxihuayi.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://yx.bjjhwx.cn

[T43] Perl：字符串插值
来源：http://lk.521024.cn

"值: $a"
来源：http://nf.shtwfgs.cn

[T44] Perl：条件
来源：http://bu.shxzukj.cn

if ($a > 0) { print "正"; }
来源：http://uw.bookmarksfly.cn

[T45] Perl：数组遍历
来源：http://tr.shxzukj.cn

for my $x (@arr) { print $x; }
来源：http://or.jctech888.com.cn

[T46] Perl：哈希操作
来源：http://pq.gzmigu.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://rv.hahajie.cn

[T47] Perl：正则捕获
来源：http://rj.newstarts.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://fb.yuexingan06.cn

[T48] Perl：正则替换
来源：http://zq.lnxyls.cn

$s =~ s/old/new/g;
来源：http://jx.shtwfgs.cn

[T49] Perl：函数
来源：http://je.jctech888.com.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://qn.lnxyls.cn

[T50] Perl：逐行读文件
来源：http://kb.nicolike.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ci.521024.cn

while (my $line = <$fh>) { print $line; }
来源：http://zq.wgjwhj.cn

[T51] Scala：Hello World
来源：http://bd.lnxyls.cn

println("Hello")
来源：http://cu.panjiajie.cn

[T52] Scala：变量
来源：http://vx.hnjuh.cn

val a = 1;  var b = 2
来源：http://of.jctech888.com.cn

[T53] Scala：字符串插值
来源：http://fj.lnxyls.cn

s"值: $b"
来源：http://ab.huanxung.cn

[T54] Scala：集合映射
来源：http://iz.hahajie.cn

List(1, 2, 3).map(_ * 2)
来源：http://uv.jctech888.com.cn

[T55] Scala：集合过滤
来源：http://io.chemitech.net.cn

List(1, 2, 3).filter(_ > 1)
来源：http://ya.shtwfgs.cn

[T56] Scala：样例类
来源：http://ao.haigaiapp.cn

case class User(name: String, age: Int)
来源：http://pg.bjjhwx.cn

[T57] Scala：模式匹配
来源：http://oj.jianghongdianzi.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://qq.chemitech.net.cn

[T58] Scala：函数定义
来源：http://bz.muxihuayi.cn

def add(a: Int, b: Int): Int = a + b
来源：http://dc.shxzukj.cn

[T59] Scala：循环
来源：http://lx.gzmigu.cn

for (i <- 1 to 10) println(i)
来源：http://lg.wgjwhj.cn

[T60] Scala：折叠
来源：http://po.colortex.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://qd.yuntaijiaju.cn

================================================================================
来源：http://il.huixinmuqiang.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://nv.szsharing.cn

================================================================================
来源：http://rn.huixinmuqiang.cn

[U01] Py：创建虚拟环境
来源：http://we.szsharing.cn

python -m venv .venv && source .venv/bin/activate
来源：http://xe.huanxung.cn

[U02] Py：导出 / 安装依赖
来源：http://yf.yuntaijiaju.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://hf.jctech888.com.cn


<!-- 参考信息 -->