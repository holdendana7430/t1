代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://wj.521024.cn

[R52] 统计行数
来源：http://kb.hnjuh.cn

wc -l a.txt
来源：http://da.muxihuayi.cn

[R53] 查看文件头与实时尾
来源：http://ll.lnxyls.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://hr.lnxyls.cn

[R54] 比较两个文件
来源：http://gm.shxzukj.cn

diff a.txt b.txt
来源：http://ku.chemitech.net.cn

[R55] 压缩与解压
来源：http://er.colortex.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://sq.colortex.cn

[R56] 远程拷贝
来源：http://nz.muxihuayi.cn

scp file user@host:/path/
来源：http://bw.wgjwhj.cn

[R57] 远程执行命令
来源：http://if.yuexingan06.cn

ssh user@host 'uptime'
来源：http://zl.shxzukj.cn

[R58] 下载文件
来源：http://qo.nszjky.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://bz.9csxet.cn

[R59] 发 POST JSON
来源：http://pd.shxzukj.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vo.shtwfgs.cn

[R60] 只看 HTTP 状态码
来源：http://hl.shxzskj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://fn.bookmarksfly.cn

[R61] 磁盘占用
来源：http://pr.shtwfgs.cn

df -h;  du -sh *
来源：http://nf.9csxet.cn

[R62] 找最占空间的文件
来源：http://im.jianghongdianzi.cn

du -ah . | sort -rh | head -10
来源：http://zb.chemitech.net.cn

[R63] 内存与进程
来源：http://rp.panjiajie.cn

free -h;  ps aux | grep nginx
来源：http://vd.hnjuh.cn

[R64] 结束进程
来源：http://hh.shxzukj.cn

kill -9 $(pgrep -f app.py)
来源：http://vx.chemitech.net.cn

[R65] 查看端口占用
来源：http://da.jctech888.com.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://qw.nszjky.cn

[R66] 定时任务
来源：http://ti.chemitech.net.cn

crontab -e;  crontab -l
来源：http://by.szxytkj.cn

[R67] 生成随机十六进制串
来源：http://rm.szxytkj.cn

openssl rand -hex 16
来源：http://ht.huixiangedu.cn

[R68] 计算文件校验值
来源：http://is.hahajie.cn

sha256sum a.txt;  md5sum a.txt
来源：http://em.hahajie.cn

[R69] 生成随机密码
来源：http://qn.yuntaijiaju.cn

head -c 16 /dev/urandom | base64
来源：http://es.haigaiapp.cn

[R70] 时间戳与互转
来源：http://bt.chemitech.net.cn

date +%s;  date -d @1700000000
来源：http://oz.shtwfgs.cn

[R71] 日期格式化
来源：http://is.bjjhwx.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://eu.newstarts.cn

[R72] 等待端口就绪
来源：http://el.jctech888.com.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://cr.nszjky.cn

[R73] 分割大日志
来源：http://ue.bookmarksfly.cn

split -l 1000 big.log part_
来源：http://re.shxzukj.cn

[R74] 批量重命名
来源：http://lx.hahajie.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ti.nicolike.cn

[R75] 导出环境变量
来源：http://aj.lnxyls.cn

export PATH="$HOME/bin:$PATH"
来源：http://bs.yuntaijiaju.cn

[R76] 使用临时文件
来源：http://kd.huanxung.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mu.szsharing.cn

[R77] 读取用户输入
来源：http://zt.jctech888.com.cn

read -rp "请输入: " ans
来源：http://lm.nicolike.cn

[R78] 交互式菜单
来源：http://kr.yuntaijiaju.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://gx.nszjky.cn

[R79] 解析命令行选项
来源：http://im.panjiajie.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://mh.hnjuh.cn

[R80] 查看脚本执行耗时
来源：http://wn.bookmarksfly.cn

time ./run.sh
来源：http://kf.hahajie.cn

================================================================================
来源：http://ou.szxytkj.cn

S. C / C++ 专题
来源：http://pb.newstarts.cn

