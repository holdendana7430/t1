代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：http://ka.wgjwhj.cn

[R48] awk 取指定列
来源：http://iv.shxzskj.cn

awk '{print $1, $3}' a.txt
来源：http://er.szxytkj.cn

[R49] awk 带条件
来源：http://aj.bjjhwx.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://lu.huixiangedu.cn

[R50] awk 求和
来源：http://tr.nszjky.cn

awk '{s += $2} END {print s}' a.txt
来源：http://yp.huixiangedu.cn

[R51] 排序去重取前几
来源：http://bm.9csxet.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://nh.nicolike.cn

[R52] 统计行数
来源：http://ik.jianghongdianzi.cn

wc -l a.txt
来源：http://nr.hahajie.cn

[R53] 查看文件头与实时尾
来源：http://cj.asd995.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://nl.asd995.cn

[R54] 比较两个文件
来源：http://bt.521024.cn

diff a.txt b.txt
来源：http://tb.hnjuh.cn

[R55] 压缩与解压
来源：http://ei.huixiangedu.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://be.yuntaijiaju.cn

[R56] 远程拷贝
来源：http://hj.hahajie.cn

scp file user@host:/path/
来源：http://wo.shtwfgs.cn

[R57] 远程执行命令
来源：http://bv.gzmigu.cn

ssh user@host 'uptime'
来源：http://uf.muxihuayi.cn

[R58] 下载文件
来源：http://xl.9csxet.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://by.panjiajie.cn

[R59] 发 POST JSON
来源：http://qc.gzmigu.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://hg.newstarts.cn

[R60] 只看 HTTP 状态码
来源：http://kt.shxzukj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ym.colortex.cn

[R61] 磁盘占用
来源：http://oo.yuexingan06.cn

df -h;  du -sh *
来源：http://so.chemitech.net.cn

[R62] 找最占空间的文件
来源：http://vd.shtwfgs.cn

du -ah . | sort -rh | head -10
来源：http://gr.bjjhwx.cn

[R63] 内存与进程
来源：http://cy.shxzukj.cn

free -h;  ps aux | grep nginx
来源：http://xn.newstarts.cn

[R64] 结束进程
来源：http://fp.newstarts.cn

kill -9 $(pgrep -f app.py)
来源：http://ej.haigaiapp.cn

[R65] 查看端口占用
来源：http://mh.nszjky.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://gg.shxzukj.cn

[R66] 定时任务
来源：http://av.szxytkj.cn

crontab -e;  crontab -l
来源：http://hi.muxihuayi.cn

[R67] 生成随机十六进制串
来源：http://av.newstarts.cn

openssl rand -hex 16
来源：http://ck.yuexingan06.cn

[R68] 计算文件校验值
来源：http://tw.jctech888.com.cn

sha256sum a.txt;  md5sum a.txt
来源：http://rv.lnxyls.cn

[R69] 生成随机密码
来源：http://pl.lnxyls.cn

head -c 16 /dev/urandom | base64
来源：http://xd.hnjuh.cn

[R70] 时间戳与互转
来源：http://tj.bookmarksfly.cn

date +%s;  date -d @1700000000
来源：http://ta.gzmigu.cn

[R71] 日期格式化
来源：http://sm.jctech888.com.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://vx.asd995.cn

[R72] 等待端口就绪
来源：http://vz.hnjuh.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://wj.huanxung.cn

[R73] 分割大日志
来源：http://na.nicolike.cn

split -l 1000 big.log part_
来源：http://ra.jianghongdianzi.cn

[R74] 批量重命名
来源：http://nk.hahajie.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ii.panjiajie.cn

[R75] 导出环境变量
来源：http://as.wgjwhj.cn

export PATH="$HOME/bin:$PATH"
来源：http://nu.shtwfgs.cn

[R76] 使用临时文件
来源：http://et.szsharing.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ae.9csxet.cn

[R77] 读取用户输入
来源：http://zk.szsharing.cn

