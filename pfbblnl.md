代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：http://ly.szxytkj.cn

[R48] awk 取指定列
来源：http://cg.newstarts.cn

awk '{print $1, $3}' a.txt
来源：http://ay.szsharing.cn

[R49] awk 带条件
来源：http://ld.bjjhwx.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://su.9csxet.cn

[R50] awk 求和
来源：http://mc.colortex.cn

awk '{s += $2} END {print s}' a.txt
来源：http://nw.nszjky.cn

[R51] 排序去重取前几
来源：http://cx.hahajie.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://pc.yuexingan06.cn

[R52] 统计行数
来源：http://ug.huixiangedu.cn

wc -l a.txt
来源：http://yi.szsharing.cn

[R53] 查看文件头与实时尾
来源：http://bb.shxzukj.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://er.yuntaijiaju.cn

[R54] 比较两个文件
来源：http://nb.shtwfgs.cn

diff a.txt b.txt
来源：http://st.colortex.cn

[R55] 压缩与解压
来源：http://ua.szsharing.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://mz.shtwfgs.cn

[R56] 远程拷贝
来源：http://qr.nszjky.cn

scp file user@host:/path/
来源：http://lw.9csxet.cn

[R57] 远程执行命令
来源：http://pe.wgjwhj.cn

ssh user@host 'uptime'
来源：http://oq.muxihuayi.cn

[R58] 下载文件
来源：http://ll.szxytkj.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://yi.yuexingan06.cn

[R59] 发 POST JSON
来源：http://il.shxzskj.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://vl.haigaiapp.cn

[R60] 只看 HTTP 状态码
来源：http://mr.newstarts.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://oe.haigaiapp.cn

[R61] 磁盘占用
来源：http://dt.huanxung.cn

df -h;  du -sh *
来源：http://mf.nszjky.cn

[R62] 找最占空间的文件
来源：http://ai.gzmigu.cn

du -ah . | sort -rh | head -10
来源：http://aq.nszjky.cn

[R63] 内存与进程
来源：http://za.huanxung.cn

free -h;  ps aux | grep nginx
来源：http://mo.bjjhwx.cn

[R64] 结束进程
来源：http://wl.panjiajie.cn

kill -9 $(pgrep -f app.py)
来源：http://wi.colortex.cn

[R65] 查看端口占用
来源：http://tv.gzmigu.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://sw.521024.cn

[R66] 定时任务
来源：http://tg.bjjhwx.cn

crontab -e;  crontab -l
来源：http://lx.haigaiapp.cn

[R67] 生成随机十六进制串
来源：http://ll.chemitech.net.cn

openssl rand -hex 16
来源：http://hq.szsharing.cn

[R68] 计算文件校验值
来源：http://ur.gzmigu.cn

sha256sum a.txt;  md5sum a.txt
来源：http://nq.jianghongdianzi.cn

[R69] 生成随机密码
来源：http://qh.huanxung.cn

head -c 16 /dev/urandom | base64
来源：http://kj.panjiajie.cn

[R70] 时间戳与互转
来源：http://qz.szxytkj.cn

date +%s;  date -d @1700000000
来源：http://ug.huixiangedu.cn

[R71] 日期格式化
来源：http://bf.szsharing.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://nj.colortex.cn

[R72] 等待端口就绪
来源：http://bs.szsharing.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ro.shxzskj.cn

[R73] 分割大日志
来源：http://ix.haigaiapp.cn

split -l 1000 big.log part_
来源：http://wu.yuexingan06.cn

[R74] 批量重命名
来源：http://en.bjjhwx.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://td.nszjky.cn

[R75] 导出环境变量
来源：http://bi.hahajie.cn

export PATH="$HOME/bin:$PATH"
来源：http://fs.shxzskj.cn

[R76] 使用临时文件
来源：http://xg.9csxet.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://uk.yuntaijiaju.cn

[R77] 读取用户输入
来源：http://ru.jianghongdianzi.cn