================================================================================
来源：http://qs.521024.cn

[S01] C：Hello World
来源：http://nx.521024.cn

#include <stdio.h>
来源：http://dp.huanxung.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://sg.nicolike.cn

[S02] C：变量与格式化输出
来源：http://xn.nicolike.cn

int a = 10; printf("%d\n", a);
来源：http://st.gzmigu.cn

[S03] C：读入整数
来源：http://sk.asd995.cn

int x; scanf("%d", &x);
来源：http://ql.newstarts.cn

[S04] C：字符串复制
来源：http://ra.huixiangedu.cn

char dst[32]; strcpy(dst, "hi");
来源：http://vg.shxzukj.cn

[S05] C：字符串长度
来源：http://em.hnjuh.cn

strlen(s)
来源：http://fx.bookmarksfly.cn

[S06] C：字符串比较
来源：http://cn.hnjuh.cn

strcmp(a, b) == 0
来源：http://it.bookmarksfly.cn

[S07] C：数组遍历求和
来源：http://kz.haigaiapp.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wv.newstarts.cn

[S08] C：动态内存分配与释放
来源：http://zx.newstarts.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://sa.hahajie.cn

[S09] C：结构体定义与初始化
来源：http://ix.yuntaijiaju.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://cz.lnxyls.cn

[S10] C：指针与解引用
来源：http://gk.shxzukj.cn

int *p = &a;  *p = 5;
来源：http://pk.jianghongdianzi.cn

[S11] C：逐行读文件
来源：http://kn.jctech888.com.cn

FILE *f = fopen("a.txt", "r");
来源：http://yw.huanxung.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://rv.hnjuh.cn

fclose(f);
来源：http://cl.huanxung.cn

[S12] C：写文件
来源：http://ec.nszjky.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://wi.shtwfgs.cn

[S13] C：宏定义
来源：http://ct.huanxung.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://xy.asd995.cn

[S14] C：枚举
来源：http://bx.gzmigu.cn

enum Color { RED, GREEN, BLUE };
来源：http://kk.muxihuayi.cn

[S15] C：类型转换
来源：http://rc.muxihuayi.cn

(double) a / b
来源：http://xv.huixiangedu.cn

[S16] C：位操作置位
来源：http://ws.nszjky.cn

x |= (1 << 3);
来源：http://vg.gzmigu.cn

[S17] C：安全拼接字符串
来源：http://fb.gzmigu.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://uv.szxytkj.cn

[S18] C：命令行参数
来源：http://tp.huixiangedu.cn

int main(int argc, char **argv)
来源：http://po.haigaiapp.cn

[S19] C：快速排序
来源：http://hr.jianghongdianzi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://xc.lnxyls.cn

[S20] C：二分查找
来源：http://gz.shtwfgs.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ll.bjjhwx.cn

[S21] C：字符类别判断
来源：http://yg.jianghongdianzi.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xo.521024.cn

[S22] C：字符串转数字
来源：http://sv.nicolike.cn

atoi("42");  strtod("3.14", NULL);
来源：http://xe.521024.cn

[S23] C：随机数
来源：http://zv.nszjky.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ym.szsharing.cn

[S24] C：获取本地时间
来源：http://ld.gzmigu.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://jl.newstarts.cn

[S25] C：内存拷贝
来源：http://uk.haigaiapp.cn

memcpy(dst, src, n);
来源：http://wg.haigaiapp.cn

[S26] C：内存清零
来源：http://oy.haigaiapp.cn

memset(a, 0, sizeof a);
来源：http://tj.szsharing.cn

[S27] C：定义常量
来源：http://wj.chemitech.net.cn

const double PI = 3.14159;
来源：http://tu.shtwfgs.cn

[S28] C：静态变量
来源：http://zd.newstarts.cn

static int counter = 0;
来源：http://ul.jianghongdianzi.cn

[S29] C：变参函数
来源：http://qk.szsharing.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://fr.haigaiapp.cn

