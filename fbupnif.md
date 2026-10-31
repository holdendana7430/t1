代发 wailian999

find . -name "*.tmp" -delete
来源：http://jr.lnxyls.cn

[R46] 递归替换文件内容
来源：http://ui.shxzukj.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://qw.lnxyls.cn

[R47] sed 单行替换
来源：http://iw.asd995.cn

sed -i 's/foo/bar/g' a.txt
来源：http://vm.nicolike.cn

[R48] awk 取指定列
来源：http://dg.huixinmuqiang.cn

awk '{print $1, $3}' a.txt
来源：http://un.chemitech.net.cn

[R49] awk 带条件
来源：http://rb.521024.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ks.hnjuh.cn

[R50] awk 求和
来源：http://jk.gzmigu.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ql.asd995.cn

[R51] 排序去重取前几
来源：http://bt.haigaiapp.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://dw.szsharing.cn

[R52] 统计行数
来源：http://yz.huixinmuqiang.cn

wc -l a.txt
来源：http://eb.muxihuayi.cn

[R53] 查看文件头与实时尾
来源：http://ja.shtwfgs.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://gk.muxihuayi.cn

[R54] 比较两个文件
来源：http://nt.nicolike.cn

diff a.txt b.txt
来源：http://dm.9csxet.cn

[R55] 压缩与解压
来源：http://xl.bookmarksfly.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ab.haigaiapp.cn

[R56] 远程拷贝
来源：http://zk.9csxet.cn

scp file user@host:/path/
来源：http://jf.colortex.cn

[R57] 远程执行命令
来源：http://vn.muxihuayi.cn

ssh user@host 'uptime'
来源：http://ff.huanxung.cn

[R58] 下载文件
来源：http://mj.hahajie.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://ef.jctech888.com.cn

[R59] 发 POST JSON
来源：http://uc.shtwfgs.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ua.shxzskj.cn

[R60] 只看 HTTP 状态码
来源：http://hi.muxihuayi.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://in.szsharing.cn

[R61] 磁盘占用
来源：http://bp.jctech888.com.cn

df -h;  du -sh *
来源：http://id.szxytkj.cn

[R62] 找最占空间的文件
来源：http://xg.wgjwhj.cn

du -ah . | sort -rh | head -10
来源：http://ld.haigaiapp.cn

[R63] 内存与进程
来源：http://um.shxzukj.cn

free -h;  ps aux | grep nginx
来源：http://qv.shtwfgs.cn

[R64] 结束进程
来源：http://ck.colortex.cn

kill -9 $(pgrep -f app.py)
来源：http://wt.bjjhwx.cn

[R65] 查看端口占用
来源：http://ax.nszjky.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://fs.yuexingan06.cn

[R66] 定时任务
来源：http://xe.nicolike.cn

crontab -e;  crontab -l
来源：http://by.panjiajie.cn

[R67] 生成随机十六进制串
来源：http://hp.yuntaijiaju.cn

openssl rand -hex 16
来源：http://vc.lnxyls.cn

[R68] 计算文件校验值
来源：http://ps.jianghongdianzi.cn

sha256sum a.txt;  md5sum a.txt
来源：http://qm.szsharing.cn

[R69] 生成随机密码
来源：http://rz.szsharing.cn

head -c 16 /dev/urandom | base64
来源：http://cl.yuexingan06.cn

[R70] 时间戳与互转
来源：http://zk.yuexingan06.cn

date +%s;  date -d @1700000000
来源：http://oy.wgjwhj.cn

[R71] 日期格式化
来源：http://ae.shtwfgs.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://tq.9csxet.cn

[R72] 等待端口就绪
来源：http://wt.huixiangedu.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://sg.hahajie.cn

[R73] 分割大日志
来源：http://dy.nszjky.cn

split -l 1000 big.log part_
来源：http://cr.gzmigu.cn

[R74] 批量重命名
来源：http://sc.newstarts.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://qu.wgjwhj.cn

