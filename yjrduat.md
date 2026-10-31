代发 wailian999

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://dj.9csxet.cn

[R50] awk 求和
来源：http://hw.bjjhwx.cn

awk '{s += $2} END {print s}' a.txt
来源：http://vq.521024.cn

[R51] 排序去重取前几
来源：http://zz.huanxung.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://zw.jctech888.com.cn

[R52] 统计行数
来源：http://cw.shxzskj.cn

wc -l a.txt
来源：http://xy.gzmigu.cn

[R53] 查看文件头与实时尾
来源：http://hz.colortex.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://nk.panjiajie.cn

[R54] 比较两个文件
来源：http://ug.9csxet.cn

diff a.txt b.txt
来源：http://db.yuntaijiaju.cn

[R55] 压缩与解压
来源：http://fp.hnjuh.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://eo.521024.cn

[R56] 远程拷贝
来源：http://ut.shxzskj.cn

scp file user@host:/path/
来源：http://ad.9csxet.cn

[R57] 远程执行命令
来源：http://wf.bjjhwx.cn

ssh user@host 'uptime'
来源：http://bk.nszjky.cn

[R58] 下载文件
来源：http://bt.lnxyls.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://il.colortex.cn

[R59] 发 POST JSON
来源：http://ec.huanxung.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://df.nszjky.cn

[R60] 只看 HTTP 状态码
来源：http://jp.asd995.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://xf.bookmarksfly.cn

[R61] 磁盘占用
来源：http://yi.shxzskj.cn

df -h;  du -sh *
来源：http://na.szsharing.cn

[R62] 找最占空间的文件
来源：http://cs.lnxyls.cn

du -ah . | sort -rh | head -10
来源：http://jj.chemitech.net.cn

[R63] 内存与进程
来源：http://bj.nszjky.cn

free -h;  ps aux | grep nginx
来源：http://ce.shtwfgs.cn

[R64] 结束进程
来源：http://hz.nszjky.cn

kill -9 $(pgrep -f app.py)
来源：http://ve.yuexingan06.cn

[R65] 查看端口占用
来源：http://zc.shxzskj.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://cd.szxytkj.cn

[R66] 定时任务
来源：http://gl.hnjuh.cn

crontab -e;  crontab -l
来源：http://fr.gzmigu.cn

[R67] 生成随机十六进制串
来源：http://ke.shtwfgs.cn

openssl rand -hex 16
来源：http://uk.hnjuh.cn

[R68] 计算文件校验值
来源：http://uw.jctech888.com.cn

sha256sum a.txt;  md5sum a.txt
来源：http://ti.shxzskj.cn

[R69] 生成随机密码
来源：http://jg.lnxyls.cn

head -c 16 /dev/urandom | base64
来源：http://zg.jctech888.com.cn

[R70] 时间戳与互转
来源：http://wf.jianghongdianzi.cn

date +%s;  date -d @1700000000
来源：http://vf.muxihuayi.cn

[R71] 日期格式化
来源：http://or.jctech888.com.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://hi.szsharing.cn

[R72] 等待端口就绪
来源：http://dr.shxzskj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://tw.shtwfgs.cn

[R73] 分割大日志
来源：http://oq.nicolike.cn

split -l 1000 big.log part_
来源：http://cf.9csxet.cn

[R74] 批量重命名
来源：http://bz.chemitech.net.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://og.gzmigu.cn

[R75] 导出环境变量
来源：http://dd.haigaiapp.cn

export PATH="$HOME/bin:$PATH"
来源：http://if.muxihuayi.cn

[R76] 使用临时文件
来源：http://xo.nszjky.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://yc.yuntaijiaju.cn

[R77] 读取用户输入
来源：http://ub.huixiangedu.cn

read -rp "请输入: " ans
来源：http://pe.wgjwhj.cn

[R78] 交互式菜单
来源：http://rl.muxihuayi.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://qi.shtwfgs.cn

[R79] 解析命令行选项
来源：http://pk.521024.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://yl.shxzukj.cn