[S30] C：头文件保护
来源：http://zg.shxzskj.cn

#ifndef X_H
来源：http://ue.gzmigu.cn

#define X_H
来源：http://np.shxzskj.cn

#endif
来源：http://qt.bookmarksfly.cn

[S31] C++：Hello World
来源：http://et.yuexingan06.cn

#include <iostream>
来源：http://zf.hnjuh.cn

int main() { std::cout << "Hello\n"; }
来源：http://yl.yuexingan06.cn

[S32] C++：字符串
来源：http://zz.shxzskj.cn

std::string s = "hi";  s += "!";
来源：http://vp.huixinmuqiang.cn

[S33] C++：vector 增删
来源：http://mb.szsharing.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://nf.szxytkj.cn

[S34] C++：遍历 vector
来源：http://sl.huixinmuqiang.cn

for (auto &x : v) { std::cout << x; }
来源：http://is.haigaiapp.cn

[S35] C++：map
来源：http://cm.bookmarksfly.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://gl.newstarts.cn

[S36] C++：unordered_map
来源：http://fp.huixiangedu.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ec.huixinmuqiang.cn

[S37] C++：set
来源：http://if.jianghongdianzi.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://oc.bookmarksfly.cn

[S38] C++：排序
来源：http://lb.521024.cn

std::sort(v.begin(), v.end());
来源：http://ff.shxzukj.cn

[S39] C++：自定义比较器排序
来源：http://ai.bjjhwx.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://nq.haigaiapp.cn

[S40] C++：查找元素
来源：http://yz.yuntaijiaju.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://tw.yuntaijiaju.cn

[S41] C++：类与构造函数
来源：http://wi.muxihuayi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://lv.szsharing.cn

[S42] C++：继承与虚函数
来源：http://tm.9csxet.cn

class B : public Base { public: void f() override {} };
来源：http://jn.szxytkj.cn

[S43] C++：智能指针
来源：http://tc.huixiangedu.cn

auto p = std::make_unique<int>(5);
来源：http://ks.asd995.cn

[S44] C++：引用传参
来源：http://rl.hahajie.cn

void inc(int &x) { ++x; }
来源：http://ix.gzmigu.cn

[S45] C++：lambda
来源：http://ta.asd995.cn

auto add = [](int a, int b) { return a + b; };
来源：http://hy.jianghongdianzi.cn

[S46] C++：函数模板
来源：http://ui.hnjuh.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ev.haigaiapp.cn

[S47] C++：结构化绑定遍历
来源：http://hr.huanxung.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://td.hnjuh.cn

[S48] C++：逐行读文件
来源：http://zz.bookmarksfly.cn

std::ifstream in("a.txt");  std::string line;
来源：http://am.bjjhwx.cn

while (std::getline(in, line)) { }
来源：http://jz.shtwfgs.cn

[S49] C++：写文件
来源：http://aa.bookmarksfly.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://wd.yuexingan06.cn

[S50] C++：格式化数字
来源：http://ki.9csxet.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://bz.lnxyls.cn

[S51] C++：显式类型转换
来源：http://nt.wgjwhj.cn

static_cast<double>(a) / b
来源：http://yq.bjjhwx.cn

[S52] C++：const 与 noexcept
来源：http://th.hnjuh.cn

int size() const noexcept { return n_; }
来源：http://th.huixinmuqiang.cn

[S53] C++：移动语义
来源：http://ui.bookmarksfly.cn

std::vector<int> w = std::move(v);
来源：http://sz.huixinmuqiang.cn

[S54] C++：异常处理
来源：http://ww.muxihuayi.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://dv.hahajie.cn

[S55] C++：结构化绑定
来源：http://nv.szxytkj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://zt.lnxyls.cn

[S56] C++：optional
来源：http://cv.bjjhwx.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://zv.yuntaijiaju.cn

[S57] C++：编译期常量
来源：http://lw.yuexingan06.cn

constexpr int N = 10;
来源：http://gx.wgjwhj.cn

