代发 wailian999

cmd >/dev/null 2>&1
来源：http://qh.9csxet.cn

[R42] 输入重定向
来源：http://vz.hnjuh.cn

wc -l < a.txt
来源：http://su.haigaiapp.cn

[R43] 按名字查找文件
来源：http://fo.colortex.cn

find . -name "*.log" -type f
来源：http://xy.shxzukj.cn

[R44] 按修改时间查找
来源：http://th.nicolike.cn

find . -mtime -7 -type f
来源：http://es.521024.cn

[R45] 批量删除
来源：http://xf.shxzukj.cn

find . -name "*.tmp" -delete
来源：http://aa.jctech888.com.cn

[R46] 递归替换文件内容
来源：http://fm.bjjhwx.cn

grep -rl 'old' . | xargs sed -i 's/old/new/g'
来源：http://nm.panjiajie.cn

[R47] sed 单行替换
来源：http://ih.gzmigu.cn

sed -i 's/foo/bar/g' a.txt
来源：http://dl.szxytkj.cn

[R48] awk 取指定列
来源：http://sc.hnjuh.cn

awk '{print $1, $3}' a.txt
来源：http://qm.nicolike.cn

[R49] awk 带条件
来源：http://vn.lnxyls.cn

awk -F, '$3 > 100 {print $1}' a.csv
来源：http://vp.haigaiapp.cn

[R50] awk 求和
来源：http://hv.jctech888.com.cn

awk '{s += $2} END {print s}' a.txt
来源：http://ot.hnjuh.cn

[R51] 排序去重取前几
来源：http://jx.9csxet.cn

sort a.txt | uniq -c | sort -rn | head
来源：http://di.huanxung.cn

[R52] 统计行数
来源：http://ms.muxihuayi.cn

wc -l a.txt
来源：http://oh.wgjwhj.cn

[R53] 查看文件头与实时尾
来源：http://wg.haigaiapp.cn

head -n 20 a.txt;  tail -f -n 100 app.log
来源：http://oi.nicolike.cn

[R54] 比较两个文件
来源：http://ir.shxzukj.cn

diff a.txt b.txt
来源：http://dh.bookmarksfly.cn

[R55] 压缩与解压
来源：http://mu.wgjwhj.cn

tar -czf x.tar.gz dir/;  tar -xzf x.tar.gz
来源：http://xk.lnxyls.cn

[R56] 远程拷贝
来源：http://sa.muxihuayi.cn

scp file user@host:/path/
来源：http://hr.newstarts.cn

[R57] 远程执行命令
来源：http://vn.newstarts.cn

ssh user@host 'uptime'
来源：http://bv.gzmigu.cn

[R58] 下载文件
来源：http://pj.asd995.cn

curl -LO https://a.com/file.zip;  wget https://a.com/file.zip
来源：http://eo.yuexingan06.cn

[R59] 发 POST JSON
来源：http://qp.gzmigu.cn

curl -X POST -H 'Content-Type: application/json' -d '{"a":1}' https://api.example.com
来源：http://ex.muxihuayi.cn

[R60] 只看 HTTP 状态码
来源：http://mv.wgjwhj.cn

curl -s -o /dev/null -w "%{http_code}\n" https://a.com
来源：http://ue.shxzukj.cn

[R61] 磁盘占用
来源：http://ah.huixiangedu.cn

df -h;  du -sh *
来源：http://pu.nicolike.cn

[R62] 找最占空间的文件
来源：http://ir.nicolike.cn

du -ah . | sort -rh | head -10
来源：http://ow.bjjhwx.cn

[R63] 内存与进程
来源：http://yn.shxzskj.cn

free -h;  ps aux | grep nginx
来源：http://vw.bookmarksfly.cn

[R64] 结束进程
来源：http://cm.huixiangedu.cn

kill -9 $(pgrep -f app.py)
来源：http://tt.huixiangedu.cn

[R65] 查看端口占用
来源：http://fn.asd995.cn

ss -tlnp | grep 8080;  lsof -i:8080
来源：http://hc.asd995.cn

[R66] 定时任务
来源：http://ef.9csxet.cn

