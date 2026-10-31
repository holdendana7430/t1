代发 wailian999

find . -name "*.tmp" -delete
来源：http://mu.yuntaijiaju.cn

[R46] 递归替换文件内容
来源：http://wh.colortex.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://tl.lnxyls.cn

[R47] sed 单行替换
来源：http://is.wgjwhj.cn

sed -i 's/foo/bar/g' a.txt
来源：http://hm.chemitech.net.cn

[R48] awk 取指定列
来源：http://vg.wgjwhj.cn

awk '{print $1, $3}' a.txt
来源：http://df.521024.cn

[R49] awk 带条件
来源：http://bd.shxzukj.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://cc.bookmarksfly.cn

[R50] awk 求和
来源：http://jd.jianghongdianzi.cn

awk '{s += $2} END {print s}' a.txt
来源：http://fv.jianghongdianzi.cn

[R51] 排序去重取前几
来源：http://nr.szsharing.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://gb.lnxyls.cn

[R52] 统计行数
来源：http://ht.gzmigu.cn

wc -l a.txt
来源：http://py.yuexingan06.cn

[R53] 查看文件头与实时尾
来源：http://bg.shxzukj.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://rn.yuntaijiaju.cn

[R54] 比较两个文件
来源：http://jj.hahajie.cn

diff a.txt b.txt
来源：http://ki.521024.cn

[R55] 压缩与解压
来源：http://oa.huixinmuqiang.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://lz.huixiangedu.cn

[R56] 远程拷贝
来源：http://at.chemitech.net.cn

scp file user@host:/path/
来源：http://ff.haigaiapp.cn

[R57] 远程执行命令
来源：http://mj.jianghongdianzi.cn

ssh user@host 'uptime'
来源：http://uo.nszjky.cn

[R58] 下载文件
来源：http://jg.wgjwhj.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://kn.szsharing.cn

[R59] 发 POST JSON
来源：http://rb.shtwfgs.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://om.asd995.cn

[R60] 只看 HTTP 状态码
来源：http://rq.jctech888.com.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ih.bjjhwx.cn

[R61] 磁盘占用
来源：http://xt.chemitech.net.cn

df -h;  du -sh *
来源：http://kp.panjiajie.cn

[R62] 找最占空间的文件
来源：http://ir.muxihuayi.cn

du -ah . | sort -rh | head -10
来源：http://ka.shtwfgs.cn

[R63] 内存与进程
来源：http://cc.bookmarksfly.cn

free -h;  ps aux | grep nginx
来源：http://wy.hahajie.cn

[R64] 结束进程
来源：http://cq.shxzskj.cn

kill -9 $(pgrep -f app.py)
来源：http://ec.wgjwhj.cn

[R65] 查看端口占用
来源：http://pn.bookmarksfly.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://gm.newstarts.cn

[R66] 定时任务
来源：http://sl.jianghongdianzi.cn

crontab -e;  crontab -l
来源：http://qw.521024.cn

[R67] 生成随机十六进制串
来源：http://vr.jctech888.com.cn

openssl rand -hex 16
来源：http://aq.hnjuh.cn

[R68] 计算文件校验值
来源：http://jb.jianghongdianzi.cn

sha256sum a.txt;  md5sum a.txt
来源：http://eb.colortex.cn

[R69] 生成随机密码
来源：http://zw.shxzskj.cn

head -c 16 /dev/urandom | base64
来源：http://xq.521024.cn

[R70] 时间戳与互转
来源：http://kc.asd995.cn

date +%s;  date -d @1700000000
来源：http://ur.jianghongdianzi.cn

[R71] 日期格式化
来源：http://hv.jctech888.com.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://es.yuexingan06.cn

[R72] 等待端口就绪
来源：http://jj.gzmigu.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://yx.wgjwhj.cn

[R73] 分割大日志
来源：http://oj.szxytkj.cn

split -l 1000 big.log part_
来源：http://vk.shxzskj.cn

[R74] 批量重命名
来源：http://rn.521024.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://vf.asd995.cn

