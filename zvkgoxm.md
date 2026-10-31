代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：http://vs.muxihuayi.cn

[R48] awk 取指定列
来源：http://ww.panjiajie.cn

awk '{print $1, $3}' a.txt
来源：http://ks.asd995.cn

[R49] awk 带条件
来源：http://kb.newstarts.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://oo.muxihuayi.cn

[R50] awk 求和
来源：http://hb.bookmarksfly.cn

awk '{s += $2} END {print s}' a.txt
来源：http://yu.shxzukj.cn

[R51] 排序去重取前几
来源：http://sz.521024.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ei.szsharing.cn

[R52] 统计行数
来源：http://kf.jianghongdianzi.cn

wc -l a.txt
来源：http://me.jianghongdianzi.cn

[R53] 查看文件头与实时尾
来源：http://tq.9csxet.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://tc.szsharing.cn

[R54] 比较两个文件
来源：http://se.hnjuh.cn

diff a.txt b.txt
来源：http://vp.huixiangedu.cn

[R55] 压缩与解压
来源：http://to.bjjhwx.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://vy.huixiangedu.cn

[R56] 远程拷贝
来源：http://pp.haigaiapp.cn

scp file user@host:/path/
来源：http://qf.panjiajie.cn

[R57] 远程执行命令
来源：http://ww.muxihuayi.cn

ssh user@host 'uptime'
来源：http://uj.wgjwhj.cn

[R58] 下载文件
来源：http://gd.muxihuayi.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://gh.bookmarksfly.cn

[R59] 发 POST JSON
来源：http://vz.hahajie.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://rj.shtwfgs.cn

[R60] 只看 HTTP 状态码
来源：http://lj.521024.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://tl.chemitech.net.cn

[R61] 磁盘占用
来源：http://sq.jctech888.com.cn

df -h;  du -sh *
来源：http://nf.asd995.cn

[R62] 找最占空间的文件
来源：http://zv.newstarts.cn

du -ah . | sort -rh | head -10
来源：http://sz.hahajie.cn

[R63] 内存与进程
来源：http://yd.nicolike.cn

free -h;  ps aux | grep nginx
来源：http://wb.jctech888.com.cn

[R64] 结束进程
来源：http://pf.szxytkj.cn

kill -9 $(pgrep -f app.py)
来源：http://fe.haigaiapp.cn

[R65] 查看端口占用
来源：http://nc.haigaiapp.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ye.newstarts.cn

[R66] 定时任务
来源：http://ss.shxzskj.cn

crontab -e;  crontab -l
来源：http://kj.muxihuayi.cn

[R67] 生成随机十六进制串
来源：http://lb.nicolike.cn

openssl rand -hex 16
来源：http://eh.yuntaijiaju.cn

[R68] 计算文件校验值
来源：http://ni.jctech888.com.cn

sha256sum a.txt;  md5sum a.txt
来源：http://en.haigaiapp.cn

[R69] 生成随机密码
来源：http://qg.huixiangedu.cn

head -c 16 /dev/urandom | base64
来源：http://up.wgjwhj.cn

[R70] 时间戳与互转
来源：http://mq.asd995.cn

date +%s;  date -d @1700000000
来源：http://kz.haigaiapp.cn

[R71] 日期格式化
来源：http://ee.hahajie.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://yz.newstarts.cn

[R72] 等待端口就绪
来源：http://lp.nicolike.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://vp.jctech888.com.cn

[R73] 分割大日志
来源：http://uf.huanxung.cn

split -l 1000 big.log part_
来源：http://ns.szxytkj.cn

[R74] 批量重命名
来源：http://wq.panjiajie.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://eg.yuexingan06.cn

[R75] 导出环境变量
来源：http://yk.huixiangedu.cn

export PATH="$HOME/bin:$PATH"
来源：http://du.huanxung.cn

[R76] 使用临时文件
来源：http://cg.hnjuh.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ps.jctech888.com.cn

