代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：http://bg.bjjhwx.cn

[R48] awk 取指定列
来源：http://hg.shxzukj.cn

awk '{print $1, $3}' a.txt
来源：http://ov.nicolike.cn

[R49] awk 带条件
来源：http://rc.huixiangedu.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://pk.shxzskj.cn

[R50] awk 求和
来源：http://uu.9csxet.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ab.szxytkj.cn

[R51] 排序去重取前几
来源：http://wr.szxytkj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://ho.hahajie.cn

[R52] 统计行数
来源：http://pd.hnjuh.cn

wc -l a.txt
来源：http://pd.yuexingan06.cn

[R53] 查看文件头与实时尾
来源：http://tf.wgjwhj.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ls.shxzskj.cn

[R54] 比较两个文件
来源：http://qt.szxytkj.cn

diff a.txt b.txt
来源：http://zl.huixinmuqiang.cn

[R55] 压缩与解压
来源：http://hz.9csxet.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ww.wgjwhj.cn

[R56] 远程拷贝
来源：http://fg.yuexingan06.cn

scp file user@host:/path/
来源：http://gk.colortex.cn

[R57] 远程执行命令
来源：http://wh.yuntaijiaju.cn

ssh user@host 'uptime'
来源：http://qr.yuexingan06.cn

[R58] 下载文件
来源：http://qh.hnjuh.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://bq.asd995.cn

[R59] 发 POST JSON
来源：http://yb.haigaiapp.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://dm.bookmarksfly.cn

[R60] 只看 HTTP 状态码
来源：http://jb.521024.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://dq.szsharing.cn

[R61] 磁盘占用
来源：http://lm.asd995.cn

df -h;  du -sh *
来源：http://ya.gzmigu.cn

[R62] 找最占空间的文件
来源：http://ui.jianghongdianzi.cn

du -ah . | sort -rh | head -10
来源：http://vh.bookmarksfly.cn

[R63] 内存与进程
来源：http://wm.nicolike.cn

free -h;  ps aux | grep nginx
来源：http://oq.huixiangedu.cn

[R64] 结束进程
来源：http://qv.hnjuh.cn

kill -9 $(pgrep -f app.py)
来源：http://gf.colortex.cn

[R65] 查看端口占用
来源：http://fg.9csxet.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ue.gzmigu.cn

[R66] 定时任务
来源：http://ib.jctech888.com.cn

crontab -e;  crontab -l
来源：http://ny.yuexingan06.cn

[R67] 生成随机十六进制串
来源：http://zm.shtwfgs.cn

openssl rand -hex 16
来源：http://nd.9csxet.cn

[R68] 计算文件校验值
来源：http://ey.huixinmuqiang.cn

sha256sum a.txt;  md5sum a.txt
来源：http://qg.newstarts.cn

[R69] 生成随机密码
来源：http://wj.bjjhwx.cn

head -c 16 /dev/urandom | base64
来源：http://tt.yuexingan06.cn

[R70] 时间戳与互转
来源：http://or.hahajie.cn

date +%s;  date -d @1700000000
来源：http://ef.haigaiapp.cn

[R71] 日期格式化
来源：http://ka.newstarts.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://bp.huixiangedu.cn

[R72] 等待端口就绪
来源：http://mm.jianghongdianzi.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://gs.haigaiapp.cn

[R73] 分割大日志
来源：http://ro.jctech888.com.cn

split -l 1000 big.log part_
来源：http://gn.hahajie.cn

[R74] 批量重命名
来源：http://is.shxzskj.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://bg.wgjwhj.cn

[R75] 导出环境变量
来源：http://od.shxzukj.cn

export PATH="$HOME/bin:$PATH"
来源：http://za.asd995.cn

[R76] 使用临时文件
来源：http://cq.nszjky.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://mi.shxzskj.cn

[R77] 读取用户输入
来源：http://mn.huixinmuqiang.cn

read -rp "请输入: " ans
来源：http://em.panjiajie.cn