[S58] C++：命名空间
来源：http://cs.shxzukj.cn

namespace ns { int f() { return 1; } }
来源：http://zj.wgjwhj.cn

[S59] C++：静态断言
来源：http://ra.521024.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ri.nicolike.cn

[S60] C++：遍历并删除元素
来源：http://fj.yuntaijiaju.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://it.asd995.cn

================================================================================
来源：http://jd.shtwfgs.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://pz.huixinmuqiang.cn

================================================================================
来源：http://te.hnjuh.cn

[T01] Kotlin：Hello World
来源：http://pk.hnjuh.cn

println("Hello")
来源：http://rr.newstarts.cn

[T02] Kotlin：变量
来源：http://iu.huanxung.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://vs.szxytkj.cn

[T03] Kotlin：字符串模板
来源：http://yl.nszjky.cn

"值: $b"
来源：http://kd.muxihuayi.cn

[T04] Kotlin：空安全
来源：http://pi.bjjhwx.cn

val n: String? = null;  n?.length
来源：http://ok.bookmarksfly.cn

[T05] Kotlin：when 表达式
来源：http://cu.huanxung.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://us.nszjky.cn

[T06] Kotlin：集合映射
来源：http://nm.haigaiapp.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://lz.huanxung.cn

[T07] Kotlin：集合过滤
来源：http://mi.shxzukj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ca.lnxyls.cn

[T08] Kotlin：数据类
来源：http://bv.yuexingan06.cn

data class User(val name: String, val age: Int)
来源：http://lu.bookmarksfly.cn

[T09] Kotlin：扩展函数
来源：http://uo.jctech888.com.cn

fun String.exclaim() = this + "!"
来源：http://hh.colortex.cn

[T10] Kotlin：默认参数
来源：http://ch.chemitech.net.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://gc.shxzukj.cn

[T11] Kotlin：协程
来源：http://ls.hahajie.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://fi.chemitech.net.cn

[T12] Kotlin：解构声明
来源：http://ip.lnxyls.cn

val (a, b) = Pair(1, 2)
来源：http://ej.wgjwhj.cn

[T13] Kotlin：只读 Map
来源：http://yp.jctech888.com.cn

val m = mapOf("a" to 1)
来源：http://il.shxzskj.cn

[T14] Kotlin：循环
来源：http://pk.panjiajie.cn

for (i in 1..10) println(i)
来源：http://xs.szsharing.cn

[T15] Kotlin：接口
来源：http://mr.newstarts.cn

interface Shape { fun area(): Double }
来源：http://wu.hnjuh.cn

[T16] Swift：Hello World
来源：http://tk.hnjuh.cn

print("Hello")
来源：http://yo.bookmarksfly.cn

[T17] Swift：变量与常量
来源：http://jh.asd995.cn

var a = 1;  let b = 2
来源：http://wr.haigaiapp.cn

[T18] Swift：字符串插值
来源：http://ll.nszjky.cn

"值: \(b)"
来源：http://bk.hahajie.cn

[T19] Swift：可选绑定
来源：http://xf.chemitech.net.cn

if let n = opt { print(n) }
来源：http://fn.szsharing.cn

[T20] Swift：数组操作
来源：http://vn.bookmarksfly.cn

var a = [1, 2, 3];  a.append(4)
来源：http://um.gzmigu.cn

[T21] Swift：遍历
来源：http://od.nicolike.cn

for x in a { print(x) }
来源：http://te.nszjky.cn

[T22] Swift：字典
来源：http://sv.shtwfgs.cn

var d = ["a": 1];  d["b"] = 2
来源：http://hl.yuexingan06.cn

[T23] Swift：函数
来源：http://qw.asd995.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ps.szsharing.cn

[T24] Swift：闭包
来源：http://jw.colortex.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://zk.colortex.cn

[T25] Swift：结构体
来源：http://ms.gzmigu.cn

struct P { var x: Int }
来源：http://gf.hahajie.cn

[T26] Swift：类与重写
来源：http://ns.haigaiapp.cn

