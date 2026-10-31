代发 wailian999

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vj.hahajie.cn

[R60] 只看 HTTP 状态码
来源：http://fl.muxihuayi.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://sl.hahajie.cn

[R61] 磁盘占用
来源：http://de.colortex.cn

df -h;  du -sh *
来源：http://ol.hahajie.cn

[R62] 找最占空间的文件
来源：http://ia.gzmigu.cn

du -ah . | sort -rh | head -10
来源：http://gq.9csxet.cn

[R63] 内存与进程
来源：http://vb.muxihuayi.cn

free -h;  ps aux | grep nginx
来源：http://mo.colortex.cn

[R64] 结束进程
来源：http://pd.bjjhwx.cn

kill -9 $(pgrep -f app.py)
来源：http://xp.newstarts.cn

[R65] 查看端口占用
来源：http://cm.wgjwhj.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ro.shtwfgs.cn

[R66] 定时任务
来源：http://ia.hahajie.cn

crontab -e;  crontab -l
来源：http://tr.wgjwhj.cn

[R67] 生成随机十六进制串
来源：http://he.nicolike.cn

openssl rand -hex 16
来源：http://sf.haigaiapp.cn

[R68] 计算文件校验值
来源：http://jm.hnjuh.cn

sha256sum a.txt;  md5sum a.txt
来源：http://at.521024.cn

[R69] 生成随机密码
来源：http://rj.yuntaijiaju.cn

head -c 16 /dev/urandom | base64
来源：http://xy.asd995.cn

[R70] 时间戳与互转
来源：http://uy.521024.cn

date +%s;  date -d @1700000000
来源：http://qy.nszjky.cn

[R71] 日期格式化
来源：http://kb.wgjwhj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://xz.nszjky.cn

[R72] 等待端口就绪
来源：http://ff.521024.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://kg.bookmarksfly.cn

[R73] 分割大日志
来源：http://oy.shtwfgs.cn

split -l 1000 big.log part_
来源：http://ql.asd995.cn

[R74] 批量重命名
来源：http://tl.szsharing.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://jl.panjiajie.cn

[R75] 导出环境变量
来源：http://tl.huanxung.cn

export PATH="$HOME/bin:$PATH"
来源：http://dt.szsharing.cn

[R76] 使用临时文件
来源：http://qn.jianghongdianzi.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://xa.newstarts.cn

[R77] 读取用户输入
来源：http://ix.shtwfgs.cn

read -rp "请输入: " ans
来源：http://ht.muxihuayi.cn

[R78] 交互式菜单
来源：http://yt.huanxung.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://nr.jianghongdianzi.cn

[R79] 解析命令行选项
来源：http://je.haigaiapp.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://yi.hnjuh.cn

[R80] 查看脚本执行耗时
来源：http://vh.bookmarksfly.cn

time ./run.sh
来源：http://bq.yuexingan06.cn

================================================================================
来源：http://vz.lnxyls.cn

S. C / C++ 专题
来源：http://fo.yuntaijiaju.cn

================================================================================
来源：http://bg.huixinmuqiang.cn

[S01] C：Hello World
来源：http://od.huixinmuqiang.cn

#include <stdio.h>
来源：http://pu.muxihuayi.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://om.lnxyls.cn

[S02] C：变量与格式化输出
来源：http://zf.hahajie.cn

int a = 10; printf("%d\n", a);
来源：http://ts.nicolike.cn

[S03] C：读入整数
来源：http://aa.hnjuh.cn

int x; scanf("%d", &x);
来源：http://ua.asd995.cn

[S04] C：字符串复制
来源：http://vw.9csxet.cn

char dst[32]; strcpy(dst, "hi");
来源：http://kv.szsharing.cn

[S05] C：字符串长度
来源：http://zt.haigaiapp.cn

strlen(s)
来源：http://sp.jianghongdianzi.cn

[S06] C：字符串比较
来源：http://ac.gzmigu.cn

strcmp(a, b) == 0
来源：http://rv.yuexingan06.cn

