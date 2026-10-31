代发 wailian999

find . -name "*.log" -type f
来源：http://gx.muxihuayi.cn

[R44] 按修改时间查找
来源：http://pp.szxytkj.cn

find . -mtime -7 -type f
来源：http://vv.panjiajie.cn

[R45] 批量删除
来源：http://vb.shtwfgs.cn

find . -name "*.tmp" -delete
来源：http://dj.panjiajie.cn

[R46] 递归替换文件内容
来源：http://ng.newstarts.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://qr.wgjwhj.cn

[R47] sed 单行替换
来源：http://xb.jianghongdianzi.cn

sed -i 's/foo/bar/g' a.txt
来源：http://zu.chemitech.net.cn

[R48] awk 取指定列
来源：http://xv.hnjuh.cn

awk '{print $1, $3}' a.txt
来源：http://qe.asd995.cn

[R49] awk 带条件
来源：http://qg.nicolike.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://wb.haigaiapp.cn

[R50] awk 求和
来源：http://yl.nszjky.cn

awk '{s += $2} END {print s}' a.txt
来源：http://fw.huixinmuqiang.cn

[R51] 排序去重取前几
来源：http://ox.521024.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://om.lnxyls.cn

[R52] 统计行数
来源：http://mw.jianghongdianzi.cn

wc -l a.txt
来源：http://ki.chemitech.net.cn

[R53] 查看文件头与实时尾
来源：http://ak.shxzskj.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://bo.nszjky.cn

[R54] 比较两个文件
来源：http://ao.lnxyls.cn

diff a.txt b.txt
来源：http://eg.panjiajie.cn

[R55] 压缩与解压
来源：http://zo.bookmarksfly.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://bw.bjjhwx.cn

[R56] 远程拷贝
来源：http://uf.muxihuayi.cn

scp file user@host:/path/
来源：http://zy.muxihuayi.cn

[R57] 远程执行命令
来源：http://ho.muxihuayi.cn

ssh user@host 'uptime'
来源：http://xt.bjjhwx.cn

[R58] 下载文件
来源：http://oa.bjjhwx.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://lu.hahajie.cn

[R59] 发 POST JSON
来源：http://lg.muxihuayi.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://qf.yuexingan06.cn

[R60] 只看 HTTP 状态码
来源：http://av.szxytkj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://cd.szsharing.cn

[R61] 磁盘占用
来源：http://af.muxihuayi.cn

df -h;  du -sh *
来源：http://jq.chemitech.net.cn

[R62] 找最占空间的文件
来源：http://ia.szxytkj.cn

du -ah . | sort -rh | head -10
来源：http://gj.hahajie.cn

[R63] 内存与进程
来源：http://pa.gzmigu.cn

free -h;  ps aux | grep nginx
来源：http://gh.huixinmuqiang.cn

[R64] 结束进程
来源：http://mh.9csxet.cn

kill -9 $(pgrep -f app.py)
来源：http://rc.yuexingan06.cn

[R65] 查看端口占用
来源：http://fz.newstarts.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://el.9csxet.cn

[R66] 定时任务
来源：http://bx.shxzukj.cn

crontab -e;  crontab -l
来源：http://af.colortex.cn

[R67] 生成随机十六进制串
来源：http://bt.szxytkj.cn

openssl rand -hex 16
来源：http://ck.hnjuh.cn

[R68] 计算文件校验值
来源：http://su.hnjuh.cn

sha256sum a.txt;  md5sum a.txt
来源：http://fg.shxzukj.cn

[R69] 生成随机密码
来源：http://vu.shxzskj.cn

head -c 16 /dev/urandom | base64
来源：http://rr.szsharing.cn

[R70] 时间戳与互转
来源：http://mv.muxihuayi.cn

date +%s;  date -d @1700000000
来源：http://pv.hnjuh.cn

[R71] 日期格式化
来源：http://vb.lnxyls.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://lg.9csxet.cn

[R72] 等待端口就绪
来源：http://xk.szsharing.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://vz.lnxyls.cn

