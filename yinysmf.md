代发 wailian999

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://bf.521024.cn

[R60] 只看 HTTP 状态码
来源：http://ir.newstarts.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ur.shxzukj.cn

[R61] 磁盘占用
来源：http://vl.jianghongdianzi.cn

df -h;  du -sh *
来源：http://id.newstarts.cn

[R62] 找最占空间的文件
来源：http://ew.shxzskj.cn

du -ah . | sort -rh | head -10
来源：http://jl.nicolike.cn

[R63] 内存与进程
来源：http://su.szxytkj.cn

free -h;  ps aux | grep nginx
来源：http://qx.newstarts.cn

[R64] 结束进程
来源：http://rr.shxzskj.cn

kill -9 $(pgrep -f app.py)
来源：http://co.panjiajie.cn

[R65] 查看端口占用
来源：http://ft.lnxyls.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://df.newstarts.cn

[R66] 定时任务
来源：http://xv.shtwfgs.cn

crontab -e;  crontab -l
来源：http://fj.521024.cn

[R67] 生成随机十六进制串
来源：http://si.jctech888.com.cn

openssl rand -hex 16
来源：http://sz.bookmarksfly.cn

[R68] 计算文件校验值
来源：http://my.asd995.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ga.521024.cn

[R69] 生成随机密码
来源：http://iz.newstarts.cn

head -c 16 /dev/urandom | base64
来源：http://of.wgjwhj.cn

[R70] 时间戳与互转
来源：http://hk.muxihuayi.cn

date +%s;  date -d @1700000000
来源：http://fu.shtwfgs.cn

[R71] 日期格式化
来源：http://sg.newstarts.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://px.nszjky.cn

[R72] 等待端口就绪
来源：http://pd.haigaiapp.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://mx.yuexingan06.cn

[R73] 分割大日志
来源：http://ta.nszjky.cn

split -l 1000 big.log part_
来源：http://oa.jctech888.com.cn

[R74] 批量重命名
来源：http://ii.huixinmuqiang.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://sw.nszjky.cn

[R75] 导出环境变量
来源：http://ml.yuntaijiaju.cn

export PATH="$HOME/bin:$PATH"
来源：http://sp.szxytkj.cn

[R76] 使用临时文件
来源：http://eh.jctech888.com.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://rk.panjiajie.cn

[R77] 读取用户输入
来源：http://et.huixiangedu.cn

read -rp "请输入: " ans
来源：http://ph.bjjhwx.cn

[R78] 交互式菜单
来源：http://iy.chemitech.net.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://el.haigaiapp.cn

[R79] 解析命令行选项
来源：http://ej.521024.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://bz.bjjhwx.cn

[R80] 查看脚本执行耗时
来源：http://kk.lnxyls.cn

time ./run.sh
来源：http://no.wgjwhj.cn

================================================================================
来源：http://pd.huixiangedu.cn

S. C / C++ 专题
来源：http://vi.yuntaijiaju.cn

================================================================================
来源：http://va.bookmarksfly.cn

[S01] C：Hello World
来源：http://mo.haigaiapp.cn

#include <stdio.h>
来源：http://ik.gzmigu.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://em.haigaiapp.cn

[S02] C：变量与格式化输出
来源：http://ys.yuexingan06.cn

int a = 10; printf("%d\n", a);
来源：http://tm.asd995.cn

[S03] C：读入整数
来源：http://ga.hnjuh.cn

int x; scanf("%d", &x);
来源：http://jp.shtwfgs.cn

[S04] C：字符串复制
来源：http://wp.hahajie.cn

char dst[32]; strcpy(dst, "hi");
来源：http://hs.wgjwhj.cn

[S05] C：字符串长度
来源：http://sz.hnjuh.cn

strlen(s)
来源：http://el.chemitech.net.cn

[S06] C：字符串比较
来源：http://ja.haigaiapp.cn

strcmp(a, b) == 0
来源：http://sc.jianghongdianzi.cn