[R78] 交互式菜单
来源：http://iw.jctech888.com.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://nc.nszjky.cn

[R79] 解析命令行选项
来源：http://ma.shxzskj.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://lo.lnxyls.cn

[R80] 查看脚本执行耗时
来源：http://lt.huixiangedu.cn

time ./run.sh
来源：http://fz.szxytkj.cn

================================================================================
来源：http://gw.shxzskj.cn

S. C / C++ 专题
来源：http://vf.huixinmuqiang.cn

================================================================================
来源：http://ap.asd995.cn

[S01] C：Hello World
来源：http://mc.szsharing.cn

#include <stdio.h>
来源：http://rw.jianghongdianzi.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://zl.hnjuh.cn

[S02] C：变量与格式化输出
来源：http://ny.bjjhwx.cn

int a = 10; printf("%d\n", a);
来源：http://co.jctech888.com.cn

[S03] C：读入整数
来源：http://na.colortex.cn

int x; scanf("%d", &x);
来源：http://fr.wgjwhj.cn

[S04] C：字符串复制
来源：http://fj.nicolike.cn

char dst[32]; strcpy(dst, "hi");
来源：http://lt.hnjuh.cn

[S05] C：字符串长度
来源：http://cr.hahajie.cn

strlen(s)
来源：http://kf.szsharing.cn

[S06] C：字符串比较
来源：http://ie.bjjhwx.cn

strcmp(a, b) == 0
来源：http://vy.shtwfgs.cn

[S07] C：数组遍历求和
来源：http://hr.muxihuayi.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://sd.huanxung.cn

[S08] C：动态内存分配与释放
来源：http://md.hahajie.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://li.panjiajie.cn

[S09] C：结构体定义与初始化
来源：http://gm.newstarts.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://lj.muxihuayi.cn

[S10] C：指针与解引用
来源：http://oi.haigaiapp.cn

int *p = &a;  *p = 5;
来源：http://sr.hahajie.cn

[S11] C：逐行读文件
来源：http://pp.haigaiapp.cn

FILE *f = fopen("a.txt", "r");
来源：http://xk.bookmarksfly.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://kh.huixinmuqiang.cn

fclose(f);
来源：http://zm.jianghongdianzi.cn

[S12] C：写文件
来源：http://pp.panjiajie.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ti.asd995.cn

[S13] C：宏定义
来源：http://lw.bjjhwx.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jd.szxytkj.cn

[S14] C：枚举
来源：http://hu.shxzukj.cn

enum Color { RED, GREEN, BLUE };
来源：http://wl.bjjhwx.cn

[S15] C：类型转换
来源：http://dt.lnxyls.cn

(double) a / b
来源：http://qj.shxzukj.cn

[S16] C：位操作置位
来源：http://yo.yuntaijiaju.cn

x |= (1 << 3);
来源：http://qn.wgjwhj.cn

[S17] C：安全拼接字符串
来源：http://bk.jianghongdianzi.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://gm.hahajie.cn

[S18] C：命令行参数
来源：http://kt.hahajie.cn

int main(int argc, char **argv)
来源：http://jx.huixinmuqiang.cn

[S19] C：快速排序
来源：http://ba.nicolike.cn

qsort(a, n, sizeof(int), cmp);
来源：http://co.521024.cn

[S20] C：二分查找
来源：http://yw.szsharing.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://pg.haigaiapp.cn

[S21] C：字符类别判断
来源：http://nf.lnxyls.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://lr.nszjky.cn

[S22] C：字符串转数字
来源：http://uh.szxytkj.cn

atoi("42");  strtod("3.14", NULL);
来源：http://gz.newstarts.cn

[S23] C：随机数
来源：http://ul.lnxyls.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://lg.szsharing.cn

[S24] C：获取本地时间
来源：http://zf.hahajie.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://tn.szsharing.cn

[S25] C：内存拷贝
来源：http://ce.szsharing.cn

