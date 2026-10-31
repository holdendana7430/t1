代发 wailian999

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://wu.huixiangedu.cn

[R56] 远程拷贝
来源：http://pe.lnxyls.cn

scp file user@host:/path/
来源：http://uk.huixiangedu.cn

[R57] 远程执行命令
来源：http://rh.nszjky.cn

ssh user@host 'uptime'
来源：http://ag.521024.cn

[R58] 下载文件
来源：http://gz.jctech888.com.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://iz.yuntaijiaju.cn

[R59] 发 POST JSON
来源：http://zx.bookmarksfly.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://cn.huanxung.cn

[R60] 只看 HTTP 状态码
来源：http://nb.gzmigu.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://im.panjiajie.cn

[R61] 磁盘占用
来源：http://ga.shxzukj.cn

df -h;  du -sh *
来源：http://he.panjiajie.cn

[R62] 找最占空间的文件
来源：http://eb.huixiangedu.cn

du -ah . | sort -rh | head -10
来源：http://hz.hnjuh.cn

[R63] 内存与进程
来源：http://zp.panjiajie.cn

free -h;  ps aux | grep nginx
来源：http://bd.panjiajie.cn

[R64] 结束进程
来源：http://fo.muxihuayi.cn

kill -9 $(pgrep -f app.py)
来源：http://ng.nicolike.cn

[R65] 查看端口占用
来源：http://lf.shtwfgs.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://er.521024.cn

[R66] 定时任务
来源：http://oj.nicolike.cn

crontab -e;  crontab -l
来源：http://rx.shxzskj.cn

[R67] 生成随机十六进制串
来源：http://zv.gzmigu.cn

openssl rand -hex 16
来源：http://aw.lnxyls.cn

[R68] 计算文件校验值
来源：http://wn.shtwfgs.cn

sha256sum a.txt;  md5sum a.txt
来源：http://de.nszjky.cn

[R69] 生成随机密码
来源：http://up.bookmarksfly.cn

head -c 16 /dev/urandom | base64
来源：http://dv.shxzskj.cn

[R70] 时间戳与互转
来源：http://jm.newstarts.cn

date +%s;  date -d @1700000000
来源：http://mb.bjjhwx.cn

[R71] 日期格式化
来源：http://lw.yuexingan06.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://vt.9csxet.cn

[R72] 等待端口就绪
来源：http://ip.muxihuayi.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://gt.yuntaijiaju.cn

[R73] 分割大日志
来源：http://wc.newstarts.cn

split -l 1000 big.log part_
来源：http://nz.gzmigu.cn

[R74] 批量重命名
来源：http://lb.chemitech.net.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://kn.shtwfgs.cn

[R75] 导出环境变量
来源：http://iv.huixiangedu.cn

export PATH="$HOME/bin:$PATH"
来源：http://pg.hahajie.cn

[R76] 使用临时文件
来源：http://js.hnjuh.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://jg.shxzukj.cn

[R77] 读取用户输入
来源：http://wp.nicolike.cn

read -rp "请输入: " ans
来源：http://jf.haigaiapp.cn

[R78] 交互式菜单
来源：http://jq.shtwfgs.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://wa.szxytkj.cn

[R79] 解析命令行选项
来源：http://up.lnxyls.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://sd.nicolike.cn

[R80] 查看脚本执行耗时
来源：http://tm.nszjky.cn

time ./run.sh
来源：http://dr.huanxung.cn

================================================================================
来源：http://us.szsharing.cn

S. C / C++ 专题
来源：http://rx.bjjhwx.cn

================================================================================
来源：http://eu.yuexingan06.cn

[S01] C：Hello World
来源：http://iw.9csxet.cn

#include <stdio.h>
来源：http://nu.asd995.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://qb.huanxung.cn

[S02] C：变量与格式化输出
来源：http://st.shxzukj.cn

int a = 10; printf("%d\n", a);
来源：http://xy.haigaiapp.cn

[S03] C：读入整数
来源：http://ns.szsharing.cn

