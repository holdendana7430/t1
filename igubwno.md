代发 wailian999

ssh user@host 'uptime'
来源：http://uv.bookmarksfly.cn

[R58] 下载文件
来源：http://yp.szsharing.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://mx.shtwfgs.cn

[R59] 发 POST JSON
来源：http://lp.colortex.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://uo.szsharing.cn

[R60] 只看 HTTP 状态码
来源：http://vg.yuexingan06.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://jf.bjjhwx.cn

[R61] 磁盘占用
来源：http://ba.shxzskj.cn

df -h;  du -sh *
来源：http://bj.colortex.cn

[R62] 找最占空间的文件
来源：http://lg.shxzskj.cn

du -ah . | sort -rh | head -10
来源：http://gb.hahajie.cn

[R63] 内存与进程
来源：http://py.szsharing.cn

free -h;  ps aux | grep nginx
来源：http://kh.shtwfgs.cn

[R64] 结束进程
来源：http://ui.521024.cn

kill -9 $(pgrep -f app.py)
来源：http://mx.bjjhwx.cn

[R65] 查看端口占用
来源：http://uw.asd995.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://vi.shtwfgs.cn

[R66] 定时任务
来源：http://lk.hahajie.cn

crontab -e;  crontab -l
来源：http://wk.szxytkj.cn

[R67] 生成随机十六进制串
来源：http://gf.chemitech.net.cn

openssl rand -hex 16
来源：http://ou.jianghongdianzi.cn

[R68] 计算文件校验值
来源：http://zm.muxihuayi.cn

sha256sum a.txt;  md5sum a.txt
来源：http://di.gzmigu.cn

[R69] 生成随机密码
来源：http://yj.jctech888.com.cn

head -c 16 /dev/urandom | base64
来源：http://ul.nszjky.cn

[R70] 时间戳与互转
来源：http://tc.shxzskj.cn

date +%s;  date -d @1700000000
来源：http://sl.chemitech.net.cn

[R71] 日期格式化
来源：http://rb.nicolike.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://yj.yuexingan06.cn

[R72] 等待端口就绪
来源：http://rr.asd995.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://cp.yuexingan06.cn

[R73] 分割大日志
来源：http://ph.yuexingan06.cn

split -l 1000 big.log part_
来源：http://vd.nicolike.cn

[R74] 批量重命名
来源：http://gt.huixinmuqiang.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ym.hahajie.cn

[R75] 导出环境变量
来源：http://sl.jctech888.com.cn

export PATH="$HOME/bin:$PATH"
来源：http://nm.asd995.cn

[R76] 使用临时文件
来源：http://oe.9csxet.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://hw.muxihuayi.cn

[R77] 读取用户输入
来源：http://un.newstarts.cn

read -rp "请输入: " ans
来源：http://df.nicolike.cn

[R78] 交互式菜单
来源：http://cd.colortex.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://dt.chemitech.net.cn

[R79] 解析命令行选项
来源：http://yi.haigaiapp.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://be.huixiangedu.cn

[R80] 查看脚本执行耗时
来源：http://kp.haigaiapp.cn

time ./run.sh
来源：http://zw.bjjhwx.cn

================================================================================
来源：http://bb.muxihuayi.cn

S. C / C++ 专题
来源：http://bh.panjiajie.cn

================================================================================
来源：http://yl.9csxet.cn

[S01] C：Hello World
来源：http://uv.haigaiapp.cn

#include <stdio.h>
来源：http://ba.nszjky.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://qg.muxihuayi.cn

[S02] C：变量与格式化输出
来源：http://oa.asd995.cn

int a = 10; printf("%d\n", a);
来源：http://fw.lnxyls.cn

[S03] C：读入整数
来源：http://hl.szsharing.cn

int x; scanf("%d", &x);
来源：http://fs.lnxyls.cn

[S04] C：字符串复制
来源：http://bs.haigaiapp.cn

char dst[32]; strcpy(dst, "hi");
来源：http://lg.szsharing.cn

[S05] C：字符串长度
来源：http://yb.9csxet.cn

