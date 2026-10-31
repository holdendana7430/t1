代发 wailian999

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://sc.shtwfgs.cn

[R56] 远程拷贝
来源：http://lk.bjjhwx.cn

scp file user@host:/path/
来源：http://mb.gzmigu.cn

[R57] 远程执行命令
来源：http://am.hnjuh.cn

ssh user@host 'uptime'
来源：http://lp.wgjwhj.cn

[R58] 下载文件
来源：http://hu.lnxyls.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://lu.chemitech.net.cn

[R59] 发 POST JSON
来源：http://at.9csxet.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://bq.asd995.cn

[R60] 只看 HTTP 状态码
来源：http://wy.huixiangedu.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://pw.nicolike.cn

[R61] 磁盘占用
来源：http://su.chemitech.net.cn

df -h;  du -sh *
来源：http://wi.yuntaijiaju.cn

[R62] 找最占空间的文件
来源：http://ig.shxzukj.cn

du -ah . | sort -rh | head -10
来源：http://hq.huanxung.cn

[R63] 内存与进程
来源：http://va.hahajie.cn

free -h;  ps aux | grep nginx
来源：http://kl.nszjky.cn

[R64] 结束进程
来源：http://mk.huanxung.cn

kill -9 $(pgrep -f app.py)
来源：http://wt.nszjky.cn

[R65] 查看端口占用
来源：http://su.jianghongdianzi.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://wp.chemitech.net.cn

[R66] 定时任务
来源：http://ua.shxzskj.cn

crontab -e;  crontab -l
来源：http://wh.jctech888.com.cn

[R67] 生成随机十六进制串
来源：http://ns.muxihuayi.cn

openssl rand -hex 16
来源：http://bv.gzmigu.cn

[R68] 计算文件校验值
来源：http://ez.shxzskj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://rc.muxihuayi.cn

[R69] 生成随机密码
来源：http://xl.wgjwhj.cn

head -c 16 /dev/urandom | base64
来源：http://sj.wgjwhj.cn

[R70] 时间戳与互转
来源：http://pf.shxzukj.cn

date +%s;  date -d @1700000000
来源：http://nc.wgjwhj.cn

[R71] 日期格式化
来源：http://gf.huanxung.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://cg.asd995.cn

[R72] 等待端口就绪
来源：http://rc.colortex.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://yj.asd995.cn

[R73] 分割大日志
来源：http://qe.colortex.cn

split -l 1000 big.log part_
来源：http://sg.huixinmuqiang.cn

[R74] 批量重命名
来源：http://hi.huixinmuqiang.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://se.lnxyls.cn

[R75] 导出环境变量
来源：http://lk.asd995.cn

export PATH="$HOME/bin:$PATH"
来源：http://tn.hahajie.cn

[R76] 使用临时文件
来源：http://ub.nicolike.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://it.bjjhwx.cn

[R77] 读取用户输入
来源：http://qn.shtwfgs.cn

read -rp "请输入: " ans
来源：http://jk.jctech888.com.cn

[R78] 交互式菜单
来源：http://km.bookmarksfly.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://rt.9csxet.cn

[R79] 解析命令行选项
来源：http://av.shxzskj.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://kk.shxzukj.cn

[R80] 查看脚本执行耗时
来源：http://yq.9csxet.cn

time ./run.sh
来源：http://dv.huixinmuqiang.cn

================================================================================
来源：http://ga.muxihuayi.cn

S. C / C++ 专题
来源：http://mn.jctech888.com.cn

================================================================================
来源：http://gd.muxihuayi.cn

[S01] C：Hello World
来源：http://ib.panjiajie.cn

#include <stdio.h>
来源：http://gh.nszjky.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ta.huanxung.cn

[S02] C：变量与格式化输出
来源：http://cl.gzmigu.cn

int a = 10; printf("%d\n", a);
来源：http://pu.huixiangedu.cn

[S03] C：读入整数
来源：http://zf.chemitech.net.cn

int x; scanf("%d", &x);
来源：http://yl.bjjhwx.cn

