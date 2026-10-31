代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://sp.lnxyls.cn

[R52] 统计行数
来源：http://vy.asd995.cn

wc -l a.txt
来源：http://nk.newstarts.cn

[R53] 查看文件头与实时尾
来源：http://zm.colortex.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://pp.chemitech.net.cn

[R54] 比较两个文件
来源：http://hk.colortex.cn

diff a.txt b.txt
来源：http://gy.gzmigu.cn

[R55] 压缩与解压
来源：http://le.szsharing.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://hj.lnxyls.cn

[R56] 远程拷贝
来源：http://ah.nicolike.cn

scp file user@host:/path/
来源：http://fr.gzmigu.cn

[R57] 远程执行命令
来源：http://vp.yuntaijiaju.cn

ssh user@host 'uptime'
来源：http://cw.huixinmuqiang.cn

[R58] 下载文件
来源：http://sm.521024.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://yl.bookmarksfly.cn

[R59] 发 POST JSON
来源：http://is.nszjky.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ih.chemitech.net.cn

[R60] 只看 HTTP 状态码
来源：http://si.nicolike.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ky.szsharing.cn

[R61] 磁盘占用
来源：http://yt.muxihuayi.cn

df -h;  du -sh *
来源：http://ai.521024.cn

[R62] 找最占空间的文件
来源：http://jz.szxytkj.cn

du -ah . | sort -rh | head -10
来源：http://qc.haigaiapp.cn

[R63] 内存与进程
来源：http://tj.hnjuh.cn

free -h;  ps aux | grep nginx
来源：http://ox.lnxyls.cn

[R64] 结束进程
来源：http://nm.asd995.cn

kill -9 $(pgrep -f app.py)
来源：http://zo.huixiangedu.cn

[R65] 查看端口占用
来源：http://rx.yuexingan06.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://qo.nicolike.cn

[R66] 定时任务
来源：http://cj.muxihuayi.cn

crontab -e;  crontab -l
来源：http://tn.nszjky.cn

[R67] 生成随机十六进制串
来源：http://sb.gzmigu.cn

openssl rand -hex 16
来源：http://ft.asd995.cn

[R68] 计算文件校验值
来源：http://jl.nicolike.cn

sha256sum a.txt;  md5sum a.txt
来源：http://vj.shxzskj.cn

[R69] 生成随机密码
来源：http://od.jctech888.com.cn

head -c 16 /dev/urandom | base64
来源：http://xb.jctech888.com.cn

[R70] 时间戳与互转
来源：http://uy.jianghongdianzi.cn

date +%s;  date -d @1700000000
来源：http://iy.huixinmuqiang.cn

[R71] 日期格式化
来源：http://dn.yuexingan06.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://wq.colortex.cn

[R72] 等待端口就绪
来源：http://jj.asd995.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://zb.jianghongdianzi.cn

[R73] 分割大日志
来源：http://or.lnxyls.cn

split -l 1000 big.log part_
来源：http://nv.hnjuh.cn

[R74] 批量重命名
来源：http://jm.chemitech.net.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://wa.hnjuh.cn

[R75] 导出环境变量
来源：http://ob.9csxet.cn

export PATH="$HOME/bin:$PATH"
来源：http://ns.yuntaijiaju.cn

[R76] 使用临时文件
来源：http://uv.asd995.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ix.panjiajie.cn

[R77] 读取用户输入
来源：http://bd.nszjky.cn

read -rp "请输入: " ans
来源：http://mi.newstarts.cn

[R78] 交互式菜单
来源：http://aw.szxytkj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://rs.szxytkj.cn

[R79] 解析命令行选项
来源：http://ps.yuexingan06.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://qu.jctech888.com.cn

[R80] 查看脚本执行耗时
来源：http://ss.huixiangedu.cn

time ./run.sh
来源：http://rn.yuntaijiaju.cn

================================================================================
来源：http://eq.huanxung.cn

S. C / C++ 专题
来源：http://zs.lnxyls.cn