read -rp "请输入: " ans
来源：http://nr.nszjky.cn

[R78] 交互式菜单
来源：http://bi.bjjhwx.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://qq.szsharing.cn

[R79] 解析命令行选项
来源：http://qn.jianghongdianzi.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://qi.huixiangedu.cn

[R80] 查看脚本执行耗时
来源：http://bt.yuexingan06.cn

time ./run.sh
来源：http://dm.lnxyls.cn

================================================================================
来源：http://op.jianghongdianzi.cn

S. C / C++ 专题
来源：http://cj.panjiajie.cn

================================================================================
来源：http://sy.asd995.cn

[S01] C：Hello World
来源：http://xy.gzmigu.cn

#include <stdio.h>
来源：http://nl.shxzskj.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://cl.shtwfgs.cn

[S02] C：变量与格式化输出
来源：http://vo.9csxet.cn

int a = 10; printf("%d\n", a);
来源：http://jo.gzmigu.cn

[S03] C：读入整数
来源：http://pe.yuexingan06.cn

int x; scanf("%d", &x);
来源：http://ra.muxihuayi.cn

[S04] C：字符串复制
来源：http://tl.shxzukj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://yj.9csxet.cn

[S05] C：字符串长度
来源：http://gs.521024.cn

strlen(s)
来源：http://no.bookmarksfly.cn

[S06] C：字符串比较
来源：http://ns.gzmigu.cn

strcmp(a, b) == 0
来源：http://yd.9csxet.cn

[S07] C：数组遍历求和
来源：http://uh.huixiangedu.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://dn.jctech888.com.cn

[S08] C：动态内存分配与释放
来源：http://od.shxzukj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://xt.bjjhwx.cn

[S09] C：结构体定义与初始化
来源：http://za.wgjwhj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://xs.bookmarksfly.cn

[S10] C：指针与解引用
来源：http://js.huanxung.cn

int *p = &a;  *p = 5;
来源：http://bp.wgjwhj.cn

[S11] C：逐行读文件
来源：http://pk.wgjwhj.cn

FILE *f = fopen("a.txt", "r");
来源：http://wf.nszjky.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://lu.huixinmuqiang.cn

fclose(f);
来源：http://lq.chemitech.net.cn

[S12] C：写文件
来源：http://jq.asd995.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://el.panjiajie.cn

[S13] C：宏定义
来源：http://us.gzmigu.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://et.jianghongdianzi.cn

[S14] C：枚举
来源：http://ca.shtwfgs.cn

enum Color { RED, GREEN, BLUE };
来源：http://gi.huanxung.cn

[S15] C：类型转换
来源：http://ce.asd995.cn

(double) a / b
来源：http://tc.nszjky.cn

[S16] C：位操作置位
来源：http://jo.nszjky.cn

x |= (1 << 3);
来源：http://hv.yuntaijiaju.cn

[S17] C：安全拼接字符串
来源：http://kx.muxihuayi.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://tw.521024.cn

[S18] C：命令行参数
来源：http://ku.haigaiapp.cn

int main(int argc, char **argv)
来源：http://jc.wgjwhj.cn

[S19] C：快速排序
来源：http://oe.nicolike.cn

qsort(a, n, sizeof(int), cmp);
来源：http://vd.yuntaijiaju.cn

[S20] C：二分查找
来源：http://kd.shtwfgs.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://zn.jctech888.com.cn

[S21] C：字符类别判断
来源：http://jh.huixiangedu.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://gj.yuntaijiaju.cn

[S22] C：字符串转数字
来源：http://fx.huixiangedu.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ex.panjiajie.cn

[S23] C：随机数
来源：http://zy.haigaiapp.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://yj.9csxet.cn

[S24] C：获取本地时间
来源：http://hj.huixinmuqiang.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://kf.shxzskj.cn

[S25] C：内存拷贝
来源：http://no.nicolike.cn

memcpy(dst, src, n);
来源：http://ds.muxihuayi.cn

