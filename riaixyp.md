代发 wailian999

find . -name "*.tmp" -delete
来源：http://xp.nicolike.cn

[R46] 递归替换文件内容
来源：http://yj.lnxyls.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://qt.huanxung.cn

[R47] sed 单行替换
来源：http://zg.gzmigu.cn

sed -i 's/foo/bar/g' a.txt
来源：http://rl.shtwfgs.cn

[R48] awk 取指定列
来源：http://cd.jctech888.com.cn

awk '{print $1, $3}' a.txt
来源：http://st.wgjwhj.cn

[R49] awk 带条件
来源：http://tj.9csxet.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://tg.lnxyls.cn

[R50] awk 求和
来源：http://fg.lnxyls.cn

awk '{s += $2} END {print s}' a.txt
来源：http://da.bjjhwx.cn

[R51] 排序去重取前几
来源：http://rm.huanxung.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://nq.hnjuh.cn

[R52] 统计行数
来源：http://ju.muxihuayi.cn

wc -l a.txt
来源：http://de.jctech888.com.cn

[R53] 查看文件头与实时尾
来源：http://xs.nicolike.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ns.9csxet.cn

[R54] 比较两个文件
来源：http://il.muxihuayi.cn

diff a.txt b.txt
来源：http://xy.hnjuh.cn

[R55] 压缩与解压
来源：http://tw.lnxyls.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://yj.huixiangedu.cn

[R56] 远程拷贝
来源：http://td.colortex.cn

scp file user@host:/path/
来源：http://ce.colortex.cn

[R57] 远程执行命令
来源：http://jx.hnjuh.cn

ssh user@host 'uptime'
来源：http://gb.jianghongdianzi.cn

[R58] 下载文件
来源：http://pl.yuexingan06.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://et.shtwfgs.cn

[R59] 发 POST JSON
来源：http://un.hahajie.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://uv.huanxung.cn

[R60] 只看 HTTP 状态码
来源：http://rb.hahajie.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ax.bjjhwx.cn

[R61] 磁盘占用
来源：http://mf.szsharing.cn

df -h;  du -sh *
来源：http://yf.shtwfgs.cn

[R62] 找最占空间的文件
来源：http://yd.nicolike.cn

du -ah . | sort -rh | head -10
来源：http://hz.asd995.cn

[R63] 内存与进程
来源：http://db.szsharing.cn

free -h;  ps aux | grep nginx
来源：http://ol.nszjky.cn

[R64] 结束进程
来源：http://vd.shxzukj.cn

kill -9 $(pgrep -f app.py)
来源：http://ia.huixiangedu.cn

[R65] 查看端口占用
来源：http://me.lnxyls.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://kk.colortex.cn

[R66] 定时任务
来源：http://ow.huixinmuqiang.cn

crontab -e;  crontab -l
来源：http://ac.gzmigu.cn

[R67] 生成随机十六进制串
来源：http://sw.szxytkj.cn

openssl rand -hex 16
来源：http://fw.9csxet.cn

[R68] 计算文件校验值
来源：http://bz.hnjuh.cn

sha256sum a.txt;  md5sum a.txt
来源：http://uw.nszjky.cn

[R69] 生成随机密码
来源：http://jb.muxihuayi.cn

head -c 16 /dev/urandom | base64
来源：http://xt.nicolike.cn

[R70] 时间戳与互转
来源：http://fv.hnjuh.cn

date +%s;  date -d @1700000000
来源：http://lh.nszjky.cn

[R71] 日期格式化
来源：http://kg.haigaiapp.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://xd.lnxyls.cn

[R72] 等待端口就绪
来源：http://gd.panjiajie.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://te.gzmigu.cn

[R73] 分割大日志
来源：http://rg.hahajie.cn

split -l 1000 big.log part_
来源：http://gb.9csxet.cn

[R74] 批量重命名
来源：http://wl.9csxet.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://fq.colortex.cn

[R75] 导出环境变量
来源：http://mw.chemitech.net.cn

