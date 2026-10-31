代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：http://vz.wgjwhj.cn

[R48] awk 取指定列
来源：http://tk.chemitech.net.cn

awk '{print $1, $3}' a.txt
来源：http://um.huixinmuqiang.cn

[R49] awk 带条件
来源：http://zi.huanxung.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://is.szsharing.cn

[R50] awk 求和
来源：http://ac.szsharing.cn

awk '{s += $2} END {print s}' a.txt
来源：http://an.9csxet.cn

[R51] 排序去重取前几
来源：http://uy.gzmigu.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://bh.haigaiapp.cn

[R52] 统计行数
来源：http://su.muxihuayi.cn

wc -l a.txt
来源：http://ru.wgjwhj.cn

[R53] 查看文件头与实时尾
来源：http://cb.haigaiapp.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://mn.bjjhwx.cn

[R54] 比较两个文件
来源：http://xl.colortex.cn

diff a.txt b.txt
来源：http://fj.yuntaijiaju.cn

[R55] 压缩与解压
来源：http://rh.szxytkj.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://rz.nicolike.cn

[R56] 远程拷贝
来源：http://mj.hnjuh.cn

scp file user@host:/path/
来源：http://gn.lnxyls.cn

[R57] 远程执行命令
来源：http://iv.colortex.cn

ssh user@host 'uptime'
来源：http://bv.newstarts.cn

[R58] 下载文件
来源：http://lq.lnxyls.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://fd.wgjwhj.cn

[R59] 发 POST JSON
来源：http://nn.szsharing.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://jq.gzmigu.cn

[R60] 只看 HTTP 状态码
来源：http://nw.colortex.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://fn.yuexingan06.cn

[R61] 磁盘占用
来源：http://ka.panjiajie.cn

df -h;  du -sh *
来源：http://cp.nszjky.cn

[R62] 找最占空间的文件
来源：http://tp.jianghongdianzi.cn

du -ah . | sort -rh | head -10
来源：http://dy.gzmigu.cn

[R63] 内存与进程
来源：http://lb.muxihuayi.cn

free -h;  ps aux | grep nginx
来源：http://ur.gzmigu.cn

[R64] 结束进程
来源：http://oy.hahajie.cn

kill -9 $(pgrep -f app.py)
来源：http://hn.shxzskj.cn

[R65] 查看端口占用
来源：http://ur.huixinmuqiang.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://en.jctech888.com.cn

[R66] 定时任务
来源：http://hp.szsharing.cn

crontab -e;  crontab -l
来源：http://oo.szxytkj.cn

[R67] 生成随机十六进制串
来源：http://hi.nicolike.cn

openssl rand -hex 16
来源：http://lk.panjiajie.cn

[R68] 计算文件校验值
来源：http://yp.bookmarksfly.cn

sha256sum a.txt;  md5sum a.txt
来源：http://yc.huixiangedu.cn

[R69] 生成随机密码
来源：http://kb.newstarts.cn

head -c 16 /dev/urandom | base64
来源：http://vb.jianghongdianzi.cn

[R70] 时间戳与互转
来源：http://ya.521024.cn

date +%s;  date -d @1700000000
来源：http://eq.asd995.cn

[R71] 日期格式化
来源：http://gc.gzmigu.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://bm.panjiajie.cn

[R72] 等待端口就绪
来源：http://gf.bjjhwx.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://tn.chemitech.net.cn

[R73] 分割大日志
来源：http://dt.newstarts.cn

split -l 1000 big.log part_
来源：http://qd.hnjuh.cn

[R74] 批量重命名
来源：http://bg.gzmigu.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://qr.muxihuayi.cn

[R75] 导出环境变量
来源：http://ge.huanxung.cn

export PATH="$HOME/bin:$PATH"
来源：http://kn.521024.cn

[R76] 使用临时文件
来源：http://qb.jctech888.com.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://lb.huixinmuqiang.cn

