代发 wailian999

find . -name "*.tmp" -delete
来源：http://fb.colortex.cn

[R46] 递归替换文件内容
来源：http://xf.szxytkj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://od.muxihuayi.cn

[R47] sed 单行替换
来源：http://qu.jianghongdianzi.cn

sed -i 's/foo/bar/g' a.txt
来源：http://vb.nszjky.cn

[R48] awk 取指定列
来源：http://yl.haigaiapp.cn

awk '{print $1, $3}' a.txt
来源：http://vv.szxytkj.cn

[R49] awk 带条件
来源：http://jg.huanxung.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://bo.colortex.cn

[R50] awk 求和
来源：http://to.huixinmuqiang.cn

awk '{s += $2} END {print s}' a.txt
来源：http://py.haigaiapp.cn

[R51] 排序去重取前几
来源：http://tq.9csxet.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://hf.bookmarksfly.cn

[R52] 统计行数
来源：http://uv.shxzukj.cn

wc -l a.txt
来源：http://vl.lnxyls.cn

[R53] 查看文件头与实时尾
来源：http://sq.huixiangedu.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://jn.huixiangedu.cn

[R54] 比较两个文件
来源：http://qq.hnjuh.cn

diff a.txt b.txt
来源：http://vy.huixinmuqiang.cn

[R55] 压缩与解压
来源：http://jq.lnxyls.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ov.panjiajie.cn

[R56] 远程拷贝
来源：http://la.asd995.cn

scp file user@host:/path/
来源：http://mc.9csxet.cn

[R57] 远程执行命令
来源：http://gp.newstarts.cn

ssh user@host 'uptime'
来源：http://ei.huixinmuqiang.cn

[R58] 下载文件
来源：http://ln.huanxung.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://vu.hahajie.cn

[R59] 发 POST JSON
来源：http://km.colortex.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://wi.nszjky.cn

[R60] 只看 HTTP 状态码
来源：http://lg.huanxung.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ja.lnxyls.cn

[R61] 磁盘占用
来源：http://ts.asd995.cn

df -h;  du -sh *
来源：http://as.jianghongdianzi.cn

[R62] 找最占空间的文件
来源：http://zl.bjjhwx.cn

du -ah . | sort -rh | head -10
来源：http://is.haigaiapp.cn

[R63] 内存与进程
来源：http://ah.colortex.cn

free -h;  ps aux | grep nginx
来源：http://mq.muxihuayi.cn

[R64] 结束进程
来源：http://kr.huixiangedu.cn

kill -9 $(pgrep -f app.py)
来源：http://lb.huanxung.cn

[R65] 查看端口占用
来源：http://zb.wgjwhj.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://kk.521024.cn

[R66] 定时任务
来源：http://cn.bookmarksfly.cn

crontab -e;  crontab -l
来源：http://kw.szxytkj.cn

[R67] 生成随机十六进制串
来源：http://xr.huixinmuqiang.cn

openssl rand -hex 16
来源：http://pw.wgjwhj.cn

[R68] 计算文件校验值
来源：http://xu.lnxyls.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ih.szsharing.cn

[R69] 生成随机密码
来源：http://ob.nicolike.cn

head -c 16 /dev/urandom | base64
来源：http://rl.gzmigu.cn

[R70] 时间戳与互转
来源：http://iz.huanxung.cn

date +%s;  date -d @1700000000
来源：http://bf.muxihuayi.cn

[R71] 日期格式化
来源：http://sc.9csxet.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://sb.asd995.cn

[R72] 等待端口就绪
来源：http://nt.gzmigu.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://tp.jianghongdianzi.cn

[R73] 分割大日志
来源：http://xc.huixinmuqiang.cn

split -l 1000 big.log part_
来源：http://vl.newstarts.cn

[R74] 批量重命名
来源：http://gm.chemitech.net.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://dm.shtwfgs.cn

[R75] 导出环境变量
来源：http://ja.colortex.cn

