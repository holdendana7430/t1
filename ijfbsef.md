代发 wailian999

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ih.huixinmuqiang.cn

[R56] 远程拷贝
来源：http://ph.haigaiapp.cn

scp file user@host:/path/
来源：http://uj.szsharing.cn

[R57] 远程执行命令
来源：http://dp.nszjky.cn

ssh user@host 'uptime'
来源：http://do.hnjuh.cn

[R58] 下载文件
来源：http://vp.jianghongdianzi.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://pq.lnxyls.cn

[R59] 发 POST JSON
来源：http://sh.muxihuayi.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ou.shtwfgs.cn

[R60] 只看 HTTP 状态码
来源：http://eq.colortex.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://bo.huixiangedu.cn

[R61] 磁盘占用
来源：http://nh.gzmigu.cn

df -h;  du -sh *
来源：http://vv.521024.cn

[R62] 找最占空间的文件
来源：http://ns.panjiajie.cn

du -ah . | sort -rh | head -10
来源：http://jg.huanxung.cn

[R63] 内存与进程
来源：http://ik.szxytkj.cn

free -h;  ps aux | grep nginx
来源：http://dl.huanxung.cn

[R64] 结束进程
来源：http://ez.szxytkj.cn

kill -9 $(pgrep -f app.py)
来源：http://vw.wgjwhj.cn

[R65] 查看端口占用
来源：http://vt.huanxung.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://vf.gzmigu.cn

[R66] 定时任务
来源：http://vj.yuntaijiaju.cn

crontab -e;  crontab -l
来源：http://sn.521024.cn

[R67] 生成随机十六进制串
来源：http://hr.gzmigu.cn

openssl rand -hex 16
来源：http://ph.bjjhwx.cn

[R68] 计算文件校验值
来源：http://pq.gzmigu.cn

sha256sum a.txt;  md5sum a.txt
来源：http://lq.panjiajie.cn

[R69] 生成随机密码
来源：http://uu.nicolike.cn

head -c 16 /dev/urandom | base64
来源：http://tp.bjjhwx.cn

[R70] 时间戳与互转
来源：http://ez.wgjwhj.cn

date +%s;  date -d @1700000000
来源：http://wm.huixiangedu.cn

[R71] 日期格式化
来源：http://pv.panjiajie.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://zj.huixinmuqiang.cn

[R72] 等待端口就绪
来源：http://kq.9csxet.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ic.huanxung.cn

[R73] 分割大日志
来源：http://bg.lnxyls.cn

split -l 1000 big.log part_
来源：http://ez.huixiangedu.cn

[R74] 批量重命名
来源：http://lm.chemitech.net.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ll.521024.cn

[R75] 导出环境变量
来源：http://gw.szsharing.cn

export PATH="$HOME/bin:$PATH"
来源：http://ff.jianghongdianzi.cn

[R76] 使用临时文件
来源：http://sr.nicolike.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://dv.jctech888.com.cn

[R77] 读取用户输入
来源：http://uc.lnxyls.cn

read -rp "请输入: " ans
来源：http://wk.colortex.cn

[R78] 交互式菜单
来源：http://vr.colortex.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://um.huixinmuqiang.cn

[R79] 解析命令行选项
来源：http://zw.jctech888.com.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://in.hahajie.cn

[R80] 查看脚本执行耗时
来源：http://di.jianghongdianzi.cn

time ./run.sh
来源：http://lb.521024.cn

================================================================================
来源：http://cg.shxzskj.cn

S. C / C++ 专题
来源：http://yb.yuexingan06.cn

================================================================================
来源：http://on.nszjky.cn

[S01] C：Hello World
来源：http://dn.huixinmuqiang.cn

#include <stdio.h>
来源：http://xn.gzmigu.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://op.shxzukj.cn

[S02] C：变量与格式化输出
来源：http://rv.yuexingan06.cn

int a = 10; printf("%d\n", a);
来源：http://vy.szsharing.cn

[S03] C：读入整数
来源：http://mm.panjiajie.cn

