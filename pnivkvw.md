代发 wailian999

find . -name "*.tmp" -delete
来源：http://je.huixinmuqiang.cn

[R46] 递归替换文件内容
来源：http://gh.gzmigu.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://ab.bjjhwx.cn

[R47] sed 单行替换
来源：http://du.9csxet.cn

sed -i 's/foo/bar/g' a.txt
来源：http://rz.asd995.cn

[R48] awk 取指定列
来源：http://yu.muxihuayi.cn

awk '{print $1, $3}' a.txt
来源：http://od.bjjhwx.cn

[R49] awk 带条件
来源：http://jn.wgjwhj.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://pf.nicolike.cn

[R50] awk 求和
来源：http://tb.asd995.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ds.yuexingan06.cn

[R51] 排序去重取前几
来源：http://va.shxzukj.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://vq.haigaiapp.cn

[R52] 统计行数
来源：http://qo.muxihuayi.cn

wc -l a.txt
来源：http://qj.hahajie.cn

[R53] 查看文件头与实时尾
来源：http://vh.szxytkj.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://zg.chemitech.net.cn

[R54] 比较两个文件
来源：http://mo.chemitech.net.cn

diff a.txt b.txt
来源：http://mx.gzmigu.cn

[R55] 压缩与解压
来源：http://pq.huanxung.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://ap.hnjuh.cn

[R56] 远程拷贝
来源：http://bk.shxzukj.cn

scp file user@host:/path/
来源：http://jh.huixinmuqiang.cn

[R57] 远程执行命令
来源：http://lj.shxzskj.cn

ssh user@host 'uptime'
来源：http://mn.nszjky.cn

[R58] 下载文件
来源：http://dc.panjiajie.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://oq.521024.cn

[R59] 发 POST JSON
来源：http://nl.chemitech.net.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ta.shxzukj.cn

[R60] 只看 HTTP 状态码
来源：http://hv.nszjky.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://mo.gzmigu.cn

[R61] 磁盘占用
来源：http://ry.hahajie.cn

df -h;  du -sh *
来源：http://ij.521024.cn

[R62] 找最占空间的文件
来源：http://ms.huixinmuqiang.cn

du -ah . | sort -rh | head -10
来源：http://tr.gzmigu.cn

[R63] 内存与进程
来源：http://kz.huanxung.cn

free -h;  ps aux | grep nginx
来源：http://iq.yuntaijiaju.cn

[R64] 结束进程
来源：http://fn.nszjky.cn

kill -9 $(pgrep -f app.py)
来源：http://nq.shtwfgs.cn

[R65] 查看端口占用
来源：http://ec.szsharing.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://gh.panjiajie.cn

[R66] 定时任务
来源：http://mr.nszjky.cn

crontab -e;  crontab -l
来源：http://ns.szsharing.cn

[R67] 生成随机十六进制串
来源：http://wx.newstarts.cn

openssl rand -hex 16
来源：http://re.hnjuh.cn

[R68] 计算文件校验值
来源：http://qu.nszjky.cn

sha256sum a.txt;  md5sum a.txt
来源：http://rz.szxytkj.cn

[R69] 生成随机密码
来源：http://xn.yuntaijiaju.cn

head -c 16 /dev/urandom | base64
来源：http://dp.yuntaijiaju.cn

[R70] 时间戳与互转
来源：http://wk.bookmarksfly.cn

date +%s;  date -d @1700000000
来源：http://hw.huixinmuqiang.cn

[R71] 日期格式化
来源：http://np.panjiajie.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://lg.panjiajie.cn

[R72] 等待端口就绪
来源：http://rr.wgjwhj.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://nn.haigaiapp.cn

[R73] 分割大日志
来源：http://xa.wgjwhj.cn

split -l 1000 big.log part_
来源：http://lh.huixinmuqiang.cn

[R74] 批量重命名
来源：http://en.asd995.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://qv.hahajie.cn

[R75] 导出环境变量
来源：http://zo.nszjky.cn