[S04] C：字符串复制
来源：http://et.gzmigu.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ro.huixinmuqiang.cn

[S05] C：字符串长度
来源：http://vz.521024.cn

strlen(s)
来源：http://xg.shxzskj.cn

[S06] C：字符串比较
来源：http://br.shtwfgs.cn

strcmp(a, b) == 0
来源：http://xl.szsharing.cn

[S07] C：数组遍历求和
来源：http://vg.lnxyls.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mb.huixiangedu.cn

[S08] C：动态内存分配与释放
来源：http://qk.bjjhwx.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://qv.asd995.cn

[S09] C：结构体定义与初始化
来源：http://hc.muxihuayi.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://sh.newstarts.cn

[S10] C：指针与解引用
来源：http://fn.muxihuayi.cn

int *p = &a;  *p = 5;
来源：http://xt.szxytkj.cn

[S11] C：逐行读文件
来源：http://zv.szxytkj.cn

FILE *f = fopen("a.txt", "r");
来源：http://vz.yuexingan06.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ai.yuntaijiaju.cn

fclose(f);
来源：http://fn.hahajie.cn

[S12] C：写文件
来源：http://qx.huixinmuqiang.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://so.huixinmuqiang.cn

[S13] C：宏定义
来源：http://wt.shtwfgs.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://uk.gzmigu.cn

[S14] C：枚举
来源：http://my.9csxet.cn

enum Color { RED, GREEN, BLUE };
来源：http://bt.shxzskj.cn

[S15] C：类型转换
来源：http://ow.jianghongdianzi.cn

(double) a / b
来源：http://sk.shtwfgs.cn

[S16] C：位操作置位
来源：http://bm.jianghongdianzi.cn

x |= (1 << 3);
来源：http://pc.huixiangedu.cn

[S17] C：安全拼接字符串
来源：http://fw.9csxet.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ci.gzmigu.cn

[S18] C：命令行参数
来源：http://qy.chemitech.net.cn

int main(int argc, char **argv)
来源：http://oy.panjiajie.cn

[S19] C：快速排序
来源：http://jn.nszjky.cn

qsort(a, n, sizeof(int), cmp);
来源：http://gw.hahajie.cn

[S20] C：二分查找
来源：http://df.szxytkj.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://tu.szsharing.cn

[S21] C：字符类别判断
来源：http://nl.haigaiapp.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://la.hnjuh.cn

[S22] C：字符串转数字
来源：http://tk.panjiajie.cn

atoi("42");  strtod("3.14", NULL);
来源：http://fz.colortex.cn

[S23] C：随机数
来源：http://ss.bjjhwx.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ag.huixiangedu.cn

[S24] C：获取本地时间
来源：http://um.wgjwhj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://im.wgjwhj.cn

[S25] C：内存拷贝
来源：http://mq.hahajie.cn

memcpy(dst, src, n);
来源：http://ta.huanxung.cn

[S26] C：内存清零
来源：http://gx.asd995.cn

memset(a, 0, sizeof a);
来源：http://nh.muxihuayi.cn

[S27] C：定义常量
来源：http://vo.colortex.cn

const double PI = 3.14159;
来源：http://ni.bookmarksfly.cn

[S28] C：静态变量
来源：http://rl.lnxyls.cn

static int counter = 0;
来源：http://rt.yuexingan06.cn

[S29] C：变参函数
来源：http://yz.szxytkj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://da.jctech888.com.cn

[S30] C：头文件保护
来源：http://ii.shxzukj.cn

#ifndef X_H
来源：http://og.nicolike.cn

#define X_H
来源：http://ce.newstarts.cn

#endif
来源：http://lo.huixinmuqiang.cn

[S31] C++：Hello World
来源：http://mh.9csxet.cn

#include <iostream>
来源：http://vx.chemitech.net.cn

int main() { std::cout << "Hello\n"; }
来源：http://ia.9csxet.cn

[S32] C++：字符串
来源：http://ww.muxihuayi.cn