read -rp "请输入: " ans
来源：http://bw.szsharing.cn

[R78] 交互式菜单
来源：http://wy.haigaiapp.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://dv.hnjuh.cn

[R79] 解析命令行选项
来源：http://lv.muxihuayi.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://rs.szxytkj.cn

[R80] 查看脚本执行耗时
来源：http://ay.jctech888.com.cn

time ./run.sh
来源：http://vl.9csxet.cn

================================================================================
来源：http://ls.huixiangedu.cn

S. C / C++ 专题
来源：http://zi.lnxyls.cn

================================================================================
来源：http://bt.hnjuh.cn

[S01] C：Hello World
来源：http://tq.huixiangedu.cn

#include <stdio.h>
来源：http://vb.muxihuayi.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://aq.panjiajie.cn

[S02] C：变量与格式化输出
来源：http://mv.jianghongdianzi.cn

int a = 10; printf("%d\n", a);
来源：http://vg.gzmigu.cn

[S03] C：读入整数
来源：http://zm.shtwfgs.cn

int x; scanf("%d", &x);
来源：http://cm.nicolike.cn

[S04] C：字符串复制
来源：http://uf.colortex.cn

char dst[32]; strcpy(dst, "hi");
来源：http://fw.shtwfgs.cn

[S05] C：字符串长度
来源：http://lr.yuexingan06.cn

strlen(s)
来源：http://kz.asd995.cn

[S06] C：字符串比较
来源：http://tg.nszjky.cn

strcmp(a, b) == 0
来源：http://qo.haigaiapp.cn

[S07] C：数组遍历求和
来源：http://wb.szxytkj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://vy.colortex.cn

[S08] C：动态内存分配与释放
来源：http://hi.yuntaijiaju.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://sq.yuntaijiaju.cn

[S09] C：结构体定义与初始化
来源：http://fd.yuexingan06.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ul.colortex.cn

[S10] C：指针与解引用
来源：http://zc.panjiajie.cn

int *p = &a;  *p = 5;
来源：http://uy.bjjhwx.cn

[S11] C：逐行读文件
来源：http://fh.hnjuh.cn

FILE *f = fopen("a.txt", "r");
来源：http://js.chemitech.net.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://dm.huixinmuqiang.cn

fclose(f);
来源：http://od.bjjhwx.cn

[S12] C：写文件
来源：http://em.szxytkj.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xl.szxytkj.cn

[S13] C：宏定义
来源：http://re.gzmigu.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jn.wgjwhj.cn

[S14] C：枚举
来源：http://cx.chemitech.net.cn

enum Color { RED, GREEN, BLUE };
来源：http://xv.lnxyls.cn

[S15] C：类型转换
来源：http://qb.yuntaijiaju.cn

(double) a / b
来源：http://kn.asd995.cn

[S16] C：位操作置位
来源：http://xq.huixinmuqiang.cn

x |= (1 << 3);
来源：http://jp.nszjky.cn

[S17] C：安全拼接字符串
来源：http://mg.newstarts.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://nt.nicolike.cn

[S18] C：命令行参数
来源：http://dv.jianghongdianzi.cn

int main(int argc, char **argv)
来源：http://xb.chemitech.net.cn

[S19] C：快速排序
来源：http://ir.panjiajie.cn

qsort(a, n, sizeof(int), cmp);
来源：http://jg.shxzukj.cn

[S20] C：二分查找
来源：http://nf.shtwfgs.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://kn.lnxyls.cn

[S21] C：字符类别判断
来源：http://tb.lnxyls.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://fv.hnjuh.cn

[S22] C：字符串转数字
来源：http://dp.9csxet.cn

atoi("42");  strtod("3.14", NULL);
来源：http://wi.hahajie.cn

[S23] C：随机数
来源：http://ci.colortex.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://bi.9csxet.cn

[S24] C：获取本地时间
来源：http://ii.9csxet.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://mb.lnxyls.cn

[S25] C：内存拷贝
来源：http://jr.huanxung.cn

