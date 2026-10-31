代发 wailian999

sort a.txt | uniq -c | sort -rn | head
来源：http://qz.yuexingan06.cn

[R52] 统计行数
来源：http://an.hnjuh.cn

wc -l a.txt
来源：http://tc.shxzskj.cn

[R53] 查看文件头与实时尾
来源：http://hf.colortex.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://rm.jianghongdianzi.cn

[R54] 比较两个文件
来源：http://sf.bjjhwx.cn

diff a.txt b.txt
来源：http://zc.shtwfgs.cn

[R55] 压缩与解压
来源：http://yk.nicolike.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://rt.nicolike.cn

[R56] 远程拷贝
来源：http://sj.huanxung.cn

scp file user@host:/path/
来源：http://go.bookmarksfly.cn

[R57] 远程执行命令
来源：http://sg.nszjky.cn

ssh user@host 'uptime'
来源：http://pj.hnjuh.cn

[R58] 下载文件
来源：http://ff.huixinmuqiang.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://bi.9csxet.cn

[R59] 发 POST JSON
来源：http://bc.bookmarksfly.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://nu.newstarts.cn

[R60] 只看 HTTP 状态码
来源：http://df.shxzukj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://xw.bookmarksfly.cn

[R61] 磁盘占用
来源：http://zl.hahajie.cn

df -h;  du -sh *
来源：http://mo.huixiangedu.cn

[R62] 找最占空间的文件
来源：http://cz.jianghongdianzi.cn

du -ah . | sort -rh | head -10
来源：http://oq.yuntaijiaju.cn

[R63] 内存与进程
来源：http://ki.hahajie.cn

free -h;  ps aux | grep nginx
来源：http://kt.lnxyls.cn

[R64] 结束进程
来源：http://mn.shxzukj.cn

kill -9 $(pgrep -f app.py)
来源：http://yv.asd995.cn

[R65] 查看端口占用
来源：http://la.colortex.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://mk.shxzukj.cn

[R66] 定时任务
来源：http://to.szsharing.cn

crontab -e;  crontab -l
来源：http://bt.hnjuh.cn

[R67] 生成随机十六进制串
来源：http://kr.asd995.cn

openssl rand -hex 16
来源：http://bn.asd995.cn

[R68] 计算文件校验值
来源：http://wt.szsharing.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ub.haigaiapp.cn

[R69] 生成随机密码
来源：http://zr.lnxyls.cn

head -c 16 /dev/urandom | base64
来源：http://se.wgjwhj.cn

[R70] 时间戳与互转
来源：http://wz.yuexingan06.cn

date +%s;  date -d @1700000000
来源：http://zj.wgjwhj.cn

[R71] 日期格式化
来源：http://mk.hahajie.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://tf.haigaiapp.cn

[R72] 等待端口就绪
来源：http://yo.shxzukj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://xs.panjiajie.cn

[R73] 分割大日志
来源：http://gw.huixinmuqiang.cn

split -l 1000 big.log part_
来源：http://gg.jctech888.com.cn

[R74] 批量重命名
来源：http://mm.szxytkj.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://kh.bookmarksfly.cn

[R75] 导出环境变量
来源：http://us.wgjwhj.cn

export PATH="$HOME/bin:$PATH"
来源：http://fd.jctech888.com.cn

[R76] 使用临时文件
来源：http://fv.9csxet.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ix.lnxyls.cn

[R77] 读取用户输入
来源：http://wi.haigaiapp.cn

read -rp "请输入: " ans
来源：http://na.huixinmuqiang.cn

[R78] 交互式菜单
来源：http://lx.chemitech.net.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://sy.gzmigu.cn

[R79] 解析命令行选项
来源：http://ld.yuexingan06.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://df.gzmigu.cn

[R80] 查看脚本执行耗时
来源：http://zt.gzmigu.cn

time ./run.sh
来源：http://jm.chemitech.net.cn

================================================================================
来源：http://zg.jctech888.com.cn

