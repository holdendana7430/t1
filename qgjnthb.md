代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://zg.bjjhwx.cn

[R50] awk 求和
来源：http://gd.yuntaijiaju.cn

awk '{s += $2} END {print s}' a.txt
来源：http://jf.huanxung.cn

[R51] 排序去重取前几
来源：http://vt.bookmarksfly.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://tp.nicolike.cn

[R52] 统计行数
来源：http://wp.bookmarksfly.cn

wc -l a.txt
来源：http://qh.wgjwhj.cn

[R53] 查看文件头与实时尾
来源：http://wi.9csxet.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://pz.yuexingan06.cn

[R54] 比较两个文件
来源：http://ms.szsharing.cn

diff a.txt b.txt
来源：http://ni.yuexingan06.cn

[R55] 压缩与解压
来源：http://gr.wgjwhj.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://lk.huixiangedu.cn

[R56] 远程拷贝
来源：http://yt.jianghongdianzi.cn

scp file user@host:/path/
来源：http://ky.huixinmuqiang.cn

[R57] 远程执行命令
来源：http://qw.shtwfgs.cn

ssh user@host 'uptime'
来源：http://hb.shtwfgs.cn

[R58] 下载文件
来源：http://tz.yuntaijiaju.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://vz.panjiajie.cn

[R59] 发 POST JSON
来源：http://xv.yuexingan06.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wl.shxzukj.cn

[R60] 只看 HTTP 状态码
来源：http://vq.521024.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://gc.szsharing.cn

[R61] 磁盘占用
来源：http://zx.bjjhwx.cn

df -h;  du -sh *
来源：http://ep.nicolike.cn

[R62] 找最占空间的文件
来源：http://ge.yuntaijiaju.cn

du -ah . | sort -rh | head -10
来源：http://xx.shxzskj.cn

[R63] 内存与进程
来源：http://ja.nszjky.cn

free -h;  ps aux | grep nginx
来源：http://ei.bookmarksfly.cn

[R64] 结束进程
来源：http://ug.521024.cn

kill -9 $(pgrep -f app.py)
来源：http://fe.muxihuayi.cn

[R65] 查看端口占用
来源：http://nk.huanxung.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://gu.szsharing.cn

[R66] 定时任务
来源：http://zf.shtwfgs.cn

crontab -e;  crontab -l
来源：http://tc.nicolike.cn

[R67] 生成随机十六进制串
来源：http://hy.hahajie.cn

openssl rand -hex 16
来源：http://zu.bjjhwx.cn

[R68] 计算文件校验值
来源：http://ui.newstarts.cn

sha256sum a.txt;  md5sum a.txt
来源：http://mb.gzmigu.cn

[R69] 生成随机密码
来源：http://ec.szxytkj.cn

head -c 16 /dev/urandom | base64
来源：http://vm.9csxet.cn

[R70] 时间戳与互转
来源：http://xj.huixinmuqiang.cn

date +%s;  date -d @1700000000
来源：http://pb.nicolike.cn

[R71] 日期格式化
来源：http://he.521024.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://dk.gzmigu.cn

[R72] 等待端口就绪
来源：http://jr.asd995.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://iw.newstarts.cn

[R73] 分割大日志
来源：http://ah.huanxung.cn

split -l 1000 big.log part_
来源：http://oo.jctech888.com.cn

[R74] 批量重命名
来源：http://kt.bookmarksfly.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://oy.gzmigu.cn

[R75] 导出环境变量
来源：http://rk.huanxung.cn

export PATH="$HOME/bin:$PATH"
来源：http://lm.yuntaijiaju.cn

[R76] 使用临时文件
来源：http://xw.gzmigu.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://tt.9csxet.cn

[R77] 读取用户输入
来源：http://vo.muxihuayi.cn

read -rp "请输入: " ans
来源：http://dz.szxytkj.cn

[R78] 交互式菜单
来源：http://pq.bjjhwx.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://fe.nszjky.cn