================================================================================
来源：http://hq.shxzukj.cn

[S01] C：Hello World
来源：http://st.shxzukj.cn

#include <stdio.h>
来源：http://wu.jctech888.com.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://nl.jctech888.com.cn

[S02] C：变量与格式化输出
来源：http://bg.hnjuh.cn

int a = 10; printf("%d\n", a);
来源：http://ui.gzmigu.cn

[S03] C：读入整数
来源：http://fg.9csxet.cn

int x; scanf("%d", &x);
来源：http://vt.9csxet.cn

[S04] C：字符串复制
来源：http://ye.muxihuayi.cn

char dst[32]; strcpy(dst, "hi");
来源：http://cl.521024.cn

[S05] C：字符串长度
来源：http://ab.nszjky.cn

strlen(s)
来源：http://ff.chemitech.net.cn

[S06] C：字符串比较
来源：http://ue.shtwfgs.cn

strcmp(a, b) == 0
来源：http://qo.nszjky.cn

[S07] C：数组遍历求和
来源：http://yn.asd995.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://fh.huanxung.cn

[S08] C：动态内存分配与释放
来源：http://fc.bjjhwx.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://pw.jianghongdianzi.cn

[S09] C：结构体定义与初始化
来源：http://nj.chemitech.net.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://gc.colortex.cn

[S10] C：指针与解引用
来源：http://th.wgjwhj.cn

int *p = &a;  *p = 5;
来源：http://pp.yuntaijiaju.cn

[S11] C：逐行读文件
来源：http://jm.panjiajie.cn

FILE *f = fopen("a.txt", "r");
来源：http://oj.haigaiapp.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://wa.panjiajie.cn

fclose(f);
来源：http://in.bjjhwx.cn

[S12] C：写文件
来源：http://oj.jctech888.com.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://fa.panjiajie.cn

[S13] C：宏定义
来源：http://hm.asd995.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ce.panjiajie.cn

[S14] C：枚举
来源：http://ym.hnjuh.cn

enum Color { RED, GREEN, BLUE };
来源：http://tb.szsharing.cn

[S15] C：类型转换
来源：http://bv.bjjhwx.cn

(double) a / b
来源：http://gp.jianghongdianzi.cn

[S16] C：位操作置位
来源：http://ro.newstarts.cn

x |= (1 << 3);
来源：http://wq.huixinmuqiang.cn

[S17] C：安全拼接字符串
来源：http://tn.hnjuh.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://dp.bjjhwx.cn

[S18] C：命令行参数
来源：http://bj.shtwfgs.cn

int main(int argc, char **argv)
来源：http://nu.shxzskj.cn

[S19] C：快速排序
来源：http://qi.521024.cn

qsort(a, n, sizeof(int), cmp);
来源：http://wy.yuntaijiaju.cn

[S20] C：二分查找
来源：http://xs.szsharing.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wl.wgjwhj.cn

[S21] C：字符类别判断
来源：http://cv.chemitech.net.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://zo.gzmigu.cn

[S22] C：字符串转数字
来源：http://ud.yuntaijiaju.cn

atoi("42");  strtod("3.14", NULL);
来源：http://tv.huixiangedu.cn

[S23] C：随机数
来源：http://ub.wgjwhj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://yp.jianghongdianzi.cn

[S24] C：获取本地时间
来源：http://im.yuntaijiaju.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://pg.521024.cn

[S25] C：内存拷贝
来源：http://nl.hahajie.cn

memcpy(dst, src, n);
来源：http://yk.hnjuh.cn

[S26] C：内存清零
来源：http://np.colortex.cn

memset(a, 0, sizeof a);
来源：http://mo.jianghongdianzi.cn

[S27] C：定义常量
来源：http://ft.colortex.cn

const double PI = 3.14159;
来源：http://qg.shxzukj.cn

[S28] C：静态变量
来源：http://ag.muxihuayi.cn

static int counter = 0;
来源：http://nv.asd995.cn

[S29] C：变参函数
来源：http://tn.huanxung.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://yd.newstarts.cn

