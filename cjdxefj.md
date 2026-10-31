代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：http://nn.521024.cn

[R48] awk 取指定列
来源：http://fl.asd995.cn

awk '{print $1, $3}' a.txt
来源：http://hl.huanxung.cn

[R49] awk 带条件
来源：http://tg.shtwfgs.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ka.lnxyls.cn

[R50] awk 求和
来源：http://bz.shxzukj.cn

awk '{s += $2} END {print s}' a.txt
来源：http://hj.gzmigu.cn

[R51] 排序去重取前几
来源：http://pm.lnxyls.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://op.newstarts.cn

[R52] 统计行数
来源：http://om.wgjwhj.cn

wc -l a.txt
来源：http://jg.jianghongdianzi.cn

[R53] 查看文件头与实时尾
来源：http://mc.haigaiapp.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://bf.yuntaijiaju.cn

[R54] 比较两个文件
来源：http://ca.chemitech.net.cn

diff a.txt b.txt
来源：http://dw.shxzukj.cn

[R55] 压缩与解压
来源：http://fh.nszjky.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://gy.haigaiapp.cn

[R56] 远程拷贝
来源：http://zq.asd995.cn

scp file user@host:/path/
来源：http://dq.hahajie.cn

[R57] 远程执行命令
来源：http://ul.nicolike.cn

ssh user@host 'uptime'
来源：http://nt.hahajie.cn

[R58] 下载文件
来源：http://ho.shxzskj.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ji.521024.cn

[R59] 发 POST JSON
来源：http://yp.nszjky.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://zs.gzmigu.cn

[R60] 只看 HTTP 状态码
来源：http://xq.asd995.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ik.hahajie.cn

[R61] 磁盘占用
来源：http://da.huixiangedu.cn

df -h;  du -sh *
来源：http://ef.huanxung.cn

[R62] 找最占空间的文件
来源：http://pu.gzmigu.cn

du -ah . | sort -rh | head -10
来源：http://mn.jctech888.com.cn

[R63] 内存与进程
来源：http://bk.jctech888.com.cn

free -h;  ps aux | grep nginx
来源：http://uf.asd995.cn

[R64] 结束进程
来源：http://ie.9csxet.cn

kill -9 $(pgrep -f app.py)
来源：http://xl.bjjhwx.cn

[R65] 查看端口占用
来源：http://ne.yuexingan06.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://vz.gzmigu.cn

[R66] 定时任务
来源：http://jd.jctech888.com.cn

crontab -e;  crontab -l
来源：http://ao.asd995.cn

[R67] 生成随机十六进制串
来源：http://zw.asd995.cn

openssl rand -hex 16
来源：http://xl.hnjuh.cn

[R68] 计算文件校验值
来源：http://kj.huanxung.cn

sha256sum a.txt;  md5sum a.txt
来源：http://vk.huixiangedu.cn

[R69] 生成随机密码
来源：http://fr.lnxyls.cn

head -c 16 /dev/urandom | base64
来源：http://bv.gzmigu.cn

[R70] 时间戳与互转
来源：http://tr.shtwfgs.cn

date +%s;  date -d @1700000000
来源：http://dy.shxzskj.cn

[R71] 日期格式化
来源：http://hr.nicolike.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ry.jctech888.com.cn

[R72] 等待端口就绪
来源：http://va.gzmigu.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://db.bookmarksfly.cn

[R73] 分割大日志
来源：http://kt.haigaiapp.cn

split -l 1000 big.log part_
来源：http://et.szxytkj.cn

[R74] 批量重命名
来源：http://ey.shtwfgs.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mv.wgjwhj.cn

[R75] 导出环境变量
来源：http://vf.szsharing.cn

export PATH="$HOME/bin:$PATH"
来源：http://tb.chemitech.net.cn

[R76] 使用临时文件
来源：http://kd.hnjuh.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://bm.jianghongdianzi.cn

[R77] 读取用户输入
来源：http://hc.wgjwhj.cn