[R75] 导出环境变量
来源：http://fk.shxzskj.cn

export PATH="$HOME/bin:$PATH"
来源：http://vl.yuntaijiaju.cn

[R76] 使用临时文件
来源：http://kh.shtwfgs.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://jt.shxzukj.cn

[R77] 读取用户输入
来源：http://tl.szsharing.cn

read -rp "请输入: " ans
来源：http://id.hnjuh.cn

[R78] 交互式菜单
来源：http://kt.521024.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://sz.huixiangedu.cn

[R79] 解析命令行选项
来源：http://xh.jianghongdianzi.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://jy.521024.cn

[R80] 查看脚本执行耗时
来源：http://ca.colortex.cn

time ./run.sh
来源：http://bd.chemitech.net.cn

================================================================================
来源：http://yp.lnxyls.cn

S. C / C++ 专题
来源：http://rx.hnjuh.cn

================================================================================
来源：http://jd.bjjhwx.cn

[S01] C：Hello World
来源：http://gb.yuntaijiaju.cn

#include <stdio.h>
来源：http://vk.muxihuayi.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://zd.nszjky.cn

[S02] C：变量与格式化输出
来源：http://ji.hnjuh.cn

int a = 10; printf("%d\n", a);
来源：http://jf.yuexingan06.cn

[S03] C：读入整数
来源：http://wy.nszjky.cn

int x; scanf("%d", &x);
来源：http://lx.haigaiapp.cn

[S04] C：字符串复制
来源：http://pb.yuntaijiaju.cn

char dst[32]; strcpy(dst, "hi");
来源：http://yg.nicolike.cn

[S05] C：字符串长度
来源：http://dn.asd995.cn

strlen(s)
来源：http://mb.bookmarksfly.cn

[S06] C：字符串比较
来源：http://xe.muxihuayi.cn

strcmp(a, b) == 0
来源：http://yj.yuexingan06.cn

[S07] C：数组遍历求和
来源：http://sb.wgjwhj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://na.gzmigu.cn

[S08] C：动态内存分配与释放
来源：http://gw.szsharing.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://fk.yuntaijiaju.cn

[S09] C：结构体定义与初始化
来源：http://yp.haigaiapp.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://tq.hahajie.cn

[S10] C：指针与解引用
来源：http://ww.wgjwhj.cn

int *p = &a;  *p = 5;
来源：http://cs.nicolike.cn

[S11] C：逐行读文件
来源：http://pt.huanxung.cn

FILE *f = fopen("a.txt", "r");
来源：http://kl.shxzskj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ec.gzmigu.cn

fclose(f);
来源：http://qa.hahajie.cn

[S12] C：写文件
来源：http://ip.jctech888.com.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://vx.jctech888.com.cn

[S13] C：宏定义
来源：http://ib.hahajie.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://gv.shtwfgs.cn

[S14] C：枚举
来源：http://kh.nszjky.cn

enum Color { RED, GREEN, BLUE };
来源：http://bh.yuntaijiaju.cn

[S15] C：类型转换
来源：http://pq.haigaiapp.cn

(double) a / b
来源：http://mh.yuntaijiaju.cn

[S16] C：位操作置位
来源：http://qx.newstarts.cn

x |= (1 << 3);
来源：http://cz.szsharing.cn

[S17] C：安全拼接字符串
来源：http://uc.yuntaijiaju.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ef.jianghongdianzi.cn

[S18] C：命令行参数
来源：http://qi.yuntaijiaju.cn

int main(int argc, char **argv)
来源：http://vz.muxihuayi.cn

[S19] C：快速排序
来源：http://zb.szxytkj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ap.haigaiapp.cn

[S20] C：二分查找
来源：http://zw.yuexingan06.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://rf.hnjuh.cn

[S21] C：字符类别判断
来源：http://vk.nicolike.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://it.huanxung.cn

[S22] C：字符串转数字
来源：http://pk.panjiajie.cn

atoi("42");  strtod("3.14", NULL);
来源：http://dw.yuexingan06.cn