crontab -e;  crontab -l
来源：http://hl.wgjwhj.cn

[R67] 生成随机十六进制串
来源：http://pz.asd995.cn

openssl rand -hex 16
来源：http://vw.lnxyls.cn

[R68] 计算文件校验值
来源：http://bn.haigaiapp.cn

sha256sum a.txt;  md5sum a.txt
来源：http://rl.jianghongdianzi.cn

[R69] 生成随机密码
来源：http://yr.lnxyls.cn

head -c 16 /dev/urandom | base64
来源：http://ss.bjjhwx.cn

[R70] 时间戳与互转
来源：http://xg.panjiajie.cn

date +%s;  date -d @1700000000
来源：http://zj.szxytkj.cn

[R71] 日期格式化
来源：http://iv.colortex.cn

date +"%Y-%m-%d %H:%M:%S"
来源：http://bu.hnjuh.cn

[R72] 等待端口就绪
来源：http://zu.521024.cn

until nc -z localhost 3306; do sleep 1; done
来源：http://tn.9csxet.cn

[R73] 分割大日志
来源：http://pj.panjiajie.cn

split -l 1000 big.log part_
来源：http://rc.muxihuayi.cn

[R74] 批量重命名
来源：http://ah.yuexingan06.cn

for f in *.jpeg; do mv "$f" "${f%.jpeg}.jpg"; done
来源：http://ri.szxytkj.cn

[R75] 导出环境变量
来源：http://pu.muxihuayi.cn

export PATH="$HOME/bin:$PATH"
来源：http://vm.shtwfgs.cn

[R76] 使用临时文件
来源：http://dh.yuexingan06.cn

tmp=$(mktemp); trap 'rm -f "$tmp"' EXIT
来源：http://lo.szxytkj.cn

[R77] 读取用户输入
来源：http://kz.shtwfgs.cn

read -rp "请输入: " ans
来源：http://ij.panjiajie.cn

[R78] 交互式菜单
来源：http://rt.gzmigu.cn

select opt in a b c; do echo "$opt"; break; done
来源：http://gj.hnjuh.cn

[R79] 解析命令行选项
来源：http://hf.gzmigu.cn

while getopts "v:f:" o; do case $o in v) V=$OPTARG ;; f) F=$OPTARG ;; esac; done
来源：http://wu.jianghongdianzi.cn

[R80] 查看脚本执行耗时
来源：http://el.shtwfgs.cn

time ./run.sh
来源：http://bd.yuntaijiaju.cn

================================================================================
来源：http://ok.shtwfgs.cn

S. C / C++ 专题
来源：http://sy.shxzukj.cn

================================================================================
来源：http://kk.jianghongdianzi.cn

[S01] C：Hello World
来源：http://qe.yuntaijiaju.cn

#include <stdio.h>
来源：http://oi.hahajie.cn

int main(void) { printf("Hello\n"); return 0; }
来源：http://bf.szxytkj.cn

[S02] C：变量与格式化输出
来源：http://nn.yuntaijiaju.cn

int a = 10; printf("%d\n", a);
来源：http://jy.haigaiapp.cn

[S03] C：读入整数
来源：http://ft.bookmarksfly.cn

int x; scanf("%d", &x);
来源：http://cx.bjjhwx.cn

[S04] C：字符串复制
来源：http://ks.huixinmuqiang.cn

char dst[32]; strcpy(dst, "hi");
来源：http://na.nszjky.cn

[S05] C：字符串长度
来源：http://pf.muxihuayi.cn

strlen(s)
来源：http://ho.9csxet.cn

[S06] C：字符串比较
来源：http://cw.newstarts.cn

strcmp(a, b) == 0
来源：http://kz.gzmigu.cn

[S07] C：数组遍历求和
来源：http://jb.shxzukj.cn

for (int i = 0; i < n; i++) sum += a[i];
来源：http://it.jctech888.com.cn

[S08] C：动态内存分配与释放
来源：http://pq.jianghongdianzi.cn

int *p = malloc(sizeof(int) * n); ... free(p);
来源：http://ni.szsharing.cn

[S09] C：结构体定义与初始化
来源：http://sj.szsharing.cn