S. C / C++ 专题
来源：http://th.szsharing.cn

================================================================================
来源：http://bk.muxihuayi.cn

[S01] C：Hello World
来源：http://rx.bjjhwx.cn

#include <stdio.h>
来源：http://vz.521024.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://mw.chemitech.net.cn

[S02] C：变量与格式化输出
来源：http://zh.jctech888.com.cn

int a = 10; printf("%d\n", a);
来源：http://pr.newstarts.cn

[S03] C：读入整数
来源：http://wk.nszjky.cn

int x; scanf("%d", &x);
来源：http://kx.yuntaijiaju.cn

[S04] C：字符串复制
来源：http://iy.shxzskj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://mb.wgjwhj.cn

[S05] C：字符串长度
来源：http://jh.muxihuayi.cn

strlen(s)
来源：http://wh.wgjwhj.cn

[S06] C：字符串比较
来源：http://rc.bjjhwx.cn

strcmp(a, b) == 0
来源：http://ut.hnjuh.cn

[S07] C：数组遍历求和
来源：http://mq.yuntaijiaju.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ow.jianghongdianzi.cn

[S08] C：动态内存分配与释放
来源：http://ca.521024.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://lp.huixiangedu.cn

[S09] C：结构体定义与初始化
来源：http://ar.shxzukj.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://sd.muxihuayi.cn

[S10] C：指针与解引用
来源：http://jb.9csxet.cn

int *p = &a;  *p = 5;
来源：http://xv.nicolike.cn

[S11] C：逐行读文件
来源：http://ga.521024.cn

FILE *f = fopen("a.txt", "r");
来源：http://st.chemitech.net.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://mi.521024.cn

fclose(f);
来源：http://hq.jctech888.com.cn

[S12] C：写文件
来源：http://uc.chemitech.net.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://dm.bookmarksfly.cn

[S13] C：宏定义
来源：http://ye.shtwfgs.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ot.lnxyls.cn

[S14] C：枚举
来源：http://fj.huixinmuqiang.cn

enum Color { RED, GREEN, BLUE };
来源：http://dd.bookmarksfly.cn

[S15] C：类型转换
来源：http://nc.nicolike.cn

(double) a / b
来源：http://zk.huixinmuqiang.cn

[S16] C：位操作置位
来源：http://ry.muxihuayi.cn

x |= (1 << 3);
来源：http://nx.wgjwhj.cn

[S17] C：安全拼接字符串
来源：http://rz.colortex.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://sv.huanxung.cn

[S18] C：命令行参数
来源：http://dt.huixinmuqiang.cn

int main(int argc, char **argv)
来源：http://oy.hnjuh.cn

[S19] C：快速排序
来源：http://yg.shtwfgs.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ky.nicolike.cn

[S20] C：二分查找
来源：http://uc.bookmarksfly.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://jc.chemitech.net.cn

[S21] C：字符类别判断
来源：http://gw.gzmigu.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xc.szsharing.cn

[S22] C：字符串转数字
来源：http://jo.szxytkj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://px.yuexingan06.cn

[S23] C：随机数
来源：http://ug.haigaiapp.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://js.haigaiapp.cn

[S24] C：获取本地时间
来源：http://jy.shxzukj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://qt.haigaiapp.cn

[S25] C：内存拷贝
来源：http://tf.yuexingan06.cn

memcpy(dst, src, n);
来源：http://go.hnjuh.cn

[S26] C：内存清零
来源：http://ud.bookmarksfly.cn

memset(a, 0, sizeof a);
来源：http://vs.panjiajie.cn

[S27] C：定义常量
来源：http://xa.jianghongdianzi.cn

const double PI = 3.14159;
来源：http://lj.nszjky.cn

[S28] C：静态变量
来源：http://jo.nicolike.cn

static int counter = 0;
来源：http://ra.521024.cn

[S29] C：变参函数
来源：http://io.yuntaijiaju.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://al.huixiangedu.cn

