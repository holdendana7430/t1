代发 wailian999

ssh user@host 'uptime'
来源：http://pt.wgjwhj.cn

[R58] 下载文件
来源：http://of.wgjwhj.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://it.shtwfgs.cn

[R59] 发 POST JSON
来源：http://hm.bjjhwx.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://xv.shxzukj.cn

[R60] 只看 HTTP 状态码
来源：http://eb.nszjky.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://bk.jianghongdianzi.cn

[R61] 磁盘占用
来源：http://wa.panjiajie.cn

df -h;  du -sh *
来源：http://kt.colortex.cn

[R62] 找最占空间的文件
来源：http://qv.asd995.cn

du -ah . | sort -rh | head -10
来源：http://kw.asd995.cn

[R63] 内存与进程
来源：http://oq.9csxet.cn

free -h;  ps aux | grep nginx
来源：http://zh.gzmigu.cn

[R64] 结束进程
来源：http://yq.huanxung.cn

kill -9 $(pgrep -f app.py)
来源：http://uv.colortex.cn

[R65] 查看端口占用
来源：http://cu.asd995.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://xp.jianghongdianzi.cn

[R66] 定时任务
来源：http://bs.colortex.cn

crontab -e;  crontab -l
来源：http://rc.521024.cn

[R67] 生成随机十六进制串
来源：http://hk.haigaiapp.cn

openssl rand -hex 16
来源：http://pu.shtwfgs.cn

[R68] 计算文件校验值
来源：http://qk.hahajie.cn

sha256sum a.txt;  md5sum a.txt
来源：http://iv.colortex.cn

[R69] 生成随机密码
来源：http://ww.panjiajie.cn

head -c 16 /dev/urandom | base64
来源：http://vc.yuntaijiaju.cn

[R70] 时间戳与互转
来源：http://eu.521024.cn

date +%s;  date -d @1700000000
来源：http://ai.hahajie.cn

[R71] 日期格式化
来源：http://ku.bookmarksfly.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ch.gzmigu.cn

[R72] 等待端口就绪
来源：http://ez.hnjuh.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://jm.shxzskj.cn

[R73] 分割大日志
来源：http://le.nicolike.cn

split -l 1000 big.log part_
来源：http://kc.jianghongdianzi.cn

[R74] 批量重命名
来源：http://bb.bjjhwx.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://sw.wgjwhj.cn

[R75] 导出环境变量
来源：http://kw.panjiajie.cn

export PATH="$HOME/bin:$PATH"
来源：http://ta.9csxet.cn

[R76] 使用临时文件
来源：http://wq.szsharing.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ej.gzmigu.cn

[R77] 读取用户输入
来源：http://sp.asd995.cn

read -rp "请输入: " ans
来源：http://de.asd995.cn

[R78] 交互式菜单
来源：http://mo.lnxyls.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://am.9csxet.cn

[R79] 解析命令行选项
来源：http://eh.nicolike.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ii.gzmigu.cn

[R80] 查看脚本执行耗时
来源：http://km.szsharing.cn

time ./run.sh
来源：http://tf.muxihuayi.cn

================================================================================
来源：http://xi.bookmarksfly.cn

S. C / C++ 专题
来源：http://lw.panjiajie.cn

================================================================================
来源：http://pp.bookmarksfly.cn

[S01] C：Hello World
来源：http://in.9csxet.cn

#include <stdio.h>
来源：http://xv.wgjwhj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://by.yuexingan06.cn

[S02] C：变量与格式化输出
来源：http://ml.haigaiapp.cn

int a = 10; printf("%d\n", a);
来源：http://sa.shxzukj.cn

[S03] C：读入整数
来源：http://di.nicolike.cn

int x; scanf("%d", &x);
来源：http://fl.shxzukj.cn

[S04] C：字符串复制
来源：http://hk.szxytkj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://iq.huanxung.cn

[S05] C：字符串长度
来源：http://bi.521024.cn

strlen(s)
来源：http://hn.yuexingan06.cn