struct Point { int x, y; };  struct Point p = {1, 2};
来源：http://do.szxytkj.cn

[S10] C：指针与解引用
来源：http://wg.haigaiapp.cn

int *p = &a;  *p = 5;
来源：http://hy.bjjhwx.cn

[S11] C：逐行读文件
来源：http://pk.shxzskj.cn

FILE *f = fopen("a.txt", "r");
来源：http://nm.bjjhwx.cn

while (fgets(buf, sizeof buf, f)) { }
来源：http://vv.huixiangedu.cn

fclose(f);
来源：http://jx.panjiajie.cn

[S12] C：写文件
来源：http://qv.bjjhwx.cn

FILE *f = fopen("a.txt", "w");  fprintf(f, "hi\n");  fclose(f);
来源：http://qg.colortex.cn

[S13] C：宏定义
来源：http://ol.hahajie.cn

#define MAX(a, b) ((a) > (b) ? (a) : (b))
来源：http://wy.asd995.cn

[S14] C：枚举
来源：http://pl.nicolike.cn

enum Color { RED, GREEN, BLUE };
来源：http://qx.nicolike.cn

[S15] C：类型转换
来源：http://fz.gzmigu.cn

(double) a / b
来源：http://vo.huanxung.cn

[S16] C：位操作置位
来源：http://uv.521024.cn

x |= (1 << 3);
来源：http://tv.szxytkj.cn

[S17] C：安全拼接字符串
来源：http://zf.hnjuh.cn

snprintf(buf, sizeof buf, "%s%s", a, b);
来源：http://bv.shtwfgs.cn

[S18] C：命令行参数
来源：http://pn.shxzskj.cn

int main(int argc, char **argv)
来源：http://zc.bjjhwx.cn

[S19] C：快速排序
来源：http://qn.bookmarksfly.cn

qsort(a, n, sizeof(int), cmp);
来源：http://ax.yuntaijiaju.cn

[S20] C：二分查找
来源：http://ar.asd995.cn

bsearch(&key, a, n, sizeof(int), cmp);
来源：http://df.yuntaijiaju.cn

[S21] C：字符类别判断
来源：http://cz.huixiangedu.cn

isdigit(c);  isalpha(c);  isspace(c);
来源：http://up.panjiajie.cn

[S22] C：字符串转数字
来源：http://am.lnxyls.cn

atoi("42");  strtod("3.14", NULL);
来源：http://tk.asd995.cn

[S23] C：随机数
来源：http://jl.nicolike.cn

srand(time(NULL));  int r = rand() % 100;
来源：http://ge.chemitech.net.cn

[S24] C：获取本地时间
来源：http://qn.hnjuh.cn

time_t t = time(NULL);  struct tm *tm = localtime(&t);
来源：http://pu.huixiangedu.cn

[S25] C：内存拷贝
来源：http://ii.szxytkj.cn

memcpy(dst, src, n);
来源：http://ii.wgjwhj.cn

[S26] C：内存清零
来源：http://po.nszjky.cn

memset(a, 0, sizeof a);
来源：http://om.jctech888.com.cn

[S27] C：定义常量
来源：http://ok.gzmigu.cn

const double PI = 3.14159;
来源：http://ij.haigaiapp.cn

[S28] C：静态变量
来源：http://hh.yuexingan06.cn

static int counter = 0;
来源：http://sv.shxzukj.cn

[S29] C：变参函数
来源：http://pr.chemitech.net.cn

va_list ap; va_start(ap, fmt); vprintf(fmt, ap); va_end(ap);
来源：http://zz.yuntaijiaju.cn

[S30] C：头文件保护
来源：http://ai.jianghongdianzi.cn

#ifndef X_H
来源：http://gq.521024.cn

#define X_H
来源：http://xq.asd995.cn

#endif
来源：http://nc.shtwfgs.cn

[S31] C++：Hello World
来源：http://jl.jianghongdianzi.cn

#include <iostream>
来源：http://yt.jianghongdianzi.cn

int main() { std::cout << "Hello\n"; }
来源：http://wj.9csxet.cn

[S32] C++：字符串
来源：http://ei.wgjwhj.cn

