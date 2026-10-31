代发 wailian999

find . -name "*.log" -type f
来源：http://tp.nicolike.cn

[R44] 按修改时间查找
来源：http://rl.asd995.cn

find . -mtime -7 -type f
来源：http://wh.haigaiapp.cn

[R45] 批量删除
来源：http://gm.jctech888.com.cn

find . -name "*.tmp" -delete
来源：http://od.yuntaijiaju.cn

[R46] 递归替换文件内容
来源：http://pu.haigaiapp.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://qg.lnxyls.cn

[R47] sed 单行替换
来源：http://oj.lnxyls.cn

sed -i 's/foo/bar/g' a.txt
来源：http://yb.colortex.cn

[R48] awk 取指定列
来源：http://ca.hnjuh.cn

awk '{print $1, $3}' a.txt
来源：http://wl.hahajie.cn

[R49] awk 带条件
来源：http://ur.yuntaijiaju.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://jc.panjiajie.cn

[R50] awk 求和
来源：http://uh.wgjwhj.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ba.asd995.cn

[R51] 排序去重取前几
来源：http://si.asd995.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://xw.newstarts.cn

[R52] 统计行数
来源：http://ue.szxytkj.cn

wc -l a.txt
来源：http://wv.panjiajie.cn

[R53] 查看文件头与实时尾
来源：http://ce.asd995.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://ja.asd995.cn

[R54] 比较两个文件
来源：http://di.szxytkj.cn

diff a.txt b.txt
来源：http://cq.hahajie.cn

[R55] 压缩与解压
来源：http://fu.chemitech.net.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://yc.shxzskj.cn

[R56] 远程拷贝
来源：http://dz.shxzskj.cn

scp file user@host:/path/
来源：http://yo.hnjuh.cn

[R57] 远程执行命令
来源：http://uu.huixiangedu.cn

ssh user@host 'uptime'
来源：http://rf.asd995.cn

[R58] 下载文件
来源：http://ux.huixinmuqiang.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://jg.yuntaijiaju.cn

[R59] 发 POST JSON
来源：http://it.bjjhwx.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://bs.szsharing.cn

[R60] 只看 HTTP 状态码
来源：http://av.nicolike.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://pg.asd995.cn

[R61] 磁盘占用
来源：http://fk.jianghongdianzi.cn

df -h;  du -sh *
来源：http://qo.yuexingan06.cn

[R62] 找最占空间的文件
来源：http://mr.521024.cn

du -ah . | sort -rh | head -10
来源：http://ds.szxytkj.cn

[R63] 内存与进程
来源：http://xu.hnjuh.cn

free -h;  ps aux | grep nginx
来源：http://qs.521024.cn

[R64] 结束进程
来源：http://vb.colortex.cn

kill -9 $(pgrep -f app.py)
来源：http://lm.shtwfgs.cn

[R65] 查看端口占用
来源：http://xp.colortex.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://xe.shxzskj.cn

[R66] 定时任务
来源：http://tn.wgjwhj.cn

crontab -e;  crontab -l
来源：http://oe.jianghongdianzi.cn

[R67] 生成随机十六进制串
来源：http://gq.gzmigu.cn

openssl rand -hex 16
来源：http://wj.lnxyls.cn

[R68] 计算文件校验值
来源：http://ye.9csxet.cn

sha256sum a.txt;  md5sum a.txt
来源：http://is.bjjhwx.cn

[R69] 生成随机密码
来源：http://hj.szsharing.cn

head -c 16 /dev/urandom | base64
来源：http://ns.yuexingan06.cn

[R70] 时间戳与互转
来源：http://ir.wgjwhj.cn

date +%s;  date -d @1700000000
来源：http://nj.nszjky.cn

[R71] 日期格式化
来源：http://us.chemitech.net.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://cq.521024.cn

[R72] 等待端口就绪
来源：http://he.nszjky.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://ja.hnjuh.cn

[R73] 分割大日志
来源：http://ff.newstarts.cn

split -l 1000 big.log part_
来源：http://pd.huixiangedu.cn