class A: Base { override func f() {} }
来源：http://yn.wgjwhj.cn

[T27] Swift：错误处理
来源：http://tl.521024.cn

do { try f() } catch { print(error) }
来源：http://rj.chemitech.net.cn

[T28] Swift：枚举
来源：http://ex.nicolike.cn

enum Color { case red, green }
来源：http://vh.chemitech.net.cn

[T29] Swift：guard 提前返回
来源：http://nc.gzmigu.cn

guard let x = opt else { return }
来源：http://fy.shxzskj.cn

[T30] Swift：协议
来源：http://ld.bjjhwx.cn

protocol Shape { func area() -> Double }
来源：http://fh.shxzukj.cn

[T31] Lua：Hello World
来源：http://qo.muxihuayi.cn

print("Hello")
来源：http://he.asd995.cn

[T32] Lua：局部变量
来源：http://hj.gzmigu.cn

local a = 1
来源：http://zy.panjiajie.cn

[T33] Lua：表（数组）
来源：http://zb.gzmigu.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://iz.lnxyls.cn

[T34] Lua：遍历表
来源：http://ab.gzmigu.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://rn.gzmigu.cn

[T35] Lua：字典表
来源：http://wr.newstarts.cn

local d = { a = 1 };  d.b = 2
来源：http://zu.szsharing.cn

[T36] Lua：函数
来源：http://sd.jianghongdianzi.cn

function add(a, b) return a + b end
来源：http://lm.wgjwhj.cn

[T37] Lua：字符串拼接
来源：http://zh.szsharing.cn

"a" .. "b"
来源：http://vp.shxzukj.cn

[T38] Lua：条件
来源：http://vb.lnxyls.cn

if x > 0 then print("正") end
来源：http://gr.shxzskj.cn

[T39] Lua：模式匹配
来源：http://kn.nicolike.cn

string.find(s, "%d+")
来源：http://yv.huixiangedu.cn

[T40] Lua：元表
来源：http://fs.wgjwhj.cn

setmetatable({}, { __index = base })
来源：http://dz.shtwfgs.cn

[T41] Perl：Hello World
来源：http://kv.nicolike.cn

print "Hello\n";
来源：http://jj.szsharing.cn

[T42] Perl：变量类型
来源：http://kz.bookmarksfly.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://gd.yuntaijiaju.cn

[T43] Perl：字符串插值
来源：http://nq.muxihuayi.cn

"值: $a"
来源：http://av.9csxet.cn

[T44] Perl：条件
来源：http://gw.bjjhwx.cn

if ($a > 0) { print "正"; }
来源：http://kn.shxzukj.cn

[T45] Perl：数组遍历
来源：http://rc.yuexingan06.cn

for my $x (@arr) { print $x; }
来源：http://re.colortex.cn

[T46] Perl：哈希操作
来源：http://kx.szsharing.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ze.nszjky.cn

[T47] Perl：正则捕获
来源：http://kf.bjjhwx.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://sr.huanxung.cn

[T48] Perl：正则替换
来源：http://sa.521024.cn

$s =~ s/old/new/g;
来源：http://od.lnxyls.cn

[T49] Perl：函数
来源：http://uw.szsharing.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://on.hahajie.cn

[T50] Perl：逐行读文件
来源：http://kt.nicolike.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://xn.jianghongdianzi.cn

while (my $line = <$fh>) { print $line; }
来源：http://hd.jctech888.com.cn

[T51] Scala：Hello World
来源：http://oh.gzmigu.cn

println("Hello")
来源：http://jd.muxihuayi.cn

[T52] Scala：变量
来源：http://ey.chemitech.net.cn

val a = 1;  var b = 2
来源：http://rh.szxytkj.cn

[T53] Scala：字符串插值
来源：http://kl.newstarts.cn

s"值: $b"
来源：http://jz.shxzukj.cn

[T54] Scala：集合映射
来源：http://fs.yuexingan06.cn


<!-- 参考信息 -->