[S07] C：数组遍历求和
来源：http://qm.9csxet.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://gn.yuexingan06.cn

[S08] C：动态内存分配与释放
来源：http://fn.lnxyls.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ol.nszjky.cn

[S09] C：结构体定义与初始化
来源：http://ht.yuexingan06.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://rr.shtwfgs.cn

[S10] C：指针与解引用
来源：http://so.muxihuayi.cn

int *p = &a;  *p = 5;
来源：http://xg.nszjky.cn

[S11] C：逐行读文件
来源：http://bm.shxzukj.cn

FILE *f = fopen("a.txt", "r");
来源：http://vk.colortex.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://xv.521024.cn

fclose(f);
来源：http://qd.huanxung.cn

[S12] C：写文件
来源：http://wa.wgjwhj.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://fv.panjiajie.cn

[S13] C：宏定义
来源：http://nf.huixiangedu.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://yp.nicolike.cn

[S14] C：枚举
来源：http://gf.muxihuayi.cn

enum Color { RED, GREEN, BLUE };
来源：http://dx.panjiajie.cn

[S15] C：类型转换
来源：http://dv.hnjuh.cn

(double) a / b
来源：http://ls.jctech888.com.cn

[S16] C：位操作置位
来源：http://my.shtwfgs.cn

x |= (1 << 3);
来源：http://tj.szsharing.cn

[S17] C：安全拼接字符串
来源：http://gc.chemitech.net.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://hi.shxzukj.cn

[S18] C：命令行参数
来源：http://dd.yuexingan06.cn

int main(int argc, char **argv)
来源：http://ta.9csxet.cn

[S19] C：快速排序
来源：http://td.hahajie.cn

qsort(a, n, sizeof(int), cmp);
来源：http://da.gzmigu.cn

[S20] C：二分查找
来源：http://ql.huixinmuqiang.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://dk.huanxung.cn

[S21] C：字符类别判断
来源：http://do.chemitech.net.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xw.shxzskj.cn

[S22] C：字符串转数字
来源：http://lf.newstarts.cn

atoi("42");  strtod("3.14", NULL);
来源：http://cg.shtwfgs.cn

[S23] C：随机数
来源：http://ju.yuntaijiaju.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://wi.shxzskj.cn

[S24] C：获取本地时间
来源：http://zu.hnjuh.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://pu.yuntaijiaju.cn

[S25] C：内存拷贝
来源：http://gp.hahajie.cn

memcpy(dst, src, n);
来源：http://xh.haigaiapp.cn

[S26] C：内存清零
来源：http://tq.9csxet.cn

memset(a, 0, sizeof a);
来源：http://nt.asd995.cn

[S27] C：定义常量
来源：http://vw.huixinmuqiang.cn

const double PI = 3.14159;
来源：http://uo.nicolike.cn

[S28] C：静态变量
来源：http://bv.muxihuayi.cn

static int counter = 0;
来源：http://nz.bjjhwx.cn

[S29] C：变参函数
来源：http://wd.haigaiapp.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://kq.wgjwhj.cn

[S30] C：头文件保护
来源：http://gr.shxzukj.cn

#ifndef X_H
来源：http://vi.huanxung.cn

#define X_H
来源：http://uv.lnxyls.cn

#endif
来源：http://mu.huixiangedu.cn

[S31] C++：Hello World
来源：http://bp.shtwfgs.cn

#include <iostream>
来源：http://am.hahajie.cn

int main() { std::cout << "Hello\n"; }
来源：http://xm.gzmigu.cn

[S32] C++：字符串
来源：http://by.yuexingan06.cn

std::string s = "hi";  s += "!";
来源：http://dm.newstarts.cn

[S33] C++：vector 增删
来源：http://ik.yuexingan06.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ic.521024.cn

[S34] C++：遍历 vector
来源：http://yp.huanxung.cn

for (auto &x : v) { std::cout << x; }
来源：http://jw.jctech888.com.cn

[S35] C++：map
来源：http://ry.muxihuayi.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://lg.yuntaijiaju.cn

