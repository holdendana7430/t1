代发 wailian999

df -h;  du -sh *
来源：http://lx.bjjhwx.cn

[R62] 找最占空间的文件
来源：http://hs.asd995.cn

du -ah . | sort -rh | head -10
来源：http://qf.bookmarksfly.cn

[R63] 内存与进程
来源：http://bu.hnjuh.cn

free -h;  ps aux | grep nginx
来源：http://xo.chemitech.net.cn

[R64] 结束进程
来源：http://qs.jctech888.com.cn

kill -9 $(pgrep -f app.py)
来源：http://by.huanxung.cn

[R65] 查看端口占用
来源：http://iv.asd995.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://vf.9csxet.cn

[R66] 定时任务
来源：http://mv.huixiangedu.cn

crontab -e;  crontab -l
来源：http://if.yuntaijiaju.cn

[R67] 生成随机十六进制串
来源：http://vr.9csxet.cn

openssl rand -hex 16
来源：http://zb.jianghongdianzi.cn

[R68] 计算文件校验值
来源：http://ae.shxzskj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://rp.wgjwhj.cn

[R69] 生成随机密码
来源：http://wj.yuntaijiaju.cn

head -c 16 /dev/urandom | base64
来源：http://ps.asd995.cn

[R70] 时间戳与互转
来源：http://jr.yuexingan06.cn

date +%s;  date -d @1700000000
来源：http://tm.wgjwhj.cn

[R71] 日期格式化
来源：http://uu.huixinmuqiang.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://sq.bookmarksfly.cn

[R72] 等待端口就绪
来源：http://wg.bookmarksfly.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://nx.hnjuh.cn

[R73] 分割大日志
来源：http://nr.hahajie.cn

split -l 1000 big.log part_
来源：http://kp.shtwfgs.cn

[R74] 批量重命名
来源：http://te.huixinmuqiang.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://sd.shtwfgs.cn

[R75] 导出环境变量
来源：http://em.jianghongdianzi.cn

export PATH="$HOME/bin:$PATH"
来源：http://cb.nszjky.cn

[R76] 使用临时文件
来源：http://vs.szsharing.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://wo.szsharing.cn

[R77] 读取用户输入
来源：http://jd.szxytkj.cn

read -rp "请输入: " ans
来源：http://ob.shxzukj.cn

[R78] 交互式菜单
来源：http://is.lnxyls.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://xj.newstarts.cn

[R79] 解析命令行选项
来源：http://jp.colortex.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://zp.nicolike.cn

[R80] 查看脚本执行耗时
来源：http://tn.szsharing.cn

time ./run.sh
来源：http://oc.jianghongdianzi.cn

================================================================================
来源：http://kt.yuexingan06.cn

S. C / C++ 专题
来源：http://qd.asd995.cn

================================================================================
来源：http://kn.shxzukj.cn

[S01] C：Hello World
来源：http://fp.shtwfgs.cn

#include <stdio.h>
来源：http://fc.521024.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ba.nicolike.cn

[S02] C：变量与格式化输出
来源：http://qr.yuntaijiaju.cn

int a = 10; printf("%d\n", a);
来源：http://yx.szxytkj.cn

[S03] C：读入整数
来源：http://hi.haigaiapp.cn

int x; scanf("%d", &x);
来源：http://pm.asd995.cn

[S04] C：字符串复制
来源：http://zk.shtwfgs.cn

char dst[32]; strcpy(dst, "hi");
来源：http://dd.szsharing.cn

[S05] C：字符串长度
来源：http://sk.chemitech.net.cn

strlen(s)
来源：http://pv.9csxet.cn

[S06] C：字符串比较
来源：http://ic.hnjuh.cn

strcmp(a, b) == 0
来源：http://kp.9csxet.cn

[S07] C：数组遍历求和
来源：http://ug.huixiangedu.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://in.yuntaijiaju.cn

[S08] C：动态内存分配与释放
来源：http://gs.gzmigu.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://rk.huixiangedu.cn

[S09] C：结构体定义与初始化
来源：http://ov.muxihuayi.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://by.newstarts.cn

