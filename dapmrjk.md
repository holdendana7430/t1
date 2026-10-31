代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://jh.szxytkj.cn

[R50] awk 求和
来源：http://va.szsharing.cn

awk '{s += $2} END {print s}' a.txt
来源：http://zd.jctech888.com.cn

[R51] 排序去重取前几
来源：http://nc.chemitech.net.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://mt.shtwfgs.cn

[R52] 统计行数
来源：http://rx.9csxet.cn

wc -l a.txt
来源：http://vg.szxytkj.cn

[R53] 查看文件头与实时尾
来源：http://yj.yuntaijiaju.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://kp.huixiangedu.cn

[R54] 比较两个文件
来源：http://sx.huanxung.cn

diff a.txt b.txt
来源：http://gl.bjjhwx.cn

[R55] 压缩与解压
来源：http://zk.lnxyls.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://es.hahajie.cn

[R56] 远程拷贝
来源：http://mu.jctech888.com.cn

scp file user@host:/path/
来源：http://vd.haigaiapp.cn

[R57] 远程执行命令
来源：http://bj.yuexingan06.cn

ssh user@host 'uptime'
来源：http://sw.yuexingan06.cn

[R58] 下载文件
来源：http://eq.huanxung.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://xt.shtwfgs.cn

[R59] 发 POST JSON
来源：http://fa.huixiangedu.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://cz.shxzskj.cn

[R60] 只看 HTTP 状态码
来源：http://ux.hahajie.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://rh.yuntaijiaju.cn

[R61] 磁盘占用
来源：http://pm.colortex.cn

df -h;  du -sh *
来源：http://zz.hahajie.cn

[R62] 找最占空间的文件
来源：http://bh.jianghongdianzi.cn

du -ah . | sort -rh | head -10
来源：http://vu.shtwfgs.cn

[R63] 内存与进程
来源：http://wp.521024.cn

free -h;  ps aux | grep nginx
来源：http://tb.wgjwhj.cn

[R64] 结束进程
来源：http://rh.jctech888.com.cn

kill -9 $(pgrep -f app.py)
来源：http://yf.hahajie.cn

[R65] 查看端口占用
来源：http://pl.colortex.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hb.newstarts.cn

[R66] 定时任务
来源：http://sn.jianghongdianzi.cn

crontab -e;  crontab -l
来源：http://cb.nicolike.cn

[R67] 生成随机十六进制串
来源：http://tj.asd995.cn

openssl rand -hex 16
来源：http://py.jctech888.com.cn

[R68] 计算文件校验值
来源：http://cs.szxytkj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://pq.newstarts.cn

[R69] 生成随机密码
来源：http://mz.shtwfgs.cn

head -c 16 /dev/urandom | base64
来源：http://aa.gzmigu.cn

[R70] 时间戳与互转
来源：http://ut.newstarts.cn

date +%s;  date -d @1700000000
来源：http://lt.hnjuh.cn

[R71] 日期格式化
来源：http://fg.huixiangedu.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://in.shxzskj.cn

[R72] 等待端口就绪
来源：http://mb.colortex.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://bd.521024.cn

[R73] 分割大日志
来源：http://kh.colortex.cn

split -l 1000 big.log part_
来源：http://ib.9csxet.cn

[R74] 批量重命名
来源：http://gh.hahajie.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://rx.huixinmuqiang.cn

[R75] 导出环境变量
来源：http://xv.asd995.cn

export PATH="$HOME/bin:$PATH"
来源：http://vv.jianghongdianzi.cn

[R76] 使用临时文件
来源：http://av.shxzskj.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://bd.newstarts.cn

[R77] 读取用户输入
来源：http://ps.szxytkj.cn

read -rp "请输入: " ans
来源：http://kv.hahajie.cn

[R78] 交互式菜单
来源：http://zc.nicolike.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://es.asd995.cn

[R79] 解析命令行选项
来源：http://zn.jctech888.com.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://oj.bookmarksfly.cn