[R77] 读取用户输入
来源：http://xg.shtwfgs.cn

read -rp "请输入: " ans
来源：http://qv.nszjky.cn

[R78] 交互式菜单
来源：http://uy.szxytkj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ae.yuntaijiaju.cn

[R79] 解析命令行选项
来源：http://mb.9csxet.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://fq.huanxung.cn

[R80] 查看脚本执行耗时
来源：http://vo.asd995.cn

time ./run.sh
来源：http://rv.yuntaijiaju.cn

================================================================================
来源：http://yp.muxihuayi.cn

S. C / C++ 专题
来源：http://sg.gzmigu.cn

================================================================================
来源：http://nm.panjiajie.cn

[S01] C：Hello World
来源：http://bc.jctech888.com.cn

#include <stdio.h>
来源：http://cy.newstarts.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://xo.asd995.cn

[S02] C：变量与格式化输出
来源：http://sa.huixiangedu.cn

int a = 10; printf("%d\n", a);
来源：http://ti.521024.cn

[S03] C：读入整数
来源：http://fy.hahajie.cn

int x; scanf("%d", &x);
来源：http://wf.wgjwhj.cn

[S04] C：字符串复制
来源：http://wq.shxzskj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://om.lnxyls.cn

[S05] C：字符串长度
来源：http://bs.jctech888.com.cn

strlen(s)
来源：http://od.szsharing.cn

[S06] C：字符串比较
来源：http://ur.jianghongdianzi.cn

strcmp(a, b) == 0
来源：http://gy.gzmigu.cn

[S07] C：数组遍历求和
来源：http://xo.hnjuh.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://cz.yuexingan06.cn

[S08] C：动态内存分配与释放
来源：http://ox.szxytkj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://xd.szxytkj.cn

[S09] C：结构体定义与初始化
来源：http://sm.nicolike.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://re.yuntaijiaju.cn

[S10] C：指针与解引用
来源：http://bs.hahajie.cn

int *p = &a;  *p = 5;
来源：http://ys.colortex.cn

[S11] C：逐行读文件
来源：http://gn.bookmarksfly.cn

FILE *f = fopen("a.txt", "r");
来源：http://mh.gzmigu.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ak.panjiajie.cn

fclose(f);
来源：http://dj.huixiangedu.cn

[S12] C：写文件
来源：http://hv.chemitech.net.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ne.lnxyls.cn

[S13] C：宏定义
来源：http://wx.huanxung.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wd.huixinmuqiang.cn

[S14] C：枚举
来源：http://uz.gzmigu.cn

enum Color { RED, GREEN, BLUE };
来源：http://lr.huixinmuqiang.cn

[S15] C：类型转换
来源：http://wu.lnxyls.cn

(double) a / b
来源：http://eb.szxytkj.cn

[S16] C：位操作置位
来源：http://wm.wgjwhj.cn

x |= (1 << 3);
来源：http://rf.jianghongdianzi.cn

[S17] C：安全拼接字符串
来源：http://wn.asd995.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://kx.panjiajie.cn

[S18] C：命令行参数
来源：http://gh.nszjky.cn

int main(int argc, char **argv)
来源：http://em.haigaiapp.cn

[S19] C：快速排序
来源：http://vf.chemitech.net.cn

qsort(a, n, sizeof(int), cmp);
来源：http://fi.nicolike.cn

[S20] C：二分查找
来源：http://js.bookmarksfly.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://cd.nicolike.cn

[S21] C：字符类别判断
来源：http://vy.jianghongdianzi.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://af.huanxung.cn

[S22] C：字符串转数字
来源：http://af.lnxyls.cn

atoi("42");  strtod("3.14", NULL);
来源：http://rt.szxytkj.cn

[S23] C：随机数
来源：http://gv.szsharing.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://du.jctech888.com.cn

[S24] C：获取本地时间
来源：http://sz.asd995.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://qo.shxzukj.cn

[S25] C：内存拷贝
来源：http://er.huixinmuqiang.cn

