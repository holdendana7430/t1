代发 wailian999

sed -i 's/foo/bar/g' a.txt
来源：http://dv.muxihuayi.cn

[R48] awk 取指定列
来源：http://xh.szsharing.cn

awk '{print $1, $3}' a.txt
来源：http://bi.gzmigu.cn

[R49] awk 带条件
来源：http://uv.wgjwhj.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://ng.hahajie.cn

[R50] awk 求和
来源：http://tm.521024.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ym.szxytkj.cn

[R51] 排序去重取前几
来源：http://tn.gzmigu.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://px.newstarts.cn

[R52] 统计行数
来源：http://mz.shxzukj.cn

wc -l a.txt
来源：http://zu.huixinmuqiang.cn

[R53] 查看文件头与实时尾
来源：http://tp.bjjhwx.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ja.yuntaijiaju.cn

[R54] 比较两个文件
来源：http://pj.szxytkj.cn

diff a.txt b.txt
来源：http://we.wgjwhj.cn

[R55] 压缩与解压
来源：http://du.bookmarksfly.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://xt.newstarts.cn

[R56] 远程拷贝
来源：http://fz.gzmigu.cn

scp file user@host:/path/
来源：http://wz.521024.cn

[R57] 远程执行命令
来源：http://fl.hnjuh.cn

ssh user@host 'uptime'
来源：http://tq.huanxung.cn

[R58] 下载文件
来源：http://qd.nszjky.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://pq.panjiajie.cn

[R59] 发 POST JSON
来源：http://no.chemitech.net.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ye.szxytkj.cn

[R60] 只看 HTTP 状态码
来源：http://ha.newstarts.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://rz.newstarts.cn

[R61] 磁盘占用
来源：http://xs.shxzukj.cn

df -h;  du -sh *
来源：http://av.huixiangedu.cn

[R62] 找最占空间的文件
来源：http://rt.wgjwhj.cn

du -ah . | sort -rh | head -10
来源：http://jk.bjjhwx.cn

[R63] 内存与进程
来源：http://jg.huixinmuqiang.cn

free -h;  ps aux | grep nginx
来源：http://vi.bookmarksfly.cn

[R64] 结束进程
来源：http://zk.szxytkj.cn

kill -9 $(pgrep -f app.py)
来源：http://fy.yuntaijiaju.cn

[R65] 查看端口占用
来源：http://wm.haigaiapp.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hr.nszjky.cn

[R66] 定时任务
来源：http://tk.nszjky.cn

crontab -e;  crontab -l
来源：http://uz.jctech888.com.cn

[R67] 生成随机十六进制串
来源：http://th.yuexingan06.cn

openssl rand -hex 16
来源：http://ft.jianghongdianzi.cn

[R68] 计算文件校验值
来源：http://wc.szxytkj.cn

sha256sum a.txt;  md5sum a.txt
来源：http://fu.bjjhwx.cn

[R69] 生成随机密码
来源：http://ci.chemitech.net.cn

head -c 16 /dev/urandom | base64
来源：http://am.huixiangedu.cn

[R70] 时间戳与互转
来源：http://hl.9csxet.cn

date +%s;  date -d @1700000000
来源：http://fn.9csxet.cn

[R71] 日期格式化
来源：http://ep.gzmigu.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://ca.muxihuayi.cn

[R72] 等待端口就绪
来源：http://yh.yuntaijiaju.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ib.jctech888.com.cn

[R73] 分割大日志
来源：http://fl.jctech888.com.cn

split -l 1000 big.log part_
来源：http://ca.lnxyls.cn

[R74] 批量重命名
来源：http://bz.shtwfgs.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://bv.9csxet.cn

[R75] 导出环境变量
来源：http://hf.jianghongdianzi.cn

export PATH="$HOME/bin:$PATH"
来源：http://aq.panjiajie.cn

[R76] 使用临时文件
来源：http://bd.wgjwhj.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://qx.gzmigu.cn

