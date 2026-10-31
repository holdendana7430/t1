代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://iv.jctech888.com.cn

[R54] 比较两个文件
来源：http://bl.bookmarksfly.cn

diff a.txt b.txt
来源：http://dg.521024.cn

[R55] 压缩与解压
来源：http://ew.jianghongdianzi.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://uf.shxzukj.cn

[R56] 远程拷贝
来源：http://sy.huixiangedu.cn

scp file user@host:/path/
来源：http://wx.szsharing.cn

[R57] 远程执行命令
来源：http://ft.bjjhwx.cn

ssh user@host 'uptime'
来源：http://ty.chemitech.net.cn

[R58] 下载文件
来源：http://bg.bjjhwx.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://av.jianghongdianzi.cn

[R59] 发 POST JSON
来源：http://zv.panjiajie.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hs.huanxung.cn

[R60] 只看 HTTP 状态码
来源：http://ew.colortex.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://zf.chemitech.net.cn

[R61] 磁盘占用
来源：http://mj.gzmigu.cn

df -h;  du -sh *
来源：http://kz.jianghongdianzi.cn

[R62] 找最占空间的文件
来源：http://pu.huixinmuqiang.cn

du -ah . | sort -rh | head -10
来源：http://vd.nszjky.cn

[R63] 内存与进程
来源：http://pk.lnxyls.cn

free -h;  ps aux | grep nginx
来源：http://iz.szsharing.cn

[R64] 结束进程
来源：http://kh.nicolike.cn

kill -9 $(pgrep -f app.py)
来源：http://az.newstarts.cn

[R65] 查看端口占用
来源：http://qg.huanxung.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://er.panjiajie.cn

[R66] 定时任务
来源：http://nb.asd995.cn

crontab -e;  crontab -l
来源：http://jy.shtwfgs.cn

[R67] 生成随机十六进制串
来源：http://ia.hnjuh.cn

openssl rand -hex 16
来源：http://ch.newstarts.cn

[R68] 计算文件校验值
来源：http://ng.szxytkj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://qb.bookmarksfly.cn

[R69] 生成随机密码
来源：http://pp.9csxet.cn

head -c 16 /dev/urandom | base64
来源：http://zb.521024.cn

[R70] 时间戳与互转
来源：http://xi.asd995.cn

date +%s;  date -d @1700000000
来源：http://tf.shxzskj.cn

[R71] 日期格式化
来源：http://hb.asd995.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://cc.9csxet.cn

[R72] 等待端口就绪
来源：http://wg.shtwfgs.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://fx.bookmarksfly.cn

[R73] 分割大日志
来源：http://cl.9csxet.cn

split -l 1000 big.log part_
来源：http://vz.hnjuh.cn

[R74] 批量重命名
来源：http://jz.panjiajie.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://nr.wgjwhj.cn

[R75] 导出环境变量
来源：http://vg.muxihuayi.cn

export PATH="$HOME/bin:$PATH"
来源：http://et.newstarts.cn

[R76] 使用临时文件
来源：http://kn.521024.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mr.huixinmuqiang.cn

[R77] 读取用户输入
来源：http://ib.wgjwhj.cn

read -rp "请输入: " ans
来源：http://pb.muxihuayi.cn

[R78] 交互式菜单
来源：http://fm.lnxyls.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ud.nicolike.cn

[R79] 解析命令行选项
来源：http://zb.jianghongdianzi.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://xl.yuexingan06.cn

[R80] 查看脚本执行耗时
来源：http://qw.shtwfgs.cn

time ./run.sh
来源：http://rv.gzmigu.cn

================================================================================
来源：http://sc.muxihuayi.cn

S. C / C++ 专题
来源：http://nz.huixiangedu.cn

================================================================================
来源：http://ql.newstarts.cn

[S01] C：Hello World
来源：http://qr.wgjwhj.cn

#include <stdio.h>
来源：http://bq.muxihuayi.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://uj.bookmarksfly.cn