[R73] 分割大日志
来源：http://us.chemitech.net.cn

split -l 1000 big.log part_
来源：http://ua.nicolike.cn

[R74] 批量重命名
来源：http://mz.muxihuayi.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://na.muxihuayi.cn

[R75] 导出环境变量
来源：http://tg.panjiajie.cn

export PATH="$HOME/bin:$PATH"
来源：http://ve.nicolike.cn

[R76] 使用临时文件
来源：http://lj.huixiangedu.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ni.huixinmuqiang.cn

[R77] 读取用户输入
来源：http://aq.panjiajie.cn

read -rp "请输入: " ans
来源：http://cw.wgjwhj.cn

[R78] 交互式菜单
来源：http://ee.szxytkj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://xr.muxihuayi.cn

[R79] 解析命令行选项
来源：http://rk.asd995.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://qx.szxytkj.cn

[R80] 查看脚本执行耗时
来源：http://xp.hahajie.cn

time ./run.sh
来源：http://wl.bjjhwx.cn

================================================================================
来源：http://qi.jctech888.com.cn

S. C / C++ 专题
来源：http://ui.shtwfgs.cn

================================================================================
来源：http://uv.yuntaijiaju.cn

[S01] C：Hello World
来源：http://en.nszjky.cn

#include <stdio.h>
来源：http://np.bookmarksfly.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://dh.521024.cn

[S02] C：变量与格式化输出
来源：http://up.hahajie.cn

int a = 10; printf("%d\n", a);
来源：http://jh.haigaiapp.cn

[S03] C：读入整数
来源：http://rc.yuexingan06.cn

int x; scanf("%d", &x);
来源：http://uh.yuexingan06.cn

[S04] C：字符串复制
来源：http://ap.521024.cn

char dst[32]; strcpy(dst, "hi");
来源：http://gg.muxihuayi.cn

[S05] C：字符串长度
来源：http://ks.colortex.cn

strlen(s)
来源：http://fn.huixiangedu.cn

[S06] C：字符串比较
来源：http://aj.colortex.cn

strcmp(a, b) == 0
来源：http://kq.chemitech.net.cn

[S07] C：数组遍历求和
来源：http://ij.panjiajie.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://wd.9csxet.cn

[S08] C：动态内存分配与释放
来源：http://dq.bookmarksfly.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://uq.hahajie.cn

[S09] C：结构体定义与初始化
来源：http://yw.huanxung.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://qx.colortex.cn

[S10] C：指针与解引用
来源：http://uj.hahajie.cn

int *p = &a;  *p = 5;
来源：http://on.haigaiapp.cn

[S11] C：逐行读文件
来源：http://av.huanxung.cn

FILE *f = fopen("a.txt", "r");
来源：http://xq.jctech888.com.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ee.521024.cn

fclose(f);
来源：http://lz.colortex.cn

[S12] C：写文件
来源：http://as.nicolike.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://pv.hahajie.cn

[S13] C：宏定义
来源：http://yp.shxzskj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ei.asd995.cn

[S14] C：枚举
来源：http://pj.bjjhwx.cn

enum Color { RED, GREEN, BLUE };
来源：http://vt.nszjky.cn

[S15] C：类型转换
来源：http://uj.jianghongdianzi.cn

(double) a / b
来源：http://vv.nszjky.cn

[S16] C：位操作置位
来源：http://xm.asd995.cn

x |= (1 << 3);
来源：http://aa.haigaiapp.cn

[S17] C：安全拼接字符串
来源：http://wc.shxzskj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ga.newstarts.cn

[S18] C：命令行参数
来源：http://rd.shxzskj.cn

int main(int argc, char **argv)
来源：http://nh.asd995.cn

[S19] C：快速排序
来源：http://iz.haigaiapp.cn

qsort(a, n, sizeof(int), cmp);
来源：http://kg.szsharing.cn

[S20] C：二分查找
来源：http://qt.nicolike.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hv.shxzskj.cn