int x; scanf("%d", &x);
来源：http://nn.huanxung.cn

[S04] C：字符串复制
来源：http://ey.bjjhwx.cn

char dst[32]; strcpy(dst, "hi");
来源：http://mg.haigaiapp.cn

[S05] C：字符串长度
来源：http://vx.huixinmuqiang.cn

strlen(s)
来源：http://ee.szsharing.cn

[S06] C：字符串比较
来源：http://pk.asd995.cn

strcmp(a, b) == 0
来源：http://rc.jianghongdianzi.cn

[S07] C：数组遍历求和
来源：http://tc.gzmigu.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://vk.wgjwhj.cn

[S08] C：动态内存分配与释放
来源：http://bx.colortex.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://tb.muxihuayi.cn

[S09] C：结构体定义与初始化
来源：http://ik.jctech888.com.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://zb.newstarts.cn

[S10] C：指针与解引用
来源：http://up.shxzskj.cn

int *p = &a;  *p = 5;
来源：http://qm.muxihuayi.cn

[S11] C：逐行读文件
来源：http://cx.shxzskj.cn

FILE *f = fopen("a.txt", "r");
来源：http://ms.jctech888.com.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://oe.chemitech.net.cn

fclose(f);
来源：http://wx.szsharing.cn

[S12] C：写文件
来源：http://az.huanxung.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://oo.asd995.cn

[S13] C：宏定义
来源：http://ju.9csxet.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://xl.wgjwhj.cn

[S14] C：枚举
来源：http://nn.colortex.cn

enum Color { RED, GREEN, BLUE };
来源：http://he.huanxung.cn

[S15] C：类型转换
来源：http://pm.hahajie.cn

(double) a / b
来源：http://qt.colortex.cn

[S16] C：位操作置位
来源：http://wt.gzmigu.cn

x |= (1 << 3);
来源：http://vv.jianghongdianzi.cn

[S17] C：安全拼接字符串
来源：http://ff.9csxet.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ll.shtwfgs.cn

[S18] C：命令行参数
来源：http://im.haigaiapp.cn

int main(int argc, char **argv)
来源：http://ls.hahajie.cn

[S19] C：快速排序
来源：http://tb.jianghongdianzi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://jg.wgjwhj.cn

[S20] C：二分查找
来源：http://pb.gzmigu.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://yz.shtwfgs.cn

[S21] C：字符类别判断
来源：http://zu.yuexingan06.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ic.yuexingan06.cn

[S22] C：字符串转数字
来源：http://xy.szxytkj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://eu.521024.cn

[S23] C：随机数
来源：http://vt.chemitech.net.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://fu.szsharing.cn

[S24] C：获取本地时间
来源：http://hw.shtwfgs.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://jq.nszjky.cn

[S25] C：内存拷贝
来源：http://as.nszjky.cn

memcpy(dst, src, n);
来源：http://sh.9csxet.cn

[S26] C：内存清零
来源：http://ui.chemitech.net.cn

memset(a, 0, sizeof a);
来源：http://hr.hnjuh.cn

[S27] C：定义常量
来源：http://wa.jianghongdianzi.cn

const double PI = 3.14159;
来源：http://xe.panjiajie.cn

[S28] C：静态变量
来源：http://mj.9csxet.cn

static int counter = 0;
来源：http://vm.asd995.cn

[S29] C：变参函数
来源：http://jd.panjiajie.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://uv.nszjky.cn

[S30] C：头文件保护
来源：http://xt.jctech888.com.cn

#ifndef X_H
来源：http://bd.huixinmuqiang.cn

#define X_H
来源：http://uu.newstarts.cn

#endif
来源：http://yu.szsharing.cn

[S31] C++：Hello World
来源：http://px.hahajie.cn

#include <iostream>
来源：http://ku.hahajie.cn

int main() { std::cout << "Hello\n"; }
来源：http://xm.szsharing.cn

[S32] C++：字符串
来源：http://vp.jctech888.com.cn