[S30] C：头文件保护
来源：http://sv.521024.cn

#ifndef X_H
来源：http://bc.521024.cn

#define X_H
来源：http://ir.huixiangedu.cn

#endif
来源：http://mt.newstarts.cn

[S31] C++：Hello World
来源：http://sf.bjjhwx.cn

#include <iostream>
来源：http://lv.huanxung.cn

int main() { std::cout << "Hello\n"; }
来源：http://sq.shxzukj.cn

[S32] C++：字符串
来源：http://bi.huixinmuqiang.cn

std::string s = "hi";  s += "!";
来源：http://iv.jianghongdianzi.cn

[S33] C++：vector 增删
来源：http://sg.jctech888.com.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://eb.yuntaijiaju.cn

[S34] C++：遍历 vector
来源：http://au.hahajie.cn

for (auto &x : v) { std::cout << x; }
来源：http://fk.9csxet.cn

[S35] C++：map
来源：http://vd.huixinmuqiang.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://kt.shxzukj.cn

[S36] C++：unordered_map
来源：http://zn.yuntaijiaju.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://xp.yuexingan06.cn

[S37] C++：set
来源：http://qj.panjiajie.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://pr.gzmigu.cn

[S38] C++：排序
来源：http://ad.panjiajie.cn

std::sort(v.begin(), v.end());
来源：http://wd.haigaiapp.cn

[S39] C++：自定义比较器排序
来源：http://uy.gzmigu.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://pw.bjjhwx.cn

[S40] C++：查找元素
来源：http://ll.521024.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://tv.huixiangedu.cn

[S41] C++：类与构造函数
来源：http://fp.hnjuh.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://rp.hahajie.cn

[S42] C++：继承与虚函数
来源：http://nd.szxytkj.cn

class B : public Base { public: void f() override {} };
来源：http://ng.hahajie.cn

[S43] C++：智能指针
来源：http://ug.chemitech.net.cn

auto p = std::make_unique<int>(5);
来源：http://rs.szsharing.cn

[S44] C++：引用传参
来源：http://gg.yuexingan06.cn

void inc(int &x) { ++x; }
来源：http://jb.panjiajie.cn

[S45] C++：lambda
来源：http://cv.szxytkj.cn

auto add = [](int a, int b) { return a + b; };
来源：http://hg.lnxyls.cn

[S46] C++：函数模板
来源：http://np.jianghongdianzi.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://se.9csxet.cn

[S47] C++：结构化绑定遍历
来源：http://pj.nicolike.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://fl.yuntaijiaju.cn

[S48] C++：逐行读文件
来源：http://vo.huanxung.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ww.shxzukj.cn

while (std::getline(in, line)) { }
来源：http://ei.colortex.cn

[S49] C++：写文件
来源：http://iv.bjjhwx.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://qr.panjiajie.cn

[S50] C++：格式化数字
来源：http://ic.shxzskj.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://iu.asd995.cn

[S51] C++：显式类型转换
来源：http://kl.shxzskj.cn

static_cast<double>(a) / b
来源：http://od.szsharing.cn

[S52] C++：const 与 noexcept
来源：http://kh.asd995.cn

int size() const noexcept { return n_; }
来源：http://pk.muxihuayi.cn

[S53] C++：移动语义
来源：http://pj.newstarts.cn

std::vector<int> w = std::move(v);
来源：http://ma.yuntaijiaju.cn

[S54] C++：异常处理
来源：http://jd.shxzukj.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ov.shtwfgs.cn

[S55] C++：结构化绑定
来源：http://cg.hnjuh.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://eo.jctech888.com.cn

[S56] C++：optional
来源：http://ym.szxytkj.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://pk.hnjuh.cn

[S57] C++：编译期常量
来源：http://tm.yuntaijiaju.cn

constexpr int N = 10;
来源：http://qu.gzmigu.cn

[S58] C++：命名空间
来源：http://uc.521024.cn

namespace ns { int f() { return 1; } }
来源：http://jy.huixinmuqiang.cn