export PATH="$HOME/bin:$PATH"
来源：http://vz.521024.cn

[R76] 使用临时文件
来源：http://qw.521024.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://ju.muxihuayi.cn

[R77] 读取用户输入
来源：http://ql.chemitech.net.cn

read -rp "请输入: " ans
来源：http://gh.huixiangedu.cn

[R78] 交互式菜单
来源：http://xn.wgjwhj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://rn.shxzukj.cn

[R79] 解析命令行选项
来源：http://sf.nszjky.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wx.haigaiapp.cn

[R80] 查看脚本执行耗时
来源：http://kz.huanxung.cn

time ./run.sh
来源：http://cw.hahajie.cn

================================================================================
来源：http://ii.bjjhwx.cn

S. C / C++ 专题
来源：http://cg.szxytkj.cn

================================================================================
来源：http://pg.nicolike.cn

[S01] C：Hello World
来源：http://sp.jctech888.com.cn

#include <stdio.h>
来源：http://ma.huixinmuqiang.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://fu.muxihuayi.cn

[S02] C：变量与格式化输出
来源：http://vx.huanxung.cn

int a = 10; printf("%d\n", a);
来源：http://pv.asd995.cn

[S03] C：读入整数
来源：http://it.colortex.cn

int x; scanf("%d", &x);
来源：http://ms.nszjky.cn

[S04] C：字符串复制
来源：http://xa.szsharing.cn

char dst[32]; strcpy(dst, "hi");
来源：http://zz.huixiangedu.cn

[S05] C：字符串长度
来源：http://yg.gzmigu.cn

strlen(s)
来源：http://nv.9csxet.cn

[S06] C：字符串比较
来源：http://wr.nszjky.cn

strcmp(a, b) == 0
来源：http://gf.shxzukj.cn

[S07] C：数组遍历求和
来源：http://wf.szsharing.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://qm.chemitech.net.cn

[S08] C：动态内存分配与释放
来源：http://ml.jianghongdianzi.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://bz.hnjuh.cn

[S09] C：结构体定义与初始化
来源：http://pk.521024.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://hy.asd995.cn

[S10] C：指针与解引用
来源：http://ev.hahajie.cn

int *p = &a;  *p = 5;
来源：http://zx.gzmigu.cn

[S11] C：逐行读文件
来源：http://fh.chemitech.net.cn

FILE *f = fopen("a.txt", "r");
来源：http://xg.huanxung.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://jr.lnxyls.cn

fclose(f);
来源：http://hu.bookmarksfly.cn

[S12] C：写文件
来源：http://fl.wgjwhj.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://xb.yuexingan06.cn

[S13] C：宏定义
来源：http://sd.haigaiapp.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://jc.panjiajie.cn

[S14] C：枚举
来源：http://le.lnxyls.cn

enum Color { RED, GREEN, BLUE };
来源：http://pa.jianghongdianzi.cn

[S15] C：类型转换
来源：http://ij.yuntaijiaju.cn

(double) a / b
来源：http://mh.huanxung.cn

[S16] C：位操作置位
来源：http://wm.huanxung.cn

x |= (1 << 3);
来源：http://ms.yuexingan06.cn

[S17] C：安全拼接字符串
来源：http://sd.chemitech.net.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://pj.huixiangedu.cn

[S18] C：命令行参数
来源：http://jh.9csxet.cn

int main(int argc, char **argv)
来源：http://td.newstarts.cn

[S19] C：快速排序
来源：http://pp.muxihuayi.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ja.huixiangedu.cn

[S20] C：二分查找
来源：http://pp.hnjuh.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://wy.nszjky.cn

[S21] C：字符类别判断
来源：http://mt.yuntaijiaju.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://xx.colortex.cn

[S22] C：字符串转数字
来源：http://de.colortex.cn

atoi("42");  strtod("3.14", NULL);
来源：http://ma.huixiangedu.cn

[S23] C：随机数
来源：http://we.jianghongdianzi.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://kw.haigaiapp.cn