int x; scanf("%d", &x);
来源：http://di.521024.cn

[S04] C：字符串复制
来源：http://gw.newstarts.cn

char dst[32]; strcpy(dst, "hi");
来源：http://wu.yuntaijiaju.cn

[S05] C：字符串长度
来源：http://ba.huixiangedu.cn

strlen(s)
来源：http://kn.shxzukj.cn

[S06] C：字符串比较
来源：http://fm.newstarts.cn

strcmp(a, b) == 0
来源：http://sj.huixiangedu.cn

[S07] C：数组遍历求和
来源：http://sr.jctech888.com.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ci.yuntaijiaju.cn

[S08] C：动态内存分配与释放
来源：http://yw.haigaiapp.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://lh.9csxet.cn

[S09] C：结构体定义与初始化
来源：http://ei.shxzskj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://km.hnjuh.cn

[S10] C：指针与解引用
来源：http://rm.szsharing.cn

int *p = &a;  *p = 5;
来源：http://tt.wgjwhj.cn

[S11] C：逐行读文件
来源：http://md.9csxet.cn

FILE *f = fopen("a.txt", "r");
来源：http://uo.9csxet.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://bp.colortex.cn

fclose(f);
来源：http://zi.yuexingan06.cn

[S12] C：写文件
来源：http://qz.huanxung.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://at.lnxyls.cn

[S13] C：宏定义
来源：http://qm.9csxet.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ms.colortex.cn

[S14] C：枚举
来源：http://dv.szsharing.cn

enum Color { RED, GREEN, BLUE };
来源：http://ht.shtwfgs.cn

[S15] C：类型转换
来源：http://hn.lnxyls.cn

(double) a / b
来源：http://ve.newstarts.cn

[S16] C：位操作置位
来源：http://gv.521024.cn

x |= (1 << 3);
来源：http://qy.szsharing.cn

[S17] C：安全拼接字符串
来源：http://sk.bookmarksfly.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://af.panjiajie.cn

[S18] C：命令行参数
来源：http://uf.jctech888.com.cn

int main(int argc, char **argv)
来源：http://zz.yuexingan06.cn

[S19] C：快速排序
来源：http://cc.huanxung.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ez.szsharing.cn

[S20] C：二分查找
来源：http://si.haigaiapp.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ki.huixiangedu.cn

[S21] C：字符类别判断
来源：http://hy.lnxyls.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://kr.shtwfgs.cn

[S22] C：字符串转数字
来源：http://gu.panjiajie.cn

atoi("42");  strtod("3.14", NULL);
来源：http://dq.szsharing.cn

[S23] C：随机数
来源：http://rf.jianghongdianzi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://pk.wgjwhj.cn

[S24] C：获取本地时间
来源：http://xe.wgjwhj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ht.haigaiapp.cn

[S25] C：内存拷贝
来源：http://nr.wgjwhj.cn

memcpy(dst, src, n);
来源：http://yq.haigaiapp.cn

[S26] C：内存清零
来源：http://su.szxytkj.cn

memset(a, 0, sizeof a);
来源：http://rn.hahajie.cn

[S27] C：定义常量
来源：http://ng.muxihuayi.cn

const double PI = 3.14159;
来源：http://fj.huanxung.cn

[S28] C：静态变量
来源：http://ix.asd995.cn

static int counter = 0;
来源：http://da.521024.cn

[S29] C：变参函数
来源：http://xe.bookmarksfly.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://zy.muxihuayi.cn

[S30] C：头文件保护
来源：http://qj.colortex.cn

#ifndef X_H
来源：http://zp.jctech888.com.cn

#define X_H
来源：http://hs.bjjhwx.cn

#endif
来源：http://gg.panjiajie.cn

[S31] C++：Hello World
来源：http://ml.521024.cn

#include <iostream>
来源：http://yl.panjiajie.cn

int main() { std::cout << "Hello\n"; }
来源：http://do.521024.cn

[S32] C++：字符串
来源：http://of.bjjhwx.cn

