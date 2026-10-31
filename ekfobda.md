代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://up.huanxung.cn

[R50] awk 求和
来源：http://dv.521024.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ym.shxzskj.cn

[R51] 排序去重取前几
来源：http://pq.chemitech.net.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://pm.nicolike.cn

[R52] 统计行数
来源：http://oo.colortex.cn

wc -l a.txt
来源：http://io.shtwfgs.cn

[R53] 查看文件头与实时尾
来源：http://ak.shtwfgs.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://cr.hahajie.cn

[R54] 比较两个文件
来源：http://ff.szxytkj.cn

diff a.txt b.txt
来源：http://ts.colortex.cn

[R55] 压缩与解压
来源：http://no.huixiangedu.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://of.szxytkj.cn

[R56] 远程拷贝
来源：http://fy.yuexingan06.cn

scp file user@host:/path/
来源：http://kf.chemitech.net.cn

[R57] 远程执行命令
来源：http://yz.huanxung.cn

ssh user@host 'uptime'
来源：http://ae.nszjky.cn

[R58] 下载文件
来源：http://lc.nszjky.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://te.shxzskj.cn

[R59] 发 POST JSON
来源：http://sn.huixinmuqiang.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ul.shxzskj.cn

[R60] 只看 HTTP 状态码
来源：http://jc.muxihuayi.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://cl.bjjhwx.cn

[R61] 磁盘占用
来源：http://gm.nszjky.cn

df -h;  du -sh *
来源：http://qq.hahajie.cn

[R62] 找最占空间的文件
来源：http://dx.yuexingan06.cn

du -ah . | sort -rh | head -10
来源：http://kn.colortex.cn

[R63] 内存与进程
来源：http://kk.chemitech.net.cn

free -h;  ps aux | grep nginx
来源：http://wo.asd995.cn

[R64] 结束进程
来源：http://em.panjiajie.cn

kill -9 $(pgrep -f app.py)
来源：http://id.huanxung.cn

[R65] 查看端口占用
来源：http://nu.bjjhwx.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://jw.haigaiapp.cn

[R66] 定时任务
来源：http://sa.lnxyls.cn

crontab -e;  crontab -l
来源：http://go.jianghongdianzi.cn

[R67] 生成随机十六进制串
来源：http://yx.shtwfgs.cn

openssl rand -hex 16
来源：http://up.bookmarksfly.cn

[R68] 计算文件校验值
来源：http://qj.haigaiapp.cn

sha256sum a.txt;  md5sum a.txt
来源：http://gk.szsharing.cn

[R69] 生成随机密码
来源：http://uv.haigaiapp.cn

head -c 16 /dev/urandom | base64
来源：http://nr.bookmarksfly.cn

[R70] 时间戳与互转
来源：http://or.newstarts.cn

date +%s;  date -d @1700000000
来源：http://yt.hnjuh.cn

[R71] 日期格式化
来源：http://uv.9csxet.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://wj.wgjwhj.cn

[R72] 等待端口就绪
来源：http://wj.hnjuh.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ld.yuexingan06.cn

[R73] 分割大日志
来源：http://eh.huanxung.cn

split -l 1000 big.log part_
来源：http://ec.jianghongdianzi.cn

[R74] 批量重命名
来源：http://vj.jctech888.com.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://cn.jctech888.com.cn

[R75] 导出环境变量
来源：http://hc.nicolike.cn

export PATH="$HOME/bin:$PATH"
来源：http://vh.nszjky.cn

[R76] 使用临时文件
来源：http://ow.yuexingan06.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://jv.shxzskj.cn

[R77] 读取用户输入
来源：http://oh.yuexingan06.cn

read -rp "请输入: " ans
来源：http://qo.huanxung.cn

[R78] 交互式菜单
来源：http://zj.9csxet.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://of.huixiangedu.cn

[R79] 解析命令行选项
来源：http://fs.chemitech.net.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://pl.muxihuayi.cn