[R74] 批量重命名
来源：http://fu.colortex.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://mc.gzmigu.cn

[R75] 导出环境变量
来源：http://ve.9csxet.cn

export PATH="$HOME/bin:$PATH"
来源：http://xk.lnxyls.cn

[R76] 使用临时文件
来源：http://du.haigaiapp.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://en.newstarts.cn

[R77] 读取用户输入
来源：http://vx.huixinmuqiang.cn

read -rp "请输入: " ans
来源：http://ff.bookmarksfly.cn

[R78] 交互式菜单
来源：http://mj.shxzskj.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://xt.colortex.cn

[R79] 解析命令行选项
来源：http://vi.521024.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://vk.hahajie.cn

[R80] 查看脚本执行耗时
来源：http://wr.asd995.cn

time ./run.sh
来源：http://sf.lnxyls.cn

================================================================================
来源：http://hc.wgjwhj.cn

S. C / C++ 专题
来源：http://zd.gzmigu.cn

================================================================================
来源：http://sb.bookmarksfly.cn

[S01] C：Hello World
来源：http://zk.yuexingan06.cn

#include <stdio.h>
来源：http://yz.bjjhwx.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://nk.shxzukj.cn

[S02] C：变量与格式化输出
来源：http://ul.muxihuayi.cn

int a = 10; printf("%d\n", a);
来源：http://in.bjjhwx.cn

[S03] C：读入整数
来源：http://mx.chemitech.net.cn

int x; scanf("%d", &x);
来源：http://hp.panjiajie.cn

[S04] C：字符串复制
来源：http://tn.bookmarksfly.cn

char dst[32]; strcpy(dst, "hi");
来源：http://wk.yuntaijiaju.cn

[S05] C：字符串长度
来源：http://ub.huanxung.cn

strlen(s)
来源：http://cx.shxzskj.cn

[S06] C：字符串比较
来源：http://my.shtwfgs.cn

strcmp(a, b) == 0
来源：http://ct.nicolike.cn

[S07] C：数组遍历求和
来源：http://jp.9csxet.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://pk.huanxung.cn

[S08] C：动态内存分配与释放
来源：http://fy.huanxung.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://pr.huixinmuqiang.cn

[S09] C：结构体定义与初始化
来源：http://bw.yuexingan06.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://xm.shxzukj.cn

[S10] C：指针与解引用
来源：http://kl.bookmarksfly.cn

int *p = &a;  *p = 5;
来源：http://ld.panjiajie.cn

[S11] C：逐行读文件
来源：http://bd.nicolike.cn

FILE *f = fopen("a.txt", "r");
来源：http://xh.shtwfgs.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://ni.shtwfgs.cn

fclose(f);
来源：http://cl.muxihuayi.cn

[S12] C：写文件
来源：http://zx.asd995.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://pc.bookmarksfly.cn

[S13] C：宏定义
来源：http://ab.colortex.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://fg.asd995.cn

[S14] C：枚举
来源：http://da.nicolike.cn

enum Color { RED, GREEN, BLUE };
来源：http://hx.yuntaijiaju.cn

[S15] C：类型转换
来源：http://jt.jianghongdianzi.cn

(double) a / b
来源：http://ju.haigaiapp.cn

[S16] C：位操作置位
来源：http://gw.yuexingan06.cn

x |= (1 << 3);
来源：http://pl.hahajie.cn

[S17] C：安全拼接字符串
来源：http://ms.newstarts.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://ai.newstarts.cn

[S18] C：命令行参数
来源：http://zh.huixinmuqiang.cn

int main(int argc, char **argv)
来源：http://sj.bookmarksfly.cn

[S19] C：快速排序
来源：http://ho.yuexingan06.cn

qsort(a, n, sizeof(int), cmp);
来源：http://jr.gzmigu.cn

[S20] C：二分查找
来源：http://dq.yuntaijiaju.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://ln.hahajie.cn

[S21] C：字符类别判断
来源：http://gj.9csxet.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://fh.muxihuayi.cn