std::string s = "hi";  s += "!";
来源：http://nh.jctech888.com.cn

[S33] C++：vector 增删
来源：http://fo.shxzskj.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://sv.shxzskj.cn

[S34] C++：遍历 vector
来源：http://kg.haigaiapp.cn

for (auto &x : v) { std::cout << x; }
来源：http://pz.muxihuayi.cn

[S35] C++：map
来源：http://hv.shtwfgs.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://yc.haigaiapp.cn

[S36] C++：unordered_map
来源：http://ds.haigaiapp.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ee.haigaiapp.cn

[S37] C++：set
来源：http://pv.9csxet.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://bt.jctech888.com.cn

[S38] C++：排序
来源：http://wq.hahajie.cn

std::sort(v.begin(), v.end());
来源：http://kp.chemitech.net.cn

[S39] C++：自定义比较器排序
来源：http://az.521024.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://du.huixiangedu.cn

[S40] C++：查找元素
来源：http://xf.nszjky.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://tb.9csxet.cn

[S41] C++：类与构造函数
来源：http://gi.huixinmuqiang.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://og.yuexingan06.cn

[S42] C++：继承与虚函数
来源：http://vn.shxzskj.cn

class B : public Base { public: void f() override {} };
来源：http://qf.shtwfgs.cn

[S43] C++：智能指针
来源：http://xk.colortex.cn

auto p = std::make_unique<int>(5);
来源：http://ea.huixinmuqiang.cn

[S44] C++：引用传参
来源：http://uz.bookmarksfly.cn

void inc(int &x) { ++x; }
来源：http://gn.huixiangedu.cn

[S45] C++：lambda
来源：http://nf.szsharing.cn

auto add = [](int a, int b) { return a + b; };
来源：http://zx.shtwfgs.cn

[S46] C++：函数模板
来源：http://nc.nicolike.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://re.huixiangedu.cn

[S47] C++：结构化绑定遍历
来源：http://db.521024.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://lh.asd995.cn

[S48] C++：逐行读文件
来源：http://fx.panjiajie.cn

std::ifstream in("a.txt");  std::string line;
来源：http://dx.chemitech.net.cn

while (std::getline(in, line)) { }
来源：http://tf.colortex.cn

[S49] C++：写文件
来源：http://hf.shxzukj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://gu.yuntaijiaju.cn

[S50] C++：格式化数字
来源：http://jl.bjjhwx.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://es.muxihuayi.cn

[S51] C++：显式类型转换
来源：http://mx.bjjhwx.cn

static_cast<double>(a) / b
来源：http://jg.haigaiapp.cn

[S52] C++：const 与 noexcept
来源：http://fy.huixiangedu.cn

int size() const noexcept { return n_; }
来源：http://tq.gzmigu.cn

[S53] C++：移动语义
来源：http://ve.yuexingan06.cn

std::vector<int> w = std::move(v);
来源：http://li.wgjwhj.cn

[S54] C++：异常处理
来源：http://ys.yuexingan06.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://gp.wgjwhj.cn

[S55] C++：结构化绑定
来源：http://xs.huixinmuqiang.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://gb.bjjhwx.cn

[S56] C++：optional
来源：http://uk.chemitech.net.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://lz.shxzukj.cn

[S57] C++：编译期常量
来源：http://kc.huixinmuqiang.cn

constexpr int N = 10;
来源：http://hd.shtwfgs.cn

[S58] C++：命名空间
来源：http://nd.gzmigu.cn

namespace ns { int f() { return 1; } }
来源：http://ph.bjjhwx.cn

[S59] C++：静态断言
来源：http://qn.yuntaijiaju.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://vc.huanxung.cn

[S60] C++：遍历并删除元素
来源：http://ui.wgjwhj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://up.szsharing.cn

================================================================================
来源：http://rg.huixiangedu.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ds.jianghongdianzi.cn

================================================================================
来源：http://ls.521024.cn

[T01] Kotlin：Hello World
来源：http://od.chemitech.net.cn