[S30] C：头文件保护
来源：http://sh.szxytkj.cn

#ifndef X_H
来源：http://mk.jctech888.com.cn

#define X_H
来源：http://hm.yuntaijiaju.cn

#endif
来源：http://fi.huanxung.cn

[S31] C++：Hello World
来源：http://tl.huanxung.cn

#include <iostream>
来源：http://ql.gzmigu.cn

int main() { std::cout << "Hello\n"; }
来源：http://ie.hnjuh.cn

[S32] C++：字符串
来源：http://co.jianghongdianzi.cn

std::string s = "hi";  s += "!";
来源：http://zf.huixiangedu.cn

[S33] C++：vector 增删
来源：http://uo.yuntaijiaju.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://aj.nicolike.cn

[S34] C++：遍历 vector
来源：http://xq.yuexingan06.cn

for (auto &x : v) { std::cout << x; }
来源：http://fe.szxytkj.cn

[S35] C++：map
来源：http://hq.nszjky.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://wy.lnxyls.cn

[S36] C++：unordered_map
来源：http://pt.yuexingan06.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://xs.yuexingan06.cn

[S37] C++：set
来源：http://qt.9csxet.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://on.szsharing.cn

[S38] C++：排序
来源：http://vy.yuexingan06.cn

std::sort(v.begin(), v.end());
来源：http://gs.nicolike.cn

[S39] C++：自定义比较器排序
来源：http://af.yuntaijiaju.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ja.newstarts.cn

[S40] C++：查找元素
来源：http://gw.asd995.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mr.muxihuayi.cn

[S41] C++：类与构造函数
来源：http://jk.huanxung.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://jc.huixinmuqiang.cn

[S42] C++：继承与虚函数
来源：http://ys.shtwfgs.cn

class B : public Base { public: void f() override {} };
来源：http://bg.panjiajie.cn

[S43] C++：智能指针
来源：http://ez.huixinmuqiang.cn

auto p = std::make_unique<int>(5);
来源：http://xu.panjiajie.cn

[S44] C++：引用传参
来源：http://kr.colortex.cn

void inc(int &x) { ++x; }
来源：http://mt.nicolike.cn

[S45] C++：lambda
来源：http://el.gzmigu.cn

auto add = [](int a, int b) { return a + b; };
来源：http://fg.shtwfgs.cn

[S46] C++：函数模板
来源：http://jn.szsharing.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://vi.muxihuayi.cn

[S47] C++：结构化绑定遍历
来源：http://zl.gzmigu.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://lh.shxzukj.cn

[S48] C++：逐行读文件
来源：http://hh.hnjuh.cn

std::ifstream in("a.txt");  std::string line;
来源：http://dt.haigaiapp.cn

while (std::getline(in, line)) { }
来源：http://lm.shxzukj.cn

[S49] C++：写文件
来源：http://hh.bjjhwx.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://cd.shxzskj.cn

[S50] C++：格式化数字
来源：http://iz.chemitech.net.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://md.nszjky.cn

[S51] C++：显式类型转换
来源：http://cn.nicolike.cn

static_cast<double>(a) / b
来源：http://me.szxytkj.cn

[S52] C++：const 与 noexcept
来源：http://pu.szxytkj.cn

int size() const noexcept { return n_; }
来源：http://pw.wgjwhj.cn

[S53] C++：移动语义
来源：http://ui.asd995.cn

std::vector<int> w = std::move(v);
来源：http://di.jianghongdianzi.cn

[S54] C++：异常处理
来源：http://uz.asd995.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://kw.nicolike.cn

[S55] C++：结构化绑定
来源：http://ln.jctech888.com.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://os.521024.cn

[S56] C++：optional
来源：http://ei.colortex.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://nx.shxzukj.cn

[S57] C++：编译期常量
来源：http://ve.haigaiapp.cn

constexpr int N = 10;
来源：http://yc.huixiangedu.cn

[S58] C++：命名空间
来源：http://vd.shxzskj.cn