[R77] 读取用户输入
来源：http://nz.bookmarksfly.cn

read -rp "请输入: " ans
来源：http://ip.asd995.cn

[R78] 交互式菜单
来源：http://mt.szsharing.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://nt.wgjwhj.cn

[R79] 解析命令行选项
来源：http://zm.chemitech.net.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://vg.nszjky.cn

[R80] 查看脚本执行耗时
来源：http://il.lnxyls.cn

time ./run.sh
来源：http://ve.jianghongdianzi.cn

================================================================================
来源：http://mj.bookmarksfly.cn

S. C / C++ 专题
来源：http://kl.szsharing.cn

================================================================================
来源：http://qz.jctech888.com.cn

[S01] C：Hello World
来源：http://mh.yuexingan06.cn

#include <stdio.h>
来源：http://jr.asd995.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://fz.colortex.cn

[S02] C：变量与格式化输出
来源：http://iw.panjiajie.cn

int a = 10; printf("%d\n", a);
来源：http://ec.lnxyls.cn

[S03] C：读入整数
来源：http://ue.hahajie.cn

int x; scanf("%d", &x);
来源：http://te.lnxyls.cn

[S04] C：字符串复制
来源：http://zb.muxihuayi.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ie.huanxung.cn

[S05] C：字符串长度
来源：http://ig.bjjhwx.cn

strlen(s)
来源：http://yd.yuntaijiaju.cn

[S06] C：字符串比较
来源：http://te.haigaiapp.cn

strcmp(a, b) == 0
来源：http://yg.jctech888.com.cn

[S07] C：数组遍历求和
来源：http://qt.colortex.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://hs.panjiajie.cn

[S08] C：动态内存分配与释放
来源：http://tf.yuntaijiaju.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://sr.9csxet.cn

[S09] C：结构体定义与初始化
来源：http://qz.hahajie.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://lw.shxzukj.cn

[S10] C：指针与解引用
来源：http://ma.lnxyls.cn

int *p = &a;  *p = 5;
来源：http://yk.panjiajie.cn

[S11] C：逐行读文件
来源：http://xo.hnjuh.cn

FILE *f = fopen("a.txt", "r");
来源：http://oy.wgjwhj.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://yn.chemitech.net.cn

fclose(f);
来源：http://gk.newstarts.cn

[S12] C：写文件
来源：http://nl.chemitech.net.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://tc.colortex.cn

[S13] C：宏定义
来源：http://hn.jctech888.com.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://sz.gzmigu.cn

[S14] C：枚举
来源：http://ui.newstarts.cn

enum Color { RED, GREEN, BLUE };
来源：http://ez.colortex.cn

[S15] C：类型转换
来源：http://ai.asd995.cn

(double) a / b
来源：http://tm.521024.cn

[S16] C：位操作置位
来源：http://ku.huixinmuqiang.cn

x |= (1 << 3);
来源：http://sr.gzmigu.cn

[S17] C：安全拼接字符串
来源：http://ro.newstarts.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://fj.521024.cn

[S18] C：命令行参数
来源：http://gz.shxzskj.cn

int main(int argc, char **argv)
来源：http://xt.huanxung.cn

[S19] C：快速排序
来源：http://lf.wgjwhj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://so.szxytkj.cn

[S20] C：二分查找
来源：http://sx.lnxyls.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://cm.jctech888.com.cn

[S21] C：字符类别判断
来源：http://nn.hnjuh.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ze.yuexingan06.cn

[S22] C：字符串转数字
来源：http://fp.lnxyls.cn

atoi("42");  strtod("3.14", NULL);
来源：http://qp.haigaiapp.cn

[S23] C：随机数
来源：http://rd.szxytkj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://fv.nicolike.cn

[S24] C：获取本地时间
来源：http://em.bookmarksfly.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://bo.szsharing.cn

[S25] C：内存拷贝
来源：http://to.gzmigu.cn

memcpy(dst, src, n);
来源：http://fk.huanxung.cn