[S23] C：随机数
来源：http://lb.huanxung.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ee.huixiangedu.cn

[S24] C：获取本地时间
来源：http://ak.lnxyls.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://sj.hnjuh.cn

[S25] C：内存拷贝
来源：http://mo.chemitech.net.cn

memcpy(dst, src, n);
来源：http://hd.asd995.cn

[S26] C：内存清零
来源：http://vi.hnjuh.cn

memset(a, 0, sizeof a);
来源：http://ll.haigaiapp.cn

[S27] C：定义常量
来源：http://bf.nicolike.cn

const double PI = 3.14159;
来源：http://ho.jianghongdianzi.cn

[S28] C：静态变量
来源：http://jf.huixinmuqiang.cn

static int counter = 0;
来源：http://kb.nicolike.cn

[S29] C：变参函数
来源：http://to.muxihuayi.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://bn.hahajie.cn

[S30] C：头文件保护
来源：http://il.wgjwhj.cn

#ifndef X_H
来源：http://rq.muxihuayi.cn

#define X_H
来源：http://gn.wgjwhj.cn

#endif
来源：http://hk.chemitech.net.cn

[S31] C++：Hello World
来源：http://ky.jianghongdianzi.cn

#include <iostream>
来源：http://mx.panjiajie.cn

int main() { std::cout << "Hello\n"; }
来源：http://ev.bjjhwx.cn

[S32] C++：字符串
来源：http://uf.bookmarksfly.cn

std::string s = "hi";  s += "!";
来源：http://mo.jianghongdianzi.cn

[S33] C++：vector 增删
来源：http://dp.gzmigu.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://zs.huanxung.cn

[S34] C++：遍历 vector
来源：http://gc.hahajie.cn

for (auto &x : v) { std::cout << x; }
来源：http://gv.szxytkj.cn

[S35] C++：map
来源：http://bx.huanxung.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ww.szsharing.cn

[S36] C++：unordered_map
来源：http://af.lnxyls.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://gz.gzmigu.cn

[S37] C++：set
来源：http://gf.huanxung.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://fr.yuexingan06.cn

[S38] C++：排序
来源：http://za.szxytkj.cn

std::sort(v.begin(), v.end());
来源：http://nj.bookmarksfly.cn

[S39] C++：自定义比较器排序
来源：http://fe.asd995.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://rp.chemitech.net.cn

[S40] C++：查找元素
来源：http://fy.huixiangedu.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://jt.szxytkj.cn

[S41] C++：类与构造函数
来源：http://kn.colortex.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ay.shtwfgs.cn

[S42] C++：继承与虚函数
来源：http://ws.huixiangedu.cn

class B : public Base { public: void f() override {} };
来源：http://af.szsharing.cn

[S43] C++：智能指针
来源：http://li.huixiangedu.cn

auto p = std::make_unique<int>(5);
来源：http://of.521024.cn

[S44] C++：引用传参
来源：http://nl.muxihuayi.cn

void inc(int &x) { ++x; }
来源：http://ng.newstarts.cn

[S45] C++：lambda
来源：http://wr.huixiangedu.cn

auto add = [](int a, int b) { return a + b; };
来源：http://vx.szxytkj.cn

[S46] C++：函数模板
来源：http://mi.bookmarksfly.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://op.szsharing.cn

[S47] C++：结构化绑定遍历
来源：http://mj.jctech888.com.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://yv.hnjuh.cn

[S48] C++：逐行读文件
来源：http://qp.yuntaijiaju.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ux.gzmigu.cn

while (std::getline(in, line)) { }
来源：http://ys.colortex.cn

[S49] C++：写文件
来源：http://tv.muxihuayi.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://lo.muxihuayi.cn

[S50] C++：格式化数字
来源：http://zf.shxzskj.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ff.asd995.cn

[S51] C++：显式类型转换
来源：http://wz.nszjky.cn

static_cast<double>(a) / b
来源：http://wt.szxytkj.cn