memcpy(dst, src, n);
来源：http://xb.yuexingan06.cn

[S26] C：内存清零
来源：http://jt.nicolike.cn

memset(a, 0, sizeof a);
来源：http://uf.9csxet.cn

[S27] C：定义常量
来源：http://ht.jctech888.com.cn

const double PI = 3.14159;
来源：http://mm.haigaiapp.cn

[S28] C：静态变量
来源：http://he.shxzskj.cn

static int counter = 0;
来源：http://ox.shxzukj.cn

[S29] C：变参函数
来源：http://cu.bookmarksfly.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://bf.huixinmuqiang.cn

[S30] C：头文件保护
来源：http://ll.newstarts.cn

#ifndef X_H
来源：http://jr.szsharing.cn

#define X_H
来源：http://zz.chemitech.net.cn

#endif
来源：http://vw.huanxung.cn

[S31] C++：Hello World
来源：http://lk.yuexingan06.cn

#include <iostream>
来源：http://ly.9csxet.cn

int main() { std::cout << "Hello\n"; }
来源：http://iq.shxzskj.cn

[S32] C++：字符串
来源：http://qf.asd995.cn

std::string s = "hi";  s += "!";
来源：http://cy.huixiangedu.cn

[S33] C++：vector 增删
来源：http://up.colortex.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://xk.hahajie.cn

[S34] C++：遍历 vector
来源：http://yd.newstarts.cn

for (auto &x : v) { std::cout << x; }
来源：http://rc.asd995.cn

[S35] C++：map
来源：http://ae.asd995.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://dn.hnjuh.cn

[S36] C++：unordered_map
来源：http://gf.nicolike.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://vk.huanxung.cn

[S37] C++：set
来源：http://oi.nszjky.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://zr.panjiajie.cn

[S38] C++：排序
来源：http://yo.shxzskj.cn

std::sort(v.begin(), v.end());
来源：http://mq.jianghongdianzi.cn

[S39] C++：自定义比较器排序
来源：http://og.jianghongdianzi.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://yj.huanxung.cn

[S40] C++：查找元素
来源：http://cn.lnxyls.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://tb.nszjky.cn

[S41] C++：类与构造函数
来源：http://xk.jianghongdianzi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://lp.yuntaijiaju.cn

[S42] C++：继承与虚函数
来源：http://zy.shtwfgs.cn

class B : public Base { public: void f() override {} };
来源：http://ou.wgjwhj.cn

[S43] C++：智能指针
来源：http://zt.9csxet.cn

auto p = std::make_unique<int>(5);
来源：http://kn.huanxung.cn

[S44] C++：引用传参
来源：http://mr.huanxung.cn

void inc(int &x) { ++x; }
来源：http://mu.shtwfgs.cn

[S45] C++：lambda
来源：http://sm.huixiangedu.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ro.szxytkj.cn

[S46] C++：函数模板
来源：http://ye.yuntaijiaju.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://jd.jianghongdianzi.cn

[S47] C++：结构化绑定遍历
来源：http://qf.huixiangedu.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://nq.shtwfgs.cn

[S48] C++：逐行读文件
来源：http://fs.gzmigu.cn

std::ifstream in("a.txt");  std::string line;
来源：http://lk.gzmigu.cn

while (std::getline(in, line)) { }
来源：http://fg.chemitech.net.cn

[S49] C++：写文件
来源：http://vb.huanxung.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://cw.521024.cn

[S50] C++：格式化数字
来源：http://xf.muxihuayi.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://es.lnxyls.cn

[S51] C++：显式类型转换
来源：http://kn.yuexingan06.cn

static_cast<double>(a) / b
来源：http://jg.szsharing.cn

[S52] C++：const 与 noexcept
来源：http://yw.shtwfgs.cn

int size() const noexcept { return n_; }
来源：http://zf.yuntaijiaju.cn

[S53] C++：移动语义
来源：http://ti.521024.cn