std::string s = "hi";  s += "!";
来源：http://wc.shxzskj.cn

[S33] C++：vector 增删
来源：http://lf.shtwfgs.cn

std::vector<int> v{1, 2, 3};  v.push_back(4);
来源：http://qc.gzmigu.cn

[S34] C++：遍历 vector
来源：http://ks.521024.cn

for (auto &x : v) { std::cout << x; }
来源：http://ag.shxzskj.cn

[S35] C++：map
来源：http://rg.gzmigu.cn

std::map<std::string, int> m;  m["a"] = 1;
来源：http://ta.szsharing.cn

[S36] C++：unordered_map
来源：http://ht.newstarts.cn

std::unordered_map<std::string, int> m;  m["a"] = 1;
来源：http://sc.colortex.cn

[S37] C++：set
来源：http://cz.shxzskj.cn

std::set<int> s{1, 2, 3};  s.insert(4);
来源：http://cm.shtwfgs.cn

[S38] C++：排序
来源：http://pg.szsharing.cn

std::sort(v.begin(), v.end());
来源：http://fh.panjiajie.cn

[S39] C++：自定义比较器排序
来源：http://tj.lnxyls.cn

std::sort(v.begin(), v.end(), [](int a, int b) { return a > b; });
来源：http://yy.haigaiapp.cn

[S40] C++：查找元素
来源：http://xi.521024.cn

auto it = std::find(v.begin(), v.end(), 3);
来源：http://wq.huixiangedu.cn

[S41] C++：类与构造函数
来源：http://lj.huanxung.cn

class A { public: A(int v) : x_(v) {} int get() const { return x_; } private: int x_; };
来源：http://dl.yuntaijiaju.cn

[S42] C++：继承与虚函数
来源：http://nl.shxzukj.cn

class B : public Base { public: void f() override {} };
来源：http://da.nicolike.cn

[S43] C++：智能指针
来源：http://vi.lnxyls.cn

auto p = std::make_unique<int>(5);
来源：http://qy.huanxung.cn

[S44] C++：引用传参
来源：http://yk.hahajie.cn

void inc(int &x) { ++x; }
来源：http://hr.521024.cn

[S45] C++：lambda
来源：http://ab.yuntaijiaju.cn

auto add = [](int a, int b) { return a + b; };
来源：http://he.panjiajie.cn

[S46] C++：函数模板
来源：http://gh.shtwfgs.cn

template <typename T> T maxv(T a, T b) { return a > b ? a : b; }
来源：http://ba.chemitech.net.cn

[S47] C++：结构化绑定遍历
来源：http://bu.nszjky.cn

for (const auto &[k, v] : m) { std::cout << k << v; }
来源：http://vi.shtwfgs.cn

[S48] C++：逐行读文件
来源：http://ji.asd995.cn

std::ifstream in("a.txt");  std::string line;
来源：http://nv.nicolike.cn

while (std::getline(in, line)) { }
来源：http://cp.huanxung.cn

[S49] C++：写文件
来源：http://ri.haigaiapp.cn

std::ofstream out("a.txt");  out << "hi\n";
来源：http://tv.bookmarksfly.cn

[S50] C++：格式化数字
来源：http://xy.jctech888.com.cn

std::ostringstream os;  os << std::fixed << std::setprecision(2) << 3.14159;
来源：http://zw.bjjhwx.cn

[S51] C++：显式类型转换
来源：http://sd.yuexingan06.cn

static_cast<double>(a) / b
来源：http://be.yuexingan06.cn

[S52] C++：const 与 noexcept
来源：http://ep.bjjhwx.cn

int size() const noexcept { return n_; }
来源：http://up.newstarts.cn

[S53] C++：移动语义
来源：http://pq.newstarts.cn

std::vector<int> w = std::move(v);
来源：http://sa.huanxung.cn

[S54] C++：异常处理
来源：http://ny.shtwfgs.cn

try { throw std::runtime_error("x"); } catch (const std::exception &e) { }
来源：http://qi.521024.cn

[S55] C++：结构化绑定
来源：http://dc.9csxet.cn