[S21] C：字符类别判断
来源：http://hs.chemitech.net.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ae.bjjhwx.cn

[S22] C：字符串转数字
来源：http://bs.shtwfgs.cn

atoi("42");  strtod("3.14", NULL);
来源：http://lb.nicolike.cn

[S23] C：随机数
来源：http://ep.bjjhwx.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://dr.bookmarksfly.cn

[S24] C：获取本地时间
来源：http://uz.muxihuayi.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://zl.newstarts.cn

[S25] C：内存拷贝
来源：http://jl.wgjwhj.cn

memcpy(dst, src, n);
来源：http://nd.shxzukj.cn

[S26] C：内存清零
来源：http://al.bjjhwx.cn

memset(a, 0, sizeof a);
来源：http://pn.jianghongdianzi.cn

[S27] C：定义常量
来源：http://fw.szxytkj.cn

const double PI = 3.14159;
来源：http://yj.huixinmuqiang.cn

[S28] C：静态变量
来源：http://ow.bjjhwx.cn

static int counter = 0;
来源：http://xa.hnjuh.cn

[S29] C：变参函数
来源：http://jr.szxytkj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ug.bookmarksfly.cn

[S30] C：头文件保护
来源：http://es.nszjky.cn

#ifndef X_H
来源：http://vn.huixiangedu.cn

#define X_H
来源：http://br.muxihuayi.cn

#endif
来源：http://kx.lnxyls.cn

[S31] C++：Hello World
来源：http://ll.yuexingan06.cn

#include <iostream>
来源：http://yj.jctech888.com.cn

int main() { std::cout << "Hello\n"; }
来源：http://wb.hnjuh.cn

[S32] C++：字符串
来源：http://rh.gzmigu.cn

std::string s = "hi";  s += "!";
来源：http://eu.jianghongdianzi.cn

[S33] C++：vector 增删
来源：http://ob.colortex.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://xj.nicolike.cn

[S34] C++：遍历 vector
来源：http://iu.huixinmuqiang.cn

for (auto &x : v) { std::cout << x; }
来源：http://fp.lnxyls.cn

[S35] C++：map
来源：http://sq.colortex.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ce.gzmigu.cn

[S36] C++：unordered_map
来源：http://pd.szxytkj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://xn.hahajie.cn

[S37] C++：set
来源：http://fp.newstarts.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://av.bjjhwx.cn

[S38] C++：排序
来源：http://dz.nszjky.cn

std::sort(v.begin(), v.end());
来源：http://dc.gzmigu.cn

[S39] C++：自定义比较器排序
来源：http://qr.521024.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ha.yuntaijiaju.cn

[S40] C++：查找元素
来源：http://tq.huixiangedu.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ns.wgjwhj.cn

[S41] C++：类与构造函数
来源：http://fa.chemitech.net.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://et.hnjuh.cn

[S42] C++：继承与虚函数
来源：http://tq.nszjky.cn

class B : public Base { public: void f() override {} };
来源：http://ob.asd995.cn

[S43] C++：智能指针
来源：http://zs.shtwfgs.cn

auto p = std::make_unique<int>(5);
来源：http://mu.szxytkj.cn

[S44] C++：引用传参
来源：http://qv.huixinmuqiang.cn

void inc(int &x) { ++x; }
来源：http://qh.wgjwhj.cn

[S45] C++：lambda
来源：http://um.shxzskj.cn

auto add = [](int a, int b) { return a + b; };
来源：http://hp.hahajie.cn

[S46] C++：函数模板
来源：http://kg.lnxyls.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://qn.hnjuh.cn

[S47] C++：结构化绑定遍历
来源：http://db.chemitech.net.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://bg.bjjhwx.cn

[S48] C++：逐行读文件
来源：http://do.muxihuayi.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ik.huanxung.cn

while (std::getline(in, line)) { }
来源：http://gk.bookmarksfly.cn

[S49] C++：写文件
来源：http://cl.jianghongdianzi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://cp.hahajie.cn