[S06] C：字符串比较
来源：http://xj.gzmigu.cn

strcmp(a, b) == 0
来源：http://lx.muxihuayi.cn

[S07] C：数组遍历求和
来源：http://rr.newstarts.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ph.newstarts.cn

[S08] C：动态内存分配与释放
来源：http://dm.chemitech.net.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://pj.9csxet.cn

[S09] C：结构体定义与初始化
来源：http://wh.huanxung.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ya.lnxyls.cn

[S10] C：指针与解引用
来源：http://nn.yuexingan06.cn

int *p = &a;  *p = 5;
来源：http://tm.yuexingan06.cn

[S11] C：逐行读文件
来源：http://pu.huanxung.cn

FILE *f = fopen("a.txt", "r");
来源：http://il.huixiangedu.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://yj.chemitech.net.cn

fclose(f);
来源：http://ab.szxytkj.cn

[S12] C：写文件
来源：http://cs.shtwfgs.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://zn.nszjky.cn

[S13] C：宏定义
来源：http://sc.shtwfgs.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://dp.lnxyls.cn

[S14] C：枚举
来源：http://oi.newstarts.cn

enum Color { RED, GREEN, BLUE };
来源：http://ov.panjiajie.cn

[S15] C：类型转换
来源：http://rl.panjiajie.cn

(double) a / b
来源：http://ci.haigaiapp.cn

[S16] C：位操作置位
来源：http://hc.jianghongdianzi.cn

x |= (1 << 3);
来源：http://xa.colortex.cn

[S17] C：安全拼接字符串
来源：http://do.gzmigu.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ir.chemitech.net.cn

[S18] C：命令行参数
来源：http://xq.shxzskj.cn

int main(int argc, char **argv)
来源：http://ly.yuexingan06.cn

[S19] C：快速排序
来源：http://xe.jianghongdianzi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://sm.huanxung.cn

[S20] C：二分查找
来源：http://xg.yuntaijiaju.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://fy.nszjky.cn

[S21] C：字符类别判断
来源：http://gw.huixinmuqiang.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ug.shxzskj.cn

[S22] C：字符串转数字
来源：http://dq.colortex.cn

atoi("42");  strtod("3.14", NULL);
来源：http://sl.newstarts.cn

[S23] C：随机数
来源：http://jl.yuntaijiaju.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://la.shxzukj.cn

[S24] C：获取本地时间
来源：http://zw.9csxet.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://tv.shtwfgs.cn

[S25] C：内存拷贝
来源：http://wd.asd995.cn

memcpy(dst, src, n);
来源：http://nk.colortex.cn

[S26] C：内存清零
来源：http://tc.shxzskj.cn

memset(a, 0, sizeof a);
来源：http://vl.szxytkj.cn

[S27] C：定义常量
来源：http://pq.lnxyls.cn

const double PI = 3.14159;
来源：http://go.yuexingan06.cn

[S28] C：静态变量
来源：http://ap.szsharing.cn

static int counter = 0;
来源：http://mc.panjiajie.cn

[S29] C：变参函数
来源：http://ox.yuntaijiaju.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://nw.shtwfgs.cn

[S30] C：头文件保护
来源：http://oh.newstarts.cn

#ifndef X_H
来源：http://xx.hnjuh.cn

#define X_H
来源：http://fs.szsharing.cn

#endif
来源：http://eb.521024.cn

[S31] C++：Hello World
来源：http://wh.wgjwhj.cn

#include <iostream>
来源：http://kp.huixiangedu.cn

int main() { std::cout << "Hello\n"; }
来源：http://pu.shxzskj.cn

[S32] C++：字符串
来源：http://sj.gzmigu.cn

std::string s = "hi";  s += "!";
来源：http://fk.asd995.cn

[S33] C++：vector 增删
来源：http://mg.jianghongdianzi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://de.nicolike.cn

[S34] C++：遍历 vector
来源：http://ox.jctech888.com.cn