[R75] 导出环境变量
来源：http://ca.wgjwhj.cn

export PATH="$HOME/bin:$PATH"
来源：http://pg.bjjhwx.cn

[R76] 使用临时文件
来源：http://hy.chemitech.net.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://kn.bookmarksfly.cn

[R77] 读取用户输入
来源：http://hu.yuntaijiaju.cn

read -rp "请输入: " ans
来源：http://xl.521024.cn

[R78] 交互式菜单
来源：http://pf.asd995.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://qj.shxzskj.cn

[R79] 解析命令行选项
来源：http://qz.huanxung.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://ar.shxzukj.cn

[R80] 查看脚本执行耗时
来源：http://rf.huixinmuqiang.cn

time ./run.sh
来源：http://et.newstarts.cn

================================================================================
来源：http://tc.bjjhwx.cn

S. C / C++ 专题
来源：http://yz.nicolike.cn

================================================================================
来源：http://hx.hnjuh.cn

[S01] C：Hello World
来源：http://sq.newstarts.cn

#include <stdio.h>
来源：http://fe.nszjky.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://sy.shtwfgs.cn

[S02] C：变量与格式化输出
来源：http://rd.huixinmuqiang.cn

int a = 10; printf("%d\n", a);
来源：http://it.muxihuayi.cn

[S03] C：读入整数
来源：http://kr.szxytkj.cn

int x; scanf("%d", &x);
来源：http://th.yuntaijiaju.cn

[S04] C：字符串复制
来源：http://pz.jctech888.com.cn

char dst[32]; strcpy(dst, "hi");
来源：http://lw.lnxyls.cn

[S05] C：字符串长度
来源：http://em.panjiajie.cn

strlen(s)
来源：http://ml.jianghongdianzi.cn

[S06] C：字符串比较
来源：http://pj.huixinmuqiang.cn

strcmp(a, b) == 0
来源：http://rv.521024.cn

[S07] C：数组遍历求和
来源：http://rh.bookmarksfly.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://uw.asd995.cn

[S08] C：动态内存分配与释放
来源：http://tk.szxytkj.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ta.szsharing.cn

[S09] C：结构体定义与初始化
来源：http://ge.521024.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://pc.panjiajie.cn

[S10] C：指针与解引用
来源：http://qy.nicolike.cn

int *p = &a;  *p = 5;
来源：http://zv.szxytkj.cn

[S11] C：逐行读文件
来源：http://in.yuexingan06.cn

FILE *f = fopen("a.txt", "r");
来源：http://pb.huixinmuqiang.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://sf.gzmigu.cn

fclose(f);
来源：http://ob.yuntaijiaju.cn

[S12] C：写文件
来源：http://wn.shxzukj.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://lv.newstarts.cn

[S13] C：宏定义
来源：http://pl.shxzskj.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://aj.bjjhwx.cn

[S14] C：枚举
来源：http://dh.gzmigu.cn

enum Color { RED, GREEN, BLUE };
来源：http://wt.szxytkj.cn

[S15] C：类型转换
来源：http://yl.huixinmuqiang.cn

(double) a / b
来源：http://st.asd995.cn

[S16] C：位操作置位
来源：http://mg.chemitech.net.cn

x |= (1 << 3);
来源：http://wy.nszjky.cn

[S17] C：安全拼接字符串
来源：http://cu.hnjuh.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://mj.lnxyls.cn

[S18] C：命令行参数
来源：http://xg.wgjwhj.cn

int main(int argc, char **argv)
来源：http://os.wgjwhj.cn

[S19] C：快速排序
来源：http://ao.shxzskj.cn

qsort(a, n, sizeof(int), cmp);
来源：http://fm.lnxyls.cn

[S20] C：二分查找
来源：http://go.shtwfgs.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://yc.bjjhwx.cn

[S21] C：字符类别判断
来源：http://rs.9csxet.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://ut.szxytkj.cn

[S22] C：字符串转数字
来源：http://kp.nicolike.cn

