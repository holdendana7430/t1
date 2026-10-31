代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：http://nd.huixiangedu.cn

[R48] awk 取指定列
来源：http://sl.wgjwhj.cn

awk '{print $1, $3}' a.txt
来源：http://wh.9csxet.cn

[R49] awk 带条件
来源：http://lv.colortex.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://it.bookmarksfly.cn

[R50] awk 求和
来源：http://rq.muxihuayi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://bt.nszjky.cn

[R51] 排序去重取前几
来源：http://yo.shxzskj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://to.gzmigu.cn

[R52] 统计行数
来源：http://uk.gzmigu.cn

wc -l a.txt
来源：http://oy.nicolike.cn

[R53] 查看文件头与实时尾
来源：http://lh.yuntaijiaju.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ai.yuexingan06.cn

[R54] 比较两个文件
来源：http://qa.colortex.cn

diff a.txt b.txt
来源：http://ia.lnxyls.cn

[R55] 压缩与解压
来源：http://ez.shxzukj.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://kd.yuntaijiaju.cn

[R56] 远程拷贝
来源：http://ic.521024.cn

scp file user@host:/path/
来源：http://kn.9csxet.cn

[R57] 远程执行命令
来源：http://yp.huixinmuqiang.cn

ssh user@host 'uptime'
来源：http://ll.9csxet.cn

[R58] 下载文件
来源：http://tq.jctech888.com.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://zt.bjjhwx.cn

[R59] 发 POST JSON
来源：http://bx.szxytkj.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://zq.yuexingan06.cn

[R60] 只看 HTTP 状态码
来源：http://vn.haigaiapp.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://vb.jctech888.com.cn

[R61] 磁盘占用
来源：http://al.asd995.cn

df -h;  du -sh *
来源：http://zw.huixiangedu.cn

[R62] 找最占空间的文件
来源：http://ap.nicolike.cn

du -ah . | sort -rh | head -10
来源：http://op.newstarts.cn

[R63] 内存与进程
来源：http://ys.gzmigu.cn

free -h;  ps aux | grep nginx
来源：http://ev.shtwfgs.cn

[R64] 结束进程
来源：http://ny.jianghongdianzi.cn

kill -9 $(pgrep -f app.py)
来源：http://hq.shxzukj.cn

[R65] 查看端口占用
来源：http://tr.nicolike.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://rp.gzmigu.cn

[R66] 定时任务
来源：http://gf.bjjhwx.cn

crontab -e;  crontab -l
来源：http://pd.shxzskj.cn

[R67] 生成随机十六进制串
来源：http://sk.huixinmuqiang.cn

openssl rand -hex 16
来源：http://pg.szxytkj.cn

[R68] 计算文件校验值
来源：http://rk.shxzukj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://mm.wgjwhj.cn

[R69] 生成随机密码
来源：http://kw.shxzskj.cn

head -c 16 /dev/urandom | base64
来源：http://da.yuexingan06.cn

[R70] 时间戳与互转
来源：http://yd.nicolike.cn

date +%s;  date -d @1700000000
来源：http://av.shxzukj.cn

[R71] 日期格式化
来源：http://rl.szxytkj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://dv.yuexingan06.cn

[R72] 等待端口就绪
来源：http://jx.9csxet.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://zh.shxzskj.cn

[R73] 分割大日志
来源：http://sp.bjjhwx.cn

split -l 1000 big.log part_
来源：http://gm.panjiajie.cn

[R74] 批量重命名
来源：http://ro.wgjwhj.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://pk.huanxung.cn

[R75] 导出环境变量
来源：http://ri.colortex.cn

export PATH="$HOME/bin:$PATH"
来源：http://mu.chemitech.net.cn

[R76] 使用临时文件
来源：http://pb.hahajie.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://tg.nszjky.cn

[R77] 读取用户输入
来源：http://ef.jianghongdianzi.cn

read -rp "请输入: " ans
来源：http://yp.szsharing.cn