[S02] C：变量与格式化输出
来源：http://xd.hahajie.cn

int a = 10; printf("%d\n", a);
来源：http://ta.panjiajie.cn

[S03] C：读入整数
来源：http://xl.shxzskj.cn

int x; scanf("%d", &x);
来源：http://jd.gzmigu.cn

[S04] C：字符串复制
来源：http://hc.nszjky.cn

char dst[32]; strcpy(dst, "hi");
来源：http://yi.9csxet.cn

[S05] C：字符串长度
来源：http://xc.yuntaijiaju.cn

strlen(s)
来源：http://no.colortex.cn

[S06] C：字符串比较
来源：http://bk.9csxet.cn

strcmp(a, b) == 0
来源：http://br.gzmigu.cn

[S07] C：数组遍历求和
来源：http://tn.nszjky.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://zk.newstarts.cn

[S08] C：动态内存分配与释放
来源：http://qb.hahajie.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://tj.nicolike.cn

[S09] C：结构体定义与初始化
来源：http://po.huanxung.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://er.nicolike.cn

[S10] C：指针与解引用
来源：http://oi.bookmarksfly.cn

int *p = &a;  *p = 5;
来源：http://gk.szsharing.cn

[S11] C：逐行读文件
来源：http://ew.szsharing.cn

FILE *f = fopen("a.txt", "r");
来源：http://ia.shtwfgs.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://bc.hnjuh.cn

fclose(f);
来源：http://ps.nicolike.cn

[S12] C：写文件
来源：http://zw.bjjhwx.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://yh.newstarts.cn

[S13] C：宏定义
来源：http://fe.521024.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://uo.nszjky.cn

[S14] C：枚举
来源：http://be.shtwfgs.cn

enum Color { RED, GREEN, BLUE };
来源：http://ma.shtwfgs.cn

[S15] C：类型转换
来源：http://mr.9csxet.cn

(double) a / b
来源：http://qq.yuntaijiaju.cn

[S16] C：位操作置位
来源：http://po.shtwfgs.cn

x |= (1 << 3);
来源：http://wx.lnxyls.cn

[S17] C：安全拼接字符串
来源：http://ve.szsharing.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://eo.bjjhwx.cn

[S18] C：命令行参数
来源：http://pa.haigaiapp.cn

int main(int argc, char **argv)
来源：http://zg.9csxet.cn

[S19] C：快速排序
来源：http://ob.panjiajie.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ha.jctech888.com.cn

[S20] C：二分查找
来源：http://gg.jianghongdianzi.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://sm.asd995.cn

[S21] C：字符类别判断
来源：http://go.shxzukj.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://yu.panjiajie.cn

[S22] C：字符串转数字
来源：http://np.nicolike.cn

atoi("42");  strtod("3.14", NULL);
来源：http://wp.jianghongdianzi.cn

[S23] C：随机数
来源：http://yt.muxihuayi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://jf.asd995.cn

[S24] C：获取本地时间
来源：http://wn.bjjhwx.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://cw.gzmigu.cn

[S25] C：内存拷贝
来源：http://xo.muxihuayi.cn

memcpy(dst, src, n);
来源：http://we.chemitech.net.cn

[S26] C：内存清零
来源：http://cu.yuntaijiaju.cn

memset(a, 0, sizeof a);
来源：http://oe.chemitech.net.cn

[S27] C：定义常量
来源：http://se.yuntaijiaju.cn

const double PI = 3.14159;
来源：http://hx.nszjky.cn

[S28] C：静态变量
来源：http://mo.gzmigu.cn

static int counter = 0;
来源：http://wp.szsharing.cn

[S29] C：变参函数
来源：http://fg.asd995.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://fu.bookmarksfly.cn

[S30] C：头文件保护
来源：http://nd.lnxyls.cn

#ifndef X_H
来源：http://aj.shtwfgs.cn

#define X_H
来源：http://yk.colortex.cn

#endif
来源：http://af.szxytkj.cn

[S31] C++：Hello World
来源：http://hs.huixinmuqiang.cn