strlen(s)
来源：http://bv.jianghongdianzi.cn

[S06] C：字符串比较
来源：http://sa.shtwfgs.cn

strcmp(a, b) == 0
来源：http://ax.wgjwhj.cn

[S07] C：数组遍历求和
来源：http://he.shxzukj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wp.szsharing.cn

[S08] C：动态内存分配与释放
来源：http://ve.newstarts.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ku.nicolike.cn

[S09] C：结构体定义与初始化
来源：http://dc.hahajie.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ai.shxzskj.cn

[S10] C：指针与解引用
来源：http://mq.yuntaijiaju.cn

int *p = &a;  *p = 5;
来源：http://nm.newstarts.cn

[S11] C：逐行读文件
来源：http://yg.hnjuh.cn

FILE *f = fopen("a.txt", "r");
来源：http://ie.9csxet.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://cx.bookmarksfly.cn

fclose(f);
来源：http://qg.jianghongdianzi.cn

[S12] C：写文件
来源：http://hi.huixinmuqiang.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://qb.yuexingan06.cn

[S13] C：宏定义
来源：http://yx.haigaiapp.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://yv.jianghongdianzi.cn

[S14] C：枚举
来源：http://dk.gzmigu.cn

enum Color { RED, GREEN, BLUE };
来源：http://lw.huixinmuqiang.cn

[S15] C：类型转换
来源：http://aa.shxzukj.cn

(double) a / b
来源：http://bf.jctech888.com.cn

[S16] C：位操作置位
来源：http://os.shxzukj.cn

x |= (1 << 3);
来源：http://fl.asd995.cn

[S17] C：安全拼接字符串
来源：http://ow.asd995.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://wy.bookmarksfly.cn

[S18] C：命令行参数
来源：http://fg.hahajie.cn

int main(int argc, char **argv)
来源：http://nt.shxzukj.cn

[S19] C：快速排序
来源：http://tc.shxzukj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://zl.gzmigu.cn

[S20] C：二分查找
来源：http://un.yuexingan06.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://rc.shxzukj.cn

[S21] C：字符类别判断
来源：http://gs.jctech888.com.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://mb.gzmigu.cn

[S22] C：字符串转数字
来源：http://yj.asd995.cn

atoi("42");  strtod("3.14", NULL);
来源：http://so.muxihuayi.cn

[S23] C：随机数
来源：http://za.colortex.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ux.szxytkj.cn

[S24] C：获取本地时间
来源：http://ob.jctech888.com.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ns.hahajie.cn

[S25] C：内存拷贝
来源：http://pj.jctech888.com.cn

memcpy(dst, src, n);
来源：http://bv.yuexingan06.cn

[S26] C：内存清零
来源：http://za.newstarts.cn

memset(a, 0, sizeof a);
来源：http://rz.huixiangedu.cn

[S27] C：定义常量
来源：http://gz.hnjuh.cn

const double PI = 3.14159;
来源：http://jy.jctech888.com.cn

[S28] C：静态变量
来源：http://dy.jctech888.com.cn

static int counter = 0;
来源：http://gq.hahajie.cn

[S29] C：变参函数
来源：http://ao.9csxet.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://od.szsharing.cn

[S30] C：头文件保护
来源：http://mb.wgjwhj.cn

#ifndef X_H
来源：http://el.muxihuayi.cn

#define X_H
来源：http://ak.jctech888.com.cn

#endif
来源：http://bx.jianghongdianzi.cn

[S31] C++：Hello World
来源：http://ig.521024.cn

#include <iostream>
来源：http://bk.9csxet.cn

int main() { std::cout << "Hello\n"; }
来源：http://pc.chemitech.net.cn

[S32] C++：字符串
来源：http://zb.9csxet.cn

std::string s = "hi";  s += "!";
来源：http://yc.szsharing.cn

[S33] C++：vector 增删
来源：http://uj.jianghongdianzi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://lb.asd995.cn

[S34] C++：遍历 vector
来源：http://ii.panjiajie.cn