[S26] C：内存清零
来源：http://ny.gzmigu.cn

memset(a, 0, sizeof a);
来源：http://wg.521024.cn

[S27] C：定义常量
来源：http://oe.yuntaijiaju.cn

const double PI = 3.14159;
来源：http://gn.newstarts.cn

[S28] C：静态变量
来源：http://qo.muxihuayi.cn

static int counter = 0;
来源：http://oe.chemitech.net.cn

[S29] C：变参函数
来源：http://nt.muxihuayi.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hm.hnjuh.cn

[S30] C：头文件保护
来源：http://fi.jianghongdianzi.cn

#ifndef X_H
来源：http://xo.lnxyls.cn

#define X_H
来源：http://gz.shxzskj.cn

#endif
来源：http://yk.yuntaijiaju.cn

[S31] C++：Hello World
来源：http://vq.haigaiapp.cn

#include <iostream>
来源：http://zp.huanxung.cn

int main() { std::cout << "Hello\n"; }
来源：http://le.muxihuayi.cn

[S32] C++：字符串
来源：http://mc.nszjky.cn

std::string s = "hi";  s += "!";
来源：http://cm.nicolike.cn

[S33] C++：vector 增删
来源：http://xh.newstarts.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://zm.gzmigu.cn

[S34] C++：遍历 vector
来源：http://gt.muxihuayi.cn

for (auto &x : v) { std::cout << x; }
来源：http://hq.chemitech.net.cn

[S35] C++：map
来源：http://bh.nszjky.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mu.nicolike.cn

[S36] C++：unordered_map
来源：http://pb.shxzukj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://jt.jctech888.com.cn

[S37] C++：set
来源：http://tm.shxzskj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ma.yuexingan06.cn

[S38] C++：排序
来源：http://cx.nicolike.cn

std::sort(v.begin(), v.end());
来源：http://hn.shxzukj.cn

[S39] C++：自定义比较器排序
来源：http://er.wgjwhj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://kq.shxzukj.cn

[S40] C++：查找元素
来源：http://hx.huixinmuqiang.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://ok.521024.cn

[S41] C++：类与构造函数
来源：http://fw.yuexingan06.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ge.9csxet.cn

[S42] C++：继承与虚函数
来源：http://me.hnjuh.cn

class B : public Base { public: void f() override {} };
来源：http://tr.yuexingan06.cn

[S43] C++：智能指针
来源：http://ci.shxzukj.cn

auto p = std::make_unique<int>(5);
来源：http://jg.hnjuh.cn

[S44] C++：引用传参
来源：http://lg.huixiangedu.cn

void inc(int &x) { ++x; }
来源：http://zc.huanxung.cn

[S45] C++：lambda
来源：http://lg.wgjwhj.cn

auto add = [](int a, int b) { return a + b; };
来源：http://kf.nicolike.cn

[S46] C++：函数模板
来源：http://fe.hahajie.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://sf.yuexingan06.cn

[S47] C++：结构化绑定遍历
来源：http://le.bookmarksfly.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://tk.nszjky.cn

[S48] C++：逐行读文件
来源：http://pa.yuntaijiaju.cn

std::ifstream in("a.txt");  std::string line;
来源：http://ov.chemitech.net.cn

while (std::getline(in, line)) { }
来源：http://ir.huixiangedu.cn

[S49] C++：写文件
来源：http://ky.hnjuh.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://hz.newstarts.cn

[S50] C++：格式化数字
来源：http://ef.jianghongdianzi.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://xo.shtwfgs.cn

[S51] C++：显式类型转换
来源：http://sc.panjiajie.cn

static_cast<double>(a) / b
来源：http://ww.szsharing.cn

[S52] C++：const 与 noexcept
来源：http://hz.szxytkj.cn

int size() const noexcept { return n_; }
来源：http://wp.szsharing.cn

[S53] C++：移动语义
来源：http://mf.colortex.cn

std::vector<int> w = std::move(v);
来源：http://nq.jctech888.com.cn