std::vector<int> w = std::move(v);
来源：http://kl.bookmarksfly.cn

[S54] C++：异常处理
来源：http://ed.szxytkj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://kt.muxihuayi.cn

[S55] C++：结构化绑定
来源：http://gb.huanxung.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://fy.gzmigu.cn

[S56] C++：optional
来源：http://ih.521024.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://yu.yuexingan06.cn

[S57] C++：编译期常量
来源：http://lo.hahajie.cn

constexpr int N = 10;
来源：http://ln.bookmarksfly.cn

[S58] C++：命名空间
来源：http://mz.shxzskj.cn

namespace ns { int f() { return 1; } }
来源：http://yb.huanxung.cn

[S59] C++：静态断言
来源：http://pn.wgjwhj.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://cn.jianghongdianzi.cn

[S60] C++：遍历并删除元素
来源：http://oz.huixiangedu.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://gv.jctech888.com.cn

================================================================================
来源：http://gr.bjjhwx.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://lz.hahajie.cn

================================================================================
来源：http://zs.muxihuayi.cn

[T01] Kotlin：Hello World
来源：http://at.hnjuh.cn

println("Hello")
来源：http://wy.panjiajie.cn

[T02] Kotlin：变量
来源：http://he.nszjky.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://tg.huixinmuqiang.cn

[T03] Kotlin：字符串模板
来源：http://wr.muxihuayi.cn

"值: $b"
来源：http://au.huixiangedu.cn

[T04] Kotlin：空安全
来源：http://dg.shxzskj.cn

val n: String? = null;  n?.length
来源：http://ku.bjjhwx.cn

[T05] Kotlin：when 表达式
来源：http://sd.nszjky.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://xx.huixiangedu.cn

[T06] Kotlin：集合映射
来源：http://ca.lnxyls.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://as.shxzukj.cn

[T07] Kotlin：集合过滤
来源：http://yx.colortex.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://lh.9csxet.cn

[T08] Kotlin：数据类
来源：http://fi.yuexingan06.cn

data class User(val name: String, val age: Int)
来源：http://te.panjiajie.cn

[T09] Kotlin：扩展函数
来源：http://nc.yuntaijiaju.cn

fun String.exclaim() = this + "!"
来源：http://oe.panjiajie.cn

[T10] Kotlin：默认参数
来源：http://my.asd995.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://dc.gzmigu.cn

[T11] Kotlin：协程
来源：http://qv.panjiajie.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://pd.huixiangedu.cn

[T12] Kotlin：解构声明
来源：http://cf.bookmarksfly.cn

val (a, b) = Pair(1, 2)
来源：http://im.huanxung.cn

[T13] Kotlin：只读 Map
来源：http://pt.huixinmuqiang.cn

val m = mapOf("a" to 1)
来源：http://ox.hahajie.cn

[T14] Kotlin：循环
来源：http://ov.asd995.cn

for (i in 1..10) println(i)
来源：http://ov.gzmigu.cn

[T15] Kotlin：接口
来源：http://yx.yuexingan06.cn

interface Shape { fun area(): Double }
来源：http://lz.yuntaijiaju.cn

[T16] Swift：Hello World
来源：http://ax.szxytkj.cn

print("Hello")
来源：http://ec.newstarts.cn

[T17] Swift：变量与常量
来源：http://me.newstarts.cn

var a = 1;  let b = 2
来源：http://oo.szxytkj.cn

[T18] Swift：字符串插值
来源：http://ql.hnjuh.cn

"值: \(b)"
来源：http://oy.9csxet.cn

[T19] Swift：可选绑定
来源：http://dy.jctech888.com.cn

if let n = opt { print(n) }
来源：http://jb.yuexingan06.cn

[T20] Swift：数组操作
来源：http://ob.lnxyls.cn

var a = [1, 2, 3];  a.append(4)
来源：http://zv.newstarts.cn

[T21] Swift：遍历
来源：http://hl.521024.cn