[R80] 查看脚本执行耗时
来源：http://xx.yuntaijiaju.cn

time ./run.sh
来源：http://it.nicolike.cn

================================================================================
来源：http://dk.szxytkj.cn

S. C / C++ 专题
来源：http://zg.jianghongdianzi.cn

================================================================================
来源：http://xw.huixiangedu.cn

[S01] C：Hello World
来源：http://ku.muxihuayi.cn

#include <stdio.h>
来源：http://uo.gzmigu.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://mh.newstarts.cn

[S02] C：变量与格式化输出
来源：http://jk.szsharing.cn

int a = 10; printf("%d\n", a);
来源：http://jl.bookmarksfly.cn

[S03] C：读入整数
来源：http://vt.huanxung.cn

int x; scanf("%d", &x);
来源：http://rm.nszjky.cn

[S04] C：字符串复制
来源：http://hh.yuntaijiaju.cn

char dst[32]; strcpy(dst, "hi");
来源：http://sn.521024.cn

[S05] C：字符串长度
来源：http://gj.panjiajie.cn

strlen(s)
来源：http://gj.huixiangedu.cn

[S06] C：字符串比较
来源：http://an.521024.cn

strcmp(a, b) == 0
来源：http://bo.asd995.cn

[S07] C：数组遍历求和
来源：http://bi.chemitech.net.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://an.shxzskj.cn

[S08] C：动态内存分配与释放
来源：http://jv.hahajie.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://dc.jctech888.com.cn

[S09] C：结构体定义与初始化
来源：http://ts.jctech888.com.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://qp.hnjuh.cn

[S10] C：指针与解引用
来源：http://vo.chemitech.net.cn

int *p = &a;  *p = 5;
来源：http://zy.szsharing.cn

[S11] C：逐行读文件
来源：http://rt.newstarts.cn

FILE *f = fopen("a.txt", "r");
来源：http://ih.shxzskj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://xf.shxzskj.cn

fclose(f);
来源：http://et.jianghongdianzi.cn

[S12] C：写文件
来源：http://jj.muxihuayi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://kh.newstarts.cn

[S13] C：宏定义
来源：http://wv.szsharing.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://ou.yuntaijiaju.cn

[S14] C：枚举
来源：http://di.521024.cn

enum Color { RED, GREEN, BLUE };
来源：http://sm.yuntaijiaju.cn

[S15] C：类型转换
来源：http://li.huixiangedu.cn

(double) a / b
来源：http://cq.9csxet.cn

[S16] C：位操作置位
来源：http://tq.9csxet.cn

x |= (1 << 3);
来源：http://uo.huixinmuqiang.cn

[S17] C：安全拼接字符串
来源：http://fo.yuexingan06.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ch.panjiajie.cn

[S18] C：命令行参数
来源：http://gb.huixinmuqiang.cn

int main(int argc, char **argv)
来源：http://bd.bookmarksfly.cn

[S19] C：快速排序
来源：http://hp.bjjhwx.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ni.jctech888.com.cn

[S20] C：二分查找
来源：http://au.newstarts.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://fv.muxihuayi.cn

[S21] C：字符类别判断
来源：http://fg.nicolike.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://bi.huixiangedu.cn

[S22] C：字符串转数字
来源：http://aa.jctech888.com.cn

atoi("42");  strtod("3.14", NULL);
来源：http://sw.yuexingan06.cn

[S23] C：随机数
来源：http://ba.lnxyls.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://cb.nicolike.cn

[S24] C：获取本地时间
来源：http://ti.9csxet.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://or.bookmarksfly.cn

[S25] C：内存拷贝
来源：http://rv.jianghongdianzi.cn

memcpy(dst, src, n);
来源：http://my.newstarts.cn

[S26] C：内存清零
来源：http://af.9csxet.cn

memset(a, 0, sizeof a);
来源：http://ag.wgjwhj.cn

[S27] C：定义常量
来源：http://sd.jianghongdianzi.cn

const double PI = 3.14159;
来源：http://so.yuntaijiaju.cn

