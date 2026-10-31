代发 wailian999

ssh user@host 'uptime'
来源：http://zs.hnjuh.cn

[R58] 下载文件
来源：http://in.muxihuayi.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ic.chemitech.net.cn

[R59] 发 POST JSON
来源：http://sq.haigaiapp.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://zn.huixinmuqiang.cn

[R60] 只看 HTTP 状态码
来源：http://ws.lnxyls.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://pv.9csxet.cn

[R61] 磁盘占用
来源：http://ta.huixinmuqiang.cn

df -h;  du -sh *
来源：http://li.yuexingan06.cn

[R62] 找最占空间的文件
来源：http://fd.szsharing.cn

du -ah . | sort -rh | head -10
来源：http://ae.huixinmuqiang.cn

[R63] 内存与进程
来源：http://vb.shxzskj.cn

free -h;  ps aux | grep nginx
来源：http://ax.szsharing.cn

[R64] 结束进程
来源：http://qc.muxihuayi.cn

kill -9 $(pgrep -f app.py)
来源：http://ik.szsharing.cn

[R65] 查看端口占用
来源：http://jm.521024.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://zc.hnjuh.cn

[R66] 定时任务
来源：http://dx.nicolike.cn

crontab -e;  crontab -l
来源：http://hh.hahajie.cn

[R67] 生成随机十六进制串
来源：http://wd.hnjuh.cn

openssl rand -hex 16
来源：http://xj.9csxet.cn

[R68] 计算文件校验值
来源：http://bx.shxzukj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://yf.bjjhwx.cn

[R69] 生成随机密码
来源：http://yn.panjiajie.cn

head -c 16 /dev/urandom | base64
来源：http://we.chemitech.net.cn

[R70] 时间戳与互转
来源：http://ay.yuexingan06.cn

date +%s;  date -d @1700000000
来源：http://xy.nszjky.cn

[R71] 日期格式化
来源：http://vx.panjiajie.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://am.lnxyls.cn

[R72] 等待端口就绪
来源：http://zz.szsharing.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://bs.nicolike.cn

[R73] 分割大日志
来源：http://kr.szxytkj.cn

split -l 1000 big.log part_
来源：http://tk.shxzukj.cn

[R74] 批量重命名
来源：http://eb.nicolike.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://og.shtwfgs.cn

[R75] 导出环境变量
来源：http://jc.lnxyls.cn

export PATH="$HOME/bin:$PATH"
来源：http://il.9csxet.cn

[R76] 使用临时文件
来源：http://tn.521024.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://bs.hnjuh.cn

[R77] 读取用户输入
来源：http://jq.bookmarksfly.cn

read -rp "请输入: " ans
来源：http://hk.bjjhwx.cn

[R78] 交互式菜单
来源：http://iz.jianghongdianzi.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://qm.huixiangedu.cn

[R79] 解析命令行选项
来源：http://gi.bjjhwx.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://av.nicolike.cn

[R80] 查看脚本执行耗时
来源：http://qw.huixiangedu.cn

time ./run.sh
来源：http://au.lnxyls.cn

================================================================================
来源：http://lt.szxytkj.cn

S. C / C++ 专题
来源：http://ms.nicolike.cn

================================================================================
来源：http://ts.hnjuh.cn

[S01] C：Hello World
来源：http://wt.hnjuh.cn

#include <stdio.h>
来源：http://xa.huixinmuqiang.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://jp.newstarts.cn

[S02] C：变量与格式化输出
来源：http://op.nszjky.cn

int a = 10; printf("%d\n", a);
来源：http://hu.lnxyls.cn

[S03] C：读入整数
来源：http://qb.colortex.cn

int x; scanf("%d", &x);
来源：http://cq.hahajie.cn

[S04] C：字符串复制
来源：http://ld.yuexingan06.cn

char dst[32]; strcpy(dst, "hi");
来源：http://gk.newstarts.cn

[S05] C：字符串长度
来源：http://hk.szxytkj.cn