[S50] C++：格式化数字
来源：http://go.szxytkj.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wr.bookmarksfly.cn

[S51] C++：显式类型转换
来源：http://up.chemitech.net.cn

static_cast<double>(a) / b
来源：http://id.hahajie.cn

[S52] C++：const 与 noexcept
来源：http://kt.jctech888.com.cn

int size() const noexcept { return n_; }
来源：http://rf.wgjwhj.cn

[S53] C++：移动语义
来源：http://ry.huixinmuqiang.cn

std::vector<int> w = std::move(v);
来源：http://cr.chemitech.net.cn

[S54] C++：异常处理
来源：http://be.muxihuayi.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://bp.colortex.cn

[S55] C++：结构化绑定
来源：http://hp.haigaiapp.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://bn.haigaiapp.cn

[S56] C++：optional
来源：http://vf.shtwfgs.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://gx.jianghongdianzi.cn

[S57] C++：编译期常量
来源：http://yh.bookmarksfly.cn

constexpr int N = 10;
来源：http://wh.huixinmuqiang.cn

[S58] C++：命名空间
来源：http://fc.szsharing.cn

namespace ns { int f() { return 1; } }
来源：http://hn.haigaiapp.cn

[S59] C++：静态断言
来源：http://jk.wgjwhj.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://fy.shtwfgs.cn

[S60] C++：遍历并删除元素
来源：http://zo.asd995.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://bx.wgjwhj.cn

================================================================================
来源：http://rm.huanxung.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://yf.nszjky.cn

================================================================================
来源：http://lg.newstarts.cn

[T01] Kotlin：Hello World
来源：http://og.asd995.cn

println("Hello")
来源：http://ku.nicolike.cn

[T02] Kotlin：变量
来源：http://ex.muxihuayi.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://jl.nicolike.cn

[T03] Kotlin：字符串模板
来源：http://xn.huanxung.cn

"值: $b"
来源：http://qg.panjiajie.cn

[T04] Kotlin：空安全
来源：http://am.asd995.cn

val n: String? = null;  n?.length
来源：http://qr.haigaiapp.cn

[T05] Kotlin：when 表达式
来源：http://xs.lnxyls.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://iv.huixinmuqiang.cn

[T06] Kotlin：集合映射
来源：http://wf.shxzskj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ac.jctech888.com.cn

[T07] Kotlin：集合过滤
来源：http://xi.haigaiapp.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://uc.shxzskj.cn

[T08] Kotlin：数据类
来源：http://ul.shtwfgs.cn

data class User(val name: String, val age: Int)
来源：http://uj.szxytkj.cn

[T09] Kotlin：扩展函数
来源：http://kd.huanxung.cn

fun String.exclaim() = this + "!"
来源：http://ys.panjiajie.cn

[T10] Kotlin：默认参数
来源：http://wl.gzmigu.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://fy.bjjhwx.cn

[T11] Kotlin：协程
来源：http://cl.shxzukj.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://xc.panjiajie.cn

[T12] Kotlin：解构声明
来源：http://uq.bookmarksfly.cn

val (a, b) = Pair(1, 2)
来源：http://jp.hnjuh.cn

[T13] Kotlin：只读 Map
来源：http://oi.bjjhwx.cn

val m = mapOf("a" to 1)
来源：http://bh.haigaiapp.cn

[T14] Kotlin：循环
来源：http://pb.chemitech.net.cn

for (i in 1..10) println(i)
来源：http://mo.huanxung.cn

[T15] Kotlin：接口
来源：http://tb.bjjhwx.cn

interface Shape { fun area(): Double }
来源：http://bj.hahajie.cn

[T16] Swift：Hello World
来源：http://le.huanxung.cn

print("Hello")
来源：http://qc.newstarts.cn

[T17] Swift：变量与常量
来源：http://qy.szxytkj.cn

var a = 1;  let b = 2
来源：http://xu.szxytkj.cn

[T18] Swift：字符串插值
来源：http://nc.wgjwhj.cn