[S26] C：内存清零
来源：http://we.panjiajie.cn

memset(a, 0, sizeof a);
来源：http://pv.wgjwhj.cn

[S27] C：定义常量
来源：http://qq.haigaiapp.cn

const double PI = 3.14159;
来源：http://sj.jctech888.com.cn

[S28] C：静态变量
来源：http://oc.gzmigu.cn

static int counter = 0;
来源：http://ks.huixiangedu.cn

[S29] C：变参函数
来源：http://hw.nicolike.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://wi.huixiangedu.cn

[S30] C：头文件保护
来源：http://ih.asd995.cn

#ifndef X_H
来源：http://wr.jctech888.com.cn

#define X_H
来源：http://dr.chemitech.net.cn

#endif
来源：http://jy.nszjky.cn

[S31] C++：Hello World
来源：http://yk.shxzukj.cn

#include <iostream>
来源：http://bc.colortex.cn

int main() { std::cout << "Hello\n"; }
来源：http://ox.colortex.cn

[S32] C++：字符串
来源：http://jy.nszjky.cn

std::string s = "hi";  s += "!";
来源：http://so.szsharing.cn

[S33] C++：vector 增删
来源：http://ve.hahajie.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qo.newstarts.cn

[S34] C++：遍历 vector
来源：http://qe.szsharing.cn

for (auto &x : v) { std::cout << x; }
来源：http://ib.huixiangedu.cn

[S35] C++：map
来源：http://lf.hnjuh.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://nx.9csxet.cn

[S36] C++：unordered_map
来源：http://el.szsharing.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ou.nszjky.cn

[S37] C++：set
来源：http://tt.huixinmuqiang.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://bg.colortex.cn

[S38] C++：排序
来源：http://qb.bookmarksfly.cn

std::sort(v.begin(), v.end());
来源：http://xm.lnxyls.cn

[S39] C++：自定义比较器排序
来源：http://ny.shxzskj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://yy.lnxyls.cn

[S40] C++：查找元素
来源：http://is.bjjhwx.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://xk.yuexingan06.cn

[S41] C++：类与构造函数
来源：http://lt.huanxung.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://jj.yuntaijiaju.cn

[S42] C++：继承与虚函数
来源：http://kq.yuexingan06.cn

class B : public Base { public: void f() override {} };
来源：http://qf.szsharing.cn

[S43] C++：智能指针
来源：http://fg.bjjhwx.cn

auto p = std::make_unique<int>(5);
来源：http://qg.nicolike.cn

[S44] C++：引用传参
来源：http://pw.bookmarksfly.cn

void inc(int &x) { ++x; }
来源：http://bs.gzmigu.cn

[S45] C++：lambda
来源：http://bf.nicolike.cn

auto add = [](int a, int b) { return a + b; };
来源：http://hp.shxzskj.cn

[S46] C++：函数模板
来源：http://bh.szsharing.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://hh.gzmigu.cn

[S47] C++：结构化绑定遍历
来源：http://bm.gzmigu.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://cn.nicolike.cn

[S48] C++：逐行读文件
来源：http://gy.jianghongdianzi.cn

std::ifstream in("a.txt");  std::string line;
来源：http://xb.colortex.cn

while (std::getline(in, line)) { }
来源：http://uj.9csxet.cn

[S49] C++：写文件
来源：http://hm.panjiajie.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hj.jianghongdianzi.cn

[S50] C++：格式化数字
来源：http://cp.szsharing.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wz.szsharing.cn

[S51] C++：显式类型转换
来源：http://mm.muxihuayi.cn

static_cast<double>(a) / b
来源：http://vu.bookmarksfly.cn

[S52] C++：const 与 noexcept
来源：http://le.yuntaijiaju.cn

int size() const noexcept { return n_; }
来源：http://wm.newstarts.cn

[S53] C++：移动语义
来源：http://su.wgjwhj.cn

std::vector<int> w = std::move(v);
来源：http://nd.haigaiapp.cn

