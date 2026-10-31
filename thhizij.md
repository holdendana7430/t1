代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：http://wm.shxzukj.cn

[R48] awk 取指定列
来源：http://po.bookmarksfly.cn

awk '{print $1, $3}' a.txt
来源：http://fg.szsharing.cn

[R49] awk 带条件
来源：http://ob.panjiajie.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ds.wgjwhj.cn

[R50] awk 求和
来源：http://pe.nszjky.cn

awk '{s += $2} END {print s}' a.txt
来源：http://nw.huanxung.cn

[R51] 排序去重取前几
来源：http://bf.shtwfgs.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://sn.jianghongdianzi.cn

[R52] 统计行数
来源：http://hw.chemitech.net.cn

wc -l a.txt
来源：http://pu.chemitech.net.cn

[R53] 查看文件头与实时尾
来源：http://yh.huixiangedu.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ac.jctech888.com.cn

[R54] 比较两个文件
来源：http://fz.521024.cn

diff a.txt b.txt
来源：http://xm.jianghongdianzi.cn

[R55] 压缩与解压
来源：http://so.yuexingan06.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mo.lnxyls.cn

[R56] 远程拷贝
来源：http://fu.bookmarksfly.cn

scp file user@host:/path/
来源：http://sy.shtwfgs.cn

[R57] 远程执行命令
来源：http://zf.newstarts.cn

ssh user@host 'uptime'
来源：http://pd.shxzukj.cn

[R58] 下载文件
来源：http://ns.521024.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://xh.chemitech.net.cn

[R59] 发 POST JSON
来源：http://mu.asd995.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://kg.nicolike.cn

[R60] 只看 HTTP 状态码
来源：http://dq.jctech888.com.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://yw.wgjwhj.cn

[R61] 磁盘占用
来源：http://hy.colortex.cn

df -h;  du -sh *
来源：http://bg.hnjuh.cn

[R62] 找最占空间的文件
来源：http://iq.huixiangedu.cn

du -ah . | sort -rh | head -10
来源：http://zp.colortex.cn

[R63] 内存与进程
来源：http://it.chemitech.net.cn

free -h;  ps aux | grep nginx
来源：http://ts.haigaiapp.cn

[R64] 结束进程
来源：http://aj.hahajie.cn

kill -9 $(pgrep -f app.py)
来源：http://qn.521024.cn

[R65] 查看端口占用
来源：http://vi.nszjky.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://ay.shtwfgs.cn

[R66] 定时任务
来源：http://xc.asd995.cn

crontab -e;  crontab -l
来源：http://hn.asd995.cn

[R67] 生成随机十六进制串
来源：http://df.asd995.cn

openssl rand -hex 16
来源：http://gt.szsharing.cn

[R68] 计算文件校验值
来源：http://fq.panjiajie.cn

sha256sum a.txt;  md5sum a.txt
来源：http://gk.colortex.cn

[R69] 生成随机密码
来源：http://at.huixinmuqiang.cn

head -c 16 /dev/urandom | base64
来源：http://cs.muxihuayi.cn

[R70] 时间戳与互转
来源：http://pr.521024.cn

date +%s;  date -d @1700000000
来源：http://sx.newstarts.cn

[R71] 日期格式化
来源：http://za.9csxet.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://md.521024.cn

[R72] 等待端口就绪
来源：http://ku.jianghongdianzi.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://xo.nszjky.cn

[R73] 分割大日志
来源：http://yz.bjjhwx.cn

split -l 1000 big.log part_
来源：http://yg.szxytkj.cn

[R74] 批量重命名
来源：http://bc.nicolike.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://hl.panjiajie.cn

[R75] 导出环境变量
来源：http://nh.9csxet.cn

export PATH="$HOME/bin:$PATH"
来源：http://yy.521024.cn

[R76] 使用临时文件
来源：http://oi.asd995.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://bd.shxzukj.cn

[R77] 读取用户输入
来源：http://ru.panjiajie.cn