memcpy(dst, src, n);
来源：http://sy.9csxet.cn

[S26] C：内存清零
来源：http://kg.panjiajie.cn

memset(a, 0, sizeof a);
来源：http://bb.huixinmuqiang.cn

[S27] C：定义常量
来源：http://hn.muxihuayi.cn

const double PI = 3.14159;
来源：http://ey.shtwfgs.cn

[S28] C：静态变量
来源：http://em.hnjuh.cn

static int counter = 0;
来源：http://we.bookmarksfly.cn

[S29] C：变参函数
来源：http://xj.shxzukj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://io.szsharing.cn

[S30] C：头文件保护
来源：http://en.huixiangedu.cn

#ifndef X_H
来源：http://rl.yuntaijiaju.cn

#define X_H
来源：http://jb.chemitech.net.cn

#endif
来源：http://bk.gzmigu.cn

[S31] C++：Hello World
来源：http://ul.nicolike.cn

#include <iostream>
来源：http://xc.jianghongdianzi.cn

int main() { std::cout << "Hello\n"; }
来源：http://nz.chemitech.net.cn

[S32] C++：字符串
来源：http://iu.bjjhwx.cn

std::string s = "hi";  s += "!";
来源：http://yu.panjiajie.cn

[S33] C++：vector 增删
来源：http://zk.hahajie.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://tb.9csxet.cn

[S34] C++：遍历 vector
来源：http://ow.wgjwhj.cn

for (auto &x : v) { std::cout << x; }
来源：http://cw.haigaiapp.cn

[S35] C++：map
来源：http://yp.chemitech.net.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://fr.asd995.cn

[S36] C++：unordered_map
来源：http://ol.colortex.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://pp.nicolike.cn

[S37] C++：set
来源：http://or.gzmigu.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://fy.bjjhwx.cn

[S38] C++：排序
来源：http://lh.szsharing.cn

std::sort(v.begin(), v.end());
来源：http://an.huixiangedu.cn

[S39] C++：自定义比较器排序
来源：http://sf.gzmigu.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://qc.muxihuayi.cn

[S40] C++：查找元素
来源：http://qi.asd995.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://bm.shxzskj.cn

[S41] C++：类与构造函数
来源：http://qo.521024.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://cl.bjjhwx.cn

[S42] C++：继承与虚函数
来源：http://xu.yuexingan06.cn

class B : public Base { public: void f() override {} };
来源：http://gf.gzmigu.cn

[S43] C++：智能指针
来源：http://qp.hnjuh.cn

auto p = std::make_unique<int>(5);
来源：http://zh.gzmigu.cn

[S44] C++：引用传参
来源：http://jv.hnjuh.cn

void inc(int &x) { ++x; }
来源：http://hd.hahajie.cn

[S45] C++：lambda
来源：http://ng.asd995.cn

auto add = [](int a, int b) { return a + b; };
来源：http://xh.hahajie.cn

[S46] C++：函数模板
来源：http://wu.hnjuh.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://kb.lnxyls.cn

[S47] C++：结构化绑定遍历
来源：http://cp.hahajie.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ys.szxytkj.cn

[S48] C++：逐行读文件
来源：http://ls.lnxyls.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ub.huanxung.cn

while (std::getline(in, line)) { }
来源：http://tq.asd995.cn

[S49] C++：写文件
来源：http://sf.muxihuayi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://tb.bookmarksfly.cn

[S50] C++：格式化数字
来源：http://vw.szsharing.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ur.jianghongdianzi.cn

[S51] C++：显式类型转换
来源：http://nj.jianghongdianzi.cn

static_cast<double>(a) / b
来源：http://wb.colortex.cn

[S52] C++：const 与 noexcept
来源：http://vt.huixiangedu.cn

int size() const noexcept { return n_; }
来源：http://oi.hnjuh.cn

[S53] C++：移动语义
来源：http://mb.gzmigu.cn

std::vector<int> w = std::move(v);
来源：http://oy.hnjuh.cn

