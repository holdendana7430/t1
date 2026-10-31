代发 wailian999

openssl rand -hex 16
来源：http://ht.shxzukj.cn

[R68] 计算文件校验值
来源：http://lk.wgjwhj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ky.muxihuayi.cn

[R69] 生成随机密码
来源：http://xn.asd995.cn

head -c 16 /dev/urandom | base64
来源：http://zn.chemitech.net.cn

[R70] 时间戳与互转
来源：http://kc.muxihuayi.cn

date +%s;  date -d @1700000000
来源：http://or.shtwfgs.cn

[R71] 日期格式化
来源：http://wg.szxytkj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://fz.hnjuh.cn

[R72] 等待端口就绪
来源：http://gb.panjiajie.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://qh.hahajie.cn

[R73] 分割大日志
来源：http://ky.shxzskj.cn

split -l 1000 big.log part_
来源：http://ad.nszjky.cn

[R74] 批量重命名
来源：http://kz.colortex.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ig.gzmigu.cn

[R75] 导出环境变量
来源：http://gr.bjjhwx.cn

export PATH="$HOME/bin:$PATH"
来源：http://gz.huixinmuqiang.cn

[R76] 使用临时文件
来源：http://ns.colortex.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://zm.shtwfgs.cn

[R77] 读取用户输入
来源：http://sk.nicolike.cn

read -rp "请输入: " ans
来源：http://ap.muxihuayi.cn

[R78] 交互式菜单
来源：http://et.szsharing.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://zf.yuexingan06.cn

[R79] 解析命令行选项
来源：http://kp.gzmigu.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mt.jctech888.com.cn

[R80] 查看脚本执行耗时
来源：http://cd.bjjhwx.cn

time ./run.sh
来源：http://vx.shtwfgs.cn

================================================================================
来源：http://ol.huixiangedu.cn

S. C / C++ 专题
来源：http://ss.huanxung.cn

================================================================================
来源：http://qb.haigaiapp.cn

[S01] C：Hello World
来源：http://di.hahajie.cn

#include <stdio.h>
来源：http://hs.huixinmuqiang.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://jw.shxzskj.cn

[S02] C：变量与格式化输出
来源：http://mn.asd995.cn

int a = 10; printf("%d\n", a);
来源：http://ol.jctech888.com.cn

[S03] C：读入整数
来源：http://ry.panjiajie.cn

int x; scanf("%d", &x);
来源：http://yw.lnxyls.cn

[S04] C：字符串复制
来源：http://kp.yuntaijiaju.cn

char dst[32]; strcpy(dst, "hi");
来源：http://im.shtwfgs.cn

[S05] C：字符串长度
来源：http://iy.huixiangedu.cn

strlen(s)
来源：http://go.hahajie.cn

[S06] C：字符串比较
来源：http://mw.9csxet.cn

strcmp(a, b) == 0
来源：http://fm.gzmigu.cn

[S07] C：数组遍历求和
来源：http://wn.huixiangedu.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://dd.gzmigu.cn

[S08] C：动态内存分配与释放
来源：http://tx.shtwfgs.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://sq.bookmarksfly.cn

[S09] C：结构体定义与初始化
来源：http://wf.shtwfgs.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://cc.chemitech.net.cn

[S10] C：指针与解引用
来源：http://qz.bookmarksfly.cn

int *p = &a;  *p = 5;
来源：http://dk.bjjhwx.cn

[S11] C：逐行读文件
来源：http://yq.521024.cn

FILE *f = fopen("a.txt", "r");
来源：http://wk.hnjuh.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://tk.huanxung.cn

fclose(f);
来源：http://us.bookmarksfly.cn

[S12] C：写文件
来源：http://ca.gzmigu.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://fp.gzmigu.cn

[S13] C：宏定义
来源：http://pr.huixinmuqiang.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ap.nszjky.cn

[S14] C：枚举
来源：http://mp.colortex.cn

enum Color { RED, GREEN, BLUE };
来源：http://rb.huixinmuqiang.cn