[R80] 查看脚本执行耗时
来源：http://nn.szxytkj.cn

time ./run.sh
来源：http://ec.huanxung.cn

================================================================================
来源：http://dy.shtwfgs.cn

S. C / C++ 专题
来源：http://tl.nszjky.cn

================================================================================
来源：http://il.huanxung.cn

[S01] C：Hello World
来源：http://ru.9csxet.cn

#include <stdio.h>
来源：http://tz.colortex.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://ng.shtwfgs.cn

[S02] C：变量与格式化输出
来源：http://id.panjiajie.cn

int a = 10; printf("%d\n", a);
来源：http://nd.szsharing.cn

[S03] C：读入整数
来源：http://ev.shxzukj.cn

int x; scanf("%d", &x);
来源：http://yl.haigaiapp.cn

[S04] C：字符串复制
来源：http://dw.shxzskj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ef.yuntaijiaju.cn

[S05] C：字符串长度
来源：http://an.shxzskj.cn

strlen(s)
来源：http://zp.shxzskj.cn

[S06] C：字符串比较
来源：http://vr.lnxyls.cn

strcmp(a, b) == 0
来源：http://lj.panjiajie.cn

[S07] C：数组遍历求和
来源：http://hz.9csxet.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://fp.hnjuh.cn

[S08] C：动态内存分配与释放
来源：http://vb.9csxet.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://zt.shtwfgs.cn

[S09] C：结构体定义与初始化
来源：http://vo.huixiangedu.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ra.shxzukj.cn

[S10] C：指针与解引用
来源：http://cf.hahajie.cn

int *p = &a;  *p = 5;
来源：http://uh.jctech888.com.cn

[S11] C：逐行读文件
来源：http://pj.9csxet.cn

FILE *f = fopen("a.txt", "r");
来源：http://vt.haigaiapp.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://td.bookmarksfly.cn

fclose(f);
来源：http://ld.jianghongdianzi.cn

[S12] C：写文件
来源：http://lz.hahajie.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://iy.huixinmuqiang.cn

[S13] C：宏定义
来源：http://lx.jctech888.com.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://cd.newstarts.cn

[S14] C：枚举
来源：http://fs.muxihuayi.cn

enum Color { RED, GREEN, BLUE };
来源：http://zz.bookmarksfly.cn

[S15] C：类型转换
来源：http://hp.shxzukj.cn

(double) a / b
来源：http://po.yuexingan06.cn

[S16] C：位操作置位
来源：http://or.bookmarksfly.cn

x |= (1 << 3);
来源：http://jz.huixiangedu.cn

[S17] C：安全拼接字符串
来源：http://de.9csxet.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ha.haigaiapp.cn

[S18] C：命令行参数
来源：http://ps.yuntaijiaju.cn

int main(int argc, char **argv)
来源：http://op.panjiajie.cn

[S19] C：快速排序
来源：http://qq.hnjuh.cn

qsort(a, n, sizeof(int), cmp);
来源：http://rh.chemitech.net.cn

[S20] C：二分查找
来源：http://jk.yuexingan06.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mz.szsharing.cn

[S21] C：字符类别判断
来源：http://ra.hahajie.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://yx.shxzukj.cn

[S22] C：字符串转数字
来源：http://hq.muxihuayi.cn

atoi("42");  strtod("3.14", NULL);
来源：http://fg.chemitech.net.cn

[S23] C：随机数
来源：http://sz.bjjhwx.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://nx.lnxyls.cn

[S24] C：获取本地时间
来源：http://se.nicolike.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://fl.9csxet.cn

[S25] C：内存拷贝
来源：http://ob.shxzskj.cn

memcpy(dst, src, n);
来源：http://uu.huanxung.cn

[S26] C：内存清零
来源：http://jm.shxzskj.cn

memset(a, 0, sizeof a);
来源：http://lr.panjiajie.cn

[S27] C：定义常量
来源：http://zj.szxytkj.cn