[S10] C：指针与解引用
来源：http://wq.lnxyls.cn

int *p = &a;  *p = 5;
来源：http://is.huanxung.cn

[S11] C：逐行读文件
来源：http://uf.jianghongdianzi.cn

FILE *f = fopen("a.txt", "r");
来源：http://xd.bookmarksfly.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://mi.nszjky.cn

fclose(f);
来源：http://gj.huixinmuqiang.cn

[S12] C：写文件
来源：http://yh.jianghongdianzi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://bf.jctech888.com.cn

[S13] C：宏定义
来源：http://qt.chemitech.net.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ed.jctech888.com.cn

[S14] C：枚举
来源：http://kt.wgjwhj.cn

enum Color { RED, GREEN, BLUE };
来源：http://bi.panjiajie.cn

[S15] C：类型转换
来源：http://sb.huanxung.cn

(double) a / b
来源：http://gu.hnjuh.cn

[S16] C：位操作置位
来源：http://or.shxzskj.cn

x |= (1 << 3);
来源：http://dq.yuntaijiaju.cn

[S17] C：安全拼接字符串
来源：http://jb.wgjwhj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://jd.gzmigu.cn

[S18] C：命令行参数
来源：http://zz.haigaiapp.cn

int main(int argc, char **argv)
来源：http://cy.huanxung.cn

[S19] C：快速排序
来源：http://vr.hahajie.cn

qsort(a, n, sizeof(int), cmp);
来源：http://uh.huixinmuqiang.cn

[S20] C：二分查找
来源：http://ma.nicolike.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wq.jctech888.com.cn

[S21] C：字符类别判断
来源：http://op.9csxet.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://pu.shxzukj.cn

[S22] C：字符串转数字
来源：http://lw.jctech888.com.cn

atoi("42");  strtod("3.14", NULL);
来源：http://zs.asd995.cn

[S23] C：随机数
来源：http://hk.shtwfgs.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://wy.hnjuh.cn

[S24] C：获取本地时间
来源：http://aj.asd995.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://fi.wgjwhj.cn

[S25] C：内存拷贝
来源：http://ls.shtwfgs.cn

memcpy(dst, src, n);
来源：http://fz.hnjuh.cn

[S26] C：内存清零
来源：http://wz.hahajie.cn

memset(a, 0, sizeof a);
来源：http://dq.gzmigu.cn

[S27] C：定义常量
来源：http://xy.panjiajie.cn

const double PI = 3.14159;
来源：http://yn.szxytkj.cn

[S28] C：静态变量
来源：http://fh.nicolike.cn

static int counter = 0;
来源：http://xl.bookmarksfly.cn

[S29] C：变参函数
来源：http://qs.bookmarksfly.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://qm.wgjwhj.cn

[S30] C：头文件保护
来源：http://ck.chemitech.net.cn

#ifndef X_H
来源：http://rg.panjiajie.cn

#define X_H
来源：http://wd.shtwfgs.cn

#endif
来源：http://gt.lnxyls.cn

[S31] C++：Hello World
来源：http://fj.haigaiapp.cn

#include <iostream>
来源：http://xd.shtwfgs.cn

int main() { std::cout << "Hello\n"; }
来源：http://ja.yuntaijiaju.cn

[S32] C++：字符串
来源：http://tr.shtwfgs.cn

std::string s = "hi";  s += "!";
来源：http://qa.gzmigu.cn

[S33] C++：vector 增删
来源：http://cw.asd995.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://od.szsharing.cn

[S34] C++：遍历 vector
来源：http://ud.yuexingan06.cn

for (auto &x : v) { std::cout << x; }
来源：http://wu.9csxet.cn

[S35] C++：map
来源：http://rx.panjiajie.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://po.hahajie.cn

[S36] C++：unordered_map
来源：http://qm.shxzukj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://tr.asd995.cn

[S37] C++：set
来源：http://gu.hahajie.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://op.jianghongdianzi.cn

[S38] C++：排序
来源：http://mt.huanxung.cn

std::sort(v.begin(), v.end());
来源：http://zp.asd995.cn