[S15] C：类型转换
来源：http://dn.huixinmuqiang.cn

(double) a / b
来源：http://ok.lnxyls.cn

[S16] C：位操作置位
来源：http://jw.szsharing.cn

x |= (1 << 3);
来源：http://ax.huixiangedu.cn

[S17] C：安全拼接字符串
来源：http://mk.shtwfgs.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://qs.lnxyls.cn

[S18] C：命令行参数
来源：http://nv.muxihuayi.cn

int main(int argc, char **argv)
来源：http://vf.panjiajie.cn

[S19] C：快速排序
来源：http://bb.jianghongdianzi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://li.huanxung.cn

[S20] C：二分查找
来源：http://qw.chemitech.net.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://nw.yuntaijiaju.cn

[S21] C：字符类别判断
来源：http://tu.bjjhwx.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://rs.521024.cn

[S22] C：字符串转数字
来源：http://ma.521024.cn

atoi("42");  strtod("3.14", NULL);
来源：http://so.panjiajie.cn

[S23] C：随机数
来源：http://nf.shxzskj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://zq.hnjuh.cn

[S24] C：获取本地时间
来源：http://uu.haigaiapp.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://pm.hahajie.cn

[S25] C：内存拷贝
来源：http://mb.wgjwhj.cn

memcpy(dst, src, n);
来源：http://qq.yuntaijiaju.cn

[S26] C：内存清零
来源：http://vd.newstarts.cn

memset(a, 0, sizeof a);
来源：http://lm.lnxyls.cn

[S27] C：定义常量
来源：http://bp.yuexingan06.cn

const double PI = 3.14159;
来源：http://az.colortex.cn

[S28] C：静态变量
来源：http://fs.huanxung.cn

static int counter = 0;
来源：http://rk.nicolike.cn

[S29] C：变参函数
来源：http://fj.lnxyls.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://nq.yuexingan06.cn

[S30] C：头文件保护
来源：http://wj.yuexingan06.cn

#ifndef X_H
来源：http://bc.jctech888.com.cn

#define X_H
来源：http://uf.nicolike.cn

#endif
来源：http://sb.hahajie.cn

[S31] C++：Hello World
来源：http://ty.wgjwhj.cn

#include <iostream>
来源：http://wx.jctech888.com.cn

int main() { std::cout << "Hello\n"; }
来源：http://nx.huanxung.cn

[S32] C++：字符串
来源：http://ue.colortex.cn

std::string s = "hi";  s += "!";
来源：http://ac.huixiangedu.cn

[S33] C++：vector 增删
来源：http://pj.haigaiapp.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qx.colortex.cn

[S34] C++：遍历 vector
来源：http://bq.colortex.cn

for (auto &x : v) { std::cout << x; }
来源：http://pr.szsharing.cn

[S35] C++：map
来源：http://ya.muxihuayi.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://vk.wgjwhj.cn

[S36] C++：unordered_map
来源：http://dc.jianghongdianzi.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://jo.9csxet.cn

[S37] C++：set
来源：http://ho.huanxung.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://fa.bookmarksfly.cn

[S38] C++：排序
来源：http://te.panjiajie.cn

std::sort(v.begin(), v.end());
来源：http://vk.bjjhwx.cn

[S39] C++：自定义比较器排序
来源：http://cp.lnxyls.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://tf.huixinmuqiang.cn

[S40] C++：查找元素
来源：http://vr.hahajie.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://zw.szxytkj.cn

[S41] C++：类与构造函数
来源：http://kh.nszjky.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://vj.shxzskj.cn

[S42] C++：继承与虚函数
来源：http://mq.shtwfgs.cn

class B : public Base { public: void f() override {} };
来源：http://fa.nszjky.cn

[S43] C++：智能指针
来源：http://mv.yuexingan06.cn

auto p = std::make_unique<int>(5);
来源：http://ej.lnxyls.cn

[S44] C++：引用传参
来源：http://fl.hahajie.cn

void inc(int &x) { ++x; }
来源：http://nz.yuexingan06.cn