export PATH="$HOME/bin:$PATH"
来源：http://zg.shxzskj.cn

[R76] 使用临时文件
来源：http://ky.szsharing.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://qk.9csxet.cn

[R77] 读取用户输入
来源：http://rb.wgjwhj.cn

read -rp "请输入: " ans
来源：http://rv.huixinmuqiang.cn

[R78] 交互式菜单
来源：http://mx.jctech888.com.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://gn.huanxung.cn

[R79] 解析命令行选项
来源：http://nx.panjiajie.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ns.panjiajie.cn

[R80] 查看脚本执行耗时
来源：http://qy.yuexingan06.cn

time ./run.sh
来源：http://ld.9csxet.cn

================================================================================
来源：http://kf.huixinmuqiang.cn

S. C / C++ 专题
来源：http://nj.shxzskj.cn

================================================================================
来源：http://is.9csxet.cn

[S01] C：Hello World
来源：http://wg.szsharing.cn

#include <stdio.h>
来源：http://ov.9csxet.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://yz.bjjhwx.cn

[S02] C：变量与格式化输出
来源：http://ku.hnjuh.cn

int a = 10; printf("%d\n", a);
来源：http://ip.lnxyls.cn

[S03] C：读入整数
来源：http://tq.bjjhwx.cn

int x; scanf("%d", &x);
来源：http://cg.hnjuh.cn

[S04] C：字符串复制
来源：http://zh.shxzskj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://ir.nicolike.cn

[S05] C：字符串长度
来源：http://jo.chemitech.net.cn

strlen(s)
来源：http://cy.jctech888.com.cn

[S06] C：字符串比较
来源：http://bu.wgjwhj.cn

strcmp(a, b) == 0
来源：http://ln.lnxyls.cn

[S07] C：数组遍历求和
来源：http://kp.shxzukj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://sa.haigaiapp.cn

[S08] C：动态内存分配与释放
来源：http://dj.huixinmuqiang.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://gs.bookmarksfly.cn

[S09] C：结构体定义与初始化
来源：http://md.nszjky.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://zw.newstarts.cn

[S10] C：指针与解引用
来源：http://aq.shxzskj.cn

int *p = &a;  *p = 5;
来源：http://oj.colortex.cn

[S11] C：逐行读文件
来源：http://fg.asd995.cn

FILE *f = fopen("a.txt", "r");
来源：http://fp.yuexingan06.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://wu.hnjuh.cn

fclose(f);
来源：http://gi.shxzskj.cn

[S12] C：写文件
来源：http://cn.colortex.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://qy.nszjky.cn

[S13] C：宏定义
来源：http://oe.shxzskj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://zs.szxytkj.cn

[S14] C：枚举
来源：http://ou.haigaiapp.cn

enum Color { RED, GREEN, BLUE };
来源：http://ec.chemitech.net.cn

[S15] C：类型转换
来源：http://lu.521024.cn

(double) a / b
来源：http://st.lnxyls.cn

[S16] C：位操作置位
来源：http://fx.szxytkj.cn

x |= (1 << 3);
来源：http://tj.nicolike.cn

[S17] C：安全拼接字符串
来源：http://zn.shtwfgs.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://px.shxzukj.cn

[S18] C：命令行参数
来源：http://gt.gzmigu.cn

int main(int argc, char **argv)
来源：http://gm.nszjky.cn

[S19] C：快速排序
来源：http://cy.jianghongdianzi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://dq.jctech888.com.cn

[S20] C：二分查找
来源：http://kp.yuexingan06.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://yd.hnjuh.cn

[S21] C：字符类别判断
来源：http://qj.gzmigu.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://wh.jianghongdianzi.cn

[S22] C：字符串转数字
来源：http://dr.shtwfgs.cn

atoi("42");  strtod("3.14", NULL);
来源：http://qr.wgjwhj.cn

[S23] C：随机数
来源：http://zp.shxzskj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://xj.jctech888.com.cn