atoi("42");  strtod("3.14", NULL);
来源：http://wu.muxihuayi.cn

[S23] C：随机数
来源：http://am.jctech888.com.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://kl.huanxung.cn

[S24] C：获取本地时间
来源：http://hh.shtwfgs.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://ys.muxihuayi.cn

[S25] C：内存拷贝
来源：http://ha.nszjky.cn

memcpy(dst, src, n);
来源：http://ya.gzmigu.cn

[S26] C：内存清零
来源：http://nk.hahajie.cn

memset(a, 0, sizeof a);
来源：http://ek.hahajie.cn

[S27] C：定义常量
来源：http://ya.yuntaijiaju.cn

const double PI = 3.14159;
来源：http://ur.gzmigu.cn

[S28] C：静态变量
来源：http://eb.shtwfgs.cn

static int counter = 0;
来源：http://pf.bjjhwx.cn

[S29] C：变参函数
来源：http://lm.colortex.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ta.shxzskj.cn

[S30] C：头文件保护
来源：http://vq.wgjwhj.cn

#ifndef X_H
来源：http://zj.hahajie.cn

#define X_H
来源：http://lg.panjiajie.cn

#endif
来源：http://bl.hnjuh.cn

[S31] C++：Hello World
来源：http://hf.nicolike.cn

#include <iostream>
来源：http://zs.hahajie.cn

int main() { std::cout << "Hello\n"; }
来源：http://ne.bookmarksfly.cn

[S32] C++：字符串
来源：http://zm.huixiangedu.cn

std::string s = "hi";  s += "!";
来源：http://op.gzmigu.cn

[S33] C++：vector 增删
来源：http://km.nicolike.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://af.panjiajie.cn

[S34] C++：遍历 vector
来源：http://pp.muxihuayi.cn

for (auto &x : v) { std::cout << x; }
来源：http://db.lnxyls.cn

[S35] C++：map
来源：http://aw.szxytkj.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ps.nszjky.cn

[S36] C++：unordered_map
来源：http://jl.panjiajie.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://op.huixinmuqiang.cn

[S37] C++：set
来源：http://di.shxzukj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://ic.gzmigu.cn

[S38] C++：排序
来源：http://bf.chemitech.net.cn

std::sort(v.begin(), v.end());
来源：http://il.szxytkj.cn

[S39] C++：自定义比较器排序
来源：http://oo.shxzukj.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://oz.yuexingan06.cn

[S40] C++：查找元素
来源：http://wf.gzmigu.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://mo.chemitech.net.cn

[S41] C++：类与构造函数
来源：http://od.yuexingan06.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://ae.9csxet.cn

[S42] C++：继承与虚函数
来源：http://mp.panjiajie.cn

class B : public Base { public: void f() override {} };
来源：http://no.newstarts.cn

[S43] C++：智能指针
来源：http://iv.nszjky.cn

auto p = std::make_unique<int>(5);
来源：http://na.shxzskj.cn

[S44] C++：引用传参
来源：http://ha.hnjuh.cn

void inc(int &x) { ++x; }
来源：http://nl.hnjuh.cn

[S45] C++：lambda
来源：http://wa.panjiajie.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ch.huixiangedu.cn

[S46] C++：函数模板
来源：http://zh.gzmigu.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://bn.szsharing.cn

[S47] C++：结构化绑定遍历
来源：http://mq.haigaiapp.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://on.haigaiapp.cn

[S48] C++：逐行读文件
来源：http://jo.panjiajie.cn

std::ifstream in("a.txt");  std::string line;
来源：http://vw.yuntaijiaju.cn

while (std::getline(in, line)) { }
来源：http://ln.bjjhwx.cn

[S49] C++：写文件
来源：http://nv.hnjuh.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://xw.shxzskj.cn

[S50] C++：格式化数字
来源：http://md.szsharing.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://wl.bookmarksfly.cn

[S51] C++：显式类型转换
来源：http://xs.szxytkj.cn

static_cast<double>(a) / b
来源：http://mw.muxihuayi.cn