namespace ns { int f() { return 1; } }
来源：http://wr.bookmarksfly.cn

[S59] C++：静态断言
来源：http://qd.shxzukj.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://tg.shxzukj.cn

[S60] C++：遍历并删除元素
来源：http://ls.szsharing.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://dm.shtwfgs.cn

================================================================================
来源：http://ei.huixiangedu.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://iu.shxzukj.cn

================================================================================
来源：http://gl.asd995.cn

[T01] Kotlin：Hello World
来源：http://tg.muxihuayi.cn

println("Hello")
来源：http://eu.szxytkj.cn

[T02] Kotlin：变量
来源：http://lr.521024.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://bk.szsharing.cn

[T03] Kotlin：字符串模板
来源：http://py.jianghongdianzi.cn

"值: $b"
来源：http://kf.521024.cn

[T04] Kotlin：空安全
来源：http://nj.asd995.cn

val n: String? = null;  n?.length
来源：http://kq.haigaiapp.cn

[T05] Kotlin：when 表达式
来源：http://yz.haigaiapp.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://sf.shxzukj.cn

[T06] Kotlin：集合映射
来源：http://xv.huanxung.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://io.shtwfgs.cn

[T07] Kotlin：集合过滤
来源：http://ht.jctech888.com.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://cq.huixiangedu.cn

[T08] Kotlin：数据类
来源：http://ss.lnxyls.cn

data class User(val name: String, val age: Int)
来源：http://dh.wgjwhj.cn

[T09] Kotlin：扩展函数
来源：http://to.huixinmuqiang.cn

fun String.exclaim() = this + "!"
来源：http://pv.9csxet.cn

[T10] Kotlin：默认参数
来源：http://ns.colortex.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ag.jctech888.com.cn

[T11] Kotlin：协程
来源：http://ik.shtwfgs.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://gx.szsharing.cn

[T12] Kotlin：解构声明
来源：http://jf.9csxet.cn

val (a, b) = Pair(1, 2)
来源：http://rr.shxzukj.cn

[T13] Kotlin：只读 Map
来源：http://po.hnjuh.cn

val m = mapOf("a" to 1)
来源：http://uh.hahajie.cn

[T14] Kotlin：循环
来源：http://wh.bookmarksfly.cn

for (i in 1..10) println(i)
来源：http://om.bjjhwx.cn

[T15] Kotlin：接口
来源：http://sa.huixinmuqiang.cn

interface Shape { fun area(): Double }
来源：http://vq.hnjuh.cn

[T16] Swift：Hello World
来源：http://xg.bookmarksfly.cn

print("Hello")
来源：http://zn.szsharing.cn

[T17] Swift：变量与常量
来源：http://ml.yuexingan06.cn

var a = 1;  let b = 2
来源：http://xc.szsharing.cn

[T18] Swift：字符串插值
来源：http://bl.521024.cn

"值: \(b)"
来源：http://fw.lnxyls.cn

[T19] Swift：可选绑定
来源：http://rl.jianghongdianzi.cn

if let n = opt { print(n) }
来源：http://jv.szxytkj.cn

[T20] Swift：数组操作
来源：http://yv.wgjwhj.cn

var a = [1, 2, 3];  a.append(4)
来源：http://me.hnjuh.cn

[T21] Swift：遍历
来源：http://xx.bookmarksfly.cn

for x in a { print(x) }
来源：http://an.asd995.cn

[T22] Swift：字典
来源：http://fd.panjiajie.cn

var d = ["a": 1];  d["b"] = 2
来源：http://my.bjjhwx.cn

[T23] Swift：函数
来源：http://jz.haigaiapp.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://xu.colortex.cn

[T24] Swift：闭包
来源：http://ea.gzmigu.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://vz.wgjwhj.cn

[T25] Swift：结构体
来源：http://bg.jianghongdianzi.cn

struct P { var x: Int }
来源：http://tx.szxytkj.cn

[T26] Swift：类与重写
来源：http://ak.9csxet.cn