read -rp "请输入: " ans
来源：http://hy.muxihuayi.cn

[R78] 交互式菜单
来源：http://nx.bookmarksfly.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://la.yuexingan06.cn

[R79] 解析命令行选项
来源：http://tn.yuntaijiaju.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://nu.shxzukj.cn

[R80] 查看脚本执行耗时
来源：http://if.yuexingan06.cn

time ./run.sh
来源：http://mi.jctech888.com.cn

================================================================================
来源：http://wn.521024.cn

S. C / C++ 专题
来源：http://jz.panjiajie.cn

================================================================================
来源：http://tw.nicolike.cn

[S01] C：Hello World
来源：http://qf.newstarts.cn

#include <stdio.h>
来源：http://fp.huixiangedu.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://pc.jianghongdianzi.cn

[S02] C：变量与格式化输出
来源：http://kh.huixiangedu.cn

int a = 10; printf("%d\n", a);
来源：http://jj.newstarts.cn

[S03] C：读入整数
来源：http://ge.jianghongdianzi.cn

int x; scanf("%d", &x);
来源：http://nc.9csxet.cn

[S04] C：字符串复制
来源：http://fs.szxytkj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://et.asd995.cn

[S05] C：字符串长度
来源：http://bn.huixinmuqiang.cn

strlen(s)
来源：http://cb.bookmarksfly.cn

[S06] C：字符串比较
来源：http://ve.jctech888.com.cn

strcmp(a, b) == 0
来源：http://ve.shxzukj.cn

[S07] C：数组遍历求和
来源：http://sg.bjjhwx.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://al.hnjuh.cn

[S08] C：动态内存分配与释放
来源：http://ok.szxytkj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://pq.chemitech.net.cn

[S09] C：结构体定义与初始化
来源：http://by.yuntaijiaju.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://fl.wgjwhj.cn

[S10] C：指针与解引用
来源：http://ue.hahajie.cn

int *p = &a;  *p = 5;
来源：http://rg.newstarts.cn

[S11] C：逐行读文件
来源：http://ro.yuntaijiaju.cn

FILE *f = fopen("a.txt", "r");
来源：http://ik.huixinmuqiang.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://vi.shxzukj.cn

fclose(f);
来源：http://ha.newstarts.cn

[S12] C：写文件
来源：http://fe.jianghongdianzi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://vy.haigaiapp.cn

[S13] C：宏定义
来源：http://oi.haigaiapp.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://vf.jctech888.com.cn

[S14] C：枚举
来源：http://to.bjjhwx.cn

enum Color { RED, GREEN, BLUE };
来源：http://vo.huanxung.cn

[S15] C：类型转换
来源：http://oe.colortex.cn

(double) a / b
来源：http://mt.9csxet.cn

[S16] C：位操作置位
来源：http://ps.colortex.cn

x |= (1 << 3);
来源：http://xk.asd995.cn

[S17] C：安全拼接字符串
来源：http://ue.bookmarksfly.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://iq.bookmarksfly.cn

[S18] C：命令行参数
来源：http://ol.panjiajie.cn

int main(int argc, char **argv)
来源：http://xh.hahajie.cn

[S19] C：快速排序
来源：http://zp.yuntaijiaju.cn

qsort(a, n, sizeof(int), cmp);
来源：http://zp.bookmarksfly.cn

[S20] C：二分查找
来源：http://rd.yuexingan06.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wm.hnjuh.cn

[S21] C：字符类别判断
来源：http://jb.nicolike.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://hk.szsharing.cn

[S22] C：字符串转数字
来源：http://qh.nicolike.cn

atoi("42");  strtod("3.14", NULL);
来源：http://hl.shxzukj.cn

[S23] C：随机数
来源：http://fq.bjjhwx.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ga.muxihuayi.cn

[S24] C：获取本地时间
来源：http://rp.colortex.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://vx.szxytkj.cn

[S25] C：内存拷贝
来源：http://wl.shxzskj.cn

memcpy(dst, src, n);
来源：http://ni.huixinmuqiang.cn