[R78] 交互式菜单
来源：http://sv.nicolike.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://tt.bookmarksfly.cn

[R79] 解析命令行选项
来源：http://ul.huixiangedu.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://je.colortex.cn

[R80] 查看脚本执行耗时
来源：http://lz.jctech888.com.cn

time ./run.sh
来源：http://st.haigaiapp.cn

================================================================================
来源：http://ic.bookmarksfly.cn

S. C / C++ 专题
来源：http://yw.gzmigu.cn

================================================================================
来源：http://fd.9csxet.cn

[S01] C：Hello World
来源：http://pi.shxzukj.cn

#include <stdio.h>
来源：http://cn.nicolike.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://dw.wgjwhj.cn

[S02] C：变量与格式化输出
来源：http://id.jianghongdianzi.cn

int a = 10; printf("%d\n", a);
来源：http://te.yuexingan06.cn

[S03] C：读入整数
来源：http://vr.hnjuh.cn

int x; scanf("%d", &x);
来源：http://gn.shxzukj.cn

[S04] C：字符串复制
来源：http://vo.jctech888.com.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ll.chemitech.net.cn

[S05] C：字符串长度
来源：http://kt.shxzskj.cn

strlen(s)
来源：http://fd.gzmigu.cn

[S06] C：字符串比较
来源：http://ke.521024.cn

strcmp(a, b) == 0
来源：http://vh.lnxyls.cn

[S07] C：数组遍历求和
来源：http://sk.huixinmuqiang.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://mh.shxzukj.cn

[S08] C：动态内存分配与释放
来源：http://yd.lnxyls.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://oj.panjiajie.cn

[S09] C：结构体定义与初始化
来源：http://hb.bjjhwx.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://dw.shxzukj.cn

[S10] C：指针与解引用
来源：http://wn.521024.cn

int *p = &a;  *p = 5;
来源：http://si.jianghongdianzi.cn

[S11] C：逐行读文件
来源：http://mb.nszjky.cn

FILE *f = fopen("a.txt", "r");
来源：http://iy.bookmarksfly.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://vb.asd995.cn

fclose(f);
来源：http://mj.nszjky.cn

[S12] C：写文件
来源：http://al.jianghongdianzi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://kk.wgjwhj.cn

[S13] C：宏定义
来源：http://ke.bjjhwx.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://mw.jianghongdianzi.cn

[S14] C：枚举
来源：http://pd.521024.cn

enum Color { RED, GREEN, BLUE };
来源：http://dc.bookmarksfly.cn

[S15] C：类型转换
来源：http://cz.jctech888.com.cn

(double) a / b
来源：http://bw.yuexingan06.cn

[S16] C：位操作置位
来源：http://ld.panjiajie.cn

x |= (1 << 3);
来源：http://bl.shxzskj.cn

[S17] C：安全拼接字符串
来源：http://wb.hahajie.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://oq.asd995.cn

[S18] C：命令行参数
来源：http://xx.muxihuayi.cn

int main(int argc, char **argv)
来源：http://zv.wgjwhj.cn

[S19] C：快速排序
来源：http://dq.huixinmuqiang.cn

qsort(a, n, sizeof(int), cmp);
来源：http://lo.nszjky.cn

[S20] C：二分查找
来源：http://uq.yuexingan06.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://mo.szxytkj.cn

[S21] C：字符类别判断
来源：http://ax.yuexingan06.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://cx.hahajie.cn

[S22] C：字符串转数字
来源：http://zl.bjjhwx.cn

atoi("42");  strtod("3.14", NULL);
来源：http://qn.huixinmuqiang.cn

[S23] C：随机数
来源：http://si.szxytkj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ab.chemitech.net.cn

[S24] C：获取本地时间
来源：http://zf.521024.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://op.shtwfgs.cn

[S25] C：内存拷贝
来源：http://kj.huixinmuqiang.cn

memcpy(dst, src, n);
来源：http://eo.colortex.cn