std::string s = "hi";  s += "!";
来源：http://ca.yuntaijiaju.cn

[S33] C++：vector 增删
来源：http://qp.muxihuayi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ds.yuntaijiaju.cn

[S34] C++：遍历 vector
来源：http://df.colortex.cn

for (auto &x : v) { std::cout << x; }
来源：http://at.huixiangedu.cn

[S35] C++：map
来源：http://st.jctech888.com.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://gh.shxzskj.cn

[S36] C++：unordered_map
来源：http://iv.jianghongdianzi.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://hn.hnjuh.cn

[S37] C++：set
来源：http://vx.panjiajie.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ot.huanxung.cn

[S38] C++：排序
来源：http://kc.szsharing.cn

std::sort(v.begin(), v.end());
来源：http://hy.szsharing.cn

[S39] C++：自定义比较器排序
来源：http://bj.yuexingan06.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://bn.shxzukj.cn

[S40] C++：查找元素
来源：http://ql.muxihuayi.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mt.haigaiapp.cn

[S41] C++：类与构造函数
来源：http://fz.9csxet.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://tn.9csxet.cn

[S42] C++：继承与虚函数
来源：http://ll.huixiangedu.cn

class B : public Base { public: void f() override {} };
来源：http://nd.shtwfgs.cn

[S43] C++：智能指针
来源：http://hi.9csxet.cn

auto p = std::make_unique<int>(5);
来源：http://ur.9csxet.cn

[S44] C++：引用传参
来源：http://id.huanxung.cn

void inc(int &x) { ++x; }
来源：http://mi.wgjwhj.cn

[S45] C++：lambda
来源：http://fq.hnjuh.cn

auto add = [](int a, int b) { return a + b; };
来源：http://um.hahajie.cn

[S46] C++：函数模板
来源：http://ja.bjjhwx.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://xl.huixiangedu.cn

[S47] C++：结构化绑定遍历
来源：http://lv.jctech888.com.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://iw.haigaiapp.cn

[S48] C++：逐行读文件
来源：http://xh.jctech888.com.cn

std::ifstream in("a.txt");  std::string line;
来源：http://fz.haigaiapp.cn

while (std::getline(in, line)) { }
来源：http://dq.shxzukj.cn

[S49] C++：写文件
来源：http://ml.haigaiapp.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://zb.jctech888.com.cn

[S50] C++：格式化数字
来源：http://fz.huanxung.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://pm.bookmarksfly.cn

[S51] C++：显式类型转换
来源：http://dy.jctech888.com.cn

static_cast<double>(a) / b
来源：http://mw.newstarts.cn

[S52] C++：const 与 noexcept
来源：http://uf.huixinmuqiang.cn

int size() const noexcept { return n_; }
来源：http://er.chemitech.net.cn

[S53] C++：移动语义
来源：http://kz.newstarts.cn

std::vector<int> w = std::move(v);
来源：http://ed.521024.cn

[S54] C++：异常处理
来源：http://gk.nicolike.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://qm.shxzukj.cn

[S55] C++：结构化绑定
来源：http://pw.chemitech.net.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://qm.jianghongdianzi.cn

[S56] C++：optional
来源：http://dj.lnxyls.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ce.jctech888.com.cn

[S57] C++：编译期常量
来源：http://te.chemitech.net.cn

constexpr int N = 10;
来源：http://fk.panjiajie.cn

[S58] C++：命名空间
来源：http://zi.jctech888.com.cn

namespace ns { int f() { return 1; } }
来源：http://wg.9csxet.cn

[S59] C++：静态断言
来源：http://jx.yuexingan06.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://aa.521024.cn

[S60] C++：遍历并删除元素
来源：http://qr.yuntaijiaju.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://di.colortex.cn

================================================================================
来源：http://yo.nicolike.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://kp.newstarts.cn

================================================================================
来源：http://nb.521024.cn

[T01] Kotlin：Hello World
来源：http://zg.huanxung.cn

println("Hello")
来源：http://mo.panjiajie.cn

