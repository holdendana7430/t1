代发 wailian999

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://wv.chemitech.net.cn

[R54] 比较两个文件
来源：http://jl.shxzukj.cn

diff a.txt b.txt
来源：http://bc.colortex.cn

[R55] 压缩与解压
来源：http://jg.haigaiapp.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://dn.hahajie.cn

[R56] 远程拷贝
来源：http://bn.jctech888.com.cn

scp file user@host:/path/
来源：http://jv.gzmigu.cn

[R57] 远程执行命令
来源：http://ue.newstarts.cn

ssh user@host 'uptime'
来源：http://ph.nszjky.cn

[R58] 下载文件
来源：http://vo.szsharing.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://fp.huixiangedu.cn

[R59] 发 POST JSON
来源：http://ji.jianghongdianzi.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://cv.newstarts.cn

[R60] 只看 HTTP 状态码
来源：http://tb.huanxung.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://nr.lnxyls.cn

[R61] 磁盘占用
来源：http://ep.shtwfgs.cn

df -h;  du -sh *
来源：http://qb.hnjuh.cn

[R62] 找最占空间的文件
来源：http://cj.wgjwhj.cn

du -ah . | sort -rh | head -10
来源：http://xy.huixinmuqiang.cn

[R63] 内存与进程
来源：http://bf.szxytkj.cn

free -h;  ps aux | grep nginx
来源：http://cb.yuntaijiaju.cn

[R64] 结束进程
来源：http://ef.yuntaijiaju.cn

kill -9 $(pgrep -f app.py)
来源：http://bk.huixinmuqiang.cn

[R65] 查看端口占用
来源：http://ol.bjjhwx.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://xy.jctech888.com.cn

[R66] 定时任务
来源：http://sp.shxzukj.cn

crontab -e;  crontab -l
来源：http://rh.wgjwhj.cn

[R67] 生成随机十六进制串
来源：http://ec.muxihuayi.cn

openssl rand -hex 16
来源：http://zh.gzmigu.cn

[R68] 计算文件校验值
来源：http://mx.haigaiapp.cn

sha256sum a.txt;  md5sum a.txt
来源：http://in.hnjuh.cn

[R69] 生成随机密码
来源：http://yu.nszjky.cn

head -c 16 /dev/urandom | base64
来源：http://yv.haigaiapp.cn

[R70] 时间戳与互转
来源：http://qe.gzmigu.cn

date +%s;  date -d @1700000000
来源：http://hs.shtwfgs.cn

[R71] 日期格式化
来源：http://ji.asd995.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://dy.shtwfgs.cn

[R72] 等待端口就绪
来源：http://ww.jianghongdianzi.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://rl.huanxung.cn

[R73] 分割大日志
来源：http://uh.haigaiapp.cn

split -l 1000 big.log part_
来源：http://uj.shxzukj.cn

[R74] 批量重命名
来源：http://ii.jctech888.com.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://qg.shxzskj.cn

[R75] 导出环境变量
来源：http://jz.newstarts.cn

export PATH="$HOME/bin:$PATH"
来源：http://rg.shxzskj.cn

[R76] 使用临时文件
来源：http://zr.huixinmuqiang.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://yz.szxytkj.cn

[R77] 读取用户输入
来源：http://jf.newstarts.cn

read -rp "请输入: " ans
来源：http://dm.chemitech.net.cn

[R78] 交互式菜单
来源：http://ye.bookmarksfly.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ae.nszjky.cn

[R79] 解析命令行选项
来源：http://uv.jianghongdianzi.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://rq.nicolike.cn

[R80] 查看脚本执行耗时
来源：http://bi.nicolike.cn

time ./run.sh
来源：http://dd.jianghongdianzi.cn

================================================================================
来源：http://ek.wgjwhj.cn

S. C / C++ 专题
来源：http://cv.muxihuayi.cn

================================================================================
来源：http://rh.bjjhwx.cn

[S01] C：Hello World
来源：http://zm.szxytkj.cn

#include <stdio.h>
来源：http://tu.bjjhwx.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://dt.yuntaijiaju.cn