[S26] C：内存清零
来源：http://we.nicolike.cn

memset(a, 0, sizeof a);
来源：http://sj.yuexingan06.cn

[S27] C：定义常量
来源：http://rw.newstarts.cn

const double PI = 3.14159;
来源：http://vz.shxzskj.cn

[S28] C：静态变量
来源：http://tz.panjiajie.cn

static int counter = 0;
来源：http://fb.wgjwhj.cn

[S29] C：变参函数
来源：http://ue.bookmarksfly.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mx.nszjky.cn

[S30] C：头文件保护
来源：http://uq.nicolike.cn

#ifndef X_H
来源：http://ux.shxzukj.cn

#define X_H
来源：http://mf.yuntaijiaju.cn

#endif
来源：http://ig.muxihuayi.cn

[S31] C++：Hello World
来源：http://lf.gzmigu.cn

#include <iostream>
来源：http://np.bjjhwx.cn

int main() { std::cout << "Hello\n"; }
来源：http://yt.shxzskj.cn

[S32] C++：字符串
来源：http://iq.yuexingan06.cn

std::string s = "hi";  s += "!";
来源：http://aj.hahajie.cn

[S33] C++：vector 增删
来源：http://qs.yuntaijiaju.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://od.gzmigu.cn

[S34] C++：遍历 vector
来源：http://my.chemitech.net.cn

for (auto &x : v) { std::cout << x; }
来源：http://gl.wgjwhj.cn

[S35] C++：map
来源：http://ig.bookmarksfly.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://pv.colortex.cn

[S36] C++：unordered_map
来源：http://jc.shtwfgs.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://sx.521024.cn

[S37] C++：set
来源：http://gl.jctech888.com.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://os.chemitech.net.cn

[S38] C++：排序
来源：http://oe.szsharing.cn

std::sort(v.begin(), v.end());
来源：http://uk.yuexingan06.cn

[S39] C++：自定义比较器排序
来源：http://zb.9csxet.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ju.gzmigu.cn

[S40] C++：查找元素
来源：http://uc.shxzskj.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ma.nszjky.cn

[S41] C++：类与构造函数
来源：http://so.9csxet.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ur.shxzukj.cn

[S42] C++：继承与虚函数
来源：http://as.9csxet.cn

class B : public Base { public: void f() override {} };
来源：http://zs.chemitech.net.cn

[S43] C++：智能指针
来源：http://lw.hahajie.cn

auto p = std::make_unique<int>(5);
来源：http://lp.panjiajie.cn

[S44] C++：引用传参
来源：http://qp.szsharing.cn

void inc(int &x) { ++x; }
来源：http://xf.yuexingan06.cn

[S45] C++：lambda
来源：http://ut.muxihuayi.cn

auto add = [](int a, int b) { return a + b; };
来源：http://vp.panjiajie.cn

[S46] C++：函数模板
来源：http://oo.haigaiapp.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://gx.hnjuh.cn

[S47] C++：结构化绑定遍历
来源：http://qf.newstarts.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://ez.521024.cn

[S48] C++：逐行读文件
来源：http://cz.lnxyls.cn

std::ifstream in("a.txt");  std::string line;
来源：http://kv.lnxyls.cn

while (std::getline(in, line)) { }
来源：http://qn.huixiangedu.cn

[S49] C++：写文件
来源：http://yo.huixinmuqiang.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hy.asd995.cn

[S50] C++：格式化数字
来源：http://tb.lnxyls.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://iy.szxytkj.cn

[S51] C++：显式类型转换
来源：http://xr.shxzukj.cn

static_cast<double>(a) / b
来源：http://ye.chemitech.net.cn

[S52] C++：const 与 noexcept
来源：http://lk.muxihuayi.cn

int size() const noexcept { return n_; }
来源：http://zh.asd995.cn

[S53] C++：移动语义
来源：http://ia.jctech888.com.cn

std::vector<int> w = std::move(v);
来源：http://gb.shxzskj.cn