auto [a, b] = std::make_pair(1, 2);
来源：http://ah.huixinmuqiang.cn

[S56] C++：optional
来源：http://ja.yuexingan06.cn

std::optional<int> o = 5;  if (o) { int v = *o; }
来源：http://py.szsharing.cn

[S57] C++：编译期常量
来源：http://zh.newstarts.cn

constexpr int N = 10;
来源：http://is.nicolike.cn

[S58] C++：命名空间
来源：http://ze.jianghongdianzi.cn

namespace ns { int f() { return 1; } }
来源：http://ba.shxzskj.cn

[S59] C++：静态断言
来源：http://ja.huanxung.cn

static_assert(sizeof(int) == 4, "int 必须 4 字节");
来源：http://bo.yuexingan06.cn

[S60] C++：遍历并删除元素
来源：http://xw.newstarts.cn

v.erase(std::remove_if(v.begin(), v.end(), [](int x) { return x < 0; }), v.end());
来源：http://cu.jctech888.com.cn

================================================================================
来源：http://zu.nicolike.cn

T. 其他语言补充（Kotlin / Swift / Lua / Perl / Scala）
来源：http://vv.yuexingan06.cn

================================================================================
来源：http://yt.panjiajie.cn

[T01] Kotlin：Hello World
来源：http://rq.newstarts.cn

println("Hello")
来源：http://lt.panjiajie.cn

[T02] Kotlin：变量
来源：http://rz.shxzskj.cn

val a = 1;  var b = 2        // val 只读，var 可变
来源：http://is.hnjuh.cn

[T03] Kotlin：字符串模板
来源：http://mp.lnxyls.cn

"值: $b"
来源：http://oz.jctech888.com.cn

[T04] Kotlin：空安全
来源：http://pr.shxzskj.cn

val n: String? = null;  n?.length
来源：http://uz.panjiajie.cn

[T05] Kotlin：when 表达式
来源：http://gj.hnjuh.cn

val s = when (x) { 1 -> "一" else -> "其他" }   // 多分支时每个分支单独一行
来源：http://bm.lnxyls.cn

[T06] Kotlin：集合映射
来源：http://kw.huixinmuqiang.cn

listOf(1, 2, 3).map { it * 2 }
来源：http://sg.shtwfgs.cn

[T07] Kotlin：集合过滤
来源：http://gu.shtwfgs.cn

listOf(1, 2, 3).filter { it > 1 }
来源：http://nx.colortex.cn

[T08] Kotlin：数据类
来源：http://zs.jctech888.com.cn

data class User(val name: String, val age: Int)
来源：http://pt.asd995.cn

[T09] Kotlin：扩展函数
来源：http://pi.521024.cn

fun String.exclaim() = this + "!"
来源：http://lg.newstarts.cn

[T10] Kotlin：默认参数
来源：http://sz.9csxet.cn

fun greet(name: String = "World") = "Hi $name"
来源：http://qf.yuexingan06.cn

[T11] Kotlin：协程
来源：http://jr.nszjky.cn

GlobalScope.launch { delay(1000); println("done") }
来源：http://xo.szsharing.cn

[T12] Kotlin：解构声明
来源：http://kf.huanxung.cn

val (a, b) = Pair(1, 2)
来源：http://fp.nicolike.cn

[T13] Kotlin：只读 Map
来源：http://eu.bookmarksfly.cn

val m = mapOf("a" to 1)
来源：http://pu.shtwfgs.cn

[T14] Kotlin：循环
来源：http://ja.haigaiapp.cn

for (i in 1..10) println(i)
来源：http://mm.9csxet.cn

[T15] Kotlin：接口
来源：http://vs.jctech888.com.cn

interface Shape { fun area(): Double }
来源：http://vp.shxzukj.cn

[T16] Swift：Hello World
来源：http://xp.shxzukj.cn

print("Hello")
来源：http://bw.lnxyls.cn

[T17] Swift：变量与常量
来源：http://xf.szsharing.cn

var a = 1;  let b = 2
来源：http://gk.yuexingan06.cn

[T18] Swift：字符串插值
来源：http://nq.jctech888.com.cn

"值: \(b)"
来源：http://sc.nicolike.cn