[S02] C：变量与格式化输出
来源：http://mm.huixiangedu.cn

int a = 10; printf("%d\n", a);
来源：http://nx.nicolike.cn

[S03] C：读入整数
来源：http://og.9csxet.cn

int x; scanf("%d", &x);
来源：http://gt.lnxyls.cn

[S04] C：字符串复制
来源：http://js.9csxet.cn

char dst[32]; strcpy(dst, "hi");
来源：http://zs.yuntaijiaju.cn

[S05] C：字符串长度
来源：http://iz.yuntaijiaju.cn

strlen(s)
来源：http://ge.bjjhwx.cn

[S06] C：字符串比较
来源：http://ie.yuexingan06.cn

strcmp(a, b) == 0
来源：http://qv.muxihuayi.cn

[S07] C：数组遍历求和
来源：http://xd.jianghongdianzi.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://gm.bookmarksfly.cn

[S08] C：动态内存分配与释放
来源：http://rd.muxihuayi.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://hc.bookmarksfly.cn

[S09] C：结构体定义与初始化
来源：http://zu.bjjhwx.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://nx.shtwfgs.cn

[S10] C：指针与解引用
来源：http://fq.bjjhwx.cn

int *p = &a;  *p = 5;
来源：http://xj.haigaiapp.cn

[S11] C：逐行读文件
来源：http://iz.asd995.cn

FILE *f = fopen("a.txt", "r");
来源：http://bo.nszjky.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://vq.521024.cn

fclose(f);
来源：http://tq.colortex.cn

[S12] C：写文件
来源：http://ga.wgjwhj.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://fy.wgjwhj.cn

[S13] C：宏定义
来源：http://ds.asd995.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://aj.yuntaijiaju.cn

[S14] C：枚举
来源：http://cv.521024.cn

enum Color { RED, GREEN, BLUE };
来源：http://iv.nszjky.cn

[S15] C：类型转换
来源：http://hn.huixiangedu.cn

(double) a / b
来源：http://ne.nicolike.cn

[S16] C：位操作置位
来源：http://lv.colortex.cn

x |= (1 << 3);
来源：http://uo.9csxet.cn

[S17] C：安全拼接字符串
来源：http://sp.huixinmuqiang.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://nq.asd995.cn

[S18] C：命令行参数
来源：http://kd.lnxyls.cn

int main(int argc, char **argv)
来源：http://yf.9csxet.cn

[S19] C：快速排序
来源：http://to.nicolike.cn

qsort(a, n, sizeof(int), cmp);
来源：http://my.jianghongdianzi.cn

[S20] C：二分查找
来源：http://sh.huixiangedu.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://xh.haigaiapp.cn

[S21] C：字符类别判断
来源：http://ii.bookmarksfly.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://en.yuexingan06.cn

[S22] C：字符串转数字
来源：http://zb.wgjwhj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://az.newstarts.cn

[S23] C：随机数
来源：http://kf.shxzskj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://hr.chemitech.net.cn

[S24] C：获取本地时间
来源：http://wc.nicolike.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ki.9csxet.cn

[S25] C：内存拷贝
来源：http://dt.yuntaijiaju.cn

memcpy(dst, src, n);
来源：http://qf.huixiangedu.cn

[S26] C：内存清零
来源：http://je.jctech888.com.cn

memset(a, 0, sizeof a);
来源：http://kb.gzmigu.cn

[S27] C：定义常量
来源：http://fp.nicolike.cn

const double PI = 3.14159;
来源：http://zt.yuntaijiaju.cn

[S28] C：静态变量
来源：http://aa.521024.cn

static int counter = 0;
来源：http://et.jctech888.com.cn

[S29] C：变参函数
来源：http://rd.hahajie.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://zi.yuexingan06.cn

[S30] C：头文件保护
来源：http://br.huixinmuqiang.cn

#ifndef X_H
来源：http://mb.shxzukj.cn

#define X_H
来源：http://ul.huixinmuqiang.cn