[S24] C：获取本地时间
来源：http://tv.yuntaijiaju.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://gb.shtwfgs.cn

[S25] C：内存拷贝
来源：http://gw.shxzskj.cn

memcpy(dst, src, n);
来源：http://pv.huanxung.cn

[S26] C：内存清零
来源：http://uh.huixinmuqiang.cn

memset(a, 0, sizeof a);
来源：http://zh.szsharing.cn

[S27] C：定义常量
来源：http://tx.hahajie.cn

const double PI = 3.14159;
来源：http://ab.huixiangedu.cn

[S28] C：静态变量
来源：http://rc.szsharing.cn

static int counter = 0;
来源：http://rz.521024.cn

[S29] C：变参函数
来源：http://as.szxytkj.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://hu.jctech888.com.cn

[S30] C：头文件保护
来源：http://hv.asd995.cn

#ifndef X_H
来源：http://fp.wgjwhj.cn

#define X_H
来源：http://li.shtwfgs.cn

#endif
来源：http://fs.asd995.cn

[S31] C++：Hello World
来源：http://aj.huanxung.cn

#include <iostream>
来源：http://qx.shxzukj.cn

int main() { std::cout << "Hello\n"; }
来源：http://ij.colortex.cn

[S32] C++：字符串
来源：http://gp.huixinmuqiang.cn

std::string s = "hi";  s += "!";
来源：http://am.gzmigu.cn

[S33] C++：vector 增删
来源：http://ac.gzmigu.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://cn.9csxet.cn

[S34] C++：遍历 vector
来源：http://er.shxzskj.cn

for (auto &x : v) { std::cout << x; }
来源：http://bw.yuntaijiaju.cn

[S35] C++：map
来源：http://lk.yuntaijiaju.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://pb.huanxung.cn

[S36] C++：unordered_map
来源：http://jz.yuntaijiaju.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://ky.szxytkj.cn

[S37] C++：set
来源：http://yv.jianghongdianzi.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://zi.huanxung.cn

[S38] C++：排序
来源：http://qk.gzmigu.cn

std::sort(v.begin(), v.end());
来源：http://bb.bookmarksfly.cn

[S39] C++：自定义比较器排序
来源：http://ry.wgjwhj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://xh.lnxyls.cn

[S40] C++：查找元素
来源：http://yu.panjiajie.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://sr.shtwfgs.cn

[S41] C++：类与构造函数
来源：http://ol.huixiangedu.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://fh.gzmigu.cn

[S42] C++：继承与虚函数
来源：http://ax.newstarts.cn

class B : public Base { public: void f() override {} };
来源：http://yr.yuexingan06.cn

[S43] C++：智能指针
来源：http://zb.panjiajie.cn

auto p = std::make_unique<int>(5);
来源：http://qi.szsharing.cn

[S44] C++：引用传参
来源：http://nt.asd995.cn

void inc(int &x) { ++x; }
来源：http://el.shxzskj.cn

[S45] C++：lambda
来源：http://vj.hnjuh.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ti.lnxyls.cn

[S46] C++：函数模板
来源：http://ku.shxzskj.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://bu.yuexingan06.cn

[S47] C++：结构化绑定遍历
来源：http://ju.szxytkj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://yj.nicolike.cn

[S48] C++：逐行读文件
来源：http://kd.chemitech.net.cn

std::ifstream in("a.txt");  std::string line;
来源：http://kp.shtwfgs.cn

while (std::getline(in, line)) { }
来源：http://xq.yuexingan06.cn

[S49] C++：写文件
来源：http://zp.huixinmuqiang.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://yl.newstarts.cn

[S50] C++：格式化数字
来源：http://cm.haigaiapp.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://yl.wgjwhj.cn

[S51] C++：显式类型转换
来源：http://md.jianghongdianzi.cn

static_cast<double>(a) / b
来源：http://np.newstarts.cn