[R77] 读取用户输入
来源：http://ql.jctech888.com.cn

read -rp "请输入: " ans
来源：http://iz.gzmigu.cn

[R78] 交互式菜单
来源：http://tg.newstarts.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://hb.szsharing.cn

[R79] 解析命令行选项
来源：http://sn.shxzukj.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://in.gzmigu.cn

[R80] 查看脚本执行耗时
来源：http://xj.bjjhwx.cn

time ./run.sh
来源：http://zc.muxihuayi.cn

================================================================================
来源：http://nf.bjjhwx.cn

S. C / C++ 专题
来源：http://aq.huanxung.cn

================================================================================
来源：http://um.szsharing.cn

[S01] C：Hello World
来源：http://pi.nicolike.cn

#include <stdio.h>
来源：http://jy.bookmarksfly.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://cg.colortex.cn

[S02] C：变量与格式化输出
来源：http://zu.newstarts.cn

int a = 10; printf("%d\n", a);
来源：http://cq.nszjky.cn

[S03] C：读入整数
来源：http://ug.shxzukj.cn

int x; scanf("%d", &x);
来源：http://di.521024.cn

[S04] C：字符串复制
来源：http://lf.gzmigu.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ne.huixinmuqiang.cn

[S05] C：字符串长度
来源：http://be.nszjky.cn

strlen(s)
来源：http://bo.wgjwhj.cn

[S06] C：字符串比较
来源：http://zx.bjjhwx.cn

strcmp(a, b) == 0
来源：http://zp.colortex.cn

[S07] C：数组遍历求和
来源：http://vs.colortex.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://zv.jianghongdianzi.cn

[S08] C：动态内存分配与释放
来源：http://kd.asd995.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://gm.gzmigu.cn

[S09] C：结构体定义与初始化
来源：http://sl.nszjky.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://jz.newstarts.cn

[S10] C：指针与解引用
来源：http://ln.bjjhwx.cn

int *p = &a;  *p = 5;
来源：http://hs.hahajie.cn

[S11] C：逐行读文件
来源：http://dt.nicolike.cn

FILE *f = fopen("a.txt", "r");
来源：http://jv.gzmigu.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://jt.shtwfgs.cn

fclose(f);
来源：http://qn.9csxet.cn

[S12] C：写文件
来源：http://uc.asd995.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://ev.521024.cn

[S13] C：宏定义
来源：http://wl.yuexingan06.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://iu.szxytkj.cn

[S14] C：枚举
来源：http://of.newstarts.cn

enum Color { RED, GREEN, BLUE };
来源：http://gb.lnxyls.cn

[S15] C：类型转换
来源：http://kq.huanxung.cn

(double) a / b
来源：http://we.colortex.cn

[S16] C：位操作置位
来源：http://um.nszjky.cn

x |= (1 << 3);
来源：http://tf.hnjuh.cn

[S17] C：安全拼接字符串
来源：http://sj.9csxet.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://zr.hnjuh.cn

[S18] C：命令行参数
来源：http://ei.wgjwhj.cn

int main(int argc, char **argv)
来源：http://si.yuexingan06.cn

[S19] C：快速排序
来源：http://cg.shxzskj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://om.nicolike.cn

[S20] C：二分查找
来源：http://kh.jctech888.com.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://vc.nicolike.cn

[S21] C：字符类别判断
来源：http://qf.shxzskj.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ql.jianghongdianzi.cn

[S22] C：字符串转数字
来源：http://qe.9csxet.cn

atoi("42");  strtod("3.14", NULL);
来源：http://un.huixiangedu.cn

[S23] C：随机数
来源：http://tj.shtwfgs.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://kv.521024.cn

[S24] C：获取本地时间
来源：http://wr.hnjuh.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://rv.nicolike.cn

[S25] C：内存拷贝
来源：http://nv.wgjwhj.cn

memcpy(dst, src, n);
来源：http://mi.huixiangedu.cn

[S26] C：内存清零
来源：http://wo.yuexingan06.cn