for (auto &x : v) { std::cout << x; }
来源：http://og.wgjwhj.cn

[S35] C++：map
来源：http://xg.nicolike.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://em.nicolike.cn

[S36] C++：unordered_map
来源：http://tx.nszjky.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://cf.9csxet.cn

[S37] C++：set
来源：http://vg.lnxyls.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://tp.jianghongdianzi.cn

[S38] C++：排序
来源：http://ny.szsharing.cn

std::sort(v.begin(), v.end());
来源：http://tx.yuexingan06.cn

[S39] C++：自定义比较器排序
来源：http://zd.muxihuayi.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://uf.nszjky.cn

[S40] C++：查找元素
来源：http://ou.chemitech.net.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://or.asd995.cn

[S41] C++：类与构造函数
来源：http://lf.wgjwhj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://bg.bookmarksfly.cn

[S42] C++：继承与虚函数
来源：http://wp.jctech888.com.cn

class B : public Base { public: void f() override {} };
来源：http://gw.nszjky.cn

[S43] C++：智能指针
来源：http://ti.asd995.cn

auto p = std::make_unique<int>(5);
来源：http://tv.521024.cn

[S44] C++：引用传参
来源：http://ur.haigaiapp.cn

void inc(int &x) { ++x; }
来源：http://rn.wgjwhj.cn

[S45] C++：lambda
来源：http://gm.wgjwhj.cn

auto add = [](int a, int b) { return a + b; };
来源：http://qd.jianghongdianzi.cn

[S46] C++：函数模板
来源：http://ou.nicolike.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ix.muxihuayi.cn

[S47] C++：结构化绑定遍历
来源：http://so.bookmarksfly.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://xm.muxihuayi.cn

[S48] C++：逐行读文件
来源：http://yp.521024.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ep.bookmarksfly.cn

while (std::getline(in, line)) { }
来源：http://tt.haigaiapp.cn

[S49] C++：写文件
来源：http://kr.shxzukj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ff.wgjwhj.cn

[S50] C++：格式化数字
来源：http://ze.9csxet.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://pq.asd995.cn

[S51] C++：显式类型转换
来源：http://or.colortex.cn

static_cast<double>(a) / b
来源：http://dk.colortex.cn

[S52] C++：const 与 noexcept
来源：http://bn.bookmarksfly.cn

int size() const noexcept { return n_; }
来源：http://vm.9csxet.cn

[S53] C++：移动语义
来源：http://my.hahajie.cn

std::vector<int> w = std::move(v);
来源：http://pd.yuexingan06.cn

[S54] C++：异常处理
来源：http://je.gzmigu.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://kz.521024.cn

[S55] C++：结构化绑定
来源：http://ic.hnjuh.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://dh.hnjuh.cn

[S56] C++：optional
来源：http://kz.9csxet.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://zu.jctech888.com.cn

[S57] C++：编译期常量
来源：http://bi.chemitech.net.cn

constexpr int N = 10;
来源：http://jq.haigaiapp.cn

[S58] C++：命名空间
来源：http://ls.gzmigu.cn

namespace ns { int f() { return 1; } }
来源：http://yo.shtwfgs.cn

[S59] C++：静态断言
来源：http://eb.szxytkj.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://tl.szxytkj.cn

[S60] C++：遍历并删除元素
来源：http://qr.shxzukj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://rd.newstarts.cn

================================================================================
来源：http://af.huixiangedu.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://lt.bookmarksfly.cn

================================================================================
来源：http://gk.shxzukj.cn

[T01] Kotlin：Hello World
来源：http://ux.muxihuayi.cn

println("Hello")
来源：http://wq.shtwfgs.cn

[T02] Kotlin：变量
来源：http://ve.lnxyls.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ff.haigaiapp.cn

[T03] Kotlin：字符串模板
来源：http://go.szsharing.cn

"值: $b"
来源：http://dc.szsharing.cn

[T04] Kotlin：空安全
来源：http://xs.newstarts.cn