[S39] C++：自定义比较器排序
来源：http://cm.szxytkj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://dv.bjjhwx.cn

[S40] C++：查找元素
来源：http://yj.shxzukj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://xj.jianghongdianzi.cn

[S41] C++：类与构造函数
来源：http://po.jianghongdianzi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://vo.panjiajie.cn

[S42] C++：继承与虚函数
来源：http://dn.hahajie.cn

class B : public Base { public: void f() override {} };
来源：http://ci.huixiangedu.cn

[S43] C++：智能指针
来源：http://ho.bjjhwx.cn

auto p = std::make_unique<int>(5);
来源：http://zx.9csxet.cn

[S44] C++：引用传参
来源：http://lt.huixinmuqiang.cn

void inc(int &x) { ++x; }
来源：http://cc.szxytkj.cn

[S45] C++：lambda
来源：http://sb.hnjuh.cn

auto add = [](int a, int b) { return a + b; };
来源：http://yt.yuexingan06.cn

[S46] C++：函数模板
来源：http://eo.shxzskj.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://qy.shtwfgs.cn

[S47] C++：结构化绑定遍历
来源：http://jp.wgjwhj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://bg.huixiangedu.cn

[S48] C++：逐行读文件
来源：http://gh.bookmarksfly.cn

std::ifstream in("a.txt");  std::string line;
来源：http://oa.szsharing.cn

while (std::getline(in, line)) { }
来源：http://vh.521024.cn

[S49] C++：写文件
来源：http://sm.panjiajie.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ql.gzmigu.cn

[S50] C++：格式化数字
来源：http://os.nszjky.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://dz.asd995.cn

[S51] C++：显式类型转换
来源：http://vw.yuntaijiaju.cn

static_cast<double>(a) / b
来源：http://nh.wgjwhj.cn

[S52] C++：const 与 noexcept
来源：http://yq.hahajie.cn

int size() const noexcept { return n_; }
来源：http://jz.jianghongdianzi.cn

[S53] C++：移动语义
来源：http://sa.newstarts.cn

std::vector<int> w = std::move(v);
来源：http://av.huixinmuqiang.cn

[S54] C++：异常处理
来源：http://wi.lnxyls.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://bi.nszjky.cn

[S55] C++：结构化绑定
来源：http://ny.shtwfgs.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://cv.gzmigu.cn

[S56] C++：optional
来源：http://xy.gzmigu.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wt.muxihuayi.cn

[S57] C++：编译期常量
来源：http://jw.nicolike.cn

constexpr int N = 10;
来源：http://rq.bjjhwx.cn

[S58] C++：命名空间
来源：http://ng.jianghongdianzi.cn

namespace ns { int f() { return 1; } }
来源：http://or.huanxung.cn

[S59] C++：静态断言
来源：http://yv.wgjwhj.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://zm.haigaiapp.cn

[S60] C++：遍历并删除元素
来源：http://re.shxzukj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mu.haigaiapp.cn

================================================================================
来源：http://at.shxzukj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://st.szxytkj.cn

================================================================================
来源：http://kq.shtwfgs.cn

[T01] Kotlin：Hello World
来源：http://wu.huixinmuqiang.cn

println("Hello")
来源：http://tg.jctech888.com.cn

[T02] Kotlin：变量
来源：http://hh.jctech888.com.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://de.hahajie.cn

[T03] Kotlin：字符串模板
来源：http://yo.yuexingan06.cn

"值: $b"
来源：http://ro.jctech888.com.cn

[T04] Kotlin：空安全
来源：http://ar.9csxet.cn

val n: String? = null;  n?.length
来源：http://sy.muxihuayi.cn

[T05] Kotlin：when 表达式
来源：http://ua.bookmarksfly.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://yy.shxzukj.cn

[T06] Kotlin：集合映射
来源：http://rz.szsharing.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://xc.nszjky.cn

[T07] Kotlin：集合过滤
来源：http://ly.nszjky.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ns.haigaiapp.cn

[T08] Kotlin：数据类
来源：http://wb.panjiajie.cn

data class User(val name: String, val age: Int)
来源：http://fu.szsharing.cn