[S54] C++：异常处理
来源：http://sx.huixiangedu.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://kn.yuntaijiaju.cn

[S55] C++：结构化绑定
来源：http://gs.jianghongdianzi.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ij.lnxyls.cn

[S56] C++：optional
来源：http://fh.huanxung.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://zb.yuexingan06.cn

[S57] C++：编译期常量
来源：http://mn.haigaiapp.cn

constexpr int N = 10;
来源：http://yq.jianghongdianzi.cn

[S58] C++：命名空间
来源：http://nx.colortex.cn

namespace ns { int f() { return 1; } }
来源：http://oq.bookmarksfly.cn

[S59] C++：静态断言
来源：http://sb.lnxyls.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://kc.asd995.cn

[S60] C++：遍历并删除元素
来源：http://dq.nicolike.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://gr.huixinmuqiang.cn

================================================================================
来源：http://li.chemitech.net.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://ma.gzmigu.cn

================================================================================
来源：http://yh.nszjky.cn

[T01] Kotlin：Hello World
来源：http://xv.huixiangedu.cn

println("Hello")
来源：http://wd.lnxyls.cn

[T02] Kotlin：变量
来源：http://uk.haigaiapp.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ia.lnxyls.cn

[T03] Kotlin：字符串模板
来源：http://tb.521024.cn

"值: $b"
来源：http://bj.nszjky.cn

[T04] Kotlin：空安全
来源：http://ku.szxytkj.cn

val n: String? = null;  n?.length
来源：http://xc.chemitech.net.cn

[T05] Kotlin：when 表达式
来源：http://fe.chemitech.net.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://eh.szsharing.cn

[T06] Kotlin：集合映射
来源：http://fs.colortex.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://nq.9csxet.cn

[T07] Kotlin：集合过滤
来源：http://ha.shxzskj.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://pl.colortex.cn

[T08] Kotlin：数据类
来源：http://ug.muxihuayi.cn

data class User(val name: String, val age: Int)
来源：http://ca.szsharing.cn

[T09] Kotlin：扩展函数
来源：http://lt.szxytkj.cn

fun String.exclaim() = this + "!"
来源：http://hf.huanxung.cn

[T10] Kotlin：默认参数
来源：http://ll.bjjhwx.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ay.yuntaijiaju.cn

[T11] Kotlin：协程
来源：http://wk.szsharing.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://sd.newstarts.cn

[T12] Kotlin：解构声明
来源：http://ck.yuexingan06.cn

val (a, b) = Pair(1, 2)
来源：http://sa.huixinmuqiang.cn

[T13] Kotlin：只读 Map
来源：http://om.521024.cn

val m = mapOf("a" to 1)
来源：http://hy.lnxyls.cn

[T14] Kotlin：循环
来源：http://wx.asd995.cn

for (i in 1..10) println(i)
来源：http://rk.panjiajie.cn

[T15] Kotlin：接口
来源：http://bk.szsharing.cn

interface Shape { fun area(): Double }
来源：http://xi.asd995.cn

[T16] Swift：Hello World
来源：http://nf.bjjhwx.cn

print("Hello")
来源：http://ri.huixinmuqiang.cn

[T17] Swift：变量与常量
来源：http://cw.nszjky.cn

var a = 1;  let b = 2
来源：http://vo.jctech888.com.cn

[T18] Swift：字符串插值
来源：http://yz.yuexingan06.cn

"值: \(b)"
来源：http://ud.jctech888.com.cn

[T19] Swift：可选绑定
来源：http://ta.shxzukj.cn

if let n = opt { print(n) }
来源：http://rt.bjjhwx.cn

[T20] Swift：数组操作
来源：http://ai.nszjky.cn

var a = [1, 2, 3];  a.append(4)
来源：http://qo.szxytkj.cn

[T21] Swift：遍历
来源：http://kj.chemitech.net.cn

for x in a { print(x) }
来源：http://rm.hnjuh.cn