val n: String? = null;  n?.length
来源：http://ye.bookmarksfly.cn

[T05] Kotlin：when 表达式
来源：http://by.haigaiapp.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://up.colortex.cn

[T06] Kotlin：集合映射
来源：http://nn.huanxung.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://qz.yuexingan06.cn

[T07] Kotlin：集合过滤
来源：http://nf.nszjky.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://xk.lnxyls.cn

[T08] Kotlin：数据类
来源：http://rz.haigaiapp.cn

data class User(val name: String, val age: Int)
来源：http://kt.521024.cn

[T09] Kotlin：扩展函数
来源：http://hr.yuexingan06.cn

fun String.exclaim() = this + "!"
来源：http://gj.hahajie.cn

[T10] Kotlin：默认参数
来源：http://lz.szxytkj.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://vf.haigaiapp.cn

[T11] Kotlin：协程
来源：http://ue.newstarts.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ls.asd995.cn

[T12] Kotlin：解构声明
来源：http://st.huixiangedu.cn

val (a, b) = Pair(1, 2)
来源：http://kx.huixiangedu.cn

[T13] Kotlin：只读 Map
来源：http://ih.szxytkj.cn

val m = mapOf("a" to 1)
来源：http://xh.chemitech.net.cn

[T14] Kotlin：循环
来源：http://os.shtwfgs.cn

for (i in 1..10) println(i)
来源：http://vv.huixinmuqiang.cn

[T15] Kotlin：接口
来源：http://yg.9csxet.cn

interface Shape { fun area(): Double }
来源：http://bk.huixiangedu.cn

[T16] Swift：Hello World
来源：http://hz.shxzskj.cn

print("Hello")
来源：http://ni.lnxyls.cn

[T17] Swift：变量与常量
来源：http://sb.muxihuayi.cn

var a = 1;  let b = 2
来源：http://qm.chemitech.net.cn

[T18] Swift：字符串插值
来源：http://aj.bjjhwx.cn

"值: \(b)"
来源：http://zb.szxytkj.cn

[T19] Swift：可选绑定
来源：http://si.newstarts.cn

if let n = opt { print(n) }
来源：http://cx.lnxyls.cn

[T20] Swift：数组操作
来源：http://dq.jianghongdianzi.cn

var a = [1, 2, 3];  a.append(4)
来源：http://zd.chemitech.net.cn

[T21] Swift：遍历
来源：http://pj.panjiajie.cn

for x in a { print(x) }
来源：http://rv.jianghongdianzi.cn

[T22] Swift：字典
来源：http://rs.shxzukj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://xs.haigaiapp.cn

[T23] Swift：函数
来源：http://rc.nicolike.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://le.bjjhwx.cn

[T24] Swift：闭包
来源：http://hm.colortex.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://nc.szxytkj.cn

[T25] Swift：结构体
来源：http://sn.hnjuh.cn

struct P { var x: Int }
来源：http://vq.panjiajie.cn

[T26] Swift：类与重写
来源：http://uz.bjjhwx.cn

class A: Base { override func f() {} }
来源：http://er.gzmigu.cn

[T27] Swift：错误处理
来源：http://dx.szxytkj.cn

do { try f() } catch { print(error) }
来源：http://ay.muxihuayi.cn

[T28] Swift：枚举
来源：http://rb.bookmarksfly.cn

enum Color { case red, green }
来源：http://yj.nszjky.cn

[T29] Swift：guard 提前返回
来源：http://hz.huixinmuqiang.cn

guard let x = opt else { return }
来源：http://zl.asd995.cn

[T30] Swift：协议
来源：http://io.wgjwhj.cn

protocol Shape { func area() -> Double }
来源：http://fk.bjjhwx.cn

[T31] Lua：Hello World
来源：http://vg.9csxet.cn

print("Hello")
来源：http://pq.panjiajie.cn

[T32] Lua：局部变量
来源：http://sz.gzmigu.cn

local a = 1
来源：http://uy.jctech888.com.cn