memset(a, 0, sizeof a);
来源：http://vx.haigaiapp.cn

[S27] C：定义常量
来源：http://dx.huanxung.cn

const double PI = 3.14159;
来源：http://hk.huixinmuqiang.cn

[S28] C：静态变量
来源：http://cp.gzmigu.cn

static int counter = 0;
来源：http://kx.muxihuayi.cn

[S29] C：变参函数
来源：http://zy.asd995.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://fs.huixinmuqiang.cn

[S30] C：头文件保护
来源：http://mw.chemitech.net.cn

#ifndef X_H
来源：http://bj.panjiajie.cn

#define X_H
来源：http://ws.lnxyls.cn

#endif
来源：http://tn.asd995.cn

[S31] C++：Hello World
来源：http://db.bjjhwx.cn

#include <iostream>
来源：http://tq.9csxet.cn

int main() { std::cout << "Hello\n"; }
来源：http://ov.wgjwhj.cn

[S32] C++：字符串
来源：http://ge.szsharing.cn

std::string s = "hi";  s += "!";
来源：http://sq.asd995.cn

[S33] C++：vector 增删
来源：http://hx.newstarts.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://nu.jianghongdianzi.cn

[S34] C++：遍历 vector
来源：http://px.jctech888.com.cn

for (auto &x : v) { std::cout << x; }
来源：http://hb.jctech888.com.cn

[S35] C++：map
来源：http://cm.hnjuh.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://gg.colortex.cn

[S36] C++：unordered_map
来源：http://sv.bookmarksfly.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ur.muxihuayi.cn

[S37] C++：set
来源：http://qk.haigaiapp.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://sq.newstarts.cn

[S38] C++：排序
来源：http://rb.szsharing.cn

std::sort(v.begin(), v.end());
来源：http://vw.jctech888.com.cn

[S39] C++：自定义比较器排序
来源：http://ws.szxytkj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ls.lnxyls.cn

[S40] C++：查找元素
来源：http://sm.nicolike.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ar.colortex.cn

[S41] C++：类与构造函数
来源：http://dc.9csxet.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://zk.shxzukj.cn

[S42] C++：继承与虚函数
来源：http://xi.bjjhwx.cn

class B : public Base { public: void f() override {} };
来源：http://xr.huanxung.cn

[S43] C++：智能指针
来源：http://wf.huanxung.cn

auto p = std::make_unique<int>(5);
来源：http://ig.wgjwhj.cn

[S44] C++：引用传参
来源：http://uo.muxihuayi.cn

void inc(int &x) { ++x; }
来源：http://fy.lnxyls.cn

[S45] C++：lambda
来源：http://qc.yuexingan06.cn

auto add = [](int a, int b) { return a + b; };
来源：http://hq.shxzskj.cn

[S46] C++：函数模板
来源：http://lq.yuexingan06.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://lp.wgjwhj.cn

[S47] C++：结构化绑定遍历
来源：http://vz.jianghongdianzi.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://nw.huanxung.cn

[S48] C++：逐行读文件
来源：http://fk.gzmigu.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ei.huanxung.cn

while (std::getline(in, line)) { }
来源：http://eh.hahajie.cn

[S49] C++：写文件
来源：http://rd.bookmarksfly.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://zi.nszjky.cn

[S50] C++：格式化数字
来源：http://vv.chemitech.net.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://zr.shxzskj.cn

[S51] C++：显式类型转换
来源：http://nb.521024.cn

static_cast<double>(a) / b
来源：http://jw.521024.cn

[S52] C++：const 与 noexcept
来源：http://ae.newstarts.cn

int size() const noexcept { return n_; }
来源：http://rd.nszjky.cn

[S53] C++：移动语义
来源：http://ln.chemitech.net.cn

std::vector<int> w = std::move(v);
来源：http://sk.shxzukj.cn

[S54] C++：异常处理
来源：http://kw.shtwfgs.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://hc.jctech888.com.cn