[T22] Swift：字典
来源：http://jt.9csxet.cn

var d = ["a": 1];  d["b"] = 2
来源：http://jf.jianghongdianzi.cn

[T23] Swift：函数
来源：http://pg.9csxet.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://kg.yuntaijiaju.cn

[T24] Swift：闭包
来源：http://yf.hnjuh.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://cq.haigaiapp.cn

[T25] Swift：结构体
来源：http://te.jctech888.com.cn

struct P { var x: Int }
来源：http://dk.newstarts.cn

[T26] Swift：类与重写
来源：http://fy.huixinmuqiang.cn

class A: Base { override func f() {} }
来源：http://so.shxzukj.cn

[T27] Swift：错误处理
来源：http://yb.colortex.cn

do { try f() } catch { print(error) }
来源：http://am.nszjky.cn

[T28] Swift：枚举
来源：http://hl.gzmigu.cn

enum Color { case red, green }
来源：http://wt.yuexingan06.cn

[T29] Swift：guard 提前返回
来源：http://vc.yuntaijiaju.cn

guard let x = opt else { return }
来源：http://rt.szxytkj.cn

[T30] Swift：协议
来源：http://cq.jianghongdianzi.cn

protocol Shape { func area() -> Double }
来源：http://hl.muxihuayi.cn

[T31] Lua：Hello World
来源：http://fb.panjiajie.cn

print("Hello")
来源：http://oa.wgjwhj.cn

[T32] Lua：局部变量
来源：http://gp.muxihuayi.cn

local a = 1
来源：http://up.9csxet.cn

[T33] Lua：表（数组）
来源：http://en.asd995.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://ty.521024.cn

[T34] Lua：遍历表
来源：http://yy.gzmigu.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://st.shxzukj.cn

[T35] Lua：字典表
来源：http://tg.nszjky.cn

local d = { a = 1 };  d.b = 2
来源：http://rj.lnxyls.cn

[T36] Lua：函数
来源：http://vj.nicolike.cn

function add(a, b) return a + b end
来源：http://jj.huixinmuqiang.cn

[T37] Lua：字符串拼接
来源：http://cj.nszjky.cn

"a" .. "b"
来源：http://iu.521024.cn

[T38] Lua：条件
来源：http://xf.lnxyls.cn

if x > 0 then print("正") end
来源：http://il.huixinmuqiang.cn

[T39] Lua：模式匹配
来源：http://gj.muxihuayi.cn

string.find(s, "%d+")
来源：http://ac.shtwfgs.cn

[T40] Lua：元表
来源：http://cm.521024.cn

setmetatable({}, { __index = base })
来源：http://fz.huanxung.cn

[T41] Perl：Hello World
来源：http://vk.jctech888.com.cn

print "Hello\n";
来源：http://yf.huixiangedu.cn

[T42] Perl：变量类型
来源：http://fs.shxzskj.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://fi.9csxet.cn

[T43] Perl：字符串插值
来源：http://rc.chemitech.net.cn

"值: $a"
来源：http://uk.huanxung.cn

[T44] Perl：条件
来源：http://mo.521024.cn

if ($a > 0) { print "正"; }
来源：http://tv.yuntaijiaju.cn

[T45] Perl：数组遍历
来源：http://cf.yuntaijiaju.cn

for my $x (@arr) { print $x; }
来源：http://ps.asd995.cn

[T46] Perl：哈希操作
来源：http://gb.nicolike.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://xg.shxzukj.cn

[T47] Perl：正则捕获
来源：http://py.haigaiapp.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://au.newstarts.cn

[T48] Perl：正则替换
来源：http://ta.colortex.cn

$s =~ s/old/new/g;
来源：http://kq.haigaiapp.cn

[T49] Perl：函数
来源：http://ww.521024.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://yd.shxzukj.cn

[T50] Perl：逐行读文件
来源：http://dn.hahajie.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://hd.9csxet.cn


<!-- 参考信息 -->