export PATH="$HOME/bin:$PATH"
来源：http://zk.muxihuayi.cn

[R76] 使用临时文件
来源：http://no.muxihuayi.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://bp.nszjky.cn

[R77] 读取用户输入
来源：http://hn.panjiajie.cn

read -rp "请输入: " ans
来源：http://cq.jctech888.com.cn

[R78] 交互式菜单
来源：http://rp.colortex.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://oi.jianghongdianzi.cn

[R79] 解析命令行选项
来源：http://na.shtwfgs.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://kg.nicolike.cn

[R80] 查看脚本执行耗时
来源：http://wq.9csxet.cn

time ./run.sh
来源：http://wt.yuntaijiaju.cn

================================================================================
来源：http://jh.newstarts.cn

S. C / C++ 专题
来源：http://ar.newstarts.cn

================================================================================
来源：http://ug.asd995.cn

[S01] C：Hello World
来源：http://og.shxzskj.cn

#include <stdio.h>
来源：http://ss.nszjky.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://xh.gzmigu.cn

[S02] C：变量与格式化输出
来源：http://lv.huixiangedu.cn

int a = 10; printf("%d\n", a);
来源：http://qp.shxzskj.cn

[S03] C：读入整数
来源：http://bn.szsharing.cn

int x; scanf("%d", &x);
来源：http://rc.shxzukj.cn

[S04] C：字符串复制
来源：http://dk.jctech888.com.cn

char dst[32]; strcpy(dst, "hi");
来源：http://qw.nicolike.cn

[S05] C：字符串长度
来源：http://hf.chemitech.net.cn

strlen(s)
来源：http://rd.colortex.cn

[S06] C：字符串比较
来源：http://ni.lnxyls.cn

strcmp(a, b) == 0
来源：http://jm.bjjhwx.cn

[S07] C：数组遍历求和
来源：http://en.bookmarksfly.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://ws.newstarts.cn

[S08] C：动态内存分配与释放
来源：http://oz.yuntaijiaju.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ht.colortex.cn

[S09] C：结构体定义与初始化
来源：http://bh.panjiajie.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://jo.chemitech.net.cn

[S10] C：指针与解引用
来源：http://pu.szxytkj.cn

int *p = &a;  *p = 5;
来源：http://ex.521024.cn

[S11] C：逐行读文件
来源：http://ot.521024.cn

FILE *f = fopen("a.txt", "r");
来源：http://li.9csxet.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ad.chemitech.net.cn

fclose(f);
来源：http://eq.bookmarksfly.cn

[S12] C：写文件
来源：http://no.hnjuh.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://qn.hnjuh.cn

[S13] C：宏定义
来源：http://cl.yuntaijiaju.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://eh.nszjky.cn

[S14] C：枚举
来源：http://eu.hahajie.cn

enum Color { RED, GREEN, BLUE };
来源：http://yf.newstarts.cn

[S15] C：类型转换
来源：http://aq.asd995.cn

(double) a / b
来源：http://oh.shxzukj.cn

[S16] C：位操作置位
来源：http://sa.huixiangedu.cn

x |= (1 << 3);
来源：http://nr.newstarts.cn

[S17] C：安全拼接字符串
来源：http://jg.colortex.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ap.newstarts.cn

[S18] C：命令行参数
来源：http://sa.shxzskj.cn

int main(int argc, char **argv)
来源：http://gw.szxytkj.cn

[S19] C：快速排序
来源：http://sp.nszjky.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ja.szsharing.cn

[S20] C：二分查找
来源：http://le.wgjwhj.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://hc.lnxyls.cn

[S21] C：字符类别判断
来源：http://sm.huixinmuqiang.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://jo.nicolike.cn

[S22] C：字符串转数字
来源：http://bu.colortex.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ph.yuexingan06.cn

[S23] C：随机数
来源：http://vp.muxihuayi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ot.gzmigu.cn

[S24] C：获取本地时间
来源：http://mp.chemitech.net.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ii.bjjhwx.cn