[S55] C++：结构化绑定
来源：http://zk.newstarts.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ts.colortex.cn

[S56] C++：optional
来源：http://vm.chemitech.net.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://rz.bookmarksfly.cn

[S57] C++：编译期常量
来源：http://ok.9csxet.cn

constexpr int N = 10;
来源：http://xl.szsharing.cn

[S58] C++：命名空间
来源：http://qx.huanxung.cn

namespace ns { int f() { return 1; } }
来源：http://bi.jctech888.com.cn

[S59] C++：静态断言
来源：http://es.muxihuayi.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://cw.bookmarksfly.cn

[S60] C++：遍历并删除元素
来源：http://qg.szsharing.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://mr.chemitech.net.cn

================================================================================
来源：http://jp.yuntaijiaju.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ex.huixiangedu.cn

================================================================================
来源：http://jz.newstarts.cn

[T01] Kotlin：Hello World
来源：http://rn.nszjky.cn

println("Hello")
来源：http://wf.huixinmuqiang.cn

[T02] Kotlin：变量
来源：http://vo.shtwfgs.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://tj.nszjky.cn

[T03] Kotlin：字符串模板
来源：http://wh.nicolike.cn

"值: $b"
来源：http://sd.521024.cn

[T04] Kotlin：空安全
来源：http://ux.panjiajie.cn

val n: String? = null;  n?.length
来源：http://pw.newstarts.cn

[T05] Kotlin：when 表达式
来源：http://uz.panjiajie.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ir.nszjky.cn

[T06] Kotlin：集合映射
来源：http://ru.jianghongdianzi.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://wb.bjjhwx.cn

[T07] Kotlin：集合过滤
来源：http://jt.huixiangedu.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ci.chemitech.net.cn

[T08] Kotlin：数据类
来源：http://kl.asd995.cn

data class User(val name: String, val age: Int)
来源：http://su.wgjwhj.cn

[T09] Kotlin：扩展函数
来源：http://tm.bookmarksfly.cn

fun String.exclaim() = this + "!"
来源：http://tk.chemitech.net.cn

[T10] Kotlin：默认参数
来源：http://pt.jctech888.com.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://yz.jctech888.com.cn

[T11] Kotlin：协程
来源：http://as.colortex.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://zl.huixinmuqiang.cn

[T12] Kotlin：解构声明
来源：http://nu.hahajie.cn

val (a, b) = Pair(1, 2)
来源：http://ct.yuexingan06.cn

[T13] Kotlin：只读 Map
来源：http://og.panjiajie.cn

val m = mapOf("a" to 1)
来源：http://rq.newstarts.cn

[T14] Kotlin：循环
来源：http://qc.9csxet.cn

for (i in 1..10) println(i)
来源：http://zy.newstarts.cn

[T15] Kotlin：接口
来源：http://pc.chemitech.net.cn

interface Shape { fun area(): Double }
来源：http://ie.nszjky.cn

[T16] Swift：Hello World
来源：http://kv.szxytkj.cn

print("Hello")
来源：http://ns.szxytkj.cn

[T17] Swift：变量与常量
来源：http://iw.hnjuh.cn

var a = 1;  let b = 2
来源：http://qq.chemitech.net.cn

[T18] Swift：字符串插值
来源：http://km.panjiajie.cn

"值: \(b)"
来源：http://yd.yuexingan06.cn

[T19] Swift：可选绑定
来源：http://rs.asd995.cn

if let n = opt { print(n) }
来源：http://eu.szsharing.cn

[T20] Swift：数组操作
来源：http://hc.huixinmuqiang.cn

var a = [1, 2, 3];  a.append(4)
来源：http://wg.yuexingan06.cn

[T21] Swift：遍历
来源：http://id.bjjhwx.cn

for x in a { print(x) }
来源：http://jn.521024.cn

[T22] Swift：字典
来源：http://oy.jianghongdianzi.cn