[S28] C：静态变量
来源：http://xx.yuntaijiaju.cn

static int counter = 0;
来源：http://yi.nicolike.cn

[S29] C：变参函数
来源：http://df.asd995.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://vj.hahajie.cn

[S30] C：头文件保护
来源：http://ey.nszjky.cn

#ifndef X_H
来源：http://ff.szsharing.cn

#define X_H
来源：http://cc.bookmarksfly.cn

#endif
来源：http://tg.shxzskj.cn

[S31] C++：Hello World
来源：http://wc.chemitech.net.cn

#include <iostream>
来源：http://cd.shtwfgs.cn

int main() { std::cout << "Hello\n"; }
来源：http://fk.colortex.cn

[S32] C++：字符串
来源：http://ny.haigaiapp.cn

std::string s = "hi";  s += "!";
来源：http://ox.yuexingan06.cn

[S33] C++：vector 增删
来源：http://jf.muxihuayi.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://nx.muxihuayi.cn

[S34] C++：遍历 vector
来源：http://dz.panjiajie.cn

for (auto &x : v) { std::cout << x; }
来源：http://gy.jianghongdianzi.cn

[S35] C++：map
来源：http://gs.shxzskj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://yq.yuexingan06.cn

[S36] C++：unordered_map
来源：http://tw.lnxyls.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://uc.bjjhwx.cn

[S37] C++：set
来源：http://vn.yuexingan06.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ui.shxzukj.cn

[S38] C++：排序
来源：http://yg.yuntaijiaju.cn

std::sort(v.begin(), v.end());
来源：http://ky.wgjwhj.cn

[S39] C++：自定义比较器排序
来源：http://zf.chemitech.net.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ke.shtwfgs.cn

[S40] C++：查找元素
来源：http://ir.shtwfgs.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://rt.huixiangedu.cn

[S41] C++：类与构造函数
来源：http://rh.panjiajie.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://rr.muxihuayi.cn

[S42] C++：继承与虚函数
来源：http://fn.jctech888.com.cn

class B : public Base { public: void f() override {} };
来源：http://bo.nicolike.cn

[S43] C++：智能指针
来源：http://na.bookmarksfly.cn

auto p = std::make_unique<int>(5);
来源：http://jb.yuexingan06.cn

[S44] C++：引用传参
来源：http://im.9csxet.cn

void inc(int &x) { ++x; }
来源：http://xp.bookmarksfly.cn

[S45] C++：lambda
来源：http://bs.jianghongdianzi.cn

auto add = [](int a, int b) { return a + b; };
来源：http://za.shxzskj.cn

[S46] C++：函数模板
来源：http://rp.huixiangedu.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ae.bookmarksfly.cn

[S47] C++：结构化绑定遍历
来源：http://sk.muxihuayi.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://qu.shtwfgs.cn

[S48] C++：逐行读文件
来源：http://zb.bjjhwx.cn

std::ifstream in("a.txt");  std::string line;
来源：http://rv.yuntaijiaju.cn

while (std::getline(in, line)) { }
来源：http://ki.shxzukj.cn

[S49] C++：写文件
来源：http://jk.hahajie.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ny.chemitech.net.cn

[S50] C++：格式化数字
来源：http://sl.szxytkj.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://tg.hnjuh.cn

[S51] C++：显式类型转换
来源：http://dg.chemitech.net.cn

static_cast<double>(a) / b
来源：http://xm.lnxyls.cn

[S52] C++：const 与 noexcept
来源：http://dp.huanxung.cn

int size() const noexcept { return n_; }
来源：http://wy.shxzukj.cn

[S53] C++：移动语义
来源：http://il.yuexingan06.cn

std::vector<int> w = std::move(v);
来源：http://sw.yuexingan06.cn

[S54] C++：异常处理
来源：http://by.colortex.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mq.gzmigu.cn

[S55] C++：结构化绑定
来源：http://gd.9csxet.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://bg.huixiangedu.cn