#endif
来源：http://gt.muxihuayi.cn

[S31] C++：Hello World
来源：http://qh.yuntaijiaju.cn

#include <iostream>
来源：http://ro.hnjuh.cn

int main() { std::cout << "Hello\n"; }
来源：http://ni.bookmarksfly.cn

[S32] C++：字符串
来源：http://dm.colortex.cn

std::string s = "hi";  s += "!";
来源：http://ff.hnjuh.cn

[S33] C++：vector 增删
来源：http://pu.bookmarksfly.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://nu.hahajie.cn

[S34] C++：遍历 vector
来源：http://cf.nszjky.cn

for (auto &x : v) { std::cout << x; }
来源：http://bz.jianghongdianzi.cn

[S35] C++：map
来源：http://ic.shtwfgs.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://qg.muxihuayi.cn

[S36] C++：unordered_map
来源：http://xg.colortex.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://rr.shxzskj.cn

[S37] C++：set
来源：http://rf.shtwfgs.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://fi.yuexingan06.cn

[S38] C++：排序
来源：http://bs.huixinmuqiang.cn

std::sort(v.begin(), v.end());
来源：http://bp.521024.cn

[S39] C++：自定义比较器排序
来源：http://nx.521024.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://qo.newstarts.cn

[S40] C++：查找元素
来源：http://bj.muxihuayi.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://kb.bjjhwx.cn

[S41] C++：类与构造函数
来源：http://ir.muxihuayi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://kb.shxzukj.cn

[S42] C++：继承与虚函数
来源：http://pr.jianghongdianzi.cn

class B : public Base { public: void f() override {} };
来源：http://jn.9csxet.cn

[S43] C++：智能指针
来源：http://wy.yuexingan06.cn

auto p = std::make_unique<int>(5);
来源：http://uv.szxytkj.cn

[S44] C++：引用传参
来源：http://wh.nicolike.cn

void inc(int &x) { ++x; }
来源：http://rl.lnxyls.cn

[S45] C++：lambda
来源：http://wk.yuntaijiaju.cn

auto add = [](int a, int b) { return a + b; };
来源：http://hl.szxytkj.cn

[S46] C++：函数模板
来源：http://nk.chemitech.net.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://zs.asd995.cn

[S47] C++：结构化绑定遍历
来源：http://jd.9csxet.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://if.wgjwhj.cn

[S48] C++：逐行读文件
来源：http://be.521024.cn

std::ifstream in("a.txt");  std::string line;
来源：http://uh.yuntaijiaju.cn

while (std::getline(in, line)) { }
来源：http://pb.jctech888.com.cn

[S49] C++：写文件
来源：http://tn.haigaiapp.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://jq.colortex.cn

[S50] C++：格式化数字
来源：http://ba.asd995.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://hz.521024.cn

[S51] C++：显式类型转换
来源：http://wh.colortex.cn

static_cast<double>(a) / b
来源：http://mr.bookmarksfly.cn

[S52] C++：const 与 noexcept
来源：http://bd.wgjwhj.cn

int size() const noexcept { return n_; }
来源：http://vl.lnxyls.cn

[S53] C++：移动语义
来源：http://oz.shtwfgs.cn

std::vector<int> w = std::move(v);
来源：http://fh.haigaiapp.cn

[S54] C++：异常处理
来源：http://si.huixinmuqiang.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://sh.shxzskj.cn

[S55] C++：结构化绑定
来源：http://mm.szxytkj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://wk.asd995.cn

[S56] C++：optional
来源：http://or.gzmigu.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ag.bjjhwx.cn

[S57] C++：编译期常量
来源：http://eq.asd995.cn

constexpr int N = 10;
来源：http://lk.hahajie.cn

[S58] C++：命名空间
来源：http://kw.lnxyls.cn

namespace ns { int f() { return 1; } }
来源：http://hg.huixinmuqiang.cn

[S59] C++：静态断言
来源：http://om.newstarts.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://bi.yuntaijiaju.cn

[S60] C++：遍历并删除元素
来源：http://gk.lnxyls.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ir.shxzskj.cn