[S36] C++：unordered_map
来源：http://ef.nszjky.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://fq.muxihuayi.cn

[S37] C++：set
来源：http://ok.yuexingan06.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ro.nicolike.cn

[S38] C++：排序
来源：http://iu.hnjuh.cn

std::sort(v.begin(), v.end());
来源：http://vx.jianghongdianzi.cn

[S39] C++：自定义比较器排序
来源：http://mq.nszjky.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://md.yuexingan06.cn

[S40] C++：查找元素
来源：http://si.bjjhwx.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://zr.colortex.cn

[S41] C++：类与构造函数
来源：http://tu.jianghongdianzi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://up.newstarts.cn

[S42] C++：继承与虚函数
来源：http://uw.wgjwhj.cn

class B : public Base { public: void f() override {} };
来源：http://wc.huixinmuqiang.cn

[S43] C++：智能指针
来源：http://cb.hahajie.cn

auto p = std::make_unique<int>(5);
来源：http://gm.huanxung.cn

[S44] C++：引用传参
来源：http://af.lnxyls.cn

void inc(int &x) { ++x; }
来源：http://zd.jianghongdianzi.cn

[S45] C++：lambda
来源：http://le.9csxet.cn

auto add = [](int a, int b) { return a + b; };
来源：http://eh.nszjky.cn

[S46] C++：函数模板
来源：http://tr.yuexingan06.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ja.9csxet.cn

[S47] C++：结构化绑定遍历
来源：http://yz.shxzukj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://wp.muxihuayi.cn

[S48] C++：逐行读文件
来源：http://zu.yuexingan06.cn

std::ifstream in("a.txt");  std::string line;
来源：http://gw.yuntaijiaju.cn

while (std::getline(in, line)) { }
来源：http://ir.hahajie.cn

[S49] C++：写文件
来源：http://wx.newstarts.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://qt.huixinmuqiang.cn

[S50] C++：格式化数字
来源：http://cm.jctech888.com.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ho.haigaiapp.cn

[S51] C++：显式类型转换
来源：http://om.hahajie.cn

static_cast<double>(a) / b
来源：http://nt.colortex.cn

[S52] C++：const 与 noexcept
来源：http://lo.9csxet.cn

int size() const noexcept { return n_; }
来源：http://cj.haigaiapp.cn

[S53] C++：移动语义
来源：http://ut.asd995.cn

std::vector<int> w = std::move(v);
来源：http://lj.asd995.cn

[S54] C++：异常处理
来源：http://ni.chemitech.net.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://bt.szxytkj.cn

[S55] C++：结构化绑定
来源：http://ug.bjjhwx.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://vv.nicolike.cn

[S56] C++：optional
来源：http://tt.shtwfgs.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://vn.huanxung.cn

[S57] C++：编译期常量
来源：http://cy.521024.cn

constexpr int N = 10;
来源：http://ge.szsharing.cn

[S58] C++：命名空间
来源：http://rq.szxytkj.cn

namespace ns { int f() { return 1; } }
来源：http://zc.huixiangedu.cn

[S59] C++：静态断言
来源：http://zz.haigaiapp.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ys.panjiajie.cn

[S60] C++：遍历并删除元素
来源：http://il.yuntaijiaju.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://hi.shxzukj.cn

================================================================================
来源：http://yh.lnxyls.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hp.bjjhwx.cn

================================================================================
来源：http://fc.wgjwhj.cn

[T01] Kotlin：Hello World
来源：http://ur.chemitech.net.cn

println("Hello")
来源：http://xu.huixinmuqiang.cn

[T02] Kotlin：变量
来源：http://ck.521024.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wn.newstarts.cn

[T03] Kotlin：字符串模板
来源：http://lq.huixiangedu.cn

"值: $b"
来源：http://cv.newstarts.cn

[T04] Kotlin：空安全
来源：http://nd.nicolike.cn

val n: String? = null;  n?.length
来源：http://eh.szsharing.cn