[R80] 查看脚本执行耗时
来源：http://li.huixiangedu.cn

time ./run.sh
来源：http://wy.hnjuh.cn

================================================================================
来源：http://kj.hahajie.cn

S. C / C++ 专题
来源：http://ks.9csxet.cn

================================================================================
来源：http://zx.newstarts.cn

[S01] C：Hello World
来源：http://do.gzmigu.cn

#include <stdio.h>
来源：http://pl.bookmarksfly.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://mi.9csxet.cn

[S02] C：变量与格式化输出
来源：http://ww.panjiajie.cn

int a = 10; printf("%d\n", a);
来源：http://ql.521024.cn

[S03] C：读入整数
来源：http://ck.nicolike.cn

int x; scanf("%d", &x);
来源：http://yr.szxytkj.cn

[S04] C：字符串复制
来源：http://ml.wgjwhj.cn

char dst[32]; strcpy(dst, "hi");
来源：http://mf.muxihuayi.cn

[S05] C：字符串长度
来源：http://rq.shtwfgs.cn

strlen(s)
来源：http://sd.szxytkj.cn

[S06] C：字符串比较
来源：http://aw.hahajie.cn

strcmp(a, b) == 0
来源：http://du.bjjhwx.cn

[S07] C：数组遍历求和
来源：http://op.newstarts.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://qp.szxytkj.cn

[S08] C：动态内存分配与释放
来源：http://ys.newstarts.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://xq.wgjwhj.cn

[S09] C：结构体定义与初始化
来源：http://oz.nszjky.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://ud.jctech888.com.cn

[S10] C：指针与解引用
来源：http://fh.jianghongdianzi.cn

int *p = &a;  *p = 5;
来源：http://up.hahajie.cn

[S11] C：逐行读文件
来源：http://pi.szsharing.cn

FILE *f = fopen("a.txt", "r");
来源：http://am.lnxyls.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://sk.wgjwhj.cn

fclose(f);
来源：http://wg.9csxet.cn

[S12] C：写文件
来源：http://ht.lnxyls.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://qh.asd995.cn

[S13] C：宏定义
来源：http://mr.haigaiapp.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://pm.hnjuh.cn

[S14] C：枚举
来源：http://fs.haigaiapp.cn

enum Color { RED, GREEN, BLUE };
来源：http://kk.panjiajie.cn

[S15] C：类型转换
来源：http://yq.szsharing.cn

(double) a / b
来源：http://jd.521024.cn

[S16] C：位操作置位
来源：http://xz.szxytkj.cn

x |= (1 << 3);
来源：http://yr.nicolike.cn

[S17] C：安全拼接字符串
来源：http://es.wgjwhj.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://zx.huanxung.cn

[S18] C：命令行参数
来源：http://wu.huanxung.cn

int main(int argc, char **argv)
来源：http://mo.asd995.cn

[S19] C：快速排序
来源：http://xl.muxihuayi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://bn.huixinmuqiang.cn

[S20] C：二分查找
来源：http://ge.hnjuh.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://zc.haigaiapp.cn

[S21] C：字符类别判断
来源：http://jg.huixiangedu.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://sr.asd995.cn

[S22] C：字符串转数字
来源：http://ob.huanxung.cn

atoi("42");  strtod("3.14", NULL);
来源：http://rf.jctech888.com.cn

[S23] C：随机数
来源：http://gs.nicolike.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://bv.chemitech.net.cn

[S24] C：获取本地时间
来源：http://km.szxytkj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://dq.bjjhwx.cn

[S25] C：内存拷贝
来源：http://li.newstarts.cn

memcpy(dst, src, n);
来源：http://ue.nicolike.cn

[S26] C：内存清零
来源：http://pg.521024.cn

memset(a, 0, sizeof a);
来源：http://ir.hahajie.cn

[S27] C：定义常量
来源：http://br.521024.cn

const double PI = 3.14159;
来源：http://ct.9csxet.cn

[S28] C：静态变量
来源：http://ja.yuntaijiaju.cn