================================================================================
来源：http://vg.gzmigu.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://rn.hahajie.cn

================================================================================
来源：http://bu.huixiangedu.cn

[T01] Kotlin：Hello World
来源：http://vq.yuntaijiaju.cn

println("Hello")
来源：http://zx.gzmigu.cn

[T02] Kotlin：变量
来源：http://yo.yuexingan06.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hd.bjjhwx.cn

[T03] Kotlin：字符串模板
来源：http://yo.huixinmuqiang.cn

"值: $b"
来源：http://vd.yuntaijiaju.cn

[T04] Kotlin：空安全
来源：http://sx.521024.cn

val n: String? = null;  n?.length
来源：http://qq.shxzskj.cn

[T05] Kotlin：when 表达式
来源：http://he.nszjky.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ab.szsharing.cn

[T06] Kotlin：集合映射
来源：http://qj.jctech888.com.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://jp.huixiangedu.cn

[T07] Kotlin：集合过滤
来源：http://pl.huixiangedu.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://vy.521024.cn

[T08] Kotlin：数据类
来源：http://wi.newstarts.cn

data class User(val name: String, val age: Int)
来源：http://ul.szxytkj.cn

[T09] Kotlin：扩展函数
来源：http://ta.bjjhwx.cn

fun String.exclaim() = this + "!"
来源：http://hn.huixinmuqiang.cn

[T10] Kotlin：默认参数
来源：http://lj.colortex.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://rz.jctech888.com.cn

[T11] Kotlin：协程
来源：http://pf.lnxyls.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://jb.nszjky.cn

[T12] Kotlin：解构声明
来源：http://sh.colortex.cn

val (a, b) = Pair(1, 2)
来源：http://yx.huixiangedu.cn

[T13] Kotlin：只读 Map
来源：http://xh.9csxet.cn

val m = mapOf("a" to 1)
来源：http://qb.newstarts.cn

[T14] Kotlin：循环
来源：http://bf.huixinmuqiang.cn

for (i in 1..10) println(i)
来源：http://fh.shxzukj.cn

[T15] Kotlin：接口
来源：http://zl.wgjwhj.cn

interface Shape { fun area(): Double }
来源：http://gi.szsharing.cn

[T16] Swift：Hello World
来源：http://ck.hahajie.cn

print("Hello")
来源：http://ap.huixiangedu.cn

[T17] Swift：变量与常量
来源：http://vx.haigaiapp.cn

var a = 1;  let b = 2
来源：http://fv.nszjky.cn

[T18] Swift：字符串插值
来源：http://la.newstarts.cn

"值: \(b)"
来源：http://dk.muxihuayi.cn

[T19] Swift：可选绑定
来源：http://or.newstarts.cn

if let n = opt { print(n) }
来源：http://gj.jctech888.com.cn

[T20] Swift：数组操作
来源：http://jr.shxzukj.cn

var a = [1, 2, 3];  a.append(4)
来源：http://xl.huixinmuqiang.cn

[T21] Swift：遍历
来源：http://ma.521024.cn

for x in a { print(x) }
来源：http://it.huanxung.cn

[T22] Swift：字典
来源：http://ms.yuntaijiaju.cn

var d = ["a": 1];  d["b"] = 2
来源：http://oa.hahajie.cn

[T23] Swift：函数
来源：http://yb.haigaiapp.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://hy.shtwfgs.cn

[T24] Swift：闭包
来源：http://qh.bookmarksfly.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://yl.hnjuh.cn

[T25] Swift：结构体
来源：http://xb.nicolike.cn

struct P { var x: Int }
来源：http://um.nicolike.cn

[T26] Swift：类与重写
来源：http://so.nszjky.cn

class A: Base { override func f() {} }
来源：http://wa.asd995.cn

[T27] Swift：错误处理
来源：http://gj.hahajie.cn

do { try f() } catch { print(error) }
来源：http://ml.jctech888.com.cn

[T28] Swift：枚举
来源：http://mf.shxzskj.cn