read -rp "请输入: " ans
来源：http://wp.wgjwhj.cn

[R78] 交互式菜单
来源：http://gg.chemitech.net.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://ql.shtwfgs.cn

[R79] 解析命令行选项
来源：http://vz.asd995.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://fh.yuexingan06.cn

[R80] 查看脚本执行耗时
来源：http://hz.asd995.cn

time ./run.sh
来源：http://es.huixinmuqiang.cn

================================================================================
来源：http://me.521024.cn

S. C / C++ 专题
来源：http://ah.szxytkj.cn

================================================================================
来源：http://ps.hahajie.cn

[S01] C：Hello World
来源：http://ml.nicolike.cn

#include <stdio.h>
来源：http://fx.huixinmuqiang.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://rt.yuexingan06.cn

[S02] C：变量与格式化输出
来源：http://fe.asd995.cn

int a = 10; printf("%d\n", a);
来源：http://rd.jianghongdianzi.cn

[S03] C：读入整数
来源：http://iw.shxzskj.cn

int x; scanf("%d", &x);
来源：http://ht.haigaiapp.cn

[S04] C：字符串复制
来源：http://ck.shxzukj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://hj.hahajie.cn

[S05] C：字符串长度
来源：http://va.huanxung.cn

strlen(s)
来源：http://gz.muxihuayi.cn

[S06] C：字符串比较
来源：http://wk.hnjuh.cn

strcmp(a, b) == 0
来源：http://rt.521024.cn

[S07] C：数组遍历求和
来源：http://bd.9csxet.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://xr.lnxyls.cn

[S08] C：动态内存分配与释放
来源：http://dh.hahajie.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://uz.muxihuayi.cn

[S09] C：结构体定义与初始化
来源：http://rc.9csxet.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://oo.huixinmuqiang.cn

[S10] C：指针与解引用
来源：http://wz.gzmigu.cn

int *p = &a;  *p = 5;
来源：http://fr.shxzukj.cn

[S11] C：逐行读文件
来源：http://ej.bjjhwx.cn

FILE *f = fopen("a.txt", "r");
来源：http://uq.9csxet.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://cs.9csxet.cn

fclose(f);
来源：http://ez.chemitech.net.cn

[S12] C：写文件
来源：http://hk.chemitech.net.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://nd.muxihuayi.cn

[S13] C：宏定义
来源：http://xd.nszjky.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://bx.hnjuh.cn

[S14] C：枚举
来源：http://fb.gzmigu.cn

enum Color { RED, GREEN, BLUE };
来源：http://jb.haigaiapp.cn

[S15] C：类型转换
来源：http://uk.shxzskj.cn

(double) a / b
来源：http://bl.huixinmuqiang.cn

[S16] C：位操作置位
来源：http://nd.lnxyls.cn

x |= (1 << 3);
来源：http://lo.panjiajie.cn

[S17] C：安全拼接字符串
来源：http://rn.jctech888.com.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ej.szxytkj.cn

[S18] C：命令行参数
来源：http://nt.9csxet.cn

int main(int argc, char **argv)
来源：http://ze.chemitech.net.cn

[S19] C：快速排序
来源：http://tr.hahajie.cn

qsort(a, n, sizeof(int), cmp);
来源：http://og.colortex.cn

[S20] C：二分查找
来源：http://ub.yuntaijiaju.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://as.panjiajie.cn

[S21] C：字符类别判断
来源：http://et.szsharing.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://nl.szxytkj.cn

[S22] C：字符串转数字
来源：http://ca.asd995.cn

atoi("42");  strtod("3.14", NULL);
来源：http://rn.521024.cn

[S23] C：随机数
来源：http://jg.asd995.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://xr.chemitech.net.cn

[S24] C：获取本地时间
来源：http://no.szxytkj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ua.panjiajie.cn

[S25] C：内存拷贝
来源：http://ka.hnjuh.cn