static int counter = 0;
来源：http://yq.szxytkj.cn

[S29] C：变参函数
来源：http://js.chemitech.net.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://mt.wgjwhj.cn

[S30] C：头文件保护
来源：http://fp.521024.cn

#ifndef X_H
来源：http://yy.huixinmuqiang.cn

#define X_H
来源：http://nm.hnjuh.cn

#endif
来源：http://yq.yuntaijiaju.cn

[S31] C++：Hello World
来源：http://iw.nszjky.cn

#include <iostream>
来源：http://xp.colortex.cn

int main() { std::cout << "Hello\n"; }
来源：http://qw.asd995.cn

[S32] C++：字符串
来源：http://dw.wgjwhj.cn

std::string s = "hi";  s += "!";
来源：http://qy.shtwfgs.cn

[S33] C++：vector 增删
来源：http://sa.szsharing.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://io.shxzukj.cn

[S34] C++：遍历 vector
来源：http://jk.shtwfgs.cn

for (auto &x : v) { std::cout << x; }
来源：http://bn.asd995.cn

[S35] C++：map
来源：http://ys.9csxet.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://rx.bjjhwx.cn

[S36] C++：unordered_map
来源：http://wv.521024.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ok.panjiajie.cn

[S37] C++：set
来源：http://tf.szxytkj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://iw.jctech888.com.cn

[S38] C++：排序
来源：http://jf.lnxyls.cn

std::sort(v.begin(), v.end());
来源：http://yn.lnxyls.cn

[S39] C++：自定义比较器排序
来源：http://ph.huanxung.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://vs.muxihuayi.cn

[S40] C++：查找元素
来源：http://wm.haigaiapp.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://hh.shxzskj.cn

[S41] C++：类与构造函数
来源：http://km.gzmigu.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://vr.muxihuayi.cn

[S42] C++：继承与虚函数
来源：http://pv.bookmarksfly.cn

class B : public Base { public: void f() override {} };
来源：http://ah.huanxung.cn

[S43] C++：智能指针
来源：http://fn.jianghongdianzi.cn

auto p = std::make_unique<int>(5);
来源：http://aa.asd995.cn

[S44] C++：引用传参
来源：http://nw.szsharing.cn

void inc(int &x) { ++x; }
来源：http://tv.jctech888.com.cn

[S45] C++：lambda
来源：http://dc.521024.cn

auto add = [](int a, int b) { return a + b; };
来源：http://tx.hnjuh.cn

[S46] C++：函数模板
来源：http://xm.shtwfgs.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://cg.jianghongdianzi.cn

[S47] C++：结构化绑定遍历
来源：http://ur.haigaiapp.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://oi.newstarts.cn

[S48] C++：逐行读文件
来源：http://ml.bjjhwx.cn

std::ifstream in("a.txt");  std::string line;
来源：http://va.haigaiapp.cn

while (std::getline(in, line)) { }
来源：http://zy.huanxung.cn

[S49] C++：写文件
来源：http://fl.9csxet.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ia.bookmarksfly.cn

[S50] C++：格式化数字
来源：http://wa.szsharing.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://ys.szsharing.cn

[S51] C++：显式类型转换
来源：http://dd.yuexingan06.cn

static_cast<double>(a) / b
来源：http://rl.panjiajie.cn

[S52] C++：const 与 noexcept
来源：http://wo.jianghongdianzi.cn

int size() const noexcept { return n_; }
来源：http://io.nszjky.cn

[S53] C++：移动语义
来源：http://cm.shtwfgs.cn

std::vector<int> w = std::move(v);
来源：http://am.jctech888.com.cn

[S54] C++：异常处理
来源：http://lk.gzmigu.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://kl.nszjky.cn

[S55] C++：结构化绑定
来源：http://ex.yuntaijiaju.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://sq.shxzukj.cn

[S56] C++：optional
来源：http://ga.huixiangedu.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://om.hnjuh.cn

[S57] C++：编译期常量
来源：http://eh.szsharing.cn