[S26] C：内存清零
来源：http://se.yuexingan06.cn

memset(a, 0, sizeof a);
来源：http://ij.huixiangedu.cn

[S27] C：定义常量
来源：http://qp.huixinmuqiang.cn

const double PI = 3.14159;
来源：http://sx.haigaiapp.cn

[S28] C：静态变量
来源：http://um.haigaiapp.cn

static int counter = 0;
来源：http://go.szsharing.cn

[S29] C：变参函数
来源：http://fd.panjiajie.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ky.jianghongdianzi.cn

[S30] C：头文件保护
来源：http://vs.nicolike.cn

#ifndef X_H
来源：http://xm.jctech888.com.cn

#define X_H
来源：http://pq.szsharing.cn

#endif
来源：http://ip.hahajie.cn

[S31] C++：Hello World
来源：http://pk.hnjuh.cn

#include <iostream>
来源：http://so.panjiajie.cn

int main() { std::cout << "Hello\n"; }
来源：http://xz.huixiangedu.cn

[S32] C++：字符串
来源：http://qa.gzmigu.cn

std::string s = "hi";  s += "!";
来源：http://aa.yuntaijiaju.cn

[S33] C++：vector 增删
来源：http://th.bjjhwx.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://hp.colortex.cn

[S34] C++：遍历 vector
来源：http://qy.shxzukj.cn

for (auto &x : v) { std::cout << x; }
来源：http://oz.panjiajie.cn

[S35] C++：map
来源：http://zo.nicolike.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ip.huixiangedu.cn

[S36] C++：unordered_map
来源：http://wj.szsharing.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://em.huixinmuqiang.cn

[S37] C++：set
来源：http://nh.panjiajie.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://nx.chemitech.net.cn

[S38] C++：排序
来源：http://rv.yuntaijiaju.cn

std::sort(v.begin(), v.end());
来源：http://uc.asd995.cn

[S39] C++：自定义比较器排序
来源：http://nm.hahajie.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://jm.hahajie.cn

[S40] C++：查找元素
来源：http://bd.huixinmuqiang.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://jj.9csxet.cn

[S41] C++：类与构造函数
来源：http://fs.shxzskj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://xj.9csxet.cn

[S42] C++：继承与虚函数
来源：http://kb.huanxung.cn

class B : public Base { public: void f() override {} };
来源：http://oj.muxihuayi.cn

[S43] C++：智能指针
来源：http://gp.asd995.cn

auto p = std::make_unique<int>(5);
来源：http://fw.hahajie.cn

[S44] C++：引用传参
来源：http://my.chemitech.net.cn

void inc(int &x) { ++x; }
来源：http://wc.szsharing.cn

[S45] C++：lambda
来源：http://us.jianghongdianzi.cn

auto add = [](int a, int b) { return a + b; };
来源：http://uz.shxzukj.cn

[S46] C++：函数模板
来源：http://wn.nicolike.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://el.gzmigu.cn

[S47] C++：结构化绑定遍历
来源：http://wv.jianghongdianzi.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://lw.panjiajie.cn

[S48] C++：逐行读文件
来源：http://xk.bjjhwx.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ig.jianghongdianzi.cn

while (std::getline(in, line)) { }
来源：http://ja.szsharing.cn

[S49] C++：写文件
来源：http://nl.yuntaijiaju.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://fq.shxzukj.cn

[S50] C++：格式化数字
来源：http://rz.hnjuh.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://zd.nicolike.cn

[S51] C++：显式类型转换
来源：http://gg.jctech888.com.cn

static_cast<double>(a) / b
来源：http://po.chemitech.net.cn

[S52] C++：const 与 noexcept
来源：http://se.panjiajie.cn

int size() const noexcept { return n_; }
来源：http://qi.panjiajie.cn

[S53] C++：移动语义
来源：http://zc.gzmigu.cn

std::vector<int> w = std::move(v);
来源：http://dt.9csxet.cn