[S45] C++：lambda
来源：http://th.hahajie.cn

auto add = [](int a, int b) { return a + b; };
来源：http://os.shtwfgs.cn

[S46] C++：函数模板
来源：http://sm.yuexingan06.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://qc.panjiajie.cn

[S47] C++：结构化绑定遍历
来源：http://sw.panjiajie.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://pz.521024.cn

[S48] C++：逐行读文件
来源：http://mm.521024.cn

std::ifstream in("a.txt");  std::string line;
来源：http://bm.huanxung.cn

while (std::getline(in, line)) { }
来源：http://vt.nszjky.cn

[S49] C++：写文件
来源：http://mu.bookmarksfly.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ck.shtwfgs.cn

[S50] C++：格式化数字
来源：http://by.colortex.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://fw.chemitech.net.cn

[S51] C++：显式类型转换
来源：http://in.gzmigu.cn

static_cast<double>(a) / b
来源：http://wh.gzmigu.cn

[S52] C++：const 与 noexcept
来源：http://sy.asd995.cn

int size() const noexcept { return n_; }
来源：http://gl.bookmarksfly.cn

[S53] C++：移动语义
来源：http://hb.nszjky.cn

std::vector<int> w = std::move(v);
来源：http://iu.szsharing.cn

[S54] C++：异常处理
来源：http://oa.shtwfgs.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://qb.9csxet.cn

[S55] C++：结构化绑定
来源：http://wm.newstarts.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ps.jianghongdianzi.cn

[S56] C++：optional
来源：http://bs.shxzukj.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ue.jianghongdianzi.cn

[S57] C++：编译期常量
来源：http://xd.hnjuh.cn

constexpr int N = 10;
来源：http://nk.521024.cn

[S58] C++：命名空间
来源：http://fg.bookmarksfly.cn

namespace ns { int f() { return 1; } }
来源：http://da.shxzukj.cn

[S59] C++：静态断言
来源：http://us.yuexingan06.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://uc.shxzskj.cn

[S60] C++：遍历并删除元素
来源：http://aw.hnjuh.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://vc.jianghongdianzi.cn

================================================================================
来源：http://dl.panjiajie.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ts.shxzskj.cn

================================================================================
来源：http://mz.huixinmuqiang.cn

[T01] Kotlin：Hello World
来源：http://ys.hnjuh.cn

println("Hello")
来源：http://jc.wgjwhj.cn

[T02] Kotlin：变量
来源：http://az.szsharing.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://dn.yuntaijiaju.cn

[T03] Kotlin：字符串模板
来源：http://ls.szxytkj.cn

"值: $b"
来源：http://tt.bookmarksfly.cn

[T04] Kotlin：空安全
来源：http://sj.521024.cn

val n: String? = null;  n?.length
来源：http://yi.jianghongdianzi.cn

[T05] Kotlin：when 表达式
来源：http://xp.asd995.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.shxzukj.cn

[T06] Kotlin：集合映射
来源：http://hl.jctech888.com.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ot.colortex.cn

[T07] Kotlin：集合过滤
来源：http://iz.lnxyls.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://xl.lnxyls.cn

[T08] Kotlin：数据类
来源：http://xu.huixiangedu.cn

data class User(val name: String, val age: Int)
来源：http://wi.9csxet.cn

[T09] Kotlin：扩展函数
来源：http://am.szxytkj.cn

fun String.exclaim() = this + "!"
来源：http://zc.huixiangedu.cn

[T10] Kotlin：默认参数
来源：http://kn.yuexingan06.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://fk.hnjuh.cn

[T11] Kotlin：协程
来源：http://an.jctech888.com.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://jk.huixiangedu.cn

[T12] Kotlin：解构声明
来源：http://bu.huixiangedu.cn

val (a, b) = Pair(1, 2)
来源：http://ob.szsharing.cn

[T13] Kotlin：只读 Map
来源：http://ge.huixinmuqiang.cn

val m = mapOf("a" to 1)
来源：http://wb.chemitech.net.cn