strlen(s)
来源：http://qx.hahajie.cn

[S06] C：字符串比较
来源：http://pw.jctech888.com.cn

strcmp(a, b) == 0
来源：http://vu.haigaiapp.cn

[S07] C：数组遍历求和
来源：http://or.asd995.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://th.hahajie.cn

[S08] C：动态内存分配与释放
来源：http://et.muxihuayi.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://wt.huixinmuqiang.cn

[S09] C：结构体定义与初始化
来源：http://uz.szsharing.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hm.szxytkj.cn

[S10] C：指针与解引用
来源：http://cb.nicolike.cn

int *p = &a;  *p = 5;
来源：http://ku.jianghongdianzi.cn

[S11] C：逐行读文件
来源：http://zp.bookmarksfly.cn

FILE *f = fopen("a.txt", "r");
来源：http://gv.9csxet.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://vs.yuexingan06.cn

fclose(f);
来源：http://bw.jctech888.com.cn

[S12] C：写文件
来源：http://zn.huixiangedu.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://sr.yuexingan06.cn

[S13] C：宏定义
来源：http://nq.haigaiapp.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://xz.9csxet.cn

[S14] C：枚举
来源：http://dd.yuexingan06.cn

enum Color { RED, GREEN, BLUE };
来源：http://px.gzmigu.cn

[S15] C：类型转换
来源：http://gs.yuntaijiaju.cn

(double) a / b
来源：http://gz.nicolike.cn

[S16] C：位操作置位
来源：http://oh.huanxung.cn

x |= (1 << 3);
来源：http://dn.bookmarksfly.cn

[S17] C：安全拼接字符串
来源：http://ny.nszjky.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ld.shxzskj.cn

[S18] C：命令行参数
来源：http://un.yuntaijiaju.cn

int main(int argc, char **argv)
来源：http://ag.shtwfgs.cn

[S19] C：快速排序
来源：http://fl.muxihuayi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://lg.szsharing.cn

[S20] C：二分查找
来源：http://zx.521024.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://qc.gzmigu.cn

[S21] C：字符类别判断
来源：http://ew.szxytkj.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://gb.jianghongdianzi.cn

[S22] C：字符串转数字
来源：http://ek.colortex.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ps.hahajie.cn

[S23] C：随机数
来源：http://bj.huixinmuqiang.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://os.jianghongdianzi.cn

[S24] C：获取本地时间
来源：http://jr.huanxung.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://hi.bookmarksfly.cn

[S25] C：内存拷贝
来源：http://nx.hahajie.cn

memcpy(dst, src, n);
来源：http://te.szsharing.cn

[S26] C：内存清零
来源：http://ku.jctech888.com.cn

memset(a, 0, sizeof a);
来源：http://bp.9csxet.cn

[S27] C：定义常量
来源：http://va.hahajie.cn

const double PI = 3.14159;
来源：http://xs.szxytkj.cn

[S28] C：静态变量
来源：http://ef.chemitech.net.cn

static int counter = 0;
来源：http://ht.521024.cn

[S29] C：变参函数
来源：http://ab.szsharing.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ce.huixiangedu.cn

[S30] C：头文件保护
来源：http://xn.hahajie.cn

#ifndef X_H
来源：http://mu.chemitech.net.cn

#define X_H
来源：http://au.lnxyls.cn

#endif
来源：http://ez.szxytkj.cn

[S31] C++：Hello World
来源：http://nh.newstarts.cn

#include <iostream>
来源：http://ez.colortex.cn

int main() { std::cout << "Hello\n"; }
来源：http://as.panjiajie.cn

[S32] C++：字符串
来源：http://ez.shtwfgs.cn

std::string s = "hi";  s += "!";
来源：http://hc.yuntaijiaju.cn

[S33] C++：vector 增删
来源：http://ac.lnxyls.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://as.shxzskj.cn

[S34] C++：遍历 vector
来源：http://vn.colortex.cn

for (auto &x : v) { std::cout << x; }
来源：http://qo.nicolike.cn