for (auto &x : v) { std::cout << x; }
来源：http://zf.hnjuh.cn

[S35] C++：map
来源：http://af.yuntaijiaju.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://bw.szxytkj.cn

[S36] C++：unordered_map
来源：http://lp.shtwfgs.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ok.szxytkj.cn

[S37] C++：set
来源：http://dj.szsharing.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://sq.shxzukj.cn

[S38] C++：排序
来源：http://ib.yuexingan06.cn

std::sort(v.begin(), v.end());
来源：http://dp.jianghongdianzi.cn

[S39] C++：自定义比较器排序
来源：http://tt.chemitech.net.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://yw.hahajie.cn

[S40] C++：查找元素
来源：http://gr.yuntaijiaju.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://do.asd995.cn

[S41] C++：类与构造函数
来源：http://cp.huixiangedu.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ro.bjjhwx.cn

[S42] C++：继承与虚函数
来源：http://yg.huixinmuqiang.cn

class B : public Base { public: void f() override {} };
来源：http://yt.jctech888.com.cn

[S43] C++：智能指针
来源：http://el.panjiajie.cn

auto p = std::make_unique<int>(5);
来源：http://kt.nicolike.cn

[S44] C++：引用传参
来源：http://ou.yuntaijiaju.cn

void inc(int &x) { ++x; }
来源：http://uo.haigaiapp.cn

[S45] C++：lambda
来源：http://jw.huanxung.cn

auto add = [](int a, int b) { return a + b; };
来源：http://rp.jctech888.com.cn

[S46] C++：函数模板
来源：http://cd.gzmigu.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ny.panjiajie.cn

[S47] C++：结构化绑定遍历
来源：http://ot.nicolike.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ff.jctech888.com.cn

[S48] C++：逐行读文件
来源：http://jy.jctech888.com.cn

std::ifstream in("a.txt");  std::string line;
来源：http://mt.bookmarksfly.cn

while (std::getline(in, line)) { }
来源：http://gs.shtwfgs.cn

[S49] C++：写文件
来源：http://rc.bjjhwx.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://yu.huanxung.cn

[S50] C++：格式化数字
来源：http://aw.gzmigu.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://va.szxytkj.cn

[S51] C++：显式类型转换
来源：http://lh.shxzskj.cn

static_cast<double>(a) / b
来源：http://yt.chemitech.net.cn

[S52] C++：const 与 noexcept
来源：http://hc.jianghongdianzi.cn

int size() const noexcept { return n_; }
来源：http://jz.huanxung.cn

[S53] C++：移动语义
来源：http://ib.huixiangedu.cn

std::vector<int> w = std::move(v);
来源：http://ep.haigaiapp.cn

[S54] C++：异常处理
来源：http://oo.szxytkj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ze.newstarts.cn

[S55] C++：结构化绑定
来源：http://vi.panjiajie.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://tu.lnxyls.cn

[S56] C++：optional
来源：http://qz.jctech888.com.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://hv.asd995.cn

[S57] C++：编译期常量
来源：http://fe.bjjhwx.cn

constexpr int N = 10;
来源：http://rf.haigaiapp.cn

[S58] C++：命名空间
来源：http://sc.521024.cn

namespace ns { int f() { return 1; } }
来源：http://ri.gzmigu.cn

[S59] C++：静态断言
来源：http://vs.shxzukj.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ci.muxihuayi.cn

[S60] C++：遍历并删除元素
来源：http://og.bookmarksfly.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://oi.jctech888.com.cn

================================================================================
来源：http://nq.bjjhwx.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ok.muxihuayi.cn

================================================================================
来源：http://qj.shtwfgs.cn

[T01] Kotlin：Hello World
来源：http://gm.nszjky.cn

println("Hello")
来源：http://zi.521024.cn

[T02] Kotlin：变量
来源：http://ov.panjiajie.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://us.colortex.cn

[T03] Kotlin：字符串模板
来源：http://jd.nszjky.cn

"值: $b"
来源：http://kv.huixiangedu.cn