[S54] C++：异常处理
来源：http://op.9csxet.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://cl.colortex.cn

[S55] C++：结构化绑定
来源：http://vg.jctech888.com.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://lw.hahajie.cn

[S56] C++：optional
来源：http://kb.huixinmuqiang.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://qm.newstarts.cn

[S57] C++：编译期常量
来源：http://cp.haigaiapp.cn

constexpr int N = 10;
来源：http://ne.szxytkj.cn

[S58] C++：命名空间
来源：http://ux.colortex.cn

namespace ns { int f() { return 1; } }
来源：http://zl.521024.cn

[S59] C++：静态断言
来源：http://cz.panjiajie.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ne.huixiangedu.cn

[S60] C++：遍历并删除元素
来源：http://yj.shtwfgs.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://na.hnjuh.cn

================================================================================
来源：http://ql.shxzskj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://hw.huanxung.cn

================================================================================
来源：http://wd.huixiangedu.cn

[T01] Kotlin：Hello World
来源：http://ow.huanxung.cn

println("Hello")
来源：http://yf.szsharing.cn

[T02] Kotlin：变量
来源：http://xy.huanxung.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://tt.yuexingan06.cn

[T03] Kotlin：字符串模板
来源：http://fq.9csxet.cn

"值: $b"
来源：http://et.huixiangedu.cn

[T04] Kotlin：空安全
来源：http://ae.huixiangedu.cn

val n: String? = null;  n?.length
来源：http://mw.asd995.cn

[T05] Kotlin：when 表达式
来源：http://kt.szxytkj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://gk.huixiangedu.cn

[T06] Kotlin：集合映射
来源：http://qh.wgjwhj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://gj.haigaiapp.cn

[T07] Kotlin：集合过滤
来源：http://wv.wgjwhj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://zo.nszjky.cn

[T08] Kotlin：数据类
来源：http://oi.huanxung.cn

data class User(val name: String, val age: Int)
来源：http://eu.huanxung.cn

[T09] Kotlin：扩展函数
来源：http://ck.gzmigu.cn

fun String.exclaim() = this + "!"
来源：http://af.shtwfgs.cn

[T10] Kotlin：默认参数
来源：http://go.lnxyls.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://do.panjiajie.cn

[T11] Kotlin：协程
来源：http://gm.shxzskj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://la.yuntaijiaju.cn

[T12] Kotlin：解构声明
来源：http://sz.lnxyls.cn

val (a, b) = Pair(1, 2)
来源：http://zd.lnxyls.cn

[T13] Kotlin：只读 Map
来源：http://bb.asd995.cn

val m = mapOf("a" to 1)
来源：http://in.huanxung.cn

[T14] Kotlin：循环
来源：http://id.bjjhwx.cn

for (i in 1..10) println(i)
来源：http://km.shtwfgs.cn

[T15] Kotlin：接口
来源：http://lr.jctech888.com.cn

interface Shape { fun area(): Double }
来源：http://uc.nszjky.cn

[T16] Swift：Hello World
来源：http://gx.huixiangedu.cn

print("Hello")
来源：http://pv.hnjuh.cn

[T17] Swift：变量与常量
来源：http://yj.jianghongdianzi.cn

var a = 1;  let b = 2
来源：http://jq.jctech888.com.cn

[T18] Swift：字符串插值
来源：http://sx.shxzskj.cn

"值: \(b)"
来源：http://ee.jctech888.com.cn

[T19] Swift：可选绑定
来源：http://ci.huixiangedu.cn

if let n = opt { print(n) }
来源：http://og.nicolike.cn

[T20] Swift：数组操作
来源：http://za.lnxyls.cn

var a = [1, 2, 3];  a.append(4)
来源：http://jx.wgjwhj.cn

[T21] Swift：遍历
来源：http://pu.521024.cn

for x in a { print(x) }
来源：http://gb.haigaiapp.cn

[T22] Swift：字典
来源：http://mn.bookmarksfly.cn