[S24] C：获取本地时间
来源：http://qx.9csxet.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://qj.gzmigu.cn

[S25] C：内存拷贝
来源：http://nf.szxytkj.cn

memcpy(dst, src, n);
来源：http://zv.szxytkj.cn

[S26] C：内存清零
来源：http://na.shxzskj.cn

memset(a, 0, sizeof a);
来源：http://uy.asd995.cn

[S27] C：定义常量
来源：http://oi.shxzskj.cn

const double PI = 3.14159;
来源：http://px.bjjhwx.cn

[S28] C：静态变量
来源：http://rr.9csxet.cn

static int counter = 0;
来源：http://kl.shxzukj.cn

[S29] C：变参函数
来源：http://vi.nicolike.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://qf.yuexingan06.cn

[S30] C：头文件保护
来源：http://eq.huixinmuqiang.cn

#ifndef X_H
来源：http://lv.nszjky.cn

#define X_H
来源：http://jg.jianghongdianzi.cn

#endif
来源：http://jd.jianghongdianzi.cn

[S31] C++：Hello World
来源：http://xj.nszjky.cn

#include <iostream>
来源：http://rb.bjjhwx.cn

int main() { std::cout << "Hello\n"; }
来源：http://gd.huanxung.cn

[S32] C++：字符串
来源：http://oc.szsharing.cn

std::string s = "hi";  s += "!";
来源：http://aa.nicolike.cn

[S33] C++：vector 增删
来源：http://ge.szxytkj.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://id.jctech888.com.cn

[S34] C++：遍历 vector
来源：http://aa.wgjwhj.cn

for (auto &x : v) { std::cout << x; }
来源：http://gw.hnjuh.cn

[S35] C++：map
来源：http://ms.521024.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://mx.hnjuh.cn

[S36] C++：unordered_map
来源：http://gr.asd995.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://id.huixinmuqiang.cn

[S37] C++：set
来源：http://fj.huixinmuqiang.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://th.wgjwhj.cn

[S38] C++：排序
来源：http://nf.panjiajie.cn

std::sort(v.begin(), v.end());
来源：http://fe.yuexingan06.cn

[S39] C++：自定义比较器排序
来源：http://hi.huixiangedu.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ql.yuntaijiaju.cn

[S40] C++：查找元素
来源：http://vf.panjiajie.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://kd.jctech888.com.cn

[S41] C++：类与构造函数
来源：http://zm.nicolike.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://os.shxzukj.cn

[S42] C++：继承与虚函数
来源：http://oi.jctech888.com.cn

class B : public Base { public: void f() override {} };
来源：http://do.newstarts.cn

[S43] C++：智能指针
来源：http://ml.bjjhwx.cn

auto p = std::make_unique<int>(5);
来源：http://rs.szsharing.cn

[S44] C++：引用传参
来源：http://gx.gzmigu.cn

void inc(int &x) { ++x; }
来源：http://lx.muxihuayi.cn

[S45] C++：lambda
来源：http://ma.asd995.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ws.panjiajie.cn

[S46] C++：函数模板
来源：http://qv.huixiangedu.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://lr.lnxyls.cn

[S47] C++：结构化绑定遍历
来源：http://uf.hahajie.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://cb.nicolike.cn

[S48] C++：逐行读文件
来源：http://vv.hahajie.cn

std::ifstream in("a.txt");  std::string line;
来源：http://wl.jianghongdianzi.cn

while (std::getline(in, line)) { }
来源：http://et.bookmarksfly.cn

[S49] C++：写文件
来源：http://rs.yuntaijiaju.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://iz.nicolike.cn

[S50] C++：格式化数字
来源：http://qz.yuntaijiaju.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ce.muxihuayi.cn

[S51] C++：显式类型转换
来源：http://qv.newstarts.cn

static_cast<double>(a) / b
来源：http://oj.jctech888.com.cn

[S52] C++：const 与 noexcept
来源：http://uc.huanxung.cn