[S54] C++：异常处理
来源：http://do.gzmigu.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://gq.yuexingan06.cn

[S55] C++：结构化绑定
来源：http://vy.wgjwhj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://sv.bookmarksfly.cn

[S56] C++：optional
来源：http://kl.jianghongdianzi.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://xy.shxzukj.cn

[S57] C++：编译期常量
来源：http://zk.colortex.cn

constexpr int N = 10;
来源：http://qt.huixinmuqiang.cn

[S58] C++：命名空间
来源：http://jw.panjiajie.cn

namespace ns { int f() { return 1; } }
来源：http://lc.huanxung.cn

[S59] C++：静态断言
来源：http://fu.hahajie.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hl.huixiangedu.cn

[S60] C++：遍历并删除元素
来源：http://oy.huixiangedu.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://pd.yuexingan06.cn

================================================================================
来源：http://ns.huixiangedu.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://gb.panjiajie.cn

================================================================================
来源：http://ux.gzmigu.cn

[T01] Kotlin：Hello World
来源：http://yn.panjiajie.cn

println("Hello")
来源：http://cd.nszjky.cn

[T02] Kotlin：变量
来源：http://gj.huanxung.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://nc.521024.cn

[T03] Kotlin：字符串模板
来源：http://xu.asd995.cn

"值: $b"
来源：http://og.shxzukj.cn

[T04] Kotlin：空安全
来源：http://pv.shtwfgs.cn

val n: String? = null;  n?.length
来源：http://ju.haigaiapp.cn

[T05] Kotlin：when 表达式
来源：http://bw.wgjwhj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://qb.9csxet.cn

[T06] Kotlin：集合映射
来源：http://sq.huanxung.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://vc.bookmarksfly.cn

[T07] Kotlin：集合过滤
来源：http://xb.szxytkj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://pf.bjjhwx.cn

[T08] Kotlin：数据类
来源：http://rg.chemitech.net.cn

data class User(val name: String, val age: Int)
来源：http://ua.muxihuayi.cn

[T09] Kotlin：扩展函数
来源：http://xr.colortex.cn

fun String.exclaim() = this + "!"
来源：http://wj.wgjwhj.cn

[T10] Kotlin：默认参数
来源：http://mq.shxzskj.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ot.jctech888.com.cn

[T11] Kotlin：协程
来源：http://yf.nszjky.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ra.hnjuh.cn

[T12] Kotlin：解构声明
来源：http://go.szxytkj.cn

val (a, b) = Pair(1, 2)
来源：http://mw.bjjhwx.cn

[T13] Kotlin：只读 Map
来源：http://em.hahajie.cn

val m = mapOf("a" to 1)
来源：http://dw.9csxet.cn

[T14] Kotlin：循环
来源：http://wr.521024.cn

for (i in 1..10) println(i)
来源：http://jq.bookmarksfly.cn

[T15] Kotlin：接口
来源：http://pq.bjjhwx.cn

interface Shape { fun area(): Double }
来源：http://eb.szxytkj.cn

[T16] Swift：Hello World
来源：http://kg.huixinmuqiang.cn

print("Hello")
来源：http://py.nszjky.cn

[T17] Swift：变量与常量
来源：http://bd.huixinmuqiang.cn

var a = 1;  let b = 2
来源：http://hd.jianghongdianzi.cn

[T18] Swift：字符串插值
来源：http://og.huixiangedu.cn

"值: \(b)"
来源：http://rh.521024.cn

[T19] Swift：可选绑定
来源：http://nt.huixiangedu.cn

if let n = opt { print(n) }
来源：http://ul.jctech888.com.cn

[T20] Swift：数组操作
来源：http://ke.panjiajie.cn

var a = [1, 2, 3];  a.append(4)
来源：http://un.lnxyls.cn

[T21] Swift：遍历
来源：http://zs.chemitech.net.cn

for x in a { print(x) }
来源：http://eg.shtwfgs.cn