[S54] C++：异常处理
来源：http://vj.521024.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://sz.521024.cn

[S55] C++：结构化绑定
来源：http://ze.shxzukj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://kr.shtwfgs.cn

[S56] C++：optional
来源：http://nn.yuntaijiaju.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mt.chemitech.net.cn

[S57] C++：编译期常量
来源：http://bl.jctech888.com.cn

constexpr int N = 10;
来源：http://fu.huixinmuqiang.cn

[S58] C++：命名空间
来源：http://ix.gzmigu.cn

namespace ns { int f() { return 1; } }
来源：http://iv.panjiajie.cn

[S59] C++：静态断言
来源：http://gh.bookmarksfly.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ra.huixinmuqiang.cn

[S60] C++：遍历并删除元素
来源：http://ic.nszjky.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://lk.bookmarksfly.cn

================================================================================
来源：http://nn.bookmarksfly.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://qk.huixiangedu.cn

================================================================================
来源：http://jh.haigaiapp.cn

[T01] Kotlin：Hello World
来源：http://bv.muxihuayi.cn

println("Hello")
来源：http://qq.lnxyls.cn

[T02] Kotlin：变量
来源：http://rh.huixinmuqiang.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ma.colortex.cn

[T03] Kotlin：字符串模板
来源：http://tl.chemitech.net.cn

"值: $b"
来源：http://xu.shtwfgs.cn

[T04] Kotlin：空安全
来源：http://cd.huixinmuqiang.cn

val n: String? = null;  n?.length
来源：http://cj.muxihuayi.cn

[T05] Kotlin：when 表达式
来源：http://wz.jianghongdianzi.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://sj.szxytkj.cn

[T06] Kotlin：集合映射
来源：http://tg.shxzskj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://xm.bjjhwx.cn

[T07] Kotlin：集合过滤
来源：http://hg.gzmigu.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ny.nszjky.cn

[T08] Kotlin：数据类
来源：http://pq.shxzskj.cn

data class User(val name: String, val age: Int)
来源：http://ze.asd995.cn

[T09] Kotlin：扩展函数
来源：http://im.yuntaijiaju.cn

fun String.exclaim() = this + "!"
来源：http://na.nszjky.cn

[T10] Kotlin：默认参数
来源：http://pa.shxzskj.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://dy.hnjuh.cn

[T11] Kotlin：协程
来源：http://dj.shtwfgs.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://nt.szsharing.cn

[T12] Kotlin：解构声明
来源：http://cg.colortex.cn

val (a, b) = Pair(1, 2)
来源：http://ez.szsharing.cn

[T13] Kotlin：只读 Map
来源：http://pi.panjiajie.cn

val m = mapOf("a" to 1)
来源：http://fg.9csxet.cn

[T14] Kotlin：循环
来源：http://my.panjiajie.cn

for (i in 1..10) println(i)
来源：http://hn.nszjky.cn

[T15] Kotlin：接口
来源：http://yr.chemitech.net.cn

interface Shape { fun area(): Double }
来源：http://vf.gzmigu.cn

[T16] Swift：Hello World
来源：http://qw.shxzskj.cn

print("Hello")
来源：http://se.muxihuayi.cn

[T17] Swift：变量与常量
来源：http://ph.shtwfgs.cn

var a = 1;  let b = 2
来源：http://vt.yuexingan06.cn

[T18] Swift：字符串插值
来源：http://oq.jctech888.com.cn

"值: \(b)"
来源：http://cu.nicolike.cn

[T19] Swift：可选绑定
来源：http://ad.szxytkj.cn

if let n = opt { print(n) }
来源：http://in.szsharing.cn

[T20] Swift：数组操作
来源：http://gk.muxihuayi.cn

var a = [1, 2, 3];  a.append(4)
来源：http://wq.panjiajie.cn

[T21] Swift：遍历
来源：http://kp.hahajie.cn

for x in a { print(x) }
来源：http://nu.hnjuh.cn