[S07] C：数组遍历求和
来源：http://gs.newstarts.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ke.shtwfgs.cn

[S08] C：动态内存分配与释放
来源：http://gm.hahajie.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://dc.huixinmuqiang.cn

[S09] C：结构体定义与初始化
来源：http://ui.colortex.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://uf.bookmarksfly.cn

[S10] C：指针与解引用
来源：http://zy.szsharing.cn

int *p = &a;  *p = 5;
来源：http://vx.hahajie.cn

[S11] C：逐行读文件
来源：http://rh.shxzskj.cn

FILE *f = fopen("a.txt", "r");
来源：http://nq.bookmarksfly.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://va.jctech888.com.cn

fclose(f);
来源：http://oy.newstarts.cn

[S12] C：写文件
来源：http://td.jctech888.com.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ue.huixinmuqiang.cn

[S13] C：宏定义
来源：http://qm.szxytkj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://io.bjjhwx.cn

[S14] C：枚举
来源：http://fr.colortex.cn

enum Color { RED, GREEN, BLUE };
来源：http://lc.bookmarksfly.cn

[S15] C：类型转换
来源：http://ae.haigaiapp.cn

(double) a / b
来源：http://zs.wgjwhj.cn

[S16] C：位操作置位
来源：http://vi.bjjhwx.cn

x |= (1 << 3);
来源：http://mg.bjjhwx.cn

[S17] C：安全拼接字符串
来源：http://cm.shxzukj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://qh.wgjwhj.cn

[S18] C：命令行参数
来源：http://zu.newstarts.cn

int main(int argc, char **argv)
来源：http://kh.hnjuh.cn

[S19] C：快速排序
来源：http://fw.bookmarksfly.cn

qsort(a, n, sizeof(int), cmp);
来源：http://zy.nicolike.cn

[S20] C：二分查找
来源：http://ih.chemitech.net.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://yy.wgjwhj.cn

[S21] C：字符类别判断
来源：http://qd.huixiangedu.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://rf.chemitech.net.cn

[S22] C：字符串转数字
来源：http://yi.yuntaijiaju.cn

atoi("42");  strtod("3.14", NULL);
来源：http://fr.bookmarksfly.cn

[S23] C：随机数
来源：http://cm.panjiajie.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://bs.nszjky.cn

[S24] C：获取本地时间
来源：http://yx.newstarts.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hd.bjjhwx.cn

[S25] C：内存拷贝
来源：http://gl.yuexingan06.cn

memcpy(dst, src, n);
来源：http://wp.9csxet.cn

[S26] C：内存清零
来源：http://xx.huixinmuqiang.cn

memset(a, 0, sizeof a);
来源：http://at.colortex.cn

[S27] C：定义常量
来源：http://yx.521024.cn

const double PI = 3.14159;
来源：http://tj.yuntaijiaju.cn

[S28] C：静态变量
来源：http://jv.yuexingan06.cn

static int counter = 0;
来源：http://af.lnxyls.cn

[S29] C：变参函数
来源：http://sj.nszjky.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://bq.gzmigu.cn

[S30] C：头文件保护
来源：http://qf.9csxet.cn

#ifndef X_H
来源：http://fk.nicolike.cn

#define X_H
来源：http://hw.wgjwhj.cn

#endif
来源：http://nf.yuntaijiaju.cn

[S31] C++：Hello World
来源：http://or.panjiajie.cn

#include <iostream>
来源：http://uc.lnxyls.cn

int main() { std::cout << "Hello\n"; }
来源：http://qn.yuntaijiaju.cn

[S32] C++：字符串
来源：http://lx.huixinmuqiang.cn

std::string s = "hi";  s += "!";
来源：http://oc.muxihuayi.cn

[S33] C++：vector 增删
来源：http://cq.colortex.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://jn.nszjky.cn

[S34] C++：遍历 vector
来源：http://cr.9csxet.cn

for (auto &x : v) { std::cout << x; }
来源：http://tk.shxzskj.cn

[S35] C++：map
来源：http://xz.huanxung.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://dy.huanxung.cn