[T22] Swift：字典
来源：http://ut.bjjhwx.cn

var d = ["a": 1];  d["b"] = 2
来源：http://wc.asd995.cn

[T23] Swift：函数
来源：http://it.9csxet.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://vb.szsharing.cn

[T24] Swift：闭包
来源：http://zt.shxzukj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://yn.szxytkj.cn

[T25] Swift：结构体
来源：http://lw.panjiajie.cn

struct P { var x: Int }
来源：http://bc.haigaiapp.cn

[T26] Swift：类与重写
来源：http://oe.huixinmuqiang.cn

class A: Base { override func f() {} }
来源：http://ei.jianghongdianzi.cn

[T27] Swift：错误处理
来源：http://yb.shxzukj.cn

do { try f() } catch { print(error) }
来源：http://br.jctech888.com.cn

[T28] Swift：枚举
来源：http://rn.bjjhwx.cn

enum Color { case red, green }
来源：http://zt.jctech888.com.cn

[T29] Swift：guard 提前返回
来源：http://wp.shxzukj.cn

guard let x = opt else { return }
来源：http://ox.asd995.cn

[T30] Swift：协议
来源：http://ma.huanxung.cn

protocol Shape { func area() -> Double }
来源：http://rg.yuexingan06.cn

[T31] Lua：Hello World
来源：http://xt.hahajie.cn

print("Hello")
来源：http://sh.jianghongdianzi.cn

[T32] Lua：局部变量
来源：http://yd.huixiangedu.cn

local a = 1
来源：http://sy.shxzukj.cn

[T33] Lua：表（数组）
来源：http://md.gzmigu.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://dk.9csxet.cn

[T34] Lua：遍历表
来源：http://fh.nszjky.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://fv.colortex.cn

[T35] Lua：字典表
来源：http://ei.szxytkj.cn

local d = { a = 1 };  d.b = 2
来源：http://xk.nszjky.cn

[T36] Lua：函数
来源：http://zd.huanxung.cn

function add(a, b) return a + b end
来源：http://rg.9csxet.cn

[T37] Lua：字符串拼接
来源：http://gb.panjiajie.cn

"a" .. "b"
来源：http://iw.bookmarksfly.cn

[T38] Lua：条件
来源：http://tw.hahajie.cn

if x > 0 then print("正") end
来源：http://aa.lnxyls.cn

[T39] Lua：模式匹配
来源：http://fo.shtwfgs.cn

string.find(s, "%d+")
来源：http://cv.shxzskj.cn

[T40] Lua：元表
来源：http://ge.colortex.cn

setmetatable({}, { __index = base })
来源：http://rp.gzmigu.cn

[T41] Perl：Hello World
来源：http://bz.muxihuayi.cn

print "Hello\n";
来源：http://zv.hahajie.cn

[T42] Perl：变量类型
来源：http://rf.wgjwhj.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://bo.shxzskj.cn

[T43] Perl：字符串插值
来源：http://rn.yuexingan06.cn

"值: $a"
来源：http://ff.muxihuayi.cn

[T44] Perl：条件
来源：http://it.wgjwhj.cn

if ($a > 0) { print "正"; }
来源：http://xi.lnxyls.cn

[T45] Perl：数组遍历
来源：http://ya.jctech888.com.cn

for my $x (@arr) { print $x; }
来源：http://ut.shxzukj.cn

[T46] Perl：哈希操作
来源：http://vv.hahajie.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://zv.bookmarksfly.cn

[T47] Perl：正则捕获
来源：http://wx.yuntaijiaju.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://aj.huanxung.cn

[T48] Perl：正则替换
来源：http://tv.szxytkj.cn

$s =~ s/old/new/g;
来源：http://uw.shxzskj.cn

[T49] Perl：函数
来源：http://wx.jianghongdianzi.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://xr.hnjuh.cn

[T50] Perl：逐行读文件
来源：http://nv.bjjhwx.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://oi.yuexingan06.cn


<!-- 参考信息 -->