[S56] C++：optional
来源：http://mp.huanxung.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://mh.huanxung.cn

[S57] C++：编译期常量
来源：http://ix.szxytkj.cn

constexpr int N = 10;
来源：http://sy.newstarts.cn

[S58] C++：命名空间
来源：http://ll.hahajie.cn

namespace ns { int f() { return 1; } }
来源：http://pn.szxytkj.cn

[S59] C++：静态断言
来源：http://wj.panjiajie.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ky.muxihuayi.cn

[S60] C++：遍历并删除元素
来源：http://ta.asd995.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://np.huixiangedu.cn

================================================================================
来源：http://qw.jctech888.com.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://il.521024.cn

================================================================================
来源：http://oy.shtwfgs.cn

[T01] Kotlin：Hello World
来源：http://ac.521024.cn

println("Hello")
来源：http://hw.muxihuayi.cn

[T02] Kotlin：变量
来源：http://xy.hnjuh.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://wi.huixiangedu.cn

[T03] Kotlin：字符串模板
来源：http://le.asd995.cn

"值: $b"
来源：http://aw.szxytkj.cn

[T04] Kotlin：空安全
来源：http://rf.panjiajie.cn

val n: String? = null;  n?.length
来源：http://cu.jctech888.com.cn

[T05] Kotlin：when 表达式
来源：http://ec.szxytkj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://jw.wgjwhj.cn

[T06] Kotlin：集合映射
来源：http://qp.wgjwhj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://jt.yuexingan06.cn

[T07] Kotlin：集合过滤
来源：http://xu.gzmigu.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://il.huixiangedu.cn

[T08] Kotlin：数据类
来源：http://dm.huanxung.cn

data class User(val name: String, val age: Int)
来源：http://oq.nszjky.cn

[T09] Kotlin：扩展函数
来源：http://cr.jianghongdianzi.cn

fun String.exclaim() = this + "!"
来源：http://fe.shtwfgs.cn

[T10] Kotlin：默认参数
来源：http://mv.gzmigu.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ev.jianghongdianzi.cn

[T11] Kotlin：协程
来源：http://sz.panjiajie.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://pl.shxzskj.cn

[T12] Kotlin：解构声明
来源：http://pe.bjjhwx.cn

val (a, b) = Pair(1, 2)
来源：http://qz.asd995.cn

[T13] Kotlin：只读 Map
来源：http://rx.hnjuh.cn

val m = mapOf("a" to 1)
来源：http://wy.9csxet.cn

[T14] Kotlin：循环
来源：http://cy.muxihuayi.cn

for (i in 1..10) println(i)
来源：http://cp.huixinmuqiang.cn

[T15] Kotlin：接口
来源：http://ks.shxzukj.cn

interface Shape { fun area(): Double }
来源：http://nm.jctech888.com.cn

[T16] Swift：Hello World
来源：http://ki.huanxung.cn

print("Hello")
来源：http://ht.521024.cn

[T17] Swift：变量与常量
来源：http://ug.lnxyls.cn

var a = 1;  let b = 2
来源：http://wy.9csxet.cn

[T18] Swift：字符串插值
来源：http://nr.gzmigu.cn

"值: \(b)"
来源：http://ma.jianghongdianzi.cn

[T19] Swift：可选绑定
来源：http://oy.bookmarksfly.cn

if let n = opt { print(n) }
来源：http://es.panjiajie.cn

[T20] Swift：数组操作
来源：http://gy.521024.cn

var a = [1, 2, 3];  a.append(4)
来源：http://sr.jctech888.com.cn

[T21] Swift：遍历
来源：http://ow.yuntaijiaju.cn

for x in a { print(x) }
来源：http://py.shtwfgs.cn

[T22] Swift：字典
来源：http://fy.nszjky.cn

var d = ["a": 1];  d["b"] = 2
来源：http://mh.panjiajie.cn

[T23] Swift：函数
来源：http://xo.wgjwhj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://sv.huixiangedu.cn