[S22] C：字符串转数字
来源：http://lj.hnjuh.cn

atoi("42");  strtod("3.14", NULL);
来源：http://rh.jctech888.com.cn

[S23] C：随机数
来源：http://ho.wgjwhj.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ex.jianghongdianzi.cn

[S24] C：获取本地时间
来源：http://ti.shxzskj.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://es.shxzukj.cn

[S25] C：内存拷贝
来源：http://hg.jianghongdianzi.cn

memcpy(dst, src, n);
来源：http://rg.shtwfgs.cn

[S26] C：内存清零
来源：http://od.panjiajie.cn

memset(a, 0, sizeof a);
来源：http://kj.lnxyls.cn

[S27] C：定义常量
来源：http://mi.newstarts.cn

const double PI = 3.14159;
来源：http://aw.shxzukj.cn

[S28] C：静态变量
来源：http://rg.shtwfgs.cn

static int counter = 0;
来源：http://hd.panjiajie.cn

[S29] C：变参函数
来源：http://da.szsharing.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://ur.yuntaijiaju.cn

[S30] C：头文件保护
来源：http://vt.huixiangedu.cn

#ifndef X_H
来源：http://wm.bookmarksfly.cn

#define X_H
来源：http://io.hnjuh.cn

#endif
来源：http://cr.panjiajie.cn

[S31] C++：Hello World
来源：http://fk.gzmigu.cn

#include <iostream>
来源：http://vv.asd995.cn

int main() { std::cout << "Hello\n"; }
来源：http://fm.521024.cn

[S32] C++：字符串
来源：http://hi.huixinmuqiang.cn

std::string s = "hi";  s += "!";
来源：http://wl.muxihuayi.cn

[S33] C++：vector 增删
来源：http://ne.nicolike.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://lp.asd995.cn

[S34] C++：遍历 vector
来源：http://vc.wgjwhj.cn

for (auto &x : v) { std::cout << x; }
来源：http://dn.shxzskj.cn

[S35] C++：map
来源：http://ki.chemitech.net.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://dw.huanxung.cn

[S36] C++：unordered_map
来源：http://vt.wgjwhj.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://zn.bookmarksfly.cn

[S37] C++：set
来源：http://fg.huixiangedu.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://uw.chemitech.net.cn

[S38] C++：排序
来源：http://fp.asd995.cn

std::sort(v.begin(), v.end());
来源：http://cb.hahajie.cn

[S39] C++：自定义比较器排序
来源：http://ph.yuntaijiaju.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://ek.huixiangedu.cn

[S40] C++：查找元素
来源：http://rg.szsharing.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://af.lnxyls.cn

[S41] C++：类与构造函数
来源：http://ac.jianghongdianzi.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://zn.gzmigu.cn

[S42] C++：继承与虚函数
来源：http://yo.hnjuh.cn

class B : public Base { public: void f() override {} };
来源：http://ne.hnjuh.cn

[S43] C++：智能指针
来源：http://qt.huixiangedu.cn

auto p = std::make_unique<int>(5);
来源：http://ne.shtwfgs.cn

[S44] C++：引用传参
来源：http://dw.yuexingan06.cn

void inc(int &x) { ++x; }
来源：http://rv.szsharing.cn

[S45] C++：lambda
来源：http://uf.szsharing.cn

auto add = [](int a, int b) { return a + b; };
来源：http://ax.szxytkj.cn

[S46] C++：函数模板
来源：http://mj.wgjwhj.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://tq.hahajie.cn

[S47] C++：结构化绑定遍历
来源：http://tx.shxzukj.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://je.bookmarksfly.cn

[S48] C++：逐行读文件
来源：http://oi.huixiangedu.cn

std::ifstream in("a.txt");  std::string line;
来源：http://mn.shxzukj.cn

while (std::getline(in, line)) { }
来源：http://nu.haigaiapp.cn

[S49] C++：写文件
来源：http://of.szsharing.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://ak.gzmigu.cn

[S50] C++：格式化数字
来源：http://nt.szsharing.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://lp.521024.cn