[R79] 解析命令行选项
来源：http://xb.muxihuayi.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://db.hahajie.cn

[R80] 查看脚本执行耗时
来源：http://yl.shxzskj.cn

time ./run.sh
来源：http://na.521024.cn

================================================================================
来源：http://on.panjiajie.cn

S. C / C++ 专题
来源：http://ko.wgjwhj.cn

================================================================================
来源：http://gj.jctech888.com.cn

[S01] C：Hello World
来源：http://wi.jianghongdianzi.cn

#include <stdio.h>
来源：http://yx.bookmarksfly.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://pi.lnxyls.cn

[S02] C：变量与格式化输出
来源：http://zl.shtwfgs.cn

int a = 10; printf("%d\n", a);
来源：http://so.muxihuayi.cn

[S03] C：读入整数
来源：http://vg.lnxyls.cn

int x; scanf("%d", &x);
来源：http://in.nszjky.cn

[S04] C：字符串复制
来源：http://ie.colortex.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ss.wgjwhj.cn

[S05] C：字符串长度
来源：http://se.nszjky.cn

strlen(s)
来源：http://du.huanxung.cn

[S06] C：字符串比较
来源：http://eo.haigaiapp.cn

strcmp(a, b) == 0
来源：http://or.huixinmuqiang.cn

[S07] C：数组遍历求和
来源：http://am.hahajie.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ia.wgjwhj.cn

[S08] C：动态内存分配与释放
来源：http://mv.muxihuayi.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://tn.lnxyls.cn

[S09] C：结构体定义与初始化
来源：http://ed.shtwfgs.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://kt.muxihuayi.cn

[S10] C：指针与解引用
来源：http://cu.haigaiapp.cn

int *p = &a;  *p = 5;
来源：http://gx.huanxung.cn

[S11] C：逐行读文件
来源：http://sk.colortex.cn

FILE *f = fopen("a.txt", "r");
来源：http://qv.wgjwhj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://es.szsharing.cn

fclose(f);
来源：http://gl.jctech888.com.cn

[S12] C：写文件
来源：http://ib.huixinmuqiang.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://yq.panjiajie.cn

[S13] C：宏定义
来源：http://uj.nicolike.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://si.szsharing.cn

[S14] C：枚举
来源：http://cm.gzmigu.cn

enum Color { RED, GREEN, BLUE };
来源：http://la.colortex.cn

[S15] C：类型转换
来源：http://ov.shxzskj.cn

(double) a / b
来源：http://cx.gzmigu.cn

[S16] C：位操作置位
来源：http://ft.bjjhwx.cn

x |= (1 << 3);
来源：http://jw.hahajie.cn

[S17] C：安全拼接字符串
来源：http://zv.shxzukj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ot.asd995.cn

[S18] C：命令行参数
来源：http://rr.szsharing.cn

int main(int argc, char **argv)
来源：http://gy.asd995.cn

[S19] C：快速排序
来源：http://xl.asd995.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ew.newstarts.cn

[S20] C：二分查找
来源：http://fa.huixinmuqiang.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://kv.haigaiapp.cn

[S21] C：字符类别判断
来源：http://jj.muxihuayi.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://td.bjjhwx.cn

[S22] C：字符串转数字
来源：http://bn.shxzukj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://re.szsharing.cn

[S23] C：随机数
来源：http://ag.shtwfgs.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://wm.shxzskj.cn

[S24] C：获取本地时间
来源：http://vn.9csxet.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ml.panjiajie.cn

[S25] C：内存拷贝
来源：http://sp.shxzukj.cn

memcpy(dst, src, n);
来源：http://ez.shxzskj.cn

[S26] C：内存清零
来源：http://uy.panjiajie.cn

memset(a, 0, sizeof a);
来源：http://jt.jctech888.com.cn

[S27] C：定义常量
来源：http://tr.chemitech.net.cn

const double PI = 3.14159;
来源：http://ys.gzmigu.cn

