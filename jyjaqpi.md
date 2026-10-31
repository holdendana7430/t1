代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://bg.shtwfgs.cn

[R50] awk 求和
来源：http://sc.asd995.cn

awk '{s += $2} END {print s}' a.txt
来源：http://yy.bjjhwx.cn

[R51] 排序去重取前几
来源：http://tr.shtwfgs.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://dp.asd995.cn

[R52] 统计行数
来源：http://fc.huixinmuqiang.cn

wc -l a.txt
来源：http://kn.colortex.cn

[R53] 查看文件头与实时尾
来源：http://os.yuexingan06.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://bv.chemitech.net.cn

[R54] 比较两个文件
来源：http://wg.yuntaijiaju.cn

diff a.txt b.txt
来源：http://ep.lnxyls.cn

[R55] 压缩与解压
来源：http://hv.haigaiapp.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://lr.shxzukj.cn

[R56] 远程拷贝
来源：http://xi.nszjky.cn

scp file user@host:/path/
来源：http://dl.hahajie.cn

[R57] 远程执行命令
来源：http://xa.huixiangedu.cn

ssh user@host 'uptime'
来源：http://cu.huixiangedu.cn

[R58] 下载文件
来源：http://xi.yuexingan06.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://zr.hnjuh.cn

[R59] 发 POST JSON
来源：http://hz.jctech888.com.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://jp.yuntaijiaju.cn

[R60] 只看 HTTP 状态码
来源：http://bj.hnjuh.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://cw.yuexingan06.cn

[R61] 磁盘占用
来源：http://ro.colortex.cn

df -h;  du -sh *
来源：http://fm.nszjky.cn

[R62] 找最占空间的文件
来源：http://ks.huanxung.cn

du -ah . | sort -rh | head -10
来源：http://sb.jianghongdianzi.cn

[R63] 内存与进程
来源：http://we.panjiajie.cn

free -h;  ps aux | grep nginx
来源：http://nj.shtwfgs.cn

[R64] 结束进程
来源：http://ig.newstarts.cn

kill -9 $(pgrep -f app.py)
来源：http://ce.huanxung.cn

[R65] 查看端口占用
来源：http://ke.szsharing.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://jo.colortex.cn

[R66] 定时任务
来源：http://gx.yuexingan06.cn

crontab -e;  crontab -l
来源：http://cm.wgjwhj.cn

[R67] 生成随机十六进制串
来源：http://dh.nszjky.cn

openssl rand -hex 16
来源：http://ho.huanxung.cn

[R68] 计算文件校验值
来源：http://la.wgjwhj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://uu.huixiangedu.cn

[R69] 生成随机密码
来源：http://jb.shtwfgs.cn

head -c 16 /dev/urandom | base64
来源：http://oh.jianghongdianzi.cn

[R70] 时间戳与互转
来源：http://wo.nicolike.cn

date +%s;  date -d @1700000000
来源：http://fh.asd995.cn

[R71] 日期格式化
来源：http://tg.wgjwhj.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://xt.szsharing.cn

[R72] 等待端口就绪
来源：http://ni.shxzukj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://qa.hnjuh.cn

[R73] 分割大日志
来源：http://mg.panjiajie.cn

split -l 1000 big.log part_
来源：http://ky.panjiajie.cn

[R74] 批量重命名
来源：http://wv.521024.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ly.nicolike.cn

[R75] 导出环境变量
来源：http://hu.muxihuayi.cn

export PATH="$HOME/bin:$PATH"
来源：http://nh.jianghongdianzi.cn

[R76] 使用临时文件
来源：http://jb.521024.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://gc.nszjky.cn

[R77] 读取用户输入
来源：http://nc.szxytkj.cn

read -rp "请输入: " ans
来源：http://pr.haigaiapp.cn

[R78] 交互式菜单
来源：http://qn.colortex.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://lh.muxihuayi.cn

[R79] 解析命令行选项
来源：http://hr.shxzukj.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ik.chemitech.net.cn