int size() const noexcept { return n_; }
来源：http://gs.huixiangedu.cn

[S53] C++：移动语义
来源：http://wu.shxzskj.cn

std::vector<int> w = std::move(v);
来源：http://fi.nicolike.cn

[S54] C++：异常处理
来源：http://eu.nszjky.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://ck.bjjhwx.cn

[S55] C++：结构化绑定
来源：http://ea.yuexingan06.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://kp.newstarts.cn

[S56] C++：optional
来源：http://lw.haigaiapp.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://uy.yuexingan06.cn

[S57] C++：编译期常量
来源：http://fh.nicolike.cn

constexpr int N = 10;
来源：http://ih.huanxung.cn

[S58] C++：命名空间
来源：http://xh.lnxyls.cn

namespace ns { int f() { return 1; } }
来源：http://kk.chemitech.net.cn

[S59] C++：静态断言
来源：http://oo.huixinmuqiang.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://hh.szxytkj.cn

[S60] C++：遍历并删除元素
来源：http://ws.haigaiapp.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://jl.huixinmuqiang.cn

================================================================================
来源：http://wr.haigaiapp.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://jj.newstarts.cn

================================================================================
来源：http://oo.shxzskj.cn

[T01] Kotlin：Hello World
来源：http://ac.9csxet.cn

println("Hello")
来源：http://sf.haigaiapp.cn

[T02] Kotlin：变量
来源：http://jq.colortex.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://ze.chemitech.net.cn

[T03] Kotlin：字符串模板
来源：http://hb.bjjhwx.cn

"值: $b"
来源：http://iz.9csxet.cn

[T04] Kotlin：空安全
来源：http://af.shxzukj.cn

val n: String? = null;  n?.length
来源：http://ew.haigaiapp.cn

[T05] Kotlin：when 表达式
来源：http://pm.newstarts.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://uu.9csxet.cn

[T06] Kotlin：集合映射
来源：http://tx.jianghongdianzi.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://rg.gzmigu.cn

[T07] Kotlin：集合过滤
来源：http://ig.shtwfgs.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ze.wgjwhj.cn

[T08] Kotlin：数据类
来源：http://jj.9csxet.cn

data class User(val name: String, val age: Int)
来源：http://ag.panjiajie.cn

[T09] Kotlin：扩展函数
来源：http://vk.muxihuayi.cn

fun String.exclaim() = this + "!"
来源：http://yi.huixinmuqiang.cn

[T10] Kotlin：默认参数
来源：http://vt.yuntaijiaju.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://sk.huixiangedu.cn

[T11] Kotlin：协程
来源：http://hj.newstarts.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://dr.jctech888.com.cn

[T12] Kotlin：解构声明
来源：http://yy.wgjwhj.cn

val (a, b) = Pair(1, 2)
来源：http://wn.huixinmuqiang.cn

[T13] Kotlin：只读 Map
来源：http://cd.szxytkj.cn

val m = mapOf("a" to 1)
来源：http://tn.shxzukj.cn

[T14] Kotlin：循环
来源：http://id.muxihuayi.cn

for (i in 1..10) println(i)
来源：http://uf.jianghongdianzi.cn

[T15] Kotlin：接口
来源：http://dd.asd995.cn

interface Shape { fun area(): Double }
来源：http://ts.huixinmuqiang.cn

[T16] Swift：Hello World
来源：http://nt.asd995.cn

print("Hello")
来源：http://bt.lnxyls.cn

[T17] Swift：变量与常量
来源：http://yy.yuntaijiaju.cn

var a = 1;  let b = 2
来源：http://zx.jianghongdianzi.cn

[T18] Swift：字符串插值
来源：http://vg.jianghongdianzi.cn

"值: \(b)"
来源：http://cv.shtwfgs.cn

[T19] Swift：可选绑定
来源：http://ot.asd995.cn

if let n = opt { print(n) }
来源：http://zz.hahajie.cn