const double PI = 3.14159;
来源：http://ja.nszjky.cn

[S28] C：静态变量
来源：http://fe.szxytkj.cn

static int counter = 0;
来源：http://rc.newstarts.cn

[S29] C：变参函数
来源：http://ou.huixiangedu.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mo.nszjky.cn

[S30] C：头文件保护
来源：http://gd.9csxet.cn

#ifndef X_H
来源：http://bk.szxytkj.cn

#define X_H
来源：http://gh.nicolike.cn

#endif
来源：http://wl.szsharing.cn

[S31] C++：Hello World
来源：http://oo.newstarts.cn

#include <iostream>
来源：http://yt.lnxyls.cn

int main() { std::cout << "Hello\n"; }
来源：http://ic.hnjuh.cn

[S32] C++：字符串
来源：http://ws.yuntaijiaju.cn

std::string s = "hi";  s += "!";
来源：http://sn.521024.cn

[S33] C++：vector 增删
来源：http://qw.szxytkj.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://sj.asd995.cn

[S34] C++：遍历 vector
来源：http://co.chemitech.net.cn

for (auto &x : v) { std::cout << x; }
来源：http://gf.521024.cn

[S35] C++：map
来源：http://id.wgjwhj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://em.wgjwhj.cn

[S36] C++：unordered_map
来源：http://hs.521024.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://zf.chemitech.net.cn

[S37] C++：set
来源：http://bx.bjjhwx.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://on.nszjky.cn

[S38] C++：排序
来源：http://ih.jctech888.com.cn

std::sort(v.begin(), v.end());
来源：http://gz.bjjhwx.cn

[S39] C++：自定义比较器排序
来源：http://wo.bjjhwx.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ad.hahajie.cn

[S40] C++：查找元素
来源：http://ve.newstarts.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://fb.9csxet.cn

[S41] C++：类与构造函数
来源：http://ut.gzmigu.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://wy.szsharing.cn

[S42] C++：继承与虚函数
来源：http://tg.nicolike.cn

class B : public Base { public: void f() override {} };
来源：http://rk.panjiajie.cn

[S43] C++：智能指针
来源：http://sx.gzmigu.cn

auto p = std::make_unique<int>(5);
来源：http://ov.bjjhwx.cn

[S44] C++：引用传参
来源：http://xf.asd995.cn

void inc(int &x) { ++x; }
来源：http://ot.yuntaijiaju.cn

[S45] C++：lambda
来源：http://db.521024.cn

auto add = [](int a, int b) { return a + b; };
来源：http://zf.521024.cn

[S46] C++：函数模板
来源：http://hz.shtwfgs.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://cl.9csxet.cn

[S47] C++：结构化绑定遍历
来源：http://cn.nicolike.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ps.yuexingan06.cn

[S48] C++：逐行读文件
来源：http://cs.huixiangedu.cn

std::ifstream in("a.txt");  std::string line;
来源：http://fv.shxzukj.cn

while (std::getline(in, line)) { }
来源：http://qi.nicolike.cn

[S49] C++：写文件
来源：http://rt.haigaiapp.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://lq.gzmigu.cn

[S50] C++：格式化数字
来源：http://nw.nszjky.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://qx.bookmarksfly.cn

[S51] C++：显式类型转换
来源：http://fr.gzmigu.cn

static_cast<double>(a) / b
来源：http://ax.lnxyls.cn

[S52] C++：const 与 noexcept
来源：http://cr.szxytkj.cn

int size() const noexcept { return n_; }
来源：http://dc.asd995.cn

[S53] C++：移动语义
来源：http://hl.wgjwhj.cn

std::vector<int> w = std::move(v);
来源：http://gs.jianghongdianzi.cn

[S54] C++：异常处理
来源：http://zs.lnxyls.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mn.haigaiapp.cn

[S55] C++：结构化绑定
来源：http://cm.yuntaijiaju.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ns.chemitech.net.cn