#include <iostream>
来源：http://yq.huanxung.cn

int main() { std::cout << "Hello\n"; }
来源：http://al.nicolike.cn

[S32] C++：字符串
来源：http://us.asd995.cn

std::string s = "hi";  s += "!";
来源：http://fh.szxytkj.cn

[S33] C++：vector 增删
来源：http://tv.haigaiapp.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://rc.muxihuayi.cn

[S34] C++：遍历 vector
来源：http://ok.haigaiapp.cn

for (auto &x : v) { std::cout << x; }
来源：http://yp.huixiangedu.cn

[S35] C++：map
来源：http://uk.yuntaijiaju.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://pt.muxihuayi.cn

[S36] C++：unordered_map
来源：http://zq.nicolike.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://jq.panjiajie.cn

[S37] C++：set
来源：http://ug.yuntaijiaju.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ly.muxihuayi.cn

[S38] C++：排序
来源：http://ej.shtwfgs.cn

std::sort(v.begin(), v.end());
来源：http://mp.hahajie.cn

[S39] C++：自定义比较器排序
来源：http://uy.chemitech.net.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://kp.bjjhwx.cn

[S40] C++：查找元素
来源：http://ql.shxzskj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ry.shxzukj.cn

[S41] C++：类与构造函数
来源：http://ld.9csxet.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://fx.hnjuh.cn

[S42] C++：继承与虚函数
来源：http://jg.shxzukj.cn

class B : public Base { public: void f() override {} };
来源：http://zy.bjjhwx.cn

[S43] C++：智能指针
来源：http://hm.huixinmuqiang.cn

auto p = std::make_unique<int>(5);
来源：http://vc.wgjwhj.cn

[S44] C++：引用传参
来源：http://hd.szsharing.cn

void inc(int &x) { ++x; }
来源：http://tm.panjiajie.cn

[S45] C++：lambda
来源：http://ow.nicolike.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ly.9csxet.cn

[S46] C++：函数模板
来源：http://uo.hnjuh.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://kc.hnjuh.cn

[S47] C++：结构化绑定遍历
来源：http://pk.asd995.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://zj.huanxung.cn

[S48] C++：逐行读文件
来源：http://zx.haigaiapp.cn

std::ifstream in("a.txt");  std::string line;
来源：http://uo.panjiajie.cn

while (std::getline(in, line)) { }
来源：http://pv.shtwfgs.cn

[S49] C++：写文件
来源：http://nz.hnjuh.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://pk.yuexingan06.cn

[S50] C++：格式化数字
来源：http://tl.hnjuh.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ur.muxihuayi.cn

[S51] C++：显式类型转换
来源：http://ym.shtwfgs.cn

static_cast<double>(a) / b
来源：http://so.huixinmuqiang.cn

[S52] C++：const 与 noexcept
来源：http://og.newstarts.cn

int size() const noexcept { return n_; }
来源：http://mr.gzmigu.cn

[S53] C++：移动语义
来源：http://if.9csxet.cn

std::vector<int> w = std::move(v);
来源：http://ap.jianghongdianzi.cn

[S54] C++：异常处理
来源：http://hb.huixinmuqiang.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://er.haigaiapp.cn

[S55] C++：结构化绑定
来源：http://ij.gzmigu.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://gj.hnjuh.cn

[S56] C++：optional
来源：http://dl.hnjuh.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ui.asd995.cn

[S57] C++：编译期常量
来源：http://mv.huixinmuqiang.cn

constexpr int N = 10;
来源：http://eq.nicolike.cn

[S58] C++：命名空间
来源：http://cc.nicolike.cn

namespace ns { int f() { return 1; } }
来源：http://no.szxytkj.cn

[S59] C++：静态断言
来源：http://qr.jctech888.com.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://od.chemitech.net.cn

[S60] C++：遍历并删除元素
来源：http://mf.nszjky.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://zd.521024.cn

================================================================================
来源：http://fz.bjjhwx.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://xq.hahajie.cn