[S59] C++：静态断言
来源：http://vs.asd995.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://zm.shxzskj.cn

[S60] C++：遍历并删除元素
来源：http://jj.yuexingan06.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://rn.panjiajie.cn

================================================================================
来源：http://dp.jianghongdianzi.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://up.haigaiapp.cn

================================================================================
来源：http://pq.hahajie.cn

[T01] Kotlin：Hello World
来源：http://jr.9csxet.cn

println("Hello")
来源：http://gz.colortex.cn

[T02] Kotlin：变量
来源：http://uy.chemitech.net.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://vd.huixinmuqiang.cn

[T03] Kotlin：字符串模板
来源：http://ys.szxytkj.cn

"值: $b"
来源：http://bu.huanxung.cn

[T04] Kotlin：空安全
来源：http://nv.newstarts.cn

val n: String? = null;  n?.length
来源：http://ff.huixinmuqiang.cn

[T05] Kotlin：when 表达式
来源：http://ii.wgjwhj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://hn.huixiangedu.cn

[T06] Kotlin：集合映射
来源：http://kb.nszjky.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ns.jianghongdianzi.cn

[T07] Kotlin：集合过滤
来源：http://xd.bookmarksfly.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ig.chemitech.net.cn

[T08] Kotlin：数据类
来源：http://rj.yuexingan06.cn

data class User(val name: String, val age: Int)
来源：http://xm.newstarts.cn

[T09] Kotlin：扩展函数
来源：http://xr.haigaiapp.cn

fun String.exclaim() = this + "!"
来源：http://mi.jianghongdianzi.cn

[T10] Kotlin：默认参数
来源：http://wo.colortex.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://it.huixinmuqiang.cn

[T11] Kotlin：协程
来源：http://af.haigaiapp.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://hb.shtwfgs.cn

[T12] Kotlin：解构声明
来源：http://cy.gzmigu.cn

val (a, b) = Pair(1, 2)
来源：http://we.hnjuh.cn

[T13] Kotlin：只读 Map
来源：http://vl.huixiangedu.cn

val m = mapOf("a" to 1)
来源：http://va.shtwfgs.cn

[T14] Kotlin：循环
来源：http://ef.hnjuh.cn

for (i in 1..10) println(i)
来源：http://dd.huixinmuqiang.cn

[T15] Kotlin：接口
来源：http://je.chemitech.net.cn

interface Shape { fun area(): Double }
来源：http://wm.gzmigu.cn

[T16] Swift：Hello World
来源：http://dd.hahajie.cn

print("Hello")
来源：http://xr.shxzukj.cn

[T17] Swift：变量与常量
来源：http://tu.huanxung.cn

var a = 1;  let b = 2
来源：http://rz.hnjuh.cn

[T18] Swift：字符串插值
来源：http://bx.colortex.cn

"值: \(b)"
来源：http://va.hahajie.cn

[T19] Swift：可选绑定
来源：http://xz.bjjhwx.cn

if let n = opt { print(n) }
来源：http://fk.bjjhwx.cn

[T20] Swift：数组操作
来源：http://kv.huanxung.cn

var a = [1, 2, 3];  a.append(4)
来源：http://ez.huixiangedu.cn

[T21] Swift：遍历
来源：http://qf.newstarts.cn

for x in a { print(x) }
来源：http://in.bjjhwx.cn

[T22] Swift：字典
来源：http://ly.hahajie.cn

var d = ["a": 1];  d["b"] = 2
来源：http://fa.yuexingan06.cn

[T23] Swift：函数
来源：http://rw.newstarts.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://dk.szxytkj.cn

[T24] Swift：闭包
来源：http://rn.shtwfgs.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://bt.huixinmuqiang.cn

[T25] Swift：结构体
来源：http://mv.9csxet.cn

struct P { var x: Int }
来源：http://ai.huanxung.cn

[T26] Swift：类与重写
来源：http://do.asd995.cn