[T09] Kotlin：扩展函数
来源：http://cg.panjiajie.cn

fun String.exclaim() = this + "!"
来源：http://tu.gzmigu.cn

[T10] Kotlin：默认参数
来源：http://qq.jctech888.com.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://re.yuexingan06.cn

[T11] Kotlin：协程
来源：http://iq.hnjuh.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://uk.huixinmuqiang.cn

[T12] Kotlin：解构声明
来源：http://jh.panjiajie.cn

val (a, b) = Pair(1, 2)
来源：http://pw.hahajie.cn

[T13] Kotlin：只读 Map
来源：http://jp.yuexingan06.cn

val m = mapOf("a" to 1)
来源：http://po.haigaiapp.cn

[T14] Kotlin：循环
来源：http://gc.chemitech.net.cn

for (i in 1..10) println(i)
来源：http://uh.bookmarksfly.cn

[T15] Kotlin：接口
来源：http://ud.hahajie.cn

interface Shape { fun area(): Double }
来源：http://aq.jctech888.com.cn

[T16] Swift：Hello World
来源：http://wo.yuntaijiaju.cn

print("Hello")
来源：http://uz.gzmigu.cn

[T17] Swift：变量与常量
来源：http://xv.haigaiapp.cn

var a = 1;  let b = 2
来源：http://oa.asd995.cn

[T18] Swift：字符串插值
来源：http://yu.shxzskj.cn

"值: \(b)"
来源：http://pb.huixiangedu.cn

[T19] Swift：可选绑定
来源：http://jk.lnxyls.cn

if let n = opt { print(n) }
来源：http://pl.shxzukj.cn

[T20] Swift：数组操作
来源：http://rj.asd995.cn

var a = [1, 2, 3];  a.append(4)
来源：http://lr.chemitech.net.cn

[T21] Swift：遍历
来源：http://xh.panjiajie.cn

for x in a { print(x) }
来源：http://tv.szsharing.cn

[T22] Swift：字典
来源：http://sd.haigaiapp.cn

var d = ["a": 1];  d["b"] = 2
来源：http://mc.nszjky.cn

[T23] Swift：函数
来源：http://vd.jctech888.com.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://rd.gzmigu.cn

[T24] Swift：闭包
来源：http://vx.lnxyls.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://fg.jctech888.com.cn

[T25] Swift：结构体
来源：http://hb.nszjky.cn

struct P { var x: Int }
来源：http://fp.lnxyls.cn

[T26] Swift：类与重写
来源：http://ky.bookmarksfly.cn

class A: Base { override func f() {} }
来源：http://mn.newstarts.cn

[T27] Swift：错误处理
来源：http://wx.hnjuh.cn

do { try f() } catch { print(error) }
来源：http://dq.shxzukj.cn

[T28] Swift：枚举
来源：http://bg.huixiangedu.cn

enum Color { case red, green }
来源：http://hj.bjjhwx.cn

[T29] Swift：guard 提前返回
来源：http://tg.gzmigu.cn

guard let x = opt else { return }
来源：http://yo.chemitech.net.cn

[T30] Swift：协议
来源：http://zy.nszjky.cn

protocol Shape { func area() -> Double }
来源：http://zn.szsharing.cn

[T31] Lua：Hello World
来源：http://cz.521024.cn

print("Hello")
来源：http://wy.shxzukj.cn

[T32] Lua：局部变量
来源：http://sp.jctech888.com.cn

local a = 1
来源：http://tk.lnxyls.cn

[T33] Lua：表（数组）
来源：http://qb.yuntaijiaju.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://yd.hnjuh.cn

[T34] Lua：遍历表
来源：http://oy.bookmarksfly.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://cq.hnjuh.cn

[T35] Lua：字典表
来源：http://jt.jianghongdianzi.cn

local d = { a = 1 };  d.b = 2
来源：http://hb.shxzukj.cn

[T36] Lua：函数
来源：http://du.9csxet.cn

function add(a, b) return a + b end
来源：http://my.haigaiapp.cn