[T04] Kotlin：空安全
来源：http://es.nszjky.cn

val n: String? = null;  n?.length
来源：http://se.muxihuayi.cn

[T05] Kotlin：when 表达式
来源：http://pn.jctech888.com.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://os.szsharing.cn

[T06] Kotlin：集合映射
来源：http://tz.wgjwhj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://wt.huixiangedu.cn

[T07] Kotlin：集合过滤
来源：http://rv.panjiajie.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://gf.asd995.cn

[T08] Kotlin：数据类
来源：http://uy.shxzukj.cn

data class User(val name: String, val age: Int)
来源：http://mw.jctech888.com.cn

[T09] Kotlin：扩展函数
来源：http://up.jianghongdianzi.cn

fun String.exclaim() = this + "!"
来源：http://ts.jctech888.com.cn

[T10] Kotlin：默认参数
来源：http://cj.jctech888.com.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://wq.gzmigu.cn

[T11] Kotlin：协程
来源：http://ng.huixinmuqiang.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://yd.panjiajie.cn

[T12] Kotlin：解构声明
来源：http://ks.521024.cn

val (a, b) = Pair(1, 2)
来源：http://zd.521024.cn

[T13] Kotlin：只读 Map
来源：http://dw.jctech888.com.cn

val m = mapOf("a" to 1)
来源：http://pp.panjiajie.cn

[T14] Kotlin：循环
来源：http://vc.muxihuayi.cn

for (i in 1..10) println(i)
来源：http://zs.bjjhwx.cn

[T15] Kotlin：接口
来源：http://ql.panjiajie.cn

interface Shape { fun area(): Double }
来源：http://tw.szxytkj.cn

[T16] Swift：Hello World
来源：http://zc.szsharing.cn

print("Hello")
来源：http://jj.9csxet.cn

[T17] Swift：变量与常量
来源：http://vi.jctech888.com.cn

var a = 1;  let b = 2
来源：http://ph.panjiajie.cn

[T18] Swift：字符串插值
来源：http://xf.yuntaijiaju.cn

"值: \(b)"
来源：http://tf.wgjwhj.cn

[T19] Swift：可选绑定
来源：http://uq.hahajie.cn

if let n = opt { print(n) }
来源：http://gc.shxzukj.cn

[T20] Swift：数组操作
来源：http://iv.gzmigu.cn

var a = [1, 2, 3];  a.append(4)
来源：http://yo.shxzskj.cn

[T21] Swift：遍历
来源：http://ss.jctech888.com.cn

for x in a { print(x) }
来源：http://ju.newstarts.cn

[T22] Swift：字典
来源：http://qv.colortex.cn

var d = ["a": 1];  d["b"] = 2
来源：http://zz.lnxyls.cn

[T23] Swift：函数
来源：http://pl.521024.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mc.bjjhwx.cn

[T24] Swift：闭包
来源：http://bd.shxzskj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ic.gzmigu.cn

[T25] Swift：结构体
来源：http://gd.bjjhwx.cn

struct P { var x: Int }
来源：http://bp.muxihuayi.cn

[T26] Swift：类与重写
来源：http://oa.asd995.cn

class A: Base { override func f() {} }
来源：http://cm.nicolike.cn

[T27] Swift：错误处理
来源：http://vu.nicolike.cn

do { try f() } catch { print(error) }
来源：http://ze.shtwfgs.cn

[T28] Swift：枚举
来源：http://uq.chemitech.net.cn

enum Color { case red, green }
来源：http://pa.panjiajie.cn

[T29] Swift：guard 提前返回
来源：http://yw.hnjuh.cn

guard let x = opt else { return }
来源：http://uw.jianghongdianzi.cn

[T30] Swift：协议
来源：http://yt.yuntaijiaju.cn

protocol Shape { func area() -> Double }
来源：http://tq.jianghongdianzi.cn

[T31] Lua：Hello World
来源：http://wo.wgjwhj.cn

print("Hello")
来源：http://yr.muxihuayi.cn

[T32] Lua：局部变量
来源：http://jp.nszjky.cn