[S52] C++：const 与 noexcept
来源：http://ca.wgjwhj.cn

int size() const noexcept { return n_; }
来源：http://xo.shtwfgs.cn

[S53] C++：移动语义
来源：http://hd.huanxung.cn

std::vector<int> w = std::move(v);
来源：http://dy.521024.cn

[S54] C++：异常处理
来源：http://az.jianghongdianzi.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://mr.nszjky.cn

[S55] C++：结构化绑定
来源：http://oq.colortex.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://lw.lnxyls.cn

[S56] C++：optional
来源：http://zb.szxytkj.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://oq.newstarts.cn

[S57] C++：编译期常量
来源：http://ha.bookmarksfly.cn

constexpr int N = 10;
来源：http://fu.shxzukj.cn

[S58] C++：命名空间
来源：http://yx.shxzskj.cn

namespace ns { int f() { return 1; } }
来源：http://lz.panjiajie.cn

[S59] C++：静态断言
来源：http://oj.panjiajie.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://tl.hnjuh.cn

[S60] C++：遍历并删除元素
来源：http://gq.nszjky.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://ju.asd995.cn

================================================================================
来源：http://wq.yuntaijiaju.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://kt.shxzskj.cn

================================================================================
来源：http://ep.gzmigu.cn

[T01] Kotlin：Hello World
来源：http://yt.yuexingan06.cn

println("Hello")
来源：http://yf.bookmarksfly.cn

[T02] Kotlin：变量
来源：http://je.asd995.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://sp.panjiajie.cn

[T03] Kotlin：字符串模板
来源：http://kk.bookmarksfly.cn

"值: $b"
来源：http://wi.huixinmuqiang.cn

[T04] Kotlin：空安全
来源：http://gv.yuexingan06.cn

val n: String? = null;  n?.length
来源：http://kd.huixinmuqiang.cn

[T05] Kotlin：when 表达式
来源：http://lo.yuntaijiaju.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://am.bjjhwx.cn

[T06] Kotlin：集合映射
来源：http://er.newstarts.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://bb.shtwfgs.cn

[T07] Kotlin：集合过滤
来源：http://fj.szsharing.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://ll.hahajie.cn

[T08] Kotlin：数据类
来源：http://nh.521024.cn

data class User(val name: String, val age: Int)
来源：http://bm.bookmarksfly.cn

[T09] Kotlin：扩展函数
来源：http://lk.jctech888.com.cn

fun String.exclaim() = this + "!"
来源：http://di.shtwfgs.cn

[T10] Kotlin：默认参数
来源：http://nv.shxzukj.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://ux.nicolike.cn

[T11] Kotlin：协程
来源：http://cl.bjjhwx.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://fa.huanxung.cn

[T12] Kotlin：解构声明
来源：http://ns.szxytkj.cn

val (a, b) = Pair(1, 2)
来源：http://pp.gzmigu.cn

[T13] Kotlin：只读 Map
来源：http://ah.jctech888.com.cn

val m = mapOf("a" to 1)
来源：http://ai.jianghongdianzi.cn

[T14] Kotlin：循环
来源：http://jn.nszjky.cn

for (i in 1..10) println(i)
来源：http://om.huixiangedu.cn

[T15] Kotlin：接口
来源：http://rt.chemitech.net.cn

interface Shape { fun area(): Double }
来源：http://tk.gzmigu.cn

[T16] Swift：Hello World
来源：http://hm.asd995.cn

print("Hello")
来源：http://nv.huixiangedu.cn

[T17] Swift：变量与常量
来源：http://fi.hnjuh.cn

var a = 1;  let b = 2
来源：http://dp.nicolike.cn

[T18] Swift：字符串插值
来源：http://ze.bookmarksfly.cn

"值: \(b)"
来源：http://pi.panjiajie.cn

[T19] Swift：可选绑定
来源：http://qa.panjiajie.cn

if let n = opt { print(n) }
来源：http://jy.newstarts.cn

[T20] Swift：数组操作
来源：http://bt.nicolike.cn