var d = ["a": 1];  d["b"] = 2
来源：http://po.bookmarksfly.cn

[T23] Swift：函数
来源：http://cu.yuexingan06.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://xb.huanxung.cn

[T24] Swift：闭包
来源：http://cl.shxzskj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://vg.wgjwhj.cn

[T25] Swift：结构体
来源：http://os.newstarts.cn

struct P { var x: Int }
来源：http://ce.gzmigu.cn

[T26] Swift：类与重写
来源：http://cq.hahajie.cn

class A: Base { override func f() {} }
来源：http://fe.huixinmuqiang.cn

[T27] Swift：错误处理
来源：http://rb.huixiangedu.cn

do { try f() } catch { print(error) }
来源：http://oc.wgjwhj.cn

[T28] Swift：枚举
来源：http://cq.jianghongdianzi.cn

enum Color { case red, green }
来源：http://ge.newstarts.cn

[T29] Swift：guard 提前返回
来源：http://ck.shtwfgs.cn

guard let x = opt else { return }
来源：http://id.wgjwhj.cn

[T30] Swift：协议
来源：http://mb.panjiajie.cn

protocol Shape { func area() -> Double }
来源：http://yb.szsharing.cn

[T31] Lua：Hello World
来源：http://ob.huixinmuqiang.cn

print("Hello")
来源：http://qg.haigaiapp.cn

[T32] Lua：局部变量
来源：http://go.yuntaijiaju.cn

local a = 1
来源：http://nr.jianghongdianzi.cn

[T33] Lua：表（数组）
来源：http://kc.jctech888.com.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ws.bookmarksfly.cn

[T34] Lua：遍历表
来源：http://sa.muxihuayi.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://al.haigaiapp.cn

[T35] Lua：字典表
来源：http://ys.gzmigu.cn

local d = { a = 1 };  d.b = 2
来源：http://be.asd995.cn

[T36] Lua：函数
来源：http://nm.9csxet.cn

function add(a, b) return a + b end
来源：http://qu.colortex.cn

[T37] Lua：字符串拼接
来源：http://kp.szsharing.cn

"a" .. "b"
来源：http://zc.shtwfgs.cn

[T38] Lua：条件
来源：http://po.huixinmuqiang.cn

if x > 0 then print("正") end
来源：http://zh.colortex.cn

[T39] Lua：模式匹配
来源：http://bv.gzmigu.cn

string.find(s, "%d+")
来源：http://kx.muxihuayi.cn

[T40] Lua：元表
来源：http://ng.newstarts.cn

setmetatable({}, { __index = base })
来源：http://vg.szxytkj.cn

[T41] Perl：Hello World
来源：http://nw.gzmigu.cn

print "Hello\n";
来源：http://de.jianghongdianzi.cn

[T42] Perl：变量类型
来源：http://vj.huixiangedu.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://qs.colortex.cn

[T43] Perl：字符串插值
来源：http://ex.asd995.cn

"值: $a"
来源：http://id.huixiangedu.cn

[T44] Perl：条件
来源：http://wy.huixinmuqiang.cn

if ($a > 0) { print "正"; }
来源：http://ur.chemitech.net.cn

[T45] Perl：数组遍历
来源：http://cr.jctech888.com.cn

for my $x (@arr) { print $x; }
来源：http://wm.muxihuayi.cn

[T46] Perl：哈希操作
来源：http://ko.shxzukj.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://ec.wgjwhj.cn

[T47] Perl：正则捕获
来源：http://eo.521024.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://gk.bookmarksfly.cn

[T48] Perl：正则替换
来源：http://lm.521024.cn

$s =~ s/old/new/g;
来源：http://na.szxytkj.cn

[T49] Perl：函数
来源：http://cf.huixinmuqiang.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://jh.9csxet.cn

[T50] Perl：逐行读文件
来源：http://tf.lnxyls.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://sd.wgjwhj.cn


<!-- 参考信息 -->