std::string s = "hi";  s += "!";
来源：http://nb.shxzukj.cn

[S33] C++：vector 增删
来源：http://qo.nicolike.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://po.szsharing.cn

[S34] C++：遍历 vector
来源：http://pl.panjiajie.cn

for (auto &x : v) { std::cout << x; }
来源：http://qe.szxytkj.cn

[S35] C++：map
来源：http://eg.shxzskj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ei.nszjky.cn

[S36] C++：unordered_map
来源：http://hs.jctech888.com.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ue.shxzukj.cn

[S37] C++：set
来源：http://ms.newstarts.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://xa.muxihuayi.cn

[S38] C++：排序
来源：http://yn.huixinmuqiang.cn

std::sort(v.begin(), v.end());
来源：http://bm.yuexingan06.cn

[S39] C++：自定义比较器排序
来源：http://wl.shtwfgs.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://vy.nszjky.cn

[S40] C++：查找元素
来源：http://kr.hahajie.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://cm.hahajie.cn

[S41] C++：类与构造函数
来源：http://sh.huixinmuqiang.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://qi.lnxyls.cn

[S42] C++：继承与虚函数
来源：http://rv.9csxet.cn

class B : public Base { public: void f() override {} };
来源：http://hh.bookmarksfly.cn

[S43] C++：智能指针
来源：http://ht.bookmarksfly.cn

auto p = std::make_unique<int>(5);
来源：http://ln.hnjuh.cn

[S44] C++：引用传参
来源：http://nm.haigaiapp.cn

void inc(int &x) { ++x; }
来源：http://vd.newstarts.cn

[S45] C++：lambda
来源：http://oo.bjjhwx.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ur.huixinmuqiang.cn

[S46] C++：函数模板
来源：http://au.szsharing.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://md.gzmigu.cn

[S47] C++：结构化绑定遍历
来源：http://nb.szxytkj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://bp.wgjwhj.cn

[S48] C++：逐行读文件
来源：http://kc.nicolike.cn

std::ifstream in("a.txt");  std::string line;
来源：http://iz.jianghongdianzi.cn

while (std::getline(in, line)) { }
来源：http://ds.szsharing.cn

[S49] C++：写文件
来源：http://sq.yuexingan06.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://yz.shtwfgs.cn

[S50] C++：格式化数字
来源：http://ad.huixiangedu.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ay.szsharing.cn

[S51] C++：显式类型转换
来源：http://ed.jctech888.com.cn

static_cast<double>(a) / b
来源：http://td.huixinmuqiang.cn

[S52] C++：const 与 noexcept
来源：http://ch.chemitech.net.cn

int size() const noexcept { return n_; }
来源：http://pr.yuntaijiaju.cn

[S53] C++：移动语义
来源：http://oa.jianghongdianzi.cn

std::vector<int> w = std::move(v);
来源：http://oj.jctech888.com.cn

[S54] C++：异常处理
来源：http://lx.521024.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://uy.chemitech.net.cn

[S55] C++：结构化绑定
来源：http://xa.huixiangedu.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://pi.521024.cn

[S56] C++：optional
来源：http://vk.shxzskj.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ex.muxihuayi.cn

[S57] C++：编译期常量
来源：http://ab.yuntaijiaju.cn

constexpr int N = 10;
来源：http://er.colortex.cn

[S58] C++：命名空间
来源：http://wf.szsharing.cn

namespace ns { int f() { return 1; } }
来源：http://sx.gzmigu.cn

[S59] C++：静态断言
来源：http://sl.jianghongdianzi.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://uo.haigaiapp.cn

[S60] C++：遍历并删除元素
来源：http://mu.huanxung.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://gk.huixiangedu.cn

================================================================================
来源：http://fs.muxihuayi.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://md.nicolike.cn

================================================================================
来源：http://qo.gzmigu.cn

[T01] Kotlin：Hello World
来源：http://cz.wgjwhj.cn

println("Hello")
来源：http://jz.hnjuh.cn