[S54] C++：异常处理
来源：http://ma.hahajie.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://sl.yuntaijiaju.cn

[S55] C++：结构化绑定
来源：http://bh.haigaiapp.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://xy.shxzukj.cn

[S56] C++：optional
来源：http://vj.wgjwhj.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ar.shxzukj.cn

[S57] C++：编译期常量
来源：http://ky.shxzskj.cn

constexpr int N = 10;
来源：http://hl.nicolike.cn

[S58] C++：命名空间
来源：http://zv.bookmarksfly.cn

namespace ns { int f() { return 1; } }
来源：http://wh.gzmigu.cn

[S59] C++：静态断言
来源：http://in.hnjuh.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://sj.szxytkj.cn

[S60] C++：遍历并删除元素
来源：http://ss.hahajie.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://fz.bjjhwx.cn

================================================================================
来源：http://iw.newstarts.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://de.lnxyls.cn

================================================================================
来源：http://ba.szxytkj.cn

[T01] Kotlin：Hello World
来源：http://ou.wgjwhj.cn

println("Hello")
来源：http://kl.colortex.cn

[T02] Kotlin：变量
来源：http://lk.shxzukj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://on.yuexingan06.cn

[T03] Kotlin：字符串模板
来源：http://ec.shxzskj.cn

"值: $b"
来源：http://ye.wgjwhj.cn

[T04] Kotlin：空安全
来源：http://xy.szxytkj.cn

val n: String? = null;  n?.length
来源：http://ol.hahajie.cn

[T05] Kotlin：when 表达式
来源：http://wr.shxzukj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://eb.521024.cn

[T06] Kotlin：集合映射
来源：http://ly.jianghongdianzi.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ek.bookmarksfly.cn

[T07] Kotlin：集合过滤
来源：http://ec.huixiangedu.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://dy.muxihuayi.cn

[T08] Kotlin：数据类
来源：http://ln.nszjky.cn

data class User(val name: String, val age: Int)
来源：http://aw.shxzskj.cn

[T09] Kotlin：扩展函数
来源：http://af.521024.cn

fun String.exclaim() = this + "!"
来源：http://sm.muxihuayi.cn

[T10] Kotlin：默认参数
来源：http://ve.shtwfgs.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://fr.gzmigu.cn

[T11] Kotlin：协程
来源：http://sq.hahajie.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://pt.panjiajie.cn

[T12] Kotlin：解构声明
来源：http://qx.nszjky.cn

val (a, b) = Pair(1, 2)
来源：http://bp.panjiajie.cn

[T13] Kotlin：只读 Map
来源：http://yh.yuexingan06.cn

val m = mapOf("a" to 1)
来源：http://ma.yuntaijiaju.cn

[T14] Kotlin：循环
来源：http://sg.hnjuh.cn

for (i in 1..10) println(i)
来源：http://xd.huanxung.cn

[T15] Kotlin：接口
来源：http://zw.muxihuayi.cn

interface Shape { fun area(): Double }
来源：http://aq.wgjwhj.cn

[T16] Swift：Hello World
来源：http://px.shxzskj.cn

print("Hello")
来源：http://tm.yuexingan06.cn

[T17] Swift：变量与常量
来源：http://yx.muxihuayi.cn

var a = 1;  let b = 2
来源：http://sz.huixiangedu.cn

[T18] Swift：字符串插值
来源：http://mi.hnjuh.cn

"值: \(b)"
来源：http://zv.newstarts.cn

[T19] Swift：可选绑定
来源：http://mu.muxihuayi.cn

if let n = opt { print(n) }
来源：http://te.yuexingan06.cn

[T20] Swift：数组操作
来源：http://qp.huixiangedu.cn

var a = [1, 2, 3];  a.append(4)
来源：http://fq.lnxyls.cn

[T21] Swift：遍历
来源：http://qt.haigaiapp.cn

for x in a { print(x) }
来源：http://wq.asd995.cn