[S36] C++：unordered_map
来源：http://vw.szsharing.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://em.yuntaijiaju.cn

[S37] C++：set
来源：http://yi.huanxung.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://lj.bjjhwx.cn

[S38] C++：排序
来源：http://da.bookmarksfly.cn

std::sort(v.begin(), v.end());
来源：http://ms.huixiangedu.cn

[S39] C++：自定义比较器排序
来源：http://su.wgjwhj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://aj.newstarts.cn

[S40] C++：查找元素
来源：http://ae.panjiajie.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://pd.wgjwhj.cn

[S41] C++：类与构造函数
来源：http://mi.muxihuayi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://pp.hnjuh.cn

[S42] C++：继承与虚函数
来源：http://ve.jctech888.com.cn

class B : public Base { public: void f() override {} };
来源：http://gp.haigaiapp.cn

[S43] C++：智能指针
来源：http://ai.newstarts.cn

auto p = std::make_unique<int>(5);
来源：http://dq.jianghongdianzi.cn

[S44] C++：引用传参
来源：http://ae.521024.cn

void inc(int &x) { ++x; }
来源：http://in.gzmigu.cn

[S45] C++：lambda
来源：http://lp.panjiajie.cn

auto add = [](int a, int b) { return a + b; };
来源：http://wu.shtwfgs.cn

[S46] C++：函数模板
来源：http://tv.hahajie.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://jg.huixiangedu.cn

[S47] C++：结构化绑定遍历
来源：http://jv.newstarts.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://hi.colortex.cn

[S48] C++：逐行读文件
来源：http://by.chemitech.net.cn

std::ifstream in("a.txt");  std::string line;
来源：http://kh.jctech888.com.cn

while (std::getline(in, line)) { }
来源：http://fv.yuexingan06.cn

[S49] C++：写文件
来源：http://fm.jctech888.com.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://bi.hnjuh.cn

[S50] C++：格式化数字
来源：http://nl.jctech888.com.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://jk.yuntaijiaju.cn

[S51] C++：显式类型转换
来源：http://ps.shxzskj.cn

static_cast<double>(a) / b
来源：http://sd.bookmarksfly.cn

[S52] C++：const 与 noexcept
来源：http://zo.shxzskj.cn

int size() const noexcept { return n_; }
来源：http://df.bjjhwx.cn

[S53] C++：移动语义
来源：http://do.shtwfgs.cn

std::vector<int> w = std::move(v);
来源：http://nk.9csxet.cn

[S54] C++：异常处理
来源：http://fs.huixinmuqiang.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://oo.nszjky.cn

[S55] C++：结构化绑定
来源：http://dg.lnxyls.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://di.huanxung.cn

[S56] C++：optional
来源：http://rt.szsharing.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://qm.szxytkj.cn

[S57] C++：编译期常量
来源：http://bh.jctech888.com.cn

constexpr int N = 10;
来源：http://nh.yuntaijiaju.cn

[S58] C++：命名空间
来源：http://vw.nicolike.cn

namespace ns { int f() { return 1; } }
来源：http://cf.shtwfgs.cn

[S59] C++：静态断言
来源：http://uq.bookmarksfly.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://gf.bookmarksfly.cn

[S60] C++：遍历并删除元素
来源：http://qf.shxzskj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://km.hahajie.cn

================================================================================
来源：http://ci.521024.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://zf.shxzukj.cn

================================================================================
来源：http://hk.huixinmuqiang.cn

[T01] Kotlin：Hello World
来源：http://xy.wgjwhj.cn

println("Hello")
来源：http://rk.huanxung.cn

[T02] Kotlin：变量
来源：http://yj.9csxet.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://so.bjjhwx.cn

[T03] Kotlin：字符串模板
来源：http://ps.yuntaijiaju.cn

"值: $b"
来源：http://uk.shtwfgs.cn

[T04] Kotlin：空安全
来源：http://yu.jianghongdianzi.cn

val n: String? = null;  n?.length
来源：http://oh.panjiajie.cn