for x in a { print(x) }
来源：http://un.hahajie.cn

[T22] Swift：字典
来源：http://fe.yuexingan06.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ye.9csxet.cn

[T23] Swift：函数
来源：http://ms.gzmigu.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://rz.lnxyls.cn

[T24] Swift：闭包
来源：http://zm.nicolike.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://hj.huanxung.cn

[T25] Swift：结构体
来源：http://ms.jctech888.com.cn

struct P { var x: Int }
来源：http://fj.9csxet.cn

[T26] Swift：类与重写
来源：http://wn.gzmigu.cn

class A: Base { override func f() {} }
来源：http://wn.9csxet.cn

[T27] Swift：错误处理
来源：http://bs.bookmarksfly.cn

do { try f() } catch { print(error) }
来源：http://cx.haigaiapp.cn

[T28] Swift：枚举
来源：http://qt.521024.cn

enum Color { case red, green }
来源：http://eb.521024.cn

[T29] Swift：guard 提前返回
来源：http://eh.wgjwhj.cn

guard let x = opt else { return }
来源：http://rd.shtwfgs.cn

[T30] Swift：协议
来源：http://rx.gzmigu.cn

protocol Shape { func area() -> Double }
来源：http://kl.szsharing.cn

[T31] Lua：Hello World
来源：http://um.chemitech.net.cn

print("Hello")
来源：http://yp.szxytkj.cn

[T32] Lua：局部变量
来源：http://pn.newstarts.cn

local a = 1
来源：http://vn.bjjhwx.cn

[T33] Lua：表（数组）
来源：http://fg.lnxyls.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://mi.shxzskj.cn

[T34] Lua：遍历表
来源：http://nu.hnjuh.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://qx.9csxet.cn

[T35] Lua：字典表
来源：http://zy.szsharing.cn

local d = { a = 1 };  d.b = 2
来源：http://qr.nicolike.cn

[T36] Lua：函数
来源：http://ki.haigaiapp.cn

function add(a, b) return a + b end
来源：http://vg.521024.cn

[T37] Lua：字符串拼接
来源：http://ll.jianghongdianzi.cn

"a" .. "b"
来源：http://ey.yuntaijiaju.cn

[T38] Lua：条件
来源：http://vr.huanxung.cn

if x > 0 then print("正") end
来源：http://tf.huixiangedu.cn

[T39] Lua：模式匹配
来源：http://nv.bjjhwx.cn

string.find(s, "%d+")
来源：http://nl.9csxet.cn

[T40] Lua：元表
来源：http://xt.lnxyls.cn

setmetatable({}, { __index = base })
来源：http://zx.muxihuayi.cn

[T41] Perl：Hello World
来源：http://wp.hahajie.cn

print "Hello\n";
来源：http://kx.yuntaijiaju.cn

[T42] Perl：变量类型
来源：http://hv.colortex.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ay.huixinmuqiang.cn

[T43] Perl：字符串插值
来源：http://jm.shxzukj.cn

"值: $a"
来源：http://ro.colortex.cn

[T44] Perl：条件
来源：http://an.shxzskj.cn

if ($a > 0) { print "正"; }
来源：http://qb.shxzukj.cn

[T45] Perl：数组遍历
来源：http://hj.521024.cn

for my $x (@arr) { print $x; }
来源：http://cr.bookmarksfly.cn

[T46] Perl：哈希操作
来源：http://ll.shtwfgs.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://fy.yuntaijiaju.cn

[T47] Perl：正则捕获
来源：http://cu.huanxung.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://dq.shxzskj.cn

[T48] Perl：正则替换
来源：http://ej.huixinmuqiang.cn

$s =~ s/old/new/g;
来源：http://yv.wgjwhj.cn

[T49] Perl：函数
来源：http://gr.bookmarksfly.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hu.chemitech.net.cn

[T50] Perl：逐行读文件
来源：http://fn.yuexingan06.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://xt.muxihuayi.cn


<!-- 参考信息 -->