[T05] Kotlin：when 表达式
来源：http://il.bjjhwx.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://fo.haigaiapp.cn

[T06] Kotlin：集合映射
来源：http://va.hahajie.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://hd.lnxyls.cn

[T07] Kotlin：集合过滤
来源：http://yx.szxytkj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://es.colortex.cn

[T08] Kotlin：数据类
来源：http://ak.szxytkj.cn

data class User(val name: String, val age: Int)
来源：http://hh.muxihuayi.cn

[T09] Kotlin：扩展函数
来源：http://tf.9csxet.cn

fun String.exclaim() = this + "!"
来源：http://bx.lnxyls.cn

[T10] Kotlin：默认参数
来源：http://vt.huanxung.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://qs.lnxyls.cn

[T11] Kotlin：协程
来源：http://by.jctech888.com.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://iu.hnjuh.cn

[T12] Kotlin：解构声明
来源：http://gp.shxzskj.cn

val (a, b) = Pair(1, 2)
来源：http://af.nicolike.cn

[T13] Kotlin：只读 Map
来源：http://wf.bjjhwx.cn

val m = mapOf("a" to 1)
来源：http://je.hahajie.cn

[T14] Kotlin：循环
来源：http://wm.lnxyls.cn

for (i in 1..10) println(i)
来源：http://il.shtwfgs.cn

[T15] Kotlin：接口
来源：http://tf.huanxung.cn

interface Shape { fun area(): Double }
来源：http://ne.newstarts.cn

[T16] Swift：Hello World
来源：http://xs.jctech888.com.cn

print("Hello")
来源：http://ch.szxytkj.cn

[T17] Swift：变量与常量
来源：http://xt.521024.cn

var a = 1;  let b = 2
来源：http://qy.wgjwhj.cn

[T18] Swift：字符串插值
来源：http://jr.colortex.cn

"值: \(b)"
来源：http://ry.bjjhwx.cn

[T19] Swift：可选绑定
来源：http://nw.shtwfgs.cn

if let n = opt { print(n) }
来源：http://bn.hahajie.cn

[T20] Swift：数组操作
来源：http://fq.muxihuayi.cn

var a = [1, 2, 3];  a.append(4)
来源：http://mi.bjjhwx.cn

[T21] Swift：遍历
来源：http://if.hahajie.cn

for x in a { print(x) }
来源：http://lq.shxzukj.cn

[T22] Swift：字典
来源：http://ux.szsharing.cn

var d = ["a": 1];  d["b"] = 2
来源：http://kg.gzmigu.cn

[T23] Swift：函数
来源：http://rf.bookmarksfly.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://py.huixinmuqiang.cn

[T24] Swift：闭包
来源：http://au.huixinmuqiang.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ms.nszjky.cn

[T25] Swift：结构体
来源：http://fd.muxihuayi.cn

struct P { var x: Int }
来源：http://aj.newstarts.cn

[T26] Swift：类与重写
来源：http://ow.9csxet.cn

class A: Base { override func f() {} }
来源：http://kd.hahajie.cn

[T27] Swift：错误处理
来源：http://wc.jctech888.com.cn

do { try f() } catch { print(error) }
来源：http://dd.szxytkj.cn

[T28] Swift：枚举
来源：http://yp.521024.cn

enum Color { case red, green }
来源：http://bo.huanxung.cn

[T29] Swift：guard 提前返回
来源：http://bx.asd995.cn

guard let x = opt else { return }
来源：http://jj.asd995.cn

[T30] Swift：协议
来源：http://pv.chemitech.net.cn

protocol Shape { func area() -> Double }
来源：http://td.yuntaijiaju.cn

[T31] Lua：Hello World
来源：http://gd.hahajie.cn

print("Hello")
来源：http://if.huixinmuqiang.cn

[T32] Lua：局部变量
来源：http://zu.jctech888.com.cn

local a = 1
来源：http://yl.szxytkj.cn

[T33] Lua：表（数组）
来源：http://it.hnjuh.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://gt.hahajie.cn