[S35] C++：map
来源：http://xb.hnjuh.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://jm.asd995.cn

[S36] C++：unordered_map
来源：http://gz.shxzukj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://zu.nszjky.cn

[S37] C++：set
来源：http://lr.shxzskj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ca.lnxyls.cn

[S38] C++：排序
来源：http://td.huixinmuqiang.cn

std::sort(v.begin(), v.end());
来源：http://wc.huixiangedu.cn

[S39] C++：自定义比较器排序
来源：http://lr.wgjwhj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://rk.jctech888.com.cn

[S40] C++：查找元素
来源：http://xp.asd995.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://rb.yuexingan06.cn

[S41] C++：类与构造函数
来源：http://yi.nicolike.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://lv.huixiangedu.cn

[S42] C++：继承与虚函数
来源：http://cr.lnxyls.cn

class B : public Base { public: void f() override {} };
来源：http://ge.huixinmuqiang.cn

[S43] C++：智能指针
来源：http://ce.hnjuh.cn

auto p = std::make_unique<int>(5);
来源：http://tt.hahajie.cn

[S44] C++：引用传参
来源：http://sq.nszjky.cn

void inc(int &x) { ++x; }
来源：http://df.521024.cn

[S45] C++：lambda
来源：http://el.nicolike.cn

auto add = [](int a, int b) { return a + b; };
来源：http://eb.huanxung.cn

[S46] C++：函数模板
来源：http://wf.colortex.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://el.colortex.cn

[S47] C++：结构化绑定遍历
来源：http://bt.szxytkj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://dx.jianghongdianzi.cn

[S48] C++：逐行读文件
来源：http://cf.huixinmuqiang.cn

std::ifstream in("a.txt");  std::string line;
来源：http://wt.haigaiapp.cn

while (std::getline(in, line)) { }
来源：http://iy.szsharing.cn

[S49] C++：写文件
来源：http://cx.bookmarksfly.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://tp.shxzskj.cn

[S50] C++：格式化数字
来源：http://hr.colortex.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://lk.gzmigu.cn

[S51] C++：显式类型转换
来源：http://sl.muxihuayi.cn

static_cast<double>(a) / b
来源：http://eu.bookmarksfly.cn

[S52] C++：const 与 noexcept
来源：http://im.wgjwhj.cn

int size() const noexcept { return n_; }
来源：http://if.nszjky.cn

[S53] C++：移动语义
来源：http://cb.colortex.cn

std::vector<int> w = std::move(v);
来源：http://zx.nszjky.cn

[S54] C++：异常处理
来源：http://mw.huixinmuqiang.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ho.muxihuayi.cn

[S55] C++：结构化绑定
来源：http://zq.muxihuayi.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ma.panjiajie.cn

[S56] C++：optional
来源：http://fp.colortex.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://dx.9csxet.cn

[S57] C++：编译期常量
来源：http://hn.panjiajie.cn

constexpr int N = 10;
来源：http://gj.szxytkj.cn

[S58] C++：命名空间
来源：http://pz.yuntaijiaju.cn

namespace ns { int f() { return 1; } }
来源：http://qw.szxytkj.cn

[S59] C++：静态断言
来源：http://qu.shxzskj.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://oe.lnxyls.cn

[S60] C++：遍历并删除元素
来源：http://ne.lnxyls.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://cg.gzmigu.cn

================================================================================
来源：http://jx.gzmigu.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ih.lnxyls.cn

================================================================================
来源：http://kj.nszjky.cn

[T01] Kotlin：Hello World
来源：http://jf.yuntaijiaju.cn

println("Hello")
来源：http://lm.521024.cn

[T02] Kotlin：变量
来源：http://mv.hahajie.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://en.nszjky.cn

[T03] Kotlin：字符串模板
来源：http://pi.jctech888.com.cn

"值: $b"
来源：http://cv.521024.cn

[T04] Kotlin：空安全
来源：http://lk.jctech888.com.cn