[R80] 查看脚本执行耗时
来源：http://xc.hnjuh.cn

time ./run.sh
来源：http://ou.nszjky.cn

================================================================================
来源：http://oz.nszjky.cn

S. C / C++ 专题
来源：http://nd.wgjwhj.cn

================================================================================
来源：http://gb.lnxyls.cn

[S01] C：Hello World
来源：http://tz.9csxet.cn

#include <stdio.h>
来源：http://gu.chemitech.net.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://rq.gzmigu.cn

[S02] C：变量与格式化输出
来源：http://jh.newstarts.cn

int a = 10; printf("%d\n", a);
来源：http://yd.panjiajie.cn

[S03] C：读入整数
来源：http://uz.lnxyls.cn

int x; scanf("%d", &x);
来源：http://hj.nszjky.cn

[S04] C：字符串复制
来源：http://vb.huanxung.cn

char dst[32]; strcpy(dst, "hi");
来源：http://xn.nszjky.cn

[S05] C：字符串长度
来源：http://tu.muxihuayi.cn

strlen(s)
来源：http://ga.bookmarksfly.cn

[S06] C：字符串比较
来源：http://pc.jianghongdianzi.cn

strcmp(a, b) == 0
来源：http://zn.huixinmuqiang.cn

[S07] C：数组遍历求和
来源：http://cu.szxytkj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://dk.lnxyls.cn

[S08] C：动态内存分配与释放
来源：http://gc.szsharing.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://li.9csxet.cn

[S09] C：结构体定义与初始化
来源：http://jh.chemitech.net.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://uh.nszjky.cn

[S10] C：指针与解引用
来源：http://pv.colortex.cn

int *p = &a;  *p = 5;
来源：http://bi.nszjky.cn

[S11] C：逐行读文件
来源：http://ko.huanxung.cn

FILE *f = fopen("a.txt", "r");
来源：http://sd.shtwfgs.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://rw.hahajie.cn

fclose(f);
来源：http://rb.shxzukj.cn

[S12] C：写文件
来源：http://tw.jianghongdianzi.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://gf.shxzukj.cn

[S13] C：宏定义
来源：http://hv.521024.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://rp.bjjhwx.cn

[S14] C：枚举
来源：http://in.9csxet.cn

enum Color { RED, GREEN, BLUE };
来源：http://ns.bookmarksfly.cn

[S15] C：类型转换
来源：http://zz.huixinmuqiang.cn

(double) a / b
来源：http://ha.shxzukj.cn

[S16] C：位操作置位
来源：http://cu.gzmigu.cn

x |= (1 << 3);
来源：http://kb.shtwfgs.cn

[S17] C：安全拼接字符串
来源：http://fu.shxzskj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://uy.colortex.cn

[S18] C：命令行参数
来源：http://so.hahajie.cn

int main(int argc, char **argv)
来源：http://vw.wgjwhj.cn

[S19] C：快速排序
来源：http://lt.bjjhwx.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ui.newstarts.cn

[S20] C：二分查找
来源：http://av.asd995.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://zq.szxytkj.cn

[S21] C：字符类别判断
来源：http://ix.szxytkj.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://qg.jctech888.com.cn

[S22] C：字符串转数字
来源：http://yy.huanxung.cn

atoi("42");  strtod("3.14", NULL);
来源：http://np.newstarts.cn

[S23] C：随机数
来源：http://zg.szxytkj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://cu.shxzukj.cn

[S24] C：获取本地时间
来源：http://hn.newstarts.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://fu.asd995.cn

[S25] C：内存拷贝
来源：http://hl.shxzukj.cn

memcpy(dst, src, n);
来源：http://ub.hnjuh.cn

[S26] C：内存清零
来源：http://mp.huixiangedu.cn

memset(a, 0, sizeof a);
来源：http://tl.huanxung.cn

[S27] C：定义常量
来源：http://mz.szxytkj.cn

const double PI = 3.14159;
来源：http://zo.szxytkj.cn