memcpy(dst, src, n);
来源：http://lm.bjjhwx.cn

[S26] C：内存清零
来源：http://iu.wgjwhj.cn

memset(a, 0, sizeof a);
来源：http://cc.szxytkj.cn

[S27] C：定义常量
来源：http://xs.gzmigu.cn

const double PI = 3.14159;
来源：http://gi.9csxet.cn

[S28] C：静态变量
来源：http://wa.bjjhwx.cn

static int counter = 0;
来源：http://sw.huanxung.cn

[S29] C：变参函数
来源：http://ie.szxytkj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://he.521024.cn

[S30] C：头文件保护
来源：http://yu.asd995.cn

#ifndef X_H
来源：http://ul.huanxung.cn

#define X_H
来源：http://td.muxihuayi.cn

#endif
来源：http://zd.huanxung.cn

[S31] C++：Hello World
来源：http://vm.panjiajie.cn

#include <iostream>
来源：http://ig.jctech888.com.cn

int main() { std::cout << "Hello\n"; }
来源：http://pj.hnjuh.cn

[S32] C++：字符串
来源：http://gr.hnjuh.cn

std::string s = "hi";  s += "!";
来源：http://fh.jctech888.com.cn

[S33] C++：vector 增删
来源：http://jz.9csxet.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://yw.huixiangedu.cn

[S34] C++：遍历 vector
来源：http://yd.shxzskj.cn

for (auto &x : v) { std::cout << x; }
来源：http://wm.jctech888.com.cn

[S35] C++：map
来源：http://xf.nicolike.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://gs.newstarts.cn

[S36] C++：unordered_map
来源：http://qq.shtwfgs.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://qj.shxzukj.cn

[S37] C++：set
来源：http://zt.lnxyls.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://pg.muxihuayi.cn

[S38] C++：排序
来源：http://hk.asd995.cn

std::sort(v.begin(), v.end());
来源：http://rq.chemitech.net.cn

[S39] C++：自定义比较器排序
来源：http://sv.yuexingan06.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://yq.hahajie.cn

[S40] C++：查找元素
来源：http://zk.521024.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://oo.jctech888.com.cn

[S41] C++：类与构造函数
来源：http://fv.hahajie.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ig.bookmarksfly.cn

[S42] C++：继承与虚函数
来源：http://ka.colortex.cn

class B : public Base { public: void f() override {} };
来源：http://jf.nszjky.cn

[S43] C++：智能指针
来源：http://uf.haigaiapp.cn

auto p = std::make_unique<int>(5);
来源：http://fx.nszjky.cn

[S44] C++：引用传参
来源：http://cx.hnjuh.cn

void inc(int &x) { ++x; }
来源：http://re.wgjwhj.cn

[S45] C++：lambda
来源：http://tb.nicolike.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ie.muxihuayi.cn

[S46] C++：函数模板
来源：http://lr.yuexingan06.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://cz.lnxyls.cn

[S47] C++：结构化绑定遍历
来源：http://lk.szxytkj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://mz.bjjhwx.cn

[S48] C++：逐行读文件
来源：http://yc.szxytkj.cn

std::ifstream in("a.txt");  std::string line;
来源：http://gj.muxihuayi.cn

while (std::getline(in, line)) { }
来源：http://hx.jianghongdianzi.cn

[S49] C++：写文件
来源：http://xl.haigaiapp.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://uh.muxihuayi.cn

[S50] C++：格式化数字
来源：http://jx.gzmigu.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://tb.nszjky.cn

[S51] C++：显式类型转换
来源：http://ei.panjiajie.cn

static_cast<double>(a) / b
来源：http://qo.chemitech.net.cn

[S52] C++：const 与 noexcept
来源：http://cu.newstarts.cn

int size() const noexcept { return n_; }
来源：http://us.bjjhwx.cn

[S53] C++：移动语义
来源：http://kv.bookmarksfly.cn