[T02] Kotlin：变量
来源：http://dd.yuexingan06.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://xt.huixinmuqiang.cn

[T03] Kotlin：字符串模板
来源：http://qq.panjiajie.cn

"值: $b"
来源：http://fv.colortex.cn

[T04] Kotlin：空安全
来源：http://ja.szsharing.cn

val n: String? = null;  n?.length
来源：http://dx.wgjwhj.cn

[T05] Kotlin：when 表达式
来源：http://js.nicolike.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://tu.szxytkj.cn

[T06] Kotlin：集合映射
来源：http://cr.hahajie.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://un.haigaiapp.cn

[T07] Kotlin：集合过滤
来源：http://pd.haigaiapp.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://yg.huixiangedu.cn

[T08] Kotlin：数据类
来源：http://bb.newstarts.cn

data class User(val name: String, val age: Int)
来源：http://ly.muxihuayi.cn

[T09] Kotlin：扩展函数
来源：http://to.shtwfgs.cn

fun String.exclaim() = this + "!"
来源：http://kx.shxzukj.cn

[T10] Kotlin：默认参数
来源：http://sc.jianghongdianzi.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://wp.hnjuh.cn

[T11] Kotlin：协程
来源：http://ez.muxihuayi.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://vb.muxihuayi.cn

[T12] Kotlin：解构声明
来源：http://qy.bookmarksfly.cn

val (a, b) = Pair(1, 2)
来源：http://xh.huixinmuqiang.cn

[T13] Kotlin：只读 Map
来源：http://gr.huixinmuqiang.cn

val m = mapOf("a" to 1)
来源：http://rp.huixinmuqiang.cn

[T14] Kotlin：循环
来源：http://bo.szxytkj.cn

for (i in 1..10) println(i)
来源：http://bh.bookmarksfly.cn

[T15] Kotlin：接口
来源：http://mk.gzmigu.cn

interface Shape { fun area(): Double }
来源：http://hz.panjiajie.cn

[T16] Swift：Hello World
来源：http://pr.wgjwhj.cn

print("Hello")
来源：http://ox.colortex.cn

[T17] Swift：变量与常量
来源：http://vl.jianghongdianzi.cn

var a = 1;  let b = 2
来源：http://wn.szxytkj.cn

[T18] Swift：字符串插值
来源：http://sr.yuexingan06.cn

"值: \(b)"
来源：http://rr.szsharing.cn

[T19] Swift：可选绑定
来源：http://zk.bookmarksfly.cn

if let n = opt { print(n) }
来源：http://ci.huixinmuqiang.cn

[T20] Swift：数组操作
来源：http://td.nszjky.cn

var a = [1, 2, 3];  a.append(4)
来源：http://jk.bjjhwx.cn

[T21] Swift：遍历
来源：http://ml.muxihuayi.cn

for x in a { print(x) }
来源：http://bz.huanxung.cn

[T22] Swift：字典
来源：http://eh.newstarts.cn

var d = ["a": 1];  d["b"] = 2
来源：http://oc.bookmarksfly.cn

[T23] Swift：函数
来源：http://ju.bookmarksfly.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://od.panjiajie.cn

[T24] Swift：闭包
来源：http://ru.bjjhwx.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ar.nicolike.cn

[T25] Swift：结构体
来源：http://qt.hnjuh.cn

struct P { var x: Int }
来源：http://jo.shxzskj.cn

[T26] Swift：类与重写
来源：http://sg.szsharing.cn

class A: Base { override func f() {} }
来源：http://bc.521024.cn

[T27] Swift：错误处理
来源：http://fq.jctech888.com.cn

do { try f() } catch { print(error) }
来源：http://up.panjiajie.cn

[T28] Swift：枚举
来源：http://pr.521024.cn

enum Color { case red, green }
来源：http://ix.521024.cn

[T29] Swift：guard 提前返回
来源：http://mz.shxzskj.cn

guard let x = opt else { return }
来源：http://hf.huixinmuqiang.cn

[T30] Swift：协议
来源：http://cj.huixiangedu.cn