[S28] C：静态变量
来源：http://qt.shtwfgs.cn

static int counter = 0;
来源：http://ou.colortex.cn

[S29] C：变参函数
来源：http://wt.wgjwhj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://qq.jianghongdianzi.cn

[S30] C：头文件保护
来源：http://ao.nszjky.cn

#ifndef X_H
来源：http://zk.chemitech.net.cn

#define X_H
来源：http://yr.muxihuayi.cn

#endif
来源：http://io.huixinmuqiang.cn

[S31] C++：Hello World
来源：http://uh.bjjhwx.cn

#include <iostream>
来源：http://gf.szxytkj.cn

int main() { std::cout << "Hello\n"; }
来源：http://kc.szxytkj.cn

[S32] C++：字符串
来源：http://wa.lnxyls.cn

std::string s = "hi";  s += "!";
来源：http://ru.jianghongdianzi.cn

[S33] C++：vector 增删
来源：http://hl.jctech888.com.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://ju.shxzukj.cn

[S34] C++：遍历 vector
来源：http://xu.haigaiapp.cn

for (auto &x : v) { std::cout << x; }
来源：http://cw.hahajie.cn

[S35] C++：map
来源：http://po.asd995.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://sk.shxzskj.cn

[S36] C++：unordered_map
来源：http://we.haigaiapp.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://fh.colortex.cn

[S37] C++：set
来源：http://wj.muxihuayi.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://oz.shtwfgs.cn

[S38] C++：排序
来源：http://hb.9csxet.cn

std::sort(v.begin(), v.end());
来源：http://cr.yuntaijiaju.cn

[S39] C++：自定义比较器排序
来源：http://oi.huixiangedu.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ll.9csxet.cn

[S40] C++：查找元素
来源：http://ef.hnjuh.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://zh.shxzskj.cn

[S41] C++：类与构造函数
来源：http://uq.shxzskj.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://gz.newstarts.cn

[S42] C++：继承与虚函数
来源：http://lc.nicolike.cn

class B : public Base { public: void f() override {} };
来源：http://uj.bjjhwx.cn

[S43] C++：智能指针
来源：http://qz.bookmarksfly.cn

auto p = std::make_unique<int>(5);
来源：http://np.muxihuayi.cn

[S44] C++：引用传参
来源：http://dn.nicolike.cn

void inc(int &x) { ++x; }
来源：http://vn.huixiangedu.cn

[S45] C++：lambda
来源：http://oh.lnxyls.cn

auto add = [](int a, int b) { return a + b; };
来源：http://pq.panjiajie.cn

[S46] C++：函数模板
来源：http://zp.hahajie.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://gk.szsharing.cn

[S47] C++：结构化绑定遍历
来源：http://cl.bjjhwx.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://xu.yuexingan06.cn

[S48] C++：逐行读文件
来源：http://yp.9csxet.cn

std::ifstream in("a.txt");  std::string line;
来源：http://zb.huixiangedu.cn

while (std::getline(in, line)) { }
来源：http://bu.lnxyls.cn

[S49] C++：写文件
来源：http://ts.wgjwhj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://pw.hahajie.cn

[S50] C++：格式化数字
来源：http://ch.shxzukj.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://sw.521024.cn

[S51] C++：显式类型转换
来源：http://hk.gzmigu.cn

static_cast<double>(a) / b
来源：http://ud.shtwfgs.cn

[S52] C++：const 与 noexcept
来源：http://ye.bjjhwx.cn

int size() const noexcept { return n_; }
来源：http://un.haigaiapp.cn

[S53] C++：移动语义
来源：http://yf.szxytkj.cn

std::vector<int> w = std::move(v);
来源：http://sm.chemitech.net.cn

[S54] C++：异常处理
来源：http://jx.9csxet.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://wd.huanxung.cn

[S55] C++：结构化绑定
来源：http://ct.yuexingan06.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://di.huixinmuqiang.cn

[S56] C++：optional
来源：http://mf.hnjuh.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://bc.9csxet.cn