var d = ["a": 1];  d["b"] = 2
来源：http://zk.shxzukj.cn

[T23] Swift：函数
来源：http://ns.shxzskj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://vc.huanxung.cn

[T24] Swift：闭包
来源：http://pq.panjiajie.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ph.bookmarksfly.cn

[T25] Swift：结构体
来源：http://mi.bjjhwx.cn

struct P { var x: Int }
来源：http://ji.shxzukj.cn

[T26] Swift：类与重写
来源：http://ek.huixiangedu.cn

class A: Base { override func f() {} }
来源：http://bz.bookmarksfly.cn

[T27] Swift：错误处理
来源：http://cg.yuexingan06.cn

do { try f() } catch { print(error) }
来源：http://rd.asd995.cn

[T28] Swift：枚举
来源：http://ac.shxzukj.cn

enum Color { case red, green }
来源：http://gp.yuntaijiaju.cn

[T29] Swift：guard 提前返回
来源：http://mz.shtwfgs.cn

guard let x = opt else { return }
来源：http://uz.wgjwhj.cn

[T30] Swift：协议
来源：http://ln.jctech888.com.cn

protocol Shape { func area() -> Double }
来源：http://de.shtwfgs.cn

[T31] Lua：Hello World
来源：http://uc.nicolike.cn

print("Hello")
来源：http://hv.nicolike.cn

[T32] Lua：局部变量
来源：http://sr.bookmarksfly.cn

local a = 1
来源：http://ke.yuexingan06.cn

[T33] Lua：表（数组）
来源：http://gp.muxihuayi.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://wy.panjiajie.cn

[T34] Lua：遍历表
来源：http://va.hahajie.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://tb.chemitech.net.cn

[T35] Lua：字典表
来源：http://cp.asd995.cn

local d = { a = 1 };  d.b = 2
来源：http://wv.yuntaijiaju.cn

[T36] Lua：函数
来源：http://im.hahajie.cn

function add(a, b) return a + b end
来源：http://rp.wgjwhj.cn

[T37] Lua：字符串拼接
来源：http://sg.yuexingan06.cn

"a" .. "b"
来源：http://hb.jianghongdianzi.cn

[T38] Lua：条件
来源：http://pm.huixiangedu.cn

if x > 0 then print("正") end
来源：http://bw.shxzukj.cn

[T39] Lua：模式匹配
来源：http://fz.bookmarksfly.cn

string.find(s, "%d+")
来源：http://ij.hnjuh.cn

[T40] Lua：元表
来源：http://hw.muxihuayi.cn

setmetatable({}, { __index = base })
来源：http://ml.huixinmuqiang.cn

[T41] Perl：Hello World
来源：http://da.yuntaijiaju.cn

print "Hello\n";
来源：http://qc.nszjky.cn

[T42] Perl：变量类型
来源：http://pf.nicolike.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://kn.chemitech.net.cn

[T43] Perl：字符串插值
来源：http://fa.yuntaijiaju.cn

"值: $a"
来源：http://ah.hahajie.cn

[T44] Perl：条件
来源：http://fy.hnjuh.cn

if ($a > 0) { print "正"; }
来源：http://nj.yuexingan06.cn

[T45] Perl：数组遍历
来源：http://zt.szsharing.cn

for my $x (@arr) { print $x; }
来源：http://zo.szsharing.cn

[T46] Perl：哈希操作
来源：http://ur.muxihuayi.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://xc.hahajie.cn

[T47] Perl：正则捕获
来源：http://qf.muxihuayi.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://fx.huixiangedu.cn

[T48] Perl：正则替换
来源：http://ga.bjjhwx.cn

$s =~ s/old/new/g;
来源：http://le.haigaiapp.cn

[T49] Perl：函数
来源：http://cu.jctech888.com.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://hz.nicolike.cn

[T50] Perl：逐行读文件
来源：http://bh.colortex.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://bt.huixinmuqiang.cn


<!-- 参考信息 -->