[T20] Swift：数组操作
来源：http://rq.yuexingan06.cn

var a = [1, 2, 3];  a.append(4)
来源：http://oj.jianghongdianzi.cn

[T21] Swift：遍历
来源：http://vb.newstarts.cn

for x in a { print(x) }
来源：http://mw.nszjky.cn

[T22] Swift：字典
来源：http://zr.gzmigu.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ax.colortex.cn

[T23] Swift：函数
来源：http://vv.panjiajie.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ye.shxzskj.cn

[T24] Swift：闭包
来源：http://nh.lnxyls.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://la.colortex.cn

[T25] Swift：结构体
来源：http://tm.panjiajie.cn

struct P { var x: Int }
来源：http://mt.gzmigu.cn

[T26] Swift：类与重写
来源：http://eu.huixinmuqiang.cn

class A: Base { override func f() {} }
来源：http://wb.nszjky.cn

[T27] Swift：错误处理
来源：http://pq.gzmigu.cn

do { try f() } catch { print(error) }
来源：http://hg.jianghongdianzi.cn

[T28] Swift：枚举
来源：http://la.colortex.cn

enum Color { case red, green }
来源：http://ez.newstarts.cn

[T29] Swift：guard 提前返回
来源：http://hi.chemitech.net.cn

guard let x = opt else { return }
来源：http://ou.nicolike.cn

[T30] Swift：协议
来源：http://pi.yuexingan06.cn

protocol Shape { func area() -> Double }
来源：http://lx.panjiajie.cn

[T31] Lua：Hello World
来源：http://oj.asd995.cn

print("Hello")
来源：http://wp.nicolike.cn

[T32] Lua：局部变量
来源：http://sx.panjiajie.cn

local a = 1
来源：http://ka.shxzskj.cn

[T33] Lua：表（数组）
来源：http://tz.9csxet.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://mu.wgjwhj.cn

[T34] Lua：遍历表
来源：http://lv.hnjuh.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://rt.colortex.cn

[T35] Lua：字典表
来源：http://rt.bjjhwx.cn

local d = { a = 1 };  d.b = 2
来源：http://ny.shxzukj.cn

[T36] Lua：函数
来源：http://mj.521024.cn

function add(a, b) return a + b end
来源：http://iy.asd995.cn

[T37] Lua：字符串拼接
来源：http://qp.huixiangedu.cn

"a" .. "b"
来源：http://mu.nicolike.cn

[T38] Lua：条件
来源：http://wb.yuntaijiaju.cn

if x > 0 then print("正") end
来源：http://bm.chemitech.net.cn

[T39] Lua：模式匹配
来源：http://wu.shxzskj.cn

string.find(s, "%d+")
来源：http://tg.nicolike.cn

[T40] Lua：元表
来源：http://im.yuntaijiaju.cn

setmetatable({}, { __index = base })
来源：http://kt.shxzskj.cn

[T41] Perl：Hello World
来源：http://av.9csxet.cn

print "Hello\n";
来源：http://er.newstarts.cn

[T42] Perl：变量类型
来源：http://da.hnjuh.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ih.lnxyls.cn

[T43] Perl：字符串插值
来源：http://gt.muxihuayi.cn

"值: $a"
来源：http://td.9csxet.cn

[T44] Perl：条件
来源：http://ol.yuexingan06.cn

if ($a > 0) { print "正"; }
来源：http://hs.panjiajie.cn

[T45] Perl：数组遍历
来源：http://su.521024.cn

for my $x (@arr) { print $x; }
来源：http://ho.chemitech.net.cn

[T46] Perl：哈希操作
来源：http://xt.lnxyls.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://zn.bookmarksfly.cn

[T47] Perl：正则捕获
来源：http://ux.nicolike.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://pj.huanxung.cn

[T48] Perl：正则替换
来源：http://fn.szsharing.cn

$s =~ s/old/new/g;
来源：http://bb.gzmigu.cn


<!-- 参考信息 -->