[T14] Kotlin：循环
来源：http://ak.jianghongdianzi.cn

for (i in 1..10) println(i)
来源：http://ge.szsharing.cn

[T15] Kotlin：接口
来源：http://bi.haigaiapp.cn

interface Shape { fun area(): Double }
来源：http://mo.muxihuayi.cn

[T16] Swift：Hello World
来源：http://bm.huixiangedu.cn

print("Hello")
来源：http://ty.huixinmuqiang.cn

[T17] Swift：变量与常量
来源：http://tx.yuexingan06.cn

var a = 1;  let b = 2
来源：http://is.gzmigu.cn

[T18] Swift：字符串插值
来源：http://vg.shtwfgs.cn

"值: \(b)"
来源：http://ao.chemitech.net.cn

[T19] Swift：可选绑定
来源：http://ko.haigaiapp.cn

if let n = opt { print(n) }
来源：http://ud.9csxet.cn

[T20] Swift：数组操作
来源：http://hz.hnjuh.cn

var a = [1, 2, 3];  a.append(4)
来源：http://bl.panjiajie.cn

[T21] Swift：遍历
来源：http://wj.muxihuayi.cn

for x in a { print(x) }
来源：http://vr.newstarts.cn

[T22] Swift：字典
来源：http://kg.bookmarksfly.cn

var d = ["a": 1];  d["b"] = 2
来源：http://rq.hahajie.cn

[T23] Swift：函数
来源：http://tk.huixinmuqiang.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://we.szsharing.cn

[T24] Swift：闭包
来源：http://yg.szxytkj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ey.szsharing.cn

[T25] Swift：结构体
来源：http://bv.haigaiapp.cn

struct P { var x: Int }
来源：http://jh.szsharing.cn

[T26] Swift：类与重写
来源：http://uw.chemitech.net.cn

class A: Base { override func f() {} }
来源：http://dx.huixinmuqiang.cn

[T27] Swift：错误处理
来源：http://jp.chemitech.net.cn

do { try f() } catch { print(error) }
来源：http://rv.chemitech.net.cn

[T28] Swift：枚举
来源：http://rv.huixiangedu.cn

enum Color { case red, green }
来源：http://qy.hahajie.cn

[T29] Swift：guard 提前返回
来源：http://uf.9csxet.cn

guard let x = opt else { return }
来源：http://js.huixiangedu.cn

[T30] Swift：协议
来源：http://lo.nicolike.cn

protocol Shape { func area() -> Double }
来源：http://pv.nicolike.cn

[T31] Lua：Hello World
来源：http://jc.asd995.cn

print("Hello")
来源：http://ni.haigaiapp.cn

[T32] Lua：局部变量
来源：http://jt.521024.cn

local a = 1
来源：http://tz.panjiajie.cn

[T33] Lua：表（数组）
来源：http://kj.nszjky.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://xd.shtwfgs.cn

[T34] Lua：遍历表
来源：http://ei.huixiangedu.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://cw.newstarts.cn

[T35] Lua：字典表
来源：http://zg.hnjuh.cn

local d = { a = 1 };  d.b = 2
来源：http://xo.newstarts.cn

[T36] Lua：函数
来源：http://mv.gzmigu.cn

function add(a, b) return a + b end
来源：http://ht.shtwfgs.cn

[T37] Lua：字符串拼接
来源：http://ql.shtwfgs.cn

"a" .. "b"
来源：http://xa.yuntaijiaju.cn

[T38] Lua：条件
来源：http://wj.newstarts.cn

if x > 0 then print("正") end
来源：http://vk.hahajie.cn

[T39] Lua：模式匹配
来源：http://gm.huixinmuqiang.cn

string.find(s, "%d+")
来源：http://bo.haigaiapp.cn

[T40] Lua：元表
来源：http://ok.muxihuayi.cn

setmetatable({}, { __index = base })
来源：http://tx.yuexingan06.cn

[T41] Perl：Hello World
来源：http://nb.nszjky.cn

print "Hello\n";
来源：http://ps.panjiajie.cn