std::vector<int> w = std::move(v);
来源：http://wf.521024.cn

[S54] C++：异常处理
来源：http://ih.bjjhwx.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://zi.asd995.cn

[S55] C++：结构化绑定
来源：http://kp.yuntaijiaju.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://wf.szsharing.cn

[S56] C++：optional
来源：http://sh.asd995.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://qt.nszjky.cn

[S57] C++：编译期常量
来源：http://hu.lnxyls.cn

constexpr int N = 10;
来源：http://bd.shxzskj.cn

[S58] C++：命名空间
来源：http://ej.newstarts.cn

namespace ns { int f() { return 1; } }
来源：http://jl.haigaiapp.cn

[S59] C++：静态断言
来源：http://wb.jctech888.com.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://gh.jianghongdianzi.cn

[S60] C++：遍历并删除元素
来源：http://uv.shtwfgs.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://jx.haigaiapp.cn

================================================================================
来源：http://vn.bjjhwx.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://bp.jctech888.com.cn

================================================================================
来源：http://hj.shxzskj.cn

[T01] Kotlin：Hello World
来源：http://kh.huixinmuqiang.cn

println("Hello")
来源：http://uc.bookmarksfly.cn

[T02] Kotlin：变量
来源：http://ww.hahajie.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://fm.yuexingan06.cn

[T03] Kotlin：字符串模板
来源：http://lm.yuexingan06.cn

"值: $b"
来源：http://bv.jianghongdianzi.cn

[T04] Kotlin：空安全
来源：http://ih.nszjky.cn

val n: String? = null;  n?.length
来源：http://jh.jctech888.com.cn

[T05] Kotlin：when 表达式
来源：http://ww.huixiangedu.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://eb.chemitech.net.cn

[T06] Kotlin：集合映射
来源：http://dq.muxihuayi.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ys.521024.cn

[T07] Kotlin：集合过滤
来源：http://ku.hahajie.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://tb.shxzukj.cn

[T08] Kotlin：数据类
来源：http://ip.newstarts.cn

data class User(val name: String, val age: Int)
来源：http://vk.huanxung.cn

[T09] Kotlin：扩展函数
来源：http://wq.jianghongdianzi.cn

fun String.exclaim() = this + "!"
来源：http://fo.hnjuh.cn

[T10] Kotlin：默认参数
来源：http://sj.9csxet.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://kw.asd995.cn

[T11] Kotlin：协程
来源：http://sw.hnjuh.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://qk.asd995.cn

[T12] Kotlin：解构声明
来源：http://ij.newstarts.cn

val (a, b) = Pair(1, 2)
来源：http://xm.yuexingan06.cn

[T13] Kotlin：只读 Map
来源：http://kl.yuntaijiaju.cn

val m = mapOf("a" to 1)
来源：http://il.chemitech.net.cn

[T14] Kotlin：循环
来源：http://ji.bjjhwx.cn

for (i in 1..10) println(i)
来源：http://hf.shtwfgs.cn

[T15] Kotlin：接口
来源：http://jf.yuexingan06.cn

interface Shape { fun area(): Double }
来源：http://cs.newstarts.cn

[T16] Swift：Hello World
来源：http://rq.bookmarksfly.cn

print("Hello")
来源：http://js.hnjuh.cn

[T17] Swift：变量与常量
来源：http://vl.wgjwhj.cn

var a = 1;  let b = 2
来源：http://re.huixiangedu.cn

[T18] Swift：字符串插值
来源：http://gk.huixinmuqiang.cn

"值: \(b)"
来源：http://oc.wgjwhj.cn

[T19] Swift：可选绑定
来源：http://jg.hnjuh.cn

if let n = opt { print(n) }
来源：http://ec.lnxyls.cn

[T20] Swift：数组操作
来源：http://zl.nszjky.cn

var a = [1, 2, 3];  a.append(4)
来源：http://rz.shtwfgs.cn

[T21] Swift：遍历
来源：http://lg.hnjuh.cn