[S52] C++：const 与 noexcept
来源：http://po.shtwfgs.cn

int size() const noexcept { return n_; }
来源：http://na.hahajie.cn

[S53] C++：移动语义
来源：http://si.521024.cn

std::vector<int> w = std::move(v);
来源：http://ts.muxihuayi.cn

[S54] C++：异常处理
来源：http://zg.shtwfgs.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://tt.chemitech.net.cn

[S55] C++：结构化绑定
来源：http://es.shtwfgs.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://bp.chemitech.net.cn

[S56] C++：optional
来源：http://pj.huanxung.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ye.bjjhwx.cn

[S57] C++：编译期常量
来源：http://me.szsharing.cn

constexpr int N = 10;
来源：http://ho.jctech888.com.cn

[S58] C++：命名空间
来源：http://wc.huanxung.cn

namespace ns { int f() { return 1; } }
来源：http://px.shxzukj.cn

[S59] C++：静态断言
来源：http://xx.gzmigu.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://pr.gzmigu.cn

[S60] C++：遍历并删除元素
来源：http://wt.wgjwhj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://bl.hahajie.cn

================================================================================
来源：http://qz.asd995.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://sk.newstarts.cn

================================================================================
来源：http://cn.shtwfgs.cn

[T01] Kotlin：Hello World
来源：http://lh.szsharing.cn

println("Hello")
来源：http://rl.haigaiapp.cn

[T02] Kotlin：变量
来源：http://dw.newstarts.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://yz.nszjky.cn

[T03] Kotlin：字符串模板
来源：http://gd.szsharing.cn

"值: $b"
来源：http://sy.colortex.cn

[T04] Kotlin：空安全
来源：http://xn.muxihuayi.cn

val n: String? = null;  n?.length
来源：http://ib.huanxung.cn

[T05] Kotlin：when 表达式
来源：http://ar.colortex.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://yt.yuexingan06.cn

[T06] Kotlin：集合映射
来源：http://vg.nicolike.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://ml.jianghongdianzi.cn

[T07] Kotlin：集合过滤
来源：http://jf.bookmarksfly.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ht.huixiangedu.cn

[T08] Kotlin：数据类
来源：http://uk.hahajie.cn

data class User(val name: String, val age: Int)
来源：http://sa.9csxet.cn

[T09] Kotlin：扩展函数
来源：http://ws.newstarts.cn

fun String.exclaim() = this + "!"
来源：http://df.yuntaijiaju.cn

[T10] Kotlin：默认参数
来源：http://st.szxytkj.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://qg.shxzukj.cn

[T11] Kotlin：协程
来源：http://bp.huixinmuqiang.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://by.hnjuh.cn

[T12] Kotlin：解构声明
来源：http://pw.chemitech.net.cn

val (a, b) = Pair(1, 2)
来源：http://xw.wgjwhj.cn

[T13] Kotlin：只读 Map
来源：http://gk.haigaiapp.cn

val m = mapOf("a" to 1)
来源：http://qn.huixinmuqiang.cn

[T14] Kotlin：循环
来源：http://pv.szxytkj.cn

for (i in 1..10) println(i)
来源：http://ew.shxzukj.cn

[T15] Kotlin：接口
来源：http://pe.bjjhwx.cn

interface Shape { fun area(): Double }
来源：http://pn.szsharing.cn

[T16] Swift：Hello World
来源：http://ar.asd995.cn

print("Hello")
来源：http://yn.colortex.cn

[T17] Swift：变量与常量
来源：http://sr.muxihuayi.cn

var a = 1;  let b = 2
来源：http://oh.asd995.cn

[T18] Swift：字符串插值
来源：http://yd.lnxyls.cn

"值: \(b)"
来源：http://na.shtwfgs.cn

[T19] Swift：可选绑定
来源：http://qh.521024.cn

if let n = opt { print(n) }
来源：http://mh.colortex.cn

[T20] Swift：数组操作
来源：http://ei.szsharing.cn