[T05] Kotlin：when 表达式
来源：http://pg.lnxyls.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hz.nicolike.cn

[T06] Kotlin：集合映射
来源：http://gb.nszjky.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://mb.asd995.cn

[T07] Kotlin：集合过滤
来源：http://xw.gzmigu.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://lk.521024.cn

[T08] Kotlin：数据类
来源：http://ox.yuntaijiaju.cn

data class User(val name: String, val age: Int)
来源：http://or.shxzskj.cn

[T09] Kotlin：扩展函数
来源：http://sq.haigaiapp.cn

fun String.exclaim() = this + "!"
来源：http://ta.haigaiapp.cn

[T10] Kotlin：默认参数
来源：http://vn.yuntaijiaju.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://we.szxytkj.cn

[T11] Kotlin：协程
来源：http://tr.521024.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://wp.hnjuh.cn

[T12] Kotlin：解构声明
来源：http://po.shxzskj.cn

val (a, b) = Pair(1, 2)
来源：http://zv.haigaiapp.cn

[T13] Kotlin：只读 Map
来源：http://nj.newstarts.cn

val m = mapOf("a" to 1)
来源：http://hp.yuexingan06.cn

[T14] Kotlin：循环
来源：http://vp.shtwfgs.cn

for (i in 1..10) println(i)
来源：http://ub.hnjuh.cn

[T15] Kotlin：接口
来源：http://xd.yuexingan06.cn

interface Shape { fun area(): Double }
来源：http://lk.asd995.cn

[T16] Swift：Hello World
来源：http://bh.nicolike.cn

print("Hello")
来源：http://ya.asd995.cn

[T17] Swift：变量与常量
来源：http://xl.huixiangedu.cn

var a = 1;  let b = 2
来源：http://vo.bjjhwx.cn

[T18] Swift：字符串插值
来源：http://lo.muxihuayi.cn

"值: \(b)"
来源：http://np.nicolike.cn

[T19] Swift：可选绑定
来源：http://hg.9csxet.cn

if let n = opt { print(n) }
来源：http://ab.chemitech.net.cn

[T20] Swift：数组操作
来源：http://lk.nszjky.cn

var a = [1, 2, 3];  a.append(4)
来源：http://oa.yuexingan06.cn

[T21] Swift：遍历
来源：http://jd.yuntaijiaju.cn

for x in a { print(x) }
来源：http://sf.asd995.cn

[T22] Swift：字典
来源：http://va.muxihuayi.cn

var d = ["a": 1];  d["b"] = 2
来源：http://bn.9csxet.cn

[T23] Swift：函数
来源：http://xt.yuntaijiaju.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://pp.bjjhwx.cn

[T24] Swift：闭包
来源：http://aq.lnxyls.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://uv.yuntaijiaju.cn

[T25] Swift：结构体
来源：http://mr.huanxung.cn

struct P { var x: Int }
来源：http://ex.shtwfgs.cn

[T26] Swift：类与重写
来源：http://oo.hnjuh.cn

class A: Base { override func f() {} }
来源：http://sq.panjiajie.cn

[T27] Swift：错误处理
来源：http://hh.nszjky.cn

do { try f() } catch { print(error) }
来源：http://oz.panjiajie.cn

[T28] Swift：枚举
来源：http://aq.chemitech.net.cn

enum Color { case red, green }
来源：http://fm.yuexingan06.cn

[T29] Swift：guard 提前返回
来源：http://dk.huanxung.cn

guard let x = opt else { return }
来源：http://uh.shxzukj.cn

[T30] Swift：协议
来源：http://oh.bookmarksfly.cn

protocol Shape { func area() -> Double }
来源：http://dc.shxzukj.cn

[T31] Lua：Hello World
来源：http://tb.nszjky.cn

print("Hello")
来源：http://wp.huanxung.cn

[T32] Lua：局部变量
来源：http://fp.521024.cn

local a = 1
来源：http://mb.lnxyls.cn

[T33] Lua：表（数组）
来源：http://wc.shtwfgs.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://lz.521024.cn