constexpr int N = 10;
来源：http://nx.bjjhwx.cn

[S58] C++：命名空间
来源：http://ed.haigaiapp.cn

namespace ns { int f() { return 1; } }
来源：http://oc.bookmarksfly.cn

[S59] C++：静态断言
来源：http://hx.jctech888.com.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://jj.haigaiapp.cn

[S60] C++：遍历并删除元素
来源：http://ql.muxihuayi.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://rw.jianghongdianzi.cn

================================================================================
来源：http://ge.yuntaijiaju.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://fi.shtwfgs.cn

================================================================================
来源：http://qi.nicolike.cn

[T01] Kotlin：Hello World
来源：http://ao.shtwfgs.cn

println("Hello")
来源：http://ae.panjiajie.cn

[T02] Kotlin：变量
来源：http://cb.szxytkj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://la.haigaiapp.cn

[T03] Kotlin：字符串模板
来源：http://bf.521024.cn

"值: $b"
来源：http://rn.yuntaijiaju.cn

[T04] Kotlin：空安全
来源：http://pt.nicolike.cn

val n: String? = null;  n?.length
来源：http://me.haigaiapp.cn

[T05] Kotlin：when 表达式
来源：http://rx.szxytkj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://id.muxihuayi.cn

[T06] Kotlin：集合映射
来源：http://jr.szsharing.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://si.hnjuh.cn

[T07] Kotlin：集合过滤
来源：http://iw.9csxet.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://zg.huixinmuqiang.cn

[T08] Kotlin：数据类
来源：http://vh.szsharing.cn

data class User(val name: String, val age: Int)
来源：http://ua.bookmarksfly.cn

[T09] Kotlin：扩展函数
来源：http://pa.panjiajie.cn

fun String.exclaim() = this + "!"
来源：http://pd.asd995.cn

[T10] Kotlin：默认参数
来源：http://xt.panjiajie.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://vv.521024.cn

[T11] Kotlin：协程
来源：http://fg.szsharing.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://sm.bookmarksfly.cn

[T12] Kotlin：解构声明
来源：http://ad.yuexingan06.cn

val (a, b) = Pair(1, 2)
来源：http://jk.nszjky.cn

[T13] Kotlin：只读 Map
来源：http://nv.colortex.cn

val m = mapOf("a" to 1)
来源：http://zl.lnxyls.cn

[T14] Kotlin：循环
来源：http://vn.bjjhwx.cn

for (i in 1..10) println(i)
来源：http://tq.shtwfgs.cn

[T15] Kotlin：接口
来源：http://kb.shxzskj.cn

interface Shape { fun area(): Double }
来源：http://tu.lnxyls.cn

[T16] Swift：Hello World
来源：http://qv.bjjhwx.cn

print("Hello")
来源：http://tn.jianghongdianzi.cn

[T17] Swift：变量与常量
来源：http://xf.asd995.cn

var a = 1;  let b = 2
来源：http://ai.newstarts.cn

[T18] Swift：字符串插值
来源：http://ok.panjiajie.cn

"值: \(b)"
来源：http://bw.shxzukj.cn

[T19] Swift：可选绑定
来源：http://kp.nszjky.cn

if let n = opt { print(n) }
来源：http://eg.nicolike.cn

[T20] Swift：数组操作
来源：http://ud.szxytkj.cn

var a = [1, 2, 3];  a.append(4)
来源：http://gr.shxzukj.cn

[T21] Swift：遍历
来源：http://on.jianghongdianzi.cn

for x in a { print(x) }
来源：http://iw.wgjwhj.cn

[T22] Swift：字典
来源：http://oz.jctech888.com.cn

var d = ["a": 1];  d["b"] = 2
来源：http://qi.shxzskj.cn

[T23] Swift：函数
来源：http://ug.muxihuayi.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://nm.haigaiapp.cn

[T24] Swift：闭包
来源：http://vk.chemitech.net.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://ti.hnjuh.cn

[T25] Swift：结构体
来源：http://xd.yuexingan06.cn