[S56] C++：optional
来源：http://hb.shxzukj.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://bp.shxzukj.cn

[S57] C++：编译期常量
来源：http://wi.shxzskj.cn

constexpr int N = 10;
来源：http://uw.lnxyls.cn

[S58] C++：命名空间
来源：http://io.shtwfgs.cn

namespace ns { int f() { return 1; } }
来源：http://vk.muxihuayi.cn

[S59] C++：静态断言
来源：http://gz.huanxung.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://pw.yuntaijiaju.cn

[S60] C++：遍历并删除元素
来源：http://gs.jctech888.com.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://kj.bookmarksfly.cn

================================================================================
来源：http://bz.huanxung.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://rr.lnxyls.cn

================================================================================
来源：http://yz.lnxyls.cn

[T01] Kotlin：Hello World
来源：http://pd.szxytkj.cn

println("Hello")
来源：http://sh.newstarts.cn

[T02] Kotlin：变量
来源：http://py.jctech888.com.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wt.521024.cn

[T03] Kotlin：字符串模板
来源：http://ku.szxytkj.cn

"值: $b"
来源：http://vu.panjiajie.cn

[T04] Kotlin：空安全
来源：http://xz.lnxyls.cn

val n: String? = null;  n?.length
来源：http://ov.huanxung.cn

[T05] Kotlin：when 表达式
来源：http://xt.hahajie.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://sl.yuntaijiaju.cn

[T06] Kotlin：集合映射
来源：http://cl.haigaiapp.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://mj.shxzukj.cn

[T07] Kotlin：集合过滤
来源：http://vg.newstarts.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://jk.wgjwhj.cn

[T08] Kotlin：数据类
来源：http://hz.yuexingan06.cn

data class User(val name: String, val age: Int)
来源：http://pm.huixinmuqiang.cn

[T09] Kotlin：扩展函数
来源：http://hg.wgjwhj.cn

fun String.exclaim() = this + "!"
来源：http://wx.yuntaijiaju.cn

[T10] Kotlin：默认参数
来源：http://np.asd995.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ml.lnxyls.cn

[T11] Kotlin：协程
来源：http://kb.521024.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://dc.szsharing.cn

[T12] Kotlin：解构声明
来源：http://my.bjjhwx.cn

val (a, b) = Pair(1, 2)
来源：http://oq.yuntaijiaju.cn

[T13] Kotlin：只读 Map
来源：http://jr.haigaiapp.cn

val m = mapOf("a" to 1)
来源：http://co.lnxyls.cn

[T14] Kotlin：循环
来源：http://an.szsharing.cn

for (i in 1..10) println(i)
来源：http://gm.huixiangedu.cn

[T15] Kotlin：接口
来源：http://st.gzmigu.cn

interface Shape { fun area(): Double }
来源：http://tj.huixinmuqiang.cn

[T16] Swift：Hello World
来源：http://ia.huixiangedu.cn

print("Hello")
来源：http://bs.chemitech.net.cn

[T17] Swift：变量与常量
来源：http://zk.bjjhwx.cn

var a = 1;  let b = 2
来源：http://et.colortex.cn

[T18] Swift：字符串插值
来源：http://ah.haigaiapp.cn

"值: \(b)"
来源：http://zy.shxzukj.cn

[T19] Swift：可选绑定
来源：http://ho.shtwfgs.cn

if let n = opt { print(n) }
来源：http://ok.bookmarksfly.cn

[T20] Swift：数组操作
来源：http://sg.newstarts.cn

var a = [1, 2, 3];  a.append(4)
来源：http://mi.wgjwhj.cn

[T21] Swift：遍历
来源：http://ag.shxzskj.cn

for x in a { print(x) }
来源：http://xu.szxytkj.cn

[T22] Swift：字典
来源：http://in.9csxet.cn

var d = ["a": 1];  d["b"] = 2
来源：http://rp.shtwfgs.cn

[T23] Swift：函数
来源：http://dh.asd995.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mq.asd995.cn