[T02] Kotlin：变量
来源：http://ll.yuntaijiaju.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hf.shxzskj.cn

[T03] Kotlin：字符串模板
来源：http://av.nszjky.cn

"值: $b"
来源：http://yn.huixinmuqiang.cn

[T04] Kotlin：空安全
来源：http://xo.bookmarksfly.cn

val n: String? = null;  n?.length
来源：http://et.szxytkj.cn

[T05] Kotlin：when 表达式
来源：http://dv.shxzskj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ff.newstarts.cn

[T06] Kotlin：集合映射
来源：http://tt.shtwfgs.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://hh.jianghongdianzi.cn

[T07] Kotlin：集合过滤
来源：http://gm.haigaiapp.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://yr.yuexingan06.cn

[T08] Kotlin：数据类
来源：http://dr.yuntaijiaju.cn

data class User(val name: String, val age: Int)
来源：http://io.panjiajie.cn

[T09] Kotlin：扩展函数
来源：http://qa.jctech888.com.cn

fun String.exclaim() = this + "!"
来源：http://fv.yuntaijiaju.cn

[T10] Kotlin：默认参数
来源：http://or.muxihuayi.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://vk.huanxung.cn

[T11] Kotlin：协程
来源：http://dz.yuexingan06.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://rw.wgjwhj.cn

[T12] Kotlin：解构声明
来源：http://kq.hahajie.cn

val (a, b) = Pair(1, 2)
来源：http://ki.bookmarksfly.cn

[T13] Kotlin：只读 Map
来源：http://rd.haigaiapp.cn

val m = mapOf("a" to 1)
来源：http://dc.chemitech.net.cn

[T14] Kotlin：循环
来源：http://ux.jianghongdianzi.cn

for (i in 1..10) println(i)
来源：http://hu.asd995.cn

[T15] Kotlin：接口
来源：http://qn.asd995.cn

interface Shape { fun area(): Double }
来源：http://cn.shxzukj.cn

[T16] Swift：Hello World
来源：http://nd.szsharing.cn

print("Hello")
来源：http://jl.haigaiapp.cn

[T17] Swift：变量与常量
来源：http://gj.jctech888.com.cn

var a = 1;  let b = 2
来源：http://sl.jianghongdianzi.cn

[T18] Swift：字符串插值
来源：http://uz.wgjwhj.cn

"值: \(b)"
来源：http://es.muxihuayi.cn

[T19] Swift：可选绑定
来源：http://ia.bookmarksfly.cn

if let n = opt { print(n) }
来源：http://oc.gzmigu.cn

[T20] Swift：数组操作
来源：http://ur.nszjky.cn

var a = [1, 2, 3];  a.append(4)
来源：http://zu.jctech888.com.cn

[T21] Swift：遍历
来源：http://cr.jctech888.com.cn

for x in a { print(x) }
来源：http://aw.521024.cn

[T22] Swift：字典
来源：http://su.szsharing.cn

var d = ["a": 1];  d["b"] = 2
来源：http://qy.huixiangedu.cn

[T23] Swift：函数
来源：http://pa.szxytkj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://uq.lnxyls.cn

[T24] Swift：闭包
来源：http://ss.shxzukj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ec.jianghongdianzi.cn

[T25] Swift：结构体
来源：http://jw.shxzukj.cn

struct P { var x: Int }
来源：http://ce.shxzskj.cn

[T26] Swift：类与重写
来源：http://hp.szsharing.cn

class A: Base { override func f() {} }
来源：http://xi.shxzskj.cn

[T27] Swift：错误处理
来源：http://da.hnjuh.cn

do { try f() } catch { print(error) }
来源：http://uq.colortex.cn

[T28] Swift：枚举
来源：http://pc.chemitech.net.cn

enum Color { case red, green }
来源：http://no.hahajie.cn

[T29] Swift：guard 提前返回
来源：http://re.gzmigu.cn

guard let x = opt else { return }
来源：http://aa.hahajie.cn

[T30] Swift：协议
来源：http://kh.bookmarksfly.cn