[S57] C++：编译期常量
来源：http://ul.huixiangedu.cn

constexpr int N = 10;
来源：http://mf.bjjhwx.cn

[S58] C++：命名空间
来源：http://jy.shtwfgs.cn

namespace ns { int f() { return 1; } }
来源：http://ru.bookmarksfly.cn

[S59] C++：静态断言
来源：http://od.521024.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://jh.lnxyls.cn

[S60] C++：遍历并删除元素
来源：http://dk.colortex.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ec.asd995.cn

================================================================================
来源：http://fw.bjjhwx.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://fh.shxzskj.cn

================================================================================
来源：http://wo.yuntaijiaju.cn

[T01] Kotlin：Hello World
来源：http://nx.shxzukj.cn

println("Hello")
来源：http://ss.shtwfgs.cn

[T02] Kotlin：变量
来源：http://li.huixinmuqiang.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://dl.lnxyls.cn

[T03] Kotlin：字符串模板
来源：http://pl.wgjwhj.cn

"值: $b"
来源：http://qg.shxzskj.cn

[T04] Kotlin：空安全
来源：http://be.huixiangedu.cn

val n: String? = null;  n?.length
来源：http://ag.jctech888.com.cn

[T05] Kotlin：when 表达式
来源：http://bi.newstarts.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://je.asd995.cn

[T06] Kotlin：集合映射
来源：http://rq.gzmigu.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://gt.yuntaijiaju.cn

[T07] Kotlin：集合过滤
来源：http://sg.wgjwhj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://kf.szsharing.cn

[T08] Kotlin：数据类
来源：http://jj.muxihuayi.cn

data class User(val name: String, val age: Int)
来源：http://lp.nszjky.cn

[T09] Kotlin：扩展函数
来源：http://cn.bookmarksfly.cn

fun String.exclaim() = this + "!"
来源：http://zd.newstarts.cn

[T10] Kotlin：默认参数
来源：http://qv.szsharing.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://qs.9csxet.cn

[T11] Kotlin：协程
来源：http://fi.yuexingan06.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ds.shtwfgs.cn

[T12] Kotlin：解构声明
来源：http://yp.gzmigu.cn

val (a, b) = Pair(1, 2)
来源：http://bb.lnxyls.cn

[T13] Kotlin：只读 Map
来源：http://gp.gzmigu.cn

val m = mapOf("a" to 1)
来源：http://xe.shtwfgs.cn

[T14] Kotlin：循环
来源：http://gl.nszjky.cn

for (i in 1..10) println(i)
来源：http://bw.yuexingan06.cn

[T15] Kotlin：接口
来源：http://iv.huixiangedu.cn

interface Shape { fun area(): Double }
来源：http://sa.521024.cn

[T16] Swift：Hello World
来源：http://kx.chemitech.net.cn

print("Hello")
来源：http://tz.huanxung.cn

[T17] Swift：变量与常量
来源：http://qg.yuexingan06.cn

var a = 1;  let b = 2
来源：http://ct.bjjhwx.cn

[T18] Swift：字符串插值
来源：http://vk.yuntaijiaju.cn

"值: \(b)"
来源：http://lb.shxzskj.cn

[T19] Swift：可选绑定
来源：http://io.panjiajie.cn

if let n = opt { print(n) }
来源：http://kz.muxihuayi.cn

[T20] Swift：数组操作
来源：http://jj.chemitech.net.cn

var a = [1, 2, 3];  a.append(4)
来源：http://id.521024.cn

[T21] Swift：遍历
来源：http://yg.shxzukj.cn

for x in a { print(x) }
来源：http://zt.yuntaijiaju.cn

[T22] Swift：字典
来源：http://xu.huixinmuqiang.cn

var d = ["a": 1];  d["b"] = 2
来源：http://em.jctech888.com.cn

[T23] Swift：函数
来源：http://sp.bjjhwx.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ft.gzmigu.cn

[T24] Swift：闭包
来源：http://kz.9csxet.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ge.shxzskj.cn