================================================================================
来源：http://mp.huixiangedu.cn

[T01] Kotlin：Hello World
来源：http://zg.shtwfgs.cn

println("Hello")
来源：http://kd.newstarts.cn

[T02] Kotlin：变量
来源：http://sb.huixiangedu.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://xa.nszjky.cn

[T03] Kotlin：字符串模板
来源：http://vh.wgjwhj.cn

"值: $b"
来源：http://zq.nicolike.cn

[T04] Kotlin：空安全
来源：http://tx.muxihuayi.cn

val n: String? = null;  n?.length
来源：http://rd.hnjuh.cn

[T05] Kotlin：when 表达式
来源：http://vw.lnxyls.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hn.hahajie.cn

[T06] Kotlin：集合映射
来源：http://fu.szxytkj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://be.hahajie.cn

[T07] Kotlin：集合过滤
来源：http://ll.hnjuh.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://dm.szsharing.cn

[T08] Kotlin：数据类
来源：http://it.szxytkj.cn

data class User(val name: String, val age: Int)
来源：http://sg.huixinmuqiang.cn

[T09] Kotlin：扩展函数
来源：http://fi.shxzukj.cn

fun String.exclaim() = this + "!"
来源：http://ze.shxzskj.cn

[T10] Kotlin：默认参数
来源：http://bv.panjiajie.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://th.bookmarksfly.cn

[T11] Kotlin：协程
来源：http://hz.nicolike.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://xl.lnxyls.cn

[T12] Kotlin：解构声明
来源：http://rt.yuntaijiaju.cn

val (a, b) = Pair(1, 2)
来源：http://gb.gzmigu.cn

[T13] Kotlin：只读 Map
来源：http://ut.hahajie.cn

val m = mapOf("a" to 1)
来源：http://ij.haigaiapp.cn

[T14] Kotlin：循环
来源：http://ib.hahajie.cn

for (i in 1..10) println(i)
来源：http://hb.panjiajie.cn

[T15] Kotlin：接口
来源：http://dx.newstarts.cn

interface Shape { fun area(): Double }
来源：http://um.lnxyls.cn

[T16] Swift：Hello World
来源：http://st.hnjuh.cn

print("Hello")
来源：http://jb.gzmigu.cn

[T17] Swift：变量与常量
来源：http://go.szsharing.cn

var a = 1;  let b = 2
来源：http://fx.nszjky.cn

[T18] Swift：字符串插值
来源：http://vp.shxzskj.cn

"值: \(b)"
来源：http://cr.shtwfgs.cn

[T19] Swift：可选绑定
来源：http://lg.shxzukj.cn

if let n = opt { print(n) }
来源：http://ri.muxihuayi.cn

[T20] Swift：数组操作
来源：http://qm.yuntaijiaju.cn

var a = [1, 2, 3];  a.append(4)
来源：http://tt.hnjuh.cn

[T21] Swift：遍历
来源：http://vu.colortex.cn

for x in a { print(x) }
来源：http://vf.shxzskj.cn

[T22] Swift：字典
来源：http://am.colortex.cn

var d = ["a": 1];  d["b"] = 2
来源：http://oe.yuntaijiaju.cn

[T23] Swift：函数
来源：http://ge.shxzskj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://gy.panjiajie.cn

[T24] Swift：闭包
来源：http://va.szsharing.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://pb.nszjky.cn

[T25] Swift：结构体
来源：http://fv.jctech888.com.cn

struct P { var x: Int }
来源：http://mt.bookmarksfly.cn

[T26] Swift：类与重写
来源：http://in.asd995.cn

class A: Base { override func f() {} }
来源：http://eo.haigaiapp.cn

[T27] Swift：错误处理
来源：http://bx.yuntaijiaju.cn

do { try f() } catch { print(error) }
来源：http://lx.shxzukj.cn

[T28] Swift：枚举
来源：http://zj.huanxung.cn

enum Color { case red, green }
来源：http://mk.yuexingan06.cn