enum Color { case red, green }
来源：http://fe.haigaiapp.cn

[T29] Swift：guard 提前返回
来源：http://ex.lnxyls.cn

guard let x = opt else { return }
来源：http://bo.huanxung.cn

[T30] Swift：协议
来源：http://dy.chemitech.net.cn

protocol Shape { func area() -> Double }
来源：http://wy.wgjwhj.cn

[T31] Lua：Hello World
来源：http://yq.yuexingan06.cn

print("Hello")
来源：http://qg.yuntaijiaju.cn

[T32] Lua：局部变量
来源：http://gw.521024.cn

local a = 1
来源：http://md.haigaiapp.cn

[T33] Lua：表（数组）
来源：http://ww.shxzskj.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://mr.asd995.cn

[T34] Lua：遍历表
来源：http://bi.gzmigu.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://bs.haigaiapp.cn

[T35] Lua：字典表
来源：http://jw.lnxyls.cn

local d = { a = 1 };  d.b = 2
来源：http://up.jianghongdianzi.cn

[T36] Lua：函数
来源：http://hq.bjjhwx.cn

function add(a, b) return a + b end
来源：http://na.shxzskj.cn

[T37] Lua：字符串拼接
来源：http://ey.shxzukj.cn

"a" .. "b"
来源：http://wr.panjiajie.cn

[T38] Lua：条件
来源：http://wv.shxzukj.cn

if x > 0 then print("正") end
来源：http://np.huixinmuqiang.cn

[T39] Lua：模式匹配
来源：http://bp.jctech888.com.cn

string.find(s, "%d+")
来源：http://ab.haigaiapp.cn

[T40] Lua：元表
来源：http://sg.newstarts.cn

setmetatable({}, { __index = base })
来源：http://ms.wgjwhj.cn

[T41] Perl：Hello World
来源：http://ik.muxihuayi.cn

print "Hello\n";
来源：http://jj.bookmarksfly.cn

[T42] Perl：变量类型
来源：http://dk.lnxyls.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://qs.wgjwhj.cn

[T43] Perl：字符串插值
来源：http://nw.shtwfgs.cn

"值: $a"
来源：http://da.nszjky.cn

[T44] Perl：条件
来源：http://zu.huanxung.cn

if ($a > 0) { print "正"; }
来源：http://tr.bookmarksfly.cn

[T45] Perl：数组遍历
来源：http://pe.huanxung.cn

for my $x (@arr) { print $x; }
来源：http://mu.lnxyls.cn

[T46] Perl：哈希操作
来源：http://fx.hahajie.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ap.chemitech.net.cn

[T47] Perl：正则捕获
来源：http://ui.shxzskj.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://kz.panjiajie.cn

[T48] Perl：正则替换
来源：http://fr.muxihuayi.cn

$s =~ s/old/new/g;
来源：http://cc.chemitech.net.cn

[T49] Perl：函数
来源：http://qf.wgjwhj.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://xg.jianghongdianzi.cn

[T50] Perl：逐行读文件
来源：http://xn.gzmigu.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://sr.bookmarksfly.cn

while (my $line = <$fh>) { print $line; }
来源：http://ge.yuexingan06.cn

[T51] Scala：Hello World
来源：http://ke.szsharing.cn

println("Hello")
来源：http://yx.yuntaijiaju.cn

[T52] Scala：变量
来源：http://fk.shxzskj.cn

val a = 1;  var b = 2
来源：http://zo.szxytkj.cn

[T53] Scala：字符串插值
来源：http://ko.panjiajie.cn

s"值: $b"
来源：http://eg.shxzskj.cn

[T54] Scala：集合映射
来源：http://ep.wgjwhj.cn

List(1, 2, 3).map(_ * 2)
来源：http://br.bjjhwx.cn

[T55] Scala：集合过滤
来源：http://tf.gzmigu.cn

List(1, 2, 3).filter(_ > 1)
来源：http://sq.wgjwhj.cn

[T56] Scala：样例类
来源：http://aw.shtwfgs.cn


<!-- 参考信息 -->