[S25] C：内存拷贝
来源：http://wt.bookmarksfly.cn

memcpy(dst, src, n);
来源：http://fr.shxzskj.cn

[S26] C：内存清零
来源：http://ft.bookmarksfly.cn

memset(a, 0, sizeof a);
来源：http://zt.yuntaijiaju.cn

[S27] C：定义常量
来源：http://qk.haigaiapp.cn

const double PI = 3.14159;
来源：http://ro.nszjky.cn

[S28] C：静态变量
来源：http://nd.hnjuh.cn

static int counter = 0;
来源：http://fd.jianghongdianzi.cn

[S29] C：变参函数
来源：http://hs.yuexingan06.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mc.chemitech.net.cn

[S30] C：头文件保护
来源：http://jm.gzmigu.cn

#ifndef X_H
来源：http://pc.panjiajie.cn

#define X_H
来源：http://eg.bookmarksfly.cn

#endif
来源：http://qc.panjiajie.cn

[S31] C++：Hello World
来源：http://ic.szxytkj.cn

#include <iostream>
来源：http://hh.lnxyls.cn

int main() { std::cout << "Hello\n"; }
来源：http://pq.bookmarksfly.cn

[S32] C++：字符串
来源：http://jv.newstarts.cn

std::string s = "hi";  s += "!";
来源：http://kr.shxzukj.cn

[S33] C++：vector 增删
来源：http://kg.haigaiapp.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://sq.jianghongdianzi.cn

[S34] C++：遍历 vector
来源：http://de.9csxet.cn

for (auto &x : v) { std::cout << x; }
来源：http://ui.panjiajie.cn

[S35] C++：map
来源：http://hb.szsharing.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://hl.newstarts.cn

[S36] C++：unordered_map
来源：http://hy.hnjuh.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://dj.huixiangedu.cn

[S37] C++：set
来源：http://bh.asd995.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://mc.jctech888.com.cn

[S38] C++：排序
来源：http://lw.huixiangedu.cn

std::sort(v.begin(), v.end());
来源：http://fa.chemitech.net.cn

[S39] C++：自定义比较器排序
来源：http://ck.nicolike.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://bb.lnxyls.cn

[S40] C++：查找元素
来源：http://aj.yuexingan06.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hv.szsharing.cn

[S41] C++：类与构造函数
来源：http://ew.muxihuayi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://kh.lnxyls.cn

[S42] C++：继承与虚函数
来源：http://so.bjjhwx.cn

class B : public Base { public: void f() override {} };
来源：http://ox.newstarts.cn

[S43] C++：智能指针
来源：http://bz.jctech888.com.cn

auto p = std::make_unique<int>(5);
来源：http://cd.nszjky.cn

[S44] C++：引用传参
来源：http://vv.bookmarksfly.cn

void inc(int &x) { ++x; }
来源：http://pt.huanxung.cn

[S45] C++：lambda
来源：http://un.shxzskj.cn

auto add = [](int a, int b) { return a + b; };
来源：http://gt.szsharing.cn

[S46] C++：函数模板
来源：http://oj.szsharing.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ve.nszjky.cn

[S47] C++：结构化绑定遍历
来源：http://kg.bookmarksfly.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://di.huanxung.cn

[S48] C++：逐行读文件
来源：http://nl.9csxet.cn

std::ifstream in("a.txt");  std::string line;
来源：http://oc.haigaiapp.cn

while (std::getline(in, line)) { }
来源：http://qn.nicolike.cn

[S49] C++：写文件
来源：http://xc.szxytkj.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://rf.huixiangedu.cn

[S50] C++：格式化数字
来源：http://rr.colortex.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://sp.bjjhwx.cn

[S51] C++：显式类型转换
来源：http://vg.huixinmuqiang.cn

static_cast<double>(a) / b
来源：http://zs.nicolike.cn

[S52] C++：const 与 noexcept
来源：http://mw.colortex.cn

int size() const noexcept { return n_; }
来源：http://ja.chemitech.net.cn