[T34] Lua：遍历表
来源：http://pc.shxzukj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://dq.hnjuh.cn

[T35] Lua：字典表
来源：http://ib.huixinmuqiang.cn

local d = { a = 1 };  d.b = 2
来源：http://vu.huixinmuqiang.cn

[T36] Lua：函数
来源：http://kp.shxzskj.cn

function add(a, b) return a + b end
来源：http://ej.yuexingan06.cn

[T37] Lua：字符串拼接
来源：http://ir.bjjhwx.cn

"a" .. "b"
来源：http://hm.gzmigu.cn

[T38] Lua：条件
来源：http://ux.521024.cn

if x > 0 then print("正") end
来源：http://ya.muxihuayi.cn

[T39] Lua：模式匹配
来源：http://bi.9csxet.cn

string.find(s, "%d+")
来源：http://cv.asd995.cn

[T40] Lua：元表
来源：http://ub.shtwfgs.cn

setmetatable({}, { __index = base })
来源：http://nb.9csxet.cn

[T41] Perl：Hello World
来源：http://ur.panjiajie.cn

print "Hello\n";
来源：http://ms.shtwfgs.cn

[T42] Perl：变量类型
来源：http://vv.colortex.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://aw.yuexingan06.cn

[T43] Perl：字符串插值
来源：http://ho.asd995.cn

"值: $a"
来源：http://zx.lnxyls.cn

[T44] Perl：条件
来源：http://yg.jctech888.com.cn

if ($a > 0) { print "正"; }
来源：http://jl.hnjuh.cn

[T45] Perl：数组遍历
来源：http://al.shxzskj.cn

for my $x (@arr) { print $x; }
来源：http://ab.yuexingan06.cn

[T46] Perl：哈希操作
来源：http://kl.huixiangedu.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://kp.asd995.cn

[T47] Perl：正则捕获
来源：http://tm.jctech888.com.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://bj.hahajie.cn

[T48] Perl：正则替换
来源：http://vp.newstarts.cn

$s =~ s/old/new/g;
来源：http://ev.asd995.cn

[T49] Perl：函数
来源：http://zz.jianghongdianzi.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://jq.hahajie.cn

[T50] Perl：逐行读文件
来源：http://dl.bookmarksfly.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://kj.hnjuh.cn

while (my $line = <$fh>) { print $line; }
来源：http://qm.shxzukj.cn

[T51] Scala：Hello World
来源：http://cv.jianghongdianzi.cn

println("Hello")
来源：http://bl.yuexingan06.cn

[T52] Scala：变量
来源：http://ee.muxihuayi.cn

val a = 1;  var b = 2
来源：http://ff.huanxung.cn

[T53] Scala：字符串插值
来源：http://bv.lnxyls.cn

s"值: $b"
来源：http://xl.yuntaijiaju.cn

[T54] Scala：集合映射
来源：http://kf.jianghongdianzi.cn

List(1, 2, 3).map(_ * 2)
来源：http://ka.szxytkj.cn

[T55] Scala：集合过滤
来源：http://qv.9csxet.cn

List(1, 2, 3).filter(_ > 1)
来源：http://wx.shxzukj.cn

[T56] Scala：样例类
来源：http://tx.bookmarksfly.cn

case class User(name: String, age: Int)
来源：http://kv.panjiajie.cn

[T57] Scala：模式匹配
来源：http://zd.szxytkj.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://sl.hahajie.cn

[T58] Scala：函数定义
来源：http://na.bookmarksfly.cn

def add(a: Int, b: Int): Int = a + b
来源：http://xf.bookmarksfly.cn

[T59] Scala：循环
来源：http://wh.huanxung.cn

for (i <- 1 to 10) println(i)
来源：http://bj.huixiangedu.cn

[T60] Scala：折叠
来源：http://mt.nszjky.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ht.bookmarksfly.cn

================================================================================
来源：http://zf.nicolike.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://dt.yuntaijiaju.cn

================================================================================
来源：http://tr.huixinmuqiang.cn


<!-- 参考信息 -->