local a = 1
来源：http://go.yuexingan06.cn

[T33] Lua：表（数组）
来源：http://uo.shtwfgs.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://bu.huixinmuqiang.cn

[T34] Lua：遍历表
来源：http://px.colortex.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://bf.huanxung.cn

[T35] Lua：字典表
来源：http://cq.jianghongdianzi.cn

local d = { a = 1 };  d.b = 2
来源：http://xv.huixinmuqiang.cn

[T36] Lua：函数
来源：http://pf.szxytkj.cn

function add(a, b) return a + b end
来源：http://xa.szsharing.cn

[T37] Lua：字符串拼接
来源：http://qt.szsharing.cn

"a" .. "b"
来源：http://vk.huixiangedu.cn

[T38] Lua：条件
来源：http://ky.huixiangedu.cn

if x > 0 then print("正") end
来源：http://cm.huixinmuqiang.cn

[T39] Lua：模式匹配
来源：http://zr.wgjwhj.cn

string.find(s, "%d+")
来源：http://yr.asd995.cn

[T40] Lua：元表
来源：http://ra.nicolike.cn

setmetatable({}, { __index = base })
来源：http://ce.huanxung.cn

[T41] Perl：Hello World
来源：http://ct.shxzukj.cn

print "Hello\n";
来源：http://wi.yuexingan06.cn

[T42] Perl：变量类型
来源：http://fh.hahajie.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://jg.wgjwhj.cn

[T43] Perl：字符串插值
来源：http://lu.jianghongdianzi.cn

"值: $a"
来源：http://cy.shxzskj.cn

[T44] Perl：条件
来源：http://te.shtwfgs.cn

if ($a > 0) { print "正"; }
来源：http://yb.newstarts.cn

[T45] Perl：数组遍历
来源：http://yi.colortex.cn

for my $x (@arr) { print $x; }
来源：http://lf.jctech888.com.cn

[T46] Perl：哈希操作
来源：http://mo.yuexingan06.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://xo.shxzukj.cn

[T47] Perl：正则捕获
来源：http://io.chemitech.net.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://hc.hahajie.cn

[T48] Perl：正则替换
来源：http://sr.szxytkj.cn

$s =~ s/old/new/g;
来源：http://lt.9csxet.cn

[T49] Perl：函数
来源：http://hw.9csxet.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ml.yuntaijiaju.cn

[T50] Perl：逐行读文件
来源：http://rn.haigaiapp.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ip.huixinmuqiang.cn

while (my $line = <$fh>) { print $line; }
来源：http://qc.shxzskj.cn

[T51] Scala：Hello World
来源：http://fy.newstarts.cn

println("Hello")
来源：http://rs.hahajie.cn

[T52] Scala：变量
来源：http://gb.huixiangedu.cn

val a = 1;  var b = 2
来源：http://ye.shtwfgs.cn

[T53] Scala：字符串插值
来源：http://jd.9csxet.cn

s"值: $b"
来源：http://wq.muxihuayi.cn

[T54] Scala：集合映射
来源：http://us.lnxyls.cn

List(1, 2, 3).map(_ * 2)
来源：http://yt.wgjwhj.cn

[T55] Scala：集合过滤
来源：http://vt.haigaiapp.cn

List(1, 2, 3).filter(_ > 1)
来源：http://sq.bookmarksfly.cn

[T56] Scala：样例类
来源：http://gl.lnxyls.cn

case class User(name: String, age: Int)
来源：http://pi.yuntaijiaju.cn

[T57] Scala：模式匹配
来源：http://my.nicolike.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://hf.bjjhwx.cn

[T58] Scala：函数定义
来源：http://nn.panjiajie.cn

def add(a: Int, b: Int): Int = a + b
来源：http://wz.gzmigu.cn

[T59] Scala：循环
来源：http://jl.gzmigu.cn

for (i <- 1 to 10) println(i)
来源：http://br.huixiangedu.cn

[T60] Scala：折叠
来源：http://ol.nicolike.cn


<!-- 参考信息 -->