[T24] Swift：闭包
来源：http://ng.szxytkj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://lr.chemitech.net.cn

[T25] Swift：结构体
来源：http://it.9csxet.cn

struct P { var x: Int }
来源：http://vd.gzmigu.cn

[T26] Swift：类与重写
来源：http://wv.huixinmuqiang.cn

class A: Base { override func f() {} }
来源：http://tw.hahajie.cn

[T27] Swift：错误处理
来源：http://hk.muxihuayi.cn

do { try f() } catch { print(error) }
来源：http://hl.huixinmuqiang.cn

[T28] Swift：枚举
来源：http://sz.yuntaijiaju.cn

enum Color { case red, green }
来源：http://mz.lnxyls.cn

[T29] Swift：guard 提前返回
来源：http://zk.521024.cn

guard let x = opt else { return }
来源：http://fh.panjiajie.cn

[T30] Swift：协议
来源：http://tv.huanxung.cn

protocol Shape { func area() -> Double }
来源：http://qi.nicolike.cn

[T31] Lua：Hello World
来源：http://gl.chemitech.net.cn

print("Hello")
来源：http://rl.asd995.cn

[T32] Lua：局部变量
来源：http://no.nszjky.cn

local a = 1
来源：http://zv.yuexingan06.cn

[T33] Lua：表（数组）
来源：http://cv.shxzukj.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://tk.colortex.cn

[T34] Lua：遍历表
来源：http://ro.wgjwhj.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://bx.bookmarksfly.cn

[T35] Lua：字典表
来源：http://wk.9csxet.cn

local d = { a = 1 };  d.b = 2
来源：http://zo.muxihuayi.cn

[T36] Lua：函数
来源：http://oq.9csxet.cn

function add(a, b) return a + b end
来源：http://pt.asd995.cn

[T37] Lua：字符串拼接
来源：http://kj.521024.cn

"a" .. "b"
来源：http://pd.nszjky.cn

[T38] Lua：条件
来源：http://sy.colortex.cn

if x > 0 then print("正") end
来源：http://qe.521024.cn

[T39] Lua：模式匹配
来源：http://oo.haigaiapp.cn

string.find(s, "%d+")
来源：http://bd.lnxyls.cn

[T40] Lua：元表
来源：http://er.yuntaijiaju.cn

setmetatable({}, { __index = base })
来源：http://tb.gzmigu.cn

[T41] Perl：Hello World
来源：http://ot.szxytkj.cn

print "Hello\n";
来源：http://vx.jctech888.com.cn

[T42] Perl：变量类型
来源：http://be.yuntaijiaju.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://mh.szxytkj.cn

[T43] Perl：字符串插值
来源：http://yt.lnxyls.cn

"值: $a"
来源：http://oh.shtwfgs.cn

[T44] Perl：条件
来源：http://qe.9csxet.cn

if ($a > 0) { print "正"; }
来源：http://vv.lnxyls.cn

[T45] Perl：数组遍历
来源：http://lk.nszjky.cn

for my $x (@arr) { print $x; }
来源：http://vl.shxzskj.cn

[T46] Perl：哈希操作
来源：http://xu.lnxyls.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://du.huixiangedu.cn

[T47] Perl：正则捕获
来源：http://ze.hahajie.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://st.shtwfgs.cn

[T48] Perl：正则替换
来源：http://rq.jianghongdianzi.cn

$s =~ s/old/new/g;
来源：http://uy.jianghongdianzi.cn

[T49] Perl：函数
来源：http://lj.nicolike.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://fd.bookmarksfly.cn

[T50] Perl：逐行读文件
来源：http://kc.hahajie.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://bk.yuexingan06.cn

while (my $line = <$fh>) { print $line; }
来源：http://dc.shtwfgs.cn

[T51] Scala：Hello World
来源：http://es.nszjky.cn

println("Hello")
来源：http://uz.asd995.cn

[T52] Scala：变量
来源：http://cs.wgjwhj.cn


<!-- 参考信息 -->