[T22] Swift：字典
来源：http://qm.huixiangedu.cn

var d = ["a": 1];  d["b"] = 2
来源：http://si.hnjuh.cn

[T23] Swift：函数
来源：http://pi.bjjhwx.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://vv.9csxet.cn

[T24] Swift：闭包
来源：http://kr.chemitech.net.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://bw.9csxet.cn

[T25] Swift：结构体
来源：http://cv.haigaiapp.cn

struct P { var x: Int }
来源：http://or.bjjhwx.cn

[T26] Swift：类与重写
来源：http://ay.lnxyls.cn

class A: Base { override func f() {} }
来源：http://jm.hnjuh.cn

[T27] Swift：错误处理
来源：http://wc.hahajie.cn

do { try f() } catch { print(error) }
来源：http://ny.gzmigu.cn

[T28] Swift：枚举
来源：http://gi.wgjwhj.cn

enum Color { case red, green }
来源：http://su.yuntaijiaju.cn

[T29] Swift：guard 提前返回
来源：http://jw.chemitech.net.cn

guard let x = opt else { return }
来源：http://dq.szsharing.cn

[T30] Swift：协议
来源：http://ob.shtwfgs.cn

protocol Shape { func area() -> Double }
来源：http://zm.wgjwhj.cn

[T31] Lua：Hello World
来源：http://sw.shxzukj.cn

print("Hello")
来源：http://br.chemitech.net.cn

[T32] Lua：局部变量
来源：http://zh.szxytkj.cn

local a = 1
来源：http://qr.hahajie.cn

[T33] Lua：表（数组）
来源：http://ka.huanxung.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://tt.hahajie.cn

[T34] Lua：遍历表
来源：http://xn.hnjuh.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://gf.haigaiapp.cn

[T35] Lua：字典表
来源：http://he.bjjhwx.cn

local d = { a = 1 };  d.b = 2
来源：http://sa.hnjuh.cn

[T36] Lua：函数
来源：http://yg.shtwfgs.cn

function add(a, b) return a + b end
来源：http://wr.521024.cn

[T37] Lua：字符串拼接
来源：http://pm.colortex.cn

"a" .. "b"
来源：http://ss.asd995.cn

[T38] Lua：条件
来源：http://fm.bookmarksfly.cn

if x > 0 then print("正") end
来源：http://fw.shxzskj.cn

[T39] Lua：模式匹配
来源：http://zn.shxzukj.cn

string.find(s, "%d+")
来源：http://is.haigaiapp.cn

[T40] Lua：元表
来源：http://yh.panjiajie.cn

setmetatable({}, { __index = base })
来源：http://ug.haigaiapp.cn

[T41] Perl：Hello World
来源：http://mg.9csxet.cn

print "Hello\n";
来源：http://jb.yuntaijiaju.cn

[T42] Perl：变量类型
来源：http://ae.szsharing.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://nt.szxytkj.cn

[T43] Perl：字符串插值
来源：http://aw.huanxung.cn

"值: $a"
来源：http://hg.nicolike.cn

[T44] Perl：条件
来源：http://ov.haigaiapp.cn

if ($a > 0) { print "正"; }
来源：http://yf.jianghongdianzi.cn

[T45] Perl：数组遍历
来源：http://tf.shxzukj.cn

for my $x (@arr) { print $x; }
来源：http://rw.huixiangedu.cn

[T46] Perl：哈希操作
来源：http://vy.jctech888.com.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://xa.hnjuh.cn

[T47] Perl：正则捕获
来源：http://ur.muxihuayi.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://bv.haigaiapp.cn

[T48] Perl：正则替换
来源：http://mx.huixinmuqiang.cn

$s =~ s/old/new/g;
来源：http://bi.shxzukj.cn

[T49] Perl：函数
来源：http://cl.muxihuayi.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://eh.shxzskj.cn

[T50] Perl：逐行读文件
来源：http://op.huixinmuqiang.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://hr.yuexingan06.cn


<!-- 参考信息 -->