protocol Shape { func area() -> Double }
来源：http://do.yuexingan06.cn

[T31] Lua：Hello World
来源：http://xw.hahajie.cn

print("Hello")
来源：http://no.shtwfgs.cn

[T32] Lua：局部变量
来源：http://nh.bjjhwx.cn

local a = 1
来源：http://zs.hahajie.cn

[T33] Lua：表（数组）
来源：http://qg.nszjky.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://kb.nszjky.cn

[T34] Lua：遍历表
来源：http://sj.shxzskj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://zi.szxytkj.cn

[T35] Lua：字典表
来源：http://vx.hahajie.cn

local d = { a = 1 };  d.b = 2
来源：http://sa.yuntaijiaju.cn

[T36] Lua：函数
来源：http://gt.521024.cn

function add(a, b) return a + b end
来源：http://yz.gzmigu.cn

[T37] Lua：字符串拼接
来源：http://rc.lnxyls.cn

"a" .. "b"
来源：http://ly.jianghongdianzi.cn

[T38] Lua：条件
来源：http://ng.panjiajie.cn

if x > 0 then print("正") end
来源：http://lm.yuexingan06.cn

[T39] Lua：模式匹配
来源：http://fq.jctech888.com.cn

string.find(s, "%d+")
来源：http://pn.szsharing.cn

[T40] Lua：元表
来源：http://qv.shtwfgs.cn

setmetatable({}, { __index = base })
来源：http://iu.yuexingan06.cn

[T41] Perl：Hello World
来源：http://fl.huixinmuqiang.cn

print "Hello\n";
来源：http://ac.hnjuh.cn

[T42] Perl：变量类型
来源：http://xl.lnxyls.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://az.bjjhwx.cn

[T43] Perl：字符串插值
来源：http://pn.hahajie.cn

"值: $a"
来源：http://cf.yuntaijiaju.cn

[T44] Perl：条件
来源：http://lo.gzmigu.cn

if ($a > 0) { print "正"; }
来源：http://yk.lnxyls.cn

[T45] Perl：数组遍历
来源：http://dx.bjjhwx.cn

for my $x (@arr) { print $x; }
来源：http://lr.lnxyls.cn

[T46] Perl：哈希操作
来源：http://hg.9csxet.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ae.wgjwhj.cn

[T47] Perl：正则捕获
来源：http://rc.lnxyls.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://bt.szsharing.cn

[T48] Perl：正则替换
来源：http://pk.nicolike.cn

$s =~ s/old/new/g;
来源：http://oj.haigaiapp.cn

[T49] Perl：函数
来源：http://rg.muxihuayi.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://xe.asd995.cn

[T50] Perl：逐行读文件
来源：http://pc.shxzskj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://zr.nicolike.cn

while (my $line = <$fh>) { print $line; }
来源：http://vr.nszjky.cn

[T51] Scala：Hello World
来源：http://gk.521024.cn

println("Hello")
来源：http://fg.huanxung.cn

[T52] Scala：变量
来源：http://ix.lnxyls.cn

val a = 1;  var b = 2
来源：http://cm.szsharing.cn

[T53] Scala：字符串插值
来源：http://lm.yuexingan06.cn

s"值: $b"
来源：http://cj.huanxung.cn

[T54] Scala：集合映射
来源：http://gs.szxytkj.cn

List(1, 2, 3).map(_ * 2)
来源：http://jh.huanxung.cn

[T55] Scala：集合过滤
来源：http://un.9csxet.cn

List(1, 2, 3).filter(_ > 1)
来源：http://si.huixinmuqiang.cn

[T56] Scala：样例类
来源：http://rs.shxzukj.cn

case class User(name: String, age: Int)
来源：http://ax.wgjwhj.cn

[T57] Scala：模式匹配
来源：http://dq.jianghongdianzi.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://zv.huixiangedu.cn

[T58] Scala：函数定义
来源：http://lb.bookmarksfly.cn


<!-- 参考信息 -->