[T29] Swift：guard 提前返回
来源：http://co.szsharing.cn

guard let x = opt else { return }
来源：http://gj.shxzukj.cn

[T30] Swift：协议
来源：http://gp.szsharing.cn

protocol Shape { func area() -> Double }
来源：http://rz.yuntaijiaju.cn

[T31] Lua：Hello World
来源：http://wg.lnxyls.cn

print("Hello")
来源：http://ul.yuexingan06.cn

[T32] Lua：局部变量
来源：http://pn.nicolike.cn

local a = 1
来源：http://ro.szxytkj.cn

[T33] Lua：表（数组）
来源：http://jl.jctech888.com.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://hv.haigaiapp.cn

[T34] Lua：遍历表
来源：http://xo.szxytkj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ms.huixinmuqiang.cn

[T35] Lua：字典表
来源：http://xr.jctech888.com.cn

local d = { a = 1 };  d.b = 2
来源：http://qo.huixiangedu.cn

[T36] Lua：函数
来源：http://hj.nicolike.cn

function add(a, b) return a + b end
来源：http://lo.nszjky.cn

[T37] Lua：字符串拼接
来源：http://hw.haigaiapp.cn

"a" .. "b"
来源：http://zj.bookmarksfly.cn

[T38] Lua：条件
来源：http://xa.haigaiapp.cn

if x > 0 then print("正") end
来源：http://fw.521024.cn

[T39] Lua：模式匹配
来源：http://hz.szsharing.cn

string.find(s, "%d+")
来源：http://ay.colortex.cn

[T40] Lua：元表
来源：http://vl.muxihuayi.cn

setmetatable({}, { __index = base })
来源：http://dg.yuexingan06.cn

[T41] Perl：Hello World
来源：http://hy.hnjuh.cn

print "Hello\n";
来源：http://da.huanxung.cn

[T42] Perl：变量类型
来源：http://hb.bjjhwx.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://yo.shtwfgs.cn

[T43] Perl：字符串插值
来源：http://wu.szxytkj.cn

"值: $a"
来源：http://av.bjjhwx.cn

[T44] Perl：条件
来源：http://dz.hnjuh.cn

if ($a > 0) { print "正"; }
来源：http://bn.nszjky.cn

[T45] Perl：数组遍历
来源：http://dx.newstarts.cn

for my $x (@arr) { print $x; }
来源：http://cv.chemitech.net.cn

[T46] Perl：哈希操作
来源：http://vj.huixinmuqiang.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://jz.nszjky.cn

[T47] Perl：正则捕获
来源：http://wv.chemitech.net.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://wb.nicolike.cn

[T48] Perl：正则替换
来源：http://lx.lnxyls.cn

$s =~ s/old/new/g;
来源：http://im.yuntaijiaju.cn

[T49] Perl：函数
来源：http://pg.yuexingan06.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://rr.bookmarksfly.cn

[T50] Perl：逐行读文件
来源：http://zq.huixinmuqiang.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://sh.shtwfgs.cn

while (my $line = <$fh>) { print $line; }
来源：http://am.huixinmuqiang.cn

[T51] Scala：Hello World
来源：http://nd.colortex.cn

println("Hello")
来源：http://mq.jctech888.com.cn

[T52] Scala：变量
来源：http://hp.newstarts.cn

val a = 1;  var b = 2
来源：http://yy.huanxung.cn

[T53] Scala：字符串插值
来源：http://mt.nszjky.cn

s"值: $b"
来源：http://ei.haigaiapp.cn

[T54] Scala：集合映射
来源：http://js.bjjhwx.cn

List(1, 2, 3).map(_ * 2)
来源：http://iz.huixinmuqiang.cn

[T55] Scala：集合过滤
来源：http://ph.panjiajie.cn

List(1, 2, 3).filter(_ > 1)
来源：http://py.bjjhwx.cn

[T56] Scala：样例类
来源：http://zf.shxzskj.cn


<!-- 参考信息 -->