[T22] Swift：字典
来源：http://gp.bjjhwx.cn

var d = ["a": 1];  d["b"] = 2
来源：http://pk.shxzskj.cn

[T23] Swift：函数
来源：http://sr.bjjhwx.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mi.shtwfgs.cn

[T24] Swift：闭包
来源：http://kc.bjjhwx.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ji.lnxyls.cn

[T25] Swift：结构体
来源：http://jt.shtwfgs.cn

struct P { var x: Int }
来源：http://im.9csxet.cn

[T26] Swift：类与重写
来源：http://pu.huixinmuqiang.cn

class A: Base { override func f() {} }
来源：http://ng.bjjhwx.cn

[T27] Swift：错误处理
来源：http://wd.shxzskj.cn

do { try f() } catch { print(error) }
来源：http://th.gzmigu.cn

[T28] Swift：枚举
来源：http://ot.panjiajie.cn

enum Color { case red, green }
来源：http://mo.lnxyls.cn

[T29] Swift：guard 提前返回
来源：http://ia.newstarts.cn

guard let x = opt else { return }
来源：http://ph.jctech888.com.cn

[T30] Swift：协议
来源：http://fb.asd995.cn

protocol Shape { func area() -> Double }
来源：http://iq.huixinmuqiang.cn

[T31] Lua：Hello World
来源：http://zk.yuexingan06.cn

print("Hello")
来源：http://fs.yuntaijiaju.cn

[T32] Lua：局部变量
来源：http://fy.nszjky.cn

local a = 1
来源：http://nm.colortex.cn

[T33] Lua：表（数组）
来源：http://yb.asd995.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://sy.jctech888.com.cn

[T34] Lua：遍历表
来源：http://ue.jctech888.com.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://uy.huixinmuqiang.cn

[T35] Lua：字典表
来源：http://ar.asd995.cn

local d = { a = 1 };  d.b = 2
来源：http://qa.bjjhwx.cn

[T36] Lua：函数
来源：http://yu.colortex.cn

function add(a, b) return a + b end
来源：http://oq.gzmigu.cn

[T37] Lua：字符串拼接
来源：http://za.shxzskj.cn

"a" .. "b"
来源：http://lt.gzmigu.cn

[T38] Lua：条件
来源：http://ak.shxzukj.cn

if x > 0 then print("正") end
来源：http://ko.9csxet.cn

[T39] Lua：模式匹配
来源：http://ww.newstarts.cn

string.find(s, "%d+")
来源：http://id.gzmigu.cn

[T40] Lua：元表
来源：http://dw.9csxet.cn

setmetatable({}, { __index = base })
来源：http://cf.szsharing.cn

[T41] Perl：Hello World
来源：http://io.bjjhwx.cn

print "Hello\n";
来源：http://of.szsharing.cn

[T42] Perl：变量类型
来源：http://di.jctech888.com.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://fl.jctech888.com.cn

[T43] Perl：字符串插值
来源：http://jv.chemitech.net.cn

"值: $a"
来源：http://bu.huanxung.cn

[T44] Perl：条件
来源：http://pk.asd995.cn

if ($a > 0) { print "正"; }
来源：http://rf.bookmarksfly.cn

[T45] Perl：数组遍历
来源：http://du.yuexingan06.cn

for my $x (@arr) { print $x; }
来源：http://tr.bookmarksfly.cn

[T46] Perl：哈希操作
来源：http://sd.szxytkj.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://cf.shxzskj.cn

[T47] Perl：正则捕获
来源：http://zz.521024.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://pa.lnxyls.cn

[T48] Perl：正则替换
来源：http://ap.nszjky.cn

$s =~ s/old/new/g;
来源：http://fc.huixinmuqiang.cn

[T49] Perl：函数
来源：http://nz.gzmigu.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://vq.521024.cn

[T50] Perl：逐行读文件
来源：http://td.szsharing.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://em.chemitech.net.cn


<!-- 参考信息 -->