[T34] Lua：遍历表
来源：http://xm.nszjky.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://dp.huixiangedu.cn

[T35] Lua：字典表
来源：http://lh.jianghongdianzi.cn

local d = { a = 1 };  d.b = 2
来源：http://fm.muxihuayi.cn

[T36] Lua：函数
来源：http://op.9csxet.cn

function add(a, b) return a + b end
来源：http://ht.huanxung.cn

[T37] Lua：字符串拼接
来源：http://eu.lnxyls.cn

"a" .. "b"
来源：http://tz.lnxyls.cn

[T38] Lua：条件
来源：http://ug.yuntaijiaju.cn

if x > 0 then print("正") end
来源：http://iv.colortex.cn

[T39] Lua：模式匹配
来源：http://do.shtwfgs.cn

string.find(s, "%d+")
来源：http://dh.jctech888.com.cn

[T40] Lua：元表
来源：http://jd.huanxung.cn

setmetatable({}, { __index = base })
来源：http://ex.huanxung.cn

[T41] Perl：Hello World
来源：http://vn.jianghongdianzi.cn

print "Hello\n";
来源：http://ky.muxihuayi.cn

[T42] Perl：变量类型
来源：http://se.521024.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ac.shxzskj.cn

[T43] Perl：字符串插值
来源：http://kg.yuexingan06.cn

"值: $a"
来源：http://yn.szxytkj.cn

[T44] Perl：条件
来源：http://ym.huanxung.cn

if ($a > 0) { print "正"; }
来源：http://ly.huanxung.cn

[T45] Perl：数组遍历
来源：http://vk.wgjwhj.cn

for my $x (@arr) { print $x; }
来源：http://wq.shtwfgs.cn

[T46] Perl：哈希操作
来源：http://pa.asd995.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ns.haigaiapp.cn

[T47] Perl：正则捕获
来源：http://uc.huixinmuqiang.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://jr.gzmigu.cn

[T48] Perl：正则替换
来源：http://tg.nicolike.cn

$s =~ s/old/new/g;
来源：http://bz.panjiajie.cn

[T49] Perl：函数
来源：http://ub.bookmarksfly.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://am.shtwfgs.cn

[T50] Perl：逐行读文件
来源：http://jr.521024.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://jg.yuntaijiaju.cn

while (my $line = <$fh>) { print $line; }
来源：http://lg.nszjky.cn

[T51] Scala：Hello World
来源：http://wm.nicolike.cn

println("Hello")
来源：http://je.bookmarksfly.cn

[T52] Scala：变量
来源：http://ge.521024.cn

val a = 1;  var b = 2
来源：http://kw.jianghongdianzi.cn

[T53] Scala：字符串插值
来源：http://eb.huanxung.cn

s"值: $b"
来源：http://ay.shtwfgs.cn

[T54] Scala：集合映射
来源：http://qy.yuexingan06.cn

List(1, 2, 3).map(_ * 2)
来源：http://ed.jctech888.com.cn

[T55] Scala：集合过滤
来源：http://ap.jianghongdianzi.cn

List(1, 2, 3).filter(_ > 1)
来源：http://db.haigaiapp.cn

[T56] Scala：样例类
来源：http://bq.shxzskj.cn

case class User(name: String, age: Int)
来源：http://mh.colortex.cn

[T57] Scala：模式匹配
来源：http://ky.chemitech.net.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://dg.hahajie.cn

[T58] Scala：函数定义
来源：http://qi.shtwfgs.cn

def add(a: Int, b: Int): Int = a + b
来源：http://be.huixiangedu.cn

[T59] Scala：循环
来源：http://uy.shtwfgs.cn

for (i <- 1 to 10) println(i)
来源：http://wd.yuntaijiaju.cn

[T60] Scala：折叠
来源：http://rh.huixinmuqiang.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://ny.wgjwhj.cn

================================================================================
来源：http://fg.yuexingan06.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://de.521024.cn

================================================================================
来源：http://oy.szsharing.cn


<!-- 参考信息 -->