struct P { var x: Int }
来源：http://uo.haigaiapp.cn

[T26] Swift：类与重写
来源：http://ml.hahajie.cn

class A: Base { override func f() {} }
来源：http://kw.9csxet.cn

[T27] Swift：错误处理
来源：http://ta.nicolike.cn

do { try f() } catch { print(error) }
来源：http://at.bjjhwx.cn

[T28] Swift：枚举
来源：http://wn.bookmarksfly.cn

enum Color { case red, green }
来源：http://ih.521024.cn

[T29] Swift：guard 提前返回
来源：http://bk.yuexingan06.cn

guard let x = opt else { return }
来源：http://gr.hnjuh.cn

[T30] Swift：协议
来源：http://cm.shtwfgs.cn

protocol Shape { func area() -> Double }
来源：http://ir.haigaiapp.cn

[T31] Lua：Hello World
来源：http://lb.szsharing.cn

print("Hello")
来源：http://yg.shxzskj.cn

[T32] Lua：局部变量
来源：http://ge.bjjhwx.cn

local a = 1
来源：http://xs.asd995.cn

[T33] Lua：表（数组）
来源：http://kj.colortex.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://hr.chemitech.net.cn

[T34] Lua：遍历表
来源：http://ts.huanxung.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ot.shxzskj.cn

[T35] Lua：字典表
来源：http://cj.hahajie.cn

local d = { a = 1 };  d.b = 2
来源：http://hn.panjiajie.cn

[T36] Lua：函数
来源：http://eu.shtwfgs.cn

function add(a, b) return a + b end
来源：http://mo.wgjwhj.cn

[T37] Lua：字符串拼接
来源：http://gf.huixiangedu.cn

"a" .. "b"
来源：http://da.lnxyls.cn

[T38] Lua：条件
来源：http://af.colortex.cn

if x > 0 then print("正") end
来源：http://qt.bookmarksfly.cn

[T39] Lua：模式匹配
来源：http://vz.jctech888.com.cn

string.find(s, "%d+")
来源：http://mn.yuexingan06.cn

[T40] Lua：元表
来源：http://gs.huixinmuqiang.cn

setmetatable({}, { __index = base })
来源：http://lh.lnxyls.cn

[T41] Perl：Hello World
来源：http://xv.lnxyls.cn

print "Hello\n";
来源：http://cf.bookmarksfly.cn

[T42] Perl：变量类型
来源：http://fm.shxzukj.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://zq.lnxyls.cn

[T43] Perl：字符串插值
来源：http://ab.wgjwhj.cn

"值: $a"
来源：http://sf.521024.cn

[T44] Perl：条件
来源：http://vf.muxihuayi.cn

if ($a > 0) { print "正"; }
来源：http://mg.chemitech.net.cn

[T45] Perl：数组遍历
来源：http://zv.9csxet.cn

for my $x (@arr) { print $x; }
来源：http://it.shtwfgs.cn

[T46] Perl：哈希操作
来源：http://iv.lnxyls.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://yl.lnxyls.cn

[T47] Perl：正则捕获
来源：http://ae.521024.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://it.colortex.cn

[T48] Perl：正则替换
来源：http://yh.wgjwhj.cn

$s =~ s/old/new/g;
来源：http://nv.hahajie.cn

[T49] Perl：函数
来源：http://rz.wgjwhj.cn

sub add { my ($a, $b) = @_; return $a + $b; }
来源：http://ry.hahajie.cn

[T50] Perl：逐行读文件
来源：http://gv.9csxet.cn

open my $fh, "<", "a.txt" or die $!;
来源：http://gi.wgjwhj.cn

while (my $line = <$fh>) { print $line; }
来源：http://sl.huixinmuqiang.cn

[T51] Scala：Hello World
来源：http://ng.hnjuh.cn

println("Hello")
来源：http://me.huanxung.cn

[T52] Scala：变量
来源：http://yk.huixinmuqiang.cn


<!-- 参考信息 -->