[S52] C++：const 与 noexcept
来源：http://dz.newstarts.cn

int size() const noexcept { return n_; }
来源：http://sj.jctech888.com.cn

[S53] C++：移动语义
来源：http://vu.yuexingan06.cn

std::vector<int> w = std::move(v);
来源：http://xz.yuexingan06.cn

[S54] C++：异常处理
来源：http://kq.shtwfgs.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://xc.hahajie.cn

[S55] C++：结构化绑定
来源：http://pa.newstarts.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://qj.shxzskj.cn

[S56] C++：optional
来源：http://xu.bjjhwx.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://wd.shxzskj.cn

[S57] C++：编译期常量
来源：http://ri.szsharing.cn

constexpr int N = 10;
来源：http://lf.lnxyls.cn

[S58] C++：命名空间
来源：http://aw.hnjuh.cn

namespace ns { int f() { return 1; } }
来源：http://fs.jctech888.com.cn

[S59] C++：静态断言
来源：http://bb.chemitech.net.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://oh.panjiajie.cn

[S60] C++：遍历并删除元素
来源：http://is.chemitech.net.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://rg.jctech888.com.cn

================================================================================
来源：http://gr.nicolike.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://af.bookmarksfly.cn

================================================================================
来源：http://ui.nszjky.cn

[T01] Kotlin：Hello World
来源：http://fc.9csxet.cn

println("Hello")
来源：http://jc.szsharing.cn

[T02] Kotlin：变量
来源：http://ot.shxzukj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://kk.shxzskj.cn

[T03] Kotlin：字符串模板
来源：http://kf.jctech888.com.cn

"值: $b"
来源：http://oo.hnjuh.cn

[T04] Kotlin：空安全
来源：http://ko.huixiangedu.cn

val n: String? = null;  n?.length
来源：http://st.521024.cn

[T05] Kotlin：when 表达式
来源：http://pt.shxzskj.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://mf.shxzskj.cn

[T06] Kotlin：集合映射
来源：http://cr.wgjwhj.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://mp.wgjwhj.cn

[T07] Kotlin：集合过滤
来源：http://am.huanxung.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://dk.gzmigu.cn

[T08] Kotlin：数据类
来源：http://ek.lnxyls.cn

data class User(val name: String, val age: Int)
来源：http://jp.yuexingan06.cn

[T09] Kotlin：扩展函数
来源：http://kd.haigaiapp.cn

fun String.exclaim() = this + "!"
来源：http://xb.gzmigu.cn

[T10] Kotlin：默认参数
来源：http://sa.szsharing.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://de.huixiangedu.cn

[T11] Kotlin：协程
来源：http://jh.szsharing.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ao.shxzukj.cn

[T12] Kotlin：解构声明
来源：http://rq.muxihuayi.cn

val (a, b) = Pair(1, 2)
来源：http://de.szsharing.cn

[T13] Kotlin：只读 Map
来源：http://rx.huixiangedu.cn

val m = mapOf("a" to 1)
来源：http://ku.nicolike.cn

[T14] Kotlin：循环
来源：http://oo.yuexingan06.cn

for (i in 1..10) println(i)
来源：http://pp.shxzukj.cn

[T15] Kotlin：接口
来源：http://ck.chemitech.net.cn

interface Shape { fun area(): Double }
来源：http://oc.jianghongdianzi.cn

[T16] Swift：Hello World
来源：http://pt.colortex.cn

print("Hello")
来源：http://kf.hnjuh.cn

[T17] Swift：变量与常量
来源：http://qc.asd995.cn

var a = 1;  let b = 2
来源：http://kr.szsharing.cn

[T18] Swift：字符串插值
来源：http://kv.nicolike.cn

"值: \(b)"
来源：http://pm.yuntaijiaju.cn

[T19] Swift：可选绑定
来源：http://un.nicolike.cn

if let n = opt { print(n) }
来源：http://az.521024.cn

[T20] Swift：数组操作
来源：http://dh.bookmarksfly.cn

var a = [1, 2, 3];  a.append(4)
来源：http://xl.gzmigu.cn