var a = [1, 2, 3];  a.append(4)
来源：http://lh.shtwfgs.cn

[T21] Swift：遍历
来源：http://wg.gzmigu.cn

for x in a { print(x) }
来源：http://ig.huixinmuqiang.cn

[T22] Swift：字典
来源：http://lg.newstarts.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ns.hnjuh.cn

[T23] Swift：函数
来源：http://kd.colortex.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://yi.newstarts.cn

[T24] Swift：闭包
来源：http://kf.colortex.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://zf.haigaiapp.cn

[T25] Swift：结构体
来源：http://zv.hnjuh.cn

struct P { var x: Int }
来源：http://ms.lnxyls.cn

[T26] Swift：类与重写
来源：http://jb.bookmarksfly.cn

class A: Base { override func f() {} }
来源：http://gt.yuntaijiaju.cn

[T27] Swift：错误处理
来源：http://he.huixiangedu.cn

do { try f() } catch { print(error) }
来源：http://my.shtwfgs.cn

[T28] Swift：枚举
来源：http://wr.huixinmuqiang.cn

enum Color { case red, green }
来源：http://gs.shxzukj.cn

[T29] Swift：guard 提前返回
来源：http://vh.lnxyls.cn

guard let x = opt else { return }
来源：http://vj.asd995.cn

[T30] Swift：协议
来源：http://gp.chemitech.net.cn

protocol Shape { func area() -> Double }
来源：http://bj.huanxung.cn

[T31] Lua：Hello World
来源：http://wz.nicolike.cn

print("Hello")
来源：http://ct.bjjhwx.cn

[T32] Lua：局部变量
来源：http://yw.szxytkj.cn

local a = 1
来源：http://uc.bookmarksfly.cn

[T33] Lua：表（数组）
来源：http://gl.szsharing.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://dt.yuntaijiaju.cn

[T34] Lua：遍历表
来源：http://iw.9csxet.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://if.hnjuh.cn

[T35] Lua：字典表
来源：http://fb.shxzskj.cn

local d = { a = 1 };  d.b = 2
来源：http://jk.lnxyls.cn

[T36] Lua：函数
来源：http://xe.chemitech.net.cn

function add(a, b) return a + b end
来源：http://oy.colortex.cn

[T37] Lua：字符串拼接
来源：http://tj.huixinmuqiang.cn

"a" .. "b"
来源：http://ji.colortex.cn

[T38] Lua：条件
来源：http://pk.jctech888.com.cn

if x > 0 then print("正") end
来源：http://to.gzmigu.cn

[T39] Lua：模式匹配
来源：http://uz.bjjhwx.cn

string.find(s, "%d+")
来源：http://ww.asd995.cn

[T40] Lua：元表
来源：http://vb.muxihuayi.cn

setmetatable({}, { __index = base })
来源：http://mw.521024.cn

[T41] Perl：Hello World
来源：http://vd.bookmarksfly.cn

print "Hello\n";
来源：http://lf.asd995.cn

[T42] Perl：变量类型
来源：http://ri.nszjky.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://sn.muxihuayi.cn

[T43] Perl：字符串插值
来源：http://kk.lnxyls.cn

"值: $a"
来源：http://xf.yuntaijiaju.cn

[T44] Perl：条件
来源：http://iy.chemitech.net.cn

if ($a > 0) { print "正"; }
来源：http://ei.9csxet.cn

[T45] Perl：数组遍历
来源：http://iv.chemitech.net.cn

for my $x (@arr) { print $x; }
来源：http://wp.asd995.cn

[T46] Perl：哈希操作
来源：http://qb.newstarts.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://bg.muxihuayi.cn

[T47] Perl：正则捕获
来源：http://up.panjiajie.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://fh.9csxet.cn

[T48] Perl：正则替换
来源：http://fs.gzmigu.cn

$s =~ s/old/new/g;
来源：http://zm.yuntaijiaju.cn


<!-- 参考信息 -->