class A: Base { override func f() {} }
来源：http://jw.hahajie.cn

[T27] Swift：错误处理
来源：http://qo.jctech888.com.cn

do { try f() } catch { print(error) }
来源：http://pi.muxihuayi.cn

[T28] Swift：枚举
来源：http://nf.shtwfgs.cn

enum Color { case red, green }
来源：http://qa.szxytkj.cn

[T29] Swift：guard 提前返回
来源：http://ns.yuntaijiaju.cn

guard let x = opt else { return }
来源：http://yt.bjjhwx.cn

[T30] Swift：协议
来源：http://lg.huanxung.cn

protocol Shape { func area() -> Double }
来源：http://aq.gzmigu.cn

[T31] Lua：Hello World
来源：http://iu.521024.cn

print("Hello")
来源：http://al.szsharing.cn

[T32] Lua：局部变量
来源：http://by.shtwfgs.cn

local a = 1
来源：http://cx.muxihuayi.cn

[T33] Lua：表（数组）
来源：http://be.panjiajie.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://pa.jianghongdianzi.cn

[T34] Lua：遍历表
来源：http://xd.newstarts.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://jz.haigaiapp.cn

[T35] Lua：字典表
来源：http://po.jianghongdianzi.cn

local d = { a = 1 };  d.b = 2
来源：http://ui.shxzskj.cn

[T36] Lua：函数
来源：http://zy.muxihuayi.cn

function add(a, b) return a + b end
来源：http://dg.huanxung.cn

[T37] Lua：字符串拼接
来源：http://vp.asd995.cn

"a" .. "b"
来源：http://ha.huanxung.cn

[T38] Lua：条件
来源：http://wg.panjiajie.cn

if x > 0 then print("正") end
来源：http://qv.gzmigu.cn

[T39] Lua：模式匹配
来源：http://us.haigaiapp.cn

string.find(s, "%d+")
来源：http://gb.huixiangedu.cn

[T40] Lua：元表
来源：http://px.bjjhwx.cn

setmetatable({}, { __index = base })
来源：http://oe.lnxyls.cn

[T41] Perl：Hello World
来源：http://qv.szsharing.cn

print "Hello\n";
来源：http://ak.bookmarksfly.cn

[T42] Perl：变量类型
来源：http://hd.szsharing.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://rf.szsharing.cn

[T43] Perl：字符串插值
来源：http://qh.huixiangedu.cn

"值: $a"
来源：http://wy.szsharing.cn

[T44] Perl：条件
来源：http://qh.huanxung.cn

if ($a > 0) { print "正"; }
来源：http://gk.wgjwhj.cn

[T45] Perl：数组遍历
来源：http://ip.panjiajie.cn

for my $x (@arr) { print $x; }
来源：http://iy.huixiangedu.cn

[T46] Perl：哈希操作
来源：http://kp.9csxet.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://la.newstarts.cn

[T47] Perl：正则捕获
来源：http://vj.jctech888.com.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://wn.hahajie.cn

[T48] Perl：正则替换
来源：http://qi.shtwfgs.cn

$s =~ s/old/new/g;
来源：http://qr.panjiajie.cn

[T49] Perl：函数
来源：http://oq.newstarts.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://rm.huixinmuqiang.cn

[T50] Perl：逐行读文件
来源：http://jn.szsharing.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://vx.shxzskj.cn

while (my $line = <$fh>) { print $line; }
来源：http://so.shtwfgs.cn

[T51] Scala：Hello World
来源：http://cz.shxzskj.cn

println("Hello")
来源：http://zf.huanxung.cn

[T52] Scala：变量
来源：http://vs.9csxet.cn

val a = 1;  var b = 2
来源：http://dm.yuntaijiaju.cn

[T53] Scala：字符串插值
来源：http://hh.huanxung.cn

s"值: $b"
来源：http://rc.bookmarksfly.cn

[T54] Scala：集合映射
来源：http://nw.chemitech.net.cn


<!-- 参考信息 -->