[S51] C++：显式类型转换
来源：http://eu.szxytkj.cn

static_cast<double>(a) / b
来源：http://ot.nszjky.cn

[S52] C++：const 与 noexcept
来源：http://tb.chemitech.net.cn

int size() const noexcept { return n_; }
来源：http://nw.huanxung.cn

[S53] C++：移动语义
来源：http://zj.shtwfgs.cn

std::vector<int> w = std::move(v);
来源：http://wa.huixiangedu.cn

[S54] C++：异常处理
来源：http://ii.szsharing.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://eh.huixiangedu.cn

[S55] C++：结构化绑定
来源：http://ft.szxytkj.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://kl.muxihuayi.cn

[S56] C++：optional
来源：http://yc.wgjwhj.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://ny.hahajie.cn

[S57] C++：编译期常量
来源：http://rb.hnjuh.cn

constexpr int N = 10;
来源：http://sg.gzmigu.cn

[S58] C++：命名空间
来源：http://fp.hnjuh.cn

namespace ns { int f() { return 1; } }
来源：http://eo.jctech888.com.cn

[S59] C++：静态断言
来源：http://jp.huanxung.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://ca.haigaiapp.cn

[S60] C++：遍历并删除元素
来源：http://fq.szxytkj.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://er.jctech888.com.cn

================================================================================
来源：http://rr.shxzskj.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://su.yuexingan06.cn

================================================================================
来源：http://ck.bookmarksfly.cn

[T01] Kotlin：Hello World
来源：http://jq.szxytkj.cn

println("Hello")
来源：http://hj.hahajie.cn

[T02] Kotlin：变量
来源：http://kr.yuexingan06.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://iq.jianghongdianzi.cn

[T03] Kotlin：字符串模板
来源：http://ql.lnxyls.cn

"值: $b"
来源：http://kv.shtwfgs.cn

[T04] Kotlin：空安全
来源：http://ya.szxytkj.cn

val n: String? = null;  n?.length
来源：http://to.gzmigu.cn

[T05] Kotlin：when 表达式
来源：http://kf.gzmigu.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://xe.huixiangedu.cn

[T06] Kotlin：集合映射
来源：http://of.yuexingan06.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://xg.haigaiapp.cn

[T07] Kotlin：集合过滤
来源：http://vu.bookmarksfly.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://hk.jianghongdianzi.cn

[T08] Kotlin：数据类
来源：http://ng.bookmarksfly.cn

data class User(val name: String, val age: Int)
来源：http://fj.huanxung.cn

[T09] Kotlin：扩展函数
来源：http://lj.jianghongdianzi.cn

fun String.exclaim() = this + "!"
来源：http://qi.haigaiapp.cn

[T10] Kotlin：默认参数
来源：http://ns.nszjky.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://qo.hahajie.cn

[T11] Kotlin：协程
来源：http://gv.gzmigu.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://ci.nszjky.cn

[T12] Kotlin：解构声明
来源：http://zf.huixiangedu.cn

val (a, b) = Pair(1, 2)
来源：http://sj.szxytkj.cn

[T13] Kotlin：只读 Map
来源：http://ky.yuntaijiaju.cn

val m = mapOf("a" to 1)
来源：http://is.nszjky.cn

[T14] Kotlin：循环
来源：http://ye.szsharing.cn

for (i in 1..10) println(i)
来源：http://wg.lnxyls.cn

[T15] Kotlin：接口
来源：http://az.muxihuayi.cn

interface Shape { fun area(): Double }
来源：http://on.huanxung.cn

[T16] Swift：Hello World
来源：http://wt.bjjhwx.cn

print("Hello")
来源：http://bb.hnjuh.cn

[T17] Swift：变量与常量
来源：http://zf.521024.cn

var a = 1;  let b = 2
来源：http://ar.szsharing.cn

[T18] Swift：字符串插值
来源：http://ou.huixiangedu.cn

"值: \(b)"
来源：http://tf.szxytkj.cn

[T19] Swift：可选绑定
来源：http://ix.yuexingan06.cn