[S28] C：静态变量
来源：http://fz.shxzukj.cn

static int counter = 0;
来源：http://wl.hahajie.cn

[S29] C：变参函数
来源：http://ct.nszjky.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ln.bookmarksfly.cn

[S30] C：头文件保护
来源：http://qc.chemitech.net.cn

#ifndef X_H
来源：http://ea.jianghongdianzi.cn

#define X_H
来源：http://kb.muxihuayi.cn

#endif
来源：http://mq.shtwfgs.cn

[S31] C++：Hello World
来源：http://mc.shxzukj.cn

#include <iostream>
来源：http://wx.jctech888.com.cn

int main() { std::cout << "Hello\n"; }
来源：http://tk.bjjhwx.cn

[S32] C++：字符串
来源：http://mk.hnjuh.cn

std::string s = "hi";  s += "!";
来源：http://wn.bookmarksfly.cn

[S33] C++：vector 增删
来源：http://qo.colortex.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ps.colortex.cn

[S34] C++：遍历 vector
来源：http://uy.jianghongdianzi.cn

for (auto &x : v) { std::cout << x; }
来源：http://rk.chemitech.net.cn

[S35] C++：map
来源：http://zm.hahajie.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hn.bookmarksfly.cn

[S36] C++：unordered_map
来源：http://zn.jctech888.com.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://pz.huixiangedu.cn

[S37] C++：set
来源：http://ay.panjiajie.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://eq.huixiangedu.cn

[S38] C++：排序
来源：http://lc.shxzskj.cn

std::sort(v.begin(), v.end());
来源：http://zi.haigaiapp.cn

[S39] C++：自定义比较器排序
来源：http://fq.gzmigu.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://sk.521024.cn

[S40] C++：查找元素
来源：http://os.wgjwhj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://nz.gzmigu.cn

[S41] C++：类与构造函数
来源：http://xc.shxzskj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://nk.huixinmuqiang.cn

[S42] C++：继承与虚函数
来源：http://ai.bjjhwx.cn

class B : public Base { public: void f() override {} };
来源：http://um.huixiangedu.cn

[S43] C++：智能指针
来源：http://zq.panjiajie.cn

auto p = std::make_unique<int>(5);
来源：http://wj.wgjwhj.cn

[S44] C++：引用传参
来源：http://gu.shxzskj.cn

void inc(int &x) { ++x; }
来源：http://ac.jianghongdianzi.cn

[S45] C++：lambda
来源：http://be.lnxyls.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ss.chemitech.net.cn

[S46] C++：函数模板
来源：http://sw.panjiajie.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://yr.hahajie.cn

[S47] C++：结构化绑定遍历
来源：http://nx.huixiangedu.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://op.chemitech.net.cn

[S48] C++：逐行读文件
来源：http://zn.jctech888.com.cn

std::ifstream in("a.txt");  std::string line;
来源：http://pk.hahajie.cn

while (std::getline(in, line)) { }
来源：http://ap.lnxyls.cn

[S49] C++：写文件
来源：http://dp.colortex.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://nl.521024.cn

[S50] C++：格式化数字
来源：http://wh.asd995.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://vy.shxzskj.cn

[S51] C++：显式类型转换
来源：http://hh.panjiajie.cn

static_cast<double>(a) / b
来源：http://mq.chemitech.net.cn

[S52] C++：const 与 noexcept
来源：http://wj.gzmigu.cn

int size() const noexcept { return n_; }
来源：http://op.nicolike.cn

[S53] C++：移动语义
来源：http://pn.bjjhwx.cn

std::vector<int> w = std::move(v);
来源：http://rd.gzmigu.cn

[S54] C++：异常处理
来源：http://jt.hahajie.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://rk.bjjhwx.cn

[S55] C++：结构化绑定
来源：http://vg.huixinmuqiang.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://yc.jctech888.com.cn

[S56] C++：optional
来源：http://cz.szsharing.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ik.muxihuayi.cn