[T21] Swift：遍历
来源：http://tp.colortex.cn

for x in a { print(x) }
来源：http://sc.yuexingan06.cn

[T22] Swift：字典
来源：http://vh.yuexingan06.cn

var d = ["a": 1];  d["b"] = 2
来源：http://ap.colortex.cn

[T23] Swift：函数
来源：http://of.asd995.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://fl.nszjky.cn

[T24] Swift：闭包
来源：http://mx.shxzukj.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://gy.colortex.cn

[T25] Swift：结构体
来源：http://xe.huixiangedu.cn

struct P { var x: Int }
来源：http://jl.gzmigu.cn

[T26] Swift：类与重写
来源：http://be.wgjwhj.cn

class A: Base { override func f() {} }
来源：http://sv.bookmarksfly.cn

[T27] Swift：错误处理
来源：http://ry.yuntaijiaju.cn

do { try f() } catch { print(error) }
来源：http://fp.bookmarksfly.cn

[T28] Swift：枚举
来源：http://gg.szxytkj.cn

enum Color { case red, green }
来源：http://zm.szsharing.cn

[T29] Swift：guard 提前返回
来源：http://gu.lnxyls.cn

guard let x = opt else { return }
来源：http://cc.shxzskj.cn

[T30] Swift：协议
来源：http://vw.nszjky.cn

protocol Shape { func area() -> Double }
来源：http://va.wgjwhj.cn

[T31] Lua：Hello World
来源：http://iv.jctech888.com.cn

print("Hello")
来源：http://yg.hahajie.cn

[T32] Lua：局部变量
来源：http://vi.huixiangedu.cn

local a = 1
来源：http://tt.bookmarksfly.cn

[T33] Lua：表（数组）
来源：http://is.huixinmuqiang.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://yc.shxzukj.cn

[T34] Lua：遍历表
来源：http://ys.huanxung.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://vh.gzmigu.cn

[T35] Lua：字典表
来源：http://ba.huixinmuqiang.cn

local d = { a = 1 };  d.b = 2
来源：http://bm.lnxyls.cn

[T36] Lua：函数
来源：http://vp.hnjuh.cn

function add(a, b) return a + b end
来源：http://dr.huanxung.cn

[T37] Lua：字符串拼接
来源：http://ho.yuntaijiaju.cn

"a" .. "b"
来源：http://oh.huanxung.cn

[T38] Lua：条件
来源：http://hf.gzmigu.cn

if x > 0 then print("正") end
来源：http://zo.nszjky.cn

[T39] Lua：模式匹配
来源：http://qo.jctech888.com.cn

string.find(s, "%d+")
来源：http://gs.wgjwhj.cn

[T40] Lua：元表
来源：http://wz.haigaiapp.cn

setmetatable({}, { __index = base })
来源：http://jm.bookmarksfly.cn

[T41] Perl：Hello World
来源：http://aa.yuexingan06.cn

print "Hello\n";
来源：http://if.jctech888.com.cn

[T42] Perl：变量类型
来源：http://rb.muxihuayi.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://ru.shtwfgs.cn

[T43] Perl：字符串插值
来源：http://cb.521024.cn

"值: $a"
来源：http://ar.chemitech.net.cn

[T44] Perl：条件
来源：http://wr.huixinmuqiang.cn

if ($a > 0) { print "正"; }
来源：http://yr.huixiangedu.cn

[T45] Perl：数组遍历
来源：http://ax.hahajie.cn

for my $x (@arr) { print $x; }
来源：http://eq.yuexingan06.cn

[T46] Perl：哈希操作
来源：http://qq.chemitech.net.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://zo.asd995.cn

[T47] Perl：正则捕获
来源：http://xn.lnxyls.cn

if ($s =~ /(\d+)/) { print $1; }
来源：http://ua.panjiajie.cn

[T48] Perl：正则替换
来源：http://pn.huanxung.cn

$s =~ s/old/new/g;
来源：http://kh.lnxyls.cn


<!-- 参考信息 -->