[T25] Swift：结构体
来源：http://pt.asd995.cn

struct P { var x: Int }
来源：http://qq.chemitech.net.cn

[T26] Swift：类与重写
来源：http://pp.nszjky.cn

class A: Base { override func f() {} }
来源：http://el.wgjwhj.cn

[T27] Swift：错误处理
来源：http://lt.bjjhwx.cn

do { try f() } catch { print(error) }
来源：http://as.szxytkj.cn

[T28] Swift：枚举
来源：http://bv.yuntaijiaju.cn

enum Color { case red, green }
来源：http://fr.lnxyls.cn

[T29] Swift：guard 提前返回
来源：http://rf.hnjuh.cn

guard let x = opt else { return }
来源：http://xt.gzmigu.cn

[T30] Swift：协议
来源：http://ft.huixinmuqiang.cn

protocol Shape { func area() -> Double }
来源：http://au.jianghongdianzi.cn

[T31] Lua：Hello World
来源：http://wq.muxihuayi.cn

print("Hello")
来源：http://kf.huixinmuqiang.cn

[T32] Lua：局部变量
来源：http://mf.9csxet.cn

local a = 1
来源：http://ig.yuntaijiaju.cn

[T33] Lua：表（数组）
来源：http://qh.jctech888.com.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://fm.newstarts.cn

[T34] Lua：遍历表
来源：http://yu.asd995.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://qb.wgjwhj.cn

[T35] Lua：字典表
来源：http://uy.521024.cn

local d = { a = 1 };  d.b = 2
来源：http://mr.shtwfgs.cn

[T36] Lua：函数
来源：http://kr.chemitech.net.cn

function add(a, b) return a + b end
来源：http://hf.bookmarksfly.cn

[T37] Lua：字符串拼接
来源：http://bv.szsharing.cn

"a" .. "b"
来源：http://bl.bookmarksfly.cn

[T38] Lua：条件
来源：http://ta.muxihuayi.cn

if x > 0 then print("正") end
来源：http://ou.hnjuh.cn

[T39] Lua：模式匹配
来源：http://qx.huixinmuqiang.cn

string.find(s, "%d+")
来源：http://tx.hnjuh.cn

[T40] Lua：元表
来源：http://vw.asd995.cn

setmetatable({}, { __index = base })
来源：http://eb.jctech888.com.cn

[T41] Perl：Hello World
来源：http://xo.haigaiapp.cn

print "Hello\n";
来源：http://xm.shtwfgs.cn

[T42] Perl：变量类型
来源：http://jr.panjiajie.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://fv.bookmarksfly.cn

[T43] Perl：字符串插值
来源：http://ed.nszjky.cn

"值: $a"
来源：http://jz.9csxet.cn

[T44] Perl：条件
来源：http://hc.newstarts.cn

if ($a > 0) { print "正"; }
来源：http://yi.yuexingan06.cn

[T45] Perl：数组遍历
来源：http://gy.bjjhwx.cn

for my $x (@arr) { print $x; }
来源：http://ur.jctech888.com.cn

[T46] Perl：哈希操作
来源：http://xn.yuntaijiaju.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://qi.muxihuayi.cn

[T47] Perl：正则捕获
来源：http://ua.szxytkj.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ao.wgjwhj.cn

[T48] Perl：正则替换
来源：http://yj.colortex.cn

$s =~ s/old/new/g;
来源：http://ed.huixiangedu.cn

[T49] Perl：函数
来源：http://qd.chemitech.net.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://mg.asd995.cn

[T50] Perl：逐行读文件
来源：http://od.nszjky.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://uc.jctech888.com.cn

while (my $line = <$fh>) { print $line; }
来源：http://vg.jianghongdianzi.cn

[T51] Scala：Hello World
来源：http://yb.shtwfgs.cn

println("Hello")
来源：http://bf.jianghongdianzi.cn

[T52] Scala：变量
来源：http://aj.panjiajie.cn


<!-- 参考信息 -->