memcpy(dst, src, n);
来源：http://kd.huixiangedu.cn

[S26] C：内存清零
来源：http://uu.szsharing.cn

memset(a, 0, sizeof a);
来源：http://ya.newstarts.cn

[S27] C：定义常量
来源：http://im.9csxet.cn

const double PI = 3.14159;
来源：http://nr.szxytkj.cn

[S28] C：静态变量
来源：http://ht.wgjwhj.cn

static int counter = 0;
来源：http://qt.bookmarksfly.cn

[S29] C：变参函数
来源：http://ta.colortex.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://se.nszjky.cn

[S30] C：头文件保护
来源：http://zv.hnjuh.cn

#ifndef X_H
来源：http://oc.szsharing.cn

#define X_H
来源：http://lw.panjiajie.cn

#endif
来源：http://lr.nszjky.cn

[S31] C++：Hello World
来源：http://yz.panjiajie.cn

#include <iostream>
来源：http://yt.nszjky.cn

int main() { std::cout << "Hello\n"; }
来源：http://jn.lnxyls.cn

[S32] C++：字符串
来源：http://dy.bookmarksfly.cn

std::string s = "hi";  s += "!";
来源：http://ew.hahajie.cn

[S33] C++：vector 增删
来源：http://fz.nicolike.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://pt.szsharing.cn

[S34] C++：遍历 vector
来源：http://uk.hahajie.cn

for (auto &x : v) { std::cout << x; }
来源：http://zg.nicolike.cn

[S35] C++：map
来源：http://gk.wgjwhj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://oo.newstarts.cn

[S36] C++：unordered_map
来源：http://jg.shtwfgs.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://yy.shtwfgs.cn

[S37] C++：set
来源：http://el.nicolike.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://qi.shxzskj.cn

[S38] C++：排序
来源：http://nw.bookmarksfly.cn

std::sort(v.begin(), v.end());
来源：http://bm.jianghongdianzi.cn

[S39] C++：自定义比较器排序
来源：http://pg.panjiajie.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ns.wgjwhj.cn

[S40] C++：查找元素
来源：http://yy.huanxung.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hb.huixiangedu.cn

[S41] C++：类与构造函数
来源：http://ls.shxzskj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://mj.panjiajie.cn

[S42] C++：继承与虚函数
来源：http://oy.lnxyls.cn

class B : public Base { public: void f() override {} };
来源：http://xz.asd995.cn

[S43] C++：智能指针
来源：http://em.szsharing.cn

auto p = std::make_unique<int>(5);
来源：http://qi.muxihuayi.cn

[S44] C++：引用传参
来源：http://im.huixiangedu.cn

void inc(int &x) { ++x; }
来源：http://ov.jctech888.com.cn

[S45] C++：lambda
来源：http://aj.bookmarksfly.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ue.hnjuh.cn

[S46] C++：函数模板
来源：http://jj.haigaiapp.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://vu.panjiajie.cn

[S47] C++：结构化绑定遍历
来源：http://wr.hnjuh.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qi.chemitech.net.cn

[S48] C++：逐行读文件
来源：http://md.asd995.cn

std::ifstream in("a.txt");  std::string line;
来源：http://wx.shxzskj.cn

while (std::getline(in, line)) { }
来源：http://jz.haigaiapp.cn

[S49] C++：写文件
来源：http://ud.shxzskj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://bg.9csxet.cn

[S50] C++：格式化数字
来源：http://mn.shxzukj.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ct.szsharing.cn

[S51] C++：显式类型转换
来源：http://qe.huixiangedu.cn

static_cast<double>(a) / b
来源：http://iz.huixiangedu.cn

[S52] C++：const 与 noexcept
来源：http://oq.hnjuh.cn

int size() const noexcept { return n_; }
来源：http://ex.bjjhwx.cn

[S53] C++：移动语义
来源：http://qa.newstarts.cn

std::vector<int> w = std::move(v);
来源：http://ca.lnxyls.cn