[T42] Perl：变量类型
来源：http://ad.huixiangedu.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ww.szsharing.cn

[T43] Perl：字符串插值
来源：http://kz.nszjky.cn

"值: $a"
来源：http://tw.szsharing.cn

[T44] Perl：条件
来源：http://xh.nszjky.cn

if ($a > 0) { print "正"; }
来源：http://jn.521024.cn

[T45] Perl：数组遍历
来源：http://sl.szxytkj.cn

for my $x (@arr) { print $x; }
来源：http://lz.muxihuayi.cn

[T46] Perl：哈希操作
来源：http://of.panjiajie.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ae.yuexingan06.cn

[T47] Perl：正则捕获
来源：http://rt.shxzskj.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ru.colortex.cn

[T48] Perl：正则替换
来源：http://zv.jctech888.com.cn

$s =~ s/old/new/g;
来源：http://tu.colortex.cn

[T49] Perl：函数
来源：http://ca.shxzskj.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ot.gzmigu.cn

[T50] Perl：逐行读文件
来源：http://rk.shxzskj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://bp.shxzukj.cn

while (my $line = <$fh>) { print $line; }
来源：http://tf.yuntaijiaju.cn

[T51] Scala：Hello World
来源：http://vg.hnjuh.cn

println("Hello")
来源：http://wu.colortex.cn

[T52] Scala：变量
来源：http://hh.szsharing.cn

val a = 1;  var b = 2
来源：http://hr.szsharing.cn

[T53] Scala：字符串插值
来源：http://da.nicolike.cn

s"值: $b"
来源：http://zt.huanxung.cn

[T54] Scala：集合映射
来源：http://zy.szxytkj.cn

List(1, 2, 3).map(_ * 2)
来源：http://fq.huanxung.cn

[T55] Scala：集合过滤
来源：http://eq.hahajie.cn

List(1, 2, 3).filter(_ > 1)
来源：http://js.jianghongdianzi.cn

[T56] Scala：样例类
来源：http://bv.szxytkj.cn

case class User(name: String, age: Int)
来源：http://xx.jianghongdianzi.cn

[T57] Scala：模式匹配
来源：http://kt.hnjuh.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://ea.nicolike.cn

[T58] Scala：函数定义
来源：http://me.9csxet.cn

def add(a: Int, b: Int): Int = a + b
来源：http://re.huixiangedu.cn

[T59] Scala：循环
来源：http://ag.521024.cn

for (i <- 1 to 10) println(i)
来源：http://ov.521024.cn

[T60] Scala：折叠
来源：http://bq.gzmigu.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://vz.huanxung.cn

================================================================================
来源：http://bn.wgjwhj.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://ic.hahajie.cn

================================================================================
来源：http://tl.nszjky.cn

[U01] Py：创建虚拟环境
来源：http://ko.yuexingan06.cn

python -m venv .venv && source .venv/bin/activate
来源：http://ie.hahajie.cn

[U02] Py：导出 / 安装依赖
来源：http://gs.lnxyls.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://un.huanxung.cn

[U03] Py：加载 .env 配置
来源：http://xf.hnjuh.cn

from dotenv import load_dotenv; load_dotenv()
来源：http://jn.huanxung.cn

[U04] Py：变量调试打印
来源：http://tf.hahajie.cn

print(f"{x=}")            # 输出 x=值，Python 3.8+
来源：http://ev.bookmarksfly.cn

[U05] Py：列表去重且保序
来源：http://mq.muxihuayi.cn

list(dict.fromkeys(arr))
来源：http://dz.newstarts.cn

[U06] Py：合并两个字典
来源：http://ji.chemitech.net.cn

{**a, **b}
来源：http://dj.colortex.cn

[U07] Py：反转字典键值
来源：http://xt.jianghongdianzi.cn

{v: k for k, v in d.items()}
来源：http://cw.shxzukj.cn

[U08] Py：展平二维列表
来源：http://ib.huanxung.cn

[y for x in nested for y in x]
来源：http://ik.hahajie.cn


<!-- 参考信息 -->