[T24] Swift：闭包
来源：http://vg.haigaiapp.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://mm.9csxet.cn

[T25] Swift：结构体
来源：http://uu.asd995.cn

struct P { var x: Int }
来源：http://rm.jctech888.com.cn

[T26] Swift：类与重写
来源：http://fz.yuexingan06.cn

class A: Base { override func f() {} }
来源：http://uc.nicolike.cn

[T27] Swift：错误处理
来源：http://vk.huanxung.cn

do { try f() } catch { print(error) }
来源：http://hv.huixiangedu.cn

[T28] Swift：枚举
来源：http://ap.asd995.cn

enum Color { case red, green }
来源：http://cb.huixiangedu.cn

[T29] Swift：guard 提前返回
来源：http://ji.nicolike.cn

guard let x = opt else { return }
来源：http://mu.szxytkj.cn

[T30] Swift：协议
来源：http://ki.nszjky.cn

protocol Shape { func area() -> Double }
来源：http://kd.bookmarksfly.cn

[T31] Lua：Hello World
来源：http://ug.bjjhwx.cn

print("Hello")
来源：http://kn.huixinmuqiang.cn

[T32] Lua：局部变量
来源：http://df.szsharing.cn

local a = 1
来源：http://sb.521024.cn

[T33] Lua：表（数组）
来源：http://pk.nicolike.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://fy.wgjwhj.cn

[T34] Lua：遍历表
来源：http://jo.muxihuayi.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://wu.521024.cn

[T35] Lua：字典表
来源：http://ok.9csxet.cn

local d = { a = 1 };  d.b = 2
来源：http://es.shxzskj.cn

[T36] Lua：函数
来源：http://gs.huixinmuqiang.cn

function add(a, b) return a + b end
来源：http://ij.wgjwhj.cn

[T37] Lua：字符串拼接
来源：http://bp.wgjwhj.cn

"a" .. "b"
来源：http://fg.colortex.cn

[T38] Lua：条件
来源：http://jl.gzmigu.cn

if x > 0 then print("正") end
来源：http://ba.9csxet.cn

[T39] Lua：模式匹配
来源：http://nb.nicolike.cn

string.find(s, "%d+")
来源：http://vb.9csxet.cn

[T40] Lua：元表
来源：http://vy.asd995.cn

setmetatable({}, { __index = base })
来源：http://bm.jianghongdianzi.cn

[T41] Perl：Hello World
来源：http://zy.9csxet.cn

print "Hello\n";
来源：http://jj.lnxyls.cn

[T42] Perl：变量类型
来源：http://kx.asd995.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://nw.hahajie.cn

[T43] Perl：字符串插值
来源：http://hi.521024.cn

"值: $a"
来源：http://uz.hnjuh.cn

[T44] Perl：条件
来源：http://kc.haigaiapp.cn

if ($a > 0) { print "正"; }
来源：http://ty.newstarts.cn

[T45] Perl：数组遍历
来源：http://fe.newstarts.cn

for my $x (@arr) { print $x; }
来源：http://pg.szsharing.cn

[T46] Perl：哈希操作
来源：http://ph.newstarts.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ek.521024.cn

[T47] Perl：正则捕获
来源：http://wu.panjiajie.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://jy.nszjky.cn

[T48] Perl：正则替换
来源：http://oq.yuexingan06.cn

$s =~ s/old/new/g;
来源：http://lk.hnjuh.cn

[T49] Perl：函数
来源：http://rt.szsharing.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://va.panjiajie.cn

[T50] Perl：逐行读文件
来源：http://ly.wgjwhj.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://kx.nszjky.cn

while (my $line = <$fh>) { print $line; }
来源：http://ld.chemitech.net.cn

[T51] Scala：Hello World
来源：http://lp.hnjuh.cn

println("Hello")
来源：http://it.asd995.cn

[T52] Scala：变量
来源：http://so.wgjwhj.cn


<!-- 参考信息 -->