class A: Base { override func f() {} }
来源：http://gv.hahajie.cn

[T27] Swift：错误处理
来源：http://cu.9csxet.cn

do { try f() } catch { print(error) }
来源：http://lk.shtwfgs.cn

[T28] Swift：枚举
来源：http://dn.shxzskj.cn

enum Color { case red, green }
来源：http://ns.gzmigu.cn

[T29] Swift：guard 提前返回
来源：http://ee.shxzskj.cn

guard let x = opt else { return }
来源：http://cw.bjjhwx.cn

[T30] Swift：协议
来源：http://tu.asd995.cn

protocol Shape { func area() -> Double }
来源：http://mt.newstarts.cn

[T31] Lua：Hello World
来源：http://jr.wgjwhj.cn

print("Hello")
来源：http://gm.shxzukj.cn

[T32] Lua：局部变量
来源：http://bc.bookmarksfly.cn

local a = 1
来源：http://pk.hnjuh.cn

[T33] Lua：表（数组）
来源：http://kg.nszjky.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://pw.huixinmuqiang.cn

[T34] Lua：遍历表
来源：http://qm.haigaiapp.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://jg.jctech888.com.cn

[T35] Lua：字典表
来源：http://tv.shxzskj.cn

local d = { a = 1 };  d.b = 2
来源：http://np.yuexingan06.cn

[T36] Lua：函数
来源：http://fs.bookmarksfly.cn

function add(a, b) return a + b end
来源：http://mg.lnxyls.cn

[T37] Lua：字符串拼接
来源：http://wr.bookmarksfly.cn

"a" .. "b"
来源：http://nv.yuexingan06.cn

[T38] Lua：条件
来源：http://ml.huixinmuqiang.cn

if x > 0 then print("正") end
来源：http://ek.wgjwhj.cn

[T39] Lua：模式匹配
来源：http://pn.wgjwhj.cn

string.find(s, "%d+")
来源：http://kb.yuexingan06.cn

[T40] Lua：元表
来源：http://tr.bookmarksfly.cn

setmetatable({}, { __index = base })
来源：http://ii.shxzskj.cn

[T41] Perl：Hello World
来源：http://hk.nicolike.cn

print "Hello\n";
来源：http://bn.yuexingan06.cn

[T42] Perl：变量类型
来源：http://cw.521024.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://dc.shxzskj.cn

[T43] Perl：字符串插值
来源：http://mo.gzmigu.cn

"值: $a"
来源：http://rs.newstarts.cn

[T44] Perl：条件
来源：http://ty.gzmigu.cn

if ($a > 0) { print "正"; }
来源：http://cv.chemitech.net.cn

[T45] Perl：数组遍历
来源：http://uj.chemitech.net.cn

for my $x (@arr) { print $x; }
来源：http://pg.chemitech.net.cn

[T46] Perl：哈希操作
来源：http://uk.yuntaijiaju.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://wt.lnxyls.cn

[T47] Perl：正则捕获
来源：http://ya.nicolike.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ee.yuexingan06.cn

[T48] Perl：正则替换
来源：http://vu.nszjky.cn

$s =~ s/old/new/g;
来源：http://wr.szsharing.cn

[T49] Perl：函数
来源：http://zl.haigaiapp.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://fp.yuexingan06.cn

[T50] Perl：逐行读文件
来源：http://sc.bookmarksfly.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://yg.asd995.cn

while (my $line = <$fh>) { print $line; }
来源：http://iw.yuexingan06.cn

[T51] Scala：Hello World
来源：http://av.muxihuayi.cn

println("Hello")
来源：http://wc.muxihuayi.cn

[T52] Scala：变量
来源：http://hy.nicolike.cn

val a = 1;  var b = 2
来源：http://md.szxytkj.cn

[T53] Scala：字符串插值
来源：http://dp.jctech888.com.cn

s"值: $b"
来源：http://em.shxzskj.cn

[T54] Scala：集合映射
来源：http://rl.yuntaijiaju.cn


<!-- 参考信息 -->