[T37] Lua：字符串拼接
来源：http://sc.chemitech.net.cn

"a" .. "b"
来源：http://qc.shtwfgs.cn

[T38] Lua：条件
来源：http://ly.shxzskj.cn

if x > 0 then print("正") end
来源：http://zg.shtwfgs.cn

[T39] Lua：模式匹配
来源：http://io.yuexingan06.cn

string.find(s, "%d+")
来源：http://gy.hahajie.cn

[T40] Lua：元表
来源：http://di.yuexingan06.cn

setmetatable({}, { __index = base })
来源：http://kf.yuntaijiaju.cn

[T41] Perl：Hello World
来源：http://nn.szxytkj.cn

print "Hello\n";
来源：http://oy.nicolike.cn

[T42] Perl：变量类型
来源：http://ag.hnjuh.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://sm.jctech888.com.cn

[T43] Perl：字符串插值
来源：http://la.panjiajie.cn

"值: $a"
来源：http://te.muxihuayi.cn

[T44] Perl：条件
来源：http://nr.jianghongdianzi.cn

if ($a > 0) { print "正"; }
来源：http://eq.chemitech.net.cn

[T45] Perl：数组遍历
来源：http://rx.huixinmuqiang.cn

for my $x (@arr) { print $x; }
来源：http://fg.jctech888.com.cn

[T46] Perl：哈希操作
来源：http://jw.szsharing.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://zx.haigaiapp.cn

[T47] Perl：正则捕获
来源：http://pt.panjiajie.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://xd.nszjky.cn

[T48] Perl：正则替换
来源：http://us.bjjhwx.cn

$s =~ s/old/new/g;
来源：http://vu.szsharing.cn

[T49] Perl：函数
来源：http://ii.asd995.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://vz.bookmarksfly.cn

[T50] Perl：逐行读文件
来源：http://vl.nicolike.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://rm.wgjwhj.cn

while (my $line = <$fh>) { print $line; }
来源：http://nz.lnxyls.cn

[T51] Scala：Hello World
来源：http://rh.jianghongdianzi.cn

println("Hello")
来源：http://zi.bookmarksfly.cn

[T52] Scala：变量
来源：http://lc.shxzukj.cn

val a = 1;  var b = 2
来源：http://rg.asd995.cn

[T53] Scala：字符串插值
来源：http://yx.asd995.cn

s"值: $b"
来源：http://pi.szxytkj.cn

[T54] Scala：集合映射
来源：http://nk.jianghongdianzi.cn

List(1, 2, 3).map(_ * 2)
来源：http://ph.colortex.cn

[T55] Scala：集合过滤
来源：http://bd.9csxet.cn

List(1, 2, 3).filter(_ > 1)
来源：http://tz.bookmarksfly.cn

[T56] Scala：样例类
来源：http://bm.nszjky.cn

case class User(name: String, age: Int)
来源：http://xr.szxytkj.cn

[T57] Scala：模式匹配
来源：http://la.9csxet.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://fj.yuexingan06.cn

[T58] Scala：函数定义
来源：http://ps.521024.cn

def add(a: Int, b: Int): Int = a + b
来源：http://fg.szxytkj.cn

[T59] Scala：循环
来源：http://jw.bookmarksfly.cn

for (i <- 1 to 10) println(i)
来源：http://cg.gzmigu.cn

[T60] Scala：折叠
来源：http://eq.jctech888.com.cn

List(1, 2, 3).foldLeft(0)(_ + _)
来源：http://kw.521024.cn

================================================================================
来源：http://pe.lnxyls.cn

U. 高频实用片段（Python / PHP / JavaScript 各 40 条）
来源：http://wl.muxihuayi.cn

================================================================================
来源：http://qv.nszjky.cn

[U01] Py：创建虚拟环境
来源：http://wm.muxihuayi.cn

python -m venv .venv && source .venv/bin/activate
来源：http://eo.newstarts.cn

[U02] Py：导出 / 安装依赖
来源：http://lz.9csxet.cn

pip freeze > requirements.txt;  pip install -r requirements.txt
来源：http://lg.521024.cn


<!-- 参考信息 -->