for x in a { print(x) }
来源：http://dv.asd995.cn

[T22] Swift：字典
来源：http://nv.shxzukj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://or.shxzskj.cn

[T23] Swift：函数
来源：http://zv.shxzskj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://dv.newstarts.cn

[T24] Swift：闭包
来源：http://cd.9csxet.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ro.wgjwhj.cn

[T25] Swift：结构体
来源：http://rd.muxihuayi.cn

struct P { var x: Int }
来源：http://dd.colortex.cn

[T26] Swift：类与重写
来源：http://cx.wgjwhj.cn

class A: Base { override func f() {} }
来源：http://gc.jctech888.com.cn

[T27] Swift：错误处理
来源：http://hz.gzmigu.cn

do { try f() } catch { print(error) }
来源：http://gq.9csxet.cn

[T28] Swift：枚举
来源：http://is.hahajie.cn

enum Color { case red, green }
来源：http://av.nszjky.cn

[T29] Swift：guard 提前返回
来源：http://ze.jctech888.com.cn

guard let x = opt else { return }
来源：http://tb.jianghongdianzi.cn

[T30] Swift：协议
来源：http://ia.wgjwhj.cn

protocol Shape { func area() -> Double }
来源：http://vw.chemitech.net.cn

[T31] Lua：Hello World
来源：http://iz.nszjky.cn

print("Hello")
来源：http://cu.hahajie.cn

[T32] Lua：局部变量
来源：http://zs.wgjwhj.cn

local a = 1
来源：http://nt.szxytkj.cn

[T33] Lua：表（数组）
来源：http://pi.muxihuayi.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://xy.yuntaijiaju.cn

[T34] Lua：遍历表
来源：http://nb.nszjky.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://pd.szsharing.cn

[T35] Lua：字典表
来源：http://oz.bjjhwx.cn

local d = { a = 1 };  d.b = 2
来源：http://ym.haigaiapp.cn

[T36] Lua：函数
来源：http://gy.panjiajie.cn

function add(a, b) return a + b end
来源：http://yf.nszjky.cn

[T37] Lua：字符串拼接
来源：http://jr.huixiangedu.cn

"a" .. "b"
来源：http://om.yuexingan06.cn

[T38] Lua：条件
来源：http://qz.haigaiapp.cn

if x > 0 then print("正") end
来源：http://zu.newstarts.cn

[T39] Lua：模式匹配
来源：http://hf.hnjuh.cn

string.find(s, "%d+")
来源：http://fr.jianghongdianzi.cn

[T40] Lua：元表
来源：http://aa.shtwfgs.cn

setmetatable({}, { __index = base })
来源：http://iw.nszjky.cn

[T41] Perl：Hello World
来源：http://hz.muxihuayi.cn

print "Hello\n";
来源：http://ft.szsharing.cn

[T42] Perl：变量类型
来源：http://yi.asd995.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://qb.bjjhwx.cn

[T43] Perl：字符串插值
来源：http://tm.panjiajie.cn

"值: $a"
来源：http://gg.bjjhwx.cn

[T44] Perl：条件
来源：http://lp.asd995.cn

if ($a > 0) { print "正"; }
来源：http://kt.9csxet.cn

[T45] Perl：数组遍历
来源：http://ug.nicolike.cn

for my $x (@arr) { print $x; }
来源：http://rs.huixiangedu.cn

[T46] Perl：哈希操作
来源：http://fq.yuntaijiaju.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://mo.asd995.cn

[T47] Perl：正则捕获
来源：http://dh.huixinmuqiang.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://dw.521024.cn

[T48] Perl：正则替换
来源：http://ck.huanxung.cn

$s =~ s/old/new/g;
来源：http://jz.huixiangedu.cn

[T49] Perl：函数
来源：http://fd.nicolike.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://bk.shxzskj.cn

[T50] Perl：逐行读文件
来源：http://gh.nszjky.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://ay.muxihuayi.cn


<!-- 参考信息 -->