println("Hello")
来源：http://pm.muxihuayi.cn

[T02] Kotlin：变量
来源：http://iw.huixinmuqiang.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://uz.chemitech.net.cn

[T03] Kotlin：字符串模板
来源：http://hf.shxzukj.cn

"值: $b"
来源：http://oi.shxzskj.cn

[T04] Kotlin：空安全
来源：http://ca.wgjwhj.cn

val n: String? = null;  n?.length
来源：http://ze.hnjuh.cn

[T05] Kotlin：when 表达式
来源：http://ep.nicolike.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://sw.szsharing.cn

[T06] Kotlin：集合映射
来源：http://zq.yuexingan06.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://lw.yuntaijiaju.cn

[T07] Kotlin：集合过滤
来源：http://rs.shxzskj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://eq.jctech888.com.cn

[T08] Kotlin：数据类
来源：http://hk.hahajie.cn

data class User(val name: String, val age: Int)
来源：http://rs.9csxet.cn

[T09] Kotlin：扩展函数
来源：http://xx.panjiajie.cn

fun String.exclaim() = this + "!"
来源：http://ey.shxzukj.cn

[T10] Kotlin：默认参数
来源：http://tu.panjiajie.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://iw.huixiangedu.cn

[T11] Kotlin：协程
来源：http://af.wgjwhj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://lf.huanxung.cn

[T12] Kotlin：解构声明
来源：http://aq.szxytkj.cn

val (a, b) = Pair(1, 2)
来源：http://sc.panjiajie.cn

[T13] Kotlin：只读 Map
来源：http://iu.chemitech.net.cn

val m = mapOf("a" to 1)
来源：http://dr.gzmigu.cn

[T14] Kotlin：循环
来源：http://zh.nszjky.cn

for (i in 1..10) println(i)
来源：http://kn.nszjky.cn

[T15] Kotlin：接口
来源：http://ml.bookmarksfly.cn

interface Shape { fun area(): Double }
来源：http://xv.hnjuh.cn

[T16] Swift：Hello World
来源：http://ne.yuexingan06.cn

print("Hello")
来源：http://co.szsharing.cn

[T17] Swift：变量与常量
来源：http://vg.colortex.cn

var a = 1;  let b = 2
来源：http://na.jianghongdianzi.cn

[T18] Swift：字符串插值
来源：http://dm.gzmigu.cn

"值: \(b)"
来源：http://wl.shxzukj.cn

[T19] Swift：可选绑定
来源：http://ld.asd995.cn

if let n = opt { print(n) }
来源：http://pd.wgjwhj.cn

[T20] Swift：数组操作
来源：http://sj.jctech888.com.cn

var a = [1, 2, 3];  a.append(4)
来源：http://xc.bjjhwx.cn

[T21] Swift：遍历
来源：http://wk.shxzskj.cn

for x in a { print(x) }
来源：http://ug.9csxet.cn

[T22] Swift：字典
来源：http://ug.szxytkj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ar.bookmarksfly.cn

[T23] Swift：函数
来源：http://mv.521024.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hu.szxytkj.cn

[T24] Swift：闭包
来源：http://uv.gzmigu.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://xf.nszjky.cn

[T25] Swift：结构体
来源：http://dh.521024.cn

struct P { var x: Int }
来源：http://ly.jctech888.com.cn

[T26] Swift：类与重写
来源：http://aq.asd995.cn

class A: Base { override func f() {} }
来源：http://os.shtwfgs.cn

[T27] Swift：错误处理
来源：http://ve.lnxyls.cn

do { try f() } catch { print(error) }
来源：http://bs.shxzukj.cn

[T28] Swift：枚举
来源：http://nt.jianghongdianzi.cn

enum Color { case red, green }
来源：http://kp.521024.cn

[T29] Swift：guard 提前返回
来源：http://ra.shxzskj.cn

guard let x = opt else { return }
来源：http://wz.hahajie.cn

[T30] Swift：协议
来源：http://as.huixinmuqiang.cn