[S53] C++：移动语义
来源：http://yp.yuntaijiaju.cn

std::vector<int> w = std::move(v);
来源：http://fk.gzmigu.cn

[S54] C++：异常处理
来源：http://fc.newstarts.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://io.shxzukj.cn

[S55] C++：结构化绑定
来源：http://sf.shxzukj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://yh.lnxyls.cn

[S56] C++：optional
来源：http://gr.shxzskj.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://vu.bjjhwx.cn

[S57] C++：编译期常量
来源：http://eg.lnxyls.cn

constexpr int N = 10;
来源：http://cw.huixinmuqiang.cn

[S58] C++：命名空间
来源：http://va.chemitech.net.cn

namespace ns { int f() { return 1; } }
来源：http://vd.chemitech.net.cn

[S59] C++：静态断言
来源：http://oj.gzmigu.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://cs.lnxyls.cn

[S60] C++：遍历并删除元素
来源：http://sh.521024.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ti.jctech888.com.cn

================================================================================
来源：http://qv.521024.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://uf.chemitech.net.cn

================================================================================
来源：http://zm.shtwfgs.cn

[T01] Kotlin：Hello World
来源：http://hp.yuntaijiaju.cn

println("Hello")
来源：http://sy.newstarts.cn

[T02] Kotlin：变量
来源：http://eq.hnjuh.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ss.shxzskj.cn

[T03] Kotlin：字符串模板
来源：http://ei.gzmigu.cn

"值: $b"
来源：http://fq.shtwfgs.cn

[T04] Kotlin：空安全
来源：http://st.hnjuh.cn

val n: String? = null;  n?.length
来源：http://kc.shtwfgs.cn

[T05] Kotlin：when 表达式
来源：http://vl.gzmigu.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://ly.haigaiapp.cn

[T06] Kotlin：集合映射
来源：http://pq.bookmarksfly.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://rx.haigaiapp.cn

[T07] Kotlin：集合过滤
来源：http://wc.hnjuh.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://mt.asd995.cn

[T08] Kotlin：数据类
来源：http://ar.9csxet.cn

data class User(val name: String, val age: Int)
来源：http://gg.jctech888.com.cn

[T09] Kotlin：扩展函数
来源：http://hp.muxihuayi.cn

fun String.exclaim() = this + "!"
来源：http://gj.521024.cn

[T10] Kotlin：默认参数
来源：http://ho.huixinmuqiang.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ey.bjjhwx.cn

[T11] Kotlin：协程
来源：http://qh.jianghongdianzi.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ye.hnjuh.cn

[T12] Kotlin：解构声明
来源：http://qv.wgjwhj.cn

val (a, b) = Pair(1, 2)
来源：http://xp.bookmarksfly.cn

[T13] Kotlin：只读 Map
来源：http://sq.jianghongdianzi.cn

val m = mapOf("a" to 1)
来源：http://ho.nicolike.cn

[T14] Kotlin：循环
来源：http://bj.shxzukj.cn

for (i in 1..10) println(i)
来源：http://hj.bjjhwx.cn

[T15] Kotlin：接口
来源：http://dl.nszjky.cn

interface Shape { fun area(): Double }
来源：http://fb.wgjwhj.cn

[T16] Swift：Hello World
来源：http://nu.yuntaijiaju.cn

print("Hello")
来源：http://yz.shtwfgs.cn

[T17] Swift：变量与常量
来源：http://kl.huixiangedu.cn

var a = 1;  let b = 2
来源：http://vg.szxytkj.cn

[T18] Swift：字符串插值
来源：http://uk.hnjuh.cn

"值: \(b)"
来源：http://pm.hnjuh.cn

[T19] Swift：可选绑定
来源：http://zl.521024.cn

if let n = opt { print(n) }
来源：http://tm.huixinmuqiang.cn

[T20] Swift：数组操作
来源：http://nf.gzmigu.cn