if let n = opt { print(n) }
来源：http://xq.szxytkj.cn

[T20] Swift：数组操作
来源：http://tm.shtwfgs.cn

var a = [1, 2, 3];  a.append(4)
来源：http://cp.muxihuayi.cn

[T21] Swift：遍历
来源：http://js.huanxung.cn

for x in a { print(x) }
来源：http://mn.nicolike.cn

[T22] Swift：字典
来源：http://yu.wgjwhj.cn

var d = ["a": 1];  d["b"] = 2
来源：http://zp.jianghongdianzi.cn

[T23] Swift：函数
来源：http://ut.jianghongdianzi.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://mz.szxytkj.cn

[T24] Swift：闭包
来源：http://cf.szsharing.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://dp.haigaiapp.cn

[T25] Swift：结构体
来源：http://ne.hnjuh.cn

struct P { var x: Int }
来源：http://ob.shxzukj.cn

[T26] Swift：类与重写
来源：http://te.nszjky.cn

class A: Base { override func f() {} }
来源：http://xn.521024.cn

[T27] Swift：错误处理
来源：http://kl.szsharing.cn

do { try f() } catch { print(error) }
来源：http://kp.newstarts.cn

[T28] Swift：枚举
来源：http://cy.chemitech.net.cn

enum Color { case red, green }
来源：http://fv.521024.cn

[T29] Swift：guard 提前返回
来源：http://md.szxytkj.cn

guard let x = opt else { return }
来源：http://ab.lnxyls.cn

[T30] Swift：协议
来源：http://jm.newstarts.cn

protocol Shape { func area() -> Double }
来源：http://ku.gzmigu.cn

[T31] Lua：Hello World
来源：http://ze.jianghongdianzi.cn

print("Hello")
来源：http://cc.wgjwhj.cn

[T32] Lua：局部变量
来源：http://qb.shtwfgs.cn

local a = 1
来源：http://xm.nicolike.cn

[T33] Lua：表（数组）
来源：http://xq.huixiangedu.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://hi.yuntaijiaju.cn

[T34] Lua：遍历表
来源：http://gl.newstarts.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://ip.521024.cn

[T35] Lua：字典表
来源：http://mv.wgjwhj.cn

local d = { a = 1 };  d.b = 2
来源：http://lx.wgjwhj.cn

[T36] Lua：函数
来源：http://vv.hnjuh.cn

function add(a, b) return a + b end
来源：http://fp.shxzskj.cn

[T37] Lua：字符串拼接
来源：http://pr.nicolike.cn

"a" .. "b"
来源：http://sk.nszjky.cn

[T38] Lua：条件
来源：http://qq.muxihuayi.cn

if x > 0 then print("正") end
来源：http://wx.yuexingan06.cn

[T39] Lua：模式匹配
来源：http://oh.jctech888.com.cn

string.find(s, "%d+")
来源：http://fu.jctech888.com.cn

[T40] Lua：元表
来源：http://ws.gzmigu.cn

setmetatable({}, { __index = base })
来源：http://xv.newstarts.cn

[T41] Perl：Hello World
来源：http://zk.yuexingan06.cn

print "Hello\n";
来源：http://lt.huixinmuqiang.cn

[T42] Perl：变量类型
来源：http://ez.yuntaijiaju.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://tt.shxzukj.cn

[T43] Perl：字符串插值
来源：http://lu.wgjwhj.cn

"值: $a"
来源：http://zq.bookmarksfly.cn

[T44] Perl：条件
来源：http://ib.521024.cn

if ($a > 0) { print "正"; }
来源：http://mz.shxzskj.cn

[T45] Perl：数组遍历
来源：http://ey.yuntaijiaju.cn

for my $x (@arr) { print $x; }
来源：http://ps.shtwfgs.cn

[T46] Perl：哈希操作
来源：http://uj.huanxung.cn

$h{b} = 2;  for my $k (keys %h) { print "$k=$h{$k}"; }
来源：http://fy.newstarts.cn


<!-- 参考信息 -->