[S54] C++：异常处理
来源：http://ii.newstarts.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://zf.muxihuayi.cn

[S55] C++：结构化绑定
来源：http://ag.9csxet.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://rj.huixiangedu.cn

[S56] C++：optional
来源：http://dz.yuntaijiaju.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://lj.lnxyls.cn

[S57] C++：编译期常量
来源：http://lc.shxzukj.cn

constexpr int N = 10;
来源：http://gg.gzmigu.cn

[S58] C++：命名空间
来源：http://jt.9csxet.cn

namespace ns { int f() { return 1; } }
来源：http://ao.hahajie.cn

[S59] C++：静态断言
来源：http://ww.yuntaijiaju.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://uu.shxzukj.cn

[S60] C++：遍历并删除元素
来源：http://lw.newstarts.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://vf.jctech888.com.cn

================================================================================
来源：http://fx.chemitech.net.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://cy.521024.cn

================================================================================
来源：http://kr.panjiajie.cn

[T01] Kotlin：Hello World
来源：http://qj.shtwfgs.cn

println("Hello")
来源：http://mr.newstarts.cn

[T02] Kotlin：变量
来源：http://wz.9csxet.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://vg.asd995.cn

[T03] Kotlin：字符串模板
来源：http://az.muxihuayi.cn

"值: $b"
来源：http://eo.wgjwhj.cn

[T04] Kotlin：空安全
来源：http://mv.newstarts.cn

val n: String? = null;  n?.length
来源：http://iq.jianghongdianzi.cn

[T05] Kotlin：when 表达式
来源：http://rp.hahajie.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ju.huixinmuqiang.cn

[T06] Kotlin：集合映射
来源：http://xq.nicolike.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://se.nszjky.cn

[T07] Kotlin：集合过滤
来源：http://yc.huanxung.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://iy.yuntaijiaju.cn

[T08] Kotlin：数据类
来源：http://tt.bjjhwx.cn

data class User(val name: String, val age: Int)
来源：http://ye.huixiangedu.cn

[T09] Kotlin：扩展函数
来源：http://pj.gzmigu.cn

fun String.exclaim() = this + "!"
来源：http://ah.muxihuayi.cn

[T10] Kotlin：默认参数
来源：http://rf.wgjwhj.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://kg.wgjwhj.cn

[T11] Kotlin：协程
来源：http://zi.jianghongdianzi.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://pu.szxytkj.cn

[T12] Kotlin：解构声明
来源：http://xu.muxihuayi.cn

val (a, b) = Pair(1, 2)
来源：http://xs.hahajie.cn

[T13] Kotlin：只读 Map
来源：http://dd.521024.cn

val m = mapOf("a" to 1)
来源：http://ro.bjjhwx.cn

[T14] Kotlin：循环
来源：http://ph.colortex.cn

for (i in 1..10) println(i)
来源：http://xf.521024.cn

[T15] Kotlin：接口
来源：http://cs.yuntaijiaju.cn

interface Shape { fun area(): Double }
来源：http://xv.521024.cn

[T16] Swift：Hello World
来源：http://xq.9csxet.cn

print("Hello")
来源：http://xl.colortex.cn

[T17] Swift：变量与常量
来源：http://oz.huixiangedu.cn

var a = 1;  let b = 2
来源：http://vb.huixiangedu.cn

[T18] Swift：字符串插值
来源：http://rm.huixinmuqiang.cn

"值: \(b)"
来源：http://bb.521024.cn

[T19] Swift：可选绑定
来源：http://eb.9csxet.cn

if let n = opt { print(n) }
来源：http://bv.hahajie.cn

[T20] Swift：数组操作
来源：http://dn.panjiajie.cn

var a = [1, 2, 3];  a.append(4)
来源：http://nz.9csxet.cn

[T21] Swift：遍历
来源：http://ki.huanxung.cn

for x in a { print(x) }
来源：http://fx.szxytkj.cn