var a = [1, 2, 3];  a.append(4)
来源：http://iq.szxytkj.cn

[T21] Swift：遍历
来源：http://ro.hnjuh.cn

for x in a { print(x) }
来源：http://mq.panjiajie.cn

[T22] Swift：字典
来源：http://pq.huixiangedu.cn

var d = ["a": 1];  d["b"] = 2
来源：http://kp.szxytkj.cn

[T23] Swift：函数
来源：http://dl.wgjwhj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://oq.hnjuh.cn

[T24] Swift：闭包
来源：http://dc.huixinmuqiang.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ab.jctech888.com.cn

[T25] Swift：结构体
来源：http://cj.colortex.cn

struct P { var x: Int }
来源：http://ei.shxzukj.cn

[T26] Swift：类与重写
来源：http://tw.asd995.cn

class A: Base { override func f() {} }
来源：http://mf.nszjky.cn

[T27] Swift：错误处理
来源：http://vz.bjjhwx.cn

do { try f() } catch { print(error) }
来源：http://wb.yuntaijiaju.cn

[T28] Swift：枚举
来源：http://ow.hahajie.cn

enum Color { case red, green }
来源：http://fw.yuexingan06.cn

[T29] Swift：guard 提前返回
来源：http://yc.haigaiapp.cn

guard let x = opt else { return }
来源：http://vh.bookmarksfly.cn

[T30] Swift：协议
来源：http://vn.bookmarksfly.cn

protocol Shape { func area() -> Double }
来源：http://po.haigaiapp.cn

[T31] Lua：Hello World
来源：http://qh.bookmarksfly.cn

print("Hello")
来源：http://vf.hnjuh.cn

[T32] Lua：局部变量
来源：http://ez.yuntaijiaju.cn

local a = 1
来源：http://kk.9csxet.cn

[T33] Lua：表（数组）
来源：http://id.szsharing.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ub.wgjwhj.cn

[T34] Lua：遍历表
来源：http://yx.haigaiapp.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://on.shtwfgs.cn

[T35] Lua：字典表
来源：http://qx.hnjuh.cn

local d = { a = 1 };  d.b = 2
来源：http://qn.yuexingan06.cn

[T36] Lua：函数
来源：http://kh.newstarts.cn

function add(a, b) return a + b end
来源：http://an.muxihuayi.cn

[T37] Lua：字符串拼接
来源：http://vz.wgjwhj.cn

"a" .. "b"
来源：http://xr.chemitech.net.cn

[T38] Lua：条件
来源：http://jm.bookmarksfly.cn

if x > 0 then print("正") end
来源：http://qv.shxzukj.cn

[T39] Lua：模式匹配
来源：http://tp.chemitech.net.cn

string.find(s, "%d+")
来源：http://pe.bjjhwx.cn

[T40] Lua：元表
来源：http://mq.bjjhwx.cn

setmetatable({}, { __index = base })
来源：http://pg.huanxung.cn

[T41] Perl：Hello World
来源：http://mo.asd995.cn

print "Hello\n";
来源：http://jn.szxytkj.cn

[T42] Perl：变量类型
来源：http://zk.shxzukj.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ol.9csxet.cn

[T43] Perl：字符串插值
来源：http://bs.hahajie.cn

"值: $a"
来源：http://rt.huanxung.cn

[T44] Perl：条件
来源：http://ga.shxzskj.cn

if ($a > 0) { print "正"; }
来源：http://lm.newstarts.cn

[T45] Perl：数组遍历
来源：http://ft.bjjhwx.cn

for my $x (@arr) { print $x; }
来源：http://yq.asd995.cn

[T46] Perl：哈希操作
来源：http://uy.bjjhwx.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://tp.chemitech.net.cn

[T47] Perl：正则捕获
来源：http://gh.szsharing.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ir.521024.cn

[T48] Perl：正则替换
来源：http://iz.muxihuayi.cn

$s =~ s/old/new/g;
来源：http://zl.yuexingan06.cn


<!-- 参考信息 -->