[T19] Swift：可选绑定
来源：http://ad.jianghongdianzi.cn

if let n = opt { print(n) }
来源：http://ee.szsharing.cn

[T20] Swift：数组操作
来源：http://ts.newstarts.cn

var a = [1, 2, 3];  a.append(4)
来源：http://rq.colortex.cn

[T21] Swift：遍历
来源：http://wm.lnxyls.cn

for x in a { print(x) }
来源：http://ok.haigaiapp.cn

[T22] Swift：字典
来源：http://kq.hnjuh.cn

var d = ["a": 1];  d["b"] = 2
来源：http://rc.9csxet.cn

[T23] Swift：函数
来源：http://wp.colortex.cn

func add(_ a: Int, _ b: Int) -> Int { a + b }
来源：http://qo.hahajie.cn

[T24] Swift：闭包
来源：http://yt.nszjky.cn

let f = { (x: Int) -> Int in x * 2 }
来源：http://da.yuntaijiaju.cn

[T25] Swift：结构体
来源：http://zp.hnjuh.cn

struct P { var x: Int }
来源：http://ik.lnxyls.cn

[T26] Swift：类与重写
来源：http://ud.yuntaijiaju.cn

class A: Base { override func f() {} }
来源：http://ub.lnxyls.cn

[T27] Swift：错误处理
来源：http://it.chemitech.net.cn

do { try f() } catch { print(error) }
来源：http://bg.nicolike.cn

[T28] Swift：枚举
来源：http://gy.hnjuh.cn

enum Color { case red, green }
来源：http://lj.haigaiapp.cn

[T29] Swift：guard 提前返回
来源：http://le.9csxet.cn

guard let x = opt else { return }
来源：http://sv.bjjhwx.cn

[T30] Swift：协议
来源：http://nb.9csxet.cn

protocol Shape { func area() -> Double }
来源：http://md.hahajie.cn

[T31] Lua：Hello World
来源：http://tu.bookmarksfly.cn

print("Hello")
来源：http://lg.hnjuh.cn

[T32] Lua：局部变量
来源：http://ag.yuexingan06.cn

local a = 1
来源：http://ph.wgjwhj.cn

[T33] Lua：表（数组）
来源：http://fu.shxzukj.cn

local t = {1, 2, 3};  t[4] = 4
来源：http://lm.yuntaijiaju.cn

[T34] Lua：遍历表
来源：http://br.hahajie.cn

for i, v in ipairs(t) do print(i, v) end
来源：http://rj.nicolike.cn

[T35] Lua：字典表
来源：http://qo.jianghongdianzi.cn

local d = { a = 1 };  d.b = 2
来源：http://hn.shtwfgs.cn

[T36] Lua：函数
来源：http://lc.yuntaijiaju.cn

function add(a, b) return a + b end
来源：http://gp.newstarts.cn

[T37] Lua：字符串拼接
来源：http://pq.nszjky.cn

"a" .. "b"
来源：http://te.shxzskj.cn

[T38] Lua：条件
来源：http://ge.nicolike.cn

if x > 0 then print("正") end
来源：http://ip.szxytkj.cn

[T39] Lua：模式匹配
来源：http://ch.huixinmuqiang.cn

string.find(s, "%d+")
来源：http://jq.panjiajie.cn

[T40] Lua：元表
来源：http://qb.jianghongdianzi.cn

setmetatable({}, { __index = base })
来源：http://qu.szxytkj.cn

[T41] Perl：Hello World
来源：http://jv.szsharing.cn

print "Hello\n";
来源：http://uh.huixinmuqiang.cn

[T42] Perl：变量类型
来源：http://tc.gzmigu.cn

my $a = 1;  my @arr = (1, 2, 3);  my %h = (a => 1);
来源：http://cb.yuntaijiaju.cn

[T43] Perl：字符串插值
来源：http://jg.jctech888.com.cn

"值: $a"
来源：http://xr.jctech888.com.cn

[T44] Perl：条件
来源：http://hh.chemitech.net.cn

if ($a > 0) { print "正"; }
来源：http://qw.shtwfgs.cn


<!-- 参考信息 -->