"值: \(b)"
来源：http://rz.jianghongdianzi.cn

[T19] Swift：可选绑定
来源：http://zv.521024.cn

if let n = opt { print(n) }
来源：http://lx.gzmigu.cn

[T20] Swift：数组操作
来源：http://vf.hnjuh.cn

var a = [1, 2, 3];  a.append(4)
来源：http://bu.szxytkj.cn

[T21] Swift：遍历
来源：http://xp.hnjuh.cn

for x in a { print(x) }
来源：http://mb.nszjky.cn

[T22] Swift：字典
来源：http://as.muxihuayi.cn

var d = ["a": 1];  d["b"] = 2
来源：http://qb.hnjuh.cn

[T23] Swift：函数
来源：http://ka.hnjuh.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://jl.newstarts.cn

[T24] Swift：闭包
来源：http://kx.lnxyls.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://bp.shtwfgs.cn

[T25] Swift：结构体
来源：http://lm.521024.cn

struct P { var x: Int }
来源：http://yf.521024.cn

[T26] Swift：类与重写
来源：http://ym.yuntaijiaju.cn

class A: Base { override func f() {} }
来源：http://oy.nszjky.cn

[T27] Swift：错误处理
来源：http://ph.lnxyls.cn

do { try f() } catch { print(error) }
来源：http://lv.panjiajie.cn

[T28] Swift：枚举
来源：http://sv.huanxung.cn

enum Color { case red, green }
来源：http://ql.wgjwhj.cn

[T29] Swift：guard 提前返回
来源：http://jg.nszjky.cn

guard let x = opt else { return }
来源：http://vi.wgjwhj.cn

[T30] Swift：协议
来源：http://md.jctech888.com.cn

protocol Shape { func area() -> Double }
来源：http://tl.jctech888.com.cn

[T31] Lua：Hello World
来源：http://dz.huanxung.cn

print("Hello")
来源：http://di.newstarts.cn

[T32] Lua：局部变量
来源：http://bp.shxzukj.cn

local a = 1
来源：http://je.shxzukj.cn

[T33] Lua：表（数组）
来源：http://hw.huixiangedu.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://xk.shtwfgs.cn

[T34] Lua：遍历表
来源：http://em.muxihuayi.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://xb.asd995.cn

[T35] Lua：字典表
来源：http://hh.yuntaijiaju.cn

local d = { a = 1 };  d.b = 2
来源：http://om.hahajie.cn

[T36] Lua：函数
来源：http://aj.wgjwhj.cn

function add(a, b) return a + b end
来源：http://qj.lnxyls.cn

[T37] Lua：字符串拼接
来源：http://bh.szsharing.cn

"a" .. "b"
来源：http://yk.yuexingan06.cn

[T38] Lua：条件
来源：http://bs.asd995.cn

if x > 0 then print("正") end
来源：http://co.nszjky.cn

[T39] Lua：模式匹配
来源：http://ug.lnxyls.cn

string.find(s, "%d+")
来源：http://dt.shxzskj.cn

[T40] Lua：元表
来源：http://xy.szsharing.cn

setmetatable({}, { __index = base })
来源：http://wg.shxzukj.cn

[T41] Perl：Hello World
来源：http://gs.shtwfgs.cn

print "Hello\n";
来源：http://xc.shxzskj.cn

[T42] Perl：变量类型
来源：http://mr.panjiajie.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://kd.jianghongdianzi.cn

[T43] Perl：字符串插值
来源：http://zx.521024.cn

"值: $a"
来源：http://fx.jianghongdianzi.cn

[T44] Perl：条件
来源：http://gr.huixinmuqiang.cn

if ($a > 0) { print "正"; }
来源：http://og.panjiajie.cn

[T45] Perl：数组遍历
来源：http://ht.asd995.cn

for my $x (@arr) { print $x; }
来源：http://qe.szsharing.cn

[T46] Perl：哈希操作
来源：http://pn.panjiajie.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://hj.shtwfgs.cn


<!-- 参考信息 -->