[T22] Swift：字典
来源：http://ke.panjiajie.cn

var d = ["a": 1];  d["b"] = 2
来源：http://tt.521024.cn

[T23] Swift：函数
来源：http://gx.huanxung.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://jg.nszjky.cn

[T24] Swift：闭包
来源：http://tz.jianghongdianzi.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://eh.newstarts.cn

[T25] Swift：结构体
来源：http://gs.shtwfgs.cn

struct P { var x: Int }
来源：http://cy.huanxung.cn

[T26] Swift：类与重写
来源：http://wq.asd995.cn

class A: Base { override func f() {} }
来源：http://hf.szxytkj.cn

[T27] Swift：错误处理
来源：http://dq.szxytkj.cn

do { try f() } catch { print(error) }
来源：http://ie.szxytkj.cn

[T28] Swift：枚举
来源：http://oy.9csxet.cn

enum Color { case red, green }
来源：http://ww.newstarts.cn

[T29] Swift：guard 提前返回
来源：http://zq.jctech888.com.cn

guard let x = opt else { return }
来源：http://ys.521024.cn

[T30] Swift：协议
来源：http://vz.colortex.cn

protocol Shape { func area() -> Double }
来源：http://tg.lnxyls.cn

[T31] Lua：Hello World
来源：http://ev.nicolike.cn

print("Hello")
来源：http://zo.haigaiapp.cn

[T32] Lua：局部变量
来源：http://vy.wgjwhj.cn

local a = 1
来源：http://ra.521024.cn

[T33] Lua：表（数组）
来源：http://mw.yuexingan06.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://bb.huixinmuqiang.cn

[T34] Lua：遍历表
来源：http://zb.nicolike.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://tb.newstarts.cn

[T35] Lua：字典表
来源：http://gn.huixinmuqiang.cn

local d = { a = 1 };  d.b = 2
来源：http://hu.haigaiapp.cn

[T36] Lua：函数
来源：http://sw.yuntaijiaju.cn

function add(a, b) return a + b end
来源：http://id.yuexingan06.cn

[T37] Lua：字符串拼接
来源：http://hw.muxihuayi.cn

"a" .. "b"
来源：http://ad.asd995.cn

[T38] Lua：条件
来源：http://pj.wgjwhj.cn

if x > 0 then print("正") end
来源：http://of.shtwfgs.cn

[T39] Lua：模式匹配
来源：http://xr.shxzukj.cn

string.find(s, "%d+")
来源：http://sm.nszjky.cn

[T40] Lua：元表
来源：http://kx.muxihuayi.cn

setmetatable({}, { __index = base })
来源：http://er.huixinmuqiang.cn

[T41] Perl：Hello World
来源：http://yt.shxzukj.cn

print "Hello\n";
来源：http://zl.huanxung.cn

[T42] Perl：变量类型
来源：http://mk.asd995.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://qz.shxzukj.cn

[T43] Perl：字符串插值
来源：http://ko.colortex.cn

"值: $a"
来源：http://mt.521024.cn

[T44] Perl：条件
来源：http://pg.jctech888.com.cn

if ($a > 0) { print "正"; }
来源：http://xd.muxihuayi.cn

[T45] Perl：数组遍历
来源：http://jb.newstarts.cn

for my $x (@arr) { print $x; }
来源：http://gl.nszjky.cn

[T46] Perl：哈希操作
来源：http://wj.hnjuh.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://jr.hnjuh.cn

[T47] Perl：正则捕获
来源：http://is.nszjky.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://jy.jctech888.com.cn

[T48] Perl：正则替换
来源：http://bx.9csxet.cn

$s =~ s/old/new/g;
来源：http://en.bookmarksfly.cn

[T49] Perl：函数
来源：http://ub.nicolike.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://fx.9csxet.cn

[T50] Perl：逐行读文件
来源：http://df.bookmarksfly.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://gr.hahajie.cn


<!-- 参考信息 -->