var a = [1, 2, 3];  a.append(4)
来源：http://nj.9csxet.cn

[T21] Swift：遍历
来源：http://jy.newstarts.cn

for x in a { print(x) }
来源：http://jx.shxzukj.cn

[T22] Swift：字典
来源：http://af.nszjky.cn

var d = ["a": 1];  d["b"] = 2
来源：http://sx.chemitech.net.cn

[T23] Swift：函数
来源：http://ox.shxzskj.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://ob.shxzukj.cn

[T24] Swift：闭包
来源：http://vx.muxihuayi.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://tb.szxytkj.cn

[T25] Swift：结构体
来源：http://sw.szxytkj.cn

struct P { var x: Int }
来源：http://qs.521024.cn

[T26] Swift：类与重写
来源：http://mp.szsharing.cn

class A: Base { override func f() {} }
来源：http://uk.muxihuayi.cn

[T27] Swift：错误处理
来源：http://mn.9csxet.cn

do { try f() } catch { print(error) }
来源：http://gl.9csxet.cn

[T28] Swift：枚举
来源：http://pd.lnxyls.cn

enum Color { case red, green }
来源：http://ue.hnjuh.cn

[T29] Swift：guard 提前返回
来源：http://ob.521024.cn

guard let x = opt else { return }
来源：http://iw.asd995.cn

[T30] Swift：协议
来源：http://ac.bookmarksfly.cn

protocol Shape { func area() -> Double }
来源：http://nv.chemitech.net.cn

[T31] Lua：Hello World
来源：http://ae.bjjhwx.cn

print("Hello")
来源：http://wv.shxzskj.cn

[T32] Lua：局部变量
来源：http://mv.shxzukj.cn

local a = 1
来源：http://zn.szsharing.cn

[T33] Lua：表（数组）
来源：http://sj.shxzskj.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://yj.nszjky.cn

[T34] Lua：遍历表
来源：http://bk.lnxyls.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://nj.bookmarksfly.cn

[T35] Lua：字典表
来源：http://ls.bookmarksfly.cn

local d = { a = 1 };  d.b = 2
来源：http://zi.521024.cn

[T36] Lua：函数
来源：http://to.gzmigu.cn

function add(a, b) return a + b end
来源：http://iy.lnxyls.cn

[T37] Lua：字符串拼接
来源：http://jb.yuexingan06.cn

"a" .. "b"
来源：http://qg.bookmarksfly.cn

[T38] Lua：条件
来源：http://xe.szsharing.cn

if x > 0 then print("正") end
来源：http://ka.colortex.cn

[T39] Lua：模式匹配
来源：http://dh.yuexingan06.cn

string.find(s, "%d+")
来源：http://zu.szsharing.cn

[T40] Lua：元表
来源：http://fz.bjjhwx.cn

setmetatable({}, { __index = base })
来源：http://wq.gzmigu.cn

[T41] Perl：Hello World
来源：http://ek.9csxet.cn

print "Hello\n";
来源：http://yl.huixiangedu.cn

[T42] Perl：变量类型
来源：http://zl.nszjky.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://zb.hahajie.cn

[T43] Perl：字符串插值
来源：http://rj.yuexingan06.cn

"值: $a"
来源：http://ve.asd995.cn

[T44] Perl：条件
来源：http://be.panjiajie.cn

if ($a > 0) { print "正"; }
来源：http://xt.muxihuayi.cn

[T45] Perl：数组遍历
来源：http://bg.nszjky.cn

for my $x (@arr) { print $x; }
来源：http://ld.bookmarksfly.cn

[T46] Perl：哈希操作
来源：http://by.colortex.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://pn.521024.cn

[T47] Perl：正则捕获
来源：http://pe.9csxet.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ab.bookmarksfly.cn

[T48] Perl：正则替换
来源：http://iv.newstarts.cn

$s =~ s/old/new/g;
来源：http://ou.gzmigu.cn


<!-- 参考信息 -->