val n: String? = null;  n?.length
来源：http://nc.yuexingan06.cn

[T05] Kotlin：when 表达式
来源：http://mp.huixiangedu.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://df.huanxung.cn

[T06] Kotlin：集合映射
来源：http://iv.shtwfgs.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://dx.hnjuh.cn

[T07] Kotlin：集合过滤
来源：http://cl.szxytkj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ne.asd995.cn

[T08] Kotlin：数据类
来源：http://pk.szxytkj.cn

data class User(val name: String, val age: Int)
来源：http://hf.bookmarksfly.cn

[T09] Kotlin：扩展函数
来源：http://od.yuexingan06.cn

fun String.exclaim() = this + "!"
来源：http://bz.jianghongdianzi.cn

[T10] Kotlin：默认参数
来源：http://mi.newstarts.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://mf.jianghongdianzi.cn

[T11] Kotlin：协程
来源：http://nb.shtwfgs.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://nm.panjiajie.cn

[T12] Kotlin：解构声明
来源：http://ad.jctech888.com.cn

val (a, b) = Pair(1, 2)
来源：http://oi.hnjuh.cn

[T13] Kotlin：只读 Map
来源：http://af.chemitech.net.cn

val m = mapOf("a" to 1)
来源：http://nb.huixiangedu.cn

[T14] Kotlin：循环
来源：http://hh.lnxyls.cn

for (i in 1..10) println(i)
来源：http://xw.wgjwhj.cn

[T15] Kotlin：接口
来源：http://ox.szxytkj.cn

interface Shape { fun area(): Double }
来源：http://es.yuexingan06.cn

[T16] Swift：Hello World
来源：http://vd.shtwfgs.cn

print("Hello")
来源：http://rx.huanxung.cn

[T17] Swift：变量与常量
来源：http://ol.shtwfgs.cn

var a = 1;  let b = 2
来源：http://zb.gzmigu.cn

[T18] Swift：字符串插值
来源：http://do.hnjuh.cn

"值: \(b)"
来源：http://ao.wgjwhj.cn

[T19] Swift：可选绑定
来源：http://ds.wgjwhj.cn

if let n = opt { print(n) }
来源：http://lh.gzmigu.cn

[T20] Swift：数组操作
来源：http://hq.colortex.cn

var a = [1, 2, 3];  a.append(4)
来源：http://kq.9csxet.cn

[T21] Swift：遍历
来源：http://mo.asd995.cn

for x in a { print(x) }
来源：http://az.wgjwhj.cn

[T22] Swift：字典
来源：http://dc.yuexingan06.cn

var d = ["a": 1];  d["b"] = 2
来源：http://iq.yuntaijiaju.cn

[T23] Swift：函数
来源：http://au.yuntaijiaju.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://as.hnjuh.cn

[T24] Swift：闭包
来源：http://ny.muxihuayi.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://os.521024.cn

[T25] Swift：结构体
来源：http://sh.lnxyls.cn

struct P { var x: Int }
来源：http://bf.shtwfgs.cn

[T26] Swift：类与重写
来源：http://kl.yuexingan06.cn

class A: Base { override func f() {} }
来源：http://pm.nicolike.cn

[T27] Swift：错误处理
来源：http://qn.haigaiapp.cn

do { try f() } catch { print(error) }
来源：http://wf.asd995.cn

[T28] Swift：枚举
来源：http://mn.shtwfgs.cn

enum Color { case red, green }
来源：http://lt.asd995.cn

[T29] Swift：guard 提前返回
来源：http://us.hnjuh.cn

guard let x = opt else { return }
来源：http://vk.shtwfgs.cn

[T30] Swift：协议
来源：http://jn.hnjuh.cn

protocol Shape { func area() -> Double }
来源：http://dc.muxihuayi.cn

[T31] Lua：Hello World
来源：http://ta.521024.cn

print("Hello")
来源：http://kp.chemitech.net.cn

[T32] Lua：局部变量
来源：http://pd.colortex.cn