[S57] C++：编译期常量
来源：http://hf.haigaiapp.cn

constexpr int N = 10;
来源：http://sh.newstarts.cn

[S58] C++：命名空间
来源：http://vq.gzmigu.cn

namespace ns { int f() { return 1; } }
来源：http://gz.huixinmuqiang.cn

[S59] C++：静态断言
来源：http://ax.shxzskj.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://dp.shxzskj.cn

[S60] C++：遍历并删除元素
来源：http://fg.shtwfgs.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://jx.panjiajie.cn

================================================================================
来源：http://bt.huixiangedu.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://se.haigaiapp.cn

================================================================================
来源：http://ms.yuntaijiaju.cn

[T01] Kotlin：Hello World
来源：http://up.jctech888.com.cn

println("Hello")
来源：http://ph.colortex.cn

[T02] Kotlin：变量
来源：http://cj.jctech888.com.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://hk.colortex.cn

[T03] Kotlin：字符串模板
来源：http://li.newstarts.cn

"值: $b"
来源：http://ot.colortex.cn

[T04] Kotlin：空安全
来源：http://jg.colortex.cn

val n: String? = null;  n?.length
来源：http://pt.huanxung.cn

[T05] Kotlin：when 表达式
来源：http://cd.shtwfgs.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://or.colortex.cn

[T06] Kotlin：集合映射
来源：http://hd.chemitech.net.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://gb.chemitech.net.cn

[T07] Kotlin：集合过滤
来源：http://qe.bookmarksfly.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://pt.shtwfgs.cn

[T08] Kotlin：数据类
来源：http://gu.newstarts.cn

data class User(val name: String, val age: Int)
来源：http://np.colortex.cn

[T09] Kotlin：扩展函数
来源：http://au.shxzskj.cn

fun String.exclaim() = this + "!"
来源：http://kc.szsharing.cn

[T10] Kotlin：默认参数
来源：http://mh.hahajie.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ft.hnjuh.cn

[T11] Kotlin：协程
来源：http://gj.colortex.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://pg.chemitech.net.cn

[T12] Kotlin：解构声明
来源：http://ry.colortex.cn

val (a, b) = Pair(1, 2)
来源：http://uy.shtwfgs.cn

[T13] Kotlin：只读 Map
来源：http://as.shxzskj.cn

val m = mapOf("a" to 1)
来源：http://gj.nicolike.cn

[T14] Kotlin：循环
来源：http://tj.huanxung.cn

for (i in 1..10) println(i)
来源：http://jk.hahajie.cn

[T15] Kotlin：接口
来源：http://nf.colortex.cn

interface Shape { fun area(): Double }
来源：http://hp.hnjuh.cn

[T16] Swift：Hello World
来源：http://wa.haigaiapp.cn

print("Hello")
来源：http://fp.nicolike.cn

[T17] Swift：变量与常量
来源：http://po.nicolike.cn

var a = 1;  let b = 2
来源：http://po.chemitech.net.cn

[T18] Swift：字符串插值
来源：http://is.shxzskj.cn

"值: \(b)"
来源：http://br.huixiangedu.cn

[T19] Swift：可选绑定
来源：http://in.wgjwhj.cn

if let n = opt { print(n) }
来源：http://la.huixiangedu.cn

[T20] Swift：数组操作
来源：http://hu.haigaiapp.cn

var a = [1, 2, 3];  a.append(4)
来源：http://zb.huixiangedu.cn

[T21] Swift：遍历
来源：http://ey.huixiangedu.cn

for x in a { print(x) }
来源：http://zn.hahajie.cn

[T22] Swift：字典
来源：http://lu.bookmarksfly.cn

var d = ["a": 1];  d["b"] = 2
来源：http://vf.huixinmuqiang.cn

[T23] Swift：函数
来源：http://om.shxzskj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://cd.huixiangedu.cn

[T24] Swift：闭包
来源：http://ei.colortex.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://km.hahajie.cn