protocol Shape { func area() -> Double }
来源：http://av.gzmigu.cn

[T31] Lua：Hello World
来源：http://ze.szxytkj.cn

print("Hello")
来源：http://sp.nszjky.cn

[T32] Lua：局部变量
来源：http://uj.huixiangedu.cn

local a = 1
来源：http://wv.huixinmuqiang.cn

[T33] Lua：表（数组）
来源：http://id.bookmarksfly.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://kf.wgjwhj.cn

[T34] Lua：遍历表
来源：http://gt.shtwfgs.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://oz.bjjhwx.cn

[T35] Lua：字典表
来源：http://ap.chemitech.net.cn

local d = { a = 1 };  d.b = 2
来源：http://sz.521024.cn

[T36] Lua：函数
来源：http://vp.lnxyls.cn

function add(a, b) return a + b end
来源：http://bw.muxihuayi.cn

[T37] Lua：字符串拼接
来源：http://ar.yuntaijiaju.cn

"a" .. "b"
来源：http://qt.yuexingan06.cn

[T38] Lua：条件
来源：http://gb.huixinmuqiang.cn

if x > 0 then print("正") end
来源：http://qc.colortex.cn

[T39] Lua：模式匹配
来源：http://pa.muxihuayi.cn

string.find(s, "%d+")
来源：http://pu.9csxet.cn

[T40] Lua：元表
来源：http://cs.huixiangedu.cn

setmetatable({}, { __index = base })
来源：http://ad.nicolike.cn

[T41] Perl：Hello World
来源：http://ln.bookmarksfly.cn

print "Hello\n";
来源：http://mb.newstarts.cn

[T42] Perl：变量类型
来源：http://wc.yuntaijiaju.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://pu.huixiangedu.cn

[T43] Perl：字符串插值
来源：http://lb.shxzukj.cn

"值: $a"
来源：http://pw.colortex.cn

[T44] Perl：条件
来源：http://aa.yuexingan06.cn

if ($a > 0) { print "正"; }
来源：http://mf.jctech888.com.cn

[T45] Perl：数组遍历
来源：http://zs.wgjwhj.cn

for my $x (@arr) { print $x; }
来源：http://zw.huixinmuqiang.cn

[T46] Perl：哈希操作
来源：http://vl.colortex.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://bi.panjiajie.cn

[T47] Perl：正则捕获
来源：http://xl.gzmigu.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://hf.yuntaijiaju.cn

[T48] Perl：正则替换
来源：http://wd.szsharing.cn

$s =~ s/old/new/g;
来源：http://eq.wgjwhj.cn

[T49] Perl：函数
来源：http://bq.huixiangedu.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mg.hahajie.cn

[T50] Perl：逐行读文件
来源：http://fu.jianghongdianzi.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://fn.jianghongdianzi.cn

while (my $line = <$fh>) { print $line; }
来源：http://fq.panjiajie.cn

[T51] Scala：Hello World
来源：http://eh.yuntaijiaju.cn

println("Hello")
来源：http://fh.shtwfgs.cn

[T52] Scala：变量
来源：http://jq.asd995.cn

val a = 1;  var b = 2
来源：http://ec.bjjhwx.cn

[T53] Scala：字符串插值
来源：http://si.newstarts.cn

s"值: $b"
来源：http://ap.huanxung.cn

[T54] Scala：集合映射
来源：http://iw.bjjhwx.cn

List(1, 2, 3).map(_ * 2)
来源：http://pm.yuntaijiaju.cn

[T55] Scala：集合过滤
来源：http://zw.wgjwhj.cn

List(1, 2, 3).filter(_ > 1)
来源：http://nc.huixiangedu.cn

[T56] Scala：样例类
来源：http://pg.bookmarksfly.cn

case class User(name: String, age: Int)
来源：http://bd.muxihuayi.cn

[T57] Scala：模式匹配
来源：http://nc.shxzukj.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://hg.huanxung.cn

[T58] Scala：函数定义
来源：http://cu.asd995.cn


<!-- 参考信息 -->