local a = 1
来源：http://ue.hnjuh.cn

[T33] Lua：表（数组）
来源：http://it.jianghongdianzi.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://mb.muxihuayi.cn

[T34] Lua：遍历表
来源：http://cg.chemitech.net.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://wa.hahajie.cn

[T35] Lua：字典表
来源：http://lh.shxzskj.cn

local d = { a = 1 };  d.b = 2
来源：http://bn.huixiangedu.cn

[T36] Lua：函数
来源：http://xz.bjjhwx.cn

function add(a, b) return a + b end
来源：http://yk.gzmigu.cn

[T37] Lua：字符串拼接
来源：http://xg.yuexingan06.cn

"a" .. "b"
来源：http://cc.521024.cn

[T38] Lua：条件
来源：http://gu.szsharing.cn

if x > 0 then print("正") end
来源：http://ud.shxzukj.cn

[T39] Lua：模式匹配
来源：http://rx.shxzukj.cn

string.find(s, "%d+")
来源：http://xf.haigaiapp.cn

[T40] Lua：元表
来源：http://qy.panjiajie.cn

setmetatable({}, { __index = base })
来源：http://vq.muxihuayi.cn

[T41] Perl：Hello World
来源：http://tm.hahajie.cn

print "Hello\n";
来源：http://sw.jianghongdianzi.cn

[T42] Perl：变量类型
来源：http://uq.yuntaijiaju.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://gr.521024.cn

[T43] Perl：字符串插值
来源：http://if.szxytkj.cn

"值: $a"
来源：http://cj.huixiangedu.cn

[T44] Perl：条件
来源：http://vq.colortex.cn

if ($a > 0) { print "正"; }
来源：http://vo.yuexingan06.cn

[T45] Perl：数组遍历
来源：http://to.hahajie.cn

for my $x (@arr) { print $x; }
来源：http://uq.asd995.cn

[T46] Perl：哈希操作
来源：http://qp.bookmarksfly.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://bq.shxzskj.cn

[T47] Perl：正则捕获
来源：http://ie.lnxyls.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ap.newstarts.cn

[T48] Perl：正则替换
来源：http://ny.szsharing.cn

$s =~ s/old/new/g;
来源：http://eu.panjiajie.cn

[T49] Perl：函数
来源：http://zv.9csxet.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://bg.shxzskj.cn

[T50] Perl：逐行读文件
来源：http://ui.newstarts.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://er.jctech888.com.cn

while (my $line = <$fh>) { print $line; }
来源：http://hk.hnjuh.cn

[T51] Scala：Hello World
来源：http://fh.lnxyls.cn

println("Hello")
来源：http://fy.newstarts.cn

[T52] Scala：变量
来源：http://it.newstarts.cn

val a = 1;  var b = 2
来源：http://dy.colortex.cn

[T53] Scala：字符串插值
来源：http://df.jianghongdianzi.cn

s"值: $b"
来源：http://iu.hnjuh.cn

[T54] Scala：集合映射
来源：http://di.hnjuh.cn

List(1, 2, 3).map(_ * 2)
来源：http://mk.bjjhwx.cn

[T55] Scala：集合过滤
来源：http://mb.bookmarksfly.cn

List(1, 2, 3).filter(_ > 1)
来源：http://bn.huixiangedu.cn

[T56] Scala：样例类
来源：http://fa.colortex.cn

case class User(name: String, age: Int)
来源：http://fy.shxzskj.cn

[T57] Scala：模式匹配
来源：http://pw.huixinmuqiang.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://sx.muxihuayi.cn

[T58] Scala：函数定义
来源：http://qc.jianghongdianzi.cn

def add(a: Int, b: Int): Int = a + b
来源：http://ty.jctech888.com.cn

[T59] Scala：循环
来源：http://tw.521024.cn

for (i <- 1 to 10) println(i)
来源：http://ke.bookmarksfly.cn

[T60] Scala：折叠
来源：http://ra.shxzukj.cn


<!-- 参考信息 -->