[T25] Swift：结构体
来源：http://ht.9csxet.cn

struct P { var x: Int }
来源：http://cb.nicolike.cn

[T26] Swift：类与重写
来源：http://fz.yuntaijiaju.cn

class A: Base { override func f() {} }
来源：http://es.bookmarksfly.cn

[T27] Swift：错误处理
来源：http://wn.yuntaijiaju.cn

do { try f() } catch { print(error) }
来源：http://sz.bookmarksfly.cn

[T28] Swift：枚举
来源：http://aq.jianghongdianzi.cn

enum Color { case red, green }
来源：http://fc.shxzukj.cn

[T29] Swift：guard 提前返回
来源：http://gm.jctech888.com.cn

guard let x = opt else { return }
来源：http://pa.haigaiapp.cn

[T30] Swift：协议
来源：http://qg.yuntaijiaju.cn

protocol Shape { func area() -> Double }
来源：http://yv.huanxung.cn

[T31] Lua：Hello World
来源：http://yu.muxihuayi.cn

print("Hello")
来源：http://hx.szxytkj.cn

[T32] Lua：局部变量
来源：http://cy.hnjuh.cn

local a = 1
来源：http://ak.muxihuayi.cn

[T33] Lua：表（数组）
来源：http://sx.wgjwhj.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://iy.bjjhwx.cn

[T34] Lua：遍历表
来源：http://zw.hnjuh.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ut.huixinmuqiang.cn

[T35] Lua：字典表
来源：http://iw.yuntaijiaju.cn

local d = { a = 1 };  d.b = 2
来源：http://kp.9csxet.cn

[T36] Lua：函数
来源：http://tf.yuexingan06.cn

function add(a, b) return a + b end
来源：http://yy.hnjuh.cn

[T37] Lua：字符串拼接
来源：http://pz.yuntaijiaju.cn

"a" .. "b"
来源：http://km.colortex.cn

[T38] Lua：条件
来源：http://xo.nszjky.cn

if x > 0 then print("正") end
来源：http://dp.newstarts.cn

[T39] Lua：模式匹配
来源：http://pt.huanxung.cn

string.find(s, "%d+")
来源：http://cu.huixinmuqiang.cn

[T40] Lua：元表
来源：http://uq.bjjhwx.cn

setmetatable({}, { __index = base })
来源：http://nc.szsharing.cn

[T41] Perl：Hello World
来源：http://wc.hahajie.cn

print "Hello\n";
来源：http://es.huanxung.cn

[T42] Perl：变量类型
来源：http://xf.asd995.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://at.yuexingan06.cn

[T43] Perl：字符串插值
来源：http://ca.gzmigu.cn

"值: $a"
来源：http://zs.haigaiapp.cn

[T44] Perl：条件
来源：http://ku.huixinmuqiang.cn

if ($a > 0) { print "正"; }
来源：http://bl.jianghongdianzi.cn

[T45] Perl：数组遍历
来源：http://ds.lnxyls.cn

for my $x (@arr) { print $x; }
来源：http://os.huixiangedu.cn

[T46] Perl：哈希操作
来源：http://ba.jianghongdianzi.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://bd.hahajie.cn

[T47] Perl：正则捕获
来源：http://ot.jctech888.com.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://xo.nszjky.cn

[T48] Perl：正则替换
来源：http://ec.shxzukj.cn

$s =~ s/old/new/g;
来源：http://xw.asd995.cn

[T49] Perl：函数
来源：http://xj.newstarts.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://wi.hnjuh.cn

[T50] Perl：逐行读文件
来源：http://zh.9csxet.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://cf.huanxung.cn

while (my $line = <$fh>) { print $line; }
来源：http://lt.521024.cn

[T51] Scala：Hello World
来源：http://wy.hnjuh.cn

println("Hello")
来源：http://ra.asd995.cn

[T52] Scala：变量
来源：http://pp.szxytkj.cn


<!-- 参考信息 -->