[T33] Lua：表（数组）
来源：http://ax.huixinmuqiang.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://vn.huixiangedu.cn

[T34] Lua：遍历表
来源：http://it.muxihuayi.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://nm.shtwfgs.cn

[T35] Lua：字典表
来源：http://xc.nicolike.cn

local d = { a = 1 };  d.b = 2
来源：http://fd.yuntaijiaju.cn

[T36] Lua：函数
来源：http://ob.chemitech.net.cn

function add(a, b) return a + b end
来源：http://lo.panjiajie.cn

[T37] Lua：字符串拼接
来源：http://io.shxzukj.cn

"a" .. "b"
来源：http://by.jianghongdianzi.cn

[T38] Lua：条件
来源：http://zs.szxytkj.cn

if x > 0 then print("正") end
来源：http://sg.yuntaijiaju.cn

[T39] Lua：模式匹配
来源：http://bg.szsharing.cn

string.find(s, "%d+")
来源：http://ru.shxzukj.cn

[T40] Lua：元表
来源：http://ux.9csxet.cn

setmetatable({}, { __index = base })
来源：http://hk.hahajie.cn

[T41] Perl：Hello World
来源：http://vx.muxihuayi.cn

print "Hello\n";
来源：http://xe.newstarts.cn

[T42] Perl：变量类型
来源：http://uz.huixiangedu.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://tt.szxytkj.cn

[T43] Perl：字符串插值
来源：http://xc.gzmigu.cn

"值: $a"
来源：http://er.panjiajie.cn

[T44] Perl：条件
来源：http://of.521024.cn

if ($a > 0) { print "正"; }
来源：http://if.wgjwhj.cn

[T45] Perl：数组遍历
来源：http://ts.muxihuayi.cn

for my $x (@arr) { print $x; }
来源：http://wg.hnjuh.cn

[T46] Perl：哈希操作
来源：http://vt.jianghongdianzi.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ak.huixiangedu.cn

[T47] Perl：正则捕获
来源：http://us.shxzskj.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://jg.muxihuayi.cn

[T48] Perl：正则替换
来源：http://ry.huanxung.cn

$s =~ s/old/new/g;
来源：http://zn.newstarts.cn

[T49] Perl：函数
来源：http://qc.huixinmuqiang.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ym.huixiangedu.cn

[T50] Perl：逐行读文件
来源：http://cd.shxzskj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://zf.asd995.cn

while (my $line = <$fh>) { print $line; }
来源：http://ci.haigaiapp.cn

[T51] Scala：Hello World
来源：http://hz.huanxung.cn

println("Hello")
来源：http://zh.shxzukj.cn

[T52] Scala：变量
来源：http://qq.shtwfgs.cn

val a = 1;  var b = 2
来源：http://di.huixinmuqiang.cn

[T53] Scala：字符串插值
来源：http://lb.hahajie.cn

s"值: $b"
来源：http://xb.muxihuayi.cn

[T54] Scala：集合映射
来源：http://vx.hahajie.cn

List(1, 2, 3).map(_ * 2)
来源：http://bv.szsharing.cn

[T55] Scala：集合过滤
来源：http://wf.bjjhwx.cn

List(1, 2, 3).filter(_ > 1)
来源：http://su.newstarts.cn

[T56] Scala：样例类
来源：http://on.muxihuayi.cn

case class User(name: String, age: Int)
来源：http://wq.szxytkj.cn

[T57] Scala：模式匹配
来源：http://di.asd995.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://fb.nszjky.cn

[T58] Scala：函数定义
来源：http://cw.nszjky.cn

def add(a: Int, b: Int): Int = a + b
来源：http://wo.huixiangedu.cn

[T59] Scala：循环
来源：http://bu.gzmigu.cn

for (i <- 1 to 10) println(i)
来源：http://fm.yuexingan06.cn

[T60] Scala：折叠
来源：http://uu.muxihuayi.cn


<!-- 参考信息 -->