protocol Shape { func area() -> Double }
来源：http://yk.szxytkj.cn

[T31] Lua：Hello World
来源：http://jj.jctech888.com.cn

print("Hello")
来源：http://qt.gzmigu.cn

[T32] Lua：局部变量
来源：http://pi.bookmarksfly.cn

local a = 1
来源：http://qi.shxzskj.cn

[T33] Lua：表（数组）
来源：http://eq.shtwfgs.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://nl.shxzukj.cn

[T34] Lua：遍历表
来源：http://xi.shtwfgs.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ey.szsharing.cn

[T35] Lua：字典表
来源：http://cb.shxzukj.cn

local d = { a = 1 };  d.b = 2
来源：http://se.bjjhwx.cn

[T36] Lua：函数
来源：http://kx.nszjky.cn

function add(a, b) return a + b end
来源：http://rq.huixinmuqiang.cn

[T37] Lua：字符串拼接
来源：http://xg.shtwfgs.cn

"a" .. "b"
来源：http://ly.521024.cn

[T38] Lua：条件
来源：http://fj.huixinmuqiang.cn

if x > 0 then print("正") end
来源：http://le.shxzskj.cn

[T39] Lua：模式匹配
来源：http://xy.521024.cn

string.find(s, "%d+")
来源：http://zz.jianghongdianzi.cn

[T40] Lua：元表
来源：http://ul.haigaiapp.cn

setmetatable({}, { __index = base })
来源：http://zu.9csxet.cn

[T41] Perl：Hello World
来源：http://lh.521024.cn

print "Hello\n";
来源：http://yy.huixiangedu.cn

[T42] Perl：变量类型
来源：http://uu.huixiangedu.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://kh.chemitech.net.cn

[T43] Perl：字符串插值
来源：http://dk.shxzskj.cn

"值: $a"
来源：http://hl.wgjwhj.cn

[T44] Perl：条件
来源：http://bn.shxzskj.cn

if ($a > 0) { print "正"; }
来源：http://vu.newstarts.cn

[T45] Perl：数组遍历
来源：http://an.hahajie.cn

for my $x (@arr) { print $x; }
来源：http://hj.jctech888.com.cn

[T46] Perl：哈希操作
来源：http://sh.newstarts.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://bk.lnxyls.cn

[T47] Perl：正则捕获
来源：http://cg.yuntaijiaju.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://tq.shxzskj.cn

[T48] Perl：正则替换
来源：http://ei.bookmarksfly.cn

$s =~ s/old/new/g;
来源：http://wp.521024.cn

[T49] Perl：函数
来源：http://wn.haigaiapp.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ul.muxihuayi.cn

[T50] Perl：逐行读文件
来源：http://eq.hnjuh.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ih.szxytkj.cn

while (my $line = <$fh>) { print $line; }
来源：http://tz.yuntaijiaju.cn

[T51] Scala：Hello World
来源：http://nj.colortex.cn

println("Hello")
来源：http://bu.yuntaijiaju.cn

[T52] Scala：变量
来源：http://dl.szxytkj.cn

val a = 1;  var b = 2
来源：http://ll.haigaiapp.cn

[T53] Scala：字符串插值
来源：http://it.chemitech.net.cn

s"值: $b"
来源：http://co.bjjhwx.cn

[T54] Scala：集合映射
来源：http://df.shxzukj.cn

List(1, 2, 3).map(_ * 2)
来源：http://cr.jianghongdianzi.cn

[T55] Scala：集合过滤
来源：http://vv.chemitech.net.cn

List(1, 2, 3).filter(_ > 1)
来源：http://cw.bjjhwx.cn

[T56] Scala：样例类
来源：http://sp.szsharing.cn

case class User(name: String, age: Int)
来源：http://dy.shxzskj.cn

[T57] Scala：模式匹配
来源：http://dk.hnjuh.cn

x match { case 1 => "一"; case _ => "其他" }
来源：http://tw.nicolike.cn

[T58] Scala：函数定义
来源：http://jo.521024.cn


<!-- 参考信息 -->